# Comparing `tmp/cyberonix-3.0.3.tar.gz` & `tmp/cyberonix-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberonix-3.0.3.tar", last modified: Tue May 21 04:12:55 2024, max compression
+gzip compressed data, was "cyberonix-3.0.4.tar", last modified: Tue May 21 04:21:00 2024, max compression
```

## Comparing `cyberonix-3.0.3.tar` & `cyberonix-3.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.646157 cyberonix-3.0.3/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:12:55.646157 cyberonix-3.0.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.638157 cyberonix-3.0.3/cyberonix/
--rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.3/cyberonix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13585 2024-05-21 04:11:30.000000 cyberonix-3.0.3/cyberonix/cyberonix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.638157 cyberonix-3.0.3/cyberonix/main/
--rw-r--r--   0 root         (0) root         (0)    24214 2024-05-21 04:01:49.000000 cyberonix-3.0.3/cyberonix/main/Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31514 2024-05-21 04:01:32.000000 cyberonix-3.0.3/cyberonix/main/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-05-21 04:01:59.000000 cyberonix-3.0.3/cyberonix/main/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.642157 cyberonix-3.0.3/cyberonix/main/tools/
--rw-r--r--   0 root         (0) root         (0)     4424 2024-05-21 04:02:32.000000 cyberonix-3.0.3/cyberonix/main/tools/Anonymity.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-05-21 04:02:42.000000 cyberonix-3.0.3/cyberonix/main/tools/Authentication.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-05-21 04:02:52.000000 cyberonix-3.0.3/cyberonix/main/tools/Authorization.py
--rw-r--r--   0 root         (0) root         (0)    13287 2024-05-21 04:03:15.000000 cyberonix-3.0.3/cyberonix/main/tools/Configuration_Management.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-21 04:03:30.000000 cyberonix-3.0.3/cyberonix/main/tools/Cryptography.py
--rw-r--r--   0 root         (0) root         (0)    10863 2024-05-21 04:04:02.000000 cyberonix-3.0.3/cyberonix/main/tools/Exploitation_Tools.py
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-21 04:04:11.000000 cyberonix-3.0.3/cyberonix/main/tools/File_Upload.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-21 04:04:36.000000 cyberonix-3.0.3/cyberonix/main/tools/Framework.py
--rw-r--r--   0 root         (0) root         (0)    28889 2024-05-21 04:05:17.000000 cyberonix-3.0.3/cyberonix/main/tools/Password_Hacking.py
--rw-r--r--   0 root         (0) root         (0)     4881 2024-05-21 04:05:32.000000 cyberonix-3.0.3/cyberonix/main/tools/Pentesting_Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)    16560 2024-05-21 04:05:45.000000 cyberonix-3.0.3/cyberonix/main/tools/PostExploitationAttacks.py
--rw-r--r--   0 root         (0) root         (0)   171224 2024-05-21 04:05:55.000000 cyberonix-3.0.3/cyberonix/main/tools/Recommended_Tool.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-05-21 04:06:19.000000 cyberonix-3.0.3/cyberonix/main/tools/RiskyFuncPayment.py
--rw-r--r--   0 root         (0) root         (0)     5204 2024-05-21 04:06:31.000000 cyberonix-3.0.3/cyberonix/main/tools/Secure_Transmission.py
--rw-r--r--   0 root         (0) root         (0)    11474 2024-05-21 04:06:42.000000 cyberonix-3.0.3/cyberonix/main/tools/Session_Management.py
--rw-r--r--   0 root         (0) root         (0)    10736 2024-05-21 04:06:51.000000 cyberonix-3.0.3/cyberonix/main/tools/Sniffing_and_Spoofing.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-05-21 04:07:13.000000 cyberonix-3.0.3/cyberonix/main/tools/Vulnerability_Analysis.py
--rw-r--r--   0 root         (0) root         (0)    13445 2024-05-21 04:07:26.000000 cyberonix-3.0.3/cyberonix/main/tools/WEB_Application_Analysis.py
--rw-r--r--   0 root         (0) root         (0)     6825 2024-05-21 04:07:40.000000 cyberonix-3.0.3/cyberonix/main/tools/Wireless_Hacking.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-05-21 04:03:01.000000 cyberonix-3.0.3/cyberonix/main/tools/banner.py
--rw-r--r--   0 root         (0) root         (0)      207 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/colors.py
--rw-r--r--   0 root         (0) root         (0)    27322 2024-05-21 04:03:43.000000 cyberonix-3.0.3/cyberonix/main/tools/data_validation.py
--rw-r--r--   0 root         (0) root         (0)     5787 2024-05-21 04:03:52.000000 cyberonix-3.0.3/cyberonix/main/tools/dos.py
--rw-r--r--   0 root         (0) root         (0)     4864 2024-05-21 04:04:21.000000 cyberonix-3.0.3/cyberonix/main/tools/forensic.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-05-21 04:04:48.000000 cyberonix-3.0.3/cyberonix/main/tools/html5.py
--rw-r--r--   0 root         (0) root         (0)    18178 2024-05-21 04:05:05.000000 cyberonix-3.0.3/cyberonix/main/tools/information_gathering.py
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/run_on_browser.py
--rw-r--r--   0 root         (0) root         (0)    16802 2024-05-21 04:07:02.000000 cyberonix-3.0.3/cyberonix/main/tools/template.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/waiting.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-21 04:07:51.000000 cyberonix-3.0.3/cyberonix/main/tools/writeup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.638157 cyberonix-3.0.3/cyberonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 04:12:55.646157 cyberonix-3.0.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1330 2024-05-21 03:37:54.000000 cyberonix-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:21:00.374394 cyberonix-3.0.4/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:21:00.374394 cyberonix-3.0.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:21:00.366394 cyberonix-3.0.4/cyberonix/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.4/cyberonix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13609 2024-05-21 04:20:28.000000 cyberonix-3.0.4/cyberonix/cyberonix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:21:00.366394 cyberonix-3.0.4/cyberonix/main/
+-rw-r--r--   0 root         (0) root         (0)    24214 2024-05-21 04:01:49.000000 cyberonix-3.0.4/cyberonix/main/Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-17 14:30:27.000000 cyberonix-3.0.4/cyberonix/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31514 2024-05-21 04:01:32.000000 cyberonix-3.0.4/cyberonix/main/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-05-21 04:01:59.000000 cyberonix-3.0.4/cyberonix/main/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:21:00.374394 cyberonix-3.0.4/cyberonix/main/tools/
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-21 04:02:32.000000 cyberonix-3.0.4/cyberonix/main/tools/Anonymity.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-05-21 04:02:42.000000 cyberonix-3.0.4/cyberonix/main/tools/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-21 04:02:52.000000 cyberonix-3.0.4/cyberonix/main/tools/Authorization.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2024-05-21 04:03:15.000000 cyberonix-3.0.4/cyberonix/main/tools/Configuration_Management.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-21 04:03:30.000000 cyberonix-3.0.4/cyberonix/main/tools/Cryptography.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2024-05-21 04:04:02.000000 cyberonix-3.0.4/cyberonix/main/tools/Exploitation_Tools.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-21 04:04:11.000000 cyberonix-3.0.4/cyberonix/main/tools/File_Upload.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-21 04:04:36.000000 cyberonix-3.0.4/cyberonix/main/tools/Framework.py
+-rw-r--r--   0 root         (0) root         (0)    28889 2024-05-21 04:05:17.000000 cyberonix-3.0.4/cyberonix/main/tools/Password_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2024-05-21 04:05:32.000000 cyberonix-3.0.4/cyberonix/main/tools/Pentesting_Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)    16560 2024-05-21 04:05:45.000000 cyberonix-3.0.4/cyberonix/main/tools/PostExploitationAttacks.py
+-rw-r--r--   0 root         (0) root         (0)   171224 2024-05-21 04:05:55.000000 cyberonix-3.0.4/cyberonix/main/tools/Recommended_Tool.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-21 04:06:19.000000 cyberonix-3.0.4/cyberonix/main/tools/RiskyFuncPayment.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2024-05-21 04:06:31.000000 cyberonix-3.0.4/cyberonix/main/tools/Secure_Transmission.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2024-05-21 04:06:42.000000 cyberonix-3.0.4/cyberonix/main/tools/Session_Management.py
+-rw-r--r--   0 root         (0) root         (0)    10736 2024-05-21 04:06:51.000000 cyberonix-3.0.4/cyberonix/main/tools/Sniffing_and_Spoofing.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-05-21 04:07:13.000000 cyberonix-3.0.4/cyberonix/main/tools/Vulnerability_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)    13445 2024-05-21 04:07:26.000000 cyberonix-3.0.4/cyberonix/main/tools/WEB_Application_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-21 04:07:40.000000 cyberonix-3.0.4/cyberonix/main/tools/Wireless_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-17 14:30:27.000000 cyberonix-3.0.4/cyberonix/main/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-21 04:03:01.000000 cyberonix-3.0.4/cyberonix/main/tools/banner.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-05-17 14:30:27.000000 cyberonix-3.0.4/cyberonix/main/tools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    27322 2024-05-21 04:03:43.000000 cyberonix-3.0.4/cyberonix/main/tools/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)     5787 2024-05-21 04:03:52.000000 cyberonix-3.0.4/cyberonix/main/tools/dos.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-05-21 04:04:21.000000 cyberonix-3.0.4/cyberonix/main/tools/forensic.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-05-21 04:04:48.000000 cyberonix-3.0.4/cyberonix/main/tools/html5.py
+-rw-r--r--   0 root         (0) root         (0)    18178 2024-05-21 04:05:05.000000 cyberonix-3.0.4/cyberonix/main/tools/information_gathering.py
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-17 14:30:27.000000 cyberonix-3.0.4/cyberonix/main/tools/run_on_browser.py
+-rw-r--r--   0 root         (0) root         (0)    16802 2024-05-21 04:07:02.000000 cyberonix-3.0.4/cyberonix/main/tools/template.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-17 14:30:27.000000 cyberonix-3.0.4/cyberonix/main/tools/waiting.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-21 04:07:51.000000 cyberonix-3.0.4/cyberonix/main/tools/writeup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:21:00.366394 cyberonix-3.0.4/cyberonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:21:00.000000 cyberonix-3.0.4/cyberonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-21 04:21:00.000000 cyberonix-3.0.4/cyberonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 04:21:00.000000 cyberonix-3.0.4/cyberonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-21 04:21:00.000000 cyberonix-3.0.4/cyberonix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-21 04:21:00.000000 cyberonix-3.0.4/cyberonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 04:21:00.000000 cyberonix-3.0.4/cyberonix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 04:21:00.374394 cyberonix-3.0.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2024-05-21 04:20:51.000000 cyberonix-3.0.4/setup.py
```

### Comparing `cyberonix-3.0.3/PKG-INFO` & `cyberonix-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.3
+Version: 3.0.4
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamDefronix/Cyberonix
 Author: Defronix
 Author-email: hello@defronix.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.3 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.4 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-3.0.3/README.md` & `cyberonix-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/cyberonix.py` & `cyberonix-3.0.4/cyberonix/cyberonix.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 try:
     def starting():
         try:
                 subprocess.run('sudo mv cyberonix.1 /usr/local/man/man1/',shell=True, check = True)
         except Exception as err:
                 try:
-			subprocess.run('sudo mv cyberonix/cyberonix.1 /usr/local/man/man1/',shell=True, check = True)
-		except:
-			pass
+			        subprocess.run('sudo mv cyberonix/cyberonix.1 /usr/local/man/man1/',shell=True, check = True)
+		        except:
+			        pass
         #os.system("sudo mv cyberonix.1 /usr/local/man/man1/")
         parser = argparse.ArgumentParser(
             description="Cyberonix is a complete resource hub for Cyber Security Community. Our aim is to make this tool an 1 stop solution for all the Hackers out there to get resources of various topics in Cyber Security. We will keep updating this tool & adding new & updated resources on the go.",
         )
         main_args = parser.add_argument_group('Main Arguments')
             
         main_args.add_argument(
```

### Comparing `cyberonix-3.0.3/cyberonix/main/Bug_Bounty.py` & `cyberonix-3.0.4/cyberonix/main/Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/arguments.py` & `cyberonix-3.0.4/cyberonix/main/arguments.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tool.py` & `cyberonix-3.0.4/cyberonix/main/tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Anonymity.py` & `cyberonix-3.0.4/cyberonix/main/tools/Anonymity.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Authentication.py` & `cyberonix-3.0.4/cyberonix/main/tools/Authentication.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Authorization.py` & `cyberonix-3.0.4/cyberonix/main/tools/Authorization.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Configuration_Management.py` & `cyberonix-3.0.4/cyberonix/main/tools/Configuration_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Cryptography.py` & `cyberonix-3.0.4/cyberonix/main/tools/Cryptography.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Exploitation_Tools.py` & `cyberonix-3.0.4/cyberonix/main/tools/Exploitation_Tools.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/File_Upload.py` & `cyberonix-3.0.4/cyberonix/main/tools/File_Upload.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Password_Hacking.py` & `cyberonix-3.0.4/cyberonix/main/tools/Password_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Pentesting_Bug_Bounty.py` & `cyberonix-3.0.4/cyberonix/main/tools/Pentesting_Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/PostExploitationAttacks.py` & `cyberonix-3.0.4/cyberonix/main/tools/PostExploitationAttacks.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Recommended_Tool.py` & `cyberonix-3.0.4/cyberonix/main/tools/Recommended_Tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/RiskyFuncPayment.py` & `cyberonix-3.0.4/cyberonix/main/tools/RiskyFuncPayment.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Secure_Transmission.py` & `cyberonix-3.0.4/cyberonix/main/tools/Secure_Transmission.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Session_Management.py` & `cyberonix-3.0.4/cyberonix/main/tools/Session_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Sniffing_and_Spoofing.py` & `cyberonix-3.0.4/cyberonix/main/tools/Sniffing_and_Spoofing.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Vulnerability_Analysis.py` & `cyberonix-3.0.4/cyberonix/main/tools/Vulnerability_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/WEB_Application_Analysis.py` & `cyberonix-3.0.4/cyberonix/main/tools/WEB_Application_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/Wireless_Hacking.py` & `cyberonix-3.0.4/cyberonix/main/tools/Wireless_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/banner.py` & `cyberonix-3.0.4/cyberonix/main/tools/banner.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/data_validation.py` & `cyberonix-3.0.4/cyberonix/main/tools/data_validation.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/dos.py` & `cyberonix-3.0.4/cyberonix/main/tools/dos.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/forensic.py` & `cyberonix-3.0.4/cyberonix/main/tools/forensic.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/html5.py` & `cyberonix-3.0.4/cyberonix/main/tools/html5.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/information_gathering.py` & `cyberonix-3.0.4/cyberonix/main/tools/information_gathering.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/run_on_browser.py` & `cyberonix-3.0.4/cyberonix/main/tools/run_on_browser.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/template.py` & `cyberonix-3.0.4/cyberonix/main/tools/template.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix/main/tools/writeup.py` & `cyberonix-3.0.4/cyberonix/main/tools/writeup.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/cyberonix.egg-info/PKG-INFO` & `cyberonix-3.0.4/cyberonix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.3
+Version: 3.0.4
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamDefronix/Cyberonix
 Author: Defronix
 Author-email: hello@defronix.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.3 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.4 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-3.0.3/cyberonix.egg-info/SOURCES.txt` & `cyberonix-3.0.4/cyberonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.3/setup.py` & `cyberonix-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cyberonix",
-    version="3.0.3",
+    version="3.0.4",
     author="Defronix",
     author_email="hello@defronix.com",
     description="Cyberonix is a complete resource hub for Cyber Security Community.",
     url='https://github.com/TeamDefronix/Cyberonix',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

