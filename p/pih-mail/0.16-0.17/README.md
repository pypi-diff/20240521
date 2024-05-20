# Comparing `tmp/pih-mail-0.16.tar.gz` & `tmp/pih-mail-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mail-0.16.tar", last modified: Fri Apr 19 02:30:10 2024, max compression
+gzip compressed data, was "pih-mail-0.17.tar", last modified: Mon May 20 22:57:39 2024, max compression
```

## Comparing `pih-mail-0.16.tar` & `pih-mail-0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 02:30:10.982240 pih-mail-0.16/
-drwxrwxrwx   0        0        0        0 2024-04-19 02:30:10.182738 pih-mail-0.16/MailService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mail-0.16/MailService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-15 01:08:42.000000 pih-mail-0.16/MailService/__main__.py
--rw-rw-rw-   0        0        0        2 2023-07-09 01:12:40.000000 pih-mail-0.16/MailService/api.py
--rw-rw-rw-   0        0        0     1178 2024-04-19 02:26:40.000000 pih-mail-0.16/MailService/const.py
--rw-rw-rw-   0        0        0    11073 2024-04-18 06:12:00.000000 pih-mail-0.16/MailService/service.py
--rw-rw-rw-   0        0        0      318 2024-04-19 02:30:10.935373 pih-mail-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 02:30:10.904116 pih-mail-0.16/pih_mail.egg-info/
--rw-rw-rw-   0        0        0      318 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 02:30:10.982240 pih-mail-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:57:39.492799 pih-mail-0.17/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:57:38.825217 pih-mail-0.17/MailService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mail-0.17/MailService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-15 01:08:42.000000 pih-mail-0.17/MailService/__main__.py
+-rw-rw-rw-   0        0        0        2 2023-07-09 01:12:40.000000 pih-mail-0.17/MailService/api.py
+-rw-rw-rw-   0        0        0     1178 2024-05-20 22:38:29.000000 pih-mail-0.17/MailService/const.py
+-rw-rw-rw-   0        0        0    11073 2024-04-18 06:12:00.000000 pih-mail-0.17/MailService/service.py
+-rw-rw-rw-   0        0        0      318 2024-05-20 22:57:39.399026 pih-mail-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:57:39.336532 pih-mail-0.17/pih_mail.egg-info/
+-rw-rw-rw-   0        0        0      318 2024-05-20 22:57:36.000000 pih-mail-0.17/pih_mail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-20 22:57:38.000000 pih-mail-0.17/pih_mail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:57:37.000000 pih-mail-0.17/pih_mail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-20 22:57:37.000000 pih-mail-0.17/pih_mail.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-05-20 22:57:37.000000 pih-mail-0.17/pih_mail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 22:57:37.000000 pih-mail-0.17/pih_mail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:57:39.508416 pih-mail-0.17/setup.cfg
```

### Comparing `pih-mail-0.16/MailService/const.py` & `pih-mail-0.17/MailService/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 NAME: str = "Mail"
 SECTION: str = "MailboxInfo"
 
 HOST = Hosts.WS255
 
 # 0.1 - Persistance caching for email address deliverability checking status and  recall for email deliverability checking if status == UNKNOWN
 # 0.12 - using new method for checking mail deliverity
-VERSION: str = "0.16"
+VERSION: str = "0.17"
 
 TIMEOUT: int = 10
 TRY_AGAIN_COUNT: int = 5
 TRY_AGAIN_SLEEP_TIME: int = 1
 PACKAGES: tuple[str, ...] = (
     "imap_tools",
     "dnspython",
```

### Comparing `pih-mail-0.16/MailService/service.py` & `pih-mail-0.17/MailService/service.py`

 * *Files identical despite different names*

