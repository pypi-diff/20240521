# Comparing `tmp/cyberonix-3.0.2.tar.gz` & `tmp/cyberonix-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberonix-3.0.2.tar", last modified: Sun May 12 17:49:00 2024, max compression
+gzip compressed data, was "cyberonix-3.0.3.tar", last modified: Tue May 21 04:12:55 2024, max compression
```

## Comparing `cyberonix-3.0.2.tar` & `cyberonix-3.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:49:00.761998 cyberonix-3.0.2/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:49:00.761998 cyberonix-3.0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:49:00.733998 cyberonix-3.0.2/cyberonix/
--rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.2/cyberonix/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    13347 2024-05-12 17:42:40.000000 cyberonix-3.0.2/cyberonix/cyberonix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:49:00.741998 cyberonix-3.0.2/cyberonix/main/
--rw-r--r--   0 root         (0) root         (0)    21630 2024-05-12 16:50:20.000000 cyberonix-3.0.2/cyberonix/main/Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-14 18:35:27.000000 cyberonix-3.0.2/cyberonix/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31929 2024-05-12 16:49:42.000000 cyberonix-3.0.2/cyberonix/main/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-05-12 16:50:50.000000 cyberonix-3.0.2/cyberonix/main/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:49:00.761998 cyberonix-3.0.2/cyberonix/main/tools/
--rw-r--r--   0 root         (0) root         (0)     3876 2024-05-12 16:51:19.000000 cyberonix-3.0.2/cyberonix/main/tools/Anonymity.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-05-12 16:51:44.000000 cyberonix-3.0.2/cyberonix/main/tools/Authentication.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-05-12 16:52:23.000000 cyberonix-3.0.2/cyberonix/main/tools/Authorization.py
--rw-r--r--   0 root         (0) root         (0)    13287 2024-05-12 16:52:53.000000 cyberonix-3.0.2/cyberonix/main/tools/Configuration_Management.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-12 16:53:28.000000 cyberonix-3.0.2/cyberonix/main/tools/Cryptography.py
--rw-r--r--   0 root         (0) root         (0)    10863 2024-05-12 16:54:13.000000 cyberonix-3.0.2/cyberonix/main/tools/Exploitation_Tools.py
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-12 16:54:24.000000 cyberonix-3.0.2/cyberonix/main/tools/File_Upload.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-12 16:54:45.000000 cyberonix-3.0.2/cyberonix/main/tools/Framework.py
--rw-r--r--   0 root         (0) root         (0)    28866 2024-05-12 16:55:48.000000 cyberonix-3.0.2/cyberonix/main/tools/Password_Hacking.py
--rw-r--r--   0 root         (0) root         (0)     4881 2024-05-12 17:47:09.000000 cyberonix-3.0.2/cyberonix/main/tools/Pentesting_Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)    16476 2024-05-12 16:56:09.000000 cyberonix-3.0.2/cyberonix/main/tools/PostExploitationAttacks.py
--rw-------   0 root         (0) root         (0)   169451 2024-05-12 16:56:29.000000 cyberonix-3.0.2/cyberonix/main/tools/Recommended_Tool.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-05-12 16:56:38.000000 cyberonix-3.0.2/cyberonix/main/tools/RiskyFuncPayment.py
--rw-r--r--   0 root         (0) root         (0)     5204 2024-05-12 16:56:52.000000 cyberonix-3.0.2/cyberonix/main/tools/Secure_Transmission.py
--rw-r--r--   0 root         (0) root         (0)    11474 2024-05-12 16:58:23.000000 cyberonix-3.0.2/cyberonix/main/tools/Session_Management.py
--rw-r--r--   0 root         (0) root         (0)    10604 2024-05-12 16:58:33.000000 cyberonix-3.0.2/cyberonix/main/tools/Sniffing_and_Spoofing.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-05-12 16:58:54.000000 cyberonix-3.0.2/cyberonix/main/tools/Vulnerability_Analysis.py
--rw-r--r--   0 root         (0) root         (0)    13388 2024-05-12 16:59:05.000000 cyberonix-3.0.2/cyberonix/main/tools/WEB_Application_Analysis.py
--rw-r--r--   0 root         (0) root         (0)     6825 2024-05-12 16:59:16.000000 cyberonix-3.0.2/cyberonix/main/tools/Wireless_Hacking.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-12 17:00:57.000000 cyberonix-3.0.2/cyberonix/main/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-05-12 16:52:40.000000 cyberonix-3.0.2/cyberonix/main/tools/banner.py
--rw-r--r--   0 root         (0) root         (0)      207 2024-03-14 18:35:27.000000 cyberonix-3.0.2/cyberonix/main/tools/colors.py
--rw-r--r--   0 root         (0) root         (0)    27128 2024-05-12 16:53:49.000000 cyberonix-3.0.2/cyberonix/main/tools/data_validation.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-05-12 16:53:59.000000 cyberonix-3.0.2/cyberonix/main/tools/dos.py
--rw-r--r--   0 root         (0) root         (0)     4864 2024-05-12 16:54:31.000000 cyberonix-3.0.2/cyberonix/main/tools/forensic.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-05-12 16:55:06.000000 cyberonix-3.0.2/cyberonix/main/tools/html5.py
--rw-r--r--   0 root         (0) root         (0)    18178 2024-05-12 16:55:28.000000 cyberonix-3.0.2/cyberonix/main/tools/information_gathering.py
--rw-r--r--   0 root         (0) root         (0)      654 2024-03-14 18:35:27.000000 cyberonix-3.0.2/cyberonix/main/tools/run_on_browser.py
--rw-r--r--   0 root         (0) root         (0)    16803 2024-05-12 16:58:45.000000 cyberonix-3.0.2/cyberonix/main/tools/template.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-03-14 18:35:27.000000 cyberonix-3.0.2/cyberonix/main/tools/waiting.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-12 16:59:26.000000 cyberonix-3.0.2/cyberonix/main/tools/writeup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:49:00.737998 cyberonix-3.0.2/cyberonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:49:00.000000 cyberonix-3.0.2/cyberonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-12 17:49:00.000000 cyberonix-3.0.2/cyberonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 17:49:00.000000 cyberonix-3.0.2/cyberonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-12 17:49:00.000000 cyberonix-3.0.2/cyberonix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-12 17:49:00.000000 cyberonix-3.0.2/cyberonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-12 17:49:00.000000 cyberonix-3.0.2/cyberonix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 17:49:00.761998 cyberonix-3.0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1337 2024-05-12 17:48:45.000000 cyberonix-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.646157 cyberonix-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:12:55.646157 cyberonix-3.0.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.638157 cyberonix-3.0.3/cyberonix/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.3/cyberonix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13585 2024-05-21 04:11:30.000000 cyberonix-3.0.3/cyberonix/cyberonix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.638157 cyberonix-3.0.3/cyberonix/main/
+-rw-r--r--   0 root         (0) root         (0)    24214 2024-05-21 04:01:49.000000 cyberonix-3.0.3/cyberonix/main/Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31514 2024-05-21 04:01:32.000000 cyberonix-3.0.3/cyberonix/main/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-05-21 04:01:59.000000 cyberonix-3.0.3/cyberonix/main/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.642157 cyberonix-3.0.3/cyberonix/main/tools/
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-21 04:02:32.000000 cyberonix-3.0.3/cyberonix/main/tools/Anonymity.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-05-21 04:02:42.000000 cyberonix-3.0.3/cyberonix/main/tools/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-21 04:02:52.000000 cyberonix-3.0.3/cyberonix/main/tools/Authorization.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2024-05-21 04:03:15.000000 cyberonix-3.0.3/cyberonix/main/tools/Configuration_Management.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-21 04:03:30.000000 cyberonix-3.0.3/cyberonix/main/tools/Cryptography.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2024-05-21 04:04:02.000000 cyberonix-3.0.3/cyberonix/main/tools/Exploitation_Tools.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-21 04:04:11.000000 cyberonix-3.0.3/cyberonix/main/tools/File_Upload.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-21 04:04:36.000000 cyberonix-3.0.3/cyberonix/main/tools/Framework.py
+-rw-r--r--   0 root         (0) root         (0)    28889 2024-05-21 04:05:17.000000 cyberonix-3.0.3/cyberonix/main/tools/Password_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2024-05-21 04:05:32.000000 cyberonix-3.0.3/cyberonix/main/tools/Pentesting_Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)    16560 2024-05-21 04:05:45.000000 cyberonix-3.0.3/cyberonix/main/tools/PostExploitationAttacks.py
+-rw-r--r--   0 root         (0) root         (0)   171224 2024-05-21 04:05:55.000000 cyberonix-3.0.3/cyberonix/main/tools/Recommended_Tool.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-21 04:06:19.000000 cyberonix-3.0.3/cyberonix/main/tools/RiskyFuncPayment.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2024-05-21 04:06:31.000000 cyberonix-3.0.3/cyberonix/main/tools/Secure_Transmission.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2024-05-21 04:06:42.000000 cyberonix-3.0.3/cyberonix/main/tools/Session_Management.py
+-rw-r--r--   0 root         (0) root         (0)    10736 2024-05-21 04:06:51.000000 cyberonix-3.0.3/cyberonix/main/tools/Sniffing_and_Spoofing.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-05-21 04:07:13.000000 cyberonix-3.0.3/cyberonix/main/tools/Vulnerability_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)    13445 2024-05-21 04:07:26.000000 cyberonix-3.0.3/cyberonix/main/tools/WEB_Application_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-21 04:07:40.000000 cyberonix-3.0.3/cyberonix/main/tools/Wireless_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-21 04:03:01.000000 cyberonix-3.0.3/cyberonix/main/tools/banner.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    27322 2024-05-21 04:03:43.000000 cyberonix-3.0.3/cyberonix/main/tools/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)     5787 2024-05-21 04:03:52.000000 cyberonix-3.0.3/cyberonix/main/tools/dos.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-05-21 04:04:21.000000 cyberonix-3.0.3/cyberonix/main/tools/forensic.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-05-21 04:04:48.000000 cyberonix-3.0.3/cyberonix/main/tools/html5.py
+-rw-r--r--   0 root         (0) root         (0)    18178 2024-05-21 04:05:05.000000 cyberonix-3.0.3/cyberonix/main/tools/information_gathering.py
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/run_on_browser.py
+-rw-r--r--   0 root         (0) root         (0)    16802 2024-05-21 04:07:02.000000 cyberonix-3.0.3/cyberonix/main/tools/template.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-17 14:30:27.000000 cyberonix-3.0.3/cyberonix/main/tools/waiting.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-21 04:07:51.000000 cyberonix-3.0.3/cyberonix/main/tools/writeup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:12:55.638157 cyberonix-3.0.3/cyberonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 04:12:55.000000 cyberonix-3.0.3/cyberonix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 04:12:55.646157 cyberonix-3.0.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2024-05-21 03:37:54.000000 cyberonix-3.0.3/setup.py
```

### Comparing `cyberonix-3.0.2/PKG-INFO` & `cyberonix-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.2
+Version: 3.0.3
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
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.2 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.3 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-3.0.2/README.md` & `cyberonix-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/cyberonix.py` & `cyberonix-3.0.3/cyberonix/cyberonix.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,22 @@
     os.system("clear")
     banner.main()
     print("\033[38;5;105m","[+] Thanks visit again".title())
     exit()
 
 try:
     def starting():
+        try:
+                subprocess.run('sudo mv cyberonix.1 /usr/local/man/man1/',shell=True, check = True)
+        except Exception as err:
+                try:
+			subprocess.run('sudo mv cyberonix/cyberonix.1 /usr/local/man/man1/',shell=True, check = True)
+		except:
+			pass
+        #os.system("sudo mv cyberonix.1 /usr/local/man/man1/")
         parser = argparse.ArgumentParser(
             description="Cyberonix is a complete resource hub for Cyber Security Community. Our aim is to make this tool an 1 stop solution for all the Hackers out there to get resources of various topics in Cyber Security. We will keep updating this tool & adding new & updated resources on the go.",
         )
         main_args = parser.add_argument_group('Main Arguments')
             
         main_args.add_argument(
             "--tools", "-t",type=str,help=": Access various cybersecurity tools."
@@ -159,15 +167,15 @@
                     arguments.remove_dublicates(location=args.file, output=args.output)
                 else:
                     arguments.remove_dublicates(location=args.file)
 
             else:
                 print(
                     f"{colors.red}[!] Please enter file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
-)
+                )
 
         elif args.asnrecord:
             if args.file:
                 if args.output:
                     arguments.asnrecord(path=args.file, output=args.output)
                 else:
                     arguments.asnrecord(path=args.file)
@@ -252,37 +260,33 @@
                         arguments.dnsrecords(url=args.domain, names=args.record)
                 else:
                     print("please give --record also")
         else:
             main()
 
     def main():
-        #update()
-        os.system("chmod +x *")
+        #os.system("chmod +x *")
         proc = subprocess.Popen([f"id"], stdout=subprocess.PIPE, shell=True)
         #there keyfor success output and noththere for error output
         (there, notthere) = proc.communicate()
         there=there.decode()
         if "root" not in there:
             try:
                 subprocess.run('sudo cyberonix',shell=True, check = True)
             except Exception as err:
-                os.system("sudo python3 cyberonix.py")
+                os.system("cyberonix")
             # os.system("sudo cyberonix")
             exit()
         while True:
             os.system("clear")
             banner.main()
             list_attacks=["TOOLS","CHEATSHEET","Bug Bounty","Certifications & Roadmap","Write Ups","Man Page","exit"]
             for i in range(len(list_attacks)):
                 print(colors.options,f"{i+1}) {list_attacks[i]}".title(),colors.reset)
-            try:
-                option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
-            except KeyboardInterrupt:
-                exit_program()
+            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
             if option=="1":
                 os.system("clear")
                 tool.main()
             elif option=="2":
                 run_on_browser.main("https://github.com/defronixpro/Defronix-Cybersecurity-Roadmap/blob/main/cheatsheet.md")
             elif option == "3":
                 os.system("clear")
```

### Comparing `cyberonix-3.0.2/cyberonix/main/Bug_Bounty.py` & `cyberonix-3.0.3/cyberonix/main/Bug_Bounty.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bs4 import BeautifulSoup
 
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Bug Bounty")
-        list_root_attacks = ["Bug Bounty Videos Series","Reconnaissance", "Intel Discovery", "Enumeration","Vulnerability Analysis","Exploitation","Reporting", "go back"]
+        list_root_attacks = ["Bug Bounty Video Series","Reconnaissance", "Intel Discovery", "Enumeration","Vulnerability Analysis","Exploitation","Reporting", "go back"]
         for i in range(len(list_root_attacks)):
             print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
             return
         if option == "1":
@@ -126,15 +126,15 @@
                      break
 
         elif option == "3":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Discovery tools")
-                banner.description("")
+                banner.description("Intel Discovery in the context of bug bounty refers to Intel's bug bounty program, which aims to identify and address security vulnerabilities in their products. Researchers and ethical hackers are invited to discover and report security flaws in Intel hardware, software, and firmware. In return, they may receive monetary rewards, recognition, and the opportunity to help improve the security of Intel products. The program emphasizes responsible disclosure, meaning vulnerabilities should be reported privately to Intel to allow them to fix the issues before public disclosure.")
                 list_root_attacks = ["Burpsuite\t\t(Recommended)","Owasp Zap\t\t(Recommended)","Nessus\t\t(Recommended)","Metasploit framework(Recommended)", "Dirb ","Dirsearch ","Gobuster\t\t(Recommended) ","go back"]
                 for i in range(len(list_root_attacks)):
                     print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     return
@@ -163,15 +163,15 @@
                      break
                 
         elif option == "4":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Enumeration")
-                banner.description("")
+                banner.description("Enumeration in bug bounty refers to the process of systematically gathering information about a target system to identify potential entry points for exploitation. This can include discovering subdomains, open ports, services running on those ports, directories, files, and user accounts. Enumeration is a crucial step in the reconnaissance phase of a bug bounty program, as it helps bug hunters map the attack surface and uncover vulnerabilities that can be exploited.")
                 list_root_attacks = ["Nmap\t\t(Recommended)","Unicornscan","Masscan\t\t(Recommended)","Nikto ","DNSRecon\t\t(Recommended)","go back"]
                 for i in range(len(list_root_attacks)):
                     print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     return
@@ -194,15 +194,15 @@
                      break
 
         elif option == "5":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Vulnerability Analysis")
-                banner.description("")
+                banner.description("Vulnerability Analysis in bug bounty refers to the process of identifying, evaluating, and prioritizing security weaknesses in a target system. This involves examining the system's components, configurations, and code to find potential vulnerabilities that could be exploited by attackers. Bug hunters use various tools and techniques during this phase to detect issues such as SQL injection, cross-site scripting (XSS), and insecure configurations. The goal of vulnerability analysis is to understand the nature and impact of the discovered weaknesses, allowing for effective reporting and remediation.")
                 list_root_attacks = ["Wpscan","Burpsuite\t\t(Recommended)","OWASP ZAP\t\t(Recommended)","Nessus\t\t(Recommended)","Sqlmap\t\t(Recommended)","go back"]
                 for i in range(len(list_root_attacks)):
                     print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     return
@@ -225,31 +225,31 @@
                      break
                 
         elif option == "6":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Exploitation")
-                banner.description("")
-                list_root_attacks = ["Crackmapexec\t(Recommended)","Masscan","Beef-XSS\t\t(Recommended)","Social Engineering Toolkit","PowerSploit","Mimikatz\t\t(Recommended)","go back"]
+                banner.description("Exploitation in bug bounty refers to the phase where a bug hunter attempts to leverage identified vulnerabilities to execute attacks on a target system. The objective is to demonstrate the practical impact of a vulnerability, such as gaining unauthorized access, escalating privileges, or exfiltrating sensitive data. This step often involves crafting and executing specific exploits to prove that the vulnerability can be used in a real-world scenario. Successful exploitation helps validate the severity of the vulnerability, guiding the target organization on necessary remediation actions.")
+                list_root_attacks = ["Crackmapexec\t(Recommended)","Masscan","Beef\t\t(Recommended)","Social Engineering Toolkit","PowerSploit","Mimikatz\t\t(Recommended)","go back"]
                 for i in range(len(list_root_attacks)):
                     print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     return
                 if ask == "1":
                     print("\n[+] Crackmapexec")
                     Exploitation_Tools.crackmapexec()
                 elif ask == "2":
                     print("\n[+] Masscan")
                     masscan()
                 elif ask == "3":
-                    print("\n[+] Beef")
-                    Exploitation_Tools.beef
+                    print("\n[+] beef")
+                    Exploitation_Tools.beef()
                 elif ask == "4":
                     print("\n[+]Social Engineering Toolkit")
                     Password_Hacking.setoolkit()
                 elif ask == "5":
                     print("\n[+]powersploit")
                     powersploit()               
                 elif ask == "6":
@@ -262,15 +262,15 @@
                      break   
 
         elif option == "7":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Reporting Tools")
-                banner.description("")
+                banner.description("Reporting tools in bug bounty are specialized software or platforms that help bug hunters document and submit their findings to the target organization. These tools facilitate the structured reporting of vulnerabilities, including details such as the type of vulnerability, steps to reproduce it, potential impact, and suggested mitigations. ")
                 list_root_attacks = ["Dradis","CherryTree\t\t(Recommended)","faradaystart","recordmydesktop ","pipal","maltego\t\t(Recommended)","go back"]
                 for i in range(len(list_root_attacks)):
                     print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     return
@@ -295,15 +295,15 @@
                 else:
                      break  
         else:
             return            
 
 def recordmydesktop():
     os.system("clear")
-    github ="recordmydesktop application produces an ogg-encapsulated theora-vorbis file. recordMyDesktop tries to be as unobstrusive as possible by proccessing only regions of the screen that have changed"
+    github ="recordmydesktop application produces an ogg-encapsulated theora-vorbis file. recordMyDesktop tries to be as unobstrusive as possible by proccessing only regions of the screen that have changed."
     template.template("recordmydesktop","recordmydesktop --help",github.strip(),{"How to record screencasts with recordMyDesktop":"https://opensource.com/business/15/11/how-record-screencasts","recordmydesktop Tool help file":"https://www.kali.org/tools/recordmydesktop/",})
                 
 def faraday():
     os.system("clear")
     github ="Faraday introduces a new concept (IPE) Integrated Penetration-Test Environment a multiuser Penetration test IDE. Designed for distribution, indexation and analysis of the generated data during the process of a security audit."  
     template.template("faraday","faraday --help",github.strip(),{"faraday Tool Documentation":"https://www.kali.org/tools/python-faraday/#tool-documentation","How to scan web sites with Faraday IDE on Kali Linux":"https://www.securityhardening.com/library/Article33.pdf",})
```

### Comparing `cyberonix-3.0.2/cyberonix/main/arguments.py` & `cyberonix-3.0.3/cyberonix/main/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,38 +177,27 @@
         passwords = [
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/xato-net-10-million-passwords.txt",
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Common-Credentials/10-million-password-list-top-1000000.txt",
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Common-Credentials/10-million-password-list-top-100000.txt",
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/xato-net-10-million-passwords-1000000.txt",
         ]
         for link in range(len(passwords)):
-            try:
-                pass_check(passwords[link], result_str, link)
-            except KeyboardInterrupt:
-                exit_program()
+            pass_check(passwords[link], result_str, link)
 
 
 def pass_check(url, password, number):
         print(f"{colors.blue}Test {number}{colors.reset}")
-        try:
-            raw = requests.get(url)
-            lists = raw.text.split("\n")
-            for i in lists:
-                if password == i:
-                    print(f"{colors.red}FAILED{colors.reset}")
-            else:
-                print(f"{colors.green}PASSED{colors.reset}")
-
-        except KeyboardInterrupt:
-                exit_program()
-        except Exception as err:
-            os.system("clear")
-            banner.main()
-            banner.attack(f"{colors.red}ERROR{colors.reset}")
-            banner.description(f"{colors.red}{err}{colors.reset}")
+        raw = requests.get(url)
+        lists = raw.text.split("\n")
+        for i in lists:
+            if password == i:
+                print(f"{colors.red}FAILED{colors.reset}")
+        else:
+            print(f"{colors.green}PASSED{colors.reset}")
+
 
 def exit_program():
     print("\033[38;5;105m", "[+] Thanks visit again".title())
     exit()
 
 
 def asnrecord(path="", url="", output=""):
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tool.py` & `cyberonix-3.0.3/cyberonix/main/tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Anonymity.py` & `cyberonix-3.0.3/cyberonix/main/tools/Anonymity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 from cyberonix.main.tools import banner, colors, template, banner,Recommended_Tool
 import os
 import requests
 from bs4 import BeautifulSoup
 import subprocess
 
+def check_tor_installed():
+    try:
+        # Run the 'which tor' command
+        result = subprocess.run(['which', 'tor'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        
+        # Decode the output from bytes to string
+        output = result.stdout.decode().strip()
+        
+        if output:
+            return
+        else:
+            os.system("apt install tor -y")     # for tor installation
+    except Exception as e:
+        print("An error occurred:", str(e))
+
+
+
+
 
 def main():
     
     while True:
         
         os.system("clear")
         banner.main()
@@ -19,14 +37,15 @@
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
             return
         if option == "1":
             os.system("clear")
             banner.main()
             banner.attack("Tor")
+            check_tor_installed()  # Check if Tor is installed
             Recommended_Tool.recommended("tor")
 
         elif option == "2":
             print("\n[+] Anonsurf")
             anonsurf()
         elif option == "3":
             print("\n[+] ProxyChains ")
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Authentication.py` & `cyberonix-3.0.3/cyberonix/main/tools/Authentication.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Authorization.py` & `cyberonix-3.0.3/cyberonix/main/tools/Authorization.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Configuration_Management.py` & `cyberonix-3.0.3/cyberonix/main/tools/Configuration_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Cryptography.py` & `cyberonix-3.0.3/cyberonix/main/tools/Cryptography.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Exploitation_Tools.py` & `cyberonix-3.0.3/cyberonix/main/tools/Exploitation_Tools.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/File_Upload.py` & `cyberonix-3.0.3/cyberonix/main/tools/File_Upload.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Password_Hacking.py` & `cyberonix-3.0.3/cyberonix/main/tools/Password_Hacking.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     template.template("set", "setoolkit", github.strip(), {"Phishing using SET": "https://www.golinuxcloud.com/social-engineering-toolkit-phishing/",
                                       "Phishing using SET by Hengky Sanjaya": "https://medium.com/hengky-sanjaya-blog/social-engineering-toolkit-set-23be8b66aa18"})
 
 
 def hiddeneye():
     github = "HiddenEye is a modern phishing tool with advanced functionality. It is written in Python and can be run on Windows, Linux, and Mac OS X. It allows you to perform various phishing attacks."
     template.template("HiddenEye", "python HiddenEye.py", github.strip(), {"HiddenEye by GeeksForGeeks": "https://www.geeksforgeeks.org/hiddeneye-modern-phishing-tool-with-advanced-functionality/", "HiddenEye by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/",
-                                      "HiddenEye by Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"}, method="github", github_install="git clone https://github.com/Morsmalleo/HiddenEye && cd HiddenEye && pip install -r requirements.txt", github_check="HiddenEye")
+                                      "HiddenEye by Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"}, method="github", github_install="git clone https://github.com/Morsmalleo/HiddenEye && cd HiddenEye && pip install -r requirements.txt && pip install pyngrok", github_check="HiddenEye")
 def r3bu5():
     github = "It is a Phishing tool that has latest and updated login pages, Mask URL support, Beginners Friendly, Multiple tunneling options"
     template.template("r3bu5", "./r3bu5.sh", github.strip(), {"Github Repo of r3bu5": " https://github.com/k46-db0y/r3bu5"}, method="github",
                                       github_install="git clone https://github.com/k46-db0y/r3bu5.git && cd r3bu5 && chmod +x r3bu5.sh", github_check="r3bu5")
         
 def zphisher():
     github = "Zphisher is an open-source phishing tool that automates the process of creating and deploying phishing pages. It allows users to easily create phishing pages for various popular websites, such as Google, Facebook, and LinkedIn, and can be used to perform phishing attacks on targeted individuals or organizations. It can also be used to test the security awareness of an organization's employees. Zphisher is written in Shell Script and it's available for Linux and Termux."
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Pentesting_Bug_Bounty.py` & `cyberonix-3.0.3/cyberonix/main/tools/Pentesting_Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/PostExploitationAttacks.py` & `cyberonix-3.0.3/cyberonix/main/tools/PostExploitationAttacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,26 +110,26 @@
         
 def beroot():
     os.system("clear")
     github_text_0 = github_getting_text(
                 "https://github.com/AlessandroZ/BeRoot", 'p[dir=auto]', 0)
     github_text_1 = github_getting_text(
                 "https://github.com/AlessandroZ/BeRoot", 'p[dir=auto]', 1)
-    github = github_text_0 + github_text_1
+    github = github_text_0.strip().replace("\n", "").replace("\t", "") + github_text_1.strip().replace("\n", "").replace("\t", "")
     template.template("BeRoot", "cd Linux && chmod u+x * && ./beroot.py", github.strip(), {"BeRoot-Linux-Privilege-Escalation": "https://www.kitploit.com/2018/06/beroot-for-linux-privilege-escalation.html?m=0", "BeRoot-A-Post-Exploitation-Privilege-Escalation-Tool":
                               "https://blog.hackersonlineclub.com/2018/07/beroot-post-exploitation-tool-to-check.html", "BeRoot-Windows-Privilege-Escalation": "https://sevenlayers.com/index.php/273-windows-privilege-escalation"}, method="github", github_install="git clone https://github.com/AlessandroZ/BeRoot.git", github_check="BeRoot")
         
 def sudokiller():
     os.system("clear")
     github_text_6 = github_getting_text(
                 "https://github.com/TH3xACE/SUDO_KILLER", 'p[dir=auto]', 6)
     github_text_7 = github_getting_text(
                 "https://github.com/TH3xACE/SUDO_KILLER", 'p[dir=auto]', 7)
     github = github_text_6 + github_text_7
-    template.template("Sudo Killer", "chmod u+x * && ./SUDO_KILLERv2.4.2.sh", github.strip(), {"SUDO_KILLER-Demos": "https://github.com/TH3xACE/SUDO_KILLER#demos", "Sudo-Killer Information": "https://www.kitploit.com/2020/02/sudokiller-tool-to-identify-and-exploit.html",
+    template.template("Sudo Killer", "chmod u+x * && ./SUDO_KILLERv3.sh", github.strip(), {"SUDO_KILLER-Demos": "https://github.com/TH3xACE/SUDO_KILLER#demos", "Sudo-Killer Information": "https://www.kitploit.com/2020/02/sudokiller-tool-to-identify-and-exploit.html",
                               "Sudo-Killer-Identify-Abuse-Sudo-Misconfigurations": "https://null-byte.wonderhowto.com/how-to/use-sudo-killer-identify-abuse-sudo-misconfigurations-0202594"}, method="github", github_install="git clone https://github.com/TH3xACE/SUDO_KILLER.git", github_check="SUDO_KILLER")
         
 def linenum():
     os.system("clear")
     github = "LinEnum is a Linux enumeration script that can be used to enumerate information from a Linux system. It is designed to be run locally on a Linux system and will attempt to enumerate common files, folders, users, groups, services, configurations, and permissions. It can also be used to look for certain security vulnerabilities such as local privilege escalation. LinEnum can be run from the command line or can be automated using a script. The output of the script can be saved as a text file for later analysis."
     template.template("LinEnum", "chmod +x LinEnum.sh && ./LinEnum.sh -h", github.strip(), {"Use-LinEnum-Identify-Potential-Privilege-Escalation-Vectors": "https://null-byte.wonderhowto.com/how-to/use-linenum-identify-potential-privilege-escalation-vectors-0197225/", "Linux-Privilege-Escalation-With-LinEnum": "https://trevorxcohen.medium.com/linux-privilege-escalation-with-linenum-75d20a3b59f6", "LinEnum-Linux-Enumeration-Privilege-Escalation-Tool": "https://www.darknet.org.uk/2014/11/linenum-linux-enumeration-privilege-escalation-tool",
                               "Linux-Privilege-Escalation-Quick-And-Dirty": "https://reboare.gitbooks.io/booj-security/content/general-linux/privilege-escalation.html", "Linux Enumeration And Privilege Escalation – LinEnum": "https://vulners.com/n0where/N0WHERE:24819"}, method="github", github_install="curl -s https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh -o LinEnum.sh && mkdir LinEnum && mv LinEnum.sh LinEnum", github_check="LinEnum")
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Recommended_Tool.py` & `cyberonix-3.0.3/cyberonix/main/tools/Recommended_Tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cyberonix.main.tools import banner, waiting, writeup, colors, run_on_browser, Recommended_Tool,template
+from cyberonix.main.tools import banner, waiting, writeup, colors, run_on_browser, Recommended_Tool,template, Anonymity
 import os
 import readline
 targets = []
 # Function for recommmended tools
 def recommended(name):
     #print(f"{name}")
     if name.lower() == "nmap":
@@ -141,21 +141,25 @@
         anonsurf(name)
     elif name.lower() == "proxychains":
         print("proxychains is running...")
         os.system("proxychains firefox")
     elif name.lower() == "nipe":
         nipe(name)
     elif name.lower() == "tor":
+        
         tor(name)
 
 ###################################  configuration management #######################################################################
     elif name.lower() == "gobuster":
         gobuster(name)
     elif name.lower() == "securityheaders":
-        os.system("cd Tools/securityheaders && python3 securityheaders.py")
+        path = template.check_path("securityheaders")
+        os.chdir(path)
+        command_line("securityheaders","python3 securityheaders.py")
+
     elif name.lower() == "secretfinder":
         secretfinder(name)
     
     elif  name.lower() == "httpie":
         httpie(name)
     elif name.lower() == "feroxbuster":
         feroxbuster(name)
@@ -204,14 +208,15 @@
         os.system("ettercap -G")
 ###################################  File Upload  #######################################################################
 
     elif name.lower() == "fuxploider":
         fuxploider(name)
 ###################################  Risk func payment #######################################################################
     elif name.lower() == "fiddler":
+
         os.system("cd Tools/fiddler && mono Fiddler.exe")
 ###################################  NEW Bug BOUNTY SECITON #######################################################################
 ###################################  Exploitation #######################################################################
     elif name.lower() == "masscan":
         masscan(name)
     elif name.lower()  == "unicornscan":
         unicornscan(name)
@@ -254,35 +259,43 @@
                     else:
                         return 2
                 else:
                     return 2
             except Exception as e:
                 return 2       
 #command_line function
-def command_line(name):
+def command_line(name,command=""):
+    if command == "":
+        command=name
     try:
         template.load_banner(name)
-        command=""
-        while not command:
-            command = input(f"\n {colors.select}Enter a command : {colors.reset}")
-            if "exit" in command:
+        instruction=""
+        while not instruction:
+            instruction = input(f"\n {colors.select}Enter only command arguments : {colors.reset}")
+            instruction_sanitization = instruction.split()
+            if  instruction.lower() == "exit":
                 break
-            elif not command.strip(): 
-                template.load_banner(name)
-                continue
-            elif name not in command:
+            elif not instruction.strip(): 
                 template.load_banner(name)
-                print(f"\n{colors.red} please use only {name} command {colors.reset}\n")
-                command = None
                 continue
-            else:
-                template.load_banner(name)
-                os.system(command)
+
+
+# Check if there is at least one word
+            if len(instruction_sanitization) > 0:
+    # Access the string at index 0 using slicing
+    
+                if ( instruction_sanitization[0].lower() == command.lower()):
+                    print(f"\n{colors.red} E.g Don't include tool name/script before arguments {colors.reset}\n")
+    	
+                else:
+                    template.load_banner(name)
+                    os.system(f"{command} {instruction}")
+ 
     except KeyboardInterrupt:
-        return
+         return
     
 def change_target(name):
     try:
         template.load_banner(name)
         target = input(f"\n{colors.select}Enter a target : {colors.reset}")
         while not target:
             print(f"\n{colors.red} Please valid enter the target{colors.reset}\n")
@@ -1901,15 +1914,19 @@
                 print(colors.options,f"Finding Specific aspect of the system... ",colors.reset )
                 os.system(f"cd /usr/share/peass/linpeas && ./linpeas.sh -s suid") 
                 continue
             elif option== "3":
                 change_target(name)
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("LinPeas")
+                os.chdir(path)
+
+                command_line("LinPeas","bash linpeas.sh")
+
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -1946,15 +1963,20 @@
                 print(colors.options,f"Search for SUID/SGID files and binaries... ",colors.reset )
                 os.system(f"cd Tools/LinEnum && ./LinEnum.sh -t -k password -r –s") 
                 continue
             elif option== "5":
                 change_target(name)
                 continue
             elif option == "6":
-                command_line(name)
+                path = template.check_path("LinEnum")
+                os.chdir(path)
+               
+                print(path)
+                command_line("LinEnum","bash linEnum.sh")
+
                 continue
             elif option == "7":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -1968,27 +1990,30 @@
             for i in range(len(list_attacks)):
                 print(colors.options,f"{i+1}) {list_attacks[i]}".title(),colors.reset)
             option = input(f"\n {colors.select}Select a option -> {colors.reset}")
             
             if option == "1":
                 template.load_banner(name)
                 print(colors.options,f"Simple Scans is running... ",colors.reset )
-                os.system(f"cd Tools/SUDO_KILLER && chmod u+x * && ./SUDO_KILLERv2.4.2.sh ") 
+                os.system(f"cd Tools/SUDO_KILLER && chmod u+x * && ./SUDO_KILLERv3.sh ") 
                 continue
             elif option == "2":
                 template.load_banner(name)
                 print(colors.options,f"Potential vulnerabilities... ",colors.reset )
-                os.system(f"cd Tools/SUDO_KILLER && chmod u+x * && ./SUDO_KILLERv2.4.2.sh -p ") 
+                os.system(f"cd Tools/SUDO_KILLER && chmod u+x * && ./SUDO_KILLERv3.sh -p ") 
                 continue
             
             elif option== "3":
                 change_target(name)
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("SUDO_KILLER")
+                os.chdir(path)
+                command_line("SUDO_KILLER","sudo bash SUDO_KILLERv3.sh")
+
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2015,15 +2040,18 @@
                 os.system(f"cd Tools/linux-exploit-suggester-2 && ./linux-exploit-suggester-2.pl -k {kernel}") 
                 continue
             
             elif option== "3":
                 change_target(name)
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("linux-exploit-suggester-2")
+                os.chdir(path)
+                command_line("linux-exploit-suggester-2","./linux-exploit-suggester-2.pl -h")
+
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2054,15 +2082,18 @@
                 print(colors.options,f"Check for writable configuration files... ",colors.reset )
                 os.system(f"cd Tools/linux-smart-enumeration &&./lse.sh -c") 
                 continue
             elif option== "4":
                 change_target(name)
                 continue
             elif option == "5":
-                command_line(name)
+                path = template.check_path("linux-smart-enumeration")
+                os.chdir(path)
+                command_line("linux-smart-enumeration","./lse.sh -c")
+
                 continue
             elif option == "6":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2093,15 +2124,18 @@
                 print(colors.options,f"Monitor specific process... ",colors.reset )
                 os.system(f"cd Tools/PSPY && ./pspy64  | grep {process}") 
                 continue
             elif option== "4":
                 change_target(name)
                 continue
             elif option == "5":
-                command_line(name)
+                path = template.check_path("PSPY")
+                os.chdir(path)
+                command_line("PSPY"," ./pspy64")
+
                 continue
             elif option == "6":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2131,15 +2165,18 @@
             elif option == "3":
                 template.load_banner(name)
                 file = input(f"\n {colors.select} Enter path of file :  {colors.reset}")
                 print(colors.options,f"Custom compression level... ",colors.reset )
                 os.system(f"cd Tools/upx-4.0.1-i386_linux && chmod u+x upx && ./upx -o2 {file}")
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("upx-4.0.1-i386_linux")
+                os.chdir(path)
+                command_line("upx-4.0.1-i386_linux","./upx")
+
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2469,15 +2506,18 @@
                 path = template.check_path("SecretFinder")
                 print(f"\nOutput saved to {path}/result.txt")
                 continue
             elif option== "3":
                 change_target(name)
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("SecretFinder")
+                os.chdir(path)
+
+                command_line("SecretFinder","python3 SecretFinder.py")
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2519,28 +2559,31 @@
                 template.load_banner(name)
                 print(colors.options,f"xsstrike is running...",colors.reset )
                 os.system(f"cd Tools/XSStrike && python3 xsstrike.py -u '{targets[0]}' --crawl --level 3") 
             elif option=="5":
                 change_target(name)
                 continue
             elif option == "6":
-                command_line(name)
+                path = template.check_path("XSStrike")
+                os.chdir(path)
+                command_line("XSStrike","python3 xsstrike.py")
+
                 continue
             elif option == "7":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
 
 
 def dalfox(name):
     try:
         template.load_banner(name)
-        s.system("dalfox -h") 
+        os.system("dalfox -h") 
         while True:
             list_attacks=["Command Line","Open this for Best Commands(link to website)","Output handling(link to website)","Parameter Analysis and XSS Scanning(link to website)","Scanning single url's(link to website)","exit"]
             for i in range(len(list_attacks)):
                 print(colors.options,f"{i+1}){list_attacks[i]}".title(),colors.reset)
             option = input(f"\n {colors.select}Select a option -> {colors.reset}")
             
             if option == "1":
@@ -2593,15 +2636,18 @@
                 print(colors.options,f"Oralyzer is running...",colors.reset )
                 os.system(f"python3 oralyzer.py -u {targets[0]}") 
                 continue
             elif option== "3":
                 change_target(name)
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("Oralyzer")
+                os.chdir(path)
+                command_line("Oralyzer","python3 oralyzer.py")
+
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2638,15 +2684,18 @@
                 path = template.check_path("OpenRedireX")
                 print(f"\nOutput saved to {path}/result.txt")
                 continue
             elif option== "3":
                 change_target(name)
                 continue
             elif option == "4":
-                command_line(name)
+                path = template.check_path("OpenRedireX")
+                os.chdir(path)
+                command_line("OpenRedireX","python3 openredirex.py")
+
                 continue
             elif option == "5":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
@@ -2708,39 +2757,39 @@
             
             if option == "1":
                 template.load_banner(name)
                 sleeptime = input("\nEnter how much sleeptime between requests (like 60): ")
                 port = input("\nEnter the port number: ")
                 socket  = input("\nEnter how many socket you want to add  (like 600): ")
                 print(colors.options,f"Slowloris is running...",colors.reset )
-                os.system(f"cd Tools/slowloris && python3 slowloris.py {targets[0]} -s {socket} -p {port} -v -ua --sleeptime {sleeptime}") 
+                os.system(f"slowloris {targets[0]} -s {socket} -p {port} -v -ua --sleeptime {sleeptime}") 
                 continue
             elif option == "2":
                 template.load_banner(name)
                 sleeptime = input("\nEnter how much sleeptime between requests (like 60): ")
                 port = input("\nEnter the port number: ")
                 socket  = input("\nEnter how many socket you want to add  (like 600): ")
                 proxyhost = input("\nEnter proxy IP: ")
                 proxyport = input("\nEnter proxy port number: ")
                 print(colors.options,f"Slowloris is running...",colors.reset )
-                os.system(f"cd Tools/slowloris && python3 slowloris.py {targets[0]} -s {socket} -p {port} -v --proxy-host {proxyhost} --proxy-port {proxyport} --sleeptime {sleeptime}") 
+                os.system(f"slowloris {targets[0]} -s {socket} -p {port} -v --proxy-host {proxyhost} --proxy-port {proxyport} --sleeptime {sleeptime}") 
                 continue
             elif option == "3":
                 template.load_banner(name)
                 port = input("\nEnter the port number: ")
                 socket  = input("\nEnter how many socket you want to add  (like 600): ")
                 print(colors.options,f"Slowloris is running...",colors.reset )
-                os.system(f"cd Tools/slowloris && python3 slowloris.py {targets[0]} -s {socket} -p {port} -ua") 
+                os.system(f"slowloris {targets[0]} -s {socket} -p {port} -ua") 
                 continue
             elif option == "4":
                 template.load_banner(name)
                 port = input("\nEnter the port number: ")
                 socket  = input("\nEnter how many socket you want to add  (like 600): ")
                 print(colors.options,f"Slowloris is running...",colors.reset )
-                os.system(f"cd Tools/slowloris && python3 slowloris.py {targets[0]} --https -s {socket} -p {port} -ua") 
+                os.system(f"slowloris {targets[0]} --https -s {socket} -p {port} -ua") 
                 continue
             elif option== "5":
                 change_target(name)
                 continue
             elif option == "6":
                 command_line(name)
                 continue
@@ -3083,15 +3132,18 @@
                 print(colors.options,f"Advanced Scan with Proxy and Cookies...",colors.reset )
                 os.system(f"cd Tools/fuxploider && python3 fuxploider.py --cookies \"PHPSESSID=aef45aef45afeaef45aef45&JSESSID=AQSEJHQSQSG\" --not-regex \"error\" -u {targets[0]} -v ")
                 continue
             elif option== "4":
                 change_target(name)
                 continue
             elif option == "5":
-                command_line(name)
+                path = template.check_path("fuxploider")
+                os.chdir(path)
+                command_line("fuxploider","python3 fuxploider.py")
+
                 continue
             elif option == "6":
                 break
             else:
                 break
     except KeyboardInterrupt:
         return
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/RiskyFuncPayment.py` & `cyberonix-3.0.3/cyberonix/main/tools/RiskyFuncPayment.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Secure_Transmission.py` & `cyberonix-3.0.3/cyberonix/main/tools/Secure_Transmission.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Session_Management.py` & `cyberonix-3.0.3/cyberonix/main/tools/Session_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Sniffing_and_Spoofing.py` & `cyberonix-3.0.3/cyberonix/main/tools/Sniffing_and_Spoofing.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                         " Responder", " Airgeddon",  "Wifi-Pumpkin-3\t(Recommended)", "mitmproxy\t\t(Recommended) ", "zaproxy ", "Go Back"]
         for i in range(len(list_attacks)):
             print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
             return
-        if option == "0":
+        if option == "1":
             print("\n[+] Wireshark")
             Vulnerability_Analysis.wireshark()
         elif option == "2":
             print("\n[+] Bettercap")
             bettercap()
         elif option == "3":
             print("\n[+] Tcpdump")
@@ -95,15 +95,15 @@
     os.system("clear")
     github_text_0 = github_getting_text(
                 "http://netsniff-ng.org/", 'p', 0)
     github_text_1 = github_getting_text(
                 "http://netsniff-ng.org/", 'p', 1)
     github_text_2 = github_getting_text(
                 "http://netsniff-ng.org/", 'p', 2)
-    github = github_text_0 + github_text_1 + github_text_2
+    github = github_text_0.strip().replace("\n", "").replace("\t", "") + github_text_1.strip().replace("\n", "").replace("\t", "") + github_text_2.strip().replace("\n", "").replace("\t", "")
     template.template("netsniff-ng", "netsniff-ng -h", github.strip(), {"Netsniff-ng Website": "http://netsniff-ng.org/", "Sniffing Network Traffic": "https://medium.com/purple-team/sniffing-network-traffic-with-netsniff-ng-55b8f5d436c2",
                               "Manual": "https://linux.die.net/man/8/netsniff-ng", "Video Resources": "https://www.irongeek.com/i.php?page=videos/hack3rcon4/09-netsniff-ng-jon-schipp"})
         
 def macchanger():
     os.system("clear")
     github_fetch = github_getting_text(
                 "https://www.kali.org/tools/macchanger/", 'p', 0)
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Vulnerability_Analysis.py` & `cyberonix-3.0.3/cyberonix/main/tools/Vulnerability_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/WEB_Application_Analysis.py` & `cyberonix-3.0.3/cyberonix/main/tools/WEB_Application_Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from cyberonix.main.tools import banner, colors, template, waiting, writeup, Configuration_Management
 import os
 import requests
 import requests
+import re
 from bs4 import BeautifulSoup
 
 
 def main():
     while True:
         os.system("clear")
         banner.main()
@@ -143,15 +144,15 @@
             template.uninstall_tool("","burp")
         else:
             break
 
 
 def owasp_zap():
     os.system("clear")
-    github = "The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.\nIt is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox. https://www.owasp.org/index.php/ZAP"
+    github = "The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.It is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox. https://www.owasp.org/index.php/ZAP"
     template.template('zaproxy', 'zaproxy', github.strip(), {"How to setup OWASP ZAP to scan your web application for security vulnerabilities": "https://www.linkedin.com/pulse/how-setup-owasp-zap-scan-your-web-application-security-botla/", "Authenticated Scan using OWASP-ZAP in Windows.": "https://medium.com/@secureica/authenticated-scan-using-owasp-zap-f0a71dafe41",
                       "OWASP ZAP: 6 Key Capabilities and a Quick Tutorial": "https://www.hackerone.com/knowledge-center/owasp-zap-6-key-capabilities-and-quick-tutorial", "Initial Setup": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/untitled", "Setup OWASP ZAP": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/setup-owasp-zap"})
 
 
 def nessus():
     os.system("clear")
     version_grab = github_getting_text("https://www.tenable.com/downloads/nessus?loginAttempted=true",
@@ -176,13 +177,14 @@
     template.template("dirsearch", "dirsearch --help ", github.strip(), {"Dirserach helpfile": "https://www.kali.org/tools/dirsearch/",
                       "Find Hidden Web Directories with Dirsearch ": "https://null-byte.wonderhowto.com/how-to/find-hidden-web-directories-with-dirsearch-0201615/", })
 
 
 def wapiti():
     os.system("clear")
     github = github_getting_text("https://wapiti-scanner.github.io/", 'p', 6)
+    github = re.sub(r'\s+', ' ', github).strip()
     template.template("wapiti", "wapiti", github.strip(), {"wapiti free web application vulnerability scanner": "https://pentestit.medium.com/wapiti-free-web-application-vulnerability-scanner-ce7712adf644", "Official docs": "https://github.com/wapiti-scanner/wapiti", "wapiti tutorial":
                       "https://www.kalilinux.in/2021/01/wapiti-tutorial.html", "complete guide to using wapiti web vulnerability scanner to keep your web applications websites secure": "https://linuxsecurity.com/features/complete-guide-to-using-wapiti-web-vulnerability-scanner-to-keep-your-web-applications-websites-secure"})
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/Wireless_Hacking.py` & `cyberonix-3.0.3/cyberonix/main/tools/Wireless_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/banner.py` & `cyberonix-3.0.3/cyberonix/main/tools/banner.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/data_validation.py` & `cyberonix-3.0.3/cyberonix/main/tools/data_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
                 ask = vuln_options()
                 if ask == "1":
                     while True:
                         os.system("clear")
                         banner.main()
                         banner.attack("XSS")
-                        des = "It is recommended to test manually for XSS vulnerability to get better understanding & results.\nCheck out the writeup section to to learn about Cross Site Scripting"
+                        des = "It is recommended to test manually for XSS vulnerability to get better understanding & results.Check out the writeup section to to learn about Cross Site Scripting"
                         banner.description(des)
                         list_tools = ["Dalfox", "XSStrike", "Xsser", "go back"]
                         for i in range(len(list_tools)):
                             print(
                                 colors.options,
                                 f"{i+1}) {list_tools[i]}".title(),
                                 colors.reset,
@@ -239,15 +239,15 @@
                 # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
                 ask = vuln_options()
                 if ask == "1":
                     while True:
                         os.system("clear")
                         banner.main()
                         banner.attack("Open Redirection")
-                        des = "It is recommended to test manually for Open Redirection to get better understanding & results.\nCheck out the writeup section to to learn about Open Redirection"
+                        des = "It is recommended to test manually for Open Redirection to get better understanding & results.Check out the writeup section to to learn about Open Redirection"
                         banner.description(des)
                         list_tools = ["OpenRedireX", "Oralyzer", "go back"]
                         for i in range(len(list_tools)):
                             print(
                                 colors.options,
                                 f"{i+1}) {list_tools[i]}".title(),
                                 colors.reset,
@@ -361,17 +361,18 @@
                                 link="https://github.com/devanshbatham/OpenRedireX",
                                 method="github",
                                 github_install="git clone https://github.com/devanshbatham/OpenRedireX.git",
                                 github_check="OpenRedireX",
                             )
 
 def xsser():
-    github = github_getting_text(
+    github_p1 = github_getting_text(
                                 "https://www.kali.org/tools/xsser/", "p", 3
                             )
+    github = github_p1.strip().replace("\n", "").replace("\t", "")
     template.template(
                                 "xsser",
                                 "xsser -h",
                                 github.strip(),
                                 {
                                     "Detecting and Exploiting XSS Injections using XSSer Tool": "https://securityxploded.com/detecting-exploiting-xss-using-xsser-tool.php",
                                     "XSSer - Detect and Exploit XSS vulnerabilities": "https://gbhackers.com/xsser-automated-framework-detectexploit-report-xss-vulnerabilities/",
@@ -395,17 +396,15 @@
                                 },
                                 link="https://github.com/s0md3v/XSStrike.git",
                                 method="github",
                                 github_install="git clone https://github.com/s0md3v/XSStrike.git && cd XSStrike && chmod +x xsstrike.py",
                                 github_check="XSStrike",
                             )
 def dalfox():
-    github = github_getting_text(
-                                "https://github.com/hahwul/dalfox/blob/main/README.md", 'p', 1
-                            )
+    github = "DalFox is a powerful open-source tool that focuses on automation, making it ideal for quickly scanning for XSS flaws and analyzing parameters. Its advanced testing engine and niche features are designed to streamline the process of detecting and verifying vulnerabilities."
     template.template(
                                 "dalfox",
                                 "dalfox",
                                 github.strip(),
                                 {
                                     "DalFox - Parameter Analysis and XSS Scanning tool": "https://www.geeksforgeeks.org/dalfox-parameter-analysis-and-xss-scanning-tool/",
                                     "Automating XSS using Dalfox, GF and Waybackurls": "https://infosecwriteups.com/automating-xss-using-dalfox-gf-and-waybackurls-bc6de16a5c75",
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/dos.py` & `cyberonix-3.0.3/cyberonix/main/tools/dos.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,68 +54,64 @@
         return paras[indexvalue].text
     except:
         return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
 
 def slowloris():
     github = "Slowloris is a Low bandwidth  HTTP Denial of Service attack that affects threaded servers"
     template.template(
-                "Slowloris",
-                "python3 slowloris.py -h",
+                "slowloris",
+                "slowloris.py -h",
                 github.strip(),
                 {
                     "Slowloris DDOS Attack Tool in Kali Linux": "https://www.geeksforgeeks.org/slowloris-ddos-attack-tool-in-kali-linux/",
                     "What is Slowloris?": "https://www.imperva.com/learn/ddos/slowloris/",
                     "Performing a genuine slowloris attack": "https://ourcodeworld.com/articles/read/962/performing-a-genuine-slowloris-attack-slowhttp-of-indefinite-length-in-kali-linux",
-                },
-                link="https://github.com/gkbrk/slowloris.git",
-                method="github",
-                github_install="git clone https://github.com/gkbrk/slowloris.git",
-                github_check="slowloris",
-            )
+                },)
 def thc_ssl_dos():
-    github = github_getting_text(
+    github_p1 = github_getting_text(
                 "https://www.kali.org/tools/thc-ssl-dos/", "p", 1
             )
-    github += github_getting_text(
-                "https://www.kali.org/tools/thc-ssl-dos/", "p", 2
-            )
-    github += github_getting_text(
-                "https://www.kali.org/tools/thc-ssl-dos/", "p", 3
-            )
+    github_p2= github_getting_text("https://www.kali.org/tools/thc-ssl-dos/", "p", 2)
+    github_p3= github_getting_text("https://www.kali.org/tools/thc-ssl-dos/", "p", 3)
+    github = github_p1.strip().replace("\n", "").replace("\t", "")+github_p2.strip().replace("\n", "").replace("\t", "")+github_p3.strip().replace("\n", "").replace("\t", "")
     template.template(
                 "thc-ssl-dos",
                 "thc-ssl-dos -h",
                 github.strip(),
                 {
                     "THC-SSL DoS": "https://www.radware.com/security/ddos-knowledge-center/ddospedia/thc-ssl-dos/",
                     "thc-ssl-dos Usage Example": "https://www.kali.org/tools/thc-ssl-dos/",
                     "THC-SSL-DOS – DoS Tool Against Secure Web-Servers and for Testing SSL-Renegotiation": "https://kalilinuxtutorials.com/thc-ssl-dos/",
                     "The THC SSL DoS Threat": "https://resources.infosecinstitute.com/topic/thc-ssl-dos-threat/",
                 },
             )
 def slowhttptest():
-    github = github_getting_text(
+    github_p1 = github_getting_text(
                 "https://www.kali.org/tools/slowhttptest/", "p", 1
             )
+    github = github_p1.strip().replace("\n", "").replace("\t", "")
     template.template(
                 "slowhttptest",
                 "slowhttptest -h",
                 github.strip(),
                 {
                     'How to perform a DoS attack "Slow HTTP" with SlowHTTPTest': "https://ourcodeworld.com/articles/read/949/how-to-perform-a-dos-attack-slow-http-with-slowhttptest-test-your-server-slowloris-protection-in-kali-linux",
                     "slowhttptest Usage Example": "https://www.kali.org/tools/slowhttptest/",
                     "DoS website using slowhttptest in Kali Linux ": "https://www.blackmoreops.com/2015/06/07/attack-website-using-slowhttptest-in-kali-linux/",
                     "Kali Linux - Stressing Tools": "https://www.tutorialspoint.com/kali_linux/kali_linux_stressing_tools.htm",
                     "How to perform SlowHTTPtest DOS attack ": "https://support.tetcos.com/support/solutions/articles/14000130254-how-to-perform-slowhttptest-dos-attack-through-netsim-emulator-",
                 },
             )
 def goldeneye():
-    github = github_getting_text(
+    github_p1 = github_getting_text(
                 "https://www.kali.org/tools/goldeneye/", "p", 0
+	                
+
             )
+    github = github_p1.strip().replace("\n", "").replace("\t", "")
     template.template(
                 "goldeneye",
                 "goldeneye -h",
                 github.strip(),
                 {
                     "Goldeneye DDos Tool in Kali Linux": "https://www.geeksforgeeks.org/goldeneye-ddos-tool-in-kali-linux/",
                     "Golden Eye DDoS Tool: Installation and Tool usage with examples": "https://allabouttesting.org/golden-eye-ddos-tool-installation-and-tool-usage-with-examples/",
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/forensic.py` & `cyberonix-3.0.3/cyberonix/main/tools/forensic.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/html5.py` & `cyberonix-3.0.3/cyberonix/main/tools/html5.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/information_gathering.py` & `cyberonix-3.0.3/cyberonix/main/tools/information_gathering.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 "BGP-Toolkit": "https://bgp.he.net/",
                 "Mattw.io": "https://mattw.io/",
                 "Searchftps": "https://www.searchftps.net/",
                 "Security Headers": "https://securityheaders.com/",
                 "Robtex": "https://www.robtex.com/",
                 "Builtwith": "https://builtwith.com/",
                 "Intodns": "https://www.intodns.com/",
-                "Serachdns": "https://searchdns.netcraft.com/",
+                "Searchdns": "https://searchdns.netcraft.com/",
                 "Hackertarget": "https://hackertarget.com/",
                 "Vulners": "https://vulners.com/",
                 "cvedetails": "https://www.cvedetails.com/",
                 "Zero Day initiative": "https://www.zerodayinitiative.com/",
 
 
             })
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/run_on_browser.py` & `cyberonix-3.0.3/cyberonix/main/tools/run_on_browser.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/template.py` & `cyberonix-3.0.3/cyberonix/main/tools/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     elif method == "pip":
             run = input(f"\033[1m{colors.red}[+] Do You Want To Uninstall the Tool?(y/n):{colors.reset}")
             if run.lower() == "y" or run.lower() == "yes":
 	    	        os.system(f"pip uninstall {name}")
     elif method == "deb":
             run = input(f"\033[1m{colors.red}[+] Do You Want To Uninstall the Tool?(y/n):{colors.reset}")
             if run.lower() == "y" or run.lower() == "yes":
-	    	        os.system(f"sudo dpkg –purge {name}")	 
+	    	        os.system(f"sudo dpkg --purge {name}")	 
     elif method == "github":
             run = input(f"\033[1m{colors.red}[+] Do You Want To Github Uninstall the Tool?(y/n):{colors.reset}")
             if run.lower() == "y" or run.lower() == "yes":
 
                 print("Uninstallation...")
                 folder_path = check_path(name)
                 os.system(f'rm -rf {folder_path}')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cyberonix-3.0.2/cyberonix/main/tools/writeup.py` & `cyberonix-3.0.3/cyberonix/main/tools/writeup.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/cyberonix.egg-info/PKG-INFO` & `cyberonix-3.0.3/cyberonix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.2
+Version: 3.0.3
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
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.2 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.3 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-3.0.2/cyberonix.egg-info/SOURCES.txt` & `cyberonix-3.0.3/cyberonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.2/setup.py` & `cyberonix-3.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cyberonix",
-    version="3.0.2",
+    version="3.0.3",
     author="Defronix",
     author_email="hello@defronix.com",
     description="Cyberonix is a complete resource hub for Cyber Security Community.",
     url='https://github.com/TeamDefronix/Cyberonix',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
@@ -26,15 +26,15 @@
         "Programming Language :: Python :: 3.10",
         "Topic :: Security",
     ],
     install_requires=[
         "beautifulsoup4",
         "requests",
         "ipwhois",
-        "dnspython==2.3.0",
+        "dnspython",
         "selenium==4.7.2",
         "netifaces",
     ],
     entry_points={
         'console_scripts': [
             'cyberonix = cyberonix.cyberonix:starting'
         ]
```

