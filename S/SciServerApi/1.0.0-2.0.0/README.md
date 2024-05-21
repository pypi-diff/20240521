# Comparing `tmp/SciServerApi-1.0.0.tar.gz` & `tmp/SciServerApi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciServerApi-1.0.0.tar", last modified: Tue May 21 00:26:42 2024, max compression
+gzip compressed data, was "dist/SciServerApi-2.0.0.tar", last modified: Tue May 21 05:48:23 2024, max compression
```

## Comparing `SciServerApi-1.0.0.tar` & `SciServerApi-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 00:26:42.210944 SciServerApi-1.0.0/
--rw-r--r--   0 lxj       (1000) lxj       (1000)     1068 2024-05-20 02:42:11.000000 SciServerApi-1.0.0/LICENSE.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)      920 2024-05-21 00:26:42.210944 SciServerApi-1.0.0/PKG-INFO
--rw-r--r--   0 lxj       (1000) lxj       (1000)      517 2024-05-20 02:40:38.000000 SciServerApi-1.0.0/README.md
-drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 00:26:42.210944 SciServerApi-1.0.0/SciServerApi/
--rw-r--r--   0 lxj       (1000) lxj       (1000)      798 2024-05-20 23:54:12.000000 SciServerApi-1.0.0/SciServerApi/Authentication.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)    11562 2024-05-20 08:40:36.000000 SciServerApi-1.0.0/SciServerApi/Files.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)    15268 2024-05-21 00:06:33.000000 SciServerApi-1.0.0/SciServerApi/Jobs.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)       27 2024-05-19 13:01:51.000000 SciServerApi-1.0.0/SciServerApi/__init__.py
-drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 00:26:42.210944 SciServerApi-1.0.0/SciServerApi.egg-info/
--rw-r--r--   0 lxj       (1000) lxj       (1000)      920 2024-05-21 00:26:42.000000 SciServerApi-1.0.0/SciServerApi.egg-info/PKG-INFO
--rw-r--r--   0 lxj       (1000) lxj       (1000)      273 2024-05-21 00:26:42.000000 SciServerApi-1.0.0/SciServerApi.egg-info/SOURCES.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)        1 2024-05-21 00:26:42.000000 SciServerApi-1.0.0/SciServerApi.egg-info/dependency_links.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)       13 2024-05-21 00:26:42.000000 SciServerApi-1.0.0/SciServerApi.egg-info/top_level.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)       38 2024-05-21 00:26:42.210944 SciServerApi-1.0.0/setup.cfg
--rw-r--r--   0 lxj       (1000) lxj       (1000)      683 2024-05-20 02:49:39.000000 SciServerApi-1.0.0/setup.py
+drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     1068 2024-05-20 02:42:11.000000 SciServerApi-2.0.0/LICENSE.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     1036 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/PKG-INFO
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      517 2024-05-20 02:40:38.000000 SciServerApi-2.0.0/README.md
+drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi/
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      798 2024-05-20 23:54:12.000000 SciServerApi-2.0.0/SciServerApi/Authentication.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     9879 2024-05-21 00:47:20.000000 SciServerApi-2.0.0/SciServerApi/Files.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)    15248 2024-05-21 00:34:44.000000 SciServerApi-2.0.0/SciServerApi/Jobs.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     7655 2024-05-21 05:27:42.000000 SciServerApi-2.0.0/SciServerApi/Opt.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)       27 2024-05-19 13:01:51.000000 SciServerApi-2.0.0/SciServerApi/__init__.py
+drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     1036 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/PKG-INFO
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      293 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/SOURCES.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)        1 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/dependency_links.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)       13 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/top_level.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)       38 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/setup.cfg
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      683 2024-05-21 05:48:08.000000 SciServerApi-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `SciServerApi-1.0.0/LICENSE.txt` & `SciServerApi-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SciServerApi-1.0.0/PKG-INFO` & `SciServerApi-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: SciServerApi
-Version: 1.0.0
+Version: 2.0.0
 Summary: quick access to sciserver
+Home-page: UNKNOWN
+Author: UNKNOWN
+Author-email: UNKNOWN
 License: MIT License
+Description: 
+        This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
+        
+         * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
+        
+         * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
+         
+         * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
+        
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE.txt
-
-
-This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
-
- * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
-
- * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
- 
- * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
-
```

### Comparing `SciServerApi-1.0.0/README.md` & `SciServerApi-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `SciServerApi-1.0.0/SciServerApi/Authentication.py` & `SciServerApi-2.0.0/SciServerApi/Authentication.py`

 * *Files identical despite different names*

### Comparing `SciServerApi-1.0.0/SciServerApi/Files.py` & `SciServerApi-2.0.0/SciServerApi/Files.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 from SciServerApi import Authentication
 import requests
 import json
 from io import BytesIO
-import subprocess
 
 RacmApiURL = "https://apps.sciserver.org/racm"
 
-def getFileServices():
-    """
-    Gets the definitions of file services that a user is able to access. A FileService represents a file system that contains root volumes accessible to the user for public/private data storage. Within each rootVolume, users can create sharable userVolumes for storing files.
-
-    :param verbose: boolean parameter defining whether warnings will be printed (set to True) or not (set to False).
-    :return: list of dictionaries, where each dictionary represents the description of a FileService that the user is able to access.
-    :raises: Throws an exception if the user is not logged into SciServer (use Authentication.login for that purpose). Throws an exception if the HTTP request to the RACM API returns an error.
-    :example: fileServices = Files.getFileServices();
-
-    """
+def getFileServiceFromName(fileServiceName):
     url = RacmApiURL + "/storem/fileservices?TaskName=SciScript-Python.Files.getFileServices"
     headers = {'X-Auth-Token': Authentication.keyToken}
 
     res = requests.get(url, headers=headers)
 
     if res.status_code >= 200 and res.status_code < 300:
-        fileServices = [];
         fileServicesAPIs = json.loads(res.content.decode())
         for fileServicesAPI in fileServicesAPIs:
             url = fileServicesAPI.get("apiEndpoint") + "api/volumes/?TaskName=SciScript-Python.Files.getFileServices"
             res = requests.get(url, headers=headers)
             if res.status_code >= 200 and res.status_code < 300:
-                fileServices.append(json.loads(res.content.decode()))
-        return fileServices;
+                fileService = json.loads(res.content.decode())
+                if fileServiceName == fileService.get('name'):
+                    return fileService
+            else:
+                raise Exception("Error when getting the FileService.\nHttp Response from FileService returned status code " + str(res.status_code) + ":\n" + res.content.decode());
     else:
         raise Exception("Error when getting the list of FileServices.\nHttp Response from FileService API returned status code " + str(res.status_code) + ":\n" + res.content.decode());
 
-def getFileServiceFromName(fileServiceName):
-    fileServices = getFileServices()
-    for fileService in fileServices:
-        if fileServiceName == fileService.get('name'):
-            return fileService
-
 def createDir(fileService, path):
     """
     Create a directory.
 
     :param fileService: name of fileService (string), or object (dictionary) that defines a file service. A list of these kind of objects available to the user is returned by the function Files.getFileServices().
     :param path: path (in the remote file service) to the directory (string), starting from the root volume level or data volume level. Examples: rootVolume/userVolumeOwner/userVolume/directory or dataVolume/directory
     :raises: Throws an exception if the user is not logged into SciServer (use Authentication.login for that purpose). Throws an exception if the HTTP request to the FileService API returns an error.
@@ -55,15 +41,14 @@
 
     res = requests.put(url, headers=headers)
     if res.status_code >= 200 and res.status_code < 300:
         pass
     else:
         raise Exception("Error when creating directory '" + str(path) + "' in file service '" + str(fileService.get('name')) + "'.\nHttp Response from FileService API returned status code " + str(res.status_code) + ":\n" + res.content.decode());
 
-
 def dirList(fileService, path, level=1, options=''):
     """
     Lists the contents of a directory.
 
     :param fileService: name of fileService (string), or object (dictionary) that defines a file service. A list of these kind of objects available to the user is returned by the function Files.getFileServices().
     :param path: String defining the path (in the remote file service) of the directory to be listed, starting from the root volume level or data volume level. Examples: rootVolume/userVolumeOwner/userVolume/directoryToBeListed or dataVolume/directoryToBeListed
     :param level: amount (int) of listed directory levels that are below or at the same level to that of the relativePath.
@@ -124,50 +109,32 @@
     if res.status_code >= 200 and res.status_code < 300:
         pass
     else:
         raise Exception("Error when uploading file to '" + str(path) + "' in file service '" + str(fileService.get('name')) + "'.\nHttp Response from FileService API returned status code " + str(res.status_code) + ":\n" + res.content.decode());
 
 
 
-def download(fileService, path, localFilePath,**kwargs):
+def download(fileService, path, localFilePath):
     """
     Downloads a file from the remote file system into the local file system, or returns the file content as an object in several formats.
 
     :param fileService: name of fileService (string), or object (dictionary) that defines a file service. A list of these kind of objects available to the user is returned by the function Files.getFileServices().
     :param path: String defining the path (in the remote file service) of the file to be downloaded, starting from the root volume level or data volume level. Examples: rootVolume/userVolumeOwner/userVolume/fileToBeDownloaded.txt or dataVolume/fileToBeDownloaded.txt
     :param localFilePath: local destination path of the file to be downloaded. If set to None, then an object of format 'format' will be returned.
     :return: If the 'localFilePath' parameter is defined, then it will return True when the file is downloaded successfully in the local file system. If the 'localFilePath' is not defined, then the type of the returned object depends on the value of the 'format' parameter (either io.StringIO, io.BytesIO, requests.Response or string).
     :raises: Throws an exception if the user is not logged into SciServer (use Authentication.login for that purpose). Throws an exception if the HTTP request to the FileService API returns an error.
     :example: fileServices = Files.getFileServices(); Files.upload(fileServices[0], "Storage/myUserName/persistent/fileToBeDownloaded.txt", localFilePath="/fileToBeDownloaded.txt");
 
     """
-    proxies = kwargs.get("proxies",{"http": "http://127.0.0.1:7890","https": "http://127.0.0.1:7890"})
-    
+
     url = fileService.get("apiEndpoint").rstrip("/")+"/api/file/"+path.strip("/")+"?quiet=True&TaskName=SciScript-Python.Files.DownloadFile"
     headers = {'X-Auth-Token': Authentication.keyToken}
 
-    res = requests.get(url, stream=True, headers=headers,proxies = proxies)
+    res = requests.get(url, stream=True, headers=headers)
     if res.status_code < 200 or res.status_code >= 300:
         raise Exception("Error when downloading '" + str(path) + "' from file service '" + str(fileService.get("name")) + "'.\nHttp Response from FileService API returned status code " + str(res.status_code) + ":\n" + res.content.decode());
     bytesio = BytesIO(res.content)
     theFile = open(localFilePath, "w+b")
     theFile.write(bytesio.read())
     theFile.close()
     return True
 
-
-def wget(fileService, path, localFilePath, **kwargs):
-    proxies = kwargs.get("proxies",{"http": "http://127.0.0.1:7890","https": "http://127.0.0.1:7890"})
-    asyncArgs = kwargs.get("asyncArgs",False)
-    wgetArgs = kwargs.get("wgetArgs","--quiet --no-clobber")
-
-    url = fileService.get("apiEndpoint").rstrip("/") + "/api/file/" + path.strip("/") + "?TaskName=SciScript-Python.Files.DownloadFile"
-    headers = {'X-Auth-Token': Authentication.keyToken}
-
-    cmd = f"proxy=on http_proxy={proxies['http']} https_proxy={proxies['http']} wget \"{url}\" --header \'{headers}\' --output-document \"{localFilePath}\" {wgetArgs} "
-    
-    if asyncArgs:
-        pipe = subprocess.run(cmd,shell=True)
-        return pipe.returncode
-    else:
-        return subprocess.Ppoen(cmd,shell=True)
-
```

### Comparing `SciServerApi-1.0.0/SciServerApi/Jobs.py` & `SciServerApi-2.0.0/SciServerApi/Jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         raise Exception("Error when getting Docker Compute Domains from JOBM API.\nHttp Response from JOBM API returned status code " + str(res.status_code) + ":\n" + res.content.decode());
     else:
         dockerComputeDomains = json.loads(res.content.decode())
     for dockerComputeDomain in dockerComputeDomains:
         if dockerComputeDomainName == dockerComputeDomain.get('name'):
             return dockerComputeDomain
 
-def submitNotebookJob(notebookPath, dockerComputeDomain=None, dockerImageName=None, userVolumes=None,  dataVolumes=None, resultsFolderPath="", parameters="", jobAlias= ""):
+def submitNotebookJob(notebookPath, dockerComputeDomain, dockerImageName, userVolumes,  dataVolumes, resultsFolderPath="", parameters="", jobAlias= ""):
     """
     Submits a Jupyter Notebook for execution (as an asynchronous job) inside a Docker compute domain.
 
     :param notebookPath: path of the notebook within the filesystem mounted in SciServer-Compute (string). Example: notebookPath = '/home/idies/worskpace/persistent/JupyterNotebook.ipynb'
     :param dockerComputeDomain: object (dictionary) that defines a Docker compute domain. A list of these kind of objects available to the user is returned by the function Jobs.getDockerComputeDomains().
     :param dockerImageName: name (string) of the Docker image for executing the notebook. E.g.,  dockerImageName="Python (astro)". An array of available Docker images is defined as the 'images' property in the dockerComputeDomain object.
     :param userVolumes: a list with the names of user volumes (with optional write permissions) that will be mounted to the docker Image. E.g.: userVolumes = [{'name':'persistent', 'needsWriteAccess':False},{'name':'scratch', , 'needsWriteAccess':True}] . A list of available user volumes can be found as the 'userVolumes' property in the dockerComputeDomain object. If userVolumes=None, then all available user volumes are mounted, with 'needsWriteAccess' = True if the user has Write permissions on the volume.
```

### Comparing `SciServerApi-1.0.0/SciServerApi.egg-info/PKG-INFO` & `SciServerApi-2.0.0/SciServerApi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: SciServerApi
-Version: 1.0.0
+Version: 2.0.0
 Summary: quick access to sciserver
+Home-page: UNKNOWN
+Author: UNKNOWN
+Author-email: UNKNOWN
 License: MIT License
+Description: 
+        This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
+        
+         * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
+        
+         * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
+         
+         * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
+        
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE.txt
-
-
-This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
-
- * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
-
- * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
- 
- * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
-
```

### Comparing `SciServerApi-1.0.0/setup.py` & `SciServerApi-2.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='SciServerApi',  # 包名
-      version='1.0.0',  # 版本号
+      version='2.0.0',  # 版本号
       description='quick access to sciserver',
       long_description=open("README.md", "r").read(),
       install_requires=[],
       license='MIT License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
```

