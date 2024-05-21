# Comparing `tmp/chemcat-0.3.8b1.tar.gz` & `tmp/chemcat-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemcat-0.3.8b1.tar", last modified: Sun Jan  7 17:43:34 2024, max compression
+gzip compressed data, was "chemcat-0.3.9.tar", last modified: Tue May 21 08:35:16 2024, max compression
```

## Comparing `chemcat-0.3.8b1.tar` & `chemcat-0.3.9.tar`

### file list

```diff
@@ -1,1861 +1,1860 @@
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.863787 chemcat-0.3.8b1/
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.458638 chemcat-0.3.8b1/.github/
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.460367 chemcat-0.3.8b1/.github/workflows/
--rw-r--r--   0 pato       (501) staff       (20)     1548 2024-01-06 15:10:52.000000 chemcat-0.3.8b1/.github/workflows/python-package.yml
--rw-r--r--   0 pato       (501) staff       (20)    18092 2022-07-07 21:33:49.000000 chemcat-0.3.8b1/LICENSE
--rw-r--r--   0 pato       (501) staff       (20)      295 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/MANIFEST.in
--rw-r--r--   0 pato       (501) staff       (20)    22694 2024-01-07 17:43:34.863421 chemcat-0.3.8b1/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1349 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/README.md
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.461220 chemcat-0.3.8b1/chemcat/
--rw-r--r--   0 pato       (501) staff       (20)      634 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/__init__.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.464787 chemcat-0.3.8b1/chemcat/cea/
--rw-r--r--   0 pato       (501) staff       (20)      474 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/cea/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    13592 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/cea/cea.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.466923 chemcat-0.3.8b1/chemcat/data/
--rw-r--r--   0 pato       (501) staff       (20)     3259 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/chemcat/data/asplund_2009_solar_abundances.dat
--rw-r--r--   0 pato       (501) staff       (20)     3688 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/chemcat/data/asplund_2021_solar_abundances.dat
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.852275 chemcat-0.3.8b1/chemcat/data/janaf/
--rw-r--r--   0 pato       (501) staff       (20)     2975 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      854 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1803 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1727 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3428 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3802 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3848 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1170 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     1051 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1225 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3891 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3841 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3990 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3809 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     4068 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1897 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3959 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3894 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     1172 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     1055 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1227 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3968 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-028.txt
--rw-r--r--   0 pato       (501) staff       (20)      739 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-029.txt
--rw-r--r--   0 pato       (501) staff       (20)      733 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1387 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     1385 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3781 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3834 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3988 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     3774 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     4100 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     4033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     2238 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     2748 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     2916 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     4101 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     4108 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     4194 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     4192 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     1631 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     2180 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     2583 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     1033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     1152 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     2219 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     2350 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     3859 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     3834 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     3841 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     3880 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     1300 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     3805 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     1058 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     1362 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     1114 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     1626 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     2742 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     2801 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     1912 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     2170 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     3637 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     3695 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     3867 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     3889 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     3686 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     3734 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     1797 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     2799 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     2861 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     4143 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     4151 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     1074 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     4205 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     4132 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     2059 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     2796 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     2864 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     3999 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-095.txt
--rw-r--r--   0 pato       (501) staff       (20)     2147 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     1967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     1968 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-098.txt
--rw-r--r--   0 pato       (501) staff       (20)     1967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-099.txt
--rw-r--r--   0 pato       (501) staff       (20)     2752 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-100.txt
--rw-r--r--   0 pato       (501) staff       (20)     2817 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-101.txt
--rw-r--r--   0 pato       (501) staff       (20)     2133 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-102.txt
--rw-r--r--   0 pato       (501) staff       (20)     2127 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-103.txt
--rw-r--r--   0 pato       (501) staff       (20)     2135 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-104.txt
--rw-r--r--   0 pato       (501) staff       (20)     1115 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-105.txt
--rw-r--r--   0 pato       (501) staff       (20)     1244 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-106.txt
--rw-r--r--   0 pato       (501) staff       (20)     2239 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-107.txt
--rw-r--r--   0 pato       (501) staff       (20)     2316 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-108.txt
--rw-r--r--   0 pato       (501) staff       (20)     2220 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-109.txt
--rw-r--r--   0 pato       (501) staff       (20)     2872 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-110.txt
--rw-r--r--   0 pato       (501) staff       (20)     2942 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-111.txt
--rw-r--r--   0 pato       (501) staff       (20)     2181 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Al-112.txt
--rw-r--r--   0 pato       (501) staff       (20)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ar-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ar-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2918 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1543 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2613 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2361 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3627 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3803 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3993 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     4014 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3994 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-018.txt
--rw-r--r--   0 pato       (501) staff       (20)      722 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3968 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3898 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     4001 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     4120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     4088 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     1211 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     1112 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     1266 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     4163 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     3939 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3882 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-048.txt
--rw-r--r--   0 pato       (501) staff       (20)      968 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     3976 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     3919 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3891 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     1121 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     4087 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     1405 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     1401 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     3839 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     3867 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     1476 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     1464 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     1529 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     3995 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     1477 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     2086 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     2155 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     2181 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     1472 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     1771 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     1836 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     3829 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     3916 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     2425 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     4162 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     2018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     4129 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     4151 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     1042 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     4113 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     4017 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     1312 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     3984 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     1171 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-095.txt
--rw-r--r--   0 pato       (501) staff       (20)     2129 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     2171 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     4048 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-098.txt
--rw-r--r--   0 pato       (501) staff       (20)     1290 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-099.txt
--rw-r--r--   0 pato       (501) staff       (20)     2626 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-100.txt
--rw-r--r--   0 pato       (501) staff       (20)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-101.txt
--rw-r--r--   0 pato       (501) staff       (20)     3916 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-102.txt
--rw-r--r--   0 pato       (501) staff       (20)     2622 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-103.txt
--rw-r--r--   0 pato       (501) staff       (20)     3223 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-104.txt
--rw-r--r--   0 pato       (501) staff       (20)     3275 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-105.txt
--rw-r--r--   0 pato       (501) staff       (20)     4173 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-106.txt
--rw-r--r--   0 pato       (501) staff       (20)     4162 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-107.txt
--rw-r--r--   0 pato       (501) staff       (20)     4185 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-108.txt
--rw-r--r--   0 pato       (501) staff       (20)     1053 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-109.txt
--rw-r--r--   0 pato       (501) staff       (20)     4200 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-110.txt
--rw-r--r--   0 pato       (501) staff       (20)     1343 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-111.txt
--rw-r--r--   0 pato       (501) staff       (20)     4130 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-112.txt
--rw-r--r--   0 pato       (501) staff       (20)     4204 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-113.txt
--rw-r--r--   0 pato       (501) staff       (20)     4120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-114.txt
--rw-r--r--   0 pato       (501) staff       (20)     1116 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-115.txt
--rw-r--r--   0 pato       (501) staff       (20)     2194 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-116.txt
--rw-r--r--   0 pato       (501) staff       (20)     2144 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-117.txt
--rw-r--r--   0 pato       (501) staff       (20)     1437 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-118.txt
--rw-r--r--   0 pato       (501) staff       (20)     2192 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-119.txt
--rw-r--r--   0 pato       (501) staff       (20)     2140 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-120.txt
--rw-r--r--   0 pato       (501) staff       (20)     1364 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-121.txt
--rw-r--r--   0 pato       (501) staff       (20)     1546 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-122.txt
--rw-r--r--   0 pato       (501) staff       (20)     2171 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-123.txt
--rw-r--r--   0 pato       (501) staff       (20)     2248 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-124.txt
--rw-r--r--   0 pato       (501) staff       (20)     1371 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-125.txt
--rw-r--r--   0 pato       (501) staff       (20)      961 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-126.txt
--rw-r--r--   0 pato       (501) staff       (20)     4102 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-127.txt
--rw-r--r--   0 pato       (501) staff       (20)     1382 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-128.txt
--rw-r--r--   0 pato       (501) staff       (20)     1383 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-129.txt
--rw-r--r--   0 pato       (501) staff       (20)     1381 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-130.txt
--rw-r--r--   0 pato       (501) staff       (20)     1377 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-131.txt
--rw-r--r--   0 pato       (501) staff       (20)     1452 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-132.txt
--rw-r--r--   0 pato       (501) staff       (20)     2230 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-133.txt
--rw-r--r--   0 pato       (501) staff       (20)     2176 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-134.txt
--rw-r--r--   0 pato       (501) staff       (20)     1393 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-135.txt
--rw-r--r--   0 pato       (501) staff       (20)     1153 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-136.txt
--rw-r--r--   0 pato       (501) staff       (20)     1049 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-137.txt
--rw-r--r--   0 pato       (501) staff       (20)     1200 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-138.txt
--rw-r--r--   0 pato       (501) staff       (20)     4187 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-139.txt
--rw-r--r--   0 pato       (501) staff       (20)     1407 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/B-140.txt
--rw-r--r--   0 pato       (501) staff       (20)     2778 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1211 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2214 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2350 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3347 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1057 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     2092 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     2040 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3971 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1585 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2075 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     2255 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3976 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3731 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1726 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     2408 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     2704 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     4019 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-024.txt
--rw-r--r--   0 pato       (501) staff       (20)      777 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     1496 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1444 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     4014 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     3900 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     1160 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     2019 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     2037 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3216 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     3278 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     3748 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     1983 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3669 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ba-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     2828 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1299 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2147 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2092 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3430 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3828 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-007.txt
--rw-r--r--   0 pato       (501) staff       (20)      972 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3996 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1150 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1091 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1451 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1517 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1340 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     1610 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     4023 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-022.txt
--rw-r--r--   0 pato       (501) staff       (20)      901 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     1528 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     1471 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     4087 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1108 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     1857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     1806 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3855 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3883 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-034.txt
--rw-r--r--   0 pato       (501) staff       (20)      682 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-035.txt
--rw-r--r--   0 pato       (501) staff       (20)      681 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     4021 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     1018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     1140 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     1087 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     3921 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     2289 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     2231 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     3180 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     3332 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3667 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     1641 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     1516 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     1524 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     1344 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     1825 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     3659 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     3700 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     4087 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     4168 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     3908 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     2109 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     2065 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     2574 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     2735 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     4120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     4163 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     4192 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     4229 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Be-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     3780 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3910 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3717 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     4079 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1189 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3782 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3719 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1142 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1516 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     1796 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1262 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1209 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     1315 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3939 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3884 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3878 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1433 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     1513 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     1790 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3928 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3759 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3675 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3861 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     3048 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-038.txt
--rw-r--r--   0 pato       (501) staff       (20)      709 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     3067 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-040.txt
--rw-r--r--   0 pato       (501) staff       (20)      985 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     1655 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     1661 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     3971 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     1067 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     1234 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     1432 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3902 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     3991 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-049.txt
--rw-r--r--   0 pato       (501) staff       (20)      908 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-050.txt
--rw-r--r--   0 pato       (501) staff       (20)      918 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     1025 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3922 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-053.txt
--rw-r--r--   0 pato       (501) staff       (20)      927 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     3968 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-056.txt
--rw-r--r--   0 pato       (501) staff       (20)      925 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     1345 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     1351 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     3858 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     1087 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     3824 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-064.txt
--rw-r--r--   0 pato       (501) staff       (20)      791 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     1334 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     1511 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     3923 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     3902 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     1266 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     1965 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     2242 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     3972 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-073.txt
--rw-r--r--   0 pato       (501) staff       (20)      921 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-075.txt
--rw-r--r--   0 pato       (501) staff       (20)      981 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     1223 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     1390 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     4004 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-080.txt
--rw-r--r--   0 pato       (501) staff       (20)      933 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     1115 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     1420 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     3982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     4059 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     4097 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-092.txt
--rw-r--r--   0 pato       (501) staff       (20)      631 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     4008 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-095.txt
--rw-r--r--   0 pato       (501) staff       (20)      511 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     4020 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     1177 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-098.txt
--rw-r--r--   0 pato       (501) staff       (20)      635 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-099.txt
--rw-r--r--   0 pato       (501) staff       (20)      922 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-100.txt
--rw-r--r--   0 pato       (501) staff       (20)     4056 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-101.txt
--rw-r--r--   0 pato       (501) staff       (20)      811 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-102.txt
--rw-r--r--   0 pato       (501) staff       (20)     4053 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-103.txt
--rw-r--r--   0 pato       (501) staff       (20)      639 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-104.txt
--rw-r--r--   0 pato       (501) staff       (20)      864 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-105.txt
--rw-r--r--   0 pato       (501) staff       (20)      754 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-106.txt
--rw-r--r--   0 pato       (501) staff       (20)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-107.txt
--rw-r--r--   0 pato       (501) staff       (20)      686 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-108.txt
--rw-r--r--   0 pato       (501) staff       (20)      627 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-109.txt
--rw-r--r--   0 pato       (501) staff       (20)      740 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-110.txt
--rw-r--r--   0 pato       (501) staff       (20)     4016 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-111.txt
--rw-r--r--   0 pato       (501) staff       (20)      627 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-112.txt
--rw-r--r--   0 pato       (501) staff       (20)     4046 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Br-113.txt
--rw-r--r--   0 pato       (501) staff       (20)     1936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     2769 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3841 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3923 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3788 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2095 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     2868 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     2938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     2135 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     2238 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     2185 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     4020 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3677 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3823 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3864 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3984 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     4025 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3662 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3881 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     4015 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3926 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3816 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     4004 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3925 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-028.txt
--rw-r--r--   0 pato       (501) staff       (20)      756 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3918 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3737 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     3982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     4014 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     4034 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     4187 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     3984 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     3880 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     3998 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     3819 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     3965 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     4009 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     3651 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     3744 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     3840 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     3601 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     3709 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     3987 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     3988 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     3904 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-063.txt
--rw-r--r--   0 pato       (501) staff       (20)      993 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     1146 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     3882 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     1505 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     1879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     2149 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     3771 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     1523 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     1813 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     1890 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     1710 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     1590 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     1764 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-078.txt
--rw-r--r--   0 pato       (501) staff       (20)      814 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     3665 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     3688 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     1596 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     1979 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     2242 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     3786 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     3894 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     1614 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     1799 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     1980 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     3771 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     3783 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     3785 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-095.txt
--rw-r--r--   0 pato       (501) staff       (20)     3895 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-098.txt
--rw-r--r--   0 pato       (501) staff       (20)     3644 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-099.txt
--rw-r--r--   0 pato       (501) staff       (20)     2443 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-100.txt
--rw-r--r--   0 pato       (501) staff       (20)     2443 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-101.txt
--rw-r--r--   0 pato       (501) staff       (20)     3871 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-102.txt
--rw-r--r--   0 pato       (501) staff       (20)     3903 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-103.txt
--rw-r--r--   0 pato       (501) staff       (20)     3016 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-104.txt
--rw-r--r--   0 pato       (501) staff       (20)     3719 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-105.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-106.txt
--rw-r--r--   0 pato       (501) staff       (20)     2576 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-107.txt
--rw-r--r--   0 pato       (501) staff       (20)     2882 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-108.txt
--rw-r--r--   0 pato       (501) staff       (20)     2926 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-109.txt
--rw-r--r--   0 pato       (501) staff       (20)     3193 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-110.txt
--rw-r--r--   0 pato       (501) staff       (20)     3788 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-111.txt
--rw-r--r--   0 pato       (501) staff       (20)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-112.txt
--rw-r--r--   0 pato       (501) staff       (20)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-113.txt
--rw-r--r--   0 pato       (501) staff       (20)     3781 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-114.txt
--rw-r--r--   0 pato       (501) staff       (20)     3856 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-115.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-116.txt
--rw-r--r--   0 pato       (501) staff       (20)     3867 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-117.txt
--rw-r--r--   0 pato       (501) staff       (20)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-118.txt
--rw-r--r--   0 pato       (501) staff       (20)     1664 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-119.txt
--rw-r--r--   0 pato       (501) staff       (20)     3748 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-120.txt
--rw-r--r--   0 pato       (501) staff       (20)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-121.txt
--rw-r--r--   0 pato       (501) staff       (20)     4024 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-122.txt
--rw-r--r--   0 pato       (501) staff       (20)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-123.txt
--rw-r--r--   0 pato       (501) staff       (20)     3861 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-124.txt
--rw-r--r--   0 pato       (501) staff       (20)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-125.txt
--rw-r--r--   0 pato       (501) staff       (20)     3832 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-126.txt
--rw-r--r--   0 pato       (501) staff       (20)     3647 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-127.txt
--rw-r--r--   0 pato       (501) staff       (20)     3848 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-128.txt
--rw-r--r--   0 pato       (501) staff       (20)     3912 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-129.txt
--rw-r--r--   0 pato       (501) staff       (20)     3972 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-130.txt
--rw-r--r--   0 pato       (501) staff       (20)     1228 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-131.txt
--rw-r--r--   0 pato       (501) staff       (20)     1496 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-132.txt
--rw-r--r--   0 pato       (501) staff       (20)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-133.txt
--rw-r--r--   0 pato       (501) staff       (20)     3884 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-134.txt
--rw-r--r--   0 pato       (501) staff       (20)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-135.txt
--rw-r--r--   0 pato       (501) staff       (20)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-136.txt
--rw-r--r--   0 pato       (501) staff       (20)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-137.txt
--rw-r--r--   0 pato       (501) staff       (20)     3698 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-138.txt
--rw-r--r--   0 pato       (501) staff       (20)     2005 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-139.txt
--rw-r--r--   0 pato       (501) staff       (20)     1721 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-140.txt
--rw-r--r--   0 pato       (501) staff       (20)     1551 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-141.txt
--rw-r--r--   0 pato       (501) staff       (20)     3975 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-142.txt
--rw-r--r--   0 pato       (501) staff       (20)     3886 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-143.txt
--rw-r--r--   0 pato       (501) staff       (20)      993 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-144.txt
--rw-r--r--   0 pato       (501) staff       (20)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-145.txt
--rw-r--r--   0 pato       (501) staff       (20)      703 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-146.txt
--rw-r--r--   0 pato       (501) staff       (20)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-147.txt
--rw-r--r--   0 pato       (501) staff       (20)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-148.txt
--rw-r--r--   0 pato       (501) staff       (20)      740 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-149.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-150.txt
--rw-r--r--   0 pato       (501) staff       (20)     1473 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/C-151.txt
--rw-r--r--   0 pato       (501) staff       (20)     2879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      824 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1039 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1575 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1689 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3286 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1466 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     2077 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     2143 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3974 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     2705 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2889 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3933 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-019.txt
--rw-r--r--   0 pato       (501) staff       (20)      800 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     4015 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     1151 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     1761 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     1830 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     2370 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     2906 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     2957 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3647 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1962 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3646 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ca-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3800 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3922 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3850 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1550 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     1925 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     2206 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3950 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1005 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1889 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     1941 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3871 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3839 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3625 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3986 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     4028 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     4079 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3939 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     4158 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     4068 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     4112 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3852 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3978 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     1189 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     1221 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3770 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-031.txt
--rw-r--r--   0 pato       (501) staff       (20)      801 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-032.txt
--rw-r--r--   0 pato       (501) staff       (20)      700 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-033.txt
--rw-r--r--   0 pato       (501) staff       (20)      853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3781 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     1139 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     1323 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     1493 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     1207 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     1425 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     1419 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     1479 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     1043 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     1099 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     3878 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     3839 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     3637 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     1133 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     1726 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     1788 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     1086 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     3710 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     3755 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     3765 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     3918 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     3669 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     3872 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     2943 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     1145 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     1432 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     1503 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     3917 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     1074 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     4040 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     1443 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     1348 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     1513 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     3999 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     1015 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     1033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     1082 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     3933 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     1099 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     3973 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     1451 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     1742 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     1808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-095.txt
--rw-r--r--   0 pato       (501) staff       (20)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     4049 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-098.txt
--rw-r--r--   0 pato       (501) staff       (20)     1424 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-099.txt
--rw-r--r--   0 pato       (501) staff       (20)     1318 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-100.txt
--rw-r--r--   0 pato       (501) staff       (20)     1480 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-101.txt
--rw-r--r--   0 pato       (501) staff       (20)     3897 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-102.txt
--rw-r--r--   0 pato       (501) staff       (20)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-103.txt
--rw-r--r--   0 pato       (501) staff       (20)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-104.txt
--rw-r--r--   0 pato       (501) staff       (20)     4011 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-105.txt
--rw-r--r--   0 pato       (501) staff       (20)      696 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-106.txt
--rw-r--r--   0 pato       (501) staff       (20)     4041 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-107.txt
--rw-r--r--   0 pato       (501) staff       (20)     1031 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-108.txt
--rw-r--r--   0 pato       (501) staff       (20)     1449 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-109.txt
--rw-r--r--   0 pato       (501) staff       (20)     1395 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-110.txt
--rw-r--r--   0 pato       (501) staff       (20)     3931 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-111.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-112.txt
--rw-r--r--   0 pato       (501) staff       (20)      528 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-113.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-114.txt
--rw-r--r--   0 pato       (501) staff       (20)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-115.txt
--rw-r--r--   0 pato       (501) staff       (20)      657 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-116.txt
--rw-r--r--   0 pato       (501) staff       (20)     1048 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-117.txt
--rw-r--r--   0 pato       (501) staff       (20)     3941 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-118.txt
--rw-r--r--   0 pato       (501) staff       (20)     1580 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-119.txt
--rw-r--r--   0 pato       (501) staff       (20)     2072 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-120.txt
--rw-r--r--   0 pato       (501) staff       (20)     2244 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-121.txt
--rw-r--r--   0 pato       (501) staff       (20)     3977 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-122.txt
--rw-r--r--   0 pato       (501) staff       (20)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-123.txt
--rw-r--r--   0 pato       (501) staff       (20)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-124.txt
--rw-r--r--   0 pato       (501) staff       (20)     1269 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-125.txt
--rw-r--r--   0 pato       (501) staff       (20)     3859 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-126.txt
--rw-r--r--   0 pato       (501) staff       (20)     1033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-127.txt
--rw-r--r--   0 pato       (501) staff       (20)     1334 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-128.txt
--rw-r--r--   0 pato       (501) staff       (20)     1390 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-129.txt
--rw-r--r--   0 pato       (501) staff       (20)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-130.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-131.txt
--rw-r--r--   0 pato       (501) staff       (20)     4066 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-132.txt
--rw-r--r--   0 pato       (501) staff       (20)     4068 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-133.txt
--rw-r--r--   0 pato       (501) staff       (20)     1161 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-134.txt
--rw-r--r--   0 pato       (501) staff       (20)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-135.txt
--rw-r--r--   0 pato       (501) staff       (20)     1219 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-136.txt
--rw-r--r--   0 pato       (501) staff       (20)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-137.txt
--rw-r--r--   0 pato       (501) staff       (20)     4017 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-138.txt
--rw-r--r--   0 pato       (501) staff       (20)     4113 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-139.txt
--rw-r--r--   0 pato       (501) staff       (20)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-140.txt
--rw-r--r--   0 pato       (501) staff       (20)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-141.txt
--rw-r--r--   0 pato       (501) staff       (20)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-142.txt
--rw-r--r--   0 pato       (501) staff       (20)     3959 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-143.txt
--rw-r--r--   0 pato       (501) staff       (20)     1113 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-144.txt
--rw-r--r--   0 pato       (501) staff       (20)     3990 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-145.txt
--rw-r--r--   0 pato       (501) staff       (20)     1302 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-146.txt
--rw-r--r--   0 pato       (501) staff       (20)     3994 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-147.txt
--rw-r--r--   0 pato       (501) staff       (20)     4064 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-148.txt
--rw-r--r--   0 pato       (501) staff       (20)     4066 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-149.txt
--rw-r--r--   0 pato       (501) staff       (20)     4101 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-150.txt
--rw-r--r--   0 pato       (501) staff       (20)     1053 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-151.txt
--rw-r--r--   0 pato       (501) staff       (20)     1052 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-152.txt
--rw-r--r--   0 pato       (501) staff       (20)     1107 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-153.txt
--rw-r--r--   0 pato       (501) staff       (20)     4027 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-154.txt
--rw-r--r--   0 pato       (501) staff       (20)      753 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-155.txt
--rw-r--r--   0 pato       (501) staff       (20)      752 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-156.txt
--rw-r--r--   0 pato       (501) staff       (20)      808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-157.txt
--rw-r--r--   0 pato       (501) staff       (20)     4035 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-158.txt
--rw-r--r--   0 pato       (501) staff       (20)     4096 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-159.txt
--rw-r--r--   0 pato       (501) staff       (20)     4056 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-160.txt
--rw-r--r--   0 pato       (501) staff       (20)      567 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-161.txt
--rw-r--r--   0 pato       (501) staff       (20)      790 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-162.txt
--rw-r--r--   0 pato       (501) staff       (20)      922 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-163.txt
--rw-r--r--   0 pato       (501) staff       (20)     4062 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-164.txt
--rw-r--r--   0 pato       (501) staff       (20)     1287 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-165.txt
--rw-r--r--   0 pato       (501) staff       (20)     4006 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-166.txt
--rw-r--r--   0 pato       (501) staff       (20)      812 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-167.txt
--rw-r--r--   0 pato       (501) staff       (20)     4060 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-168.txt
--rw-r--r--   0 pato       (501) staff       (20)      748 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-169.txt
--rw-r--r--   0 pato       (501) staff       (20)      869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-170.txt
--rw-r--r--   0 pato       (501) staff       (20)      924 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-171.txt
--rw-r--r--   0 pato       (501) staff       (20)     4038 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-172.txt
--rw-r--r--   0 pato       (501) staff       (20)      564 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-173.txt
--rw-r--r--   0 pato       (501) staff       (20)      788 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-174.txt
--rw-r--r--   0 pato       (501) staff       (20)      679 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-175.txt
--rw-r--r--   0 pato       (501) staff       (20)     4044 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-176.txt
--rw-r--r--   0 pato       (501) staff       (20)     4038 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-177.txt
--rw-r--r--   0 pato       (501) staff       (20)      565 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-178.txt
--rw-r--r--   0 pato       (501) staff       (20)      790 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-179.txt
--rw-r--r--   0 pato       (501) staff       (20)      680 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-180.txt
--rw-r--r--   0 pato       (501) staff       (20)     4042 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-181.txt
--rw-r--r--   0 pato       (501) staff       (20)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-182.txt
--rw-r--r--   0 pato       (501) staff       (20)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-183.txt
--rw-r--r--   0 pato       (501) staff       (20)     1100 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-184.txt
--rw-r--r--   0 pato       (501) staff       (20)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-185.txt
--rw-r--r--   0 pato       (501) staff       (20)     4107 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-186.txt
--rw-r--r--   0 pato       (501) staff       (20)      989 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-187.txt
--rw-r--r--   0 pato       (501) staff       (20)     4053 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-188.txt
--rw-r--r--   0 pato       (501) staff       (20)      851 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-189.txt
--rw-r--r--   0 pato       (501) staff       (20)     1098 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-190.txt
--rw-r--r--   0 pato       (501) staff       (20)     1041 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-191.txt
--rw-r--r--   0 pato       (501) staff       (20)     1305 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-192.txt
--rw-r--r--   0 pato       (501) staff       (20)     4030 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-193.txt
--rw-r--r--   0 pato       (501) staff       (20)     4198 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cl-194.txt
--rw-r--r--   0 pato       (501) staff       (20)     2731 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1662 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2410 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2461 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3498 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3876 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3814 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1448 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1966 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     2121 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-011.txt
--rw-r--r--   0 pato       (501) staff       (20)      982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1526 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1113 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Co-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1676 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2214 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2097 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3467 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1607 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3844 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1539 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2234 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3044 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3216 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cr-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      840 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1030 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1146 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3150 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3778 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3753 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1320 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1923 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1976 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-011.txt
--rw-r--r--   0 pato       (501) staff       (20)      930 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1328 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1580 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3794 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3678 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     4028 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     4034 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3920 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     1129 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     1017 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     2296 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     4139 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cs-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     2976 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1237 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2394 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2298 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3446 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3831 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1249 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3876 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1441 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     1760 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1816 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-013.txt
--rw-r--r--   0 pato       (501) staff       (20)      987 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1321 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     1413 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1421 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1410 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     1474 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     1007 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Cu-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3805 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3744 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3478 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3812 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3732 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3708 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3737 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     2938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3707 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3730 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3662 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3684 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     2713 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/D-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3731 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     4118 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     4145 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     4193 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     4243 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3887 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     4032 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3775 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3928 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     1431 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1920 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     2088 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     1714 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     1911 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     2075 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3832 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     3873 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3838 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     2019 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     2320 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     2378 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     3950 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     3814 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     3980 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3782 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     3912 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     3854 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     3904 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     3791 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     3749 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     3913 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3802 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     2941 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     1447 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     1935 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     2105 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     3969 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     1583 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     1465 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     1637 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     4046 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     1328 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     1445 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-066.txt
--rw-r--r--   0 pato       (501) staff       (20)      991 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     3896 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     3896 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     1475 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     2084 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     2147 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     3983 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     3793 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     4023 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     3788 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     4040 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     4029 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     4024 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     3840 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     3898 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-090.txt
--rw-r--r--   0 pato       (501) staff       (20)      732 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     1090 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     1143 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     1194 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-095.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     3876 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-098.txt
--rw-r--r--   0 pato       (501) staff       (20)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-099.txt
--rw-r--r--   0 pato       (501) staff       (20)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-100.txt
--rw-r--r--   0 pato       (501) staff       (20)     4005 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-101.txt
--rw-r--r--   0 pato       (501) staff       (20)     2016 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-102.txt
--rw-r--r--   0 pato       (501) staff       (20)     2404 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-103.txt
--rw-r--r--   0 pato       (501) staff       (20)     2685 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-104.txt
--rw-r--r--   0 pato       (501) staff       (20)     3988 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-105.txt
--rw-r--r--   0 pato       (501) staff       (20)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-106.txt
--rw-r--r--   0 pato       (501) staff       (20)     1332 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-107.txt
--rw-r--r--   0 pato       (501) staff       (20)     2080 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-108.txt
--rw-r--r--   0 pato       (501) staff       (20)     2020 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-109.txt
--rw-r--r--   0 pato       (501) staff       (20)     3996 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-110.txt
--rw-r--r--   0 pato       (501) staff       (20)     1414 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-111.txt
--rw-r--r--   0 pato       (501) staff       (20)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-112.txt
--rw-r--r--   0 pato       (501) staff       (20)     4137 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-113.txt
--rw-r--r--   0 pato       (501) staff       (20)     4154 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-114.txt
--rw-r--r--   0 pato       (501) staff       (20)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-115.txt
--rw-r--r--   0 pato       (501) staff       (20)     3915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-116.txt
--rw-r--r--   0 pato       (501) staff       (20)     3998 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-117.txt
--rw-r--r--   0 pato       (501) staff       (20)     4130 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-118.txt
--rw-r--r--   0 pato       (501) staff       (20)     4023 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-119.txt
--rw-r--r--   0 pato       (501) staff       (20)     4106 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-120.txt
--rw-r--r--   0 pato       (501) staff       (20)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-121.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-122.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-123.txt
--rw-r--r--   0 pato       (501) staff       (20)     4084 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-124.txt
--rw-r--r--   0 pato       (501) staff       (20)     1332 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-125.txt
--rw-r--r--   0 pato       (501) staff       (20)     4109 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-126.txt
--rw-r--r--   0 pato       (501) staff       (20)     1015 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-127.txt
--rw-r--r--   0 pato       (501) staff       (20)     4103 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-128.txt
--rw-r--r--   0 pato       (501) staff       (20)     4167 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-129.txt
--rw-r--r--   0 pato       (501) staff       (20)     4063 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-130.txt
--rw-r--r--   0 pato       (501) staff       (20)     4143 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-131.txt
--rw-r--r--   0 pato       (501) staff       (20)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-132.txt
--rw-r--r--   0 pato       (501) staff       (20)      774 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-133.txt
--rw-r--r--   0 pato       (501) staff       (20)      773 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-134.txt
--rw-r--r--   0 pato       (501) staff       (20)      827 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-135.txt
--rw-r--r--   0 pato       (501) staff       (20)     4154 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-136.txt
--rw-r--r--   0 pato       (501) staff       (20)     4119 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-137.txt
--rw-r--r--   0 pato       (501) staff       (20)     4019 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-138.txt
--rw-r--r--   0 pato       (501) staff       (20)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-139.txt
--rw-r--r--   0 pato       (501) staff       (20)     3962 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-140.txt
--rw-r--r--   0 pato       (501) staff       (20)     4168 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-141.txt
--rw-r--r--   0 pato       (501) staff       (20)     1154 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-142.txt
--rw-r--r--   0 pato       (501) staff       (20)     4175 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-143.txt
--rw-r--r--   0 pato       (501) staff       (20)     1091 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-144.txt
--rw-r--r--   0 pato       (501) staff       (20)     4192 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-145.txt
--rw-r--r--   0 pato       (501) staff       (20)     4028 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-146.txt
--rw-r--r--   0 pato       (501) staff       (20)     4144 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-147.txt
--rw-r--r--   0 pato       (501) staff       (20)     4141 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-148.txt
--rw-r--r--   0 pato       (501) staff       (20)     4030 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-149.txt
--rw-r--r--   0 pato       (501) staff       (20)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-150.txt
--rw-r--r--   0 pato       (501) staff       (20)     4048 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-151.txt
--rw-r--r--   0 pato       (501) staff       (20)      757 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-152.txt
--rw-r--r--   0 pato       (501) staff       (20)     4154 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-153.txt
--rw-r--r--   0 pato       (501) staff       (20)     4117 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-154.txt
--rw-r--r--   0 pato       (501) staff       (20)     4058 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-155.txt
--rw-r--r--   0 pato       (501) staff       (20)      707 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-156.txt
--rw-r--r--   0 pato       (501) staff       (20)     4160 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-157.txt
--rw-r--r--   0 pato       (501) staff       (20)     4077 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-158.txt
--rw-r--r--   0 pato       (501) staff       (20)     4265 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-159.txt
--rw-r--r--   0 pato       (501) staff       (20)     4045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-160.txt
--rw-r--r--   0 pato       (501) staff       (20)     4963 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/F-161.txt
--rw-r--r--   0 pato       (501) staff       (20)     1770 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1346 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2614 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1564 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1399 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     2433 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     2445 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3491 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-010.txt
--rw-r--r--   0 pato       (501) staff       (20)      984 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     4005 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-012.txt
--rw-r--r--   0 pato       (501) staff       (20)      996 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1109 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1303 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1458 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3817 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1298 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3195 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3140 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3856 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     1420 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     1549 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2643 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     2724 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3885 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1004 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     1003 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     3965 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     1931 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1349 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     2301 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Fe-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     2996 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      573 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1662 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1779 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3386 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3800 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ga-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3802 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3742 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3750 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3981 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-006.txt
--rw-r--r--   0 pato       (501) staff       (20)      906 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3794 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1238 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1321 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     1592 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3935 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1062 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1241 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1401 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3842 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1125 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1616 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1779 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3861 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3871 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3819 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3981 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1012 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3790 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     1225 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     1611 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     1872 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     3933 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     3705 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     3828 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     3761 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3889 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     2936 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     4033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     4077 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     1309 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-056.txt
--rw-r--r--   0 pato       (501) staff       (20)      796 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     4011 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     4051 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     3704 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     3902 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-062.txt
--rw-r--r--   0 pato       (501) staff       (20)      921 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     3725 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     1473 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     1248 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     1246 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     1127 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     1121 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     1064 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-070.txt
--rw-r--r--   0 pato       (501) staff       (20)      744 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     1478 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     1422 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-074.txt
--rw-r--r--   0 pato       (501) staff       (20)      920 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     4044 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-076.txt
--rw-r--r--   0 pato       (501) staff       (20)      700 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     4040 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     3831 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     3657 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     1325 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     3679 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-084.txt
--rw-r--r--   0 pato       (501) staff       (20)      885 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-085.txt
--rw-r--r--   0 pato       (501) staff       (20)      760 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-086.txt
--rw-r--r--   0 pato       (501) staff       (20)      939 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     3831 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     1282 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-089.txt
--rw-r--r--   0 pato       (501) staff       (20)      613 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     3982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-091.txt
--rw-r--r--   0 pato       (501) staff       (20)      952 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-093.txt
--rw-r--r--   0 pato       (501) staff       (20)      960 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-094.txt
--rw-r--r--   0 pato       (501) staff       (20)      966 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-095.txt
--rw-r--r--   0 pato       (501) staff       (20)      971 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-096.txt
--rw-r--r--   0 pato       (501) staff       (20)      992 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/H-097.txt
--rw-r--r--   0 pato       (501) staff       (20)     2916 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/He-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/He-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2863 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1435 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1852 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3173 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3006 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3761 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3889 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3805 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hf-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3021 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1458 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3104 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3790 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     1116 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     1132 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1197 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-009.txt
--rw-r--r--   0 pato       (501) staff       (20)      740 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3814 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1050 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1104 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Hg-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3733 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3840 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1439 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1621 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     1793 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3923 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1554 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1614 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1666 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3825 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1430 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2013 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     2077 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3895 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3850 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3904 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     3052 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-023.txt
--rw-r--r--   0 pato       (501) staff       (20)      697 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-024.txt
--rw-r--r--   0 pato       (501) staff       (20)      837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-025.txt
--rw-r--r--   0 pato       (501) staff       (20)      949 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3103 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3959 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     3962 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     1028 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1449 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     1395 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-033.txt
--rw-r--r--   0 pato       (501) staff       (20)      959 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-035.txt
--rw-r--r--   0 pato       (501) staff       (20)      841 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     1132 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     1196 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3858 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     3822 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     1156 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     1825 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     1889 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     1262 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     1031 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     1340 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     1395 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-050.txt
--rw-r--r--   0 pato       (501) staff       (20)      673 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     3856 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-053.txt
--rw-r--r--   0 pato       (501) staff       (20)      986 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     1413 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-057.txt
--rw-r--r--   0 pato       (501) staff       (20)      441 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     3917 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     4017 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-060.txt
--rw-r--r--   0 pato       (501) staff       (20)      439 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-061.txt
--rw-r--r--   0 pato       (501) staff       (20)      558 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-062.txt
--rw-r--r--   0 pato       (501) staff       (20)      612 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     4006 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     1263 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     1041 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     1319 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     4019 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-068.txt
--rw-r--r--   0 pato       (501) staff       (20)      807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     4035 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/I-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     3029 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      471 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1020 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3163 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3787 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3757 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3795 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1085 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3686 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1288 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1308 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1661 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     2141 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2217 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     1026 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1142 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     2121 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     2304 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     4138 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     1466 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     2067 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2125 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/K-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     2917 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Kr-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Kr-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2872 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      896 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1338 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1520 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3268 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3795 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3765 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3780 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3820 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2031 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     2649 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2694 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3940 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1298 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1845 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     2761 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     2830 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     2273 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2775 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     2949 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     1024 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1459 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     2125 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     2306 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     4130 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     2158 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     2210 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-033.txt
--rw-r--r--   0 pato       (501) staff       (20)      950 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Li-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     3013 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1297 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1322 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1356 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3226 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2582 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3187 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3233 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3775 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     2036 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     2131 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2405 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     2161 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2773 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     2837 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1821 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1810 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1876 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     1476 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     2193 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     2804 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2878 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     1946 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3858 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     2175 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     2782 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     2850 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     2185 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     2792 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     2864 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     1592 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     2475 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     2538 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     1791 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     2062 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3140 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     3087 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mg-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     2847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mn-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1465 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mn-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mn-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2101 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mn-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3374 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mn-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3829 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mn-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     2958 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1771 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3287 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3049 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3761 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3896 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3852 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3838 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-010.txt
--rw-r--r--   0 pato       (501) staff       (20)      981 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-011.txt
--rw-r--r--   0 pato       (501) staff       (20)      983 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-012.txt
--rw-r--r--   0 pato       (501) staff       (20)      983 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1156 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1458 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1521 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1604 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1596 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     2369 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     2316 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Mo-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     2187 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3791 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3733 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3791 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3829 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3725 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3873 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3878 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3917 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2876 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     2882 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2929 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     2210 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     2589 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3886 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     2938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     3767 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3822 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     4005 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-028.txt
--rw-r--r--   0 pato       (501) staff       (20)      543 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-029.txt
--rw-r--r--   0 pato       (501) staff       (20)      509 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-030.txt
--rw-r--r--   0 pato       (501) staff       (20)      595 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     3728 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3894 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     1910 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-035.txt
--rw-r--r--   0 pato       (501) staff       (20)      982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/N-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     2934 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      920 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1050 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1255 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3186 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3792 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3758 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3852 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1387 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3838 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1648 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1941 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2306 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     1828 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1902 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1030 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     1128 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-020.txt
--rw-r--r--   0 pato       (501) staff       (20)      841 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-021.txt
--rw-r--r--   0 pato       (501) staff       (20)      808 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-022.txt
--rw-r--r--   0 pato       (501) staff       (20)      887 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2114 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     2389 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     4131 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     1367 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     1748 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     1734 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     2123 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     1461 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     2040 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-032.txt
--rw-r--r--   0 pato       (501) staff       (20)     2101 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-033.txt
--rw-r--r--   0 pato       (501) staff       (20)      759 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     1166 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-035.txt
--rw-r--r--   0 pato       (501) staff       (20)     1115 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Na-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     2866 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1727 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3263 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2965 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3793 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3903 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1790 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     2033 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1964 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3848 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     2109 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     2034 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     2283 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     1724 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3394 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3470 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Nb-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     2914 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ne-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ne-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2856 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1563 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2196 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2129 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3491 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3803 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1298 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     2292 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     2346 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     1197 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1295 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1252 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1324 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2545 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     2715 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-017.txt
--rw-r--r--   0 pato       (501) staff       (20)      746 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ni-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3654 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1057 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     1169 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     1586 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1853 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3767 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3881 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     2278 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     3210 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     3269 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     1720 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     1655 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     2913 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     3073 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     3820 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-022.txt
--rw-r--r--   0 pato       (501) staff       (20)     1776 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-023.txt
--rw-r--r--   0 pato       (501) staff       (20)     2317 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-024.txt
--rw-r--r--   0 pato       (501) staff       (20)     2369 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-025.txt
--rw-r--r--   0 pato       (501) staff       (20)     3823 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-026.txt
--rw-r--r--   0 pato       (501) staff       (20)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-027.txt
--rw-r--r--   0 pato       (501) staff       (20)     3795 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-028.txt
--rw-r--r--   0 pato       (501) staff       (20)     2937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-029.txt
--rw-r--r--   0 pato       (501) staff       (20)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-030.txt
--rw-r--r--   0 pato       (501) staff       (20)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-031.txt
--rw-r--r--   0 pato       (501) staff       (20)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-032.txt
--rw-r--r--   0 pato       (501) staff       (20)      893 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-033.txt
--rw-r--r--   0 pato       (501) staff       (20)     3760 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-034.txt
--rw-r--r--   0 pato       (501) staff       (20)     1880 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-035.txt
--rw-r--r--   0 pato       (501) staff       (20)      801 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-036.txt
--rw-r--r--   0 pato       (501) staff       (20)     1531 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-037.txt
--rw-r--r--   0 pato       (501) staff       (20)     2940 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-038.txt
--rw-r--r--   0 pato       (501) staff       (20)     3086 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-039.txt
--rw-r--r--   0 pato       (501) staff       (20)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-040.txt
--rw-r--r--   0 pato       (501) staff       (20)     3957 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-041.txt
--rw-r--r--   0 pato       (501) staff       (20)     1393 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-042.txt
--rw-r--r--   0 pato       (501) staff       (20)     1757 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-043.txt
--rw-r--r--   0 pato       (501) staff       (20)     2673 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-044.txt
--rw-r--r--   0 pato       (501) staff       (20)     2613 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-045.txt
--rw-r--r--   0 pato       (501) staff       (20)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-046.txt
--rw-r--r--   0 pato       (501) staff       (20)     1982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-047.txt
--rw-r--r--   0 pato       (501) staff       (20)     3763 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-048.txt
--rw-r--r--   0 pato       (501) staff       (20)     1891 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-049.txt
--rw-r--r--   0 pato       (501) staff       (20)     1896 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-050.txt
--rw-r--r--   0 pato       (501) staff       (20)     1898 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-051.txt
--rw-r--r--   0 pato       (501) staff       (20)     2493 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-052.txt
--rw-r--r--   0 pato       (501) staff       (20)     3392 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-053.txt
--rw-r--r--   0 pato       (501) staff       (20)     3462 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-054.txt
--rw-r--r--   0 pato       (501) staff       (20)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-055.txt
--rw-r--r--   0 pato       (501) staff       (20)     3709 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-056.txt
--rw-r--r--   0 pato       (501) staff       (20)     1462 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-057.txt
--rw-r--r--   0 pato       (501) staff       (20)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-058.txt
--rw-r--r--   0 pato       (501) staff       (20)     2259 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-059.txt
--rw-r--r--   0 pato       (501) staff       (20)     2456 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-060.txt
--rw-r--r--   0 pato       (501) staff       (20)     2628 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-061.txt
--rw-r--r--   0 pato       (501) staff       (20)     2116 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-062.txt
--rw-r--r--   0 pato       (501) staff       (20)     2742 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-063.txt
--rw-r--r--   0 pato       (501) staff       (20)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-064.txt
--rw-r--r--   0 pato       (501) staff       (20)     2170 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-065.txt
--rw-r--r--   0 pato       (501) staff       (20)     2065 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-066.txt
--rw-r--r--   0 pato       (501) staff       (20)     2225 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-067.txt
--rw-r--r--   0 pato       (501) staff       (20)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-068.txt
--rw-r--r--   0 pato       (501) staff       (20)     1478 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-069.txt
--rw-r--r--   0 pato       (501) staff       (20)     1120 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-070.txt
--rw-r--r--   0 pato       (501) staff       (20)     1646 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-071.txt
--rw-r--r--   0 pato       (501) staff       (20)     2117 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-072.txt
--rw-r--r--   0 pato       (501) staff       (20)     1751 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-073.txt
--rw-r--r--   0 pato       (501) staff       (20)     2133 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-074.txt
--rw-r--r--   0 pato       (501) staff       (20)     2310 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-075.txt
--rw-r--r--   0 pato       (501) staff       (20)     3940 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-076.txt
--rw-r--r--   0 pato       (501) staff       (20)     2054 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-077.txt
--rw-r--r--   0 pato       (501) staff       (20)     3406 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-078.txt
--rw-r--r--   0 pato       (501) staff       (20)     3489 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-079.txt
--rw-r--r--   0 pato       (501) staff       (20)     1238 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-080.txt
--rw-r--r--   0 pato       (501) staff       (20)     1743 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-081.txt
--rw-r--r--   0 pato       (501) staff       (20)     2798 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-082.txt
--rw-r--r--   0 pato       (501) staff       (20)     2999 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-083.txt
--rw-r--r--   0 pato       (501) staff       (20)     1217 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-084.txt
--rw-r--r--   0 pato       (501) staff       (20)     2134 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-085.txt
--rw-r--r--   0 pato       (501) staff       (20)     2214 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-086.txt
--rw-r--r--   0 pato       (501) staff       (20)     4181 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-087.txt
--rw-r--r--   0 pato       (501) staff       (20)     4128 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-088.txt
--rw-r--r--   0 pato       (501) staff       (20)     1675 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-089.txt
--rw-r--r--   0 pato       (501) staff       (20)     2827 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-090.txt
--rw-r--r--   0 pato       (501) staff       (20)     2777 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-091.txt
--rw-r--r--   0 pato       (501) staff       (20)     4201 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-092.txt
--rw-r--r--   0 pato       (501) staff       (20)     4230 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-093.txt
--rw-r--r--   0 pato       (501) staff       (20)     1175 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-094.txt
--rw-r--r--   0 pato       (501) staff       (20)     4260 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-095.txt
--rw-r--r--   0 pato       (501) staff       (20)     4299 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/O-096.txt
--rw-r--r--   0 pato       (501) staff       (20)     2875 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      937 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1254 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1468 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-004.txt
--rw-r--r--   0 pato       (501) staff       (20)      872 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-005.txt
--rw-r--r--   0 pato       (501) staff       (20)      876 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-006.txt
--rw-r--r--   0 pato       (501) staff       (20)      870 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3909 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     3764 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3722 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3218 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1365 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1982 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     2036 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/P-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3011 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1046 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1780 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1769 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3330 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3778 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     1217 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     1387 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1446 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Pb-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     3031 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      627 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1081 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1197 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3149 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3786 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3755 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3682 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rb-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rn-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Rn-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2746 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      724 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-002.txt
--rw-r--r--   0 pato       (501) staff       (20)      948 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1123 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1325 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3903 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3682 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3842 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     1972 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-010.txt
--rw-r--r--   0 pato       (501) staff       (20)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-011.txt
--rw-r--r--   0 pato       (501) staff       (20)     3172 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-012.txt
--rw-r--r--   0 pato       (501) staff       (20)     1332 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-013.txt
--rw-r--r--   0 pato       (501) staff       (20)     1437 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-014.txt
--rw-r--r--   0 pato       (501) staff       (20)     1386 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-015.txt
--rw-r--r--   0 pato       (501) staff       (20)     3688 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-016.txt
--rw-r--r--   0 pato       (501) staff       (20)     3713 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-017.txt
--rw-r--r--   0 pato       (501) staff       (20)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-018.txt
--rw-r--r--   0 pato       (501) staff       (20)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-019.txt
--rw-r--r--   0 pato       (501) staff       (20)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-020.txt
--rw-r--r--   0 pato       (501) staff       (20)     4049 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/S-021.txt
--rw-r--r--   0 pato       (501) staff       (20)     2974 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1476 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2545 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2497 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3545 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3801 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3897 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     3913 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Si-009.txt
--rw-r--r--   0 pato       (501) staff       (20)     2890 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      989 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-002.txt
--rw-r--r--   0 pato       (501) staff       (20)      967 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1777 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     1960 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3275 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3803 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Sr-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2858 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     2004 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3191 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2823 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3884 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3925 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ta-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2851 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1097 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1530 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2663 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     2580 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3569 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3812 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Ti-008.txt
--rw-r--r--   0 pato       (501) staff       (20)     2974 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1520 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     2697 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2480 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3569 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3864 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3810 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/V-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2944 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     2506 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3138 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     2945 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3927 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/W-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Xe-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     3914 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Xe-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     3017 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-001.txt
--rw-r--r--   0 pato       (501) staff       (20)      776 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1418 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     1385 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3189 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3758 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zn-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     2849 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-001.txt
--rw-r--r--   0 pato       (501) staff       (20)     1101 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-002.txt
--rw-r--r--   0 pato       (501) staff       (20)     1565 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-003.txt
--rw-r--r--   0 pato       (501) staff       (20)     3140 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-004.txt
--rw-r--r--   0 pato       (501) staff       (20)     3020 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-005.txt
--rw-r--r--   0 pato       (501) staff       (20)     3735 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-006.txt
--rw-r--r--   0 pato       (501) staff       (20)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-007.txt
--rw-r--r--   0 pato       (501) staff       (20)     3809 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf/Zr-008.txt
--rw-r--r--   0 pato       (501) staff       (20)    61498 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/chemcat/data/janaf_conversion.txt
--rw-r--r--   0 pato       (501) staff       (20)   255474 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/chemcat/data/thermo_build_cea.dat
--rw-r--r--   0 pato       (501) staff       (20)      471 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/chemcat/data/white_pages.txt
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.852646 chemcat-0.3.8b1/chemcat/janaf/
--rw-r--r--   0 pato       (501) staff       (20)      478 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/janaf/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    12470 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/janaf/janaf.py
--rw-r--r--   0 pato       (501) staff       (20)    11695 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/network.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.853213 chemcat-0.3.8b1/chemcat/utils/
--rw-r--r--   0 pato       (501) staff       (20)      478 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/utils/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    32602 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/chemcat/utils/utils.py
--rw-r--r--   0 pato       (501) staff       (20)      165 2024-01-07 17:28:21.000000 chemcat-0.3.8b1/chemcat/version.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.860603 chemcat-0.3.8b1/chemcat.egg-info/
--rw-r--r--   0 pato       (501) staff       (20)    22694 2024-01-07 17:43:34.000000 chemcat-0.3.8b1/chemcat.egg-info/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)    54173 2024-01-07 17:43:34.000000 chemcat-0.3.8b1/chemcat.egg-info/SOURCES.txt
--rw-r--r--   0 pato       (501) staff       (20)        1 2024-01-07 17:43:34.000000 chemcat-0.3.8b1/chemcat.egg-info/dependency_links.txt
--rw-r--r--   0 pato       (501) staff       (20)       87 2024-01-07 17:43:34.000000 chemcat-0.3.8b1/chemcat.egg-info/requires.txt
--rw-r--r--   0 pato       (501) staff       (20)        8 2024-01-07 17:43:34.000000 chemcat-0.3.8b1/chemcat.egg-info/top_level.txt
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.858875 chemcat-0.3.8b1/docs/
--rw-r--r--   0 pato       (501) staff       (20)     7493 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/docs/Makefile
--rw-r--r--   0 pato       (501) staff       (20)    41421 2022-07-31 16:01:48.000000 chemcat-0.3.8b1/docs/api.rst
--rw-r--r--   0 pato       (501) staff       (20)  1034062 2023-06-20 07:49:53.000000 chemcat-0.3.8b1/docs/chemistry_tutorial.ipynb
--rw-r--r--   0 pato       (501) staff       (20)     7925 2022-07-31 16:01:48.000000 chemcat-0.3.8b1/docs/chemistry_tutorial.py
--rw-r--r--   0 pato       (501) staff       (20)    13689 2023-06-19 16:47:22.000000 chemcat-0.3.8b1/docs/chemistry_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)    11708 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/docs/conf.py
--rw-r--r--   0 pato       (501) staff       (20)     2970 2022-07-15 07:34:22.000000 chemcat-0.3.8b1/docs/contributing.rst
--rw-r--r--   0 pato       (501) staff       (20)    11705 2022-07-31 16:01:48.000000 chemcat-0.3.8b1/docs/database_tutorial.ipynb
--rw-r--r--   0 pato       (501) staff       (20)     3657 2022-07-31 16:01:48.000000 chemcat-0.3.8b1/docs/database_tutorial.py
--rw-r--r--   0 pato       (501) staff       (20)     8321 2022-07-31 16:01:48.000000 chemcat-0.3.8b1/docs/database_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)       24 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/docs/docs_requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)     2707 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/docs/get_started.rst
--rw-r--r--   0 pato       (501) staff       (20)     3266 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/docs/index.rst
--rw-r--r--   0 pato       (501) staff       (20)    16405 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/docs/license.rst
--rw-r--r--   0 pato       (501) staff       (20)      865 2024-01-07 17:40:36.000000 chemcat-0.3.8b1/pyproject.toml
--rw-r--r--   0 pato       (501) staff       (20)       67 2022-07-27 09:22:34.000000 chemcat-0.3.8b1/requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)       38 2024-01-07 17:43:34.864842 chemcat-0.3.8b1/setup.cfg
--rw-r--r--   0 pato       (501) staff       (20)     1032 2024-01-07 17:41:51.000000 chemcat-0.3.8b1/setup.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.859199 chemcat-0.3.8b1/src_c/
--rw-r--r--   0 pato       (501) staff       (20)     6387 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/src_c/_thermo.c
--rw-r--r--   0 pato       (501) staff       (20)     4201 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/src_c/_utils.c
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.859515 chemcat-0.3.8b1/src_c/include/
--rw-r--r--   0 pato       (501) staff       (20)      810 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/src_c/include/ind.h
--rw-r--r--   0 pato       (501) staff       (20)    10644 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/src_c/include/newton_raphson.h
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-01-07 17:43:34.860370 chemcat-0.3.8b1/tests/
--rw-r--r--   0 pato       (501) staff       (20)    28301 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/tests/conftest.py
--rw-r--r--   0 pato       (501) staff       (20)     6300 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/tests/test_cea.py
--rw-r--r--   0 pato       (501) staff       (20)    11098 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/tests/test_janaf.py
--rw-r--r--   0 pato       (501) staff       (20)    14784 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/tests/test_network.py
--rw-r--r--   0 pato       (501) staff       (20)    13208 2024-01-05 21:24:42.000000 chemcat-0.3.8b1/tests/test_utils.py
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.390498 chemcat-0.3.9/
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.198497 chemcat-0.3.9/.github/
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.198497 chemcat-0.3.9/.github/workflows/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1548 2024-05-21 08:34:32.000000 chemcat-0.3.9/.github/workflows/python-package.yml
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    18092 2022-07-07 21:33:49.000000 chemcat-0.3.9/LICENSE
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      295 2024-01-07 20:23:08.000000 chemcat-0.3.9/MANIFEST.in
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    22692 2024-05-21 08:35:16.390498 chemcat-0.3.9/PKG-INFO
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1349 2024-01-08 14:04:24.000000 chemcat-0.3.9/README.md
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.198497 chemcat-0.3.9/chemcat/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      634 2024-01-05 21:24:42.000000 chemcat-0.3.9/chemcat/__init__.py
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.198497 chemcat-0.3.9/chemcat/cea/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      474 2024-01-05 21:24:42.000000 chemcat-0.3.9/chemcat/cea/__init__.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    13648 2024-05-21 08:34:32.000000 chemcat-0.3.9/chemcat/cea/cea.py
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.198497 chemcat-0.3.9/chemcat/data/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3259 2022-07-27 09:22:34.000000 chemcat-0.3.9/chemcat/data/asplund_2009_solar_abundances.dat
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3688 2022-07-27 09:22:34.000000 chemcat-0.3.9/chemcat/data/asplund_2021_solar_abundances.dat
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.386498 chemcat-0.3.9/chemcat/data/janaf/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2975 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      854 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1803 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1727 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3428 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3802 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3848 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1170 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1051 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1225 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3891 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3841 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3990 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3809 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4068 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1897 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3959 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3894 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1172 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1055 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1227 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3968 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      739 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      733 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1387 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1385 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3781 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3834 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3988 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3774 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4100 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2238 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2748 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2916 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4101 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4108 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4194 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4192 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1631 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2180 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2583 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1152 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2219 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2350 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3859 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3834 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3841 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3880 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1300 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3805 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1058 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1362 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1114 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1626 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2742 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2801 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1912 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2170 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3637 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3695 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3867 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3889 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3686 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3734 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1797 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2799 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2861 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4143 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4151 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1074 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4205 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4132 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2059 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2796 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2864 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3999 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2147 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1968 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-098.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-099.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2752 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-100.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2817 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-101.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2133 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-102.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2127 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-103.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2135 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-104.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1115 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-105.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1244 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-106.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2239 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-107.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2316 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-108.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2220 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-109.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2872 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-110.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2942 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-111.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2181 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Al-112.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ar-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ar-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2918 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1543 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2613 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2361 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3627 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3803 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3993 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4014 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3994 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      722 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3968 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3898 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4001 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4088 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1211 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1112 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1266 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4163 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3939 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3882 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      968 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3976 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3919 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3891 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1121 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4087 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1405 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1401 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3839 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3867 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1476 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1464 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1529 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3995 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1477 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2086 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2155 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2181 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1472 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1771 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1836 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3829 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3916 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2425 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4162 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4129 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4151 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1042 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4113 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4017 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1312 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3984 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1171 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2129 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2171 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4048 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-098.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1290 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-099.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2626 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-100.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-101.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3916 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-102.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2622 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-103.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3223 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-104.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3275 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-105.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4173 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-106.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4162 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-107.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4185 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-108.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1053 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-109.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4200 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-110.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1343 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-111.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4130 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-112.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4204 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-113.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-114.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1116 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-115.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2194 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-116.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2144 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-117.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1437 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-118.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2192 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-119.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2140 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-120.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1364 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-121.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1546 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-122.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2171 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-123.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2248 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-124.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1371 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-125.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      961 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-126.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4102 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-127.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1382 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-128.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1383 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-129.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1381 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-130.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1377 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-131.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1452 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-132.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2230 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-133.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2176 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-134.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1393 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-135.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1153 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-136.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1049 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-137.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1200 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-138.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4187 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-139.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1407 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/B-140.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2778 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1211 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2214 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2350 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3347 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1057 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2092 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2040 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3971 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1585 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2075 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2255 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3976 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3731 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1726 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2408 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2704 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4019 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      777 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1496 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1444 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4014 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3900 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1160 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2019 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2037 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3216 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3278 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3748 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1983 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3669 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ba-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2828 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1299 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2147 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2092 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3430 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3828 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      972 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3996 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1150 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1091 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1451 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1517 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1340 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1610 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4023 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      901 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1528 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1471 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4087 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1108 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1806 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3855 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3883 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      682 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      681 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4021 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1140 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1087 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3921 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2289 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2231 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3180 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3332 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3667 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1641 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1516 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1524 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1344 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1825 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3659 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3700 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4087 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4168 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3908 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2109 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2065 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2574 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2735 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4163 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4192 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4229 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Be-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3780 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3910 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3717 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4079 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1189 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3782 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3719 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1142 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1516 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1796 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1262 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1209 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1315 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3939 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3884 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3878 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1433 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1513 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1790 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3928 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3759 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3675 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3861 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3048 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      709 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3067 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      985 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1655 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1661 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3971 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1067 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1234 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1432 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3902 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3991 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      908 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      918 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1025 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3922 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      927 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3968 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      925 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1345 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1351 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3858 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1087 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3824 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      791 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1334 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1511 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3923 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3902 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1266 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1965 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2242 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3972 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      921 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      981 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1223 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1390 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4004 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      933 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1115 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1420 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4059 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4097 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      631 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4008 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      511 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4020 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1177 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-098.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      635 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-099.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      922 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-100.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4056 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-101.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      811 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-102.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4053 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-103.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      639 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-104.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      864 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-105.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      754 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-106.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-107.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      686 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-108.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      627 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-109.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      740 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-110.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4016 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-111.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      627 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-112.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4046 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Br-113.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2769 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3841 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3923 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3788 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2095 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2868 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2135 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2238 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2185 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4020 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3677 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3823 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3864 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3984 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4025 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3662 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3881 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4015 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3926 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3816 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4004 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3925 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      756 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3918 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3737 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4014 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4034 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4187 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3984 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3880 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3998 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3819 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3965 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4009 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3651 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3744 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3840 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3601 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3709 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3987 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3988 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3904 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      993 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1146 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3882 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1505 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2149 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3771 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1523 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1813 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1890 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1710 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1590 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1764 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      814 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3665 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3688 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1596 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1979 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2242 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3786 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3894 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1614 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1799 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1980 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3771 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3783 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3785 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3895 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-098.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3644 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-099.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2443 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-100.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2443 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-101.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3871 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-102.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3903 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-103.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3016 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-104.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3719 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-105.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-106.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2576 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-107.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2882 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-108.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2926 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-109.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3193 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-110.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3788 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-111.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-112.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-113.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3781 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-114.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3856 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-115.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-116.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3867 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-117.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-118.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1664 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-119.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3748 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-120.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-121.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4024 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-122.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-123.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3861 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-124.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-125.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3832 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-126.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3647 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-127.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3848 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-128.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3912 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-129.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3972 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-130.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1228 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-131.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1496 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-132.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-133.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3884 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-134.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-135.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-136.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-137.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3698 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-138.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2005 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-139.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1721 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-140.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1551 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-141.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3975 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-142.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3886 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-143.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      993 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-144.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-145.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      703 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-146.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-147.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-148.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      740 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-149.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-150.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1473 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/C-151.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      824 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1039 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1575 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1689 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3286 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1466 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2077 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2143 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3974 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3954 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2705 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2889 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3933 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      800 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4015 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1151 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1761 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1830 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2370 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2906 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2957 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3647 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1962 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3646 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ca-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3800 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3922 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3850 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1550 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1925 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2206 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3950 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1005 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1889 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1941 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3871 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3839 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3625 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3986 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4028 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4079 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3939 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4158 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4068 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4112 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3852 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3978 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1189 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1221 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3770 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      801 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      700 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3781 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1139 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1323 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1493 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1207 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1425 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1419 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1479 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1043 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1099 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3878 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3839 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3637 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1133 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1726 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1788 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1086 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3710 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3755 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3765 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3918 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3669 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3866 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3872 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2943 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1145 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1432 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1503 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3917 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1074 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4040 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1443 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1348 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1513 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3999 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1015 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1082 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3933 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1099 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3973 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1451 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1742 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4049 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-098.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1424 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-099.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1318 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-100.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1480 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-101.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3897 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-102.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-103.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4003 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-104.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4011 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-105.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      696 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-106.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4041 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-107.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1031 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-108.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1449 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-109.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1395 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-110.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3931 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-111.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-112.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      528 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-113.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-114.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-115.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      657 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-116.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1048 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-117.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3941 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-118.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1580 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-119.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2072 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-120.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2244 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-121.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3977 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-122.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-123.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-124.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1269 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-125.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3859 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-126.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-127.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1334 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-128.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1390 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-129.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-130.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-131.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4066 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-132.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4068 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-133.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1161 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-134.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-135.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1219 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-136.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-137.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4017 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-138.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4113 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-139.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-140.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-141.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-142.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3959 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-143.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1113 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-144.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3990 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-145.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1302 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-146.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3994 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-147.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4064 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-148.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4066 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-149.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4101 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-150.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1053 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-151.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1052 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-152.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1107 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-153.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4027 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-154.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      753 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-155.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      752 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-156.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-157.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4035 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-158.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4096 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-159.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4056 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-160.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      567 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-161.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      790 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-162.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      922 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-163.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4062 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-164.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1287 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-165.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4006 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-166.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      812 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-167.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4060 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-168.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      748 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-169.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-170.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      924 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-171.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4038 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-172.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      564 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-173.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      788 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-174.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      679 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-175.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4044 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-176.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4038 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-177.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      565 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-178.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      790 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-179.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      680 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-180.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4042 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-181.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-182.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-183.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1100 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-184.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4022 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-185.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4107 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-186.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      989 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-187.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4053 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-188.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      851 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-189.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1098 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-190.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1041 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-191.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1305 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-192.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4030 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-193.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4198 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cl-194.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2731 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1662 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2410 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2461 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3498 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3876 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3814 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1448 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1966 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2121 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1526 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1113 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Co-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1676 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2214 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2097 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3467 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1607 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3844 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1539 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2234 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3044 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3216 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cr-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      840 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1030 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1146 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3150 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3778 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3753 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1320 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1923 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1976 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      930 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1328 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1580 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3794 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3678 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4028 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4034 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3920 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1129 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1017 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2296 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4139 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cs-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2976 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1237 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2394 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2298 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3446 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3831 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1249 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3876 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1441 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1760 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1816 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3946 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      987 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1321 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1413 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1421 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1410 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1474 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1007 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Cu-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3805 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3744 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3478 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3812 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3732 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3708 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3737 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3707 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3730 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3662 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3684 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2713 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/D-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3731 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3830 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3942 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4118 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4145 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4193 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4243 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3887 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4032 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3992 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3775 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3928 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1431 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1920 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2088 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1714 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1911 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2075 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3832 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3873 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3838 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2019 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2320 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2378 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3950 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3814 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3980 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3782 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3912 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3843 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3854 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3904 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3791 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3749 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3913 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3802 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2941 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1447 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1935 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2105 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3969 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1583 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1465 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1637 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4046 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1328 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1445 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1391 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      991 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3896 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3896 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4026 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1475 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2084 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2147 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3983 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3793 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3893 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4023 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3788 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4040 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4029 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4024 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3840 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3898 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      732 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1090 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1143 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1194 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3876 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-098.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3949 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-099.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3955 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-100.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4005 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-101.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2016 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-102.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2404 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-103.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2685 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-104.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3988 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-105.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-106.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1332 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-107.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2080 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-108.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2020 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-109.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3996 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-110.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1414 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-111.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4018 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-112.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4137 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-113.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4154 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-114.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3997 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-115.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-116.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3998 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-117.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4130 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-118.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4023 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-119.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4106 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-120.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3951 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-121.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-122.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-123.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4084 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-124.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1332 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-125.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4109 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-126.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1015 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-127.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4103 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-128.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4167 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-129.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4063 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-130.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4143 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-131.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-132.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      774 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-133.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      773 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-134.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      827 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-135.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4154 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-136.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4119 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-137.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4019 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-138.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-139.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3962 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-140.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4168 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-141.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1154 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-142.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4175 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-143.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1091 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-144.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4192 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-145.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4028 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-146.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4144 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-147.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4141 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-148.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4030 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-149.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3970 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-150.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4048 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-151.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      757 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-152.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4154 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-153.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4117 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-154.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4058 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-155.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      707 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-156.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4160 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-157.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4077 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-158.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4265 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-159.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-160.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4963 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/F-161.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1770 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1346 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2614 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1564 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1399 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2433 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2445 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3491 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      984 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4005 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      996 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1109 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1303 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1458 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3817 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1298 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3195 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3140 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3856 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1420 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1549 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2643 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2724 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3885 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1004 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1003 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3965 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1931 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1349 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2301 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Fe-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2996 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      573 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1662 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1779 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3386 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3800 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ga-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3802 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3742 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3750 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3981 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      906 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3794 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1238 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1321 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1592 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3935 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1062 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1241 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1401 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3842 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1125 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1616 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1779 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3861 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3871 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3819 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3981 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1012 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3790 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1225 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1611 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1872 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3933 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3705 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3828 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3835 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3761 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3849 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3889 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2936 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3875 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3963 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4077 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1309 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      796 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4011 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4051 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3704 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3902 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4036 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      921 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3725 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1473 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1248 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1246 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1127 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1121 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1064 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      744 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1478 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1422 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4013 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      920 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4044 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      700 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4040 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3831 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3657 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1325 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3679 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      885 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      760 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      939 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3831 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1282 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      613 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      952 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3907 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      960 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      966 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      971 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      992 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/H-097.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2916 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/He-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3966 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/He-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2863 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1435 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1852 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3173 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3006 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3761 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3889 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3805 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hf-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3021 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1458 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3104 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3790 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1116 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1132 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1197 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3901 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      740 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3814 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1050 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1045 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1104 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Hg-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3733 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3840 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1439 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1621 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1793 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3923 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1554 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1614 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1666 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3869 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3825 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1430 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2013 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2077 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3815 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3857 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3895 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3850 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3904 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3052 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      697 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      949 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3103 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3959 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3962 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1028 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1449 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1395 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3934 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      959 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3851 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      841 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1132 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1196 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3858 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3822 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1156 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1825 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1889 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3952 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1262 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1031 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1340 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1395 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      673 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3856 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3868 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      986 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1413 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      441 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3917 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4017 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      439 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      558 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      612 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4006 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1263 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1041 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1319 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4019 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4035 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/I-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3029 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      471 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1020 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3163 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3787 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3757 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3795 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1085 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3686 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1288 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1308 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1661 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2141 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2217 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1026 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1142 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2121 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2304 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4138 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1466 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2067 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2125 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/K-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2917 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Kr-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Kr-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2872 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      896 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1338 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1520 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3268 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3795 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3765 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3780 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3820 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2031 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2649 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2694 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3940 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1298 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3953 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1845 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2761 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2830 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2273 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2775 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2949 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1024 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1459 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2125 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2306 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4130 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2158 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2210 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      950 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Li-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3013 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1297 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1322 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1356 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3226 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2582 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3187 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3233 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3775 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2036 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2131 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2405 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2161 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2773 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2837 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1821 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1810 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1876 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1476 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2193 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2804 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2878 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1946 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3858 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2175 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2782 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2850 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2185 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2792 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2864 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1592 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2475 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2538 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1791 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2062 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3140 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3087 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mg-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mn-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1465 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mn-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mn-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2101 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mn-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3374 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mn-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3829 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mn-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2958 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1771 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3287 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3049 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3761 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3896 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3852 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3838 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      981 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      983 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      983 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1156 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1458 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1521 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3958 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1604 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1596 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2369 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2316 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Mo-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2187 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3961 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3791 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3733 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3899 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3791 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3865 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3829 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3725 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3873 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3878 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3917 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2876 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2882 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2929 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2210 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2589 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3886 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3821 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3767 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3822 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4005 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      543 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      509 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      595 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3947 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3728 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3894 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1910 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/N-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2934 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      920 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1050 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1255 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3186 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3792 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3758 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3798 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3852 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1387 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3838 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1648 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1941 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2306 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1828 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1902 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1030 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1128 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      841 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      808 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      887 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2114 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2389 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4131 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1367 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1748 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1734 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2123 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1461 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2040 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2101 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      759 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1166 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1115 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Na-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2866 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1727 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3263 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2965 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3793 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3903 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3806 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1790 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2033 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1964 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3848 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2109 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2034 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2283 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3956 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1724 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3394 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3470 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Nb-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2914 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ne-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3964 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ne-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2856 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1563 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2196 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2129 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3491 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3860 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3803 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1298 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2292 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2346 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3879 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1197 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1295 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1252 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1324 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2545 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2715 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      746 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ni-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3807 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3654 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1057 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1169 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1586 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1853 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3767 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3881 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2278 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3210 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3269 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3847 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3845 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1720 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1655 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2913 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3073 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3820 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-022.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1776 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-023.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2317 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-024.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2369 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-025.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3823 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-026.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3846 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-027.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3795 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-028.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-029.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3938 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-030.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3784 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-031.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3944 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-032.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      893 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-033.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3760 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-034.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1880 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-035.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      801 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-036.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1531 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-037.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2940 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-038.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3086 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-039.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3943 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-040.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3957 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-041.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1393 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-042.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1757 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-043.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2673 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-044.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2613 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-045.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-046.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-047.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3763 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-048.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1891 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-049.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1896 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-050.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1898 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-051.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2493 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-052.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3392 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-053.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3462 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-054.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3960 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-055.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3709 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-056.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1462 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-057.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-058.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2259 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-059.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2456 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-060.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2628 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-061.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2116 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-062.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2742 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-063.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-064.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2170 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-065.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2065 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-066.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2225 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-067.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3932 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-068.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1478 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-069.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1120 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-070.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1646 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-071.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2117 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-072.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1751 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-073.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2133 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-074.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2310 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-075.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3940 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-076.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2054 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-077.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3406 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-078.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3489 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-079.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1238 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-080.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1743 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-081.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2798 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-082.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2999 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-083.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1217 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-084.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2134 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-085.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2214 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-086.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4181 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-087.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4128 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-088.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1675 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-089.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2827 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-090.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2777 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-091.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4201 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-092.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4230 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-093.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1175 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-094.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4260 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-095.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4299 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/O-096.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2875 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      937 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1254 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1468 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      872 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      876 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      870 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3909 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3764 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3722 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3218 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1365 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1982 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2036 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/P-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3011 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1046 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1780 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1769 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3330 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3778 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1217 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1387 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1446 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3833 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Pb-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3031 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      627 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1081 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1197 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3149 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3786 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3755 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3682 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rb-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rn-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3888 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Rn-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2746 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      724 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      948 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1123 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1325 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3804 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3903 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3682 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3842 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1972 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-010.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-011.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3172 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-012.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1332 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-013.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1437 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-014.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1386 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-015.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3688 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-016.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3713 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-017.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-018.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-019.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3877 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-020.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4049 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/S-021.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2974 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1476 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2545 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2497 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3545 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3862 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3801 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3897 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3913 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Si-009.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2890 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      989 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      967 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1777 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1960 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3275 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3803 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Sr-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2858 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2004 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3191 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2823 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3884 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3925 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3813 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ta-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2851 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1097 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1530 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2663 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2580 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3569 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3863 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3812 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Ti-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2974 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1520 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2697 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2480 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3569 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3864 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3810 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/V-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2944 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2506 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3138 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2945 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3874 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3927 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3799 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/W-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2915 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Xe-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3914 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Xe-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3017 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      776 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1418 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1385 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3189 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3836 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3758 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zn-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2849 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-001.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1101 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-002.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1565 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-003.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3140 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-004.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3020 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-005.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3735 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-006.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3892 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-007.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3809 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf/Zr-008.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    61498 2022-07-15 07:34:22.000000 chemcat-0.3.9/chemcat/data/janaf_conversion.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)   255474 2022-07-27 09:22:34.000000 chemcat-0.3.9/chemcat/data/thermo_build_cea.dat
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      471 2022-07-27 09:22:34.000000 chemcat-0.3.9/chemcat/data/white_pages.txt
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.386498 chemcat-0.3.9/chemcat/janaf/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      478 2024-01-05 21:24:42.000000 chemcat-0.3.9/chemcat/janaf/__init__.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    12470 2024-01-05 21:24:42.000000 chemcat-0.3.9/chemcat/janaf/janaf.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    11751 2024-05-21 08:34:32.000000 chemcat-0.3.9/chemcat/network.py
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.386498 chemcat-0.3.9/chemcat/utils/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      478 2024-01-05 21:24:42.000000 chemcat-0.3.9/chemcat/utils/__init__.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    32602 2024-01-05 21:24:42.000000 chemcat-0.3.9/chemcat/utils/utils.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      163 2024-05-21 08:34:32.000000 chemcat-0.3.9/chemcat/version.py
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.390498 chemcat-0.3.9/chemcat.egg-info/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    22692 2024-05-21 08:35:16.000000 chemcat-0.3.9/chemcat.egg-info/PKG-INFO
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    54136 2024-05-21 08:35:16.000000 chemcat-0.3.9/chemcat.egg-info/SOURCES.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)        1 2024-05-21 08:35:16.000000 chemcat-0.3.9/chemcat.egg-info/dependency_links.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)       87 2024-05-21 08:35:16.000000 chemcat-0.3.9/chemcat.egg-info/requires.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)        8 2024-05-21 08:35:16.000000 chemcat-0.3.9/chemcat.egg-info/top_level.txt
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.390498 chemcat-0.3.9/docs/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    16384 2024-05-21 08:02:12.000000 chemcat-0.3.9/docs/.conf.py.swp
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     7493 2022-07-15 07:34:22.000000 chemcat-0.3.9/docs/Makefile
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    41431 2024-05-21 08:34:32.000000 chemcat-0.3.9/docs/api.rst
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)  1639135 2024-05-21 08:34:32.000000 chemcat-0.3.9/docs/chemistry_tutorial.ipynb
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     7925 2022-07-31 16:01:48.000000 chemcat-0.3.9/docs/chemistry_tutorial.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    12089 2024-05-21 08:34:32.000000 chemcat-0.3.9/docs/conf.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2970 2022-07-15 07:34:22.000000 chemcat-0.3.9/docs/contributing.rst
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    11694 2024-05-21 08:34:32.000000 chemcat-0.3.9/docs/database_tutorial.ipynb
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3657 2022-07-31 16:01:48.000000 chemcat-0.3.9/docs/database_tutorial.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)       39 2024-05-21 08:34:32.000000 chemcat-0.3.9/docs/docs_requirements.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     2798 2024-05-21 08:34:32.000000 chemcat-0.3.9/docs/get_started.rst
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     3266 2024-05-17 15:25:39.000000 chemcat-0.3.9/docs/index.rst
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    16405 2024-01-05 21:24:42.000000 chemcat-0.3.9/docs/license.rst
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     1036 2024-01-08 14:04:24.000000 chemcat-0.3.9/pyproject.toml
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)       67 2022-07-27 09:22:34.000000 chemcat-0.3.9/requirements.txt
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)       38 2024-05-21 08:35:16.390498 chemcat-0.3.9/setup.cfg
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      870 2024-01-08 14:04:24.000000 chemcat-0.3.9/setup.py
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.390498 chemcat-0.3.9/src_c/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     6387 2024-01-05 21:24:42.000000 chemcat-0.3.9/src_c/_thermo.c
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     4201 2024-01-05 21:24:42.000000 chemcat-0.3.9/src_c/_utils.c
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.390498 chemcat-0.3.9/src_c/include/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)      810 2024-01-05 21:24:42.000000 chemcat-0.3.9/src_c/include/ind.h
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    10644 2024-01-05 21:24:42.000000 chemcat-0.3.9/src_c/include/newton_raphson.h
+drwxr-xr-x   0 pcubillos (914016776) iwf-pp   (914013294)        0 2024-05-21 08:35:16.390498 chemcat-0.3.9/tests/
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    28301 2024-01-05 21:24:42.000000 chemcat-0.3.9/tests/conftest.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)     6300 2024-01-05 21:24:42.000000 chemcat-0.3.9/tests/test_cea.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    11098 2024-01-05 21:24:42.000000 chemcat-0.3.9/tests/test_janaf.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    14784 2024-01-05 21:24:42.000000 chemcat-0.3.9/tests/test_network.py
+-rw-r--r--   0 pcubillos (914016776) iwf-pp   (914013294)    13208 2024-01-05 21:24:42.000000 chemcat-0.3.9/tests/test_utils.py
```

### Comparing `chemcat-0.3.8b1/.github/workflows/python-package.yml` & `chemcat-0.3.9/.github/workflows/python-package.yml`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
         include:
           - python-version: "3.6"
             os: ubuntu-20.04
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
```

### Comparing `chemcat-0.3.8b1/LICENSE` & `chemcat-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/PKG-INFO` & `chemcat-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemcat
-Version: 0.3.8b1
+Version: 0.3.9
 Summary: Chemistry Calculator for Atmospheres
 Author-email: Patricio Cubillos <pcubillos@fulbrightmail.org>, Jasmina Blecic <jasmina@nyu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -375,16 +375,16 @@
 
 
 ### Docs at:
 <https://chemcat.readthedocs.io/en/latest/>
 
 ### Cite as:
 ```bibtex
-@ARTICLE{CubillosBlecicEtal2022journalRadiativeChemicalEquilibrium,
+@ARTICLE{CubillosBlecicEtal2024journalRadiativeChemicalEquilibrium,
        author = {{Cubillos}, Patricio and {Blecic}, Jasmina and {Fossati}, Luca},
         title = "{Radiative and Chemical Equilibrium Calculations with Application to Exoplanets}",
       journal = {journal},
-         year = 2022,
-       adsurl = {https://ui.adsabs.harvard.edu/abs/2022journ.000....0C},
+         year = 2024,
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2024journ.000....0C},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
```

### Comparing `chemcat-0.3.8b1/README.md` & `chemcat-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 
 ### Docs at:
 <https://chemcat.readthedocs.io/en/latest/>
 
 ### Cite as:
 ```bibtex
-@ARTICLE{CubillosBlecicEtal2022journalRadiativeChemicalEquilibrium,
+@ARTICLE{CubillosBlecicEtal2024journalRadiativeChemicalEquilibrium,
        author = {{Cubillos}, Patricio and {Blecic}, Jasmina and {Fossati}, Luca},
         title = "{Radiative and Chemical Equilibrium Calculations with Application to Exoplanets}",
       journal = {journal},
-         year = 2022,
-       adsurl = {https://ui.adsabs.harvard.edu/abs/2022journ.000....0C},
+         year = 2024,
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2024journ.000....0C},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
```

### Comparing `chemcat-0.3.8b1/chemcat/__init__.py` & `chemcat-0.3.9/chemcat/__init__.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/cea/cea.py` & `chemcat-0.3.9/chemcat/cea/cea.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,16 @@
     t_coeffs: 1D float ndarray
         Temperature intervals of validity for each set of coefficients.
 
     Returns
     -------
     heat: Callable
         A function heat(temperature) that evaluates the molar heat
-        capacity, cp(T)/R, for a given temperature input
+        capacity at constant pressure (divided by the universal gas
+        constant), cp(T)/R, for a given temperature input
         (which can be a single value or a 1D iterable).
 
     Examples
     --------
     >>> import chemcat.cea as cea
 
     >>> data = cea.read_thermo_build(['H2O'])[0]
@@ -203,16 +204,15 @@
     [4.04063805 4.96614188 6.8342561 ]
     """
     def heat(temperature):
         if not isinstance(temperature, Iterable):
             temperature = [temperature]
         temperature = np.array(temperature, np.double)
 
-        heat_capacity = u.heat(
-            temperature, a_coeffs, t_coeffs)
+        heat_capacity = u.heat(temperature, a_coeffs, t_coeffs)
         return heat_capacity
     return heat
 
 
 def gibbs_func(a_coeffs, b_coeffs, t_coeffs):
     """
     Generate a callable that evaluates the Gibbs free energy
```

### Comparing `chemcat-0.3.8b1/chemcat/data/asplund_2009_solar_abundances.dat` & `chemcat-0.3.9/chemcat/data/asplund_2009_solar_abundances.dat`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/asplund_2021_solar_abundances.dat` & `chemcat-0.3.9/chemcat/data/asplund_2021_solar_abundances.dat`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-098.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-098.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-099.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-099.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-100.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-100.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-101.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-101.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-102.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-102.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-103.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-103.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-104.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-104.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-105.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-105.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-106.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-106.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-107.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-107.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-108.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-108.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-109.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-109.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-110.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-110.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-111.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-111.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Al-112.txt` & `chemcat-0.3.9/chemcat/data/janaf/Al-112.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ar-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ar-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ar-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ar-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-098.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-098.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-099.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-099.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-100.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-100.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-101.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-101.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-102.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-102.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-103.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-103.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-104.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-104.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-105.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-105.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-106.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-106.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-107.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-107.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-108.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-108.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-109.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-109.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-110.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-110.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-111.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-111.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-112.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-112.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-113.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-113.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-114.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-114.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-115.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-115.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-116.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-116.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-117.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-117.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-118.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-118.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-119.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-119.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-120.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-120.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-121.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-121.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-122.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-122.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-123.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-123.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-124.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-124.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-125.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-125.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-126.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-126.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-127.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-127.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-128.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-128.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-129.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-129.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-130.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-130.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-131.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-131.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-132.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-132.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-133.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-133.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-134.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-134.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-135.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-135.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-136.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-136.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-137.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-137.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-138.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-138.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-139.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-139.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/B-140.txt` & `chemcat-0.3.9/chemcat/data/janaf/B-140.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ba-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ba-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Be-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/Be-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-098.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-098.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-099.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-099.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-100.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-100.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-101.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-101.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-102.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-102.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-103.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-103.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-104.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-104.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-105.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-105.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-106.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-106.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-107.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-107.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-108.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-108.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-109.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-109.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-110.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-110.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-111.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-111.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-112.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-112.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Br-113.txt` & `chemcat-0.3.9/chemcat/data/janaf/Br-113.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-098.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-098.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-099.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-099.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-100.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-100.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-101.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-101.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-102.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-102.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-103.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-103.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-104.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-104.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-105.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-105.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-106.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-106.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-107.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-107.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-108.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-108.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-109.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-109.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-110.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-110.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-111.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-111.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-112.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-112.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-113.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-113.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-114.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-114.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-115.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-115.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-116.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-116.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-117.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-117.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-118.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-118.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-119.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-119.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-120.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-120.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-121.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-121.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-122.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-122.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-123.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-123.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-124.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-124.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-125.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-125.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-126.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-126.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-127.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-127.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-128.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-128.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-129.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-129.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-130.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-130.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-131.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-131.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-132.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-132.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-133.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-133.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-134.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-134.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-135.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-135.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-136.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-136.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-137.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-137.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-138.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-138.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-139.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-139.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-140.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-140.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-141.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-141.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-142.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-142.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-143.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-143.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-144.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-144.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-145.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-145.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-146.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-146.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-147.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-147.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-148.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-148.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-149.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-149.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-150.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-150.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/C-151.txt` & `chemcat-0.3.9/chemcat/data/janaf/C-151.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ca-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ca-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-098.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-098.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-099.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-099.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-100.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-100.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-101.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-101.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-102.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-102.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-103.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-103.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-104.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-104.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-105.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-105.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-106.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-106.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-107.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-107.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-108.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-108.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-109.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-109.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-110.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-110.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-111.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-111.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-112.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-112.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-113.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-113.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-114.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-114.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-115.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-115.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-116.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-116.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-117.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-117.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-118.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-118.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-119.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-119.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-120.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-120.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-121.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-121.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-122.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-122.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-123.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-123.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-124.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-124.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-125.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-125.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-126.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-126.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-127.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-127.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-128.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-128.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-129.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-129.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-130.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-130.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-131.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-131.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-132.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-132.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-133.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-133.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-134.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-134.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-135.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-135.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-136.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-136.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-137.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-137.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-138.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-138.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-139.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-139.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-140.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-140.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-141.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-141.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-142.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-142.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-143.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-143.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-144.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-144.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-145.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-145.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-146.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-146.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-147.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-147.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-148.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-148.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-149.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-149.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-150.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-150.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-151.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-151.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-152.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-152.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-153.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-153.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-154.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-154.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-155.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-155.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-156.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-156.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-157.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-157.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-158.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-158.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-159.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-159.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-160.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-160.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-161.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-161.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-162.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-162.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-163.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-163.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-164.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-164.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-165.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-165.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-166.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-166.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-167.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-167.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-168.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-168.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-169.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-169.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-170.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-170.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-171.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-171.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-172.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-172.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-173.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-173.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-174.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-174.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-175.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-175.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-176.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-176.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-177.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-177.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-178.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-178.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-179.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-179.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-180.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-180.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-181.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-181.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-182.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-182.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-183.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-183.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-184.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-184.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-185.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-185.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-186.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-186.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-187.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-187.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-188.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-188.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-189.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-189.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-190.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-190.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-191.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-191.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-192.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-192.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-193.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-193.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cl-194.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cl-194.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Co-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Co-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cr-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cr-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cs-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cs-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Cu-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Cu-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/D-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/D-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-098.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-098.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-099.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-099.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-100.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-100.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-101.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-101.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-102.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-102.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-103.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-103.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-104.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-104.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-105.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-105.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-106.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-106.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-107.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-107.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-108.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-108.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-109.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-109.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-110.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-110.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-111.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-111.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-112.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-112.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-113.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-113.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-114.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-114.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-115.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-115.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-116.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-116.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-117.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-117.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-118.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-118.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-119.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-119.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-120.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-120.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-121.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-121.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-122.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-122.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-123.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-123.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-124.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-124.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-125.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-125.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-126.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-126.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-127.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-127.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-128.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-128.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-129.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-129.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-130.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-130.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-131.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-131.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-132.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-132.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-133.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-133.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-134.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-134.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-135.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-135.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-136.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-136.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-137.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-137.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-138.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-138.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-139.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-139.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-140.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-140.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-141.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-141.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-142.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-142.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-143.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-143.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-144.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-144.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-145.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-145.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-146.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-146.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-147.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-147.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-148.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-148.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-149.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-149.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-150.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-150.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-151.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-151.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-152.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-152.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-153.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-153.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-154.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-154.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-155.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-155.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-156.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-156.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-157.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-157.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-158.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-158.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-159.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-159.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-160.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-160.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/F-161.txt` & `chemcat-0.3.9/chemcat/data/janaf/F-161.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Fe-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Fe-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ga-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ga-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/H-097.txt` & `chemcat-0.3.9/chemcat/data/janaf/H-097.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/He-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/He-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/He-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/He-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hf-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hf-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Hg-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Hg-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/I-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/I-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/K-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/K-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Kr-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Kr-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Kr-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Kr-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Li-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Li-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mg-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mg-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mn-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mn-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mn-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mn-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mn-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mn-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mn-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mn-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mn-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mn-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mn-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mn-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Mo-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Mo-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/N-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/N-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Na-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/Na-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Nb-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Nb-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ne-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ne-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ne-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ne-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ni-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ni-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-022.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-022.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-023.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-023.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-024.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-024.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-025.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-025.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-026.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-026.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-027.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-027.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-028.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-028.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-029.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-029.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-030.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-030.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-031.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-031.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-032.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-032.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-033.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-033.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-034.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-034.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-035.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-035.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-036.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-036.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-037.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-037.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-038.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-038.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-039.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-039.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-040.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-040.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-041.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-041.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-042.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-042.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-043.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-043.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-044.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-044.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-045.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-045.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-046.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-046.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-047.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-047.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-048.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-048.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-049.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-049.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-050.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-050.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-051.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-051.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-052.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-052.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-053.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-053.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-054.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-054.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-055.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-055.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-056.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-056.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-057.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-057.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-058.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-058.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-059.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-059.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-060.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-060.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-061.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-061.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-062.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-062.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-063.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-063.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-064.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-064.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-065.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-065.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-066.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-066.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-067.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-067.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-068.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-068.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-069.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-069.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-070.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-070.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-071.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-071.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-072.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-072.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-073.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-073.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-074.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-074.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-075.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-075.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-076.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-076.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-077.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-077.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-078.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-078.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-079.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-079.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-080.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-080.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-081.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-081.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-082.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-082.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-083.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-083.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-084.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-084.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-085.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-085.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-086.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-086.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-087.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-087.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-088.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-088.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-089.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-089.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-090.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-090.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-091.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-091.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-092.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-092.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-093.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-093.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-094.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-094.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-095.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-095.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/O-096.txt` & `chemcat-0.3.9/chemcat/data/janaf/O-096.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/P-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/P-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Pb-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/Pb-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rb-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rb-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rn-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rn-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Rn-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Rn-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-010.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-010.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-011.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-011.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-012.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-012.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-013.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-013.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-014.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-014.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-015.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-015.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-016.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-016.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-017.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-017.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-018.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-018.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-019.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-019.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-020.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-020.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/S-021.txt` & `chemcat-0.3.9/chemcat/data/janaf/S-021.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Si-009.txt` & `chemcat-0.3.9/chemcat/data/janaf/Si-009.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Sr-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Sr-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ta-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ta-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Ti-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Ti-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/V-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/V-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/W-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/W-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Xe-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Xe-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Xe-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Xe-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zn-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zn-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-001.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-001.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-002.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-002.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-003.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-003.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-004.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-004.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-005.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-005.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-006.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-006.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-007.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-007.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf/Zr-008.txt` & `chemcat-0.3.9/chemcat/data/janaf/Zr-008.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/janaf_conversion.txt` & `chemcat-0.3.9/chemcat/data/janaf_conversion.txt`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/data/thermo_build_cea.dat` & `chemcat-0.3.9/chemcat/data/thermo_build_cea.dat`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/janaf/janaf.py` & `chemcat-0.3.9/chemcat/janaf/janaf.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat/network.py` & `chemcat-0.3.9/chemcat/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,16 +209,17 @@
             self.e_scale,
             self.e_ratio,
         )
 
 
     def heat_capacity(self, temperature=None):
         """
-        Evaluate the heat capacity of each species in the network
-        at the given temperature (default to self.temperature if needed).
+        Compute Cp/R(temperature) for each species in the network,
+        where Cp is the molar heat capacity at constant pressure and
+        R is the universal gas constant (8.31 J mol-1 K-1).
         """
         if temperature is None:
             temperature = self.temperature
         return u.thermo_eval(temperature, self._heat_capacity)
 
 
     def gibbs_free_energy(self, temperature=None):
```

### Comparing `chemcat-0.3.8b1/chemcat/utils/utils.py` & `chemcat-0.3.9/chemcat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/chemcat.egg-info/PKG-INFO` & `chemcat-0.3.9/chemcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemcat
-Version: 0.3.8b1
+Version: 0.3.9
 Summary: Chemistry Calculator for Atmospheres
 Author-email: Patricio Cubillos <pcubillos@fulbrightmail.org>, Jasmina Blecic <jasmina@nyu.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -375,16 +375,16 @@
 
 
 ### Docs at:
 <https://chemcat.readthedocs.io/en/latest/>
 
 ### Cite as:
 ```bibtex
-@ARTICLE{CubillosBlecicEtal2022journalRadiativeChemicalEquilibrium,
+@ARTICLE{CubillosBlecicEtal2024journalRadiativeChemicalEquilibrium,
        author = {{Cubillos}, Patricio and {Blecic}, Jasmina and {Fossati}, Luca},
         title = "{Radiative and Chemical Equilibrium Calculations with Application to Exoplanets}",
       journal = {journal},
-         year = 2022,
-       adsurl = {https://ui.adsabs.harvard.edu/abs/2022journ.000....0C},
+         year = 2024,
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2024journ.000....0C},
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
```

### Comparing `chemcat-0.3.8b1/chemcat.egg-info/SOURCES.txt` & `chemcat-0.3.9/chemcat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1816,24 +1816,23 @@
 chemcat/data/janaf/Zr-006.txt
 chemcat/data/janaf/Zr-007.txt
 chemcat/data/janaf/Zr-008.txt
 chemcat/janaf/__init__.py
 chemcat/janaf/janaf.py
 chemcat/utils/__init__.py
 chemcat/utils/utils.py
+docs/.conf.py.swp
 docs/Makefile
 docs/api.rst
 docs/chemistry_tutorial.ipynb
 docs/chemistry_tutorial.py
-docs/chemistry_tutorial.rst
 docs/conf.py
 docs/contributing.rst
 docs/database_tutorial.ipynb
 docs/database_tutorial.py
-docs/database_tutorial.rst
 docs/docs_requirements.txt
 docs/get_started.rst
 docs/index.rst
 docs/license.rst
 src_c/_thermo.c
 src_c/_utils.c
 src_c/include/ind.h
```

### Comparing `chemcat-0.3.8b1/docs/Makefile` & `chemcat-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/docs/api.rst` & `chemcat-0.3.9/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _api:
+
 API
 ===
 
 
 chemcat
 _______
```

### Comparing `chemcat-0.3.8b1/docs/chemistry_tutorial.py` & `chemcat-0.3.9/docs/chemistry_tutorial.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/docs/conf.py` & `chemcat-0.3.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.mathjax',
     'sphinx.ext.viewcode',
+    'IPython.sphinxext.ipython_console_highlighting',
+#    'sphinx.ext.autosectionlabel',
+    'nbsphinx',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -68,15 +71,15 @@
 release = chemcat.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
 
@@ -112,20 +115,23 @@
 #todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'sphinx_rtd_theme'
+#html_theme = 'sphinx_rtd_theme'
+html_theme = 'furo'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+html_theme_options = {
+    "sidebar_hide_name": False,
+}
 
 # Add any paths that contain custom themes here, relative to this directory.
 #html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 #html_title = None
@@ -143,29 +149,42 @@
 #html_favicon = 'figures/favicon.ico'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+#html_css_files = [
+#    'css/custom.css',
+#]
+
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 #html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 #html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 #html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-html_sidebars = {'*':['globaltoc.html', 'relations.html', 'searchbox.html']}
+#html_sidebars = {
+#    "**": [
+#        "sidebar/scroll-start.html",
+#        "sidebar/brand.html",
+#        "sidebar/search.html",
+#        "sidebar/navigation.html",
+#        "sidebar/ethical-ads.html",
+#        "sidebar/scroll-end.html",
+#    ]
+#}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 #html_additional_pages = {}
 
 # If false, no module index is generated.
 #html_domain_indices = True
```

### Comparing `chemcat-0.3.8b1/docs/contributing.rst` & `chemcat-0.3.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/docs/database_tutorial.ipynb` & `chemcat-0.3.9/docs/database_tutorial.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9563517501017501%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'\\n\'), (3, \'\\n\'), (4, \'<div class="alert '*

 * *            'alert-info">\\n\'), (5, \'\\n\'), (6, \'You can also find this tutorial as a [Python '*

 * *            'scrip '*

 * *            "here](https://github.com/AtmoLib/chemcat/blob/main/docs/database_tutorial.py)\\n'), "*

 * *            "(7, 'or as a [jupyter notebook "*

 * *            "here](https://github.com/AtmoLib/chemcat/blob/main/docs/database_tutorial.ipynb).\\n'), "*

 * *            "(8, '\\n'), (9, '</div>\\n'), (10, ' […]*

```diff
@@ -4,14 +4,23 @@
             "cell_type": "markdown",
             "id": "ae76c7b3",
             "metadata": {},
             "source": [
                 "# Databases Tutorial\n",
                 "constructing the right chemical network is not easy, particularly finding which species exist in the thermodynamic databases is not trivial (until now).  This tutorial shows how to look up for all available chemical species in the JANAF or CEA databases, searching by atoms, atomic numbers, total number of atoms, and charge.\n",
                 "\n",
+                "\n",
+                "<div class=\"alert alert-info\">\n",
+                "\n",
+                "You can also find this tutorial as a [Python scrip here](https://github.com/AtmoLib/chemcat/blob/main/docs/database_tutorial.py)\n",
+                "or as a [jupyter notebook here](https://github.com/AtmoLib/chemcat/blob/main/docs/database_tutorial.ipynb).\n",
+                "\n",
+                "</div>\n",
+                "\n",
+                "\n",
                 "Let's start off importing the necessary modules:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "a574f6ab",
@@ -23,15 +32,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2922c392",
             "metadata": {},
             "source": [
-                "## Look up by Atom\n",
+                "## Look up by atom\n",
                 "To search for species containing specific atoms call the `find_species()` function with a list of the atomic species requested:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "c6e5ec15",
@@ -57,22 +66,14 @@
                 "print(f'JANAF salts with any amount of sodium:\\n{janaf_salts}')\n",
                 "\n",
                 "cea_salts = cea.find_species(['Na'])\n",
                 "print(f'\\nCEA salts with any amount of sodium:\\n{cea_salts}')"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "bcf5d2ed",
-            "metadata": {},
-            "source": [
-                "Multiple atomic species can be requested:"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 3,
             "id": "47c7111f",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
@@ -83,28 +84,29 @@
                         "\n",
                         "CEA salts with any amount of sodium and oxigen:\n",
                         "['NaNO2' 'NaNO3' 'NaO' 'NaOH' 'Na2O' 'Na2O2' 'Na2O2H2']\n"
                     ]
                 }
             ],
             "source": [
+                "# Multiple atomic species can be requested\n",
                 "# Get all sodium- and oxigen-bearing species:\n",
                 "janaf_sodium_oxide = janaf.find_species(['Na', 'O'])\n",
                 "print(f'JANAF salts with any amount of sodium and oxygen:\\n{janaf_sodium_oxide}')\n",
                 "\n",
                 "cea_sodium_oxide = cea.find_species(['Na', 'O'])\n",
                 "print(f'\\nCEA salts with any amount of sodium and oxigen:\\n{cea_sodium_oxide}')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e06f8843",
             "metadata": {},
             "source": [
-                "## Look up by Atomic Number\n",
+                "## Look up by atomic number\n",
                 "To search for species containing specific atoms call the `find_species()` function with a dict of the atomic species requested and their atomic values:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "27408546",
@@ -129,22 +131,14 @@
                 "print(f'JANAF salts with one sodium atom:\\n{janaf_salts1}')\n",
                 "\n",
                 "cea_salts1 = cea.find_species({'Na':1})\n",
                 "print(f'\\nCEA salts with one sodium atom:\\n{cea_salts1}')"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "bda3db5b",
-            "metadata": {},
-            "source": [
-                "Another example:"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 5,
             "id": "d53c2b92",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
@@ -155,31 +149,24 @@
                         "\n",
                         "CEA salts with two sodium atoms:\n",
                         "['Na2' 'Na2O' 'Na2O2' 'Na2O2H2']\n"
                     ]
                 }
             ],
             "source": [
+                "# Another example:\n",
                 "# Get species containing exactly two Na atoms:\n",
                 "janaf_salts2 = janaf.find_species({'Na':2})\n",
                 "print(f'JANAF salts with two sodium atoms:\\n{janaf_salts2}')\n",
                 "\n",
                 "cea_salts2 = cea.find_species({'Na':2})\n",
                 "print(f'\\nCEA salts with two sodium atoms:\\n{cea_salts2}')"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "303c27f8",
-            "metadata": {},
-            "source": [
-                "Use `None` as atomic number to request any non-zero amount of atoms for a given species:"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 6,
             "id": "968d0a61",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
@@ -193,28 +180,29 @@
                         " 'HO(CO)2OH' 'C2H3,vinyl' 'CH3CN' 'CH3CO,acetyl' 'C2H4' 'C2H4O,ethylen-o'\n",
                         " 'CH3CHO,ethanal' 'CH3COOH' 'OHCH2COOH' 'C2H5' 'C2H6' 'CH3N2CH3' 'C2H5OH'\n",
                         " 'CH3OCH3' 'CH3O2CH3' 'HCCN' 'HCCO' '(HCOOH)2']\n"
                     ]
                 }
             ],
             "source": [
+                "# Use None as atomic number to request any non-zero amount of atoms for a given species:\n",
                 "# Species containing exactly two carbon atoms and any amount of hydrogen:\n",
                 "janaf_ethane = janaf.find_species({'H':None, 'C':2})\n",
                 "print(f'JANAF ethane hydrocarbons:\\n{janaf_ethane}')\n",
                 "\n",
                 "cea_ethane = cea.find_species({'H':None, 'C':2})\n",
                 "print(f'\\nCEA ethane hydrocarbons:\\n{cea_ethane}')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ba8b9d5e",
             "metadata": {},
             "source": [
-                "## Look up by Number of Total Atoms\n",
+                "## Look up by number of atoms\n",
                 "To search for species containing a specific number of atoms call the `find_species()` function with the `num_atoms` argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "5c364d19",
@@ -245,15 +233,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4827f83e",
             "metadata": {},
             "source": [
-                "## Look up Ionic Species\n",
+                "## Look up ionic species\n",
                 "So far we have seen only neutral species, if we want to look up for charged species we need to call the `find_species()` function with the `charge` argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "2d335823",
@@ -296,22 +284,14 @@
                 "print(f'\\nNeutral JANAF sulfuric species:\\n{janaf_sulfur_neutral}')\n",
                 "\n",
                 "janaf_sulfur_ions = janaf.find_species(['S'], charge='ion')\n",
                 "print(f'\\nCharged JANAF sulfuric species:\\n{janaf_sulfur_ions}')"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "de6a60d4",
-            "metadata": {},
-            "source": [
-                "Now the same look up, but for CEA:"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 9,
             "id": "ca053fb8",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
@@ -329,41 +309,42 @@
                         "\n",
                         "Charged CEA sulfuric species:\n",
                         "['S+' 'S-' 'SH-' 'SO-' 'SO2-' 'S2-']\n"
                     ]
                 }
             ],
             "source": [
+                "# Now the same look up, but for CEA:\n",
                 "# Look up sulfuric species in CEA:\n",
                 "cea_sulfur = cea.find_species(['S'], charge='all')\n",
                 "print(f'All CEA sulfuric species:\\n{cea_sulfur}')\n",
                 "\n",
                 "cea_sulfur_neutral = cea.find_species(['S'], charge='neutral')\n",
                 "print(f'\\nNeutral CEA sulfuric species:\\n{cea_sulfur_neutral}')\n",
                 "\n",
                 "cea_sulfur_ions = cea.find_species(['S'], charge='ion')\n",
                 "print(f'\\nCharged CEA sulfuric species:\\n{cea_sulfur_ions}')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "py39",
+            "display_name": "py310",
             "language": "python",
-            "name": "py39"
+            "name": "py310"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `chemcat-0.3.8b1/docs/database_tutorial.py` & `chemcat-0.3.9/docs/database_tutorial.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/docs/get_started.rst` & `chemcat-0.3.9/docs/get_started.rst`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
   He) relative to the solar metallicity.
 * Setting the abundance of individual/custom elements.
 * Setting the abundance of individual/custom elements as elemental
   ratios (e.g., C/O, Na/H, etc.).
 
 ``chemcat`` also provides an interface to access the NIST-JANAF and
 NASA-ThermoBuild databases of thermochemical properties (see section
-:ref:`tutorial_databases`).
+`Database Tutorial <database_tutorial.ipynb>`_).
 
 Take a look at the :ref:`quick_example` section to get up to speed in
-computing ``chemcat``.  The :ref:`tutorial` section showcases the
+computing ``chemcat``.  The `Chemistry Tutorial <./chemistry_tutorial.ipynb>`_ section showcases the
 multiple ways in which ``chemcat`` enables a parameterization of the
 atmospheric composition.
 
 
 System Requirements
 -------------------
 
@@ -85,11 +85,11 @@
     temperature = np.tile(1200.0, nlayers)
     pressure = np.logspace(-8, 3, nlayers)
     molecules = 'H2O CH4 CO CO2 NH3 N2 H2 HCN OH C2H2 C2H4 H He C N O'.split()
 
     net = cat.Network(pressure, temperature, molecules)
     vmr = net.thermochemical_equilibrium()
 
-See section :ref:`tutorial` for an in-depth tutorial of the
+See section `Chemistry Tutorial <./chemistry_tutorial.ipynb>`_ for an in-depth tutorial of the
 ``chemcat`` capabilities.
 Additionally, all low-and mid-level routines can be found in the
 package's :ref:`API`.
```

### Comparing `chemcat-0.3.8b1/docs/index.rst` & `chemcat-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/docs/license.rst` & `chemcat-0.3.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/src_c/_thermo.c` & `chemcat-0.3.9/src_c/_thermo.c`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/src_c/_utils.c` & `chemcat-0.3.9/src_c/_utils.c`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/src_c/include/ind.h` & `chemcat-0.3.9/src_c/include/ind.h`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/src_c/include/newton_raphson.h` & `chemcat-0.3.9/src_c/include/newton_raphson.h`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/tests/conftest.py` & `chemcat-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/tests/test_cea.py` & `chemcat-0.3.9/tests/test_cea.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/tests/test_janaf.py` & `chemcat-0.3.9/tests/test_janaf.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/tests/test_network.py` & `chemcat-0.3.9/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `chemcat-0.3.8b1/tests/test_utils.py` & `chemcat-0.3.9/tests/test_utils.py`

 * *Files identical despite different names*

