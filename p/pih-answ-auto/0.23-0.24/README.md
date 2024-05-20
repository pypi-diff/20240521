# Comparing `tmp/pih-answ_auto-0.23.tar.gz` & `tmp/pih-answ_auto-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.23.tar", last modified: Mon May 13 01:53:06 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.24.tar", last modified: Mon May 20 22:46:40 2024, max compression
```

## Comparing `pih-answ_auto-0.23.tar` & `pih-answ_auto-0.24.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:53:06.482904 pih-answ_auto-0.23/
-drwxrwxrwx   0        0        0        0 2024-05-13 01:53:06.036154 pih-answ_auto-0.23/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.23/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.23/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      412 2024-05-13 01:49:11.000000 pih-answ_auto-0.23/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0    10088 2024-05-08 14:19:07.000000 pih-answ_auto-0.23/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      283 2024-05-13 01:53:06.434983 pih-answ_auto-0.23/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 01:53:06.388111 pih-answ_auto-0.23/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      283 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 01:53:06.482904 pih-answ_auto-0.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:40.889827 pih-answ_auto-0.24/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:40.403380 pih-answ_auto-0.24/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.24/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.24/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      412 2024-05-20 22:38:30.000000 pih-answ_auto-0.24/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0    10076 2024-05-19 12:38:30.000000 pih-answ_auto-0.24/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      283 2024-05-20 22:46:40.858556 pih-answ_auto-0.24/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:46:40.810648 pih-answ_auto-0.24/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-05-20 22:46:39.000000 pih-answ_auto-0.24/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-20 22:46:40.000000 pih-answ_auto-0.24/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:46:39.000000 pih-answ_auto-0.24/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-20 22:46:39.000000 pih-answ_auto-0.24/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 22:46:39.000000 pih-answ_auto-0.24/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-20 22:46:39.000000 pih-answ_auto-0.24/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:46:40.905450 pih-answ_auto-0.24/setup.cfg
```

### Comparing `pih-answ_auto-0.23/AnswerAutomationService/service.py` & `pih-answ_auto-0.24/AnswerAutomationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 class ANSWER_TYPE:
 
     VISIT = 1
     TAX_CERTIFICATE = 2
     VISIT_MODIFICATION = 4
     HOW_TO_GET = 8
     OTHER_QUESTION = 16
-    # LATE = 8
 
 
 def start(as_standalone: bool = False) -> None:
 
     from pih.collections import (
         Message,
         PolibasePerson,
@@ -71,15 +70,15 @@
                                         pin,
                                         nnt(polibase_person_visit_ds).FullName,
                                         nnt(polibase_person_visit_ds).telephoneNumber,
                                     )
                                     if pin == A.CT_P.PRERECORDING_PIN
                                     else A.D_P.person_by_pin(pin)
                                 )
-                                if A.A_P_N_C.update(telephone_number, sender, 1):
+                                if A.A_P_N_C.update(person.telephoneNumber, sender, 1):
 
                                     answer_type: int = 0
 
                                     message: str = nnt(nnt(whatsapp_message).message)
 
                                     if ne(message):
                                         for index, variants in enumerate(
@@ -105,18 +104,18 @@
                                         )
 
                                     def send_message(
                                         value: str | None = None,
                                         image_url: str | None = None,
                                         location: tuple[float, float] | None = None,
                                     ) -> None:
-                                        A.ME_WH_W_Q.add_message(
+                                        A.ME_WH_W_Q.add(
                                             Message(
                                                 value,
-                                                telephone_number,
+                                                person.telephoneNumber,
                                                 sender,
                                                 image_url,
                                                 location,
                                             )
                                         )
 
                                     if BM.has(answer_type, ANSWER_TYPE.VISIT):
```

