# Comparing `tmp/ibott-mail-1.0.6.tar.gz` & `tmp/ibott-mail-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibott-mail-1.0.6.tar", last modified: Wed Apr 10 09:37:42 2024, max compression
+gzip compressed data, was "ibott-mail-1.0.7.tar", last modified: Tue May 21 12:23:45 2024, max compression
```

## Comparing `ibott-mail-1.0.6.tar` & `ibott-mail-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-04-10 09:37:42.678427 ibott-mail-1.0.6/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    11355 2023-10-14 17:23:38.000000 ibott-mail-1.0.6/LICENSE
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15986 2024-04-10 09:37:42.678142 ibott-mail-1.0.6/PKG-INFO
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-04-10 09:37:42.676325 ibott-mail-1.0.6/email_activities/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        0 2022-05-16 11:27:00.000000 ibott-mail-1.0.6/email_activities/__init__.py
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     5139 2024-04-10 07:25:15.000000 ibott-mail-1.0.6/email_activities/mails.py
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-04-10 09:37:42.677711 ibott-mail-1.0.6/ibott_mail.egg-info/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15986 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/PKG-INFO
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      255 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/SOURCES.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        1 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/dependency_links.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       29 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/requires.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       17 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/top_level.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      710 2024-04-10 09:37:34.000000 ibott-mail-1.0.6/pyproject.toml
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       38 2024-04-10 09:37:42.678500 ibott-mail-1.0.6/setup.cfg
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      700 2024-04-10 09:37:34.000000 ibott-mail-1.0.6/setup.py
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-05-21 12:23:45.893556 ibott-mail-1.0.7/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    11355 2023-10-14 17:23:38.000000 ibott-mail-1.0.7/LICENSE
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15986 2024-05-21 12:23:45.893192 ibott-mail-1.0.7/PKG-INFO
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-05-21 12:23:45.891319 ibott-mail-1.0.7/email_activities/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        0 2022-05-16 11:27:00.000000 ibott-mail-1.0.7/email_activities/__init__.py
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     5129 2024-05-21 12:09:00.000000 ibott-mail-1.0.7/email_activities/mails.py
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-05-21 12:23:45.892720 ibott-mail-1.0.7/ibott_mail.egg-info/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15986 2024-05-21 12:23:45.000000 ibott-mail-1.0.7/ibott_mail.egg-info/PKG-INFO
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      255 2024-05-21 12:23:45.000000 ibott-mail-1.0.7/ibott_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        1 2024-05-21 12:23:45.000000 ibott-mail-1.0.7/ibott_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       29 2024-05-21 12:23:45.000000 ibott-mail-1.0.7/ibott_mail.egg-info/requires.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       17 2024-05-21 12:23:45.000000 ibott-mail-1.0.7/ibott_mail.egg-info/top_level.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      710 2024-05-21 12:16:25.000000 ibott-mail-1.0.7/pyproject.toml
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       38 2024-05-21 12:23:45.893644 ibott-mail-1.0.7/setup.cfg
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      700 2024-04-10 09:37:34.000000 ibott-mail-1.0.7/setup.py
```

### Comparing `ibott-mail-1.0.6/LICENSE` & `ibott-mail-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ibott-mail-1.0.6/PKG-INFO` & `ibott-mail-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott-mail
-Version: 1.0.6
+Version: 1.0.7
 Summary: This packages crates a simple way to work with, emails, send, read and download attachments
 Home-page: https://github.com/ecrespo66/files_and_folders
 Author: OnameDohe
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibott-mail-1.0.6/email_activities/mails.py` & `ibott-mail-1.0.7/email_activities/mails.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,18 +80,19 @@
 
         context = ssl.create_default_context()
 
         try:
             smtp = smtplib.SMTP_SSL(self.smtp_server, self.smtp_port, context=context)
         except:
             smtp = smtplib.SMTP(self.smtp_server, self.smtp_port)
+            smtp.starttls()
         try:
             smtp.login(self.username, self.password)
-        except:
-            print("El servidor de correo no requiere autenticación")
+        except Exception as e:
+            pass
 
         smtp.sendmail(self.username, send_to, msg.as_string())
         smtp.close()
 
     def fetch(self, folder=None, Query=None):
         """
         Get list of emails from Mailbox server
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ibott-mail-1.0.6/ibott_mail.egg-info/PKG-INFO` & `ibott-mail-1.0.7/ibott_mail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott-mail
-Version: 1.0.6
+Version: 1.0.7
 Summary: This packages crates a simple way to work with, emails, send, read and download attachments
 Home-page: https://github.com/ecrespo66/files_and_folders
 Author: OnameDohe
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibott-mail-1.0.6/pyproject.toml` & `ibott-mail-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "imap-tools==0.16.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ibott-mail"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
     { name="OnameDohe", email="enrique.crespo.debenito@gmail.com" },
 ]
 description = "This packages crates a simple way to work with, emails, send, read and download attachments"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `ibott-mail-1.0.6/setup.py` & `ibott-mail-1.0.7/setup.py`

 * *Files identical despite different names*

