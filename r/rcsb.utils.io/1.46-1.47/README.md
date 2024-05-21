# Comparing `tmp/rcsb.utils.io-1.46.tar.gz` & `tmp/rcsb_utils_io-1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.io-1.46.tar", last modified: Wed Jan 17 16:21:39 2024, max compression
+gzip compressed data, was "rcsb_utils_io-1.47.tar", last modified: Tue May 21 16:39:04 2024, max compression
```

## Comparing `rcsb.utils.io-1.46.tar` & `rcsb_utils_io-1.47.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-17 16:21:39.184005 rcsb.utils.io-1.46/
--rw-r--r--   0 vsts      (1001) docker     (127)     9634 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     5382 2024-01-17 16:21:39.184005 rcsb.utils.io-1.46/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3950 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-17 16:21:39.176005 rcsb.utils.io-1.46/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-17 16:21:39.176005 rcsb.utils.io-1.46/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-17 16:21:39.180004 rcsb.utils.io-1.46/rcsb/utils/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     1828 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/CacheUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6185 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/CryptUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4635 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/ExecUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12022 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/FastaUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5604 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/FileLock.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25377 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/FileUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12683 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/FtpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6281 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/GitUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/HashableDict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6761 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/IndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36552 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/IoUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4113 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/LogUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7429 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/MarshalUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5113 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/ProcessStatusUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6260 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/SftpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/SingletonClass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/SplitJoin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12245 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/StashUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11807 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/StashableBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3145 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14760 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/UrlRequestUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4495 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/rcsb/utils/io/decorators.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-17 16:21:39.180004 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5382 2024-01-17 16:21:39.000000 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      975 2024-01-17 16:21:39.000000 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-17 16:21:39.000000 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-17 16:17:08.000000 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-01-17 16:21:39.000000 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-01-17 16:21:39.000000 rcsb.utils.io-1.46/rcsb.utils.io.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-01-17 16:21:39.184005 rcsb.utils.io-1.46/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2271 2024-01-17 16:15:54.000000 rcsb.utils.io-1.46/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:39:04.343822 rcsb_utils_io-1.47/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9669 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     5382 2024-05-21 16:39:04.343822 rcsb_utils_io-1.47/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3950 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:39:04.339822 rcsb_utils_io-1.47/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:39:04.339822 rcsb_utils_io-1.47/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:39:04.343822 rcsb_utils_io-1.47/rcsb/utils/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1828 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/CacheUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6208 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/CryptUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4635 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/ExecUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12049 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/FastaUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5604 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/FileLock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25377 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/FileUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12683 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/FtpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6281 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/GitUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/HashableDict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6761 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/IndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36574 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/IoUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4113 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/LogUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7429 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/MarshalUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5113 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/ProcessStatusUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6260 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/SftpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/SingletonClass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/SplitJoin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12245 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/StashUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11807 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/StashableBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3145 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14760 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/UrlRequestUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4495 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/rcsb/utils/io/decorators.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 16:39:04.343822 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5382 2024-05-21 16:39:04.000000 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      975 2024-05-21 16:39:04.000000 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 16:39:04.000000 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 16:33:41.000000 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-21 16:39:04.000000 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-21 16:39:04.000000 rcsb_utils_io-1.47/rcsb.utils.io.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-21 16:39:04.347822 rcsb_utils_io-1.47/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2271 2024-05-21 16:32:08.000000 rcsb_utils_io-1.47/setup.py
```

### Comparing `rcsb.utils.io-1.46/HISTORY.txt` & `rcsb_utils_io-1.47/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -130,8 +130,9 @@
 23-Dec-2022  - V1.39 Configuration changes to support tox 4
 13-Feb-2023  - V1.40 Resolve pylint issues
 14-Mar-2023  - V1.41 Make 'timeout' parameter a keyword argument for instantiating FileUtil object
 15-Mar-2023  - V1.42 Fix checking for remote branches by name in GitUtil()
  8-May-2023  - V1.43 Use allowed_methods instead of deprecated param in UrlRequestUtil()
 15-May-2023  - V1.44 Update urllib3 requirements
 19-May-2023  - V1.45 Update DNS to PDB archive
-17-Jan-2024  - V1.46 Add BCIF import and export support to IoUtil and MarshalUtil
+17-Jan-2024  - V1.46 Add BCIF import and export support to IoUtil and MarshalUtil
+21-May-2024  - V1.47 Fix pylinting
```

### Comparing `rcsb.utils.io-1.46/LICENSE` & `rcsb_utils_io-1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/PKG-INFO` & `rcsb_utils_io-1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.io
-Version: 1.46
+Version: 1.47
 Summary: RCSB Python I/O Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_io
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.io-1.46/README.md` & `rcsb_utils_io-1.47/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/CacheUtils.py` & `rcsb_utils_io-1.47/rcsb/utils/io/CacheUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/CryptUtils.py` & `rcsb_utils_io-1.47/rcsb/utils/io/CryptUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
             hashType (str, optional): one of MD5, SHA1, or SHA256. Defaults to "SHA1".
             blockSize (int, optional): the size of incremental read operations. Defaults to 65536.
 
         Returns:
             (dict): {"hashDigest": xxxx , "hashType": 'SHA1|MD5|SHA256'}
         """
         rD = {}
+        hashObj = None
         if hashType not in ["MD5", "SHA1", "SHA256"]:
             return rD
         try:
             if hashType == "SHA1":
                 hashObj = hashlib.sha1()
             elif hashType == "SHA256":
                 hashObj = hashlib.sha256()
```

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/ExecUtils.py` & `rcsb_utils_io-1.47/rcsb/utils/io/ExecUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/FastaUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/FastaUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
             geneName = ""
             dbName = ""
             dbAccession = ""
             dbIsoform = ""
             seqId = ""
             description = ""
             taxId = ""
+            entryName = ""
             # proteinExistence = ""
             # seqVersion = ""
             #
             match = self.__uniProtCommentRegex.match(cmtLine)
             if match:
                 groups = match.groups()
                 dbName = groups[0]
```

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/FileLock.py` & `rcsb_utils_io-1.47/rcsb/utils/io/FileLock.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/FileUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/FileUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/FtpUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/FtpUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/GitUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/GitUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/HashableDict.py` & `rcsb_utils_io-1.47/rcsb/utils/io/HashableDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/IndexUtils.py` & `rcsb_utils_io-1.47/rcsb/utils/io/IndexUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/IoUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/IoUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,14 +664,15 @@
 
         Returns:
             (iterator): iterator for rowwise access to processed CSV data
         """
         encoding = kwargs.get("encoding", "utf-8-sig")
         maxInt = sys.maxsize
         csv.field_size_limit(maxInt)
+        reader = None
         try:
             if filePath[-3:] == ".gz":
                 with gzip.open(filePath, "rt", encoding=encoding, errors=encodingErrors) as csvFile:
                     startIt = itertools.dropwhile(lambda x: x.startswith("#"), csvFile) if uncomment else csvFile
                     if rowFormat == "dict":
                         reader = csv.DictReader(startIt, delimiter=delimiter)
                     elif rowFormat == "list":
```

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/LogUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/LogUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/MarshalUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/MarshalUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/ProcessStatusUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/ProcessStatusUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/SftpUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/SftpUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/SingletonClass.py` & `rcsb_utils_io-1.47/rcsb/utils/io/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/SplitJoin.py` & `rcsb_utils_io-1.47/rcsb/utils/io/SplitJoin.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/StashUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/StashUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/StashableBase.py` & `rcsb_utils_io-1.47/rcsb/utils/io/StashableBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/TimeUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/UrlRequestUtil.py` & `rcsb_utils_io-1.47/rcsb/utils/io/UrlRequestUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb/utils/io/decorators.py` & `rcsb_utils_io-1.47/rcsb/utils/io/decorators.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/rcsb.utils.io.egg-info/PKG-INFO` & `rcsb_utils_io-1.47/rcsb.utils.io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.io
-Version: 1.46
+Version: 1.47
 Summary: RCSB Python I/O Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_io
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.io-1.46/rcsb.utils.io.egg-info/SOURCES.txt` & `rcsb_utils_io-1.47/rcsb.utils.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.io-1.46/setup.py` & `rcsb_utils_io-1.47/setup.py`

 * *Files identical despite different names*

