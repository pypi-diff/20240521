# Comparing `tmp/pih-ssh-0.11.tar.gz` & `tmp/pih-ssh-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ssh-0.11.tar", last modified: Wed Apr 10 02:30:16 2024, max compression
+gzip compressed data, was "pih-ssh-0.12.tar", last modified: Mon May 20 23:16:46 2024, max compression
```

## Comparing `pih-ssh-0.11.tar` & `pih-ssh-0.12.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:30:17.018956 pih-ssh-0.11/
--rw-rw-rw-   0        0        0      288 2024-04-10 02:30:16.972063 pih-ssh-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:30:16.592923 pih-ssh-0.11/SSHService/
--rw-rw-rw-   0        0        0        0 2022-07-23 04:31:56.000000 pih-ssh-0.11/SSHService/__init__.py
--rw-rw-rw-   0        0        0      145 2024-02-14 10:50:22.000000 pih-ssh-0.11/SSHService/__main__.py
--rw-rw-rw-   0        0        0     4108 2024-02-25 01:07:12.000000 pih-ssh-0.11/SSHService/api.py
--rw-rw-rw-   0        0        0      343 2023-08-05 09:47:04.000000 pih-ssh-0.11/SSHService/api_test.py
--rw-rw-rw-   0        0        0     1031 2024-04-10 01:18:16.000000 pih-ssh-0.11/SSHService/const.py
--rw-rw-rw-   0        0        0     2632 2024-04-10 00:54:37.000000 pih-ssh-0.11/SSHService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:30:16.923126 pih-ssh-0.11/pih_ssh.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:30:17.018956 pih-ssh-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:16:46.446207 pih-ssh-0.12/
+-rw-rw-rw-   0        0        0      288 2024-05-20 23:16:46.414963 pih-ssh-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:16:46.070441 pih-ssh-0.12/SSHService/
+-rw-rw-rw-   0        0        0        0 2022-07-23 04:31:56.000000 pih-ssh-0.12/SSHService/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-02-14 10:50:22.000000 pih-ssh-0.12/SSHService/__main__.py
+-rw-rw-rw-   0        0        0     4108 2024-02-25 01:07:12.000000 pih-ssh-0.12/SSHService/api.py
+-rw-rw-rw-   0        0        0     1031 2024-05-20 22:40:33.000000 pih-ssh-0.12/SSHService/const.py
+-rw-rw-rw-   0        0        0     2632 2024-04-10 00:54:37.000000 pih-ssh-0.12/SSHService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:16:46.383714 pih-ssh-0.12/pih_ssh.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-05-20 23:16:45.000000 pih-ssh-0.12/pih_ssh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-20 23:16:45.000000 pih-ssh-0.12/pih_ssh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:16:45.000000 pih-ssh-0.12/pih_ssh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-20 23:16:45.000000 pih-ssh-0.12/pih_ssh.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 23:16:45.000000 pih-ssh-0.12/pih_ssh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 23:16:45.000000 pih-ssh-0.12/pih_ssh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:16:46.477459 pih-ssh-0.12/setup.cfg
```

### Comparing `pih-ssh-0.11/SSHService/api.py` & `pih-ssh-0.12/SSHService/api.py`

 * *Files identical despite different names*

### Comparing `pih-ssh-0.11/SSHService/const.py` & `pih-ssh-0.12/SSHService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts.ssh_hosts import SSHHosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "SSH"
 
 HOST = A.CT_H.BACKUP_WORKER
 
-VERSION: str ="0.11"
+VERSION: str ="0.12"
 
 PACKAGES: tuple[str, ...] = ("paramiko",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="SSH service",
     host=HOST.NAME,
```

### Comparing `pih-ssh-0.11/SSHService/service.py` & `pih-ssh-0.12/SSHService/service.py`

 * *Files identical despite different names*

