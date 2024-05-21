# Comparing `tmp/promg-1.0.9.tar.gz` & `tmp/promg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promg-1.0.9.tar", last modified: Mon Mar  4 09:04:17 2024, max compression
+gzip compressed data, was "C:\Users\s156229\PycharmProjects\promg-core\dist\.tmp-6ahnxpk9\promg-1.1.0.tar", last modified: Tue May 21 07:29:56 2024, max compression
```

## Comparing `promg-1.0.9.tar` & `promg-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.008238 promg-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-04 09:04:11.000000 promg-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-04 09:04:17.008238 promg-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-04 09:04:11.000000 promg-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 09:04:17.008238 promg-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-04 09:04:11.000000 promg-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.000238 promg-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.000238 promg-1.0.9/src/promg/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/cypher_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/data_importer_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/db_managment_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/exporter_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/inference_engine_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/process_discovery_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/semantic_header_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/task_identification_ql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/data_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/data_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/data_managers/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)    46016 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/data_managers/semantic_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/database_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/remote_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/facades/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/facades/oced_pg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/data_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/db_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/ekg_builder_semantic_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/process_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/task_identification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.008238 promg-1.0.9/src/promg/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/auxiliary_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/context_manager_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/get_db_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/performance_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.008238 promg-1.0.9/src/promg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/
+-rw-rw-rw-   0        0        0     7817 2023-04-24 11:35:40.000000 promg-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1219 2024-05-21 07:29:56.000000 promg-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-09-20 15:57:09.000000 promg-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:29:56.000000 promg-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2024-01-23 12:57:42.000000 promg-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:55.000000 promg-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg/
+-rw-rw-rw-   0        0        0      648 2024-01-23 12:57:42.000000 promg-1.1.0/src/promg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/cypher_queries/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/cypher_queries/__init__.py
+-rw-rw-rw-   0        0        0    11660 2024-03-04 09:07:40.000000 promg-1.1.0/src/promg/cypher_queries/data_importer_ql.py
+-rw-rw-rw-   0        0        0     9567 2024-05-16 12:04:22.000000 promg-1.1.0/src/promg/cypher_queries/db_managment_ql.py
+-rw-rw-rw-   0        0        0      942 2024-03-04 09:14:44.000000 promg-1.1.0/src/promg/cypher_queries/exporter_ql.py
+-rw-rw-rw-   0        0        0     5837 2023-09-18 13:27:26.000000 promg-1.1.0/src/promg/cypher_queries/inference_engine_ql.py
+-rw-rw-rw-   0        0        0     3728 2023-09-18 13:27:26.000000 promg-1.1.0/src/promg/cypher_queries/process_discovery_ql.py
+-rw-rw-rw-   0        0        0    18771 2024-05-16 15:19:55.000000 promg-1.1.0/src/promg/cypher_queries/semantic_header_ql.py
+-rw-rw-rw-   0        0        0     9770 2023-09-18 13:27:26.000000 promg-1.1.0/src/promg/cypher_queries/task_identification_ql.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/data_managers/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/data_managers/__init__.py
+-rw-rw-rw-   0        0        0    32893 2024-03-25 16:01:47.000000 promg-1.1.0/src/promg/data_managers/datastructures.py
+-rw-rw-rw-   0        0        0     4541 2024-05-16 15:19:55.000000 promg-1.1.0/src/promg/data_managers/properties.py
+-rw-rw-rw-   0        0        0    43708 2024-05-16 15:19:55.000000 promg-1.1.0/src/promg/data_managers/semantic_header.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/database_managers/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/database_managers/__init__.py
+-rw-rw-rw-   0        0        0      588 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/database_managers/authentication.py
+-rw-rw-rw-   0        0        0     4851 2024-05-16 15:46:48.000000 promg-1.1.0/src/promg/database_managers/db_connection.py
+-rw-rw-rw-   0        0        0      235 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/database_managers/remote_authentication.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/facades/
+-rw-rw-rw-   0        0        0        0 2023-09-18 13:27:26.000000 promg-1.1.0/src/promg/facades/__init__.py
+-rw-rw-rw-   0        0        0     8190 2024-03-04 15:15:51.000000 promg-1.1.0/src/promg/facades/oced_pg.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/modules/
+-rw-rw-rw-   0        0        0        0 2023-09-19 11:25:17.000000 promg-1.1.0/src/promg/modules/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-05-15 14:30:21.000000 promg-1.1.0/src/promg/modules/data_importer.py
+-rw-rw-rw-   0        0        0     5455 2024-05-16 12:04:22.000000 promg-1.1.0/src/promg/modules/db_management.py
+-rw-rw-rw-   0        0        0     8796 2024-05-16 12:04:22.000000 promg-1.1.0/src/promg/modules/ekg_builder_semantic_header.py
+-rw-rw-rw-   0        0        0     3304 2024-03-04 09:07:42.000000 promg-1.1.0/src/promg/modules/exporter.py
+-rw-rw-rw-   0        0        0     4824 2024-03-04 09:07:42.000000 promg-1.1.0/src/promg/modules/inference_engine.py
+-rw-rw-rw-   0        0        0     1073 2024-03-04 09:07:43.000000 promg-1.1.0/src/promg/modules/process_discovery.py
+-rw-rw-rw-   0        0        0     2453 2024-03-04 09:07:44.000000 promg-1.1.0/src/promg/modules/task_identification.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/utilities/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2136 2024-03-04 09:06:54.000000 promg-1.1.0/src/promg/utilities/configuration.py
+-rw-rw-rw-   0        0        0     1072 2023-07-25 13:07:47.000000 promg-1.1.0/src/promg/utilities/context_manager_tqdm.py
+-rw-rw-rw-   0        0        0     1876 2023-09-10 06:55:44.000000 promg-1.1.0/src/promg/utilities/get_db_size.py
+-rw-rw-rw-   0        0        0     4192 2024-03-04 15:15:51.000000 promg-1.1.0/src/promg/utilities/performance_handling.py
+-rw-rw-rw-   0        0        0      397 2023-09-18 13:27:26.000000 promg-1.1.0/src/promg/utilities/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:56.000000 promg-1.1.0/src/promg/visualize_schema/
+-rw-rw-rw-   0        0        0        0 2024-05-14 14:45:37.000000 promg-1.1.0/src/promg/visualize_schema/__init__.py
+-rw-rw-rw-   0        0        0      846 2024-05-14 14:49:25.000000 promg-1.1.0/src/promg/visualize_schema/visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg.egg-info/
+-rw-rw-rw-   0        0        0     1219 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1619 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 07:29:55.000000 promg-1.1.0/src/promg.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `promg-1.0.9/LICENSE` & `promg-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

### Comparing `promg-1.0.9/PKG-INFO` & `promg-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-Metadata-Version: 2.1
-Name: promg
-Version: 1.0.9
-Summary: Pyhton library to build Event Knowledge Graphs
-Author: A. Swevels, D.Fahland
-License: GPL 3.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: neo4j
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: tabulate
-Requires-Dist: tqdm
-Requires-Dist: pyyaml
-
-# Documentation
-
-## Hi there 👋
-
-Over here we are developing PromG, a tool enabling you to perform multi-dimensional process analytics by exploiting a multi-layered Event Knowledge Graph.
-The repository contains the source code (PromG-core) which can be installed as a Python package using `pip install promg` and several example analyses.
-
-🎥 Demo Video: We created a demo video [here](https://www.youtube.com/watch?v=EKXFqHtW3Xw&t=6s). In this demo, we illustrate PromG on the BPIC'17 dataset.
-
-🗃️ Documentation: [https://promg-dev.github.io/promg-core/](https://promg-dev.github.io/promg-core/)
-
-🏁 Getting started: [https://promg-dev.github.io/promg-core/getting-started/](https://promg-dev.github.io/promg-core/getting-started/)
-
-🛠️ Tutorial: [https://promg-dev.github.io/promg-core/tutorials](https://promg-dev.github.io/promg-core/tutorials/)
-
-📦 Python Package: [https://pypi.org/project/promg/](https://pypi.org/project/promg/)
+Metadata-Version: 2.1
+Name: promg
+Version: 1.1.0
+Summary: Pyhton library to build Event Knowledge Graphs
+Author: A. Swevels, D.Fahland
+License: GPL 3.0
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Documentation
+
+## Hi there 👋
+
+Over here we are developing PromG, a tool enabling you to perform multi-dimensional process analytics by exploiting a multi-layered Event Knowledge Graph.
+The repository contains the source code (PromG-core) which can be installed as a Python package using `pip install promg` and several example analyses.
+
+🎥 Demo Video: We created a demo video [here](https://www.youtube.com/watch?v=EKXFqHtW3Xw&t=6s). In this demo, we illustrate PromG on the BPIC'17 dataset.
+
+🗃️ Documentation: [https://promg-dev.github.io/promg-core/](https://promg-dev.github.io/promg-core/)
+
+🏁 Getting started: [https://promg-dev.github.io/promg-core/getting-started/](https://promg-dev.github.io/promg-core/getting-started/)
+
+🛠️ Tutorial: [https://promg-dev.github.io/promg-core/tutorials](https://promg-dev.github.io/promg-core/tutorials/)
+
+📦 Python Package: [https://pypi.org/project/promg/](https://pypi.org/project/promg/)
```

### Comparing `promg-1.0.9/README.md` & `promg-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Documentation
-
-## Hi there 👋
-
-Over here we are developing PromG, a tool enabling you to perform multi-dimensional process analytics by exploiting a multi-layered Event Knowledge Graph.
-The repository contains the source code (PromG-core) which can be installed as a Python package using `pip install promg` and several example analyses.
-
-🎥 Demo Video: We created a demo video [here](https://www.youtube.com/watch?v=EKXFqHtW3Xw&t=6s). In this demo, we illustrate PromG on the BPIC'17 dataset.
-
-🗃️ Documentation: [https://promg-dev.github.io/promg-core/](https://promg-dev.github.io/promg-core/)
-
-🏁 Getting started: [https://promg-dev.github.io/promg-core/getting-started/](https://promg-dev.github.io/promg-core/getting-started/)
-
-🛠️ Tutorial: [https://promg-dev.github.io/promg-core/tutorials](https://promg-dev.github.io/promg-core/tutorials/)
-
-📦 Python Package: [https://pypi.org/project/promg/](https://pypi.org/project/promg/)
+# Documentation
+
+## Hi there 👋
+
+Over here we are developing PromG, a tool enabling you to perform multi-dimensional process analytics by exploiting a multi-layered Event Knowledge Graph.
+The repository contains the source code (PromG-core) which can be installed as a Python package using `pip install promg` and several example analyses.
+
+🎥 Demo Video: We created a demo video [here](https://www.youtube.com/watch?v=EKXFqHtW3Xw&t=6s). In this demo, we illustrate PromG on the BPIC'17 dataset.
+
+🗃️ Documentation: [https://promg-dev.github.io/promg-core/](https://promg-dev.github.io/promg-core/)
+
+🏁 Getting started: [https://promg-dev.github.io/promg-core/getting-started/](https://promg-dev.github.io/promg-core/getting-started/)
+
+🛠️ Tutorial: [https://promg-dev.github.io/promg-core/tutorials](https://promg-dev.github.io/promg-core/tutorials/)
+
+📦 Python Package: [https://pypi.org/project/promg/](https://pypi.org/project/promg/)
```

### Comparing `promg-1.0.9/setup.py` & `promg-1.1.0/setup.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import find_packages, setup
-import re
-
-# read the contents of the README file
-from pathlib import Path
-
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text(encoding="utf-8")
-
-
-VERSIONFILE=f"{this_directory}/version.md"
-verstrline = open(VERSIONFILE, "rt").read()
-VSRE = r"^# version ([\d]+.[\d]+.[\d]*)"
-mo = re.search(VSRE, verstrline, re.M)
-if mo:
-    verstr = mo.group(1)
-else:
-    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
-
-setup(
-    name='promg',
-    version=str(verstr),
-    description='Pyhton library to build Event Knowledge Graphs',
-    author='A. Swevels, D.Fahland',
-    python_requires='>=3.7',
-    install_requires=['neo4j', 'numpy', 'pandas', 'tabulate', 'tqdm', 'pyyaml'],
-    license='GPL 3.0',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    packages=find_packages(
-        where='src',
-        include=['promg*']),
-    package_dir={"": "src"}
-)
+from setuptools import find_packages, setup
+import re
+
+# read the contents of the README file
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text(encoding="utf-8")
+
+
+VERSIONFILE=f"{this_directory}/version.md"
+verstrline = open(VERSIONFILE, "rt").read()
+VSRE = r"^# version ([\d]+.[\d]+.[\d]*)"
+mo = re.search(VSRE, verstrline, re.M)
+if mo:
+    verstr = mo.group(1)
+else:
+    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
+
+setup(
+    name='promg',
+    version=str(verstr),
+    description='Pyhton library to build Event Knowledge Graphs',
+    author='A. Swevels, D.Fahland',
+    python_requires='>=3.7',
+    install_requires=['neo4j', 'numpy', 'pandas', 'tabulate', 'tqdm', 'pyyaml'],
+    license='GPL 3.0',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    packages=find_packages(
+        where='src',
+        include=['promg*']),
+    package_dir={"": "src"}
+)
```

### Comparing `promg-1.0.9/src/promg/__init__.py` & `promg-1.1.0/src/promg/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .data_managers.semantic_header import SemanticHeader
-from .database_managers.db_connection import DatabaseConnection
-
-from .facades.oced_pg import OcedPg
-from .database_managers import authentication
-from .data_managers.datastructures import DatasetDescriptions
-from .database_managers.db_connection import Query
-from .utilities.performance_handling import Performance
-from .utilities.configuration import Configuration
-
-__all__ = [SemanticHeader,
-           DatabaseConnection,
-           authentication,
-           DatasetDescriptions,
-           Query,
-           Performance,
-           OcedPg,
-           Configuration]
+from .data_managers.semantic_header import SemanticHeader
+from .database_managers.db_connection import DatabaseConnection
+
+from .facades.oced_pg import OcedPg
+from .database_managers import authentication
+from .data_managers.datastructures import DatasetDescriptions
+from .database_managers.db_connection import Query
+from .utilities.performance_handling import Performance
+from .utilities.configuration import Configuration
+
+__all__ = [SemanticHeader,
+           DatabaseConnection,
+           authentication,
+           DatasetDescriptions,
+           Query,
+           Performance,
+           OcedPg,
+           Configuration]
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/data_importer_ql.py` & `promg-1.1.0/src/promg/cypher_queries/data_importer_ql.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-from typing import Dict, Optional, List, Union
-from string import Template
-
-from ..data_managers.datastructures import DataStructure, DatetimeObject
-from ..data_managers.semantic_header import RecordConstructor
-from ..database_managers.db_connection import Query
-
-
-class DataImporterQueryLibrary:
-
-    @staticmethod
-    def create_mapping_str(mapping: str) -> str:
-        """
-        Create the string including the information of the datatypes mapping used when importing records.
-
-        :param mapping: The dtype mapping of the imported records as string
-        :return: str containing the mapping in Cypher format
-        """
-        if mapping == "":
-            return ""
-        mapping_str = ''',{nullValues: [""], mapping:$mapping}''' if mapping != "" else ""
-        mapping_str = Template(mapping_str).safe_substitute({"mapping": mapping})
-        return mapping_str
-
-    @staticmethod
-    def get_import_directory_query() -> Query:
-        """
-        Query that gets the import directory of the current running database
-
-        :return: Query object to get import directory of the current running database
-        """
-
-        # language=SQL
-        query_str = """
-            Call dbms.listConfig() YIELD name, value
-            WHERE name='server.directories.import'
-            RETURN value as directory
-        """
-
-        return Query(query_str=query_str)
-
-
-    @staticmethod
-    def get_create_nodes_by_loading_csv_query(labels: str, file_name: str, mapping: str) -> Query:
-        """
-        Create event nodes for each row in the batch with labels
-        The properties of each row are also the property of the node
-        @param mapping: The dtype mapping of the imported records as string
-        @param file_name: the name of the file to be imported
-        @param labels: The labels of the record nodes
-
-        @return: Query object to create record nodes by loading csv
-        """
-
-        # $batch is a variable we can add in tx.run, this allows us to use string properties
-        # (keys in our dictionary are string)
-        # return is required when using call and yield
-        # language=SQL
-        query_str = '''
-                    CALL apoc.periodic.iterate('
-                        CALL apoc.load.csv("$file_name" $mapping_str) yield map as row return row',
-                        'CREATE (record:$labels)
-                        SET record += row'
-                    , {batchSize:10000, parallel:true, retries: 1});                    
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "file_name": file_name,
-                         "labels": labels,
-                         "mapping_str": DataImporterQueryLibrary.create_mapping_str(mapping)
-                     })
-
-    @staticmethod
-    def get_make_timestamp_date_query(required_labels_str: str, attribute: str, datetime_object: DatetimeObject,
-                                      load_status: int) -> Query:
-        """
-        Create a query to convert the strings of the timestamp to the datetime as used in Neo4j
-        Remove the str_timestamp property
-
-        @param required_labels_str: the required labels of the just imported nodes
-        @param attribute: the name of the attribute that should be converted
-        @param datetime_object: the DatetimeObject describing how the attribute should be converted
-        @param load_status: the current load status of the records that are being imported
-
-        @return: Query object to convert the timestamps string into timestamp objects
-
-        """
-        offset = datetime_object.timezone_offset
-        offset = f'{attribute}+"{offset}"' if offset != "" else attribute
-
-        # language=SQL
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                'MATCH (r:$required_labels) 
-                USING INDEX r:Record(loadStatus)
-                WHERE r.$attribute IS NOT NULL AND r.loadStatus = $load_status 
-                AND NOT apoc.meta.cypher.isType(r.$attribute, "$date_type")
-                WITH r, r.$offset as timezone_dt
-                WITH r, datetime(apoc.date.convertFormat(timezone_dt, "$datetime_object_format", 
-                    "$datetime_object_convert_to")) as converted
-                RETURN r, converted',
-                'SET r.$attribute = converted',
-                {batchSize:$batch_size, parallel:true})
-            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "required_labels": required_labels_str,
-                         "datetime_object_format": datetime_object.format,
-                         "datetime_object_convert_to": datetime_object.convert_to,
-                         "date_type": datetime_object.get_date_type(),
-                         "attribute": attribute,
-                         "offset": offset,
-                         "load_status": load_status
-                     })
-
-    @staticmethod
-    def get_convert_epoch_to_timestamp_query(required_labels_str: str, attribute: str, datetime_object: DatetimeObject,
-                                             load_status: int) -> Query:
-        """
-        Create a query to convert epoch timestamp to the datetime as used in Neo4j
-        Remove the str_timestamp property
-
-        @param required_labels_str: the required labels of the just imported nodes
-        @param attribute: the name of the attribute that should be converted
-        @param datetime_object: the DatetimeObject describing how the attribute should be converted
-        @param load_status: the current load status of the records that are being imported
-
-        @return: Query object to convert the epoch timestamps into timestamp objects
-
-        """
-
-        # language=SQL
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                'MATCH (r:$required_labels) 
-                USING INDEX r:Record(loadStatus)
-                WHERE r.$attribute IS NOT NULL AND r.loadStatus = $load_status 
-                WITH r, r.$attribute as timezone_dt
-                WITH r, apoc.date.format(timezone_dt, $unit, 
-                    $dt_format) as converted
-                RETURN r, converted',
-                'SET r.$attribute = converted',
-                {batchSize:$batch_size, parallel:false, 
-                params: {unit: $unit,
-                        dt_format: $datetime_object_format}})
-            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "attribute": attribute,
-                         "required_labels": required_labels_str
-                     },
-                     parameters={
-                         "unit": datetime_object.unit,
-                         "datetime_object_format": datetime_object.format,
-                         "load_status": load_status
-                     })
-
-    @staticmethod
-    def get_finalize_import_records_query(required_labels_str: str, load_status: int) -> Query:
-        """
-        Create a query to finalize the import of the record nodes, i.e. remove the load status
-
-        @param required_labels_str: the required labels of the just imported nodes
-        @param load_status: the current load status of the records that are being imported
-
-        @return: Query object to remove the load status attribute of the just imported nodes
-
-        """
-
-        # language=SQL
-        query_str = '''
-            CALL apoc.periodic.commit(
-                'MATCH (r:$required_labels) 
-                USING INDEX r:Record(loadStatus)
-                WHERE r.loadStatus = $load_status
-                WITH r LIMIT $limit
-                REMOVE r.loadStatus
-                RETURN count(*)',
-                {limit:$batch_size, load_status:$load_status})
-            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={"required_labels": required_labels_str},
-                     parameters={
-                         "load_status": load_status
-                     }
-                     )
-
-    @staticmethod
-    def get_filter_records_by_property_query(prop: str, load_status: int, values: Optional[List[str]] = None,
-                                             exclude: bool = True, required_labels_str="Record") -> Query:
-        """
-        Create a query to remove nodes and their relationships if they have (exlude) or have not (include) a certain
-        attribute or a certain attribute-value pairs.
-
-        @param prop: the name of the property
-        @param load_status: the current load status of the records that are being imported
-        @param values: a list of values that the property should (not) have for being removed
-        @param exclude: boolean indicating whether nodes should be removed if they match the criteria (exclude=True)
-        or be kept (exclude = False)
-        @param required_labels_str: the labels the nodes should have
-
-        @return: Query object to remove the load status attribute of the just imported nodes
-
-        """
-
-        if values is None:  # match all events that have a specific property
-            negation = "NOT" if exclude else ""
-            # query to delete all records and its relationship with property
-            # language=SQL
-            query_str = '''
-                    MATCH (r:$required_labels {loadStatus: $load_status})
-                    WHERE r.$prop IS $negation NULL
-                    DETACH DELETE r
-                    '''
-            template_string_parameters = {"prop": prop, "negation": negation}
-        else:  # match all events with specific property and value
-            negation = "" if exclude else "NOT"
-            # match all r and delete them and its relationship
-            # language=SQL
-            query_str = '''
-                    MATCH (r:$required_labels {loadStatus: $load_status})
-                    WHERE $negation r.$prop IN $values
-                    DETACH DELETE r
-                '''
-            template_string_parameters = {
-                "prop": prop,
-                "negation": negation,
-                "values": values,
-                "load_status": load_status,
-                "required_labels": required_labels_str
-            }
-
-        # execute query
-        return Query(query_str=query_str,
-                     template_string_parameters=template_string_parameters)
-
-    @staticmethod
-    def get_update_load_status_query(current_load_status: int):
-        """
-        Create a query to update the record nodes that match the current load status with 1
-
-        @param current_load_status: the current load status of the records that are being imported
-
-        @return: Query object that updates the Record nodes that match the current load status with 1
-
-        """
-
-        query_str = '''
-        CALL apoc.periodic.commit(
-            'MATCH (record:Record) 
-            WHERE record.loadStatus = $old_value
-            WITH record LIMIT $limit
-            SET record.loadStatus = record.loadStatus + 1
-            RETURN COUNT(*)',
-            {old_value: $old_value,
-            limit: $batch_size})
-                            '''
-        return Query(query_str=query_str,
-                     parameters={
-                         "old_value": current_load_status
-                     })
+from typing import Dict, Optional, List, Union
+from string import Template
+
+from ..data_managers.datastructures import DataStructure, DatetimeObject
+from ..data_managers.semantic_header import RecordConstructor
+from ..database_managers.db_connection import Query
+
+
+class DataImporterQueryLibrary:
+
+    @staticmethod
+    def create_mapping_str(mapping: str) -> str:
+        """
+        Create the string including the information of the datatypes mapping used when importing records.
+
+        :param mapping: The dtype mapping of the imported records as string
+        :return: str containing the mapping in Cypher format
+        """
+        if mapping == "":
+            return ""
+        mapping_str = ''',{nullValues: [""], mapping:$mapping}''' if mapping != "" else ""
+        mapping_str = Template(mapping_str).safe_substitute({"mapping": mapping})
+        return mapping_str
+
+    @staticmethod
+    def get_import_directory_query() -> Query:
+        """
+        Query that gets the import directory of the current running database
+
+        :return: Query object to get import directory of the current running database
+        """
+
+        # language=SQL
+        query_str = """
+            Call dbms.listConfig() YIELD name, value
+            WHERE name='server.directories.import'
+            RETURN value as directory
+        """
+
+        return Query(query_str=query_str)
+
+
+    @staticmethod
+    def get_create_nodes_by_loading_csv_query(labels: str, file_name: str, mapping: str) -> Query:
+        """
+        Create event nodes for each row in the batch with labels
+        The properties of each row are also the property of the node
+        @param mapping: The dtype mapping of the imported records as string
+        @param file_name: the name of the file to be imported
+        @param labels: The labels of the record nodes
+
+        @return: Query object to create record nodes by loading csv
+        """
+
+        # $batch is a variable we can add in tx.run, this allows us to use string properties
+        # (keys in our dictionary are string)
+        # return is required when using call and yield
+        # language=SQL
+        query_str = '''
+                    CALL apoc.periodic.iterate('
+                        CALL apoc.load.csv("$file_name" $mapping_str) yield map as row return row',
+                        'CREATE (record:$labels)
+                        SET record += row'
+                    , {batchSize:10000, parallel:true, retries: 1});                    
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "file_name": file_name,
+                         "labels": labels,
+                         "mapping_str": DataImporterQueryLibrary.create_mapping_str(mapping)
+                     })
+
+    @staticmethod
+    def get_make_timestamp_date_query(required_labels_str: str, attribute: str, datetime_object: DatetimeObject,
+                                      load_status: int) -> Query:
+        """
+        Create a query to convert the strings of the timestamp to the datetime as used in Neo4j
+        Remove the str_timestamp property
+
+        @param required_labels_str: the required labels of the just imported nodes
+        @param attribute: the name of the attribute that should be converted
+        @param datetime_object: the DatetimeObject describing how the attribute should be converted
+        @param load_status: the current load status of the records that are being imported
+
+        @return: Query object to convert the timestamps string into timestamp objects
+
+        """
+        offset = datetime_object.timezone_offset
+        offset = f'{attribute}+"{offset}"' if offset != "" else attribute
+
+        # language=SQL
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                'MATCH (r:$required_labels) 
+                USING INDEX r:Record(loadStatus)
+                WHERE r.$attribute IS NOT NULL AND r.loadStatus = $load_status 
+                AND NOT apoc.meta.cypher.isType(r.$attribute, "$date_type")
+                WITH r, r.$offset as timezone_dt
+                WITH r, datetime(apoc.date.convertFormat(timezone_dt, "$datetime_object_format", 
+                    "$datetime_object_convert_to")) as converted
+                RETURN r, converted',
+                'SET r.$attribute = converted',
+                {batchSize:$batch_size, parallel:true})
+            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "required_labels": required_labels_str,
+                         "datetime_object_format": datetime_object.format,
+                         "datetime_object_convert_to": datetime_object.convert_to,
+                         "date_type": datetime_object.get_date_type(),
+                         "attribute": attribute,
+                         "offset": offset,
+                         "load_status": load_status
+                     })
+
+    @staticmethod
+    def get_convert_epoch_to_timestamp_query(required_labels_str: str, attribute: str, datetime_object: DatetimeObject,
+                                             load_status: int) -> Query:
+        """
+        Create a query to convert epoch timestamp to the datetime as used in Neo4j
+        Remove the str_timestamp property
+
+        @param required_labels_str: the required labels of the just imported nodes
+        @param attribute: the name of the attribute that should be converted
+        @param datetime_object: the DatetimeObject describing how the attribute should be converted
+        @param load_status: the current load status of the records that are being imported
+
+        @return: Query object to convert the epoch timestamps into timestamp objects
+
+        """
+
+        # language=SQL
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                'MATCH (r:$required_labels) 
+                USING INDEX r:Record(loadStatus)
+                WHERE r.$attribute IS NOT NULL AND r.loadStatus = $load_status 
+                WITH r, r.$attribute as timezone_dt
+                WITH r, apoc.date.format(timezone_dt, $unit, 
+                    $dt_format) as converted
+                RETURN r, converted',
+                'SET r.$attribute = converted',
+                {batchSize:$batch_size, parallel:false, 
+                params: {unit: $unit,
+                        dt_format: $datetime_object_format}})
+            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "attribute": attribute,
+                         "required_labels": required_labels_str
+                     },
+                     parameters={
+                         "unit": datetime_object.unit,
+                         "datetime_object_format": datetime_object.format,
+                         "load_status": load_status
+                     })
+
+    @staticmethod
+    def get_finalize_import_records_query(required_labels_str: str, load_status: int) -> Query:
+        """
+        Create a query to finalize the import of the record nodes, i.e. remove the load status
+
+        @param required_labels_str: the required labels of the just imported nodes
+        @param load_status: the current load status of the records that are being imported
+
+        @return: Query object to remove the load status attribute of the just imported nodes
+
+        """
+
+        # language=SQL
+        query_str = '''
+            CALL apoc.periodic.commit(
+                'MATCH (r:$required_labels) 
+                USING INDEX r:Record(loadStatus)
+                WHERE r.loadStatus = $load_status
+                WITH r LIMIT $limit
+                REMOVE r.loadStatus
+                RETURN count(*)',
+                {limit:$batch_size, load_status:$load_status})
+            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={"required_labels": required_labels_str},
+                     parameters={
+                         "load_status": load_status
+                     }
+                     )
+
+    @staticmethod
+    def get_filter_records_by_property_query(prop: str, load_status: int, values: Optional[List[str]] = None,
+                                             exclude: bool = True, required_labels_str="Record") -> Query:
+        """
+        Create a query to remove nodes and their relationships if they have (exlude) or have not (include) a certain
+        attribute or a certain attribute-value pairs.
+
+        @param prop: the name of the property
+        @param load_status: the current load status of the records that are being imported
+        @param values: a list of values that the property should (not) have for being removed
+        @param exclude: boolean indicating whether nodes should be removed if they match the criteria (exclude=True)
+        or be kept (exclude = False)
+        @param required_labels_str: the labels the nodes should have
+
+        @return: Query object to remove the load status attribute of the just imported nodes
+
+        """
+
+        if values is None:  # match all events that have a specific property
+            negation = "NOT" if exclude else ""
+            # query to delete all records and its relationship with property
+            # language=SQL
+            query_str = '''
+                    MATCH (r:$required_labels {loadStatus: $load_status})
+                    WHERE r.$prop IS $negation NULL
+                    DETACH DELETE r
+                    '''
+            template_string_parameters = {"prop": prop, "negation": negation}
+        else:  # match all events with specific property and value
+            negation = "" if exclude else "NOT"
+            # match all r and delete them and its relationship
+            # language=SQL
+            query_str = '''
+                    MATCH (r:$required_labels {loadStatus: $load_status})
+                    WHERE $negation r.$prop IN $values
+                    DETACH DELETE r
+                '''
+            template_string_parameters = {
+                "prop": prop,
+                "negation": negation,
+                "values": values,
+                "load_status": load_status,
+                "required_labels": required_labels_str
+            }
+
+        # execute query
+        return Query(query_str=query_str,
+                     template_string_parameters=template_string_parameters)
+
+    @staticmethod
+    def get_update_load_status_query(current_load_status: int):
+        """
+        Create a query to update the record nodes that match the current load status with 1
+
+        @param current_load_status: the current load status of the records that are being imported
+
+        @return: Query object that updates the Record nodes that match the current load status with 1
+
+        """
+
+        query_str = '''
+        CALL apoc.periodic.commit(
+            'MATCH (record:Record) 
+            WHERE record.loadStatus = $old_value
+            WITH record LIMIT $limit
+            SET record.loadStatus = record.loadStatus + 1
+            RETURN COUNT(*)',
+            {old_value: $old_value,
+            limit: $batch_size})
+                            '''
+        return Query(query_str=query_str,
+                     parameters={
+                         "old_value": current_load_status
+                     })
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/db_managment_ql.py` & `promg-1.1.0/src/promg/cypher_queries/db_managment_ql.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,216 +1,271 @@
-from ..data_managers.semantic_header import ConstructedNodes
-from ..database_managers.db_connection import Query
-
-
-class DBManagementQueryLibrary:
-    @staticmethod
-    def get_all_rel_types_query() -> Query:
-        # find all relations and return the distinct types
-
-        # language=SQL
-        query_str = '''
-                MATCH () - [rel] - () RETURN DISTINCT type(rel) AS rel_type
-            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_all_node_labels_query() -> Query:
-        # find all nodes and return the distinct labels
-
-        # language=SQL
-        query_str = '''
-            MATCH (n) RETURN DISTINCT labels(n) AS label
-        '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_clear_db_query(db_name) -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE OR REPLACE DATABASE $db_name
-            WAIT
-        '''
-
-        return Query(query_str=query_str, database="system", template_string_parameters={"db_name": db_name})
-
-    @staticmethod
-    def get_delete_relationships_query() -> Query:
-        # language=SQL
-        query_str = '''
-                    CALL apoc.periodic.iterate(
-                        "MATCH () - [r] -> () return id(r) as id", 
-                        "MATCH () - [r] -> () WHERE id(r) = id DELETE r", 
-                        {batchSize:$batch_size})
-                    yield batches, total 
-                    RETURN batches, total
-                '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_delete_nodes_query() -> Query:
-        # language=SQL
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                    "MATCH (n) return id(n) as id", 
-                    "MATCH (n) WHERE id(n) = id DETACH DELETE n", {batchSize:$batch_size})
-                yield batches, total 
-                RETURN batches, total
-            '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_replace_db_query(db_name) -> Query:
-        # language=SQL
-        query_str = '''
-                    CREATE OR REPLACE DATABASE $db_name
-                    WAIT
-                '''
-
-        return Query(query_str=query_str, database="system", template_string_parameters={"db_name": db_name})
-
-    @staticmethod
-    def get_constraint_unique_event_id_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE CONSTRAINT unique_event_ids IF NOT EXISTS 
-            FOR (e:Event) REQUIRE e.ID IS UNIQUE
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_constraint_unique_entity_uid_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE CONSTRAINT unique_entity_ids IF NOT EXISTS 
-            FOR (en:Entity) REQUIRE en.sysId IS UNIQUE
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_constraint_unique_log_id_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE CONSTRAINT unique_entity_ids IF NOT EXISTS 
-            FOR (l:Log) REQUIRE l.ID IS UNIQUE
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_set_sysid_index_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE INDEX entity_sys_id_index IF NOT EXISTS FOR (n:Entity) ON (n.sysId)
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_set_recordid_as_key_node_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE CONSTRAINT record_id_as_key_node IF NOT EXISTS FOR (r:Record) REQUIRE (r.recordId) IS NODE KEY
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_set_recordid_as_index_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE INDEX record_id_as_index IF NOT EXISTS FOR (r:Record) ON (r.recordId)
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_set_load_status_as_index_query() -> Query:
-        # language=SQL
-        query_str = '''
-            CREATE INDEX load_status_as_index IF NOT EXISTS FOR (r:Record) ON (r.loadStatus)
-        '''
-        return Query(query_str=query_str,
-                     template_string_parameters={},
-                     parameters={})
-
-    @staticmethod
-    def get_node_count_query() -> Query:
-        # language=SQL
-        query_str = '''
-                // List all node types and counts
-                MATCH (n) 
-                WITH n, CASE labels(n)[0]
-                    WHEN 'Event' THEN 0
-                    WHEN 'Entity' THEN 1
-                    WHEN 'Class' THEN 2
-                    WHEN 'Log' THEN 3
-                    ELSE 4
-                END AS sortOrder
-                WITH  labels(n)[0] AS label,  count(n) AS numberOfNodes,sortOrder
-                RETURN label,  numberOfNodes ORDER BY sortOrder
-            '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_edge_count_query() -> Query:
-        # language=SQL
-        query_str = '''
-                // List all agg rel types and counts
-                MATCH () - [r] -> ()
-                WHERE r.type is NOT NULL
-                WITH r, CASE toUpper(r.type)
-                  WHEN 'REL' THEN 0
-                  WHEN 'DF' THEN 1
-                  ELSE 2
-                END as sortOrder
-                WITH toUpper(r.type) as aggType, count(r) as aggNumberOfRelations, sortOrder
-                RETURN aggType, aggNumberOfRelations ORDER BY sortOrder
-            '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_aggregated_edge_count_query() -> Query:
-        # language=SQL
-        query_str = '''
-                // List all rel types and counts
-                MATCH () - [r] -> ()
-                // WHERE r.type is  NULL
-                WITH r, CASE Type(r)
-                  WHEN 'CORR' THEN 0
-                  WHEN 'OBSERVED' THEN 1
-                  WHEN 'HAS' THEN 2
-                  ELSE 3
-                END as sortOrder
-                WITH Type(r) as type, count(r) as numberOfRelations, sortOrder
-                RETURN type, numberOfRelations ORDER BY sortOrder
-            '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_imported_logs_query() -> Query:
-        # language = SQL
-        query_str = '''
-            MATCH (n:Record)
-            RETURN COLLECT(DISTINCT n.log) AS logs
-        '''
-
-        return Query(query_str=query_str)
+from ..data_managers.semantic_header import ConstructedNodes
+from ..database_managers.db_connection import Query
+
+
+class DBManagementQueryLibrary:
+    @staticmethod
+    def get_all_rel_types_query() -> Query:
+        # find all relations and return the distinct types
+
+        # language=SQL
+        query_str = '''
+                MATCH () - [rel] - () RETURN DISTINCT type(rel) AS rel_type
+            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_all_node_labels_query() -> Query:
+        # find all nodes and return the distinct labels
+
+        # language=SQL
+        query_str = '''
+            MATCH (n) RETURN DISTINCT labels(n) AS label
+        '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_clear_db_query(db_name) -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE OR REPLACE DATABASE $db_name
+            WAIT
+        '''
+
+        return Query(query_str=query_str, database="system", template_string_parameters={"db_name": db_name})
+
+    @staticmethod
+    def get_delete_relationships_query() -> Query:
+        # language=SQL
+        query_str = '''
+                    CALL apoc.periodic.iterate(
+                        "MATCH () - [r] -> () return id(r) as id", 
+                        "MATCH () - [r] -> () WHERE id(r) = id DELETE r", 
+                        {batchSize:$batch_size})
+                    yield batches, total 
+                    RETURN batches, total
+                '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_delete_nodes_query() -> Query:
+        # language=SQL
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                    "MATCH (n) return id(n) as id", 
+                    "MATCH (n) WHERE id(n) = id DETACH DELETE n", {batchSize:$batch_size})
+                yield batches, total 
+                RETURN batches, total
+            '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_replace_db_query(db_name) -> Query:
+        # language=SQL
+        query_str = '''
+                    CREATE OR REPLACE DATABASE $db_name
+                    WAIT
+                '''
+
+        return Query(query_str=query_str, database="system", template_string_parameters={"db_name": db_name})
+
+    @staticmethod
+    def get_constraint_unique_event_id_query() -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE CONSTRAINT unique_event_ids IF NOT EXISTS 
+            FOR (e:Event) REQUIRE e.ID IS UNIQUE
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_constraint_unique_entity_uid_query(node_type=None) -> Query:
+        if node_type is None:
+            node_type = "Entity"
+        # language=SQL
+        query_str = '''
+            CREATE CONSTRAINT $constraint_name IF NOT EXISTS 
+            FOR (en:$node_type) REQUIRE en.sysId IS UNIQUE
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "node_type": node_type,
+                         "constraint_name": f"unique_{node_type.lower()}_ids"
+                     },
+                     parameters={})
+
+    @staticmethod
+    def get_constraint_unique_log_id_query() -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE CONSTRAINT unique_entity_ids IF NOT EXISTS 
+            FOR (l:Log) REQUIRE l.ID IS UNIQUE
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_sysid_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE RANGE INDEX entity_sys_id_index IF NOT EXISTS FOR (n:Entity) ON (n.sysId)
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_activity_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+                CREATE RANGE INDEX activity_index IF NOT EXISTS FOR (a:Activity) ON (a.activity)
+            '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_activity_event_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+                CREATE RANGE INDEX activity_event_index IF NOT EXISTS FOR (e:event) ON (e.activity)
+            '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_timestamp_event_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+                CREATE RANGE INDEX timestamp_event_index IF NOT EXISTS FOR (e:event) ON (e.timestamp)
+            '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_recordid_as_key_node_query() -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE CONSTRAINT record_id_as_key_node IF NOT EXISTS FOR (r:Record) REQUIRE (r.recordId) IS NODE KEY
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_recordid_as_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE RANGE INDEX record_id_as_index IF NOT EXISTS FOR (r:Record) ON (r.recordId)
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_record_log_as_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+                CREATE RANGE INDEX record_log_as_index IF NOT EXISTS FOR (r:Record) ON (r.log)
+            '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_record_created_as_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+                    CREATE RANGE INDEX record_created_as_index IF NOT EXISTS FOR (r:Record) ON (r.created)
+                '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_set_load_status_as_index_query() -> Query:
+        # language=SQL
+        query_str = '''
+            CREATE INDEX load_status_as_index IF NOT EXISTS FOR (r:Record) ON (r.loadStatus)
+        '''
+        return Query(query_str=query_str,
+                     template_string_parameters={},
+                     parameters={})
+
+    @staticmethod
+    def get_node_count_query() -> Query:
+        # language=SQL
+        query_str = '''
+                // List all node types and counts
+                MATCH (n) 
+                WITH n, CASE labels(n)[0]
+                    WHEN 'Event' THEN 0
+                    WHEN 'Entity' THEN 1
+                    WHEN 'Class' THEN 2
+                    WHEN 'Log' THEN 3
+                    ELSE 4
+                END AS sortOrder
+                WITH  labels(n)[0] AS label,  count(n) AS numberOfNodes,sortOrder
+                RETURN label,  numberOfNodes ORDER BY sortOrder
+            '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_edge_count_query() -> Query:
+        # language=SQL
+        query_str = '''
+                // List all agg rel types and counts
+                MATCH () - [r] -> ()
+                WHERE r.type is NOT NULL
+                WITH r, CASE toUpper(r.type)
+                  WHEN 'REL' THEN 0
+                  WHEN 'DF' THEN 1
+                  ELSE 2
+                END as sortOrder
+                WITH toUpper(r.type) as aggType, count(r) as aggNumberOfRelations, sortOrder
+                RETURN aggType, aggNumberOfRelations ORDER BY sortOrder
+            '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_aggregated_edge_count_query() -> Query:
+        # language=SQL
+        query_str = '''
+                // List all rel types and counts
+                MATCH () - [r] -> ()
+                // WHERE r.type is  NULL
+                WITH r, CASE Type(r)
+                  WHEN 'CORR' THEN 0
+                  WHEN 'OBSERVED' THEN 1
+                  WHEN 'HAS' THEN 2
+                  ELSE 3
+                END as sortOrder
+                WITH Type(r) as type, count(r) as numberOfRelations, sortOrder
+                RETURN type, numberOfRelations ORDER BY sortOrder
+            '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_imported_logs_query() -> Query:
+        # language = SQL
+        query_str = '''
+            MATCH (n:Record)
+            RETURN COLLECT(DISTINCT n.log) AS logs
+        '''
+
+        return Query(query_str=query_str)
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/exporter_ql.py` & `promg-1.1.0/src/promg/cypher_queries/exporter_ql.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from ..data_managers.semantic_header import ConstructedNodes
-from ..database_managers.db_connection import Query
-
-
-class ExporterQueryLibrary:
-
-    @staticmethod
-    def get_event_log_query(entity: ConstructedNodes, additional_event_attributes) -> Query:
-        query_str = '''
-                MATCH (e:Event) - [:CORR] -> (n:$node_label)
-                RETURN n.sysId as caseId, e.activity as activity, e.timestamp as timestamp $extra_attributes
-                ORDER BY n.ID, e.timestamp
-            '''
-
-        attributes_query = ",".join(f"e.{attribute} as {attribute}" for attribute in additional_event_attributes)
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "node_label": entity.get_label_string(),
-                         "extra_attributes": f", {attributes_query}" if len(additional_event_attributes) > 0 else ""
-                     })
+from ..data_managers.semantic_header import ConstructedNodes
+from ..database_managers.db_connection import Query
+
+
+class ExporterQueryLibrary:
+
+    @staticmethod
+    def get_event_log_query(entity: ConstructedNodes, additional_event_attributes) -> Query:
+        query_str = '''
+                MATCH (e:Event) - [:CORR] -> (n:$node_label)
+                RETURN n.sysId as caseId, e.activity as activity, e.timestamp as timestamp $extra_attributes
+                ORDER BY n.ID, e.timestamp
+            '''
+
+        attributes_query = ",".join(f"e.{attribute} as {attribute}" for attribute in additional_event_attributes)
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "node_label": entity.get_label_string(),
+                         "extra_attributes": f", {attributes_query}" if len(additional_event_attributes) > 0 else ""
+                     })
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/inference_engine_ql.py` & `promg-1.1.0/src/promg/cypher_queries/inference_engine_ql.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from ..data_managers.semantic_header import ConstructedNodes
-from ..database_managers.db_connection import Query
-
-
-class InferenceEngineQueryLibrary:
-    @staticmethod
-    def get_query_infer_items_propagate_upwards_multiple_levels(entity: ConstructedNodes, is_load=True) -> Query:
-        # language=sql
-        query_str = '''
-                MATCH (f2:Event) - [:CORR] -> (n:$entity)
-                MATCH (f2) - [:CORR] ->  (equipment:Equipment)
-                MATCH (f2) - [:OBSERVED] -> (a2:Activity) - [:AT] -> (l:Location) - [:PART_OF*0..] -> (k:Location) 
-                WITH f2, k, equipment, n
-                CALL {WITH f2, k, equipment
-                    MATCH (f0:Event) - [:OBSERVED] -> (a0: Activity)
-                    MATCH (a0) - [:$operation_type] -> (et:EntityType {name: '$entity'})  
-                    MATCH (a0) - [:AT] -> (k)
-                    MATCH (f0) - [:CORR] ->  (equipment)
-                    WHERE f0.timestamp $comparison f2.timestamp
-                    RETURN f0 as f0_first
-                    ORDER BY f0.timestamp $order_type
-                    LIMIT 1}
-                MERGE (f0_first) - [:CORR] -> (n)
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity": entity.type,
-                         "operation_type": "LOADS" if is_load else "UNLOADS",
-                         "comparison": "<=" if is_load else ">=",
-                         "order_type": "DESC" if is_load else ""
-                     })
-
-    @staticmethod
-    def get_query_infer_items_propagate_downwards_multiple_level_w_batching(entity: ConstructedNodes,
-                                                                            relative_position: ConstructedNodes) -> \
-            Query:
-        # language=sql
-        query_str = '''
-                MATCH (f2:Event) - [:CORR] -> (bp:$relative_position)
-                MATCH (f2) - [:CORR] -> (equipment :Equipment)
-                MATCH (f2) - [:OBSERVED] -> (a2:Activity) -[:AT]-> (l:Location) - [:PART_OF*0..] -> (k:Location) 
-                // ensure f2 should have operated on the required by checking that the activity operates on that entity
-                MATCH (a2) - -> (:EntityType {name: '$entity'}) 
-                WITH f2, equipment, k, bp
-                CALL {WITH f2, equipment, k
-                    MATCH (f0: Event)-[:OBSERVED]->(a0:Activity) - [:LOADS] ->  (:EntityType {name: '$entity'})
-                    MATCH (a0) - [:AT] -> (k)
-                    MATCH (f0)-[:CORR]->(resource)
-                    WHERE f0.timestamp <= f2.timestamp
-                    // find the first preceding f0
-                    RETURN f0 as f0_first_prec
-                    ORDER BY f0.timestamp DESC
-                    LIMIT 1
-                }
-                // only merge when f0_first_prec is actually related to the required entity
-                WITH f2, [(f0_first_prec)-[:CORR]->(n:$entity)- [:AT_POS] -> (bp) | n] as related_n
-                FOREACH (n in related_n | 
-                    MERGE (f2) - [:CORR] -> (n)
-                )
-            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity": entity.type,
-                         "relative_position": relative_position.type
-                     })
-
-    @staticmethod
-    def get_query_infer_items_propagate_downwards_one_level(entity: ConstructedNodes) -> Query:
-        # language=sql
-        query_str = '''
-                        MATCH (f1 :Event) - [:CORR] -> (equipment :Equipment)
-                        MATCH (f1) - [:OBSERVED] -> (a1:Activity) -[:AT]-> (l:Location)
-                        // ensure f2 should have operated on the required by checking that the activity operates on 
-                        that  
-                        entity
-                        MATCH (a1) - -> (:EntityType {name: '$entity'}) 
-                        WITH f1, equipment, l
-                        CALL {WITH f1, equipment, l
-                            MATCH (f0: Event)-[:OBSERVED]->(a0:Activity) - [:LOADS] -> (:EntityType {name: '$entity'})
-                            MATCH (a0) - [:AT] -> (l)
-                            MATCH (f0)-[:CORR]->(equipment)
-                            WHERE f0.timestamp <= f1.timestamp
-                            // find the first preceding f0
-                            RETURN f0 as f0_first_prec
-                            ORDER BY f0.timestamp DESC
-                            LIMIT 1
-                        }
-                        // only merge when f0_first_prec is actually related to a Box
-                        WITH f1, [(f0_first_prec)-[:CORR]->(n:$entity) | n] as related_n
-                        FOREACH (n in related_n | 
-                            MERGE (f1) - [:CORR] -> (n)
-                        )
-                        '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity": entity.type
-                     })
-
-    @staticmethod
-    def get_match_entity_with_batch_position_query(entity: ConstructedNodes, relative_position: ConstructedNodes) -> Query:
-        # language=sql
-        query_str = '''
-                    MATCH (e:Event) - [:CORR] -> (b:Box)
-                    MATCH (e) - [:CORR] -> (bp:$relative_position)
-                    MERGE (b:Box) - [:AT_POS] -> (bp:$relative_position)
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity": entity.type,
-                         "relative_position": relative_position.type
-                     })
+from ..data_managers.semantic_header import ConstructedNodes
+from ..database_managers.db_connection import Query
+
+
+class InferenceEngineQueryLibrary:
+    @staticmethod
+    def get_query_infer_items_propagate_upwards_multiple_levels(entity: ConstructedNodes, is_load=True) -> Query:
+        # language=sql
+        query_str = '''
+                MATCH (f2:Event) - [:CORR] -> (n:$entity)
+                MATCH (f2) - [:CORR] ->  (equipment:Equipment)
+                MATCH (f2) - [:OBSERVED] -> (a2:Activity) - [:AT] -> (l:Location) - [:PART_OF*0..] -> (k:Location) 
+                WITH f2, k, equipment, n
+                CALL {WITH f2, k, equipment
+                    MATCH (f0:Event) - [:OBSERVED] -> (a0: Activity)
+                    MATCH (a0) - [:$operation_type] -> (et:EntityType {name: '$entity'})  
+                    MATCH (a0) - [:AT] -> (k)
+                    MATCH (f0) - [:CORR] ->  (equipment)
+                    WHERE f0.timestamp $comparison f2.timestamp
+                    RETURN f0 as f0_first
+                    ORDER BY f0.timestamp $order_type
+                    LIMIT 1}
+                MERGE (f0_first) - [:CORR] -> (n)
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity": entity.type,
+                         "operation_type": "LOADS" if is_load else "UNLOADS",
+                         "comparison": "<=" if is_load else ">=",
+                         "order_type": "DESC" if is_load else ""
+                     })
+
+    @staticmethod
+    def get_query_infer_items_propagate_downwards_multiple_level_w_batching(entity: ConstructedNodes,
+                                                                            relative_position: ConstructedNodes) -> \
+            Query:
+        # language=sql
+        query_str = '''
+                MATCH (f2:Event) - [:CORR] -> (bp:$relative_position)
+                MATCH (f2) - [:CORR] -> (equipment :Equipment)
+                MATCH (f2) - [:OBSERVED] -> (a2:Activity) -[:AT]-> (l:Location) - [:PART_OF*0..] -> (k:Location) 
+                // ensure f2 should have operated on the required by checking that the activity operates on that entity
+                MATCH (a2) - -> (:EntityType {name: '$entity'}) 
+                WITH f2, equipment, k, bp
+                CALL {WITH f2, equipment, k
+                    MATCH (f0: Event)-[:OBSERVED]->(a0:Activity) - [:LOADS] ->  (:EntityType {name: '$entity'})
+                    MATCH (a0) - [:AT] -> (k)
+                    MATCH (f0)-[:CORR]->(resource)
+                    WHERE f0.timestamp <= f2.timestamp
+                    // find the first preceding f0
+                    RETURN f0 as f0_first_prec
+                    ORDER BY f0.timestamp DESC
+                    LIMIT 1
+                }
+                // only merge when f0_first_prec is actually related to the required entity
+                WITH f2, [(f0_first_prec)-[:CORR]->(n:$entity)- [:AT_POS] -> (bp) | n] as related_n
+                FOREACH (n in related_n | 
+                    MERGE (f2) - [:CORR] -> (n)
+                )
+            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity": entity.type,
+                         "relative_position": relative_position.type
+                     })
+
+    @staticmethod
+    def get_query_infer_items_propagate_downwards_one_level(entity: ConstructedNodes) -> Query:
+        # language=sql
+        query_str = '''
+                        MATCH (f1 :Event) - [:CORR] -> (equipment :Equipment)
+                        MATCH (f1) - [:OBSERVED] -> (a1:Activity) -[:AT]-> (l:Location)
+                        // ensure f2 should have operated on the required by checking that the activity operates on 
+                        that  
+                        entity
+                        MATCH (a1) - -> (:EntityType {name: '$entity'}) 
+                        WITH f1, equipment, l
+                        CALL {WITH f1, equipment, l
+                            MATCH (f0: Event)-[:OBSERVED]->(a0:Activity) - [:LOADS] -> (:EntityType {name: '$entity'})
+                            MATCH (a0) - [:AT] -> (l)
+                            MATCH (f0)-[:CORR]->(equipment)
+                            WHERE f0.timestamp <= f1.timestamp
+                            // find the first preceding f0
+                            RETURN f0 as f0_first_prec
+                            ORDER BY f0.timestamp DESC
+                            LIMIT 1
+                        }
+                        // only merge when f0_first_prec is actually related to a Box
+                        WITH f1, [(f0_first_prec)-[:CORR]->(n:$entity) | n] as related_n
+                        FOREACH (n in related_n | 
+                            MERGE (f1) - [:CORR] -> (n)
+                        )
+                        '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity": entity.type
+                     })
+
+    @staticmethod
+    def get_match_entity_with_batch_position_query(entity: ConstructedNodes, relative_position: ConstructedNodes) -> Query:
+        # language=sql
+        query_str = '''
+                    MATCH (e:Event) - [:CORR] -> (b:Box)
+                    MATCH (e) - [:CORR] -> (bp:$relative_position)
+                    MERGE (b:Box) - [:AT_POS] -> (bp:$relative_position)
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity": entity.type,
+                         "relative_position": relative_position.type
+                     })
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/process_discovery_ql.py` & `promg-1.1.0/src/promg/cypher_queries/process_discovery_ql.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from typing import Optional, List
-from ..data_managers.semantic_header import ConstructedNodes
-from ..database_managers.db_connection import Query
-
-
-class AnalysisQueryLibrary:
-
-    @staticmethod
-    def get_aggregate_df_relations_query(entity: ConstructedNodes,
-                                         include_label_in_df_a: bool = True,
-                                         df_threshold: int = 0,
-                                         relative_df_threshold: float = 0,
-                                         exclude_self_loops=True) -> Query:
-
-        # add relations between classes when desired
-        if df_threshold == 0 and relative_df_threshold == 0:
-            # corresponds to aggregate_df_relations &  aggregate_df_relations_for_entities in graphdb-event-logs
-            # aggregate only for a specific entity type and event classifier
-
-            # language=sql
-            query_str = '''
-                                MATCH 
-                                (c1:Activity) -[:OBSERVED]-> (e1:Event) 
-                                    -[df:$df_label {entityType: '$entity_type'}]-> 
-                                (e2:Event) <-  [:OBSERVED] - (c2:Activity)
-                                $classifier_self_loops
-                                WITH c1, count(df) AS df_freq,c2
-                                MERGE 
-                                (c1) 
-                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_A'}]-> 
-                                (c2) 
-                                ON CREATE SET rel2.count=df_freq'''
-        else:
-            # aggregate only for a specific entity type and event classifier
-            # include only edges with a minimum threshold, drop weak edges (similar to heuristics miner)
-
-            # language=sql
-            query_str = '''
-                                MATCH 
-                                (c1:Activity) 
-                                    -[:OBSERVED]->
-                                (e1:Event) 
-                                    -[df:$df_label {entityType: '$entity_type'}]-> 
-                                (e2:Event) <-[:OBSERVED]- (c2:Activity)
-                                MATCH (e1) -[:CORR] -> (n) <-[:CORR]- (e2)
-                                $classifier_self_loops
-                                WITH c1,count(df) AS df_freq,c2
-                                WHERE df_freq > $df_threshold
-                                OPTIONAL MATCH (c2:Activity) -[:OBSERVED]-> (e2b:Event) -[df2:$df_label {entityType: 
-                                '$entity_type'}]-> 
-                                    (e1b:Event) <-[:OBSERVED]- (c2:Activity)
-                                WITH c1,df_freq,count(df2) AS df_freq2,c2
-                                WHERE (df_freq*$relative_df_threshold > df_freq2)
-                                MERGE 
-                                (c1) 
-                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_A'}]-> 
-                                (c2) 
-                                ON CREATE SET rel2.count=df_freq'''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "df_label": entity.get_df_label(),
-                         "entity_type": entity.type,
-                         "classifier_self_loops": "WHERE c1 <> c2" if exclude_self_loops else "",
-                         "dfc_label": entity.get_df_a_label(include_label_in_df_a),
-                         "df_threshold": df_threshold,
-                         "relative_df_threshold": relative_df_threshold
-                     })
+from typing import Optional, List
+from ..data_managers.semantic_header import ConstructedNodes
+from ..database_managers.db_connection import Query
+
+
+class AnalysisQueryLibrary:
+
+    @staticmethod
+    def get_aggregate_df_relations_query(entity: ConstructedNodes,
+                                         include_label_in_df_a: bool = True,
+                                         df_threshold: int = 0,
+                                         relative_df_threshold: float = 0,
+                                         exclude_self_loops=True) -> Query:
+
+        # add relations between classes when desired
+        if df_threshold == 0 and relative_df_threshold == 0:
+            # corresponds to aggregate_df_relations &  aggregate_df_relations_for_entities in graphdb-event-logs
+            # aggregate only for a specific entity type and event classifier
+
+            # language=sql
+            query_str = '''
+                                MATCH 
+                                (c1:Activity) -[:OBSERVED]-> (e1:Event) 
+                                    -[df:$df_label {entityType: '$entity_type'}]-> 
+                                (e2:Event) <-  [:OBSERVED] - (c2:Activity)
+                                $classifier_self_loops
+                                WITH c1, count(df) AS df_freq,c2
+                                MERGE 
+                                (c1) 
+                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_A'}]-> 
+                                (c2) 
+                                ON CREATE SET rel2.count=df_freq'''
+        else:
+            # aggregate only for a specific entity type and event classifier
+            # include only edges with a minimum threshold, drop weak edges (similar to heuristics miner)
+
+            # language=sql
+            query_str = '''
+                                MATCH 
+                                (c1:Activity) 
+                                    -[:OBSERVED]->
+                                (e1:Event) 
+                                    -[df:$df_label {entityType: '$entity_type'}]-> 
+                                (e2:Event) <-[:OBSERVED]- (c2:Activity)
+                                MATCH (e1) -[:CORR] -> (n) <-[:CORR]- (e2)
+                                $classifier_self_loops
+                                WITH c1,count(df) AS df_freq,c2
+                                WHERE df_freq > $df_threshold
+                                OPTIONAL MATCH (c2:Activity) -[:OBSERVED]-> (e2b:Event) -[df2:$df_label {entityType: 
+                                '$entity_type'}]-> 
+                                    (e1b:Event) <-[:OBSERVED]- (c2:Activity)
+                                WITH c1,df_freq,count(df2) AS df_freq2,c2
+                                WHERE (df_freq*$relative_df_threshold > df_freq2)
+                                MERGE 
+                                (c1) 
+                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_A'}]-> 
+                                (c2) 
+                                ON CREATE SET rel2.count=df_freq'''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "df_label": entity.get_df_label(),
+                         "entity_type": entity.type,
+                         "classifier_self_loops": "WHERE c1 <> c2" if exclude_self_loops else "",
+                         "dfc_label": entity.get_df_a_label(include_label_in_df_a),
+                         "df_threshold": df_threshold,
+                         "relative_df_threshold": relative_df_threshold
+                     })
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/semantic_header_ql.py` & `promg-1.1.0/src/promg/cypher_queries/semantic_header_ql.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,448 +1,368 @@
-from string import Template
-from typing import Union
-
-from ..data_managers.semantic_header import ConstructedNodes, NodeConstructor, Node, \
-    RelationConstructor, RecordConstructor, ConstructedRelation
-from ..database_managers.db_connection import Query
-
-
-class SemanticHeaderQueryLibrary:
-    @staticmethod
-    def get_create_node_by_record_constructor_query(node_constructor: NodeConstructor, merge=True) -> Query:
-        # find events that contain the entity as property and not nan
-        # save the value of the entity property as id and also whether it is a virtual entity
-        # create a new entity node if it not exists yet with properties
-        merge_or_create = 'MERGE' if merge else 'CREATE'
-        set_label_str = ""
-        set_property_str = ""
-        infer_corr_str = ""
-        infer_observed_str = ""
-
-        if node_constructor.set_labels is not None:
-            set_label_str = f'SET $set_labels'''
-
-        if len(node_constructor.result.optional_properties) > 0:
-            set_property_str = 'SET $set_result_properties'
-
-        if len(node_constructor.inferred_relationships) > 0:
-            infer_corr_str = '''WITH record, $result_node_name'''
-            for relationship in node_constructor.inferred_relationships:
-                infer_rel_str = '''
-                    CALL {WITH record, $result_node_name
-                            MATCH ($event_node) - [:EXTRACTED_FROM] -> (record:$record_labels) <- [:EXTRACTED_FROM] - (
-                                $result_node_name)
-                                MERGE (event) - [:$relation_type] -> ($result_node_name)}'''
-                infer_rel_str = Template(infer_rel_str).safe_substitute({
-                    "event_node": relationship.event.get_pattern(name="event"),
-                    "record_labels": relationship.get_labels_str(),
-                    "relation_type": relationship.relation_type
-                })
-                infer_corr_str += infer_rel_str
-        elif node_constructor.infer_corr_from_event_record:
-            # language=SQL
-            infer_corr_str = '''
-            WITH record, $result_node_name
-                                MATCH (event:$event_label) - [:EXTRACTED_FROM] -> (record) <- [:EXTRACTED_FROM] - (
-                                $result_node_name)
-                                MERGE (event) - [:$corr_type] -> ($result_node_name)'''
-        elif node_constructor.infer_corr_from_entity_record:  # TODO update such that only correct events are considered
-            # language=SQL
-            infer_corr_str = '''
-                        WITH record, $result_node_name
-                                MATCH (event:$event_label) - [:EXTRACTED_FROM] -> (record) <- [:EXTRACTED_FROM] - (
-                                $result_node_name)
-                                MERGE (event) - [:$corr_type] -> ($result_node_name)'''
-        elif node_constructor.infer_observed:
-            # language=SQL
-            infer_observed_str = '''
-            WITH record, $result_node_name
-                                MATCH (event:$event_label) - [:EXTRACTED_FROM] -> (record) <- [:EXTRACTED_FROM] - (
-                                $result_node_name)
-                                CREATE (event) <- [:OBSERVED] - ($result_node_name)
-                                '''
-
-        # language=SQL
-        query_str = '''
-                    CALL apoc.periodic.commit(
-                        'MATCH ($record) 
-                        WHERE NOT record:RecordCreated
-                            WITH $record_name limit $limit
-                            $merge_or_create ($result_node)
-                            SET $record_name:RecordCreated
-                            $set_label_str
-                            $set_property_str
-                            MERGE (record) <- [:EXTRACTED_FROM] - ($result_node_name)
-                            $infer_corr_str
-                            $infer_observed_str
-                            RETURN count(*)',
-                            {limit: $batch_size})
-                    '''
-
-        query_str = Template(query_str).safe_substitute({
-            "set_label_str": set_label_str,
-            "set_property_str": set_property_str,
-            "infer_corr_str": infer_corr_str,
-            "infer_observed_str": infer_observed_str,
-            "merge_or_create": merge_or_create,
-        })
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "record": node_constructor.get_prevalent_record_pattern(node_name="record"),
-                         "record_name": "record",
-                         "conditions": node_constructor.get_where_condition(node_name="record", include_start_and=True),
-                         "result_node": node_constructor.result.get_pattern(),
-                         "result_node_name": node_constructor.result.get_name(),
-                         "set_result_properties": node_constructor.get_set_result_properties_query(),
-                         "set_labels": node_constructor.get_set_result_labels_query(),
-                         "corr_type": node_constructor.corr_type,
-                         "event_label": node_constructor.event_label
-                     })
-
-    @staticmethod
-    def get_reset_created_record_query():
-        query_str = '''
-                    CALL apoc.periodic.commit(
-                        'MATCH (record:RecordCreated) 
-                            WITH record limit $limit
-                            REMOVE record:RecordCreated
-                            RETURN count(*)',
-                            {limit: $batch_size})
-                    '''
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_number_of_ids_query(node_constructor: NodeConstructor, use_record: bool = False):
-        query_str = '''MATCH (n:$labels)
-                        RETURN count(DISTINCT n.sysId) as num_ids'''
-
-        if use_record:
-            query_str = '''MATCH ($record) 
-                           RETURN count(DISTINCT record.$attribute) as num_ids'''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "labels": node_constructor.get_label_string(),
-                         "attribute": node_constructor.result.required_properties[0].ref_attribute,
-                         "record": node_constructor.get_prevalent_record_pattern(node_name="record")
-                     })
-
-    @staticmethod
-    def get_number_of_records_query(node_constructor: NodeConstructor):
-
-        query_str = '''MATCH ($record) 
-                           RETURN count(record) as count'''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "record": node_constructor.get_prevalent_record_pattern(node_name="record")
-                     })
-
-    @staticmethod
-    def get_reset_merged_in_nodes_query(node_constructor: NodeConstructor):
-        query_str = '''
-                           CALL apoc.periodic.commit(
-                                  'MATCH (n:$labels)
-                                  WHERE n.merged = True
-                                  WITH n LIMIT $limit
-                                  SET n.merged = Null
-                           RETURN COUNT(*)',
-                           {limit:$batch_size})
-                       '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "labels": node_constructor.get_label_string(),
-                     })
-
-    @staticmethod
-    def get_merge_nodes_with_same_id_query(node_constructor: NodeConstructor):
-        if "Event" in node_constructor.get_labels():
-            return None
-
-        query_str = '''
-                    CALL apoc.periodic.commit(
-                           'MATCH (n:$labels)
-                           WHERE n.merged IS NULL
-                           // we order by sysId
-                           WITH n ORDER BY n.sysId LIMIT $limit
-                           WITH collect(n) as collection
-                           WITH collection, last(collection) as last_node, size(collection) as collection_size
-                           UNWIND collection as n
-                           WITH $idt_properties, collect(n) as same_nodes, last_node, collection_size
-                           CALL {WITH same_nodes, last_node
-                                MATCH (last_node)
-                                // last node could be the first of the list of same_nodes, we do not set to merged=true
-                                // for this node
-                                 WHERE size(same_nodes) = 1 and  head(same_nodes) <> last_node
-                                 SET head(same_nodes).merged = True}             
-                           WITH same_nodes, collection_size                   
-                           WHERE size(same_nodes) > 1
-                           UNWIND range(0, toInteger(floor(size(same_nodes)/100))) as i
-                           WITH same_nodes, i*100 as min_range, apoc.coll.min([(i+1)*100, size(same_nodes)]) AS 
-                           max_range, collection_size
-                           WITH same_nodes[min_range..max_range] as lim_nodes, collection_size
-                           CALL apoc.refactor.mergeNodes(lim_nodes, {properties: "discard", mergeRels: true})
-                           YIELD node
-                           RETURN collection_size',
-                           {limit:$batch_size})
-                       '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "labels": node_constructor.get_label_string(),
-                         "idt_properties": node_constructor.get_idt_properties_query()
-                     })
-
-    @staticmethod
-    def get_infer_corr_from_parent_query(relation_constructor, use_from):
-        if use_from:
-            node = relation_constructor.from_node.get_pattern()
-            from_or_to = "FROM"
-        else:
-            node = relation_constructor.to_node.get_pattern()
-            from_or_to = "TO"
-
-        query_str = '''
-            CALL apoc.periodic.commit('
-                MATCH (e:Event) --> ($node) - [:$from_or_to] - (relation:$relation_label_str)
-                WHERE NOT EXISTS ((e) - [:CORR] -> (relation))
-                WITH DISTINCT relation, e limit $limit
-                MERGE (e) - [:$corr_type] -> (relation)
-                RETURN COUNT(*)',
-                {limit:$batch_size}
-                )       
-            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "node": node,
-                         "from_or_to": from_or_to,
-                         "relation_label_str": relation_constructor.result.get_relation_types_str(),
-                         "corr_type": relation_constructor.corr_type
-                     })
-
-    @staticmethod
-    def get_create_relation_by_relations_query(relation_constructor: RelationConstructor) -> Query:
-        if relation_constructor.model_as_node:
-            # language=sql
-            merge_str = '''
-                            MERGE ($from_node_name) -[:FROM] -> (relation:$relation_label_str) - [:TO] -> (
-                            $to_node_name)
-                            '''
-        else:
-            merge_str = "MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)"
-
-        # language=SQL
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                '$relation_queries                        
-                RETURN distinct $from_node_name, $to_node_name',
-                '$merge_str',                        
-                {batchSize: $batch_size})
-            '''
-
-        query_str = Template(query_str).safe_substitute({
-            "merge_str": merge_str
-        })
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "relation_queries": relation_constructor.get_relations_query(),
-                         "from_node_name": relation_constructor.from_node.get_name(),
-                         "to_node_name": relation_constructor.to_node.get_name(),
-                         "rel_pattern": relation_constructor.result.get_pattern(),
-                         "relation_label_str": relation_constructor.result.get_relation_types_str()
-                     })
-
-    @staticmethod
-    def get_create_relation_using_record_query(relation_constructor: RelationConstructor) -> Query:
-        # find events that are related to different entities of which one event also has a reference to the other entity
-        # create a relation between these two entities
-        if relation_constructor.model_as_node:
-            # language=sql
-            merge_str = '''
-                            MERGE ($from_node_name) -[:FROM] -> (relation:$relation_label_str) - [:TO] -> (
-                            $to_node_name)
-                            MERGE (relation)  - [:EXTRACTED_FROM] -> (record)
-                            '''
-        else:
-            merge_str = "MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)"
-
-        query_str = '''     CALL apoc.periodic.commit('
-                            MATCH (record:$record_labels)
-                            WHERE NOT record:RecordCreated
-                            WITH  record limit $limit
-                            MATCH ($from_node) - [:EXTRACTED_FROM] -> (record)
-                            MATCH ($to_node) - [:EXTRACTED_FROM] -> (record)
-                            $merge_str
-                            SET record:RecordCreated
-                            RETURN COUNT(*)',
-                            {limit:$batch_size})
-                        '''
-
-        query_str = Template(query_str).safe_substitute({
-            "merge_str": merge_str
-        })
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "from_node": relation_constructor.from_node.get_pattern(),
-                         "from_node_name": relation_constructor.from_node.get_name(),
-                         "to_node": relation_constructor.to_node.get_pattern(),
-                         "to_node_name": relation_constructor.to_node.get_name(),
-                         "record_labels": relation_constructor.prevalent_record.get_label_str(
-                             include_first_colon=False),
-                         "rel_pattern": relation_constructor.result.get_pattern("relation"),
-                         "relation_labels": relation_constructor.result.get_relation_types_str(as_list=True),
-                         "relation_label_str": relation_constructor.result.get_relation_types_str()
-                     })
-
-    @staticmethod
-    def get_reset_created_relation_query(relation_constructor: RelationConstructor) -> Query:
-        # find events that are related to different entities of which one event also has a reference to the other entity
-        # create a relation between these two entities
-
-        query_str = '''     CALL apoc.periodic.commit('
-                              MATCH (record:$record_labels)
-                              WHERE record.rel_created = True
-                              WITH record limit $limit
-                              SET record.rel_created = Null
-                              RETURN COUNT(*)',
-                              {limit:$batch_size})
-                          '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "record_labels": relation_constructor.prevalent_record.get_label_str(
-                             include_first_colon=False)
-                     })
-
-    @staticmethod
-    def get_add_duration_query_str(add_duration) -> str:
-        if add_duration:
-            # check the type of the timestamp attributes.
-            # DATE, DATETIME, TIME --> create Duration between first and second
-            # INT, FLOAT --> save difference between second and first
-            add_duration_str = '''
-                , CASE 
-                    WHEN apoc.meta.cypher.type(first.timestamp) IN ["DATE_TIME", "TIME", "DATE"] 
-                        AND apoc.meta.cypher.type(second.timestamp) IN ["DATE_TIME", "TIME", "DATE"] 
-                        THEN duration.between(first.timestamp, second.timestamp)
-                    WHEN apoc.meta.cypher.type(first.timestamp) IN ["INTEGER", "FLOAT"]
-                     AND apoc.meta.cypher.type(second.timestamp) IN ["INTEGER", "FLOAT"]
-                     THEN  second.timestamp - first.timestamp
-                    ELSE NULL
-                END AS duration
-            '''
-        else:
-            # we don't want to add the duration, so we use NULL for duration
-            # This ensures us that we can use duration in the rest of the queries
-            add_duration_str = '''
-                , NULL as duration
-            '''
-
-        return add_duration_str
-
-    @staticmethod
-    def get_create_directly_follows_query(entity: Union[ConstructedNodes, ConstructedRelation], event_label,
-                                          add_duration: bool = False) -> Query:
-        # find the specific entities and events with a certain label correlated to that entity
-        # order all events by time, order_nr and id grouped by a node n
-        # collect the sorted nodes as a list
-        # unwind the list from 0 to the one-to-last node
-        # find neighbouring nodes and add an edge between
-
-        # language=sql
-
-        if event_label == "CompoundEvent":
-            if entity.type == "Resource":
-                query_str = '''
-                     CALL apoc.periodic.iterate(
-                        'MATCH (n:$entity_labels_string) <-[:$corr_type_string]- (e:$event_label)
-                        CALL {
-                                WITH e
-                                MATCH (e) - [:CONSISTS_OF] -> (single_event:Event)
-                                RETURN id(single_event) as min_id ORDER BY id(single_event)
-                                LIMIT 1
-                            }
-                        WITH n , e as nodes ORDER BY e.timestamp, min_id
-                        WITH n , collect (nodes) as nodeList
-                        UNWIND range(0,size(nodeList)-2) AS i
-                        WITH n , nodeList[i] as first, nodeList[i+1] as second
-                        RETURN n, first, second $add_duration_str',
-                        'MERGE (first) -[df:$df_entity {entityType: "$entity_type"}]->(second)
-                         SET df.type = "DF"
-                         SET df.entityId = n.sysId
-                         SET df.duration = duration
-                        ',
-                        {batchSize: $batch_size})
-                    '''
-            else:
-                query_str = '''
-                                     CALL apoc.periodic.iterate(
-                                        'MATCH (n:$entity_labels_string) <-[:$corr_type_string]- (e:$event_label)
-                                        CALL {
-                                                WITH e
-                                                MATCH (e) - [:CONSISTS_OF] -> (single_event:Event)
-                                                RETURN id(single_event) as min_id ORDER BY id(single_event)
-                                                LIMIT 1
-                                            }
-                                        WITH n , e as nodes ORDER BY e.timestamp, min_id
-                                        WITH n , collect (nodes) as nodeList
-                                        UNWIND range(0,size(nodeList)-2) AS i
-                                        WITH n , nodeList[i] as first, nodeList[i+1] as second
-                                        RETURN first, second $add_duration_str',
-                                        'MERGE (first) -[df:$df_entity {entityType: "$entity_type"}]->(second)
-                                         SET df.type = "DF"
-                                         SET df.duration = duration
-                                        ',
-                                        {batchSize: $batch_size})
-                                    '''
-
-        else:
-            query_str = '''
-                             CALL apoc.periodic.iterate(
-                                'MATCH (n:$entity_labels_string) <-[:$corr_type_string]- (e:$event_label)
-                                WITH n , e as nodes ORDER BY e.timestamp, ID(e)
-                                WITH n , collect (nodes) as nodeList
-                                UNWIND range(0,size(nodeList)-2) AS i
-                                WITH n , nodeList[i] as first, nodeList[i+1] as second
-                                RETURN first, second $add_duration_str',
-                                'MERGE (first) -[df:$df_entity {entityType: "$entity_type"}]->(second)
-                                 SET df.type = "DF"
-                                 SET df.duration = duration
-                                ',
-                                {batchSize: $batch_size})
-                            '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity_labels_string": entity.get_label_string(),
-                         "corr_type_string": entity.get_corr_type_strings(),
-                         "event_label": event_label,
-                         "df_entity": entity.get_df_label(),
-                         "entity_type": entity.type,
-                         "add_duration_str": SemanticHeaderQueryLibrary.get_add_duration_query_str(add_duration)
-                     })
-
-    @staticmethod
-    def get_merge_duplicate_df_entity_query(node: ConstructedNodes) -> Query:
-
-        # language=sql
-        query_str = '''
-                        MATCH (n1:Event)-[r:$df_entity {entityType: '$entity_type'}]->(n2:Event)
-                        WITH n1, n2, collect(r) AS rels
-                        WHERE size(rels) > 1
-                        // only include this and the next line if you want to remove the existing relationships
-                        UNWIND rels AS r 
-                        DELETE r
-                        MERGE (n1)
-                            -[:$df_entity {entityType: '$entity_type', count:size(rels), type: 'DF'}]->
-                              (n2)
-                    '''
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity_type": node.type,
-                         "df_entity": node.get_df_label()
-                     })
+from string import Template
+from typing import Union, Optional, List
+
+from ..data_managers.semantic_header import ConstructedNodes, NodeConstructor, Node, \
+    RelationConstructor, RecordConstructor, ConstructedRelation
+from ..database_managers.db_connection import Query
+
+
+class SemanticHeaderQueryLibrary:
+    @staticmethod
+    def get_create_node_by_record_constructor_query(node_constructor: NodeConstructor, merge=True,
+                                                    logs: Optional[List[str]] = None) -> Query:
+        # find events that contain the entity as property and not nan
+        # save the value of the entity property as id and also whether it is a virtual entity
+        # create a new entity node if it not exists yet with properties
+        merge_or_create = 'MERGE' if merge else 'CREATE'
+        set_label_str = ""
+        set_property_str = node_constructor.get_set_result_properties_query()
+        infer_corr_str = ""
+        infer_observed_str = ""
+
+        if node_constructor.set_labels is not None:
+            set_label_str = f'SET $set_labels'''
+
+        if len(node_constructor.inferred_relationships) > 0:
+            infer_corr_str = '''WITH record, $result_node_name'''
+            for relationship in node_constructor.inferred_relationships:
+                infer_rel_str = '''
+                    CALL {WITH record, $result_node_name
+                            MATCH ($event_node) - [:EXTRACTED_FROM] -> (record:$record_labels) <- [:EXTRACTED_FROM] - (
+                                $result_node_name)
+                                MERGE (event) - [:$relation_type] -> ($result_node_name)}'''
+                infer_rel_str = Template(infer_rel_str).safe_substitute({
+                    "event_node": relationship.event.get_pattern(name="event"),
+                    "record_labels": relationship.get_labels_str(),
+                    "relation_type": relationship.relation_type
+                })
+                infer_corr_str += infer_rel_str
+        elif node_constructor.infer_corr_from_event_record:
+            # language=SQL
+            infer_corr_str = '''
+            WITH record, $result_node_name
+                                MATCH (event:$event_label) - [:EXTRACTED_FROM] -> (record) <- [:EXTRACTED_FROM] - (
+                                $result_node_name)
+                                MERGE (event) - [:$corr_type] -> ($result_node_name)'''
+        elif node_constructor.infer_corr_from_entity_record:  # TODO update such that only correct events are considered
+            # language=SQL
+            infer_corr_str = '''
+                        WITH record, $result_node_name
+                                MATCH (event:$event_label) - [:EXTRACTED_FROM] -> (record) <- [:EXTRACTED_FROM] - (
+                                $result_node_name)
+                                MERGE (event) - [:$corr_type] -> ($result_node_name)'''
+        elif node_constructor.infer_observed:
+            # language=SQL
+            infer_observed_str = '''
+            WITH record, $result_node_name
+                                MATCH (event:$event_label) - [:EXTRACTED_FROM] -> (record) <- [:EXTRACTED_FROM] - (
+                                $result_node_name)
+                                CREATE (event) <- [:OBSERVED] - ($result_node_name)
+                                '''
+
+        # add check to only transform records from the imported logs
+        if logs is not None:
+            log_str = ",".join([f'"{log}"' for log in logs])
+            log_check_str = f"WHERE record.log in [{log_str}]"
+        else:
+            log_check_str = ""
+
+        # language=SQL
+        query_str = '''
+                    CALL apoc.periodic.iterate(
+                    'MATCH ($record) 
+                          $log_check_str
+                          RETURN record',
+                          '$merge_or_create ($result_node)
+                          $set_label_str
+                          $set_property_str
+                          MERGE (record) <- [:EXTRACTED_FROM] - ($result_node_name)
+                          $infer_corr_str
+                          $infer_observed_str', {batchSize:$batch_size})
+                    '''
+
+        query_str = Template(query_str).safe_substitute({
+            "set_label_str": set_label_str,
+            "set_property_str": set_property_str,
+            "infer_corr_str": infer_corr_str,
+            "infer_observed_str": infer_observed_str,
+            "merge_or_create": merge_or_create,
+            "log_check_str": log_check_str
+        })
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "record": node_constructor.get_prevalent_record_pattern(node_name="record"),
+                         "record_name": "record",
+                         "result_node": node_constructor.result.get_pattern(),
+                         "result_node_name": node_constructor.result.get_name(),
+                         "set_result_properties": node_constructor.get_set_result_properties_query(),
+                         "set_labels": node_constructor.get_set_result_labels_query(),
+                         "corr_type": node_constructor.corr_type,
+                         "event_label": node_constructor.event_label
+                     })
+
+    @staticmethod
+    def get_associated_record_labels_query(logs):
+        log_str = ",".join([f'"{log}"' for log in logs])
+        log_str = f"[{log_str}]"
+
+        query_str = '''
+            MATCH (r:Record)
+            WHERE r.log in $log_str
+            UNWIND labels(r) as _label
+            RETURN collect(distinct _label) as labels
+        '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={"log_str": log_str})
+
+    @staticmethod
+    def get_number_of_records_query(node_constructor: NodeConstructor):
+
+        query_str = '''MATCH ($record) 
+                           RETURN count(record) as count'''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "record": node_constructor.get_prevalent_record_pattern(node_name="record")
+                     })
+
+    @staticmethod
+    def get_infer_corr_from_parent_query(relation_constructor, use_from):
+        if use_from:
+            node = relation_constructor.from_node.get_pattern()
+            from_or_to = "FROM"
+        else:
+            node = relation_constructor.to_node.get_pattern()
+            from_or_to = "TO"
+
+        query_str = '''
+            CALL apoc.periodic.iterate('
+                MATCH (e:Event) --> ($node) - [:$from_or_to] - (relation:$relation_label_str)
+                WHERE NOT EXISTS ((e) - [:CORR] -> (relation))
+                RETURN DISTINCT relation, e',
+                'MERGE (e) - [:$corr_type] -> (relation)',
+                {batchSize:$batch_size}
+                )       
+            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "node": node,
+                         "from_or_to": from_or_to,
+                         "relation_label_str": relation_constructor.result.get_relation_types_str(),
+                         "corr_type": relation_constructor.corr_type
+                     })
+
+    @staticmethod
+    def get_create_relation_by_relations_query(relation_constructor: RelationConstructor) -> Query:
+        if relation_constructor.model_as_node:
+            # language=sql
+            merge_str = '''
+                            MERGE ($from_node_name) -[:FROM] -> (relation:$relation_label_str) - [:TO] -> (
+                            $to_node_name)
+                            '''
+        else:
+            merge_str = "MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)"
+
+        # language=SQL
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                '$relation_queries                        
+                RETURN distinct $from_node_name, $to_node_name',
+                '$merge_str',                        
+                {batchSize: $batch_size})
+            '''
+
+        query_str = Template(query_str).safe_substitute({
+            "merge_str": merge_str
+        })
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "relation_queries": relation_constructor.get_relations_query(),
+                         "from_node_name": relation_constructor.from_node.get_name(),
+                         "to_node_name": relation_constructor.to_node.get_name(),
+                         "rel_pattern": relation_constructor.result.get_pattern(),
+                         "relation_label_str": relation_constructor.result.get_relation_types_str()
+                     })
+
+    @staticmethod
+    def get_create_relation_using_record_query(relation_constructor: RelationConstructor,
+                                               logs: Optional[List[str]] = None) -> Query:
+        # find events that are related to different entities of which one event also has a reference to the other entity
+        # create a relation between these two entities
+        if relation_constructor.model_as_node:
+            # language=sql
+            merge_str = '''
+                            MERGE ($from_node_name) -[:FROM] -> (relation:$relation_label_str) - [:TO] -> (
+                            $to_node_name)
+                            MERGE (relation)  - [:EXTRACTED_FROM] -> (record)
+                            '''
+        else:
+            merge_str = "MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)"
+
+        # add check to only transform records from the imported logs
+        if logs is not None:
+            log_str = ",".join([f'"{log}"' for log in logs])
+            log_check_str = f"WHERE record.log in [{log_str}]"
+        else:
+            log_check_str = ""
+
+        query_str = '''     CALL apoc.periodic.iterate('
+                            MATCH (record:$record_labels)
+                            $log_check_str
+                            RETURN record',
+                            '
+                            MATCH ($from_node) - [:EXTRACTED_FROM] -> (record)
+                            MATCH ($to_node) - [:EXTRACTED_FROM] -> (record)
+                            $merge_str',
+                            {batchSize:$batch_size})
+                        '''
+
+        query_str = Template(query_str).safe_substitute({
+            "merge_str": merge_str,
+            "log_check_str": log_check_str
+        })
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "from_node": relation_constructor.from_node.get_pattern(),
+                         "from_node_name": relation_constructor.from_node.get_name(),
+                         "to_node": relation_constructor.to_node.get_pattern(),
+                         "to_node_name": relation_constructor.to_node.get_name(),
+                         "record_labels": relation_constructor.prevalent_record.get_label_str(
+                             include_first_colon=False),
+                         "rel_pattern": relation_constructor.result.get_pattern("relation"),
+                         "relation_labels": relation_constructor.result.get_relation_types_str(as_list=True),
+                         "relation_label_str": relation_constructor.result.get_relation_types_str()
+                     })
+
+    @staticmethod
+    def get_add_duration_query_str(add_duration) -> str:
+        if add_duration:
+            # check the type of the timestamp attributes.
+            # DATE, DATETIME, TIME --> create Duration between first and second
+            # INT, FLOAT --> save difference between second and first
+            add_duration_str = '''
+                , CASE 
+                    WHEN apoc.meta.cypher.type(first.timestamp) IN ["DATE_TIME", "TIME", "DATE"] 
+                        AND apoc.meta.cypher.type(second.timestamp) IN ["DATE_TIME", "TIME", "DATE"] 
+                        THEN duration.between(first.timestamp, second.timestamp)
+                    WHEN apoc.meta.cypher.type(first.timestamp) IN ["INTEGER", "FLOAT"]
+                     AND apoc.meta.cypher.type(second.timestamp) IN ["INTEGER", "FLOAT"]
+                     THEN  second.timestamp - first.timestamp
+                    ELSE NULL
+                END AS duration
+            '''
+        else:
+            # we don't want to add the duration, so we use NULL for duration
+            # This ensures us that we can use duration in the rest of the queries
+            add_duration_str = '''
+                , NULL as duration
+            '''
+
+        return add_duration_str
+
+    @staticmethod
+    def get_create_directly_follows_query(entity: Union[ConstructedNodes, ConstructedRelation], event_label,
+                                          add_duration: bool = False) -> Query:
+        # find the specific entities and events with a certain label correlated to that entity
+        # order all events by time, order_nr and id grouped by a node n
+        # collect the sorted nodes as a list
+        # unwind the list from 0 to the one-to-last node
+        # find neighbouring nodes and add an edge between
+
+        # language=sql
+
+        if event_label == "CompoundEvent":
+            if entity.type == "Resource":
+                query_str = '''
+                     CALL apoc.periodic.iterate(
+                        'MATCH (n:$entity_labels_string) <-[:$corr_type_string]- (e:$event_label)
+                        CALL {
+                                WITH e
+                                MATCH (e) - [:CONSISTS_OF] -> (single_event:Event)
+                                RETURN id(single_event) as min_id ORDER BY id(single_event)
+                                LIMIT 1
+                            }
+                        WITH n , e as nodes ORDER BY e.timestamp, min_id
+                        WITH n , collect (nodes) as nodeList
+                        UNWIND range(0,size(nodeList)-2) AS i
+                        WITH n , nodeList[i] as first, nodeList[i+1] as second
+                        RETURN n, first, second $add_duration_str',
+                        'MERGE (first) -[df:$df_entity {entityType: "$entity_type"}]->(second)
+                         SET df.type = "DF"
+                         SET df.entityId = n.sysId
+                         SET df.duration = duration
+                        ',
+                        {batchSize: $batch_size})
+                    '''
+            else:
+                query_str = '''
+                                     CALL apoc.periodic.iterate(
+                                        'MATCH (n:$entity_labels_string) <-[:$corr_type_string]- (e:$event_label)
+                                        CALL {
+                                                WITH e
+                                                MATCH (e) - [:CONSISTS_OF] -> (single_event:Event)
+                                                RETURN id(single_event) as min_id ORDER BY id(single_event)
+                                                LIMIT 1
+                                            }
+                                        WITH n , e as nodes ORDER BY e.timestamp, min_id
+                                        WITH n , collect (nodes) as nodeList
+                                        UNWIND range(0,size(nodeList)-2) AS i
+                                        WITH n , nodeList[i] as first, nodeList[i+1] as second
+                                        RETURN first, second $add_duration_str',
+                                        'MERGE (first) -[df:$df_entity {entityType: "$entity_type"}]->(second)
+                                         SET df.type = "DF"
+                                         SET df.duration = duration
+                                        ',
+                                        {batchSize: $batch_size})
+                                    '''
+
+        else:
+            query_str = '''
+                             CALL apoc.periodic.iterate(
+                                'MATCH (n:$entity_labels_string) <-[:$corr_type_string]- (e:$event_label)
+                                WITH n , e as nodes ORDER BY e.timestamp, ID(e)
+                                WITH n , collect (nodes) as nodeList
+                                UNWIND range(0,size(nodeList)-2) AS i
+                                WITH n , nodeList[i] as first, nodeList[i+1] as second
+                                RETURN first, second $add_duration_str',
+                                'MERGE (first) -[df:$df_entity {entityType: "$entity_type"}]->(second)
+                                 SET df.type = "DF"
+                                 SET df.duration = duration
+                                ',
+                                {batchSize: $batch_size})
+                            '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity_labels_string": entity.get_label_string(),
+                         "corr_type_string": entity.get_corr_type_strings(),
+                         "event_label": event_label,
+                         "df_entity": entity.get_df_label(),
+                         "entity_type": entity.type,
+                         "add_duration_str": SemanticHeaderQueryLibrary.get_add_duration_query_str(add_duration)
+                     })
+
+    @staticmethod
+    def get_merge_duplicate_df_entity_query(node: ConstructedNodes) -> Query:
+
+        # language=sql
+        query_str = '''
+                        MATCH (n1:Event)-[r:$df_entity {entityType: '$entity_type'}]->(n2:Event)
+                        WITH n1, n2, collect(r) AS rels
+                        WHERE size(rels) > 1
+                        // only include this and the next line if you want to remove the existing relationships
+                        UNWIND rels AS r 
+                        DELETE r
+                        MERGE (n1)
+                            -[:$df_entity {entityType: '$entity_type', count:size(rels), type: 'DF'}]->
+                              (n2)
+                    '''
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity_type": node.type,
+                         "df_entity": node.get_df_label()
+                     })
```

### Comparing `promg-1.0.9/src/promg/cypher_queries/task_identification_ql.py` & `promg-1.1.0/src/promg/cypher_queries/task_identification_ql.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-from string import Template
-
-from ..database_managers.db_connection import Query
-
-
-class TaskIdentifierLibrary:
-    @staticmethod
-    def get_combine_df_joint_query(resource, case):
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (e1:Event)-[:$df_resource]->(e2:Event)
-                 WHERE (e1)-[:$df_case]->(e2)
-                 RETURN e1,e2",
-                "WITH e1,e2
-                    MERGE (e1)-[:DF_JOINT]->(e2)",
-                    {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "df_resource": resource.get_df_label(),
-                         "df_case": case.get_df_label()
-                     })
-
-    @staticmethod
-    def get_create_task_instances_query(resource):
-        print("get_create_task_instances_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "CALL {
-                    MATCH (e1:Event)-[:DF_JOINT]->() WHERE NOT ()-[:DF_JOINT]->(e1)
-                    MATCH ()-[:DF_JOINT]->(e2:Event) WHERE NOT (e2)-[:DF_JOINT]->()
-                    MATCH p=(e1)-[:DF_JOINT*]->(e2)
-                    RETURN p, e1, e2
-                    UNION
-                    MATCH (e:Event) WHERE (e)-[:CORR]->(:$resource_node_label)
-                    AND NOT ()-[:DF_JOINT]->(e) AND NOT (e)-[:DF_JOINT]->()
-                    MATCH p=(e) RETURN p, e AS e1, e AS e2
-                 }
-                 RETURN [event in nodes(p) | event.activity+'+'+event.lifecycle] AS variant,
-                    nodes(p) AS events, e1.timestamp AS start_time, e2.timestamp AS end_time",
-                "WITH variant, events, start_time, end_time
-                    CREATE (ti:TaskInstance {variant:variant, start_time:start_time, end_time:end_time})
-                    WITH ti, events
-                    UNWIND events AS e
-                        CREATE (e)<-[:CONTAINS]-(ti)",
-                {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "resource_node_label": resource.type
-                     })
-
-    @staticmethod
-    def get_split_ti_nodes_create_new_1_query():
-        print("get_split_ti_nodes_create_new_1_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (ti:TaskInstance)-[:CONTAINS]->(e:Event) WHERE date(ti.start_time) <> date(ti.end_time)
-                 WITH ti, date(e.timestamp) AS date, e ORDER BY e.timestamp
-                 WITH DISTINCT ti, date, COLLECT(e) AS events
-                 WITH events[0] AS e_start, events[size(events)-1] AS e_end
-                 WITH e_start, e_end
-                 MATCH p=(e_start)-[:DF_JOINT*]->(e_end)
-                 WITH p, e_start AS e1, e_end AS e2
-                 RETURN [event in nodes(p) | event.activity+'+'+event.lifecycle] AS variant, 
-                    nodes(p) AS events, e1.timestamp AS start_time, e2.timestamp AS end_time",
-                "WITH variant, events, start_time, end_time
-                    CREATE (ti:TaskInstance {variant:variant, start_time:start_time, end_time:end_time})
-                    WITH ti, events
-                    UNWIND events AS e
-                    CREATE (e)<-[:CONTAINS]-(ti)",
-                {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_split_ti_nodes_create_new_2_query():
-        print("get_split_ti_nodes_create_new_2_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (ti:TaskInstance)-[:CONTAINS]->(e:Event) WHERE date(ti.start_time) <> date(ti.end_time)
-                 WITH ti, date(e.timestamp) AS date, e ORDER BY e.timestamp
-                 WITH DISTINCT ti, date, COLLECT(e) AS events
-                 WITH events[0] AS e_start, events[size(events)-1] AS e_end
-                 WITH e_start, e_end
-                 MATCH (e_start) MATCH (e_end) WHERE e_start = e_end
-                 MATCH p=(e_start)
-                 WITH p, e_start AS e1, e_end AS e2
-                 RETURN [event in nodes(p) | event.activity+'+'+event.lifecycle] AS variant, 
-                    nodes(p) AS events, e1.timestamp AS start_time, e2.timestamp AS end_time",
-                "WITH variant, events, start_time, end_time
-                 CREATE (ti:TaskInstance {variant:variant, start_time:start_time, end_time:end_time})
-                 WITH ti, events
-                 UNWIND events AS e
-                 CREATE (e)<-[:CONTAINS]-(ti)",
-                {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_split_ti_nodes_remove_old_query():
-        print("get_split_ti_nodes_remove_old_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (ti:TaskInstance) WHERE date(ti.start_time) <> date(ti.end_time)
-                 RETURN ti",
-                "WITH ti
-                 DETACH DELETE ti",
-                {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_remove_df_joint_query():
-        print("get_remove_df_joint_query")
-        # language=sql
-        query_str = '''
-                MATCH ()-[r:DF_JOINT]-()
-                DELETE r
-                '''
-
-        return Query(query_str=query_str)
-
-    @staticmethod
-    def get_correlate_ti_to_entity_query(entity):
-        print("get_correlate_ti_to_entity_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (ti:TaskInstance)-[:CONTAINS]->(:Event)-[:CORR]->(n:$entity_node_label)
-                 RETURN DISTINCT ti, n",
-                "WITH ti, n
-                    CREATE (ti)-[:CORR]->(n)",
-                {batchSize:$batch_size})
-                    '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity_node_label": entity.type
-                     })
-
-    @staticmethod
-    def get_lift_df_to_task_instances_query(entity):
-        print("get_lift_df_to_task_instances_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (n:$entity_node_label)
-                 MATCH (ti:TaskInstance)-[:CORR]->(n)
-                 WITH n, ti AS nodes ORDER BY ti.start_time, ID(ti)
-                 WITH n, COLLECT (nodes) as nodeList
-                 UNWIND range(0, size(nodeList)-2) AS i
-                 RETURN n, nodeList[i] as ti_first, nodeList[i+1] as ti_second",
-                "WITH n, ti_first, ti_second
-                    MERGE (ti_first)-[df:DF_TI_$entity_node_label]->(ti_second)",
-                {batchSize:$batch_size})
-                    '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "entity_node_label": entity.type
-                     })
-
-    @staticmethod
-    def get_aggregate_task_instances_query(property):
-        print("get_aggregate_task_instances_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (ti:TaskInstance) WHERE ti.$property IS NOT NULL
-                 RETURN DISTINCT ti.$property AS id, count(*) AS count",
-                 "WITH id, count
-                  MERGE (ta:TaskAggregation {Type:'$property', id:id, count:count})",
-                {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "property": property
-                     })
-
-    @staticmethod
-    def get_link_task_instances_to_aggregations_query(property):
-        print("get_link_task_instances_to_aggregations_query")
-        # language=sql
-        query_str = '''
-                CALL apoc.periodic.iterate(
-                "MATCH (ta:TaskAggregation) WHERE ta.Type = '$property'
-                 MATCH (ti:TaskInstance) WHERE ti.$property = ta.id
-                 RETURN ta, ti",
-                "WITH ta, ti
-                 CREATE (ti)-[:OBSERVED]->(ta)",
-                {batchSize:$batch_size})
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "property": property
-                     })
-
-    @staticmethod
-    def get_lift_df_to_task_aggregations_query(property, entity):
-        print("get_lift_df_to_task_aggregations_query")
-        # language=sql
-        query_str = '''
-                MATCH (ta1:TaskAggregation)<-[:OBSERVED]-(ti1:TaskInstance)-[df:DF_TI_$entity_node_label]
-                    ->(ti2:TaskInstance)-[:OBSERVED]->(ta2:TaskAggregation)
-                    WHERE ta1.Type = '$property' AND ta2.Type = '$property'
-                MATCH (ti1)-[:CORR]->(n:$entity_node_label)<-[:CORR]-(ti2)
-                WITH ta1, count(df) AS df_freq, ta2
-                MERGE (ta1)-[rel2:DF_TA_$entity_node_label]->(ta2) ON CREATE SET rel2.count=df_freq
-                '''
-
-        return Query(query_str=query_str,
-                     template_string_parameters={
-                         "property": property,
-                         "entity_node_label": entity.type
-                     })
+from string import Template
+
+from ..database_managers.db_connection import Query
+
+
+class TaskIdentifierLibrary:
+    @staticmethod
+    def get_combine_df_joint_query(resource, case):
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (e1:Event)-[:$df_resource]->(e2:Event)
+                 WHERE (e1)-[:$df_case]->(e2)
+                 RETURN e1,e2",
+                "WITH e1,e2
+                    MERGE (e1)-[:DF_JOINT]->(e2)",
+                    {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "df_resource": resource.get_df_label(),
+                         "df_case": case.get_df_label()
+                     })
+
+    @staticmethod
+    def get_create_task_instances_query(resource):
+        print("get_create_task_instances_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "CALL {
+                    MATCH (e1:Event)-[:DF_JOINT]->() WHERE NOT ()-[:DF_JOINT]->(e1)
+                    MATCH ()-[:DF_JOINT]->(e2:Event) WHERE NOT (e2)-[:DF_JOINT]->()
+                    MATCH p=(e1)-[:DF_JOINT*]->(e2)
+                    RETURN p, e1, e2
+                    UNION
+                    MATCH (e:Event) WHERE (e)-[:CORR]->(:$resource_node_label)
+                    AND NOT ()-[:DF_JOINT]->(e) AND NOT (e)-[:DF_JOINT]->()
+                    MATCH p=(e) RETURN p, e AS e1, e AS e2
+                 }
+                 RETURN [event in nodes(p) | event.activity+'+'+event.lifecycle] AS variant,
+                    nodes(p) AS events, e1.timestamp AS start_time, e2.timestamp AS end_time",
+                "WITH variant, events, start_time, end_time
+                    CREATE (ti:TaskInstance {variant:variant, start_time:start_time, end_time:end_time})
+                    WITH ti, events
+                    UNWIND events AS e
+                        CREATE (e)<-[:CONTAINS]-(ti)",
+                {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "resource_node_label": resource.type
+                     })
+
+    @staticmethod
+    def get_split_ti_nodes_create_new_1_query():
+        print("get_split_ti_nodes_create_new_1_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (ti:TaskInstance)-[:CONTAINS]->(e:Event) WHERE date(ti.start_time) <> date(ti.end_time)
+                 WITH ti, date(e.timestamp) AS date, e ORDER BY e.timestamp
+                 WITH DISTINCT ti, date, COLLECT(e) AS events
+                 WITH events[0] AS e_start, events[size(events)-1] AS e_end
+                 WITH e_start, e_end
+                 MATCH p=(e_start)-[:DF_JOINT*]->(e_end)
+                 WITH p, e_start AS e1, e_end AS e2
+                 RETURN [event in nodes(p) | event.activity+'+'+event.lifecycle] AS variant, 
+                    nodes(p) AS events, e1.timestamp AS start_time, e2.timestamp AS end_time",
+                "WITH variant, events, start_time, end_time
+                    CREATE (ti:TaskInstance {variant:variant, start_time:start_time, end_time:end_time})
+                    WITH ti, events
+                    UNWIND events AS e
+                    CREATE (e)<-[:CONTAINS]-(ti)",
+                {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_split_ti_nodes_create_new_2_query():
+        print("get_split_ti_nodes_create_new_2_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (ti:TaskInstance)-[:CONTAINS]->(e:Event) WHERE date(ti.start_time) <> date(ti.end_time)
+                 WITH ti, date(e.timestamp) AS date, e ORDER BY e.timestamp
+                 WITH DISTINCT ti, date, COLLECT(e) AS events
+                 WITH events[0] AS e_start, events[size(events)-1] AS e_end
+                 WITH e_start, e_end
+                 MATCH (e_start) MATCH (e_end) WHERE e_start = e_end
+                 MATCH p=(e_start)
+                 WITH p, e_start AS e1, e_end AS e2
+                 RETURN [event in nodes(p) | event.activity+'+'+event.lifecycle] AS variant, 
+                    nodes(p) AS events, e1.timestamp AS start_time, e2.timestamp AS end_time",
+                "WITH variant, events, start_time, end_time
+                 CREATE (ti:TaskInstance {variant:variant, start_time:start_time, end_time:end_time})
+                 WITH ti, events
+                 UNWIND events AS e
+                 CREATE (e)<-[:CONTAINS]-(ti)",
+                {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_split_ti_nodes_remove_old_query():
+        print("get_split_ti_nodes_remove_old_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (ti:TaskInstance) WHERE date(ti.start_time) <> date(ti.end_time)
+                 RETURN ti",
+                "WITH ti
+                 DETACH DELETE ti",
+                {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_remove_df_joint_query():
+        print("get_remove_df_joint_query")
+        # language=sql
+        query_str = '''
+                MATCH ()-[r:DF_JOINT]-()
+                DELETE r
+                '''
+
+        return Query(query_str=query_str)
+
+    @staticmethod
+    def get_correlate_ti_to_entity_query(entity):
+        print("get_correlate_ti_to_entity_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (ti:TaskInstance)-[:CONTAINS]->(:Event)-[:CORR]->(n:$entity_node_label)
+                 RETURN DISTINCT ti, n",
+                "WITH ti, n
+                    CREATE (ti)-[:CORR]->(n)",
+                {batchSize:$batch_size})
+                    '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity_node_label": entity.type
+                     })
+
+    @staticmethod
+    def get_lift_df_to_task_instances_query(entity):
+        print("get_lift_df_to_task_instances_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (n:$entity_node_label)
+                 MATCH (ti:TaskInstance)-[:CORR]->(n)
+                 WITH n, ti AS nodes ORDER BY ti.start_time, ID(ti)
+                 WITH n, COLLECT (nodes) as nodeList
+                 UNWIND range(0, size(nodeList)-2) AS i
+                 RETURN n, nodeList[i] as ti_first, nodeList[i+1] as ti_second",
+                "WITH n, ti_first, ti_second
+                    MERGE (ti_first)-[df:DF_TI_$entity_node_label]->(ti_second)",
+                {batchSize:$batch_size})
+                    '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "entity_node_label": entity.type
+                     })
+
+    @staticmethod
+    def get_aggregate_task_instances_query(property):
+        print("get_aggregate_task_instances_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (ti:TaskInstance) WHERE ti.$property IS NOT NULL
+                 RETURN DISTINCT ti.$property AS id, count(*) AS count",
+                 "WITH id, count
+                  MERGE (ta:TaskAggregation {Type:'$property', id:id, count:count})",
+                {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "property": property
+                     })
+
+    @staticmethod
+    def get_link_task_instances_to_aggregations_query(property):
+        print("get_link_task_instances_to_aggregations_query")
+        # language=sql
+        query_str = '''
+                CALL apoc.periodic.iterate(
+                "MATCH (ta:TaskAggregation) WHERE ta.Type = '$property'
+                 MATCH (ti:TaskInstance) WHERE ti.$property = ta.id
+                 RETURN ta, ti",
+                "WITH ta, ti
+                 CREATE (ti)-[:OBSERVED]->(ta)",
+                {batchSize:$batch_size})
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "property": property
+                     })
+
+    @staticmethod
+    def get_lift_df_to_task_aggregations_query(property, entity):
+        print("get_lift_df_to_task_aggregations_query")
+        # language=sql
+        query_str = '''
+                MATCH (ta1:TaskAggregation)<-[:OBSERVED]-(ti1:TaskInstance)-[df:DF_TI_$entity_node_label]
+                    ->(ti2:TaskInstance)-[:OBSERVED]->(ta2:TaskAggregation)
+                    WHERE ta1.Type = '$property' AND ta2.Type = '$property'
+                MATCH (ti1)-[:CORR]->(n:$entity_node_label)<-[:CORR]-(ti2)
+                WITH ta1, count(df) AS df_freq, ta2
+                MERGE (ta1)-[rel2:DF_TA_$entity_node_label]->(ta2) ON CREATE SET rel2.count=df_freq
+                '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "property": property,
+                         "entity_node_label": entity.type
+                     })
```

### Comparing `promg-1.0.9/src/promg/data_managers/datastructures.py` & `promg-1.1.0/src/promg/data_managers/datastructures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,686 +1,700 @@
-import json
-import os
-import re
-import warnings
-import random
-from pathlib import Path
-
-from typing import List, Dict, Any, Optional
-from dataclasses import dataclass
-
-import numpy as np
-import pandas as pd
-from pandas import DataFrame
-
-from .semantic_header import RecordConstructor
-from ..utilities.auxiliary_functions import replace_undefined_value, create_list
-from ..utilities.configuration import Configuration
-
-
-@dataclass
-class DatetimeObject:
-    format: str
-    timezone_offset: str
-    convert_to: str
-    is_epoch: bool
-    unit: str
-
-    def get_date_type(self):
-        if self.convert_to == "ISO_DATE":
-            return "DATE"
-        else:
-            return "DATE_TIME"
-
-    @staticmethod
-    def from_dict(obj: Any) -> 'DatetimeObject':
-        if obj is None:
-            return None
-        _format = obj.get("format")
-        _timezone_offset = replace_undefined_value(obj.get("timezone_offset"), "")
-        _convert_to = "ISO_DATE"
-        if re.search('[hkHK]', _format):
-            _convert_to = "ISO_DATE_TIME"
-
-        # _convert_to = str(obj.get("convert_to"))
-        _is_epoch = replace_undefined_value(obj.get("is_epoch"), False)
-        _unit = obj.get("unit")
-        return DatetimeObject(_format, _timezone_offset, _convert_to, _is_epoch, _unit)
-
-
-@dataclass
-class Column:
-    name: str
-    dtype: str
-    nan_values: List[str]
-    optional: bool
-    range_start: int
-    range_end: int
-
-    @staticmethod
-    def from_dict(obj: Any) -> Optional['Column']:
-        if obj is None:
-            return None
-        _name = obj.get("name")
-        _dtype = obj.get("dtype")
-        _nan_values = replace_undefined_value(obj.get("nan_values"), [])
-        _optional = replace_undefined_value(obj.get("optional"), False)
-        _range_start = obj.get("range_start")
-        _range_end = obj.get("range_end")
-        return Column(_name, _dtype, _nan_values, _optional, _range_start, _range_end)
-
-
-@dataclass
-class Attribute:
-    name: str
-    columns: List[Column]
-    separator: str
-    is_datetime: bool
-    is_compound: bool
-    optional: bool
-    datetime_object: DatetimeObject
-    na_rep_value: Any
-    na_rep_columns: List[Column]
-    filter_exclude_values: List[str]
-    filter_include_values: List[str]
-    use_filter: bool
-    is_primary_key: bool
-    is_foreign_key: bool
-
-    @staticmethod
-    def from_dict(obj: Any) -> Optional['Attribute']:
-        if obj is None:
-            return None
-        _name = obj.get("name")
-        _columns = create_list(Column, obj.get("columns"))
-        _is_compound = len(_columns) > 1
-        _optional = bool(obj.get("optional"))
-        _datetime_object = DatetimeObject.from_dict(obj.get("datetime_object"))
-        _is_datetime = _datetime_object is not None
-        _na_rep_value = obj.get("na_rep_value")
-        _na_rep_columns = create_list(Column, obj.get("na_rep_columns"))
-        _separator = obj.get("separator")
-        _filter_exclude_values = obj.get("filter_exclude_values")
-        _filter_include_values = obj.get("filter_include_values")
-        _use_filter = _filter_include_values is not None or _filter_exclude_values is not None  # default value
-        _use_filter = replace_undefined_value(obj.get("use_filter"), _use_filter)
-        _is_primary_key = replace_undefined_value(obj.get("is_primary_key"), False)
-        _is_foreign_key = replace_undefined_value(obj.get("is_foreign_key"), False)
-        return Attribute(name=_name, optional=_optional, columns=_columns, separator=_separator,
-                         is_compound=_is_compound,
-                         is_datetime=_is_datetime, datetime_object=_datetime_object,
-                         na_rep_value=_na_rep_value, na_rep_columns=_na_rep_columns,
-                         filter_exclude_values=_filter_exclude_values, filter_include_values=_filter_include_values,
-                         use_filter=_use_filter, is_primary_key=_is_primary_key, is_foreign_key=_is_foreign_key)
-
-
-@dataclass
-class Sample:
-    file_name: str
-    use_random_sample: bool
-    population_column: str
-    size: int
-    ids: List[Any]
-    between: List[str]
-    format: Optional[str]
-
-    @staticmethod
-    def from_dict(obj: Any, default_file_name: Optional[str] = None) -> Optional['Sample']:
-        if obj is None:
-            return None
-        # when there is a single file specified, then we can use the default file name
-        if default_file_name is not None:
-            _file_name = replace_undefined_value(obj.get("file_name"), default_file_name)
-        else:
-            _file_name = obj.get("file_name")
-        _use_random_sample = obj.get("use_random_sample")
-        _population_column = obj.get("population_column")
-        _size = obj.get("size")
-        _ids = obj.get("ids")
-        _between = obj.get("between")
-        _format = obj.get("datetime_format")
-
-        return Sample(_file_name, _use_random_sample, _population_column, _size, _ids, _between, _format)
-
-
-class DataStructure:
-    def __init__(self, include: bool, name: str, file_directory: str, file_names: List[str],
-                 encoding: str, seperator: str, decimal: str,
-                 labels: List[str], true_values: List[str], false_values: List[str],
-                 add_log: bool, add_index: bool,
-                 samples: Dict[str, Sample], attributes: Dict[str, Attribute],
-                 split_combined_events: bool):
-        self.include = include
-        self.name = name
-        self.file_directory = file_directory
-        self.preprocessed_file_directory = os.path.join(self.file_directory, "preprocessed_files")
-        self.file_names = file_names
-        self.encoding = encoding
-        self.seperator = seperator
-        self.decimal = decimal
-        self.labels = labels
-        if self.labels == ["Record"]:
-            self.labels = None
-        self.true_values = true_values
-        self.false_values = false_values
-        self.add_log = add_log
-        self.add_index = add_index
-        self.samples = samples
-        self.attributes = attributes
-        self.split_combined_events = split_combined_events
-        self.required_labels = None
-
-    def __repr__(self):
-        return self.name
-
-    def has_datetime_attribute(self):
-        return any([attribute.is_datetime for attribute in self.attributes.values()])
-        # return "Event" in self.labels or "EventRecord" in self.labels
-
-    def contains_composed_events(self):
-        contains_composed_events = "startTimestamp" in self.get_datetime_formats() \
-                                   or "completeTimestamp" in self.get_datetime_formats()
-        return self.has_datetime_attribute() and contains_composed_events
-
-    @staticmethod
-    def from_dict(obj: Any) -> Optional['DataStructure']:
-        if obj is None:
-            return None
-
-        _include = replace_undefined_value(obj.get("include"), True)
-
-        if not _include:
-            return None
-
-        _name = obj.get("name")
-        _path_of_executed_file = os.getcwd()
-        _file_directory = os.path.join(os.getcwd(), *obj.get("file_directory").split("\\"))
-        _file_names = obj.get("file_names") if obj.get("file_names") is not None else [obj.get("file_name")]
-        _encoding = replace_undefined_value(obj.get("encoding"), "utf-8")
-        _seperator = replace_undefined_value(obj.get("seperator"), ",")
-        _decimal = replace_undefined_value(obj.get("decimal"), ".")
-        _labels = obj.get("labels")
-        _true_values = obj.get("true_values")
-        _false_values = obj.get("false_values")
-        _add_log = replace_undefined_value(obj.get("add_log"), False)
-        _add_index = replace_undefined_value(obj.get("add_index"), True)
-
-        _samples_obj = obj.get("samples") if obj.get("samples") is not None else obj.get("sample")
-        if len(_file_names) == 1:  # single file name is defined
-            _samples = create_list(Sample, _samples_obj, _file_names[0])
-        else:
-            _samples = create_list(Sample, _samples_obj)
-
-        _samples = {sample.file_name: sample for sample in _samples}
-        _attributes = create_list(Attribute, obj.get("attributes"))
-        _attributes = {attribute.name: attribute for attribute in _attributes}
-        _split_combined_events = replace_undefined_value(obj.get("split_combined_events"), False)
-
-        return DataStructure(_include, _name, _file_directory, _file_names, _encoding, _seperator, _decimal,
-                             _labels, _true_values, _false_values, _add_log, _add_index,
-                             _samples, _attributes, _split_combined_events)
-
-    def get_primary_keys(self):
-        return [attribute_name for attribute_name, attribute in self.attributes.items() if attribute.is_primary_key]
-
-    def get_primary_keys_as_attributes(self):
-        primary_keys = self.get_primary_keys()
-        primary_key_with = [f"n.{primary_key} as {primary_key}" for primary_key in primary_keys]
-        primary_key_string = ", ".join(primary_key_with)
-        return primary_key_string
-
-    def get_label_string(self):
-        return ":".join(self.labels)
-
-    def get_foreign_keys(self):
-        return [attribute_name for attribute_name, attribute in self.attributes.items() if attribute.is_foreign_key]
-
-    def get_dtype_dict(self):
-        dtypes = {}
-        for attribute in self.attributes.values():
-            for column in attribute.columns:
-                if column.dtype is not None:
-                    if column.name not in dtypes:
-                        dtypes[column.name] = column.dtype
-                    elif column.dtype != dtypes[column.name]:
-                        warnings.warn(
-                            f"Multiple dtypes ({column.dtype} != {dtypes[column.name]}) "
-                            f"defined for {column.name}")
-        return dtypes
-
-    def get_required_columns(self):
-        required_columns = set()
-        for attribute in self.attributes.values():
-            # add column names to the required columns
-            required_columns.update([x.name for x in attribute.columns])
-            required_columns.update([x.name for x in attribute.na_rep_columns])
-
-        return list(required_columns)
-
-    def create_sample(self, file_name, df_log):
-        if self.samples is None or file_name not in self.samples:
-            warnings.warn(f"No sample population has been defined for {self.name}")
-            return df_log
-
-        sample = self.samples[file_name]
-        sample_column = sample.population_column
-        if sample.use_random_sample:
-            random_selection = random.sample(df_log[sample_column].unique().tolist(), k=sample.size)
-            df_log = df_log[df_log[sample_column].isin(random_selection)]
-        else:
-            if sample.ids is not None:
-                random_selection = sample.ids
-                df_log = df_log[df_log[sample_column].isin(random_selection)]
-            elif sample.between is not None:
-                start_date = sample.between[0]
-                end_date = sample.between[1]
-                df_log['date_time_conv'] = pd.to_datetime(df_log[sample_column], format=sample.format)
-                df_log = df_log.loc[df_log["date_time_conv"].between(start_date, end_date)]
-                df_log = df_log.drop(columns=['date_time_conv'])
-
-        df_log = df_log.reset_index(drop=True)
-        return df_log
-
-    @staticmethod
-    def replace_nan_values_based_on_na_rep_columns(df_log, attribute):
-        if len(attribute.na_rep_columns) != len(attribute.columns):
-            raise Exception(
-                f"Na_rep_columns does not have the same size as columns for attribute {attribute.name}")
-        else:  # they are the same size
-            for i, na_rep_column in zip(range(len(attribute.na_rep_columns)), attribute.na_rep_columns):
-                attribute_name = f"{attribute.name}_{i}"
-                df_log[attribute_name].fillna(df_log[na_rep_column.name], inplace=True)
-
-        return df_log
-
-    @staticmethod
-    def replace_nan_values_based_on_na_rep_value(df_log, attribute):
-        for i in range(len(attribute.columns)):
-            attribute_name = f"{attribute.name}_{i}"
-            df_log[attribute_name].fillna(attribute.na_rep_value, inplace=True)
-
-        return df_log
-
-    @staticmethod
-    def replace_nan_values_with_unknown(df_log, attribute):
-        column: Column
-        for i, column in zip(range(len(attribute.columns)), attribute.columns):
-            attribute_name = f"{attribute.name}_{i}"
-            if not column.optional:
-                try:
-                    df_log[attribute_name].fillna("Unknown", inplace=True)
-                except:
-                    df_log[attribute_name].fillna(-1, inplace=True)
-        return df_log
-
-    @staticmethod
-    def create_compound_attribute(df_log, attribute):
-        compound_column_names = [x.name for x in attribute.columns]
-        df_log[attribute.name] = df_log[compound_column_names].apply(
-            lambda row: attribute.separator.join([value for value in row.values.astype(str) if
-                                                  not (value == 'nan' or value != value)]), axis=1)
-        return df_log
-
-    @staticmethod
-    def combine_attribute_columns(df_log, attribute):
-        compound_attribute_names = [f"{attribute.name}_{i}" for i in range(len(attribute.columns))]
-        if attribute.is_compound:
-            df_log[f"{attribute.name}_attribute"] = df_log[compound_attribute_names].apply(
-                lambda row: attribute.separator.join([value for value in row.values.astype(str) if
-                                                      not (value == 'nan' or value != value)]), axis=1)
-        else:
-            df_log[f"{attribute.name}_attribute"] = df_log[f"{attribute.name}_0"]
-        df_log = df_log.drop(columns=compound_attribute_names)
-        return df_log
-
-    @staticmethod
-    def create_attribute_columns(df_log, attribute):
-        for i, column in zip(range(len(attribute.columns)), attribute.columns):
-            attribute_name = f"{attribute.name}_{i}"
-            df_log[attribute_name] = df_log[column.name]
-            if column.range_start is not None or column.range_end is not None:
-                df_log[attribute_name] = df_log[attribute_name].str[column.range_start:column.range_end]
-        return df_log
-
-    @staticmethod
-    def replace_with_nan(df_log, attribute):
-        for i, column in zip(range(len(attribute.columns)), attribute.columns):
-            attribute_name = f"{attribute.name}_{i}"
-            for nan_value in column.nan_values:
-                df_log[attribute_name] = df_log[attribute_name].replace(nan_value, np.nan, regex=False)
-        return df_log
-
-    def preprocess_according_to_attributes(self, df_log):
-        # loop over all attributes and check if they should be created, renamed or imputed
-        for attribute in self.attributes.values():
-            df_log = DataStructure.create_attribute_columns(df_log, attribute)
-            df_log = DataStructure.replace_with_nan(df_log, attribute)
-            if len(attribute.na_rep_columns) > 0:  # impute values in case of missing values
-                df_log = DataStructure.replace_nan_values_based_on_na_rep_columns(df_log, attribute)
-            if attribute.na_rep_value is not None:
-                df_log = DataStructure.replace_nan_values_based_on_na_rep_value(df_log, attribute)
-
-            df_log = DataStructure.combine_attribute_columns(df_log, attribute)
-
-        return df_log
-
-    def split_df_log_into_combined_events(self, df_log: DataFrame):
-        df_log["idx"] = df_log.reset_index().index
-        if "timestamp" in self.attributes:
-            raise ImportError(
-                "Combined events cannot be split since an attribute with name timestamp is already defined")
-
-        if "startTimestamp" in self.attributes and "completeTimestamp" in self.attributes:
-            df_log_start = df_log.drop(columns=["completeTimestamp"])
-            df_log_start["lifecycle"] = "start"
-            df_log_start = df_log_start.rename(columns={"startTimestamp": "timestamp"})
-
-            df_log_end = df_log.drop(columns=["startTimestamp"])
-            df_log_end["lifecycle"] = "complete"
-            df_log_end = df_log_end.rename(columns={"completeTimestamp": "timestamp"})
-
-            df_log = pd.concat([df_log_start, df_log_end])
-        elif "startTimestamp" in self.attributes:
-            df_log["lifecycle"] = "start"
-            df_log = df_log.rename(columns={"startTimestamp": "timestamp"})
-        elif "completeTimestamp" in self.attributes:
-            df_log["lifecycle"] = "complete"
-            df_log = df_log.rename(columns={"completeTimestamp": "timestamp"})
-
-        df_log = df_log.sort_values(by=["timestamp", "idx"])
-        df_log = df_log.drop(columns=["idx"])
-        return df_log
-
-    def update_attributes(self):
-        if "startTimestamp" in self.attributes and "completeTimestamp" in self.attributes:
-            start_dt_format = self.get_datetime_formats()["startTimestamp"].format
-            complete_dt_format = self.get_datetime_formats()["completeTimestamp"].format
-            if start_dt_format != complete_dt_format:
-                raise ValueError("startTimestamp and completeTimestamp have a different format")
-
-            start_attribute = self.attributes["startTimestamp"]
-            start_attribute.name = "timestamp"
-            self.attributes["timestamp"] = start_attribute
-            del self.attributes["startTimestamp"]
-            del self.attributes["completeTimestamp"]
-
-
-        elif "startTimestamp" in self.attributes:
-            start_attribute = self.attributes["startTimestamp"]
-            start_attribute.name = "timestamp"
-
-            self.attributes["timestamp"] = start_attribute
-            del self.attributes["startTimestamp"]
-        elif "completeTimestamp" in self.attributes:
-            complete_attribute = self.attributes["completeTimestamp"]
-            complete_attribute.name = "timestamp"
-
-            self.attributes["timestamp"] = complete_attribute
-            del self.attributes["completeTimestamp"]
-
-    def check_if_required_attributes_are_present(self, record_constructor):
-        # loop over all required attributes of the record constructor
-        # --> check whether they are required by self
-        required = True
-        for required_attribute in record_constructor.required_attributes:
-            if required_attribute == "index":  # records of an always have an index, so records will have
-                # the required attributes = index
-                continue
-            if required_attribute not in self.attributes or self.attributes[required_attribute].optional:
-                # if the required attribute does not occur in the self.attributes or the attribute is
-                # optional, then the record_constructor labels are not required
-                required = False
-        return required
-
-    def determine_required_labels(self, records: List["RecordConstructor"]):
-        # determine the required labels for the records defined by this datastructure
-        # therefore, we have to check for all record constructors in records
-        # whether the required attributes are present by the dataset description definition
-
-        # initially, self.required_labels might be None, hence we need to make it an empty list.
-        if self.required_labels is None:
-            self.required_labels = []
-
-        # loop over all record_constructors in records
-        for record_constructor in records:
-            # check whether self.labels appear in the record constructor
-            if self.labels_appear_in_record_constructor(record_constructor):
-                if record_constructor.prevalent_record.where_condition != "":
-                    # a where condition is specified, then not all records require the record_constructor labels
-                    required = False
-                else:
-                    required = self.check_if_required_attributes_are_present(record_constructor)
-                if required:
-                    # if required = true, then the record_constructor labels are required labels of self
-                    self.required_labels.extend(record_constructor.record_labels)
-        self.required_labels = list(set(self.required_labels))
-
-    def get_required_labels(self, records: List["RecordConstructor"]):
-        if self.required_labels is None:
-            self.determine_required_labels(records)
-        return self.required_labels
-
-    def get_required_labels_str(self, records: List["RecordConstructor"]):
-        """Method to convert the required labels determined by records to a string seperated by :
-        :param records: the required
-        """
-        if self.required_labels is None:
-            self.determine_required_labels(records)
-        required_labels_w_records = self.required_labels[:]
-        required_labels_w_records.insert(0, "Record")
-        required_labels_str = ":".join(required_labels_w_records)
-        return required_labels_str
-
-    def read_data_set(self, file_name, use_sample, load_status: int, store_preprocessed_file=True,
-                      use_preprocessed_file=False):
-        preprocessed_file_name = self._get_preprocessed_file_name(file_name, use_sample)
-        df_log = None
-        if use_preprocessed_file:
-            df_log = self.read_preprocessed_df_log(preprocessed_file_name)
-        if df_log is None:  # no preprocessed file was read
-            df_log = self.read_df_log(file_name, use_sample)
-            if store_preprocessed_file:
-                self.store_df_log(df_log, preprocessed_file_name)
-
-        df_log["loadStatus"] = load_status
-        return df_log
-
-    def read_df_log(self, file_name, use_sample):
-        df_log = self.prepare_event_data_sets(file_name, use_sample)
-        return df_log
-
-    def read_preprocessed_df_log(self, preprocessed_file_name):
-        preprocessed_file_path = os.path.join(self.preprocessed_file_directory, preprocessed_file_name)
-        # first try to read preprocessed file
-        if not os.path.exists(preprocessed_file_path):
-            warning_message = f"No preprocessed file {preprocessed_file_name} found, preprocessed the file " \
-                              f"instead"
-            warnings.warn(warning_message)
-            return None
-        else:  # use_preprocessed_file and file exists
-            df_log = pd.read_pickle(preprocessed_file_path)
-        return df_log
-
-    def store_df_log(self, df_log, preprocessed_file_name):
-        # only store file if we did not read from the stored file
-        os.makedirs(self.preprocessed_file_directory, exist_ok=True)
-
-        preprocessed_file_path = os.path.join(self.preprocessed_file_directory, preprocessed_file_name)
-        df_log.to_pickle(preprocessed_file_path)
-
-    def _get_preprocessed_file_name(self, file_name, use_sample):
-        # change extension from csv to pkl and add sample in case of sample
-        sample_is_used = use_sample and len(self.samples) > 0
-        preprocessed_file_name = f"{file_name[:-4]}_sample.pkl" if sample_is_used else f"{file_name[:-4]}.pkl"
-        return preprocessed_file_name
-
-    @staticmethod
-    def create_record_id_column(df_log, file_name):
-        record_id_column = df_log.index
-        record_id_column = record_id_column.astype(str) + "_" + file_name[:-4]
-        return record_id_column
-
-    def prepare_event_data_sets(self, file_name, use_sample):
-        dtypes = self.get_dtype_dict()
-        required_columns = self.get_required_columns()
-
-        true_values = self.true_values
-        false_values = self.false_values
-
-        if file_name.endswith('.csv'):
-            df_log: DataFrame = pd.read_csv(os.path.join(self.file_directory, file_name), keep_default_na=True,
-                                            usecols=required_columns, dtype=dtypes, true_values=true_values,
-                                            false_values=false_values, sep=self.seperator, decimal=self.decimal,
-                                            encoding=self.encoding)
-        else:
-            raise TypeError(f"The file extension of {file_name} is not implemented. Use .csv.")
-
-        if use_sample and self.has_datetime_attribute():
-            df_log = self.create_sample(file_name, df_log)
-
-        df_log = self.preprocess_according_to_attributes(df_log)
-
-        # all columns have been renamed to or constructed with the name attribute,
-        # hence only keep those that match with a name attribute
-        required_attributes = list([f"{attribute_name}_attribute" for attribute_name in self.attributes.keys()])
-        required_attributes_mapping = {f"{attribute_name}_attribute": f"{attribute_name}" for attribute_name in
-                                       self.attributes.keys()}
-        df_log = df_log[required_attributes]
-        df_log = df_log.rename(columns=required_attributes_mapping)
-
-        if self.split_combined_events:
-            df_log = self.split_df_log_into_combined_events(df_log)
-            self.update_attributes()
-
-        if self.add_log:
-            df_log["log"] = file_name
-
-        if self.add_index:
-            df_log["index"] = df_log.index
-
-        # drop all columns with only nan values
-        df_log = df_log.dropna(how='all', axis=1)  # drop all columns in which all values are nan (empty)
-        df_log = df_log.dropna(how='all')  # drop all columns in which all values are nan (empty)
-
-        df_log["recordId"] = self.create_record_id_column(df_log, file_name)
-
-        return df_log
-
-    def determine_optional_labels_in_log(self, df_log, records):
-        df_log["labels"] = ""
-
-        if self.required_labels is None:
-            self.determine_required_labels(records)
-
-        if set(self.required_labels) == set(self.labels):
-            return df_log
-
-        for record_constructor in records:
-            if self.labels_appear_in_record_constructor(record_constructor):
-                if set(record_constructor.record_labels) <= set(self.required_labels):
-                    continue  # record constructor only contains required labels
-
-                # one of possible labels appear in record constructor
-                should_have_label = self.all_required_attributes_are_present_in_df_log(df_log, record_constructor)
-                if should_have_label.any():  # check whether there is still a row that can have the label
-                    should_have_label = should_have_label & self.is_where_condition_satisfied(
-                        df_log, record_constructor)
-                if should_have_label.any():
-                    for label in record_constructor.record_labels:
-                        df_log.loc[should_have_label, "labels"] += ":" + label
-
-        return df_log
-
-    def labels_appear_in_record_constructor(self, record_constructor):
-        if self.labels is not None:
-            # check whether the labels have overlap with the labels of the record_constructor
-            intersection = list(set(self.labels) & set(record_constructor.record_labels))
-        else:
-            # no labels are defined, hence we consider all labels of the record constructor
-            intersection = record_constructor.record_labels
-
-        return len(intersection) > 0
-
-    def all_required_attributes_are_present_in_df_log(self, df_log, record_constructor):
-        required_attributes_are_present = pd.Series(True, index=np.arange(len(df_log)), name='present')
-        for required_attribute in record_constructor.required_attributes:
-            if required_attribute == "index" or required_attribute == "log":
-                continue
-            if required_attribute in self.attributes:
-                if self.attributes[required_attribute].optional:
-                    # if the required attribute is optional in the structure, check whether the required attribute is
-                    # not null
-                    required_attributes_are_present = required_attributes_are_present & df_log[
-                        required_attribute].notnull()
-                # else the required attributes is required in the structure, hence nothing changes
-            else:  # the required attribute is missing in the structure -> hence not all are present
-                required_attributes_are_present = pd.Series(False, index=np.arange(len(df_log)), name='present')
-                # since for all rows, at least an attribute is missing, we can return
-                return required_attributes_are_present
-
-        return required_attributes_are_present
-
-    @staticmethod
-    def is_where_condition_satisfied(df_log, record_constructor):
-        # TODO split where_condition
-        where_condition = record_constructor.prevalent_record.where_condition
-        where_condition_satisfied = pd.Series(True, index=np.arange(len(df_log)), name='satisfied')
-        if where_condition == "":
-            return where_condition_satisfied
-        where_conditions = where_condition.split("AND")
-        for condition in where_conditions:
-            stripped_condition = condition.strip()
-            if "=" in condition:
-                condition_list = stripped_condition.split("=")
-                column_name = condition_list[0].strip()
-                if "." in column_name:
-                    column_name = column_name.split(".")[1].strip()
-                column_value = condition_list[1].strip().strip('"')
-                where_condition_satisfied = where_condition_satisfied & (
-                        df_log[column_name].astype("string") == column_value)
-            elif "STARTS WITH" in condition:
-                condition_list = stripped_condition.split("STARTS WITH")
-                column_name = condition_list[0].strip()
-                if "." in column_name:
-                    column_name = column_name.split(".")[1].strip()
-                column_value = condition_list[1].strip().strip('"')
-                where_condition_satisfied = where_condition_satisfied & df_log[
-                    column_name].str.startswith(column_value)
-            elif "ENDS WITH" in condition:
-                condition_list = stripped_condition.split("ENDS WITH")
-                column_name = condition_list[0].strip()
-                if "." in column_name:
-                    column_name = column_name.split(".")[1].strip()
-                column_value = condition_list[1].strip().strip('"')
-                where_condition_satisfied = where_condition_satisfied & df_log[
-                    column_name].str.endswith(column_value)
-        return where_condition_satisfied
-
-    def get_datetime_formats(self) -> Dict[str, DatetimeObject]:
-        datetime_formats = {}
-
-        for attribute_name, attribute in self.attributes.items():
-            if attribute.is_datetime:
-                datetime_formats[attribute_name] = attribute.datetime_object
-
-        return datetime_formats
-
-    def get_attribute_value_pairs_filtered(self, exclude: bool) -> Dict[str, List[str]]:
-        attribute_value_pairs = {}
-        for attribute_name, attribute in self.attributes.items():
-            if attribute.use_filter:
-                attribute_value_pairs[attribute_name] \
-                    = attribute.filter_exclude_values if exclude else attribute.filter_include_values
-
-        return attribute_value_pairs
-
-
-class DatasetDescriptions:
-    def __init__(self, config: Configuration):
-        path = config.dataset_description_path
-
-        random.seed(1)
-        with open(path, encoding='utf-8') as f:
-            json_event_tables = json.load(f)
-
-        self.structures = [DataStructure.from_dict(item) for item in json_event_tables]
-        self.structures = [item for item in self.structures if item is not None]
+import json
+import os
+import re
+import warnings
+import random
+from pathlib import Path
+
+from typing import List, Dict, Any, Optional
+from dataclasses import dataclass
+
+import numpy as np
+import pandas as pd
+from pandas import DataFrame
+
+from .semantic_header import RecordConstructor
+from ..utilities.auxiliary_functions import replace_undefined_value, create_list
+from ..utilities.configuration import Configuration
+
+
+@dataclass
+class DatetimeObject:
+    format: str
+    timezone_offset: str
+    convert_to: str
+    is_epoch: bool
+    unit: str
+
+    def get_date_type(self):
+        if self.convert_to == "ISO_DATE":
+            return "DATE"
+        else:
+            return "DATE_TIME"
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'DatetimeObject':
+        if obj is None:
+            return None
+        _format = obj.get("format")
+        _timezone_offset = replace_undefined_value(obj.get("timezone_offset"), "")
+        _convert_to = "ISO_DATE"
+        if re.search('[hkHK]', _format):
+            _convert_to = "ISO_DATE_TIME"
+
+        # _convert_to = str(obj.get("convert_to"))
+        _is_epoch = replace_undefined_value(obj.get("is_epoch"), False)
+        _unit = obj.get("unit")
+        return DatetimeObject(_format, _timezone_offset, _convert_to, _is_epoch, _unit)
+
+
+@dataclass
+class Column:
+    name: str
+    dtype: str
+    nan_values: List[str]
+    optional: bool
+    range_start: int
+    range_end: int
+
+    @staticmethod
+    def from_dict(obj: Any) -> Optional['Column']:
+        if obj is None:
+            return None
+        _name = obj.get("name")
+        _dtype = obj.get("dtype")
+        _nan_values = replace_undefined_value(obj.get("nan_values"), [])
+        _optional = replace_undefined_value(obj.get("optional"), False)
+        _range_start = obj.get("range_start")
+        _range_end = obj.get("range_end")
+        return Column(_name, _dtype, _nan_values, _optional, _range_start, _range_end)
+
+
+@dataclass
+class Attribute:
+    name: str
+    columns: List[Column]
+    separator: str
+    is_datetime: bool
+    is_compound: bool
+    optional: bool
+    datetime_object: DatetimeObject
+    na_rep_value: Any
+    na_rep_columns: List[Column]
+    filter_exclude_values: List[str]
+    filter_include_values: List[str]
+    use_filter: bool
+    is_primary_key: bool
+    is_foreign_key: bool
+
+    @staticmethod
+    def from_dict(obj: Any) -> Optional['Attribute']:
+        if obj is None:
+            return None
+        _name = obj.get("name")
+        _columns = create_list(Column, obj.get("columns"))
+        _is_compound = len(_columns) > 1
+        _optional = bool(obj.get("optional"))
+        _datetime_object = DatetimeObject.from_dict(obj.get("datetime_object"))
+        _is_datetime = _datetime_object is not None
+        _na_rep_value = obj.get("na_rep_value")
+        _na_rep_columns = create_list(Column, obj.get("na_rep_columns"))
+        _separator = obj.get("separator")
+        _filter_exclude_values = obj.get("filter_exclude_values")
+        _filter_include_values = obj.get("filter_include_values")
+        _use_filter = _filter_include_values is not None or _filter_exclude_values is not None  # default value
+        _use_filter = replace_undefined_value(obj.get("use_filter"), _use_filter)
+        _is_primary_key = replace_undefined_value(obj.get("is_primary_key"), False)
+        _is_foreign_key = replace_undefined_value(obj.get("is_foreign_key"), False)
+        return Attribute(name=_name, optional=_optional, columns=_columns, separator=_separator,
+                         is_compound=_is_compound,
+                         is_datetime=_is_datetime, datetime_object=_datetime_object,
+                         na_rep_value=_na_rep_value, na_rep_columns=_na_rep_columns,
+                         filter_exclude_values=_filter_exclude_values, filter_include_values=_filter_include_values,
+                         use_filter=_use_filter, is_primary_key=_is_primary_key, is_foreign_key=_is_foreign_key)
+
+
+@dataclass
+class Sample:
+    file_name: str
+    use_random_sample: bool
+    population_column: str
+    size: int
+    ids: List[Any]
+    between: List[str]
+    format: Optional[str]
+
+    @staticmethod
+    def from_dict(obj: Any, default_file_name: Optional[str] = None) -> Optional['Sample']:
+        if obj is None:
+            return None
+        # when there is a single file specified, then we can use the default file name
+        if default_file_name is not None:
+            _file_name = replace_undefined_value(obj.get("file_name"), default_file_name)
+        else:
+            _file_name = obj.get("file_name")
+        _use_random_sample = obj.get("use_random_sample")
+        _population_column = obj.get("population_column")
+        _size = obj.get("size")
+        _ids = obj.get("ids")
+        _between = obj.get("between")
+        _format = obj.get("datetime_format")
+
+        return Sample(_file_name, _use_random_sample, _population_column, _size, _ids, _between, _format)
+
+
+class DataStructure:
+    def __init__(self, include: bool, name: str, file_directory: str, file_names: List[str],
+                 encoding: str, seperator: str, decimal: str,
+                 labels: List[str], true_values: List[str], false_values: List[str],
+                 add_log: bool, add_index: bool,
+                 samples: Dict[str, Sample], attributes: Dict[str, Attribute],
+                 split_combined_events: bool):
+        self.include = include
+        self.name = name
+        self.file_directory = file_directory
+        self.preprocessed_file_directory = os.path.join(self.file_directory, "preprocessed_files")
+        self.file_names = file_names
+        self.encoding = encoding
+        self.seperator = seperator
+        self.decimal = decimal
+        self.labels = labels
+        if self.labels == ["Record"]:
+            self.labels = None
+        self.true_values = true_values
+        self.false_values = false_values
+        self.add_log = add_log
+        self.add_index = add_index
+        self.samples = samples
+        self.attributes = attributes
+        self.split_combined_events = split_combined_events
+        self.required_labels = None
+
+    def __repr__(self):
+        return self.name
+
+    def has_datetime_attribute(self):
+        return any([attribute.is_datetime for attribute in self.attributes.values()])
+        # return "Event" in self.labels or "EventRecord" in self.labels
+
+    def contains_composed_events(self):
+        contains_composed_events = "startTimestamp" in self.get_datetime_formats() \
+                                   or "completeTimestamp" in self.get_datetime_formats()
+        return self.has_datetime_attribute() and contains_composed_events
+
+    @staticmethod
+    def from_dict(obj: Any) -> Optional['DataStructure']:
+        if obj is None:
+            return None
+
+        _include = replace_undefined_value(obj.get("include"), True)
+
+        if not _include:
+            return None
+
+        _name = obj.get("name")
+        _path_of_executed_file = os.getcwd()
+        _file_directory = os.path.join(os.getcwd(), *obj.get("file_directory").split("\\"))
+        _file_names = obj.get("file_names") if obj.get("file_names") is not None else [obj.get("file_name")]
+        _encoding = replace_undefined_value(obj.get("encoding"), "utf-8")
+        _seperator = replace_undefined_value(obj.get("seperator"), ",")
+        _decimal = replace_undefined_value(obj.get("decimal"), ".")
+        _labels = obj.get("labels")
+        _true_values = obj.get("true_values")
+        _false_values = obj.get("false_values")
+        _add_log = replace_undefined_value(obj.get("add_log"), False)
+        _add_index = replace_undefined_value(obj.get("add_index"), True)
+
+        _samples_obj = obj.get("samples") if obj.get("samples") is not None else obj.get("sample")
+        if len(_file_names) == 1:  # single file name is defined
+            _samples = create_list(Sample, _samples_obj, _file_names[0])
+        else:
+            _samples = create_list(Sample, _samples_obj)
+
+        _samples = {sample.file_name: sample for sample in _samples}
+        _attributes = create_list(Attribute, obj.get("attributes"))
+        _attributes = {attribute.name: attribute for attribute in _attributes}
+        _split_combined_events = replace_undefined_value(obj.get("split_combined_events"), False)
+
+        return DataStructure(_include, _name, _file_directory, _file_names, _encoding, _seperator, _decimal,
+                             _labels, _true_values, _false_values, _add_log, _add_index,
+                             _samples, _attributes, _split_combined_events)
+
+    def get_primary_keys(self):
+        return [attribute_name for attribute_name, attribute in self.attributes.items() if attribute.is_primary_key]
+
+    def get_primary_keys_as_attributes(self):
+        primary_keys = self.get_primary_keys()
+        primary_key_with = [f"n.{primary_key} as {primary_key}" for primary_key in primary_keys]
+        primary_key_string = ", ".join(primary_key_with)
+        return primary_key_string
+
+    def get_label_string(self):
+        return ":".join(self.labels)
+
+    def get_foreign_keys(self):
+        return [attribute_name for attribute_name, attribute in self.attributes.items() if attribute.is_foreign_key]
+
+    def get_dtype_dict(self):
+        dtypes = {}
+        for attribute in self.attributes.values():
+            for column in attribute.columns:
+                if column.dtype is not None:
+                    if column.name not in dtypes:
+                        dtypes[column.name] = column.dtype
+                    elif column.dtype != dtypes[column.name]:
+                        warnings.warn(
+                            f"Multiple dtypes ({column.dtype} != {dtypes[column.name]}) "
+                            f"defined for {column.name}")
+        return dtypes
+
+    def get_required_columns(self):
+        required_columns = set()
+        for attribute in self.attributes.values():
+            # add column names to the required columns
+            required_columns.update([x.name for x in attribute.columns])
+            required_columns.update([x.name for x in attribute.na_rep_columns])
+
+        return list(required_columns)
+
+    def create_sample(self, file_name, df_log):
+        if self.samples is None or file_name not in self.samples:
+            warnings.warn(f"No sample population has been defined for {self.name}")
+            return df_log
+
+        sample = self.samples[file_name]
+        sample_column = sample.population_column
+        if sample.use_random_sample:
+            random_selection = random.sample(df_log[sample_column].unique().tolist(), k=sample.size)
+            df_log = df_log[df_log[sample_column].isin(random_selection)]
+        else:
+            if sample.ids is not None:
+                random_selection = sample.ids
+                df_log = df_log[df_log[sample_column].isin(random_selection)]
+            elif sample.between is not None:
+                start_date = sample.between[0]
+                end_date = sample.between[1]
+                df_log['date_time_conv'] = pd.to_datetime(df_log[sample_column], format=sample.format)
+                df_log = df_log.loc[df_log["date_time_conv"].between(start_date, end_date)]
+                df_log = df_log.drop(columns=['date_time_conv'])
+
+        df_log = df_log.reset_index(drop=True)
+        return df_log
+
+    @staticmethod
+    def replace_nan_values_based_on_na_rep_columns(df_log, attribute):
+        if len(attribute.na_rep_columns) != len(attribute.columns):
+            raise Exception(
+                f"Na_rep_columns does not have the same size as columns for attribute {attribute.name}")
+        else:  # they are the same size
+            for i, na_rep_column in zip(range(len(attribute.na_rep_columns)), attribute.na_rep_columns):
+                attribute_name = f"{attribute.name}_{i}"
+                df_log[attribute_name].fillna(df_log[na_rep_column.name], inplace=True)
+
+        return df_log
+
+    @staticmethod
+    def replace_nan_values_based_on_na_rep_value(df_log, attribute):
+        for i in range(len(attribute.columns)):
+            attribute_name = f"{attribute.name}_{i}"
+            df_log[attribute_name].fillna(attribute.na_rep_value, inplace=True)
+
+        return df_log
+
+    @staticmethod
+    def replace_nan_values_with_unknown(df_log, attribute):
+        column: Column
+        for i, column in zip(range(len(attribute.columns)), attribute.columns):
+            attribute_name = f"{attribute.name}_{i}"
+            if not column.optional:
+                try:
+                    df_log[attribute_name].fillna("Unknown", inplace=True)
+                except:
+                    df_log[attribute_name].fillna(-1, inplace=True)
+        return df_log
+
+    @staticmethod
+    def create_compound_attribute(df_log, attribute):
+        compound_column_names = [x.name for x in attribute.columns]
+        df_log[attribute.name] = df_log[compound_column_names].apply(
+            lambda row: attribute.separator.join([value for value in row.values.astype(str) if
+                                                  not (value == 'nan' or value != value)]), axis=1)
+        return df_log
+
+    @staticmethod
+    def combine_attribute_columns(df_log, attribute):
+        compound_attribute_names = [f"{attribute.name}_{i}" for i in range(len(attribute.columns))]
+        if attribute.is_compound:
+            df_log[f"{attribute.name}_attribute"] = df_log[compound_attribute_names].apply(
+                lambda row: attribute.separator.join([value for value in row.values.astype(str) if
+                                                      not (value == 'nan' or value != value)]), axis=1)
+        else:
+            df_log[f"{attribute.name}_attribute"] = df_log[f"{attribute.name}_0"]
+        df_log = df_log.drop(columns=compound_attribute_names)
+        return df_log
+
+    @staticmethod
+    def create_attribute_columns(df_log, attribute):
+        for i, column in zip(range(len(attribute.columns)), attribute.columns):
+            attribute_name = f"{attribute.name}_{i}"
+            df_log[attribute_name] = df_log[column.name]
+            if column.range_start is not None or column.range_end is not None:
+                df_log[attribute_name] = df_log[attribute_name].str[column.range_start:column.range_end]
+        return df_log
+
+    @staticmethod
+    def replace_with_nan(df_log, attribute):
+        for i, column in zip(range(len(attribute.columns)), attribute.columns):
+            attribute_name = f"{attribute.name}_{i}"
+            for nan_value in column.nan_values:
+                df_log[attribute_name] = df_log[attribute_name].replace(nan_value, np.nan, regex=False)
+        return df_log
+
+    def preprocess_according_to_attributes(self, df_log):
+        # loop over all attributes and check if they should be created, renamed or imputed
+        for attribute in self.attributes.values():
+            df_log = DataStructure.create_attribute_columns(df_log, attribute)
+            df_log = DataStructure.replace_with_nan(df_log, attribute)
+            if len(attribute.na_rep_columns) > 0:  # impute values in case of missing values
+                df_log = DataStructure.replace_nan_values_based_on_na_rep_columns(df_log, attribute)
+            if attribute.na_rep_value is not None:
+                df_log = DataStructure.replace_nan_values_based_on_na_rep_value(df_log, attribute)
+
+            df_log = DataStructure.combine_attribute_columns(df_log, attribute)
+
+        return df_log
+
+    def split_df_log_into_combined_events(self, df_log: DataFrame):
+        df_log["idx"] = df_log.reset_index().index
+        if "timestamp" in self.attributes:
+            raise ImportError(
+                "Combined events cannot be split since an attribute with name timestamp is already defined")
+
+        if "startTimestamp" in self.attributes and "completeTimestamp" in self.attributes:
+            df_log_start = df_log.drop(columns=["completeTimestamp"])
+            df_log_start["lifecycle"] = "start"
+            df_log_start = df_log_start.rename(columns={"startTimestamp": "timestamp"})
+
+            df_log_end = df_log.drop(columns=["startTimestamp"])
+            df_log_end["lifecycle"] = "complete"
+            df_log_end = df_log_end.rename(columns={"completeTimestamp": "timestamp"})
+
+            df_log = pd.concat([df_log_start, df_log_end])
+        elif "startTimestamp" in self.attributes:
+            df_log["lifecycle"] = "start"
+            df_log = df_log.rename(columns={"startTimestamp": "timestamp"})
+        elif "completeTimestamp" in self.attributes:
+            df_log["lifecycle"] = "complete"
+            df_log = df_log.rename(columns={"completeTimestamp": "timestamp"})
+
+        df_log = df_log.sort_values(by=["timestamp", "idx"])
+        df_log = df_log.drop(columns=["idx"])
+        return df_log
+
+    def update_attributes(self):
+        if "startTimestamp" in self.attributes and "completeTimestamp" in self.attributes:
+            start_dt_format = self.get_datetime_formats()["startTimestamp"].format
+            complete_dt_format = self.get_datetime_formats()["completeTimestamp"].format
+            if start_dt_format != complete_dt_format:
+                raise ValueError("startTimestamp and completeTimestamp have a different format")
+
+            start_attribute = self.attributes["startTimestamp"]
+            start_attribute.name = "timestamp"
+            self.attributes["timestamp"] = start_attribute
+            del self.attributes["startTimestamp"]
+            del self.attributes["completeTimestamp"]
+
+
+        elif "startTimestamp" in self.attributes:
+            start_attribute = self.attributes["startTimestamp"]
+            start_attribute.name = "timestamp"
+
+            self.attributes["timestamp"] = start_attribute
+            del self.attributes["startTimestamp"]
+        elif "completeTimestamp" in self.attributes:
+            complete_attribute = self.attributes["completeTimestamp"]
+            complete_attribute.name = "timestamp"
+
+            self.attributes["timestamp"] = complete_attribute
+            del self.attributes["completeTimestamp"]
+
+    def check_if_required_attributes_are_present(self, record_constructor):
+        # loop over all required attributes of the record constructor
+        # --> check whether they are required by self
+        required = True
+        for required_attribute in record_constructor.required_attributes:
+            if required_attribute == "index":  # records of an always have an index, so records will have
+                # the required attributes = index
+                continue
+            if required_attribute not in self.attributes or self.attributes[required_attribute].optional:
+                # if the required attribute does not occur in the self.attributes or the attribute is
+                # optional, then the record_constructor labels are not required
+                required = False
+        return required
+
+    def determine_required_labels(self, records: List["RecordConstructor"]):
+        # determine the required labels for the records defined by this datastructure
+        # therefore, we have to check for all record constructors in records
+        # whether the required attributes are present by the dataset description definition
+
+        # initially, self.required_labels might be None, hence we need to make it an empty list.
+        if self.required_labels is None:
+            self.required_labels = []
+
+        # loop over all record_constructors in records
+        for record_constructor in records:
+            # check whether self.labels appear in the record constructor
+            if self.labels_appear_in_record_constructor(record_constructor):
+                if record_constructor.prevalent_record.where_condition != "":
+                    # a where condition is specified, then not all records require the record_constructor labels
+                    required = False
+                else:
+                    required = self.check_if_required_attributes_are_present(record_constructor)
+                if required:
+                    # if required = true, then the record_constructor labels are required labels of self
+                    self.required_labels.extend(record_constructor.record_labels)
+        self.required_labels = list(set(self.required_labels))
+
+    def get_required_labels(self, records: List["RecordConstructor"]):
+        if self.required_labels is None:
+            self.determine_required_labels(records)
+        return self.required_labels
+
+    def get_required_labels_str(self, records: List["RecordConstructor"]):
+        """Method to convert the required labels determined by records to a string seperated by :
+        :param records: the required
+        """
+        if self.required_labels is None:
+            self.determine_required_labels(records)
+        required_labels_w_records = self.required_labels[:]
+        required_labels_w_records.insert(0, "Record")
+        required_labels_str = ":".join(required_labels_w_records)
+        return required_labels_str
+
+    def read_data_set(self, file_name, use_sample, load_status: int, store_preprocessed_file=True,
+                      use_preprocessed_file=False):
+        preprocessed_file_name = self._get_preprocessed_file_name(file_name, use_sample)
+        df_log = None
+        if use_preprocessed_file:
+            df_log = self.read_preprocessed_df_log(preprocessed_file_name)
+        if df_log is None:  # no preprocessed file was read
+            df_log = self.read_df_log(file_name, use_sample)
+            if store_preprocessed_file:
+                self.store_df_log(df_log, preprocessed_file_name)
+
+        df_log["loadStatus"] = load_status
+        return df_log
+
+    def read_df_log(self, file_name, use_sample):
+        df_log = self.prepare_event_data_sets(file_name, use_sample)
+        return df_log
+
+    def read_preprocessed_df_log(self, preprocessed_file_name):
+        preprocessed_file_path = os.path.join(self.preprocessed_file_directory, preprocessed_file_name)
+        # first try to read preprocessed file
+        if not os.path.exists(preprocessed_file_path):
+            warning_message = f"No preprocessed file {preprocessed_file_name} found, preprocessed the file " \
+                              f"instead"
+            warnings.warn(warning_message)
+            return None
+        else:  # use_preprocessed_file and file exists
+            df_log = pd.read_pickle(preprocessed_file_path)
+        return df_log
+
+    def store_df_log(self, df_log, preprocessed_file_name):
+        # only store file if we did not read from the stored file
+        os.makedirs(self.preprocessed_file_directory, exist_ok=True)
+
+        preprocessed_file_path = os.path.join(self.preprocessed_file_directory, preprocessed_file_name)
+        df_log.to_pickle(preprocessed_file_path)
+
+    def _get_preprocessed_file_name(self, file_name, use_sample):
+        # change extension from csv to pkl and add sample in case of sample
+        sample_is_used = use_sample and len(self.samples) > 0
+        preprocessed_file_name = f"{file_name[:-4]}_sample.pkl" if sample_is_used else f"{file_name[:-4]}.pkl"
+        return preprocessed_file_name
+
+    @staticmethod
+    def create_record_id_column(df_log, file_name):
+        record_id_column = df_log.index
+        record_id_column = record_id_column.astype(str) + "_" + file_name[:-4]
+        return record_id_column
+
+    def prepare_event_data_sets(self, file_name, use_sample):
+        dtypes = self.get_dtype_dict()
+        required_columns = self.get_required_columns()
+
+        true_values = self.true_values
+        false_values = self.false_values
+
+        if file_name.endswith('.csv'):
+            df_log: DataFrame = pd.read_csv(os.path.join(self.file_directory, file_name), keep_default_na=True,
+                                            usecols=required_columns, dtype=dtypes, true_values=true_values,
+                                            false_values=false_values, sep=self.seperator, decimal=self.decimal,
+                                            encoding=self.encoding)
+        else:
+            raise TypeError(f"The file extension of {file_name} is not implemented. Use .csv.")
+
+        if use_sample and self.has_datetime_attribute():
+            df_log = self.create_sample(file_name, df_log)
+
+        df_log = self.preprocess_according_to_attributes(df_log)
+
+        # all columns have been renamed to or constructed with the name attribute,
+        # hence only keep those that match with a name attribute
+        required_attributes = list([f"{attribute_name}_attribute" for attribute_name in self.attributes.keys()])
+        required_attributes_mapping = {f"{attribute_name}_attribute": f"{attribute_name}" for attribute_name in
+                                       self.attributes.keys()}
+        df_log = df_log[required_attributes]
+        df_log = df_log.rename(columns=required_attributes_mapping)
+
+        if self.split_combined_events:
+            df_log = self.split_df_log_into_combined_events(df_log)
+            self.update_attributes()
+
+        if self.add_log:
+            df_log["log"] = file_name
+
+        if self.add_index:
+            df_log["index"] = df_log.index
+
+        # drop all columns with only nan values
+        df_log = df_log.dropna(how='all', axis=1)  # drop all columns in which all values are nan (empty)
+        df_log = df_log.dropna(how='all')  # drop all columns in which all values are nan (empty)
+
+        df_log["recordId"] = self.create_record_id_column(df_log, file_name)
+
+        return df_log
+
+    def determine_optional_labels_in_log(self, df_log, records):
+        df_log["labels"] = ""
+
+        if self.required_labels is None:
+            self.determine_required_labels(records)
+
+        if set(self.required_labels) == set(self.labels):
+            return df_log
+
+        for record_constructor in records:
+            if self.labels_appear_in_record_constructor(record_constructor):
+                if set(record_constructor.record_labels) <= set(self.required_labels):
+                    continue  # record constructor only contains required labels
+
+                # one of possible labels appear in record constructor
+                should_have_label = self.all_required_attributes_are_present_in_df_log(df_log, record_constructor)
+                if should_have_label.any():  # check whether there is still a row that can have the label
+                    should_have_label = should_have_label & self.is_where_condition_satisfied(
+                        df_log, record_constructor)
+                if should_have_label.any():
+                    for label in record_constructor.record_labels:
+                        df_log.loc[should_have_label, "labels"] += ":" + label
+
+        return df_log
+
+    def labels_appear_in_record_constructor(self, record_constructor):
+        if self.labels is not None:
+            # check whether the labels have overlap with the labels of the record_constructor
+            intersection = list(set(self.labels) & set(record_constructor.record_labels))
+        else:
+            # no labels are defined, hence we consider all labels of the record constructor
+            intersection = record_constructor.record_labels
+
+        return len(intersection) > 0
+
+    def all_required_attributes_are_present_in_df_log(self, df_log, record_constructor):
+        required_attributes_are_present = pd.Series(True, index=np.arange(len(df_log)), name='present')
+        for required_attribute in record_constructor.required_attributes:
+            if required_attribute == "index" or required_attribute == "log":
+                continue
+            if required_attribute in self.attributes:
+                if self.attributes[required_attribute].optional:
+                    # if the required attribute is optional in the structure, check whether the required attribute is
+                    # not null
+                    required_attributes_are_present = required_attributes_are_present & df_log[
+                        required_attribute].notnull()
+                # else the required attributes is required in the structure, hence nothing changes
+            else:  # the required attribute is missing in the structure -> hence not all are present
+                required_attributes_are_present = pd.Series(False, index=np.arange(len(df_log)), name='present')
+                # since for all rows, at least an attribute is missing, we can return
+                return required_attributes_are_present
+
+        return required_attributes_are_present
+
+    @staticmethod
+    def is_where_condition_satisfied(df_log, record_constructor):
+        # TODO split where_condition
+        where_condition = record_constructor.prevalent_record.where_condition
+        where_condition_satisfied = pd.Series(True, index=np.arange(len(df_log)), name='satisfied')
+        if where_condition == "":
+            return where_condition_satisfied
+        where_conditions = where_condition.split("AND")
+        for condition in where_conditions:
+            stripped_condition = condition.strip()
+            if "=" in condition:
+                condition_list = stripped_condition.split("=")
+                column_name = condition_list[0].strip()
+                if "." in column_name:
+                    column_name = column_name.split(".")[1].strip()
+                column_value = condition_list[1].strip().strip('"')
+                where_condition_satisfied = where_condition_satisfied & (
+                        df_log[column_name].astype("string") == column_value)
+            elif "STARTS WITH" in condition:
+                condition_list = stripped_condition.split("STARTS WITH")
+                column_name = condition_list[0].strip()
+                if "." in column_name:
+                    column_name = column_name.split(".")[1].strip()
+                column_value = condition_list[1].strip().strip('"')
+                where_condition_satisfied = where_condition_satisfied & df_log[
+                    column_name].str.startswith(column_value)
+            elif "ENDS WITH" in condition:
+                condition_list = stripped_condition.split("ENDS WITH")
+                column_name = condition_list[0].strip()
+                if "." in column_name:
+                    column_name = column_name.split(".")[1].strip()
+                column_value = condition_list[1].strip().strip('"')
+                where_condition_satisfied = where_condition_satisfied & df_log[
+                    column_name].str.endswith(column_value)
+        return where_condition_satisfied
+
+    def get_datetime_formats(self) -> Dict[str, DatetimeObject]:
+        datetime_formats = {}
+
+        for attribute_name, attribute in self.attributes.items():
+            if attribute.is_datetime:
+                datetime_formats[attribute_name] = attribute.datetime_object
+
+        return datetime_formats
+
+    def get_attribute_value_pairs_filtered(self, exclude: bool) -> Dict[str, List[str]]:
+        attribute_value_pairs = {}
+        for attribute_name, attribute in self.attributes.items():
+            if attribute.use_filter:
+                attribute_value_pairs[attribute_name] \
+                    = attribute.filter_exclude_values if exclude else attribute.filter_include_values
+
+        return attribute_value_pairs
+
+
+class DatasetDescriptions:
+    def __init__(self, config: Configuration):
+        path = config.dataset_description_path
+
+        random.seed(1)
+        with open(path, encoding='utf-8') as f:
+            json_event_tables = json.load(f)
+
+        self.structures = [DataStructure.from_dict(item) for item in json_event_tables]
+        self.structures = [item for item in self.structures if item is not None]
+
+    def get_structure_name_file_mapping(self):
+        # request the file names per structure
+        file_names = {}
+        for structure in self.structures:
+            file_names[structure.name] = structure.file_names
+        return file_names
+
+    def get_files_list(self):
+        # request all file names specified in self.structures in a list
+        files = []
+        for structure in self.structures:
+            files.extend(structure.file_names)
+        return files
```

### Comparing `promg-1.0.9/src/promg/database_managers/authentication.py` & `promg-1.1.0/src/promg/database_managers/authentication.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from dataclasses import dataclass
-from enum import Enum
-
-
-# from remote_authentication import remote
-# if you want a remote connection, store credentials somewhere different (e.g. remote_authentication)
-
-@dataclass
-class Credentials:
-    uri: str
-    user: str
-    password: str
-
-
-# local credentials
-local = Credentials(
-    uri="bolt://localhost:7687",
-    user="neo4j",
-    password="12345678"
-)
-
-remote = None
-
-
-class Connections(Enum):
-    REMOTE = 1
-    LOCAL = 2
-
-
-connections_map = {
-    Connections.REMOTE: remote,
-    Connections.LOCAL: local
-}
+from dataclasses import dataclass
+from enum import Enum
+
+
+# from remote_authentication import remote
+# if you want a remote connection, store credentials somewhere different (e.g. remote_authentication)
+
+@dataclass
+class Credentials:
+    uri: str
+    user: str
+    password: str
+
+
+# local credentials
+local = Credentials(
+    uri="bolt://localhost:7687",
+    user="neo4j",
+    password="12345678"
+)
+
+remote = None
+
+
+class Connections(Enum):
+    REMOTE = 1
+    LOCAL = 2
+
+
+connections_map = {
+    Connections.REMOTE: remote,
+    Connections.LOCAL: local
+}
```

### Comparing `promg-1.0.9/src/promg/database_managers/db_connection.py` & `promg-1.1.0/src/promg/database_managers/db_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,119 @@
-from string import Template
-from typing import Optional, List, Dict, Any
-
-import neo4j
-from neo4j import GraphDatabase
-from neo4j.exceptions import ServiceUnavailable
-
-from . import authentication
-from .authentication import Credentials
-from ..utilities.singleton import Singleton
-from ..utilities.configuration import Configuration
-
-
-class Query:
-    def __init__(self, query_str: str, database: str = None, parameters: Optional[Dict[str, any]] = None,
-                 template_string_parameters: Optional[Dict[str, any]] = None):
-        if template_string_parameters is not None:
-            self.query_string = Template(query_str).safe_substitute(template_string_parameters)
-        else:
-            self.query_string = query_str
-        self.kwargs = parameters
-        self.database = database
-
-
-class DatabaseConnection:
-    def __init__(self, uri: str, db_name: str, user: str, password: str, verbose: bool = False,
-                 batch_size: int = 100000):
-        self.db_name = db_name
-        self.driver = self.start_connection(uri, user, password)
-        self.verbose = verbose
-        self.batch_size = batch_size
-
-    @staticmethod
-    def start_connection(uri: str, user: str, password: str):
-        # begin config
-        # connection to Neo4J database
-        driver = GraphDatabase.driver(uri, auth=(user, password), max_connection_lifetime=200)
-        return driver
-
-    def close_connection(self):
-        self.driver.close()
-
-    def exec_query(self, function, **kwargs):
-        # check whether connection can be made
-        self.verify_connectivity()
-
-        result = function(**kwargs)
-        if result is None:
-            return
-        query = result.query_string
-        kwargs = result.kwargs
-        database = result.database
-        if kwargs is None:
-            kwargs = {}  # replace None value by an emtpy dictionary
-        if "$batch_size" in query:
-            kwargs["batch_size"] = self.batch_size
-        if "$limit" in query:
-            kwargs["limit"] = self.batch_size
-
-        if "apoc.periodic.commit" in query:
-            limit = kwargs["limit"]
-            failed_batches = 1
-            attempts = 0
-            while failed_batches > 0 and attempts <= 10:
-                result = self._exec_query(query, database, **kwargs)
-                failed_batches = result[0]['failedBatches']
-                kwargs["batch_size"] = int(limit / 2)
-                kwargs["batch_size"] = max(10000, kwargs["batch_size"])
-                attempts += 1
-            if failed_batches > 0:
-                raise Exception(f"Maximum attempts reached: {result[0]['batchErrors']}")
-
-            return result
-        else:
-
-            return self._exec_query(query, database, **kwargs)
-
-    def _exec_query(self, query: str, database: str = None, **kwargs) -> Optional[List[Dict[str, Any]]]:
-        """
-        Write a transaction of the query to  the server and return the result
-        @param query: string, query to be executed
-        @param database: string, Name of the database
-        @return: The result of the query or None
-        """
-
-        def run_query(tx: neo4j.Transaction, _query: str, **_kwargs) -> Optional[List[Dict[str, Any]]]:
-            """
-                Run the query and return the result of the query
-                @param tx: transaction class on which we can perform queries to the database
-                @param _query: string
-                @return: The result of the query or None if there is no result
-            """
-            # get the results after the query is executed
-            try:
-                _result = tx.run(_query, _kwargs).data()
-            except Exception as inst:
-                self.close_connection()
-                print(inst)
-            else:
-                if _result is not None and _result != []:  # return the values if result is not none or empty list
-                    return _result
-                else:
-                    return None
-
-        if self.verbose:
-            print(query)
-
-        if database is None:
-            database = self.db_name
-
-        with self.driver.session(database=database) as session:
-            result = session.write_transaction(run_query, query, **kwargs)
-            return result
-
-    @staticmethod
-    def set_up_connection(config: Configuration):
-        return DatabaseConnection(db_name=config.user, uri=config.uri, user=config.user,
-                                  password=config.password, verbose=config.verbose, batch_size=config.batch_size)
-
-    def verify_connectivity(self):
-        self.driver.verify_connectivity()
+from string import Template
+from typing import Optional, List, Dict, Any, Tuple
+
+import neo4j
+from ..utilities.configuration import Configuration
+
+
+class Query:
+    def __init__(self, query_str: str, database: str = None, parameters: Optional[Dict[str, any]] = None,
+                 template_string_parameters: Optional[Dict[str, any]] = None):
+        if template_string_parameters is not None:
+            self.query_string = Template(query_str).safe_substitute(template_string_parameters)
+        else:
+            self.query_string = query_str
+        self.kwargs = parameters
+        self.database = database
+
+
+class DatabaseConnection:
+    def __init__(self, uri: str, db_name: str, user: str, password: str, verbose: bool = False,
+                 batch_size: int = 100000):
+        self.db_name = db_name
+        self.driver = self.start_connection(uri, user, password)
+        self.verbose = verbose
+        self.batch_size = batch_size
+
+    @staticmethod
+    def start_connection(uri: str, user: str, password: str):
+        # begin config
+        # connection to Neo4J database
+        driver = neo4j.GraphDatabase.driver(uri, auth=(user, password), max_connection_lifetime=200)
+        return driver
+
+    def close_connection(self):
+        self.driver.close()
+
+    def exec_query(self, function, **kwargs):
+        # check whether connection can be made
+        self.verify_connectivity()
+
+        result = function(**kwargs)
+        if result is None:
+            return
+        query = result.query_string
+        kwargs = result.kwargs
+        database = result.database
+        if kwargs is None:
+            kwargs = {}  # replace None value by an emtpy dictionary
+        if "$batch_size" in query:
+            kwargs["batch_size"] = self.batch_size
+        if "$limit" in query:
+            kwargs["limit"] = self.batch_size
+
+        if "apoc.periodic.commit" in query:
+            limit = kwargs["limit"]
+            failed_batches = 1
+            attempts = 0
+            while failed_batches > 0 and attempts <= 10:
+                result = self._exec_query(query, database, **kwargs)
+                failed_batches = result[0]['failedBatches']
+                kwargs["batch_size"] = int(limit / 2)
+                kwargs["batch_size"] = max(10000, kwargs["batch_size"])
+                attempts += 1
+            if failed_batches > 0:
+                raise Exception(f"Maximum attempts reached: {result[0]['batchErrors']}")
+
+            return result
+        else:
+
+            return self._exec_query(query, database, **kwargs)
+
+    def _exec_query(self, query: str, database: str = None, **kwargs) -> Optional[List[Dict[str, Any]]]:
+        """
+        Write a transaction of the query to  the server and return the result
+        @param query: string, query to be executed
+        @param database: string, Name of the database
+        @return: The result of the query or None
+        """
+
+        def run_query(tx: neo4j.Transaction, _query: str, **_kwargs) -> Tuple[
+            Optional[List[Dict[str, Any]]], neo4j.ResultSummary]:
+
+            """
+                Run the query and return the result of the query
+                @param tx: transaction class on which we can perform queries to the database
+                @param _query: string
+                @return: The result of the query or None if there is no result
+            """
+            # get the results after the query is executed
+            _result = tx.run(_query, _kwargs)
+            _result_records = _result.data()  # obtain dict representation
+            _summary = _result.consume()  # exhaust the result
+
+            # or empty list
+            return _result_records, _summary
+
+        if self.verbose:
+            print(query)
+
+        if database is None:
+            database = self.db_name
+
+        with self.driver.session(database=database) as session:
+            try: # try to commit the transaction, if the transaction fails, it is rolled back automatically
+                result, summary = session.execute_write(run_query, query, **kwargs)
+                return result
+            except Exception as inst: # let user know the transaction failed and close the connection
+                self.close_connection()
+                print("Latest transaction was rolled back")
+                print(f"This was your latest query: {query}")
+                print(inst)
+
+    @staticmethod
+    def set_up_connection(config: Configuration):
+        return DatabaseConnection(db_name=config.user, uri=config.uri, user=config.user,
+                                  password=config.password, verbose=config.verbose, batch_size=config.batch_size)
+
+    def verify_connectivity(self):
+        self.driver.verify_connectivity()
```

### Comparing `promg-1.0.9/src/promg/facades/oced_pg.py` & `promg-1.1.0/src/promg/facades/oced_pg.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,149 +1,180 @@
-import os
-from typing import List, Optional
-
-from ..data_managers.semantic_header import SemanticHeader
-from ..data_managers.datastructures import DatasetDescriptions
-from ..modules.ekg_builder_semantic_header import EKGUsingSemanticHeaderBuilder
-from ..modules.data_importer import Importer
-from ..database_managers.db_connection import DatabaseConnection
-from ..utilities.performance_handling import Performance
-
-
-class OcedPg:
-
-    def __init__(self, database_connection: DatabaseConnection, dataset_descriptions: DatasetDescriptions,
-                 semantic_header: SemanticHeader,
-                 use_sample: bool = False,
-                 use_preprocessed_files: bool = False,
-                 store_files: bool = True,
-                 import_directory=None):
-        """
-            This is a Class that acts as a facade for used to extract, load and transform their data using OCED-PG
-
-            :param dataset_descriptions: A specification of how the data sets are structured
-            :type dataset_descriptions: DatasetDescriptions
-            :param perf: a :class:Performance to keep track of the running time of the EKG construction
-            :type perf: Performance
-            :param use_sample: boolean indicating whether the DB should be build using a sample as specified in the
-            ImportedDataStructures, defaults to False
-            :type use_sample: bool
-
-        """
-        # classes responsible for executing queries
-        self.data_importer = Importer(database_connection=database_connection,
-                                      data_structures=dataset_descriptions,
-                                      use_sample=use_sample,
-                                      use_preprocessed_files=use_preprocessed_files,
-                                      semantic_header=semantic_header,
-                                      import_directory=import_directory,
-                                      store_files=store_files)
-        self.ekg_builder = EKGUsingSemanticHeaderBuilder(database_connection=database_connection,
-                                                         semantic_header=semantic_header)
-
-    def load_and_transform(self):
-        self.load()
-        self.transform()
-
-    # region import events
-    def load(self, imported_logs=None):
-        """
-        Import data, both event data as other data, as specified in the DS files.
-        Add record labels as specified in the semantic header
-        """
-        return self.data_importer.import_data(imported_logs)
-
-    # endregion
-    def transform(self):
-        """
-            Transform the record layer into a semantic layer
-        """
-        self.create_nodes()
-        self.create_relations()
-
-    def create_nodes(self, node_types: Optional[List[str]] = None) -> None:
-        """
-        Create nodes as specified in the semantic header
-
-        Args:
-            node_types: list of nodes that should be created. In case of None, all nodes are
-            created as specified in the semantic header
-
-        """
-        self.create_nodes_by_records(node_types)
-
-    def create_nodes_by_records(self, node_types: Optional[List[str]] = None) -> None:
-        """
-        Create nodes based on records as specified in the semantic header
-
-        Args:
-            node_types: list of nodes that should be created. In case of None, all nodes are
-            created as specified in the semantic header
-
-        """
-
-        self.ekg_builder.create_nodes_by_records(node_types)
-
-    def create_relations(self, relation_types: Optional[List[str]] = None) -> None:
-        """
-        Create relations as specified in the semantic header
-
-        Args:
-            relation_types: list of relations that should be created. In case of None, all relations are
-            created as specified in the semantic header
-
-        """
-        self.create_relations_using_record(relation_types)
-        self.create_relations_using_relations(relation_types)
-
-    def create_relations_using_record(self, relation_types: Optional[List[str]] = None) -> None:
-        """
-        Create relations using records as specified in the semantic header
-
-        Args:
-            relation_types: list of relations that should be created. In case of None, all relations are
-            created as specified in the semantic header
-
-        """
-        self.ekg_builder.create_relations_using_records(relation_types)
-
-    def create_relations_using_relations(self, relation_types: Optional[List[str]] = None) -> None:
-        """
-        Create relations using a subgraph as specified in the semantic header
-
-        Args:
-            relation_types: list of relations that should be created. In case of None, all relations are
-            created as specified in the semantic header
-
-        """
-        self.ekg_builder.create_relations_using_relations(relation_types)
-
-    def create_nodes_by_relations(self, node_types: Optional[List[str]] = None) -> None:
-        """
-        Pass on method to ekg_builder to create entities based on relations as specified in the semantic header
-
-        :param node_types: list of entity types for which the entities based on relations should be created. In
-        case of None, all entities based on relations are created as specified in the semantic header
-        :type node_types: List[str], optional
-        :return: None
-
-        """
-        self.ekg_builder.create_nodes_by_relations(node_types)
-
-    def create_df_edges(self, entity_types: Optional[List[str]] = None, event_label: str = "Event",
-                        add_duration=False) -> None:
-        """
-        Pass on method to ekg_builder to merge parallel directly follows in between batching events
-
-        :return: None
-        """
-        self.ekg_builder.create_df_edges(entity_types, event_label, add_duration=add_duration)
-        self.ekg_builder.merge_duplicate_df()
-
-    def create_static_nodes_and_relations(self) -> None:
-        """
-        Pass on method to ekg_builder to create static nodes and relations
-        No implementation yet
-
-        :return: None
-        """
-        self.ekg_builder.create_static_nodes_and_relations()
+import os
+from typing import List, Optional
+
+from ..data_managers.semantic_header import SemanticHeader
+from ..data_managers.datastructures import DatasetDescriptions
+from ..modules.db_management import DBManagement
+from ..modules.ekg_builder_semantic_header import EKGUsingSemanticHeaderBuilder
+from ..modules.data_importer import Importer
+from ..database_managers.db_connection import DatabaseConnection
+from ..utilities.performance_handling import Performance
+
+
+class OcedPg:
+
+    def __init__(self, database_connection: DatabaseConnection, dataset_descriptions: DatasetDescriptions,
+                 semantic_header: SemanticHeader,
+                 use_sample: bool = False,
+                 use_preprocessed_files: bool = False,
+                 store_files: bool = True,
+                 import_directory=None):
+        """
+            This is a Class that acts as a facade for used to extract, load and transform their data using OCED-PG
+
+            :param dataset_descriptions: A specification of how the data sets are structured
+            :type dataset_descriptions: DatasetDescriptions
+            :param perf: a :class:Performance to keep track of the running time of the EKG construction
+            :type perf: Performance
+            :param use_sample: boolean indicating whether the DB should be build using a sample as specified in the
+            ImportedDataStructures, defaults to False
+            :type use_sample: bool
+
+        """
+        # classes responsible for executing queries
+        self.data_importer = Importer(database_connection=database_connection,
+                                      data_structures=dataset_descriptions,
+                                      use_sample=use_sample,
+                                      use_preprocessed_files=use_preprocessed_files,
+                                      semantic_header=semantic_header,
+                                      import_directory=import_directory,
+                                      store_files=store_files)
+        self.ekg_builder = EKGUsingSemanticHeaderBuilder(database_connection=database_connection,
+                                                         semantic_header=semantic_header)
+        self.db_manager = DBManagement(db_connection=database_connection)
+        self.semantic_header = semantic_header
+        self.dataset_descriptions = dataset_descriptions
+
+    def load_and_transform(self):
+        self.load()
+        self.transform()
+
+    # region import events
+    def load(self, logs=None):
+        """
+        Import data, both event data as other data, as specified in the DS files.
+        Add record labels as specified in the semantic header
+        Args:
+            logs: list of logs to be imported
+        """
+
+        # only import logs that are not imported yet
+        # dataset name is considered to be unique
+        already_imported_logs = self.db_manager.get_imported_logs()[0]['logs']
+        if logs is None:
+            logs = self.dataset_descriptions.get_files_list()
+        to_be_imported_logs = [log for log in logs if log not in already_imported_logs]
+
+        return self.data_importer.import_data(to_be_imported_logs=to_be_imported_logs)
+
+    # endregion
+    def transform(self, logs=None):
+        """
+            Transform the record layer into a semantic layer
+        """
+        self.create_nodes(logs)
+        self.create_relations(logs)
+
+    def create_nodes(self, node_types: Optional[List[str]] = None, logs: Optional[List[str]] = None) -> None:
+        """
+        Create nodes as specified in the semantic header
+
+        Args:
+            node_types: list of nodes that should be created. In case of None, all nodes are
+            created as specified in the semantic header
+            logs: list of logs that need to be transformed
+
+        """
+        self.create_nodes_by_records(node_types=node_types, logs=logs)
+
+    def create_nodes_by_records(self, node_types: Optional[List[str]] = None,
+                                logs: Optional[List[str]] = None) -> None:
+        """
+        Create nodes based on records as specified in the semantic header
+
+        Args:
+            node_types: list of nodes that should be created. In case of None, all nodes are
+            created as specified in the semantic header
+            logs: list of logs that need to be transformed
+
+        """
+        if logs is None:
+            files = self.dataset_descriptions.get_structure_name_file_mapping()
+            for name, files in files.items():
+                self.ekg_builder.create_nodes_by_records(node_types, logs=files)
+        else:
+            self.ekg_builder.create_nodes_by_records(node_types, logs=logs)
+
+    def create_relations(self, relation_types: Optional[List[str]] = None,
+                         logs: Optional[List[str]] = None) -> None:
+        """
+        Create relations as specified in the semantic header
+
+        Args:
+            relation_types: list of relations that should be created. In case of None, all relations are
+            created as specified in the semantic header
+            logs: list of logs that need to be transformed
+
+        """
+        if logs is None:
+            files = self.dataset_descriptions.get_structure_name_file_mapping()
+            for name, files in files.items():
+                self.create_relations_using_record(relation_types=relation_types, logs=files)
+                self.create_relations_using_relations(relation_types=relation_types)
+        else:
+            self.create_relations_using_record(relation_types=relation_types, logs=logs)
+            self.create_relations_using_relations(relation_types=relation_types)
+
+    def create_relations_using_record(self, relation_types: Optional[List[str]] = None,
+                                      logs: Optional[List[str]] = None) -> None:
+        """
+        Create relations using records as specified in the semantic header
+
+        Args:
+            relation_types: list of relations that should be created. In case of None, all relations are
+            created as specified in the semantic header
+            logs: list of logs that need to be transformed
+
+        """
+        self.ekg_builder.create_relations_using_records(relation_types=relation_types, logs=logs)
+
+    def create_relations_using_relations(self, relation_types: Optional[List[str]] = None) -> None:
+        """
+        Create relations using a subgraph as specified in the semantic header
+
+        Args:
+            relation_types: list of relations that should be created. In case of None, all relations are
+            created as specified in the semantic header
+
+        """
+        self.ekg_builder.create_relations_using_relations(relation_types)
+
+    def create_nodes_by_relations(self, node_types: Optional[List[str]] = None) -> None:
+        """
+        Pass on method to ekg_builder to create entities based on relations as specified in the semantic header
+
+        :param node_types: list of entity types for which the entities based on relations should be created. In
+        case of None, all entities based on relations are created as specified in the semantic header
+        :type node_types: List[str], optional
+        :return: None
+
+        """
+        self.ekg_builder.create_nodes_by_relations(node_types)
+
+    def create_df_edges(self, entity_types: Optional[List[str]] = None, event_label: str = "Event",
+                        add_duration=False) -> None:
+        """
+        Pass on method to ekg_builder to merge parallel directly follows in between batching events
+
+        :return: None
+        """
+        self.ekg_builder.create_df_edges(entity_types, event_label, add_duration=add_duration)
+        self.ekg_builder.merge_duplicate_df()
+
+    def create_static_nodes_and_relations(self) -> None:
+        """
+        Pass on method to ekg_builder to create static nodes and relations
+        No implementation yet
+
+        :return: None
+        """
+        self.ekg_builder.create_static_nodes_and_relations()
```

### Comparing `promg-1.0.9/src/promg/modules/data_importer.py` & `promg-1.1.0/src/promg/modules/data_importer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,184 @@
-import os
-from string import Template
-from typing import Optional
-
-from ..data_managers.semantic_header import SemanticHeader
-from ..database_managers.db_connection import DatabaseConnection
-from ..data_managers.datastructures import DatasetDescriptions
-from ..utilities.performance_handling import Performance
-from ..cypher_queries.data_importer_ql import DataImporterQueryLibrary as di_ql
-from pathlib import Path
-import pandas as pd
-
-
-class Importer:
-    def __init__(self, database_connection: DatabaseConnection,
-                 data_structures: DatasetDescriptions,
-                 semantic_header: SemanticHeader,
-                 import_directory: Optional[str] = None,
-                 use_sample: bool = False,
-                 use_preprocessed_files: bool = False,
-                 store_files: bool = False):
-        self.connection = database_connection
-        self.structures = data_structures.structures
-        self.records = semantic_header.records
-
-        self.load_batch_size = 20000
-        self.use_sample = use_sample
-        self.use_preprocessed_files = use_preprocessed_files
-        self.store_files = store_files
-        self.load_status = 0
-
-        self._import_directory = import_directory
-
-    def update_load_status(self):
-        self.connection.exec_query(di_ql.get_update_load_status_query,
-                                   **{
-                                       "current_load_status": self.load_status
-                                   })
-        self.load_status += 1
-
-    def import_data(self, imported_logs) -> None:
-        for structure in self.structures:
-            required_labels_str = structure.get_required_labels_str(records=self.records)
-
-            # read in all file names that match this structure
-            for file_name in structure.file_names:
-                if imported_logs is None or file_name not in imported_logs:
-                    # read and import the nodes
-                    df_log = structure.read_data_set(file_name=file_name,
-                                                     use_sample=self.use_sample,
-                                                     use_preprocessed_file=self.use_preprocessed_files,
-                                                     load_status=self.load_status,
-                                                     store_preprocessed_file=self.store_files)
-
-                    df_log = structure.determine_optional_labels_in_log(df_log, records=self.records)
-
-                    self._import_nodes_from_data(df_log=df_log, file_name=file_name,
-                                                 required_labels_str=required_labels_str)
-
-                    if structure.has_datetime_attribute():
-                        # once all events are imported, we convert the string timestamp to the timestamp as used in
-                        # Cypher
-                        self._reformat_timestamps(structure=structure, required_labels_str=required_labels_str)
-
-                    # TODO: move filtering to pandas dataframe
-                    self._filter_nodes(structure=structure,
-                                       required_labels_str=required_labels_str)  # filter nodes according to the
-                    # structure
-                    self._finalize_import(required_labels_str=required_labels_str)  # removes temporary properties
-
-    @Performance.track("structure")
-    def _reformat_timestamps(self, structure, required_labels_str):
-        datetime_formats = structure.get_datetime_formats()
-        for attribute, datetime_format in datetime_formats.items():
-            if datetime_format.is_epoch:
-                self.connection.exec_query(di_ql.get_convert_epoch_to_timestamp_query,
-                                           **{
-                                               "required_labels_str": required_labels_str,
-                                               "attribute": attribute,
-                                               "datetime_object": datetime_format
-                                           })
-
-            self.connection.exec_query(di_ql.get_make_timestamp_date_query,
-                                       **{
-                                           "required_labels_str": required_labels_str,
-                                           "attribute": attribute,
-                                           "datetime_object": datetime_format,
-                                           "load_status": self.load_status
-                                       })
-
-    @Performance.track("structure")
-    def _filter_nodes(self, structure, required_labels_str):
-        for exclude in [True, False]:
-            attribute_values_pairs_filtered = structure.get_attribute_value_pairs_filtered(exclude=exclude)
-            for name, values in attribute_values_pairs_filtered.items():
-                self.connection.exec_query(di_ql.get_filter_records_by_property_query,
-                                           **{
-                                               "prop": name,
-                                               "values": values,
-                                               "exclude": exclude,
-                                               "load_status": self.load_status,
-                                               "required_labels_str": required_labels_str
-                                           })
-
-    @Performance.track("structure")
-    def _finalize_import(self, required_labels_str):
-        # finalize the import
-        self.connection.exec_query(di_ql.get_finalize_import_records_query,
-                                   **{
-                                       "load_status": self.load_status,
-                                       "required_labels_str": required_labels_str
-                                   })
-        self.load_status = 0
-
-    @Performance.track("file_name")
-    def _import_nodes_from_data(self, df_log, file_name, required_labels_str):
-        grouped_by_optional_labels = df_log.groupby(by="labels")
-        mapping_str = self._determine_column_mapping_str(df_log)
-
-        for optional_labels_str, log in grouped_by_optional_labels:
-            labels_str = required_labels_str + optional_labels_str
-            new_file_name = self.determine_new_file_name(file_name, optional_labels_str)
-            self.import_log_into_db(file_name=new_file_name, labels_str=labels_str, mapping_str=mapping_str, log=log)
-
-    def import_log_into_db(self, file_name, labels_str, mapping_str, log):
-        # Temporary save the file in the import directory
-        self._save_log_grouped_by_labels(log=log, file_name=file_name)
-        self.connection.exec_query(di_ql.get_create_nodes_by_loading_csv_query,
-                                   **{
-                                       "file_name": file_name,
-                                       "labels": labels_str,
-                                       "mapping": mapping_str
-                                   })
-
-        # delete the file from the import directory
-        self._delete_log_grouped_by_labels(file_name=file_name)
-
-    @staticmethod
-    def determine_new_file_name(file_name, optional_labels_str):
-        if optional_labels_str == "":
-            return file_name
-        return file_name[:-4] + "_" + optional_labels_str.replace(":", "_") + ".csv"
-
-    def _save_log_grouped_by_labels(self, log, file_name):
-        log = log.drop(columns=["labels"])
-        log.to_csv(Path(self.get_import_directory(), file_name), index=False)
-
-    def _delete_log_grouped_by_labels(self, file_name):
-        path = Path(self.get_import_directory(), file_name)
-        if os.path.exists(path):
-            os.remove(path)
-
-    @staticmethod
-    def _determine_column_mapping_str(log):
-        mapping = {}
-        dtypes = log.dtypes.to_dict()
-        for col_name, type in dtypes.items():
-            if type == object:
-                continue  # default is STRING
-            elif pd.api.types.is_integer_dtype(type):
-                mapping[col_name] = 'INTEGER'
-            elif pd.api.types.is_float_dtype(type):
-                mapping[col_name] = 'FLOAT'
-            elif pd.api.types.is_bool_dtype(type):
-                mapping[col_name] = 'BOOLEAN'
-            else:
-                raise Exception(f"Type for column {col_name} is not defined")
-
-        template_str = '$col_name:{type:"$type"}'
-        mapping_list = [Template(template_str).substitute({"col_name": col_name, "type": type}) for col_name, type in
-                        mapping.items()]
-        mapping_str = '{' + ','.join(mapping_list) + '}'
-        return mapping_str
-
-    def retrieve_import_directory(self):
-        result = self.connection.exec_query(di_ql.get_import_directory_query)
-        # get the correct value from the result
-        self._import_directory = result[0]['directory']
-
-    def get_import_directory(self):
-        if self._import_directory is None:
-            self.retrieve_import_directory()
-        return self._import_directory
+import os
+from string import Template
+from typing import Optional
+
+from ..data_managers.semantic_header import SemanticHeader
+from ..database_managers.db_connection import DatabaseConnection
+from ..data_managers.datastructures import DatasetDescriptions
+from ..utilities.performance_handling import Performance
+from ..cypher_queries.data_importer_ql import DataImporterQueryLibrary as di_ql
+from pathlib import Path
+import pandas as pd
+
+
+class Importer:
+    def __init__(self, database_connection: DatabaseConnection,
+                 data_structures: DatasetDescriptions,
+                 semantic_header: SemanticHeader,
+                 import_directory: Optional[str] = None,
+                 use_sample: bool = False,
+                 use_preprocessed_files: bool = False,
+                 store_files: bool = False):
+        self.connection = database_connection
+        self.structures = data_structures.structures
+        self.records = semantic_header.records
+
+        self.load_batch_size = 20000
+        self.use_sample = use_sample
+        self.use_preprocessed_files = use_preprocessed_files
+        self.store_files = store_files
+        self.load_status = 0
+
+        self._import_directory = import_directory
+
+    def update_load_status(self):
+        self.connection.exec_query(di_ql.get_update_load_status_query,
+                                   **{
+                                       "current_load_status": self.load_status
+                                   })
+        self.load_status += 1
+
+    def import_data(self, to_be_imported_logs) -> None:
+        for structure in self.structures:
+            required_labels_str = structure.get_required_labels_str(records=self.records)
+
+            # read in all file names that match this structure
+            for file_name in structure.file_names:
+                # only load files that are not imported yet
+                if to_be_imported_logs is None or file_name in to_be_imported_logs:
+                    # read and import the nodes
+                    df_log = structure.read_data_set(file_name=file_name,
+                                                     use_sample=self.use_sample,
+                                                     use_preprocessed_file=self.use_preprocessed_files,
+                                                     load_status=self.load_status,
+                                                     store_preprocessed_file=self.store_files)
+
+                    df_log = structure.determine_optional_labels_in_log(df_log, records=self.records)
+
+                    self._import_nodes_from_data(df_log=df_log, file_name=file_name,
+                                                 required_labels_str=required_labels_str)
+
+                    if structure.has_datetime_attribute():
+                        # once all events are imported, we convert the string timestamp to the timestamp as used in
+                        # Cypher
+                        self._reformat_timestamps(structure=structure, required_labels_str=required_labels_str)
+
+                    # TODO: move filtering to pandas dataframe
+                    self._filter_nodes(structure=structure,
+                                       required_labels_str=required_labels_str)  # filter nodes according to the
+                    # structure
+                    self._finalize_import(required_labels_str=required_labels_str)  # removes temporary properties
+
+    @Performance.track("structure")
+    def _reformat_timestamps(self, structure, required_labels_str):
+        datetime_formats = structure.get_datetime_formats()
+        for attribute, datetime_format in datetime_formats.items():
+            if datetime_format.is_epoch:
+                self.connection.exec_query(di_ql.get_convert_epoch_to_timestamp_query,
+                                           **{
+                                               "required_labels_str": required_labels_str,
+                                               "attribute": attribute,
+                                               "datetime_object": datetime_format
+                                           })
+
+            self.connection.exec_query(di_ql.get_make_timestamp_date_query,
+                                       **{
+                                           "required_labels_str": required_labels_str,
+                                           "attribute": attribute,
+                                           "datetime_object": datetime_format,
+                                           "load_status": self.load_status
+                                       })
+
+    @Performance.track("structure")
+    def _filter_nodes(self, structure, required_labels_str):
+        for exclude in [True, False]:
+            attribute_values_pairs_filtered = structure.get_attribute_value_pairs_filtered(exclude=exclude)
+            for name, values in attribute_values_pairs_filtered.items():
+                self.connection.exec_query(di_ql.get_filter_records_by_property_query,
+                                           **{
+                                               "prop": name,
+                                               "values": values,
+                                               "exclude": exclude,
+                                               "load_status": self.load_status,
+                                               "required_labels_str": required_labels_str
+                                           })
+
+    @Performance.track("structure")
+    def _finalize_import(self, required_labels_str):
+        # finalize the import
+        self.connection.exec_query(di_ql.get_finalize_import_records_query,
+                                   **{
+                                       "load_status": self.load_status,
+                                       "required_labels_str": required_labels_str
+                                   })
+        self.load_status = 0
+
+    @Performance.track("file_name")
+    def _import_nodes_from_data(self, df_log, file_name, required_labels_str):
+        grouped_by_optional_labels = df_log.groupby(by="labels")
+        mapping_str = self._determine_column_mapping_str(df_log)
+
+        for optional_labels_str, log in grouped_by_optional_labels:
+            labels_str = required_labels_str + optional_labels_str
+            new_file_name = self.determine_new_file_name(file_name, optional_labels_str)
+            self.import_log_into_db(file_name=new_file_name, labels_str=labels_str, mapping_str=mapping_str, log=log)
+
+    def import_log_into_db(self, file_name, labels_str, mapping_str, log):
+        # Temporary save the file in the import directory
+        self._save_log_grouped_by_labels(log=log, file_name=file_name)
+        self.connection.exec_query(di_ql.get_create_nodes_by_loading_csv_query,
+                                   **{
+                                       "file_name": file_name,
+                                       "labels": labels_str,
+                                       "mapping": mapping_str
+                                   })
+
+        # delete the file from the import directory
+        self._delete_log_grouped_by_labels(file_name=file_name)
+
+    @staticmethod
+    def determine_new_file_name(file_name, optional_labels_str):
+        if optional_labels_str == "":
+            return file_name
+        return file_name[:-4] + "_" + optional_labels_str.replace(":", "_") + ".csv"
+
+    def _save_log_grouped_by_labels(self, log, file_name):
+        log = log.drop(columns=["labels"])
+        log.to_csv(Path(self.get_import_directory(), file_name), index=False)
+
+    def _delete_log_grouped_by_labels(self, file_name):
+        path = Path(self.get_import_directory(), file_name)
+        if os.path.exists(path):
+            os.remove(path)
+
+    @staticmethod
+    def _determine_column_mapping_str(log):
+        mapping = {}
+        dtypes = log.dtypes.to_dict()
+        for col_name, type in dtypes.items():
+            if type == object:
+                continue  # default is STRING
+            elif pd.api.types.is_integer_dtype(type):
+                mapping[col_name] = 'INTEGER'
+            elif pd.api.types.is_float_dtype(type):
+                mapping[col_name] = 'FLOAT'
+            elif pd.api.types.is_bool_dtype(type):
+                mapping[col_name] = 'BOOLEAN'
+            else:
+                raise Exception(f"Type for column {col_name} is not defined")
+
+        template_str = '$col_name:{type:"$type"}'
+        mapping_list = [Template(template_str).substitute({"col_name": col_name, "type": type}) for col_name, type in
+                        mapping.items()]
+        mapping_str = '{' + ','.join(mapping_list) + '}'
+        return mapping_str
+
+    def retrieve_import_directory(self):
+        result = self.connection.exec_query(di_ql.get_import_directory_query)
+        # get the correct value from the result
+        self._import_directory = result[0]['directory']
+
+    def get_import_directory(self):
+        if self._import_directory is None:
+            self.retrieve_import_directory()
+        return self._import_directory
```

### Comparing `promg-1.0.9/src/promg/modules/ekg_builder_semantic_header.py` & `promg-1.1.0/src/promg/modules/ekg_builder_semantic_header.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,151 +1,164 @@
-from typing import Optional, List, Union
-
-from ..data_managers.semantic_header import ConstructedNodes, ConstructedRelation, Relationship, SemanticHeader, \
-    NodeConstructor
-from ..database_managers.db_connection import DatabaseConnection
-from ..utilities.performance_handling import Performance
-from ..cypher_queries.semantic_header_ql import SemanticHeaderQueryLibrary as sh_ql
-
-
-class EKGUsingSemanticHeaderBuilder:
-    def __init__(self, database_connection: DatabaseConnection,
-                 semantic_header: SemanticHeader):
-        self.connection = database_connection
-        self.semantic_header = semantic_header
-
-    def create_nodes_by_records(self, node_types: Optional[List[str]]) -> None:
-        for node_constructor in self.semantic_header.get_node_by_record_constructors(node_types):
-            self._create_node_by_record(node_constructor=node_constructor)
-
-    @Performance.track("node_constructor")
-    def _create_node_by_record(self, node_constructor: NodeConstructor):
-        num_ids = self.connection.exec_query(sh_ql.get_number_of_ids_query,
-                                             **{
-                                                 "node_constructor": node_constructor,
-                                                 "use_record": True
-                                             })
-        merge_first = num_ids[0]['num_ids'] < 1000 \
-                      and "Event" not in node_constructor.get_labels() \
-                      and "EntityAttribute" not in node_constructor.get_labels()
-
-        self.connection.exec_query(sh_ql.get_create_node_by_record_constructor_query,
-                                   **{
-                                       "node_constructor": node_constructor,
-                                       "merge": merge_first
-                                   })
-
-        self.connection.exec_query(sh_ql.get_reset_created_record_query)
-
-        if merge_first:
-            print(
-                f"Node ({node_constructor.get_pattern(with_properties=False)})"
-                f"using ({node_constructor.get_prevalent_record_pattern()}) merged")
-        else:
-            print(f"Node ({node_constructor.get_pattern(with_properties=False)}) "
-                  f"using ({node_constructor.get_prevalent_record_pattern()}) "
-                  f"created")
-            if not ("Event" in node_constructor.get_labels() or "EntityAttribute" in node_constructor.get_labels()):
-                self.connection.exec_query(sh_ql.get_merge_nodes_with_same_id_query,
-                                           **{
-                                               "node_constructor": node_constructor
-                                           }
-                                           )
-
-                self.connection.exec_query(sh_ql.get_reset_merged_in_nodes_query,
-                                           **{
-                                               "node_constructor": node_constructor
-                                           }
-                                           )
-
-    def create_nodes_by_relations(self, node_types: Optional[List[str]]) -> None:
-        for node_constructors in self.semantic_header.get_nodes_constructed_by_relations(node_types).values():
-            for node_constructor in node_constructors:
-                self._create_node_by_relation(node_constructor=node_constructor)
-
-    @Performance.track("node_constructor")
-    def _create_node_by_relation(self, node_constructor: NodeConstructor):
-        pass
-
-    def create_relations_using_records(self, relation_types: Optional[List[str]]) -> None:
-        # find events that are related to different entities of which one event also has a reference to the other entity
-        # create a relation between these two entities
-        relation: ConstructedRelation
-        for relation_constructor in self.semantic_header.get_relations_constructed_by_record(relation_types):
-            self._create_relations_using_record(relation_constructor=relation_constructor)
-
-    @Performance.track("relation_constructor")
-    def _create_relations_using_record(self, relation_constructor):
-        self.connection.exec_query(sh_ql.get_create_relation_using_record_query,
-                                   **{
-                                       "relation_constructor": relation_constructor
-                                   })
-        self.connection.exec_query(sh_ql.get_reset_created_record_query)
-        self._create_corr_from_parents(relation_constructor=relation_constructor)
-
-    def create_relations_using_relations(self, relation_types: Optional[List[str]]) -> None:
-        relation: ConstructedRelation
-        for relation_constructor in self.semantic_header.get_relations_constructed_by_relations(relation_types):
-            self._create_relations_using_relation(relation_constructor=relation_constructor)
-
-    @Performance.track("relation_constructor")
-    def _create_relations_using_relation(self, relation_constructor):
-        self.connection.exec_query(sh_ql.get_create_relation_by_relations_query,
-                                   **{
-                                       "relation_constructor": relation_constructor
-                                   })
-        self._create_corr_from_parents(relation_constructor=relation_constructor)
-
-    def _create_corr_from_parents(self, relation_constructor):
-        if relation_constructor.infer_corr_from_reified_parents:
-            for use_from in [True, False]:
-                self.connection.exec_query(sh_ql.get_infer_corr_from_parent_query,
-                                           **{
-                                               "relation_constructor": relation_constructor,
-                                               "use_from": use_from
-                                           })
-
-    def create_df_edges(self, entity_types: List[str], event_label: str, add_duration: bool = False) -> None:
-        """
-        Create Directly Follows edges for the given entity types using the semantic header information
-        :param entity_types: list of entity types for which DF edge should be created. If None, we try for all entities
-        :param event_label: the labels of the event nodes for which we want to create the event_label
-        :param add_duration: boolean indicating whether we want to add the duration to the df edges
-        :return: None
-        """
-        entity: ConstructedNodes
-
-        if entity_types is None:
-            entity_types = [entity.type for entity in self.semantic_header.nodes] \
-                           + [relation.type for relation in self.semantic_header.relations if relation.model_as_node]
-
-        for entity in self.semantic_header.nodes:
-            if entity.infer_df and entity.type in entity_types:
-                self._create_df_edges_for_entity(entity=entity, event_label=event_label, add_duration=add_duration)
-
-        for relation in self.semantic_header.relations:
-            if relation.model_as_node and relation.infer_df and relation.type in entity_types:
-                self._create_df_edges_for_entity(entity=relation, event_label=event_label, add_duration=add_duration)
-
-    @Performance.track("entity")
-    def _create_df_edges_for_entity(self, entity: Union[ConstructedNodes, ConstructedRelation], event_label,
-                                    add_duration):
-        self.connection.exec_query(sh_ql.get_create_directly_follows_query,
-                                   **{
-                                       "entity": entity,
-                                       "event_label": event_label,
-                                       "add_duration": add_duration
-                                   })
-
-    def merge_duplicate_df(self):
-        node: ConstructedNodes
-        for node in self.semantic_header.nodes:
-            if node.merge_duplicate_df:
-                self._merge_duplicate_df_for_node(node=node)
-
-    @Performance.track("node")
-    def _merge_duplicate_df_for_node(self, node: ConstructedNodes):
-        self.connection.exec_query(sh_ql.get_merge_duplicate_df_entity_query, **{"node": node})
-
-    def create_static_nodes_and_relations(self):
-        print("No implementation yet")
-        pass
+from typing import Optional, List, Union
+
+from ..data_managers.semantic_header import ConstructedNodes, ConstructedRelation, Relationship, SemanticHeader, \
+    NodeConstructor
+from ..database_managers.db_connection import DatabaseConnection
+from ..utilities.performance_handling import Performance
+from ..cypher_queries.semantic_header_ql import SemanticHeaderQueryLibrary as sh_ql
+
+
+class EKGUsingSemanticHeaderBuilder:
+    def __init__(self, database_connection: DatabaseConnection,
+                 semantic_header: SemanticHeader):
+        self.connection = database_connection
+        self.semantic_header = semantic_header
+
+    def create_nodes_by_records(self, node_types: Optional[List[str]], logs: Optional[List[str]]) -> None:
+        # request all associated record labels of the imported logs
+        associated_records = self.get_associated_records(logs)
+
+        for node_constructor in self.semantic_header.get_node_by_record_constructors(node_types):
+            # check if node_constructor is subset of associated record labels
+            # if so, we need to create nodes for this record
+            is_subset = set(node_constructor.prevalent_record.labels).issubset(set(associated_records))
+            if logs is None or is_subset:
+                self._create_node_by_record(node_constructor=node_constructor, logs=logs)
+
+    def get_associated_records(self, logs):
+        # if imported logs, we can return an empty list
+        if logs is None:
+            return []
+        else:
+            # request the associated record labels
+            result = self.connection.exec_query(sh_ql.get_associated_record_labels_query,
+                                   **{
+                                       "logs": logs
+                                   })
+            return result[0]["labels"]
+
+    @Performance.track("node_constructor")
+    def _create_node_by_record(self, node_constructor: NodeConstructor, logs: Optional[List[str]]):
+
+        merge_first = "Event" not in node_constructor.get_labels() \
+                      and "EntityAttribute" not in node_constructor.get_labels()
+
+        self.connection.exec_query(sh_ql.get_create_node_by_record_constructor_query,
+                                   **{
+                                       "node_constructor": node_constructor,
+                                       "merge": merge_first,
+                                       "logs": logs
+                                   })
+
+        if merge_first:
+            print(
+                f"Node ({node_constructor.get_pattern(with_properties=False)})"
+                f"using ({node_constructor.get_prevalent_record_pattern()}) merged")
+        else:
+            print(f"Node ({node_constructor.get_pattern(with_properties=False)}) "
+                  f"using ({node_constructor.get_prevalent_record_pattern()}) "
+                  f"created")
+
+    def create_nodes_by_relations(self, node_types: Optional[List[str]]) -> None:
+        for node_constructors in self.semantic_header.get_nodes_constructed_by_relations(node_types).values():
+            for node_constructor in node_constructors:
+                self._create_node_by_relation(node_constructor=node_constructor)
+
+    @Performance.track("node_constructor")
+    def _create_node_by_relation(self, node_constructor: NodeConstructor):
+        pass
+
+    def create_relations_using_records(self, relation_types: Optional[List[str]],
+                                       logs: Optional[List[str]] = None) -> None:
+        # find events that are related to different entities of which one event also has a reference to the other entity
+        # create a relation between these two entities
+        relation: ConstructedRelation
+
+        # request all associated record labels of the imported logs
+        associated_records = self.get_associated_records(logs)
+
+        for relation_constructor in self.semantic_header.get_relations_constructed_by_record(relation_types):
+            # check if node_constructor is subset of associated record labels
+            # if so, we need to create nodes for this record
+            is_subset = set(relation_constructor.prevalent_record.labels).issubset(set(associated_records))
+            if logs is None or is_subset:
+                self._create_relations_using_record(relation_constructor=relation_constructor,
+                                                    logs=logs)
+
+
+
+    @Performance.track("relation_constructor")
+    def _create_relations_using_record(self, relation_constructor, logs: Optional[List[str]] = None):
+        self.connection.exec_query(sh_ql.get_create_relation_using_record_query,
+                                   **{
+                                       "relation_constructor": relation_constructor,
+                                       "logs": logs
+                                   })
+        self._create_corr_from_parents(relation_constructor=relation_constructor)
+
+    def create_relations_using_relations(self, relation_types: Optional[List[str]]) -> None:
+        relation: ConstructedRelation
+        for relation_constructor in self.semantic_header.get_relations_constructed_by_relations(relation_types):
+            self._create_relations_using_relation(relation_constructor=relation_constructor)
+
+    @Performance.track("relation_constructor")
+    def _create_relations_using_relation(self, relation_constructor):
+        self.connection.exec_query(sh_ql.get_create_relation_by_relations_query,
+                                   **{
+                                       "relation_constructor": relation_constructor
+                                   })
+        self._create_corr_from_parents(relation_constructor=relation_constructor)
+
+    def _create_corr_from_parents(self, relation_constructor):
+        if relation_constructor.infer_corr_from_reified_parents:
+            for use_from in [True, False]:
+                self.connection.exec_query(sh_ql.get_infer_corr_from_parent_query,
+                                           **{
+                                               "relation_constructor": relation_constructor,
+                                               "use_from": use_from
+                                           })
+
+    def create_df_edges(self, entity_types: List[str], event_label: str, add_duration: bool = False) -> None:
+        """
+        Create Directly Follows edges for the given entity types using the semantic header information
+        :param entity_types: list of entity types for which DF edge should be created. If None, we try for all entities
+        :param event_label: the labels of the event nodes for which we want to create the event_label
+        :param add_duration: boolean indicating whether we want to add the duration to the df edges
+        :return: None
+        """
+        entity: ConstructedNodes
+
+        if entity_types is None:
+            entity_types = [entity.type for entity in self.semantic_header.nodes] \
+                           + [relation.type for relation in self.semantic_header.relations if relation.model_as_node]
+
+        for entity in self.semantic_header.nodes:
+            if entity.infer_df and entity.type in entity_types:
+                self._create_df_edges_for_entity(entity=entity, event_label=event_label, add_duration=add_duration)
+
+        for relation in self.semantic_header.relations:
+            if relation.model_as_node and relation.infer_df and relation.type in entity_types:
+                self._create_df_edges_for_entity(entity=relation, event_label=event_label, add_duration=add_duration)
+
+    @Performance.track("entity")
+    def _create_df_edges_for_entity(self, entity: Union[ConstructedNodes, ConstructedRelation], event_label,
+                                    add_duration):
+        self.connection.exec_query(sh_ql.get_create_directly_follows_query,
+                                   **{
+                                       "entity": entity,
+                                       "event_label": event_label,
+                                       "add_duration": add_duration
+                                   })
+
+    def merge_duplicate_df(self):
+        node: ConstructedNodes
+        for node in self.semantic_header.nodes:
+            if node.merge_duplicate_df:
+                self._merge_duplicate_df_for_node(node=node)
+
+    @Performance.track("node")
+    def _merge_duplicate_df_for_node(self, node: ConstructedNodes):
+        self.connection.exec_query(sh_ql.get_merge_duplicate_df_entity_query, **{"node": node})
+
+    def create_static_nodes_and_relations(self):
+        print("No implementation yet")
+        pass
```

### Comparing `promg-1.0.9/src/promg/modules/exporter.py` & `promg-1.1.0/src/promg/modules/exporter.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import os
-from typing import List, Optional, Dict, Any
-
-import pandas as pd
-
-from ..cypher_queries.exporter_ql import ExporterQueryLibrary as exporter_ql
-from ..data_managers.semantic_header import ConstructedNodes, SemanticHeader
-from ..database_managers.db_connection import DatabaseConnection
-
-
-class Exporter:
-    def __init__(self, db_connection):
-        self.connection = db_connection
-
-    def get_event_log(self, entity_type, additional_event_attributes: Optional[List[str]] = None) -> List[
-        Dict[str, Any]]:
-        """
-        Get an event log extracted from the EKG for a specific entity and return it
-
-        Args:
-            entity_type: The type of the entity --> contract states that it exists
-            additional_event_attributes: list of different attributes of event that should also be stored in the
-            event log
-
-        Returns:
-            A list of events with its attributes in the form of a dictionary
-
-        Raises:
-             ValueError: when the entity has not been defined
-        """
-
-        entity_object = SemanticHeader().get_entity(entity_type)
-        if entity_object is None:
-            raise ValueError(f"Entity {entity_type} is not defined in the semantic header")
-
-        return self._get_event_log(entity_object, additional_event_attributes)
-
-    def _get_event_log(self, entity: ConstructedNodes, additional_event_attributes: Optional[List[str]] = None) -> \
-            Optional[List[Dict[str, Any]]]:
-        """
-        Get an event log extracted from the EKG for a specific entity and return it
-
-        Args:
-            entity: The entity for which we want to extract an event log
-            additional_event_attributes: list of different attributes of event that should also be stored in the
-            event log
-
-        Returns:
-            A list of events with its attributes in the form of a dictionary
-        """
-        if additional_event_attributes is None:
-            additional_event_attributes = []
-        return self.connection.exec_query(exporter_ql.get_event_log_query,
-                                          **{
-                                              "entity": entity,
-                                              "additional_event_attributes": additional_event_attributes
-                                          })
-
-    def save_event_log(self, entity_type: str, additional_event_attributes: Optional[List[str]] = None) -> None:
-        """
-        Create an event log extracted from the EKG from a specific entity and store it as a csv file
-
-        Args:
-            entity_type: The type of the entity
-             additional_event_attributes: list of different attributes of event that should also be stored in the
-             event log
-        """
-
-        event_log = self.get_event_log(entity_type, additional_event_attributes)
-        df = pd.DataFrame(event_log)
-
-        current_file_path = os.path.dirname(__file__)
-
-        dir_path = os.path.join(current_file_path, '../../..', '..', 'data', SemanticHeader().name, 'event_logs')
-        file_path = os.path.join(dir_path, f"{entity_type}.csv")
-        os.makedirs(dir_path, exist_ok=True)
-        df.to_csv(file_path, index=True, index_label="idx")
+import os
+from typing import List, Optional, Dict, Any
+
+import pandas as pd
+
+from ..cypher_queries.exporter_ql import ExporterQueryLibrary as exporter_ql
+from ..data_managers.semantic_header import ConstructedNodes, SemanticHeader
+from ..database_managers.db_connection import DatabaseConnection
+
+
+class Exporter:
+    def __init__(self, db_connection):
+        self.connection = db_connection
+
+    def get_event_log(self, entity_type, additional_event_attributes: Optional[List[str]] = None) -> List[
+        Dict[str, Any]]:
+        """
+        Get an event log extracted from the EKG for a specific entity and return it
+
+        Args:
+            entity_type: The type of the entity --> contract states that it exists
+            additional_event_attributes: list of different attributes of event that should also be stored in the
+            event log
+
+        Returns:
+            A list of events with its attributes in the form of a dictionary
+
+        Raises:
+             ValueError: when the entity has not been defined
+        """
+
+        entity_object = SemanticHeader().get_entity(entity_type)
+        if entity_object is None:
+            raise ValueError(f"Entity {entity_type} is not defined in the semantic header")
+
+        return self._get_event_log(entity_object, additional_event_attributes)
+
+    def _get_event_log(self, entity: ConstructedNodes, additional_event_attributes: Optional[List[str]] = None) -> \
+            Optional[List[Dict[str, Any]]]:
+        """
+        Get an event log extracted from the EKG for a specific entity and return it
+
+        Args:
+            entity: The entity for which we want to extract an event log
+            additional_event_attributes: list of different attributes of event that should also be stored in the
+            event log
+
+        Returns:
+            A list of events with its attributes in the form of a dictionary
+        """
+        if additional_event_attributes is None:
+            additional_event_attributes = []
+        return self.connection.exec_query(exporter_ql.get_event_log_query,
+                                          **{
+                                              "entity": entity,
+                                              "additional_event_attributes": additional_event_attributes
+                                          })
+
+    def save_event_log(self, entity_type: str, additional_event_attributes: Optional[List[str]] = None) -> None:
+        """
+        Create an event log extracted from the EKG from a specific entity and store it as a csv file
+
+        Args:
+            entity_type: The type of the entity
+             additional_event_attributes: list of different attributes of event that should also be stored in the
+             event log
+        """
+
+        event_log = self.get_event_log(entity_type, additional_event_attributes)
+        df = pd.DataFrame(event_log)
+
+        current_file_path = os.path.dirname(__file__)
+
+        dir_path = os.path.join(current_file_path, '../../..', '..', 'data', SemanticHeader().name, 'event_logs')
+        file_path = os.path.join(dir_path, f"{entity_type}.csv")
+        os.makedirs(dir_path, exist_ok=True)
+        df.to_csv(file_path, index=True, index_label="idx")
```

### Comparing `promg-1.0.9/src/promg/modules/inference_engine.py` & `promg-1.1.0/src/promg/modules/inference_engine.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from .. import SemanticHeader
-from ..cypher_queries.inference_engine_ql import InferenceEngineQueryLibrary as ie_ql
-from ..data_managers.semantic_header import ConstructedNodes
-from ..utilities.performance_handling import Performance
-from ..database_managers.db_connection import DatabaseConnection
-
-
-class InferenceEngine:
-    def __init__(self, db_connection):
-        self.connection = db_connection
-
-    def match_entity_with_batch_position(self, entity_type: str, relative_position_type: str) -> None:
-        """
-        Infer the batch position of a specific entity
-
-        Args:
-            entity_type: The type of the entity
-             relative_position_type: The type of the relative position
-
-        Raises:
-             ValueError: when the entity has not been defined
-        """
-        entity = SemanticHeader().get_entity(entity_type)
-        relative_position = SemanticHeader().get_entity(relative_position_type)
-        if entity is None:
-            raise ValueError(f"{entity_type} is not defined in semantic header")
-        if relative_position is None:
-            raise ValueError(f"{relative_position} is not defined in semantic header")
-        self._match_entity_with_batch_position(entity, relative_position)
-
-    @Performance.track("entity")
-    def _match_entity_with_batch_position(self, entity: ConstructedNodes, relative_position: ConstructedNodes):
-        self.connection.exec_query(ie_ql.get_match_entity_with_batch_position_query, **{
-            "entity": entity,
-            "relative_position": relative_position
-        })
-
-    # rule B
-    def infer_items_propagate_downwards_one_level(self, entity_type: str) -> None:
-        """
-        Infer items while propagating downwards one level
-
-        Args:
-            entity_type: The type of the entity
-
-        Raises:
-             ValueError: when the entity has not been defined
-        """
-        entity = SemanticHeader().get_entity(entity_type)
-        if entity_type is None:
-            raise ValueError(f"{entity_type} is not defined in semantic header")
-        self._infer_items_propagate_downwards_one_level(entity)
-
-    @Performance.track("entity")
-    def _infer_items_propagate_downwards_one_level(self, entity: ConstructedNodes):
-        self.connection.exec_query(ie_ql.get_query_infer_items_propagate_downwards_one_level, **{"entity": entity})
-
-    # rule C
-    def infer_items_propagate_upwards_multiple_levels(self, entity_type: str, is_load=True) -> None:
-        """
-        Infer items while propagating upwards multiple levels (Rule C)
-
-        Args:
-            entity_type: The type of the entity
-            is_load: indicating whether we are inferring upwards to load events (true) or unload events (false)
-
-        Raises:
-            ValueError: when the entity has not been defined
-        """
-
-        entity = SemanticHeader().get_entity(entity_type)
-        if entity is None:
-            raise ValueError(f"{entity_type} is not defined in semantic header")
-        self._infer_items_propagate_upwards_multiple_levels(entity, is_load)
-
-    @Performance.track("entity")
-    def _infer_items_propagate_upwards_multiple_levels(self, entity, is_load=True):
-        self.connection.exec_query(ie_ql.get_query_infer_items_propagate_upwards_multiple_levels,
-                                   **{
-                                       "entity": entity,
-                                       "is_load": is_load
-                                   })
-
-    # rule D
-    def infer_items_propagate_downwards_multiple_level_w_batching(self, entity_type: str,
-                                                                  relative_position_type: str, ) -> None:
-        """
-        Infer items while propagating downwards multiple levels with batching (rule D)
-
-        Args:
-            entity_type: The type of the entity
-            relative_position_type: The type of the relative position
-
-        Raises:
-            ValueError: when the entity has not been defined in semantic header
-        """
-        entity = SemanticHeader().get_entity(entity_type)
-        relative_position = SemanticHeader().get_entity(relative_position_type)
-        if entity_type is None:
-            raise ValueError(f"{entity_type} is not defined in semantic header")
-        self._infer_items_propagate_downwards_multiple_level_w_batching(entity, relative_position)
-
-    @Performance.track("entity")
-    def _infer_items_propagate_downwards_multiple_level_w_batching(self, entity, relative_position):
-        self.connection.exec_query(ie_ql.get_query_infer_items_propagate_downwards_multiple_level_w_batching,
-                                   **{"entity": entity, "relative_position": relative_position})
+from .. import SemanticHeader
+from ..cypher_queries.inference_engine_ql import InferenceEngineQueryLibrary as ie_ql
+from ..data_managers.semantic_header import ConstructedNodes
+from ..utilities.performance_handling import Performance
+from ..database_managers.db_connection import DatabaseConnection
+
+
+class InferenceEngine:
+    def __init__(self, db_connection):
+        self.connection = db_connection
+
+    def match_entity_with_batch_position(self, entity_type: str, relative_position_type: str) -> None:
+        """
+        Infer the batch position of a specific entity
+
+        Args:
+            entity_type: The type of the entity
+             relative_position_type: The type of the relative position
+
+        Raises:
+             ValueError: when the entity has not been defined
+        """
+        entity = SemanticHeader().get_entity(entity_type)
+        relative_position = SemanticHeader().get_entity(relative_position_type)
+        if entity is None:
+            raise ValueError(f"{entity_type} is not defined in semantic header")
+        if relative_position is None:
+            raise ValueError(f"{relative_position} is not defined in semantic header")
+        self._match_entity_with_batch_position(entity, relative_position)
+
+    @Performance.track("entity")
+    def _match_entity_with_batch_position(self, entity: ConstructedNodes, relative_position: ConstructedNodes):
+        self.connection.exec_query(ie_ql.get_match_entity_with_batch_position_query, **{
+            "entity": entity,
+            "relative_position": relative_position
+        })
+
+    # rule B
+    def infer_items_propagate_downwards_one_level(self, entity_type: str) -> None:
+        """
+        Infer items while propagating downwards one level
+
+        Args:
+            entity_type: The type of the entity
+
+        Raises:
+             ValueError: when the entity has not been defined
+        """
+        entity = SemanticHeader().get_entity(entity_type)
+        if entity_type is None:
+            raise ValueError(f"{entity_type} is not defined in semantic header")
+        self._infer_items_propagate_downwards_one_level(entity)
+
+    @Performance.track("entity")
+    def _infer_items_propagate_downwards_one_level(self, entity: ConstructedNodes):
+        self.connection.exec_query(ie_ql.get_query_infer_items_propagate_downwards_one_level, **{"entity": entity})
+
+    # rule C
+    def infer_items_propagate_upwards_multiple_levels(self, entity_type: str, is_load=True) -> None:
+        """
+        Infer items while propagating upwards multiple levels (Rule C)
+
+        Args:
+            entity_type: The type of the entity
+            is_load: indicating whether we are inferring upwards to load events (true) or unload events (false)
+
+        Raises:
+            ValueError: when the entity has not been defined
+        """
+
+        entity = SemanticHeader().get_entity(entity_type)
+        if entity is None:
+            raise ValueError(f"{entity_type} is not defined in semantic header")
+        self._infer_items_propagate_upwards_multiple_levels(entity, is_load)
+
+    @Performance.track("entity")
+    def _infer_items_propagate_upwards_multiple_levels(self, entity, is_load=True):
+        self.connection.exec_query(ie_ql.get_query_infer_items_propagate_upwards_multiple_levels,
+                                   **{
+                                       "entity": entity,
+                                       "is_load": is_load
+                                   })
+
+    # rule D
+    def infer_items_propagate_downwards_multiple_level_w_batching(self, entity_type: str,
+                                                                  relative_position_type: str, ) -> None:
+        """
+        Infer items while propagating downwards multiple levels with batching (rule D)
+
+        Args:
+            entity_type: The type of the entity
+            relative_position_type: The type of the relative position
+
+        Raises:
+            ValueError: when the entity has not been defined in semantic header
+        """
+        entity = SemanticHeader().get_entity(entity_type)
+        relative_position = SemanticHeader().get_entity(relative_position_type)
+        if entity_type is None:
+            raise ValueError(f"{entity_type} is not defined in semantic header")
+        self._infer_items_propagate_downwards_multiple_level_w_batching(entity, relative_position)
+
+    @Performance.track("entity")
+    def _infer_items_propagate_downwards_multiple_level_w_batching(self, entity, relative_position):
+        self.connection.exec_query(ie_ql.get_query_infer_items_propagate_downwards_multiple_level_w_batching,
+                                   **{"entity": entity, "relative_position": relative_position})
```

### Comparing `promg-1.0.9/src/promg/modules/task_identification.py` & `promg-1.1.0/src/promg/modules/task_identification.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from ..cypher_queries.task_identification_ql import TaskIdentifierLibrary as tf_ql
-from ..data_managers.semantic_header import ConstructedNodes, SemanticHeader
-from ..utilities.performance_handling import Performance
-from ..database_managers.db_connection import DatabaseConnection
-
-
-class TaskIdentification:
-    def __init__(self, db_connection, semantic_header, resource: str, case: str):
-        self.connection = db_connection
-        self.resource: ConstructedNodes = semantic_header.get_entity(resource)
-        self.case: ConstructedNodes = semantic_header.get_entity(case)
-
-    @Performance.track("resource")
-    def identify_tasks(self):
-        self.connection.exec_query(tf_ql.get_combine_df_joint_query,
-                                   **{
-                                       "resource": self.resource,
-                                       "case": self.case
-                                   })
-
-        self.connection.exec_query(tf_ql.get_create_task_instances_query,
-                                   **{"resource": self.resource})
-        self.connection.exec_query(tf_ql.get_split_ti_nodes_create_new_1_query)
-        self.connection.exec_query(tf_ql.get_split_ti_nodes_create_new_2_query)
-        self.connection.exec_query(tf_ql.get_split_ti_nodes_remove_old_query)
-        self.connection.exec_query(tf_ql.get_remove_df_joint_query)
-        for entity in [self.resource, self.case]:
-            self.connection.exec_query(tf_ql.get_correlate_ti_to_entity_query,
-                                       **{"entity": entity})
-            self.connection.exec_query(tf_ql.get_lift_df_to_task_instances_query,
-                                       **{"entity": entity})
-
-    @Performance.track("resource")
-    def aggregate_on_task_variant(self):
-        self.connection.exec_query(tf_ql.get_aggregate_task_instances_query,
-                                   **{"property": "variant"})
-        self.connection.exec_query(tf_ql.get_link_task_instances_to_aggregations_query,
-                                   **{"property": "variant"})
-        for entity in [self.resource, self.case]:
-            self.connection.exec_query(tf_ql.get_lift_df_to_task_aggregations_query,
-                                       **{
-                                           "property": "variant",
-                                           "entity": entity
-                                       })
+from ..cypher_queries.task_identification_ql import TaskIdentifierLibrary as tf_ql
+from ..data_managers.semantic_header import ConstructedNodes, SemanticHeader
+from ..utilities.performance_handling import Performance
+from ..database_managers.db_connection import DatabaseConnection
+
+
+class TaskIdentification:
+    def __init__(self, db_connection, semantic_header, resource: str, case: str):
+        self.connection = db_connection
+        self.resource: ConstructedNodes = semantic_header.get_entity(resource)
+        self.case: ConstructedNodes = semantic_header.get_entity(case)
+
+    @Performance.track("resource")
+    def identify_tasks(self):
+        self.connection.exec_query(tf_ql.get_combine_df_joint_query,
+                                   **{
+                                       "resource": self.resource,
+                                       "case": self.case
+                                   })
+
+        self.connection.exec_query(tf_ql.get_create_task_instances_query,
+                                   **{"resource": self.resource})
+        self.connection.exec_query(tf_ql.get_split_ti_nodes_create_new_1_query)
+        self.connection.exec_query(tf_ql.get_split_ti_nodes_create_new_2_query)
+        self.connection.exec_query(tf_ql.get_split_ti_nodes_remove_old_query)
+        self.connection.exec_query(tf_ql.get_remove_df_joint_query)
+        for entity in [self.resource, self.case]:
+            self.connection.exec_query(tf_ql.get_correlate_ti_to_entity_query,
+                                       **{"entity": entity})
+            self.connection.exec_query(tf_ql.get_lift_df_to_task_instances_query,
+                                       **{"entity": entity})
+
+    @Performance.track("resource")
+    def aggregate_on_task_variant(self):
+        self.connection.exec_query(tf_ql.get_aggregate_task_instances_query,
+                                   **{"property": "variant"})
+        self.connection.exec_query(tf_ql.get_link_task_instances_to_aggregations_query,
+                                   **{"property": "variant"})
+        for entity in [self.resource, self.case]:
+            self.connection.exec_query(tf_ql.get_lift_df_to_task_aggregations_query,
+                                       **{
+                                           "property": "variant",
+                                           "entity": entity
+                                       })
```

### Comparing `promg-1.0.9/src/promg/utilities/auxiliary_functions.py` & `promg-1.1.0/src/promg/utilities/auxiliary_functions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import re
-from typing import Any, Optional, Dict, List
-
-
-def replace_undefined_value(item, value):
-    return item if item is not None else value
-
-
-def create_list(class_type: Any, obj: Optional[Dict[str, Any]], *args) -> List[Any]:
-    if obj is None:
-        return []
-    else:
-        if type(obj) is list:
-            new_list = [class_type.from_dict(y, *args) for y in obj]
-        elif type(obj) is dict:
-            new_list = [class_type.from_dict(obj, *args)]
-        else:
-            raise TypeError(f"The type of the object of {class_type} is ill defined")
-        new_list = [item for item in new_list if item is not None]
-        return new_list
-
-
-def get_id_attribute_from_label(label):
-    search_first_lower_case = re.search("[a-z]", label)
-    if search_first_lower_case is not None:
-        first_lower_case = search_first_lower_case.start()
-    else: # no lower case has been found
-        first_lower_case = len(label)
-    return label[:first_lower_case].lower() + label[first_lower_case:] + "Id"
+import re
+from typing import Any, Optional, Dict, List
+
+
+def replace_undefined_value(item, value):
+    return item if item is not None else value
+
+
+def create_list(class_type: Any, obj: Optional[Dict[str, Any]], *args) -> List[Any]:
+    if obj is None:
+        return []
+    else:
+        if type(obj) is list:
+            new_list = [class_type.from_dict(y, *args) for y in obj]
+        elif type(obj) is dict:
+            new_list = [class_type.from_dict(obj, *args)]
+        else:
+            raise TypeError(f"The type of the object of {class_type} is ill defined")
+        new_list = [item for item in new_list if item is not None]
+        return new_list
+
+
+def get_id_attribute_from_label(label):
+    search_first_lower_case = re.search("[a-z]", label)
+    if search_first_lower_case is not None:
+        first_lower_case = search_first_lower_case.start()
+    else: # no lower case has been found
+        first_lower_case = len(label)
+    return label[:first_lower_case].lower() + label[first_lower_case:] + "Id"
```

### Comparing `promg-1.0.9/src/promg/utilities/get_db_size.py` & `promg-1.1.0/src/promg/utilities/get_db_size.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from neo4j import GraphDatabase
-
-driver = GraphDatabase.driver("bolt://localhost:7687", auth=("neo4j", "12345678"))
-
-#match (e:Event),(n:Entity),(c:Class),(l:Log),()-[df:DF]->(),()-[corr:E_EN]->() return count(e),count(n),count(c),count(l),count(df),count(corr)
-
-def get_size(tx):
-    num_events, num_entity, num_log, num_class, num_df, num_corr, num_rel, num_total_nodes, num_total_relationships\
-        = 0, 0, 0, 0, 0, 0, 0, 0, 0
-    q = f'''match (e:Event) RETURN count(e)'''
-    for record in tx.run(q):
-        num_events = record["count(e)"]
-
-    q = f'''match (e:Entity) RETURN count(e)'''
-    for record in tx.run(q):
-        num_entity = record["count(e)"]
-
-    q = f'''match (l:Log) RETURN count(l)'''
-    for record in tx.run(q):
-        num_log = record["count(l)"]
-
-    q = f'''match (c:Class) RETURN count(c)'''
-    for record in tx.run(q):
-        num_class = record["count(c)"]
-
-    q = f'''match ()-[df:DF]->() RETURN count(df)'''
-    for record in tx.run(q):
-        num_df = record["count(df)"]
-
-    q = f'''match ()-[corr:E_EN]->() RETURN count(corr)'''
-    for record in tx.run(q):
-        num_corr = record["count(corr)"]
-
-    q = f'''match ()-[r:REL]->() RETURN count(r)'''
-    for record in tx.run(q):
-        num_rel = record["count(r)"]
-
-    q = f'''match (n) RETURN count(n)'''
-    for record in tx.run(q):
-        num_total_nodes = record["count(n)"]
-
-    q = f'''match ()-[r]->() RETURN count(r)'''
-    for record in tx.run(q):
-        num_total_relationships = record["count(r)"]
-
-    print(f'''Nodes (total);Event;Entity;Log;Class;Relationships (total);DF;CORR;REL''')
-    print(f'''{num_total_nodes};{num_events};{num_entity};{num_log};{num_class};{num_total_relationships};{num_df};
-    {num_corr};{num_rel}''')
-
-
-
-with driver.session() as session:
-    session.read_transaction(get_size)
+from neo4j import GraphDatabase
+
+driver = GraphDatabase.driver("bolt://localhost:7687", auth=("neo4j", "12345678"))
+
+#match (e:Event),(n:Entity),(c:Class),(l:Log),()-[df:DF]->(),()-[corr:E_EN]->() return count(e),count(n),count(c),count(l),count(df),count(corr)
+
+def get_size(tx):
+    num_events, num_entity, num_log, num_class, num_df, num_corr, num_rel, num_total_nodes, num_total_relationships\
+        = 0, 0, 0, 0, 0, 0, 0, 0, 0
+    q = f'''match (e:Event) RETURN count(e)'''
+    for record in tx.run(q):
+        num_events = record["count(e)"]
+
+    q = f'''match (e:Entity) RETURN count(e)'''
+    for record in tx.run(q):
+        num_entity = record["count(e)"]
+
+    q = f'''match (l:Log) RETURN count(l)'''
+    for record in tx.run(q):
+        num_log = record["count(l)"]
+
+    q = f'''match (c:Class) RETURN count(c)'''
+    for record in tx.run(q):
+        num_class = record["count(c)"]
+
+    q = f'''match ()-[df:DF]->() RETURN count(df)'''
+    for record in tx.run(q):
+        num_df = record["count(df)"]
+
+    q = f'''match ()-[corr:E_EN]->() RETURN count(corr)'''
+    for record in tx.run(q):
+        num_corr = record["count(corr)"]
+
+    q = f'''match ()-[r:REL]->() RETURN count(r)'''
+    for record in tx.run(q):
+        num_rel = record["count(r)"]
+
+    q = f'''match (n) RETURN count(n)'''
+    for record in tx.run(q):
+        num_total_nodes = record["count(n)"]
+
+    q = f'''match ()-[r]->() RETURN count(r)'''
+    for record in tx.run(q):
+        num_total_relationships = record["count(r)"]
+
+    print(f'''Nodes (total);Event;Entity;Log;Class;Relationships (total);DF;CORR;REL''')
+    print(f'''{num_total_nodes};{num_events};{num_entity};{num_log};{num_class};{num_total_relationships};{num_df};
+    {num_corr};{num_rel}''')
+
+
+
+with driver.session() as session:
+    session.read_transaction(get_size)
```

### Comparing `promg-1.0.9/src/promg/utilities/performance_handling.py` & `promg-1.1.0/src/promg/utilities/performance_handling.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,113 @@
-import os
-import sys
-import time
-from datetime import datetime
-
-import pandas as pd
-from tqdm import tqdm
-
-from .singleton import Singleton
-from ..utilities.context_manager_tqdm import Nostdout
-from ..utilities.configuration import Configuration
-
-
-class Performance(metaclass=Singleton):
-    def __init__(self, perf_path: str = None, write_console=True):
-        self.start = time.time()
-        self.last = self.start
-        self.perf = pd.DataFrame(columns=["name", "start", "end", "duration"])
-        if perf_path is not None:
-            self.path = perf_path
-        self.count = 0
-        self.pbar = tqdm(file=sys.stdout)
-        self.status = "Waiting on request"
-        self.total = None
-        # start python trickery
-        self.write_console = write_console
-        if write_console:
-            self.ctx = Nostdout()
-            self.ctx.__enter__()
-
-    def string_time(self, epoch_time):
-        return datetime.utcfromtimestamp(epoch_time).strftime("%H:%M:%S")
-
-    def finished_step(self, log_message: str = None):
-        end = time.time()
-        if log_message is None:
-            self.perf = pd.concat([self.perf, pd.DataFrame.from_records([
-                {
-                    "name": log_message,
-                    "start": self.string_time(self.last),
-                    "end": self.string_time(end),
-                    "duration": (end - self.last)
-                }])])
-        self.pbar.set_description(f"{log_message}: took {round(end - self.last, 2)} seconds")
-        self.last = end
-        self.count += 1
-        self.pbar.update(1)
-
-    def track(argument: str = None):
-        def performance_tracker_wrapper(func):
-            def wrapper(self, *args, **kwargs):
-                result = func(self, *args, **kwargs)
-                end = time.time()
-                perf = Performance()
-                if argument is None or argument not in kwargs:
-                    log_message = func.__name__
-                else:
-                    log_message = f"{func.__name__} for {kwargs[argument]}"
-                perf.perf = pd.concat([perf.perf, pd.DataFrame.from_records([
-                    {
-                        "name": log_message,
-                        "start": perf.string_time(perf.last),
-                        "end": perf.string_time(end),
-                        "duration": (end - perf.last)
-                    }])])
-                perf.pbar.set_description(f"{log_message}: took {round(end - perf.last, 2)} seconds")
-                perf.status = f"{log_message}: took {round(end - perf.last, 2)} seconds"
-                perf.last = end
-                perf.count += 1
-                perf.pbar.update(1)
-                return result
-
-            return wrapper
-
-        return performance_tracker_wrapper
-
-    def finish(self):
-        end = time.time()
-        print(f"{self.count} steps")
-        self.perf = pd.concat([self.perf, pd.DataFrame.from_records([
-            {
-                "name": "total",
-                "start": self.string_time(self.start),
-                "end": self.string_time(end),
-                "duration": (end - self.start)
-            }])])
-        self.total = round(end - self.start, 2)
-        print(f"Total: took {round(end - self.start, 2)} seconds")
-        self.pbar.set_description(f"Completed")
-        self.pbar.close()
-        # close python trickery
-        if self.write_console:
-            self.ctx.__exit__()
-
-    def save(self):
-        if self.path is not None:
-            os.makedirs(os.path.dirname(self.path), exist_ok=True)
-            self.perf.to_csv(self.path, sep=";", decimal=",")
-
-    @staticmethod
-    def set_up_performance_with_path(path):
-        return Performance(perf_path=path)
-
-    @staticmethod
-    def set_up_performance(config: Configuration):
-        path = os.path.join("perf", f"{config.db_name}_{'sample_' * config.use_sample}Performance.csv")
-        return Performance.set_up_performance_with_path(path=path)
-
-    def finish_and_save(self):
-        self.finish()
-        self.save()
+import os
+import sys
+import time
+from datetime import datetime
+
+import pandas as pd
+from tqdm import tqdm
+
+from .singleton import Singleton
+from ..utilities.context_manager_tqdm import Nostdout
+from ..utilities.configuration import Configuration
+
+
+class Performance(metaclass=Singleton):
+    def __init__(self, perf_path: str = None, write_console=True):
+        self.start = time.time()
+        self.last = self.start
+        self.perf = pd.DataFrame(columns=["name", "start", "end", "duration"])
+        if perf_path is not None:
+            self.path = perf_path
+        else:
+            self.path = None
+        self.count = 0
+        self.pbar = tqdm(file=sys.stdout)
+        self.status = "Waiting on request"
+        self.total = None
+        # start python trickery
+        self.write_console = write_console
+        if write_console:
+            self.ctx = Nostdout()
+            self.ctx.__enter__()
+
+    def string_time(self, epoch_time):
+        return datetime.utcfromtimestamp(epoch_time).strftime("%H:%M:%S")
+
+    def finished_step(self, log_message: str = None):
+        end = time.time()
+        if log_message is None:
+            self.perf = pd.concat([self.perf, pd.DataFrame.from_records([
+                {
+                    "name": log_message,
+                    "start": self.string_time(self.last),
+                    "end": self.string_time(end),
+                    "duration": (end - self.last)
+                }])])
+        self.pbar.set_description(f"{log_message}: took {round(end - self.last, 2)} seconds")
+        self.last = end
+        self.count += 1
+        self.pbar.update(1)
+
+    def track(argument: str = None):
+        def performance_tracker_wrapper(func):
+            def wrapper(self, *args, **kwargs):
+                result = func(self, *args, **kwargs)
+                end = time.time()
+                perf = Performance()
+                if argument is None or argument not in kwargs:
+                    log_message = func.__name__
+                else:
+                    log_message = f"{func.__name__} for {kwargs[argument]}"
+                perf.perf = pd.concat([perf.perf, pd.DataFrame.from_records([
+                    {
+                        "name": log_message,
+                        "start": perf.string_time(perf.last),
+                        "end": perf.string_time(end),
+                        "duration": (end - perf.last)
+                    }])])
+                perf.pbar.set_description(f"{log_message}: took {round(end - perf.last, 2)} seconds")
+                perf.status = f"{log_message}: took {round(end - perf.last, 2)} seconds"
+                perf.last = end
+                perf.count += 1
+                perf.pbar.update(1)
+                return result
+
+            return wrapper
+
+        return performance_tracker_wrapper
+
+    def finish(self):
+        end = time.time()
+        print(f"{self.count} steps")
+        self.perf = pd.concat([self.perf, pd.DataFrame.from_records([
+            {
+                "name": "total",
+                "start": self.string_time(self.start),
+                "end": self.string_time(end),
+                "duration": (end - self.start)
+            }])])
+        self.total = round(end - self.start, 2)
+        print(f"Total: took {round(end - self.start, 2)} seconds")
+        self.pbar.set_description(f"Completed")
+        self.pbar.close()
+        # close python trickery
+        if self.write_console:
+            self.ctx.__exit__()
+
+    def save(self):
+        if self.path is not None:
+            os.makedirs(os.path.dirname(self.path), exist_ok=True)
+            self.perf.to_csv(self.path, sep=";", decimal=",")
+
+    @staticmethod
+    def set_up_performance_with_path(path):
+        return Performance(perf_path=path)
+
+    @staticmethod
+    def set_up_performance(config: Configuration):
+        path = os.path.join("perf", f"{config.db_name}_{'sample_' * config.use_sample}Performance.csv")
+        return Performance.set_up_performance_with_path(path=path)
+
+    def finish_and_save(self):
+        self.finish()
+        self.save()
```

### Comparing `promg-1.0.9/src/promg.egg-info/PKG-INFO` & `promg-1.1.0/src/promg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-Metadata-Version: 2.1
-Name: promg
-Version: 1.0.9
-Summary: Pyhton library to build Event Knowledge Graphs
-Author: A. Swevels, D.Fahland
-License: GPL 3.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: neo4j
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: tabulate
-Requires-Dist: tqdm
-Requires-Dist: pyyaml
-
-# Documentation
-
-## Hi there 👋
-
-Over here we are developing PromG, a tool enabling you to perform multi-dimensional process analytics by exploiting a multi-layered Event Knowledge Graph.
-The repository contains the source code (PromG-core) which can be installed as a Python package using `pip install promg` and several example analyses.
-
-🎥 Demo Video: We created a demo video [here](https://www.youtube.com/watch?v=EKXFqHtW3Xw&t=6s). In this demo, we illustrate PromG on the BPIC'17 dataset.
-
-🗃️ Documentation: [https://promg-dev.github.io/promg-core/](https://promg-dev.github.io/promg-core/)
-
-🏁 Getting started: [https://promg-dev.github.io/promg-core/getting-started/](https://promg-dev.github.io/promg-core/getting-started/)
-
-🛠️ Tutorial: [https://promg-dev.github.io/promg-core/tutorials](https://promg-dev.github.io/promg-core/tutorials/)
-
-📦 Python Package: [https://pypi.org/project/promg/](https://pypi.org/project/promg/)
+Metadata-Version: 2.1
+Name: promg
+Version: 1.1.0
+Summary: Pyhton library to build Event Knowledge Graphs
+Author: A. Swevels, D.Fahland
+License: GPL 3.0
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Documentation
+
+## Hi there 👋
+
+Over here we are developing PromG, a tool enabling you to perform multi-dimensional process analytics by exploiting a multi-layered Event Knowledge Graph.
+The repository contains the source code (PromG-core) which can be installed as a Python package using `pip install promg` and several example analyses.
+
+🎥 Demo Video: We created a demo video [here](https://www.youtube.com/watch?v=EKXFqHtW3Xw&t=6s). In this demo, we illustrate PromG on the BPIC'17 dataset.
+
+🗃️ Documentation: [https://promg-dev.github.io/promg-core/](https://promg-dev.github.io/promg-core/)
+
+🏁 Getting started: [https://promg-dev.github.io/promg-core/getting-started/](https://promg-dev.github.io/promg-core/getting-started/)
+
+🛠️ Tutorial: [https://promg-dev.github.io/promg-core/tutorials](https://promg-dev.github.io/promg-core/tutorials/)
+
+📦 Python Package: [https://pypi.org/project/promg/](https://pypi.org/project/promg/)
```

### Comparing `promg-1.0.9/src/promg.egg-info/SOURCES.txt` & `promg-1.1.0/src/promg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/promg/cypher_queries/exporter_ql.py
 src/promg/cypher_queries/inference_engine_ql.py
 src/promg/cypher_queries/process_discovery_ql.py
 src/promg/cypher_queries/semantic_header_ql.py
 src/promg/cypher_queries/task_identification_ql.py
 src/promg/data_managers/__init__.py
 src/promg/data_managers/datastructures.py
+src/promg/data_managers/properties.py
 src/promg/data_managers/semantic_header.py
 src/promg/database_managers/__init__.py
 src/promg/database_managers/authentication.py
 src/promg/database_managers/db_connection.py
 src/promg/database_managers/remote_authentication.py
 src/promg/facades/__init__.py
 src/promg/facades/oced_pg.py
@@ -34,8 +35,10 @@
 src/promg/modules/task_identification.py
 src/promg/utilities/__init__.py
 src/promg/utilities/auxiliary_functions.py
 src/promg/utilities/configuration.py
 src/promg/utilities/context_manager_tqdm.py
 src/promg/utilities/get_db_size.py
 src/promg/utilities/performance_handling.py
-src/promg/utilities/singleton.py
+src/promg/utilities/singleton.py
+src/promg/visualize_schema/__init__.py
+src/promg/visualize_schema/visualize.py
```

