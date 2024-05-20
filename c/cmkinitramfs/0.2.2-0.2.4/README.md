# Comparing `tmp/cmkinitramfs-0.2.2.tar.gz` & `tmp/cmkinitramfs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmkinitramfs-0.2.2.tar", last modified: Thu Dec  9 07:29:27 2021, max compression
+gzip compressed data, was "cmkinitramfs-0.2.4.tar", last modified: Mon May 20 22:34:21 2024, max compression
```

## Comparing `cmkinitramfs-0.2.2.tar` & `cmkinitramfs-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2021-12-09 07:29:27.400672 cmkinitramfs-0.2.2/
--rw-r--r--   0 yoshi     (1000) yoshi     (1001)     1069 2020-05-10 02:59:49.000000 cmkinitramfs-0.2.2/LICENSE.txt
--rw-r--r--   0 yoshi     (1000) yoshi     (1001)       95 2021-05-01 15:50:09.000000 cmkinitramfs-0.2.2/MANIFEST.in
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    18564 2021-12-09 07:29:27.400672 cmkinitramfs-0.2.2/PKG-INFO
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    17351 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.2/README.rst
-drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2021-12-09 07:29:27.396672 cmkinitramfs-0.2.2/cmkinitramfs/
--rw-r--r--   0 yoshi     (1000) yoshi     (1001)      357 2021-12-09 07:22:33.000000 cmkinitramfs-0.2.2/cmkinitramfs/__init__.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    19253 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.2/cmkinitramfs/bin.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    31564 2021-11-01 06:16:54.000000 cmkinitramfs-0.2.2/cmkinitramfs/data.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    24971 2021-10-31 17:55:33.000000 cmkinitramfs-0.2.2/cmkinitramfs/entry.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    17094 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.2/cmkinitramfs/init.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    18857 2021-12-09 06:55:33.000000 cmkinitramfs-0.2.2/cmkinitramfs/initramfs.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    12212 2021-05-01 15:36:42.000000 cmkinitramfs-0.2.2/cmkinitramfs/item.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)     1240 2021-05-06 04:35:00.000000 cmkinitramfs-0.2.2/cmkinitramfs/utils.py
-drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2021-12-09 07:29:27.397672 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/
--rw-r-----   0 yoshi     (1000) yoshi     (1001)    18564 2021-12-09 07:29:27.000000 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/PKG-INFO
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      701 2021-12-09 07:29:27.000000 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/SOURCES.txt
--rw-r-----   0 yoshi     (1000) yoshi     (1001)        1 2021-12-09 07:29:27.000000 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/dependency_links.txt
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      205 2021-12-09 07:29:27.000000 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/entry_points.txt
--rw-r-----   0 yoshi     (1000) yoshi     (1001)       64 2021-12-09 07:29:27.000000 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/requires.txt
--rw-r-----   0 yoshi     (1000) yoshi     (1001)       13 2021-12-09 07:29:27.000000 cmkinitramfs-0.2.2/cmkinitramfs.egg-info/top_level.txt
-drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2021-12-09 07:29:27.397672 cmkinitramfs-0.2.2/config/
--rw-r--r--   0 yoshi     (1000) yoshi     (1001)     1840 2021-05-08 05:38:50.000000 cmkinitramfs-0.2.2/config/cmkinitramfs.ini.example
-drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2021-12-09 07:29:27.398672 cmkinitramfs-0.2.2/doc/
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      638 2021-03-14 13:34:17.000000 cmkinitramfs-0.2.2/doc/Makefile
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      799 2021-03-14 13:34:17.000000 cmkinitramfs-0.2.2/doc/make.bat
-drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2021-12-09 07:29:27.400672 cmkinitramfs-0.2.2/doc/source/
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      739 2021-05-06 05:03:05.000000 cmkinitramfs-0.2.2/doc/source/bin.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)     2205 2021-03-15 14:19:47.000000 cmkinitramfs-0.2.2/doc/source/conf.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      921 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.2/doc/source/data.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      303 2021-04-30 06:01:21.000000 cmkinitramfs-0.2.2/doc/source/entry.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      388 2021-05-23 19:26:33.000000 cmkinitramfs-0.2.2/doc/source/index.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      488 2021-05-12 17:45:35.000000 cmkinitramfs-0.2.2/doc/source/init.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      568 2021-05-05 16:11:54.000000 cmkinitramfs-0.2.2/doc/source/initramfs.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      580 2021-04-29 19:15:54.000000 cmkinitramfs-0.2.2/doc/source/item.rst
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      164 2021-04-30 07:04:17.000000 cmkinitramfs-0.2.2/doc/source/utils.rst
--rw-r--r--   0 yoshi     (1000) yoshi     (1001)      285 2021-12-09 07:29:27.400672 cmkinitramfs-0.2.2/setup.cfg
--rw-r-----   0 yoshi     (1000) yoshi     (1001)     1937 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.2/setup.py
--rw-r-----   0 yoshi     (1000) yoshi     (1001)      263 2021-04-15 18:08:37.000000 cmkinitramfs-0.2.2/tox.ini
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.265017 cmkinitramfs-0.2.4/
+-rw-r--r--   0 yoshi     (1000) yoshi     (1001)     1069 2020-05-10 02:59:49.000000 cmkinitramfs-0.2.4/LICENSE.txt
+-rw-r--r--   0 yoshi     (1000) yoshi     (1001)       95 2021-05-01 15:50:09.000000 cmkinitramfs-0.2.4/MANIFEST.in
+-rw-r--r--   0 yoshi     (1000) yoshi     (1001)    20005 2024-05-20 22:34:21.265017 cmkinitramfs-0.2.4/PKG-INFO
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    18465 2024-05-20 22:30:23.000000 cmkinitramfs-0.2.4/README.rst
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.259017 cmkinitramfs-0.2.4/cmkinitramfs/
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      365 2024-05-20 22:30:23.000000 cmkinitramfs-0.2.4/cmkinitramfs/__init__.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    19253 2023-03-05 12:42:40.000000 cmkinitramfs-0.2.4/cmkinitramfs/bin.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    39531 2022-11-04 06:49:33.000000 cmkinitramfs-0.2.4/cmkinitramfs/data.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    25761 2022-10-09 08:59:15.000000 cmkinitramfs-0.2.4/cmkinitramfs/entry.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    17094 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.4/cmkinitramfs/init.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    18857 2021-12-09 06:55:33.000000 cmkinitramfs-0.2.4/cmkinitramfs/initramfs.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)    12196 2023-05-04 18:43:19.000000 cmkinitramfs-0.2.4/cmkinitramfs/item.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)     1240 2021-05-06 04:35:00.000000 cmkinitramfs-0.2.4/cmkinitramfs/utils.py
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.264016 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/
+-rw-r--r--   0 yoshi     (1000) yoshi     (1001)    20005 2024-05-20 22:34:21.000000 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/PKG-INFO
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      726 2024-05-20 22:34:21.000000 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/SOURCES.txt
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)        1 2024-05-20 22:34:21.000000 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/dependency_links.txt
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      204 2024-05-20 22:34:21.000000 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/entry_points.txt
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)       64 2024-05-20 22:34:21.000000 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/requires.txt
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)       13 2024-05-20 22:34:21.000000 cmkinitramfs-0.2.4/cmkinitramfs.egg-info/top_level.txt
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.261017 cmkinitramfs-0.2.4/config/
+-rw-r--r--   0 yoshi     (1000) yoshi     (1001)     1840 2021-05-08 05:38:50.000000 cmkinitramfs-0.2.4/config/cmkinitramfs.ini.example
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.261017 cmkinitramfs-0.2.4/doc/
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      638 2021-03-14 13:34:17.000000 cmkinitramfs-0.2.4/doc/Makefile
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      799 2021-03-14 13:34:17.000000 cmkinitramfs-0.2.4/doc/make.bat
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.264016 cmkinitramfs-0.2.4/doc/source/
+drwxr-x---   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:34:21.264016 cmkinitramfs-0.2.4/doc/source/_static/
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)        0 2024-05-20 22:11:53.000000 cmkinitramfs-0.2.4/doc/source/_static/.keep
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      739 2021-05-06 05:03:05.000000 cmkinitramfs-0.2.4/doc/source/bin.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)     2205 2021-03-15 14:19:47.000000 cmkinitramfs-0.2.4/doc/source/conf.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      921 2021-10-31 17:45:48.000000 cmkinitramfs-0.2.4/doc/source/data.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      303 2021-04-30 06:01:21.000000 cmkinitramfs-0.2.4/doc/source/entry.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      388 2021-05-23 19:26:33.000000 cmkinitramfs-0.2.4/doc/source/index.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      488 2021-05-12 17:45:35.000000 cmkinitramfs-0.2.4/doc/source/init.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      568 2021-05-05 16:11:54.000000 cmkinitramfs-0.2.4/doc/source/initramfs.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      580 2021-04-29 19:15:54.000000 cmkinitramfs-0.2.4/doc/source/item.rst
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      164 2021-04-30 07:04:17.000000 cmkinitramfs-0.2.4/doc/source/utils.rst
+-rw-r--r--   0 yoshi     (1000) yoshi     (1001)      285 2024-05-20 22:34:21.266017 cmkinitramfs-0.2.4/setup.cfg
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)     2038 2024-05-20 22:30:23.000000 cmkinitramfs-0.2.4/setup.py
+-rw-r-----   0 yoshi     (1000) yoshi     (1001)      263 2021-04-15 18:08:37.000000 cmkinitramfs-0.2.4/tox.ini
```

### Comparing `cmkinitramfs-0.2.2/LICENSE.txt` & `cmkinitramfs-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/PKG-INFO` & `cmkinitramfs-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: cmkinitramfs
-Version: 0.2.2
+Version: 0.2.4
 Summary: A customizable simple initramfs generator
-Home-page: https://github.com/teapot9/fand
+Home-page: https://github.com/teapot9/cmkinitramfs
 Author: Louis Leseur
 Author-email: louis.leseur@gmail.com
 License: MIT
 Keywords: initramfs,initramfs-generator
 Platform: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Boot
 Classifier: Topic :: System :: Boot :: Init
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: pyelftools
 Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: qa
-License-File: LICENSE.txt
+Requires-Dist: flake8; extra == "qa"
+Requires-Dist: mypy; extra == "qa"
+Requires-Dist: tox; extra == "qa"
 
 ============
 cmkinitramfs
 ============
 
 |github version badge|
 |pypi version badge|
@@ -379,14 +387,62 @@
  - ``pool`` (optional): Data identifier of the parent pool (defaults to same
    as pool name).
 
  - ``dataset`` (mandatory): Name of the dataset to unlock.
 
  - ``key`` (optional): Data identifier of a keyfile to use.
 
+Network sections
+----------------
+
+Configure a network interface.
+
+ - ``type = network`` (mandatory).
+
+ - |need|
+
+ - |load-need|
+
+ - ``device`` (mandatory): MAC address of the interface.
+
+ - ``ip`` (optional): IP address of the interface (DHCP if not set).
+
+ - ``mask`` (optional): IP mask (if static IP is defined).
+
+ - ``gateway`` (optional): default route IP (if static IP is defined).
+
+ISCSI sections
+--------------
+
+Configure an iSCSI device.
+
+ - ``type = iscsi``
+
+ - |need|
+
+ - |load-need|
+
+ - ``initiator`` (mandatory): Initiator name.
+
+ - ``target`` (mandatory): iSCSI target.
+
+ - ``portal_group`` (mandatory): target portal group tag.
+
+ - ``address`` (mandatory): iSCSI server address.
+
+ - ``port`` (mandatory): iSCSI server port.
+
+ - ``username`` (optional): authentification username.
+
+ - ``password`` (optional): authentification password.
+
+ - ``username_in`` (optional): incoming authentification username.
+
+ - ``password_in`` (optional): incoming authentification password.
+
 .. |need| replace:: ``need`` (optional): Hard dependencies: comma separated
    list of data identifiers. Those dependencies are required to load
    *and* use the data.
 
 .. |load-need| replace:: ``load-need`` (optional): Load dependencies: comma
    separated list of data identifiers. Those dependencies are only required
    to load the data, they can be unloaded when the data has been successfully
@@ -416,53 +472,54 @@
 cmkinit
 -------
 
 .. code-block:: console
 
    $ cmkinit --help
    usage: cmkinit [-h] [--version]
-
+   
    Build an init script
-
-   optional arguments:
+   
+   options:
      -h, --help  show this help message and exit
      --version   show program's version number and exit
 
 Running ``cmkinit`` will generate an init script and output it to stdout.
 No options are available, everything is defined in the configuration file.
 The ``CMKINITCFG`` environment variable may be defined to use a custom
 configuration file.
 
 cmkcpiodir
 ----------
 
 .. code-block:: console
 
    $ cmkcpiodir --help
-   usage: cmkcpiodir [-h] [--version] [--debug] [--verbose] [--quiet]
+   usage: cmkcpiodir [-h] [--verbose] [--quiet] [--version] [--debug]
                      [--output OUTPUT] [--binroot BINROOT] [--kernel KERNEL]
-                     [--only-build-archive | --only-build-directory] [--keep]
-                     [--clean] [--build-dir BUILD_DIR]
-
+                     [--no-kmod] [--only-build-archive | --only-build-directory]
+                     [--keep] [--clean] [--build-dir BUILD_DIR]
+   
    Build an initramfs using a directory.
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
-     --version             show program's version number and exit
-     --debug, -d           debugging mode: non-root, implies -k
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
+     --version             show program's version number and exit
+     --debug, -d           debugging mode: non-root, implies -k
      --output OUTPUT, -o OUTPUT
                            set the output of the CPIO archive
      --binroot BINROOT, -r BINROOT
                            set the root directory for binaries (executables and
                            libraries)
      --kernel KERNEL, -K KERNEL
-                           set the target kernel version of the initramfs,
+                           set the target kernel versions of the initramfs,
                            defaults to the running kernel
+     --no-kmod             disable kernel modules support
      --only-build-archive, -c
                            only build the CPIO archive from an existing initramfs
                            directory
      --only-build-directory, -D
                            only build the initramfs directory, implies -k
      --keep, -k            keep the created initramfs directory
      --clean, -C           overwrite temporary directory if it exists, use
@@ -478,35 +535,36 @@
 
 cmkcpiolist
 -----------
 
 .. code-block:: console
 
    $ cmkcpiolist --help
-   usage: cmkcpiolist [-h] [--version] [--debug] [--verbose] [--quiet]
+   usage: cmkcpiolist [-h] [--verbose] [--quiet] [--version] [--debug]
                       [--output OUTPUT] [--binroot BINROOT] [--kernel KERNEL]
-                      [--only-build-archive | --only-build-list] [--keep]
-                      [--cpio-list CPIO_LIST]
-
+                      [--no-kmod] [--only-build-archive | --only-build-list]
+                      [--keep] [--cpio-list CPIO_LIST]
+   
    Build an initramfs using a CPIO list
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
-     --version             show program's version number and exit
-     --debug, -d           debugging mode: non-root, implies -k
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
+     --version             show program's version number and exit
+     --debug, -d           debugging mode: non-root, implies -k
      --output OUTPUT, -o OUTPUT
                            set the output of the CPIO archive
      --binroot BINROOT, -r BINROOT
                            set the root directory for binaries (executables and
                            libraries)
      --kernel KERNEL, -K KERNEL
-                           set the target kernel version of the initramfs,
+                           set the target kernel versions of the initramfs,
                            defaults to the running kernel
+     --no-kmod             disable kernel modules support
      --only-build-archive, -c
                            only build the CPIO archive from an existing CPIO list
      --only-build-list, -L
                            only build the CPIO list, implies -k
      --keep, -k            keep the created CPIO list
      --cpio-list CPIO_LIST, -l CPIO_LIST
                            set the location of the CPIO list
@@ -520,21 +578,21 @@
 
 .. code-block:: console
 
    $ findlib --help
    usage: findlib [-h] [--verbose] [--quiet] [--version]
                   [--compatible COMPATIBLE] [--root ROOT] [--null] [--glob]
                   LIB [LIB ...]
-
+   
    Find a library on the system
-
+   
    positional arguments:
      LIB                   library to search
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
      --version             show program's version number and exit
      --compatible COMPATIBLE, -c COMPATIBLE
                            set a binary the library must be compatible with
      --root ROOT, -r ROOT  set the root directory to search for the library
@@ -600,9 +658,7 @@
    /lib64/libgcc_s.so.1
 
 ..
 
  - Search any library matching ``libgcc_s.*`` on the system and prints them
    to stdout.
 
-
-
```

### Comparing `cmkinitramfs-0.2.2/README.rst` & `cmkinitramfs-0.2.4/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -346,14 +346,62 @@
  - ``pool`` (optional): Data identifier of the parent pool (defaults to same
    as pool name).
 
  - ``dataset`` (mandatory): Name of the dataset to unlock.
 
  - ``key`` (optional): Data identifier of a keyfile to use.
 
+Network sections
+----------------
+
+Configure a network interface.
+
+ - ``type = network`` (mandatory).
+
+ - |need|
+
+ - |load-need|
+
+ - ``device`` (mandatory): MAC address of the interface.
+
+ - ``ip`` (optional): IP address of the interface (DHCP if not set).
+
+ - ``mask`` (optional): IP mask (if static IP is defined).
+
+ - ``gateway`` (optional): default route IP (if static IP is defined).
+
+ISCSI sections
+--------------
+
+Configure an iSCSI device.
+
+ - ``type = iscsi``
+
+ - |need|
+
+ - |load-need|
+
+ - ``initiator`` (mandatory): Initiator name.
+
+ - ``target`` (mandatory): iSCSI target.
+
+ - ``portal_group`` (mandatory): target portal group tag.
+
+ - ``address`` (mandatory): iSCSI server address.
+
+ - ``port`` (mandatory): iSCSI server port.
+
+ - ``username`` (optional): authentification username.
+
+ - ``password`` (optional): authentification password.
+
+ - ``username_in`` (optional): incoming authentification username.
+
+ - ``password_in`` (optional): incoming authentification password.
+
 .. |need| replace:: ``need`` (optional): Hard dependencies: comma separated
    list of data identifiers. Those dependencies are required to load
    *and* use the data.
 
 .. |load-need| replace:: ``load-need`` (optional): Load dependencies: comma
    separated list of data identifiers. Those dependencies are only required
    to load the data, they can be unloaded when the data has been successfully
@@ -383,53 +431,54 @@
 cmkinit
 -------
 
 .. code-block:: console
 
    $ cmkinit --help
    usage: cmkinit [-h] [--version]
-
+   
    Build an init script
-
-   optional arguments:
+   
+   options:
      -h, --help  show this help message and exit
      --version   show program's version number and exit
 
 Running ``cmkinit`` will generate an init script and output it to stdout.
 No options are available, everything is defined in the configuration file.
 The ``CMKINITCFG`` environment variable may be defined to use a custom
 configuration file.
 
 cmkcpiodir
 ----------
 
 .. code-block:: console
 
    $ cmkcpiodir --help
-   usage: cmkcpiodir [-h] [--version] [--debug] [--verbose] [--quiet]
+   usage: cmkcpiodir [-h] [--verbose] [--quiet] [--version] [--debug]
                      [--output OUTPUT] [--binroot BINROOT] [--kernel KERNEL]
-                     [--only-build-archive | --only-build-directory] [--keep]
-                     [--clean] [--build-dir BUILD_DIR]
-
+                     [--no-kmod] [--only-build-archive | --only-build-directory]
+                     [--keep] [--clean] [--build-dir BUILD_DIR]
+   
    Build an initramfs using a directory.
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
-     --version             show program's version number and exit
-     --debug, -d           debugging mode: non-root, implies -k
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
+     --version             show program's version number and exit
+     --debug, -d           debugging mode: non-root, implies -k
      --output OUTPUT, -o OUTPUT
                            set the output of the CPIO archive
      --binroot BINROOT, -r BINROOT
                            set the root directory for binaries (executables and
                            libraries)
      --kernel KERNEL, -K KERNEL
-                           set the target kernel version of the initramfs,
+                           set the target kernel versions of the initramfs,
                            defaults to the running kernel
+     --no-kmod             disable kernel modules support
      --only-build-archive, -c
                            only build the CPIO archive from an existing initramfs
                            directory
      --only-build-directory, -D
                            only build the initramfs directory, implies -k
      --keep, -k            keep the created initramfs directory
      --clean, -C           overwrite temporary directory if it exists, use
@@ -445,35 +494,36 @@
 
 cmkcpiolist
 -----------
 
 .. code-block:: console
 
    $ cmkcpiolist --help
-   usage: cmkcpiolist [-h] [--version] [--debug] [--verbose] [--quiet]
+   usage: cmkcpiolist [-h] [--verbose] [--quiet] [--version] [--debug]
                       [--output OUTPUT] [--binroot BINROOT] [--kernel KERNEL]
-                      [--only-build-archive | --only-build-list] [--keep]
-                      [--cpio-list CPIO_LIST]
-
+                      [--no-kmod] [--only-build-archive | --only-build-list]
+                      [--keep] [--cpio-list CPIO_LIST]
+   
    Build an initramfs using a CPIO list
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
-     --version             show program's version number and exit
-     --debug, -d           debugging mode: non-root, implies -k
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
+     --version             show program's version number and exit
+     --debug, -d           debugging mode: non-root, implies -k
      --output OUTPUT, -o OUTPUT
                            set the output of the CPIO archive
      --binroot BINROOT, -r BINROOT
                            set the root directory for binaries (executables and
                            libraries)
      --kernel KERNEL, -K KERNEL
-                           set the target kernel version of the initramfs,
+                           set the target kernel versions of the initramfs,
                            defaults to the running kernel
+     --no-kmod             disable kernel modules support
      --only-build-archive, -c
                            only build the CPIO archive from an existing CPIO list
      --only-build-list, -L
                            only build the CPIO list, implies -k
      --keep, -k            keep the created CPIO list
      --cpio-list CPIO_LIST, -l CPIO_LIST
                            set the location of the CPIO list
@@ -487,21 +537,21 @@
 
 .. code-block:: console
 
    $ findlib --help
    usage: findlib [-h] [--verbose] [--quiet] [--version]
                   [--compatible COMPATIBLE] [--root ROOT] [--null] [--glob]
                   LIB [LIB ...]
-
+   
    Find a library on the system
-
+   
    positional arguments:
      LIB                   library to search
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
      --version             show program's version number and exit
      --compatible COMPATIBLE, -c COMPATIBLE
                            set a binary the library must be compatible with
      --root ROOT, -r ROOT  set the root directory to search for the library
```

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/bin.py` & `cmkinitramfs-0.2.4/cmkinitramfs/bin.py`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/data.py` & `cmkinitramfs-0.2.4/cmkinitramfs/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -899,7 +899,247 @@
             quote(f'Failed to lock {self}'), '\n',
             '\n',
         ))
         self._post_unload(out)
 
     def path(self) -> str:
         return quote(self.dataset)
+
+
+class Network(Data):
+    """Networking configuration
+
+    :param device: MAC address of the device
+    :param ip: IP address (None for DHCP)
+    :param mask: IP mask (defaults to classful or DHCP)
+    :param gateway: default route IP (optional)
+    """
+    device: str
+    ip: Optional[str]
+    mask: Optional[str]
+    gateway: Optional[str]
+
+    @staticmethod
+    def classful_mask(ip: str) -> str:
+        first = int(ip.split('.')[0])
+        if first < 128:
+            return '255.0.0.0'
+        elif first < 192:
+            return '255.255.0.0'
+        elif first < 224:
+            return '255.255.255.0'
+        else:
+            raise ValueError(f"No classful network mask for {ip}")
+
+    @staticmethod
+    def __fun_find_iface(out: IO[str]) -> None:
+        """"Define the ``find_iface`` function
+
+        This function takes one MAC address and outputs the corresponding
+        network interface name (e.g. ``eth0``).
+
+        Return value: 0 on success, 1 on failure.
+        """
+
+        out.writelines((
+            'find_iface()\n',
+            '{\n',
+            '\tfor k in /sys/class/net/*; do\n',
+            '\t\tif ! grep -q "${1}" "${k}/address" 1>/dev/null 2>&1; ',
+            'then continue; fi\n',
+            '\t\techo "$(basename -- "${k}")"\n',
+            '\t\treturn 0\n',
+            '\tdone\n',
+            '\treturn 1\n'
+            '}\n',
+            '\n',
+        ))
+
+    @classmethod
+    def initialize(cls, out: IO[str]) -> None:
+        super().initialize(out)
+        Network.__fun_find_iface(out)
+
+    def __init__(
+        self, device: str, ip: Optional[str] = None,
+        mask: Optional[str] = None, gateway: Optional[str] = None
+    ):
+        super().__init__()
+
+        self.device = device
+        if mask is None and ip is not None:
+            mask = Network.classful_mask(ip)
+        self.ip = ip
+        self.mask = mask
+        self.gateway = gateway
+
+        self.busybox |= {'ip', 'udhcpc'}
+        self.files |= {
+            ('/usr/share/udhcpc/default.script', '/etc/udhcpc.script'),
+        }
+
+    def __str__(self) -> str:
+        return f'network interface {self.device}'
+
+    def __eq__(self, other: object) -> bool:
+        return isinstance(other, type(self)) and super().__eq__(other) \
+            and self.ip == other.ip and self.mask == other.mask \
+            and self.gateway == other.gateway and self.device == other.device
+
+    def load(self, out: IO[str]) -> None:
+        device = quote(self.device)
+        ip = quote(self.ip if self.ip is not None else '')
+        mask = quote(self.mask if self.mask is not None else '')
+        gateway = quote(self.gateway if self.gateway is not None else '')
+        iface = '"${iface}"'
+        iface_full = quote(f'{self.device} (') + iface + quote(')')
+
+        static_ip = (
+            f'ip addr add {ip}/{mask} dev {iface} || die ',
+            quote(f'Failed to add {self.ip} to '), iface_full, '\n',
+        )
+        dhcp_ip = (
+            f'udhcpc -nqfS -s /etc/udhcpc.script -i {iface} || die ',
+            quote('DHCP failed on '), iface_full, '\n',
+        )
+        gw_route = (
+            f'ip route add default via {gateway} dev {iface} || die ',
+            quote(f'Failed to set gateway {self.gateway} on '),
+            iface_full, '\n',
+        )
+
+        self._pre_load(out)
+        out.writelines((
+            'info ', quote(f'Raising {self}'), '\n',
+            f'iface="$(find_iface {device})" || die ',
+            quote(f'Failed to find network interface {self.device}'), '\n',
+            f'ip link set {iface} up || die ',
+            quote('Failed to raise network interface '), iface_full, '\n',
+            *(static_ip if self.ip is not None else dhcp_ip),
+            *(gw_route if self.gateway is not None else ()),
+            '\n',
+        ))
+        self._post_load(out)
+
+    def unload(self, out: IO[str]) -> None:
+        device = quote(self.device)
+        iface = '"${iface}"'
+        iface_full = quote(f'{self.device} (') + iface + quote(')')
+
+        self._pre_unload(out)
+        out.writelines((
+            'info ', quote(f'Shutting down {self}'), '\n',
+            f'iface="$(find_iface {device})" || die ',
+            quote(f'Failed to find network interface {self.device}'), '\n',
+            f'ip link set {iface} down || die ',
+            quote('Failed to shutdown network interface '), iface_full, '\n',
+            '\n',
+        ))
+        self._post_unload(out)
+
+
+class ISCSI(Data):
+    """iSCSI target
+
+    :param initiator: Initiator name
+    :param target: iSCSI target
+    :param portal_group: Target portal group tag
+    :param address: iSCSI server address
+    :param port: iSCSI server port
+    :param username: Authentication username
+    :param password: Authentication password
+    :param username_in: Incoming authentication username
+    :param password_in: Incoming authentication password
+    """
+    initiator: str
+    target: str
+    portal_group: int
+    address: str
+    port: int
+    username: Optional[str]
+    password: Optional[str]
+    username_in: Optional[str]
+    password_in: Optional[str]
+
+    def __init__(
+        self,
+        initiator: str,
+        target: str,
+        portal_group: int,
+        address: str,
+        port: int = 3260,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        username_in: Optional[str] = None,
+        password_in: Optional[str] = None,
+    ):
+        super().__init__()
+
+        self.initiator = initiator
+        self.target = target
+        self.portal_group = portal_group
+        self.address = address
+        self.port = port
+        self.username = username
+        self.password = password
+        self.username_in = username_in
+        self.password_in = password_in
+
+        if (self.username is None) != (self.password is None):
+            raise ValueError("Both username and password must be set")
+        if (self.username_in is None) != (self.password_in is None):
+            raise ValueError("Both username_in and password_in must be set")
+
+        self.execs |= {('iscsistart', None)}
+
+    def __str__(self) -> str:
+        return f'iSCSI target {self.target}'
+
+    def __eq__(self, other: object) -> bool:
+        return isinstance(other, type(self)) and super().__eq__(other) \
+            and self.initiator == other.initiator \
+            and self.target == other.target \
+            and self.portal_group == other.portal_group \
+            and self.address == other.address \
+            and self.port == other.port \
+            and self.username == other.username \
+            and self.password == other.password \
+            and self.username_in == other.username_in \
+            and self.password_in == other.password_in
+
+    def load(self, out: IO[str]) -> None:
+        auth = (
+            ' -u ', quote(
+                self.username if self.username is not None else ''
+            ),
+            ' -w ', quote(
+                self.password if self.password is not None else ''
+            ),
+        )
+        auth_in = (
+            ' -U ', quote(
+                self.username_in if self.username_in is not None else ''
+            ),
+            ' -W ', quote(
+                self.password_in if self.password_in is not None else ''
+            ),
+        )
+
+        self._pre_load(out)
+        out.writelines((
+            'info ', quote(f'Loading {self}'), '\n',
+            'iscsistart',
+            ' -i ', quote(self.initiator),
+            ' -t ', quote(self.target),
+            ' -g ', str(self.portal_group),
+            ' -a ', quote(self.address),
+            ' -p ', str(self.port),
+            *(auth if self.username is not None else ()),
+            *(auth_in if self.username_in is not None else ()),
+            ' || die ', quote(f'Failed to load {self}'), '\n',
+            '\n',
+        ))
+        self._post_load(out)
+
+    def unload(self, out: IO[str]) -> None:
+        self._pre_unload(out)
+        self._post_unload(out)
```

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/entry.py` & `cmkinitramfs-0.2.4/cmkinitramfs/entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,14 +174,33 @@
             data_dic[data_id] = datamod.ZFSCryptData(
                 find_data(data_config.get(
                     'pool', data_config['dataset'].split('/')[0]
                 )),
                 data_config['dataset'],
                 find_data(data_config.get('key'))
             )
+        elif data_config['type'] == 'network':
+            data_dic[data_id] = datamod.Network(
+                data_config['device'],
+                data_config.get('ip'),
+                data_config.get('mask'),
+                data_config.get('gateway'),
+            )
+        elif data_config['type'] == 'iscsi':
+            data_dic[data_id] = datamod.ISCSI(
+                data_config['initiator'],
+                data_config['target'],
+                int(data_config['portal-group']),
+                data_config['address'],
+                int(data_config.get('port', '3260')),
+                data_config.get('username'),
+                data_config.get('password'),
+                data_config.get('username-in'),
+                data_config.get('password-in'),
+            )
         else:
             raise Exception(f"Unknown config type {data_config['type']}")
 
     # Configure dependencies
     for data_id, data in data_dic.items():
         if data_id not in config.sections():
             continue
```

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/init.py` & `cmkinitramfs-0.2.4/cmkinitramfs/init.py`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/initramfs.py` & `cmkinitramfs-0.2.4/cmkinitramfs/initramfs.py`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/item.py` & `cmkinitramfs-0.2.4/cmkinitramfs/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 logger = logging.getLogger(__name__)
 
 
 class MergeError(Exception):
     """Cannot merge an Item into another"""
 
 
-@dataclass  # type: ignore
+@dataclass
 class Item(ABC):
     """An object within the initramfs"""
 
     def is_mergeable(self, other: Item) -> bool:
         """Check if two items can be merged together
 
         By default, two items can only be merged if they are equal.
```

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs/utils.py` & `cmkinitramfs-0.2.4/cmkinitramfs/utils.py`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs.egg-info/PKG-INFO` & `cmkinitramfs-0.2.4/cmkinitramfs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: cmkinitramfs
-Version: 0.2.2
+Version: 0.2.4
 Summary: A customizable simple initramfs generator
-Home-page: https://github.com/teapot9/fand
+Home-page: https://github.com/teapot9/cmkinitramfs
 Author: Louis Leseur
 Author-email: louis.leseur@gmail.com
 License: MIT
 Keywords: initramfs,initramfs-generator
 Platform: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Boot
 Classifier: Topic :: System :: Boot :: Init
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: pyelftools
 Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: qa
-License-File: LICENSE.txt
+Requires-Dist: flake8; extra == "qa"
+Requires-Dist: mypy; extra == "qa"
+Requires-Dist: tox; extra == "qa"
 
 ============
 cmkinitramfs
 ============
 
 |github version badge|
 |pypi version badge|
@@ -379,14 +387,62 @@
  - ``pool`` (optional): Data identifier of the parent pool (defaults to same
    as pool name).
 
  - ``dataset`` (mandatory): Name of the dataset to unlock.
 
  - ``key`` (optional): Data identifier of a keyfile to use.
 
+Network sections
+----------------
+
+Configure a network interface.
+
+ - ``type = network`` (mandatory).
+
+ - |need|
+
+ - |load-need|
+
+ - ``device`` (mandatory): MAC address of the interface.
+
+ - ``ip`` (optional): IP address of the interface (DHCP if not set).
+
+ - ``mask`` (optional): IP mask (if static IP is defined).
+
+ - ``gateway`` (optional): default route IP (if static IP is defined).
+
+ISCSI sections
+--------------
+
+Configure an iSCSI device.
+
+ - ``type = iscsi``
+
+ - |need|
+
+ - |load-need|
+
+ - ``initiator`` (mandatory): Initiator name.
+
+ - ``target`` (mandatory): iSCSI target.
+
+ - ``portal_group`` (mandatory): target portal group tag.
+
+ - ``address`` (mandatory): iSCSI server address.
+
+ - ``port`` (mandatory): iSCSI server port.
+
+ - ``username`` (optional): authentification username.
+
+ - ``password`` (optional): authentification password.
+
+ - ``username_in`` (optional): incoming authentification username.
+
+ - ``password_in`` (optional): incoming authentification password.
+
 .. |need| replace:: ``need`` (optional): Hard dependencies: comma separated
    list of data identifiers. Those dependencies are required to load
    *and* use the data.
 
 .. |load-need| replace:: ``load-need`` (optional): Load dependencies: comma
    separated list of data identifiers. Those dependencies are only required
    to load the data, they can be unloaded when the data has been successfully
@@ -416,53 +472,54 @@
 cmkinit
 -------
 
 .. code-block:: console
 
    $ cmkinit --help
    usage: cmkinit [-h] [--version]
-
+   
    Build an init script
-
-   optional arguments:
+   
+   options:
      -h, --help  show this help message and exit
      --version   show program's version number and exit
 
 Running ``cmkinit`` will generate an init script and output it to stdout.
 No options are available, everything is defined in the configuration file.
 The ``CMKINITCFG`` environment variable may be defined to use a custom
 configuration file.
 
 cmkcpiodir
 ----------
 
 .. code-block:: console
 
    $ cmkcpiodir --help
-   usage: cmkcpiodir [-h] [--version] [--debug] [--verbose] [--quiet]
+   usage: cmkcpiodir [-h] [--verbose] [--quiet] [--version] [--debug]
                      [--output OUTPUT] [--binroot BINROOT] [--kernel KERNEL]
-                     [--only-build-archive | --only-build-directory] [--keep]
-                     [--clean] [--build-dir BUILD_DIR]
-
+                     [--no-kmod] [--only-build-archive | --only-build-directory]
+                     [--keep] [--clean] [--build-dir BUILD_DIR]
+   
    Build an initramfs using a directory.
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
-     --version             show program's version number and exit
-     --debug, -d           debugging mode: non-root, implies -k
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
+     --version             show program's version number and exit
+     --debug, -d           debugging mode: non-root, implies -k
      --output OUTPUT, -o OUTPUT
                            set the output of the CPIO archive
      --binroot BINROOT, -r BINROOT
                            set the root directory for binaries (executables and
                            libraries)
      --kernel KERNEL, -K KERNEL
-                           set the target kernel version of the initramfs,
+                           set the target kernel versions of the initramfs,
                            defaults to the running kernel
+     --no-kmod             disable kernel modules support
      --only-build-archive, -c
                            only build the CPIO archive from an existing initramfs
                            directory
      --only-build-directory, -D
                            only build the initramfs directory, implies -k
      --keep, -k            keep the created initramfs directory
      --clean, -C           overwrite temporary directory if it exists, use
@@ -478,35 +535,36 @@
 
 cmkcpiolist
 -----------
 
 .. code-block:: console
 
    $ cmkcpiolist --help
-   usage: cmkcpiolist [-h] [--version] [--debug] [--verbose] [--quiet]
+   usage: cmkcpiolist [-h] [--verbose] [--quiet] [--version] [--debug]
                       [--output OUTPUT] [--binroot BINROOT] [--kernel KERNEL]
-                      [--only-build-archive | --only-build-list] [--keep]
-                      [--cpio-list CPIO_LIST]
-
+                      [--no-kmod] [--only-build-archive | --only-build-list]
+                      [--keep] [--cpio-list CPIO_LIST]
+   
    Build an initramfs using a CPIO list
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
-     --version             show program's version number and exit
-     --debug, -d           debugging mode: non-root, implies -k
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
+     --version             show program's version number and exit
+     --debug, -d           debugging mode: non-root, implies -k
      --output OUTPUT, -o OUTPUT
                            set the output of the CPIO archive
      --binroot BINROOT, -r BINROOT
                            set the root directory for binaries (executables and
                            libraries)
      --kernel KERNEL, -K KERNEL
-                           set the target kernel version of the initramfs,
+                           set the target kernel versions of the initramfs,
                            defaults to the running kernel
+     --no-kmod             disable kernel modules support
      --only-build-archive, -c
                            only build the CPIO archive from an existing CPIO list
      --only-build-list, -L
                            only build the CPIO list, implies -k
      --keep, -k            keep the created CPIO list
      --cpio-list CPIO_LIST, -l CPIO_LIST
                            set the location of the CPIO list
@@ -520,21 +578,21 @@
 
 .. code-block:: console
 
    $ findlib --help
    usage: findlib [-h] [--verbose] [--quiet] [--version]
                   [--compatible COMPATIBLE] [--root ROOT] [--null] [--glob]
                   LIB [LIB ...]
-
+   
    Find a library on the system
-
+   
    positional arguments:
      LIB                   library to search
-
-   optional arguments:
+   
+   options:
      -h, --help            show this help message and exit
      --verbose, -v         be verbose
      --quiet, -q           be quiet (can be repeated)
      --version             show program's version number and exit
      --compatible COMPATIBLE, -c COMPATIBLE
                            set a binary the library must be compatible with
      --root ROOT, -r ROOT  set the root directory to search for the library
@@ -600,9 +658,7 @@
    /lib64/libgcc_s.so.1
 
 ..
 
  - Search any library matching ``libgcc_s.*`` on the system and prints them
    to stdout.
 
-
-
```

### Comparing `cmkinitramfs-0.2.2/cmkinitramfs.egg-info/SOURCES.txt` & `cmkinitramfs-0.2.4/cmkinitramfs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 doc/source/conf.py
 doc/source/data.rst
 doc/source/entry.rst
 doc/source/index.rst
 doc/source/init.rst
 doc/source/initramfs.rst
 doc/source/item.rst
-doc/source/utils.rst
+doc/source/utils.rst
+doc/source/_static/.keep
```

### Comparing `cmkinitramfs-0.2.2/config/cmkinitramfs.ini.example` & `cmkinitramfs-0.2.4/config/cmkinitramfs.ini.example`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/Makefile` & `cmkinitramfs-0.2.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/make.bat` & `cmkinitramfs-0.2.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/source/bin.rst` & `cmkinitramfs-0.2.4/doc/source/bin.rst`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/source/conf.py` & `cmkinitramfs-0.2.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/source/data.rst` & `cmkinitramfs-0.2.4/doc/source/data.rst`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/source/initramfs.rst` & `cmkinitramfs-0.2.4/doc/source/initramfs.rst`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/doc/source/item.rst` & `cmkinitramfs-0.2.4/doc/source/item.rst`

 * *Files identical despite different names*

### Comparing `cmkinitramfs-0.2.2/setup.py` & `cmkinitramfs-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,20 @@
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: System :: Boot",
         "Topic :: System :: Boot :: Init",
         "Topic :: Utilities",
         "Typing :: Typed",
     ],
```

