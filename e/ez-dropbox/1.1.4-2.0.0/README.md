# Comparing `tmp/ez-dropbox-1.1.4.tar.gz` & `tmp/ez-dropbox-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-dropbox-1.1.4.tar", last modified: Mon Oct 10 07:02:56 2022, max compression
+gzip compressed data, was "ez-dropbox-2.0.0.tar", last modified: Tue May 21 18:28:54 2024, max compression
```

## Comparing `ez-dropbox-1.1.4.tar` & `ez-dropbox-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-10-10 07:02:56.119403 ez-dropbox-1.1.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2022-10-03 01:40:27.000000 ez-dropbox-1.1.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3197 2022-10-10 07:02:56.119403 ez-dropbox-1.1.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2935 2022-10-03 01:40:27.000000 ez-dropbox-1.1.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-10-10 07:02:56.119403 ez-dropbox-1.1.4/ez_dropbox.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3197 2022-10-10 07:02:56.000000 ez-dropbox-1.1.4/ez_dropbox.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      227 2022-10-10 07:02:56.000000 ez-dropbox-1.1.4/ez_dropbox.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-10-10 07:02:56.000000 ez-dropbox-1.1.4/ez_dropbox.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2022-10-10 07:02:56.000000 ez-dropbox-1.1.4/ez_dropbox.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2022-10-10 07:02:56.000000 ez-dropbox-1.1.4/ez_dropbox.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-10-10 07:02:56.119403 ez-dropbox-1.1.4/ezdbx/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      117 2022-10-10 06:59:17.000000 ez-dropbox-1.1.4/ezdbx/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12440 2022-10-10 07:02:38.000000 ez-dropbox-1.1.4/ezdbx/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2022-10-10 07:02:56.119403 ez-dropbox-1.1.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      888 2022-10-10 07:02:52.000000 ez-dropbox-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:28:54.306918 ez-dropbox-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-05-21 18:28:54.306656 ez-dropbox-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-05-12 12:48:02.000000 ez-dropbox-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:28:54.304244 ez-dropbox-2.0.0/ez_dropbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 18:28:54.000000 ez-dropbox-2.0.0/ez_dropbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:28:54.305806 ez-dropbox-2.0.0/ezdbx/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.0/ezdbx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18948 2024-05-21 18:25:05.000000 ez-dropbox-2.0.0/ezdbx/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 18:28:54.307118 ez-dropbox-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-15 10:09:33.000000 ez-dropbox-2.0.0/setup.py
```

### Comparing `ez-dropbox-1.1.4/LICENSE` & `ez-dropbox-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-dropbox-1.1.4/PKG-INFO` & `ez-dropbox-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 1.1.4
+Version: 2.0.0
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-1.1.4/README.md` & `ez-dropbox-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ez-dropbox-1.1.4/ez_dropbox.egg-info/PKG-INFO` & `ez-dropbox-2.0.0/ez_dropbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 1.1.4
+Version: 2.0.0
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-1.1.4/setup.py` & `ez-dropbox-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 packages = [
     'ezdbx'
 ]
 
 setup(
     name='ez-dropbox',
-    version='1.1.4',
+    version='2.0.0',
     license="MIT License",
     description="You can easily operate Dropbox!",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TorDataScientist',
     url='https://github.com/TorDataScientist/ez-dropbox',
     packages=packages,
```

