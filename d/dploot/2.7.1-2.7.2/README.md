# Comparing `tmp/dploot-2.7.1.tar.gz` & `tmp/dploot-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dploot-2.7.1.tar", max compression
+gzip compressed data, was "dploot-2.7.2.tar", max compression
```

## Comparing `dploot-2.7.1.tar` & `dploot-2.7.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1081 2024-03-07 17:48:20.612283 dploot-2.7.1/LICENSE
--rwxr-xr-x   0        0        0    31228 2024-04-02 15:39:26.758687 dploot-2.7.1/README.md
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/action/__init__.py
--rwxr-xr-x   0        0        0     3081 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/action/backupkey.py
--rwxr-xr-x   0        0        0     4530 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/browser.py
--rwxr-xr-x   0        0        0     4649 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/certificates.py
--rwxr-xr-x   0        0        0     4064 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/credentials.py
--rwxr-xr-x   0        0        0     4367 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/machinecertificates.py
--rwxr-xr-x   0        0        0     3810 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/machinecredentials.py
--rwxr-xr-x   0        0        0     3487 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/action/machinemasterkeys.py
--rwxr-xr-x   0        0        0     6098 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/machinetriage.py
--rwxr-xr-x   0        0        0     3732 2024-03-13 16:59:38.961736 dploot-2.7.1/dploot/action/machinevaults.py
--rwxr-xr-x   0        0        0     5543 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/masterkeys.py
--rw-r--r--   0        0        0     3382 2024-04-02 15:39:26.758687 dploot-2.7.1/dploot/action/mobaxterm.py
--rwxr-xr-x   0        0        0     4602 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/rdg.py
--rwxr-xr-x   0        0        0     3920 2024-03-20 10:31:46.018629 dploot-2.7.1/dploot/action/sccm.py
--rwxr-xr-x   0        0        0     7886 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/triage.py
--rwxr-xr-x   0        0        0     3964 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/action/vaults.py
--rwxr-xr-x   0        0        0     3798 2024-03-13 16:59:21.925855 dploot-2.7.1/dploot/action/wifi.py
--rwxr-xr-x   0        0        0     1966 2024-04-02 15:39:26.758687 dploot-2.7.1/dploot/entry.py
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/lib/__init__.py
--rwxr-xr-x   0        0        0    11632 2024-04-02 15:39:26.758687 dploot-2.7.1/dploot/lib/crypto.py
--rwxr-xr-x   0        0        0    10269 2024-04-02 15:39:26.758687 dploot-2.7.1/dploot/lib/dpapi.py
--rwxr-xr-x   0        0        0     9333 2024-03-13 17:15:33.555452 dploot-2.7.1/dploot/lib/smb.py
--rwxr-xr-x   0        0        0     5594 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/lib/target.py
--rwxr-xr-x   0        0        0     1905 2024-03-20 10:34:58.337564 dploot-2.7.1/dploot/lib/utils.py
--rw-r--r--   0        0        0     1867 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/lib/wmi.py
--rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/triage/__init__.py
--rwxr-xr-x   0        0        0     3068 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/triage/backupkey.py
--rwxr-xr-x   0        0        0    10855 2024-03-13 16:53:02.472508 dploot-2.7.1/dploot/triage/browser.py
--rwxr-xr-x   0        0        0    13166 2024-04-02 15:39:26.758687 dploot-2.7.1/dploot/triage/certificates.py
--rwxr-xr-x   0        0        0     6500 2024-03-07 14:31:27.130460 dploot-2.7.1/dploot/triage/credentials.py
--rwxr-xr-x   0        0        0     9556 2024-04-02 15:39:26.758687 dploot-2.7.1/dploot/triage/masterkeys.py
--rw-r--r--   0        0        0    16681 2024-04-03 13:01:16.684927 dploot-2.7.1/dploot/triage/mobaxterm.py
--rwxr-xr-x   0        0        0     8599 2024-03-07 14:31:27.134460 dploot-2.7.1/dploot/triage/rdg.py
--rwxr-xr-x   0        0        0     9479 2024-03-13 17:15:46.691380 dploot-2.7.1/dploot/triage/sccm.py
--rwxr-xr-x   0        0        0     9179 2024-03-20 10:32:33.930377 dploot-2.7.1/dploot/triage/vaults.py
--rwxr-xr-x   0        0        0     9425 2024-03-13 17:16:21.995184 dploot-2.7.1/dploot/triage/wifi.py
--rw-r--r--   0        0        0      901 2024-04-03 13:07:47.718285 dploot-2.7.1/pyproject.toml
--rw-r--r--   0        0        0    32170 1970-01-01 00:00:00.000000 dploot-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-03-07 17:48:20.612283 dploot-2.7.2/LICENSE
+-rwxr-xr-x   0        0        0    31401 2024-04-03 13:34:56.099274 dploot-2.7.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/action/__init__.py
+-rwxr-xr-x   0        0        0     3081 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/action/backupkey.py
+-rwxr-xr-x   0        0        0     4530 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/browser.py
+-rwxr-xr-x   0        0        0     4649 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/certificates.py
+-rwxr-xr-x   0        0        0     4064 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/credentials.py
+-rwxr-xr-x   0        0        0     4367 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/machinecertificates.py
+-rwxr-xr-x   0        0        0     3810 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/machinecredentials.py
+-rwxr-xr-x   0        0        0     3487 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/action/machinemasterkeys.py
+-rwxr-xr-x   0        0        0     6098 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/machinetriage.py
+-rwxr-xr-x   0        0        0     3732 2024-03-13 16:59:38.961736 dploot-2.7.2/dploot/action/machinevaults.py
+-rwxr-xr-x   0        0        0     5543 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/masterkeys.py
+-rw-r--r--   0        0        0     3382 2024-04-02 15:39:26.758687 dploot-2.7.2/dploot/action/mobaxterm.py
+-rwxr-xr-x   0        0        0     4602 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/rdg.py
+-rwxr-xr-x   0        0        0     3920 2024-03-20 10:31:46.018629 dploot-2.7.2/dploot/action/sccm.py
+-rwxr-xr-x   0        0        0     7886 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/triage.py
+-rwxr-xr-x   0        0        0     3964 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/action/vaults.py
+-rwxr-xr-x   0        0        0     3798 2024-03-13 16:59:21.925855 dploot-2.7.2/dploot/action/wifi.py
+-rwxr-xr-x   0        0        0     1966 2024-04-02 15:39:26.758687 dploot-2.7.2/dploot/entry.py
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/lib/__init__.py
+-rwxr-xr-x   0        0        0    11632 2024-04-02 15:39:26.758687 dploot-2.7.2/dploot/lib/crypto.py
+-rwxr-xr-x   0        0        0    10269 2024-04-02 15:39:26.758687 dploot-2.7.2/dploot/lib/dpapi.py
+-rwxr-xr-x   0        0        0     9333 2024-03-13 17:15:33.555452 dploot-2.7.2/dploot/lib/smb.py
+-rwxr-xr-x   0        0        0     5594 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/lib/target.py
+-rwxr-xr-x   0        0        0     1905 2024-03-20 10:34:58.337564 dploot-2.7.2/dploot/lib/utils.py
+-rw-r--r--   0        0        0     1867 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/lib/wmi.py
+-rw-r--r--   0        0        0        0 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/triage/__init__.py
+-rwxr-xr-x   0        0        0     3068 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/triage/backupkey.py
+-rwxr-xr-x   0        0        0    10855 2024-03-13 16:53:02.472508 dploot-2.7.2/dploot/triage/browser.py
+-rwxr-xr-x   0        0        0    13166 2024-04-02 15:39:26.758687 dploot-2.7.2/dploot/triage/certificates.py
+-rwxr-xr-x   0        0        0     6500 2024-03-07 14:31:27.130460 dploot-2.7.2/dploot/triage/credentials.py
+-rwxr-xr-x   0        0        0     9629 2024-05-21 15:39:56.855228 dploot-2.7.2/dploot/triage/masterkeys.py
+-rw-r--r--   0        0        0    16681 2024-04-03 13:01:16.684927 dploot-2.7.2/dploot/triage/mobaxterm.py
+-rwxr-xr-x   0        0        0     8599 2024-03-07 14:31:27.134460 dploot-2.7.2/dploot/triage/rdg.py
+-rwxr-xr-x   0        0        0     9479 2024-03-13 17:15:46.691380 dploot-2.7.2/dploot/triage/sccm.py
+-rwxr-xr-x   0        0        0     9179 2024-03-20 10:32:33.930377 dploot-2.7.2/dploot/triage/vaults.py
+-rwxr-xr-x   0        0        0     9425 2024-05-21 15:35:13.332052 dploot-2.7.2/dploot/triage/wifi.py
+-rw-r--r--   0        0        0      901 2024-05-21 15:40:37.339074 dploot-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0    32343 1970-01-01 00:00:00.000000 dploot-2.7.2/PKG-INFO
```

### Comparing `dploot-2.7.1/LICENSE` & `dploot-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/README.md` & `dploot-2.7.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,26 +36,30 @@
       - [backupkey](#backupkey)
       - [mobaxterm](#mobaxterm)
   - [Credits](#credits)
   - [TODO](#TODO)
 
 ## Installation
 
-You can install dploot directly from PyPI:
+You can install dploot directly from PyPI with [pipx](https://github.com/pypa/pipx):
 
 ```text
-pip install dploot
+pipx install git+https://github.com/zblurx/dploot.git
 ```
 
 OR
 
 ```text
-git clone https://github.com/zblurx/dploot.git
-cd dploot
-make
+pipx install dploot
+```
+
+On [Kali Linux](https://www.kali.org/), you can install dploot from the repositories:
+
+```text
+sudo apt install python3-dploot
 ```
 
 ## Usage
 
 ```text
 usage: dploot [-h] [-debug] [-quiet] {certificates,credentials,masterkeys,vaults,backupkey,rdg,triage,machinemasterkeys,machinecredentials,machinevaults,machinecertificates,machinetriage,browser,wifi} ...
 
@@ -719,15 +723,15 @@
 ### mobaxterm
 
 The **mobaxterm** command will extract MobaXterm secrets and masterpassword key from hive (HKU) and decrypt them with `-mkfile FILE` of one or more {GUID}:SHA1, or with `-passwords FILE` combo of user:password, `-nthashes` combo of user:nthash or a `-pvk PVKFILE` to first decrypt masterkeys. If the user is not connected on the remote target, dploot will download and extract secrets from NTUSER.dat. 
 
 With `pvk`:
 
 ```text
-dploot rdg -d waza.local -u jsmith -p 'Password#123' 192.168.56.14 -pvk key.pvk
+dploot mobaxterm -d waza.local -u jsmith -p 'Password#123' 192.168.56.14 -pvk key.pvk
 [*] Connected to 192.168.56.14 as waza.local\jsmith (admin)
 
 [*] Triage ALL USERS masterkeys
 
 {6dedb662-3f3c-43a7-bfc4-e2990a48d4dd}:32c4eeeac475910a33f531b56cf9d73f35490d5e
 {21f17bcd-eac1-4187-9538-a744f2c6e17b}:198eba83e088a59fd75e6435b38804d4973a2c1e
```

### Comparing `dploot-2.7.1/dploot/action/backupkey.py` & `dploot-2.7.2/dploot/action/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/browser.py` & `dploot-2.7.2/dploot/action/browser.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/certificates.py` & `dploot-2.7.2/dploot/action/certificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/credentials.py` & `dploot-2.7.2/dploot/action/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/machinecertificates.py` & `dploot-2.7.2/dploot/action/machinecertificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/machinecredentials.py` & `dploot-2.7.2/dploot/action/machinecredentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/machinemasterkeys.py` & `dploot-2.7.2/dploot/action/machinemasterkeys.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/machinetriage.py` & `dploot-2.7.2/dploot/action/machinetriage.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/machinevaults.py` & `dploot-2.7.2/dploot/action/machinevaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/masterkeys.py` & `dploot-2.7.2/dploot/action/masterkeys.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/mobaxterm.py` & `dploot-2.7.2/dploot/action/mobaxterm.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/rdg.py` & `dploot-2.7.2/dploot/action/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/sccm.py` & `dploot-2.7.2/dploot/action/sccm.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/triage.py` & `dploot-2.7.2/dploot/action/triage.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/vaults.py` & `dploot-2.7.2/dploot/action/vaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/action/wifi.py` & `dploot-2.7.2/dploot/action/wifi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/entry.py` & `dploot-2.7.2/dploot/entry.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/lib/crypto.py` & `dploot-2.7.2/dploot/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/lib/dpapi.py` & `dploot-2.7.2/dploot/lib/dpapi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/lib/smb.py` & `dploot-2.7.2/dploot/lib/smb.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/lib/target.py` & `dploot-2.7.2/dploot/lib/target.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/lib/utils.py` & `dploot-2.7.2/dploot/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/lib/wmi.py` & `dploot-2.7.2/dploot/lib/wmi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/backupkey.py` & `dploot-2.7.2/dploot/triage/backupkey.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/browser.py` & `dploot-2.7.2/dploot/triage/browser.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/certificates.py` & `dploot-2.7.2/dploot/triage/certificates.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/credentials.py` & `dploot-2.7.2/dploot/triage/credentials.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/masterkeys.py` & `dploot-2.7.2/dploot/triage/masterkeys.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,24 +37,26 @@
 class MasterkeysTriage:
 
     false_positive = ['.','..', 'desktop.ini','Public','Default','Default User','All Users']
     user_masterkeys_generic_path = 'AppData\\Roaming\\Microsoft\\Protect'
     system_masterkeys_generic_path = 'Windows\\System32\\Microsoft\\Protect'
     share = 'C$'
 
-    def __init__(self, target: Target, conn: DPLootSMBConnection, pvkbytes: bytes = None, passwords: Dict[str,str] = None, nthashes: Dict[str,str] = None, dpapiSystem: Dict[str,str] = {}) -> None:
+    def __init__(self, target: Target, conn: DPLootSMBConnection, pvkbytes: bytes = None, passwords: Dict[str,str] = None, nthashes: Dict[str,str] = None, dpapiSystem: Dict[str,str] = None) -> None:
         self.target = target
         self.conn = conn
         self.pvkbytes = pvkbytes
         self.passwords = passwords
         self.nthashes = nthashes
         
         self._users = None
         self.looted_files = dict()
         self.dpapiSystem = dpapiSystem
+        if self.dpapiSystem is None:
+            self.dpapiSystem = {}
         # should be {"MachineKey":"key","Userkey":"key"}
 
     def triage_system_masterkeys(self) -> List[Masterkey]:
         masterkeys = list()
         logging.getLogger("impacket").disabled = True
         if len(self.dpapiSystem) == 0:
             self.conn.enable_remoteops()
```

### Comparing `dploot-2.7.1/dploot/triage/mobaxterm.py` & `dploot-2.7.2/dploot/triage/mobaxterm.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/rdg.py` & `dploot-2.7.2/dploot/triage/rdg.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/sccm.py` & `dploot-2.7.2/dploot/triage/sccm.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/vaults.py` & `dploot-2.7.2/dploot/triage/vaults.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/dploot/triage/wifi.py` & `dploot-2.7.2/dploot/triage/wifi.py`

 * *Files identical despite different names*

### Comparing `dploot-2.7.1/pyproject.toml` & `dploot-2.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dploot"
-version = "2.7.1"
+version = "2.7.2"
 description = "DPAPI looting remotely in Python"
 readme = "README.md"
 homepage = "https://github.com/zblurx/dploot"
 repository = "https://github.com/zblurx/dploot"
 keywords = ["DPAPI", "credentials", "Windows"]
 authors = ["zblurx <seigneuret.thomas@protonmail.com>"]
 license = "MIT"
```

### Comparing `dploot-2.7.1/PKG-INFO` & `dploot-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dploot
-Version: 2.7.1
+Version: 2.7.2
 Summary: DPAPI looting remotely in Python
 Home-page: https://github.com/zblurx/dploot
 License: MIT
 Keywords: DPAPI,credentials,Windows
 Author: zblurx
 Author-email: seigneuret.thomas@protonmail.com
 Requires-Python: >=3.7,<4.0
@@ -62,26 +62,30 @@
       - [backupkey](#backupkey)
       - [mobaxterm](#mobaxterm)
   - [Credits](#credits)
   - [TODO](#TODO)
 
 ## Installation
 
-You can install dploot directly from PyPI:
+You can install dploot directly from PyPI with [pipx](https://github.com/pypa/pipx):
 
 ```text
-pip install dploot
+pipx install git+https://github.com/zblurx/dploot.git
 ```
 
 OR
 
 ```text
-git clone https://github.com/zblurx/dploot.git
-cd dploot
-make
+pipx install dploot
+```
+
+On [Kali Linux](https://www.kali.org/), you can install dploot from the repositories:
+
+```text
+sudo apt install python3-dploot
 ```
 
 ## Usage
 
 ```text
 usage: dploot [-h] [-debug] [-quiet] {certificates,credentials,masterkeys,vaults,backupkey,rdg,triage,machinemasterkeys,machinecredentials,machinevaults,machinecertificates,machinetriage,browser,wifi} ...
 
@@ -745,15 +749,15 @@
 ### mobaxterm
 
 The **mobaxterm** command will extract MobaXterm secrets and masterpassword key from hive (HKU) and decrypt them with `-mkfile FILE` of one or more {GUID}:SHA1, or with `-passwords FILE` combo of user:password, `-nthashes` combo of user:nthash or a `-pvk PVKFILE` to first decrypt masterkeys. If the user is not connected on the remote target, dploot will download and extract secrets from NTUSER.dat. 
 
 With `pvk`:
 
 ```text
-dploot rdg -d waza.local -u jsmith -p 'Password#123' 192.168.56.14 -pvk key.pvk
+dploot mobaxterm -d waza.local -u jsmith -p 'Password#123' 192.168.56.14 -pvk key.pvk
 [*] Connected to 192.168.56.14 as waza.local\jsmith (admin)
 
 [*] Triage ALL USERS masterkeys
 
 {6dedb662-3f3c-43a7-bfc4-e2990a48d4dd}:32c4eeeac475910a33f531b56cf9d73f35490d5e
 {21f17bcd-eac1-4187-9538-a744f2c6e17b}:198eba83e088a59fd75e6435b38804d4973a2c1e
```

