# Comparing `tmp/pih-rvw_auto-0.18.tar.gz` & `tmp/pih-rvw_auto-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rvw_auto-0.18.tar", last modified: Mon May  6 04:01:25 2024, max compression
+gzip compressed data, was "pih-rvw_auto-0.19.tar", last modified: Mon May 20 23:14:51 2024, max compression
```

## Comparing `pih-rvw_auto-0.18.tar` & `pih-rvw_auto-0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:01:25.677923 pih-rvw_auto-0.18/
--rw-rw-rw-   0        0        0      282 2024-05-06 04:01:25.646631 pih-rvw_auto-0.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 04:01:25.264028 pih-rvw_auto-0.18/ReviewAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.18/ReviewAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.18/ReviewAutomationService/__main__.py
--rw-rw-rw-   0        0        0     2476 2024-04-15 23:57:45.000000 pih-rvw_auto-0.18/ReviewAutomationService/api.py
--rw-rw-rw-   0        0        0      519 2024-05-06 04:00:59.000000 pih-rvw_auto-0.18/ReviewAutomationService/const.py
--rw-rw-rw-   0        0        0     8565 2024-05-02 02:09:58.000000 pih-rvw_auto-0.18/ReviewAutomationService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:01:25.599756 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/
--rw-rw-rw-   0        0        0      282 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 04:01:25.677923 pih-rvw_auto-0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:14:51.334177 pih-rvw_auto-0.19/
+-rw-rw-rw-   0        0        0      282 2024-05-20 23:14:51.318551 pih-rvw_auto-0.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:14:50.911251 pih-rvw_auto-0.19/ReviewAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.19/ReviewAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.19/ReviewAutomationService/__main__.py
+-rw-rw-rw-   0        0        0     2625 2024-05-19 13:02:43.000000 pih-rvw_auto-0.19/ReviewAutomationService/api.py
+-rw-rw-rw-   0        0        0      525 2024-05-20 22:40:33.000000 pih-rvw_auto-0.19/ReviewAutomationService/const.py
+-rw-rw-rw-   0        0        0     8114 2024-05-19 13:02:43.000000 pih-rvw_auto-0.19/ReviewAutomationService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:14:51.271674 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-05-20 23:14:50.000000 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-05-20 23:14:50.000000 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:14:50.000000 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-20 23:14:50.000000 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 23:14:50.000000 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-20 23:14:50.000000 pih-rvw_auto-0.19/pih_rvw_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:14:51.365425 pih-rvw_auto-0.19/setup.cfg
```

### Comparing `pih-rvw_auto-0.18/ReviewAutomationService/api.py` & `pih-rvw_auto-0.19/ReviewAutomationService/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ipih
 
 from pih import A
 from pih.collections import Result
 
-from pih.collections import PolibasePerson
+from pih.collections import PolibasePerson, Message
 from NotificationAutomationService.api import NotificationApi as Api
 
 
 class ReviewNotificationApi:
     @staticmethod
     def start_review_notification_distribution_action(test: bool = False) -> bool:
         sender_profile: A.CT_ME_WH_W.Profiles = A.CT_ME_WH_W.Profiles.MARKETER
@@ -16,23 +16,26 @@
 
                 def every_action(person: PolibasePerson, inpatient: bool) -> None:
                     telephone_number: str | None = A.D_F.telephone_number_international(
                         person.telephoneNumber
                     )
                     # polibase format telephone number 7
                     if A.C.telephone_number_international(telephone_number):
-                        if A.ME_WH_W_Q.add(
-                            A.S_P_RN.notification_text(
-                                person,
-                                Api.check_for_notification_confirmation(
-                                    telephone_number, sender_profile.value, test
+                        sender: str = A.D.get(sender_profile)
+                        if queued_message(
+                            Message(
+                                A.S_P_RN.notification_text(
+                                    person,
+                                    Api.check_for_notification_confirmation(
+                                        telephone_number, sender, test
+                                    ),
                                 ),
-                            ),
-                            telephone_number,
-                            sender_profile,
+                                telephone_number,
+                                sender
+                            )
                         ):
                             A.E.send(
                                 A.CT_E.POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_REGISTERED,
                                 (person.pin, inpatient, 2),
                             )
 
                 def map_function(pin_list: list[int]) -> list[PolibasePerson]:
```

### Comparing `pih-rvw_auto-0.18/ReviewAutomationService/const.py` & `pih-rvw_auto-0.19/ReviewAutomationService/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "ReviewAutomation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.18"
+VERSION: str = "0.19"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Review automation service",
     host=HOST.NAME,
     use_standalone=True,
     version=VERSION,
     standalone_name="rvw_auto",
     run_from_system_account=True,
-    python_executable_path=CONST.UNKNOWN,
+    python_executable_path=CONST.UNKNOWN_VALUE,
 )
```

### Comparing `pih-rvw_auto-0.18/ReviewAutomationService/service.py` & `pih-rvw_auto-0.19/ReviewAutomationService/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import ipih
 
-from pih import A, PIHThread
+from pih import A, PIHThread, send_message
 from ReviewAutomationService.const import SD
 
-import re
-
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
+test: bool = True
+
 
 def start(as_standalone: bool = False) -> None:
     from datetime import datetime
     from pih.consts.errors import NotFound
     from pih.collections import (
         EventDS,
-        Message,
         PolibasePerson,
         WhatsAppMessage,
         PolibasePersonNotificationConfirmation as PPNC,
     )
     from ReviewAutomationService.api import (
         ReviewNotificationApi as Api,
     )
@@ -86,51 +85,45 @@
                                                     A.CT_PI.INPATIENT.name
                                                 ]
                                                 if nn(review_event)
                                                 and nn(nnt(review_event).parameters)
                                                 else False
                                             )
                                             if answer_yes:
-                                                A.ME_WH_W_Q.add_message(
-                                                    Message(
-                                                        str(
-                                                            A.S.get(
-                                                                A.CT_S.POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT
-                                                            )
-                                                        ).format(
-                                                            name=FullNameTool.to_given_name(
-                                                                nnt(
-                                                                    nnt(person).FullName
-                                                                )
-                                                            )
-                                                        ),
-                                                        telephone_number,
-                                                        sender,
-                                                    )
-                                                )
-                                                A.ME_WH_W_Q.add_message(
-                                                    Message(
+                                                send_message(
+                                                    str(
                                                         A.S.get(
-                                                            A.CT_S.REVIEW_ACTION_URL_FOR_INPATIENT
-                                                            if is_inpatient
-                                                            else A.CT_S.REVIEW_ACTION_URL
-                                                        ),
-                                                        telephone_number,
-                                                        sender,
-                                                    )
+                                                            A.CT_S.POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT
+                                                        )
+                                                    ).format(
+                                                        name=FullNameTool.to_given_name(
+                                                            nnt(nnt(person).FullName)
+                                                        )
+                                                    ),
+                                                    telephone_number,
+                                                    sender,
+                                                    True,
+                                                )
+                                                send_message(
+                                                    A.S.get(
+                                                        A.CT_S.REVIEW_ACTION_URL_FOR_INPATIENT
+                                                        if is_inpatient
+                                                        else A.CT_S.REVIEW_ACTION_URL
+                                                    ),
+                                                    telephone_number,
+                                                    sender,
                                                 )
                                             else:
-                                                A.ME_WH_W_Q.add_message(
-                                                    Message(
-                                                        A.S.get(
-                                                            A.CT_S.POLIBASE_PERSON_NO_ANSWER_ON_NOTIFICATION_CONFIRMATION_TEXT
-                                                        ),
-                                                        telephone_number,
-                                                        sender,
-                                                    )
+                                                send_message(
+                                                    A.S.get(
+                                                        A.CT_S.POLIBASE_PERSON_NO_ANSWER_ON_NOTIFICATION_CONFIRMATION_TEXT
+                                                    ),
+                                                    telephone_number,
+                                                    sender,
+                                                    True,
                                                 )
 
                                             A.E.send(
                                                 A.CT_E.POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_ANSWERED,
                                                 (
                                                     nnt(person).pin,
                                                     j((message_text.splitlines())),
@@ -144,15 +137,16 @@
                                     j((SD.standalone_name, ": ", error.get_details()))
                                 )
                         return True
         return None
 
     def heat_beat_handler(current_datetime: datetime) -> None:
         if A.S_P_RN.is_on():
-            if A.D.is_equal_by_time(current_datetime, A.S_P_RN.start_time()):
+            if test and A.D.is_equal_by_time(current_datetime, A.S_P_RN.start_time()):
+                test = False
                 PIHThread(
                     Api.start_review_notification_distribution_action,
                 )
 
     def service_starts_handler() -> None:
         A.SRV_A.subscribe_on(SC.heart_beat)
         A.SRV_A.subscribe_on(SC.send_event)
```

