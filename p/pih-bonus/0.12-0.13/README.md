# Comparing `tmp/pih-bonus-0.12.tar.gz` & `tmp/pih-bonus-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-bonus-0.12.tar", last modified: Mon May 13 01:52:28 2024, max compression
+gzip compressed data, was "pih-bonus-0.13.tar", last modified: Mon May 20 22:48:47 2024, max compression
```

## Comparing `pih-bonus-0.12.tar` & `pih-bonus-0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:52:28.345301 pih-bonus-0.12/
-drwxrwxrwx   0        0        0        0 2024-05-13 01:52:27.805645 pih-bonus-0.12/BonusProgramService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-bonus-0.12/BonusProgramService/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-09 22:47:56.000000 pih-bonus-0.12/BonusProgramService/__main__.py
--rw-rw-rw-   0        0        0     4726 2024-04-22 02:31:18.000000 pih-bonus-0.12/BonusProgramService/api.py
--rw-rw-rw-   0        0        0      400 2024-05-13 01:49:02.000000 pih-bonus-0.12/BonusProgramService/const.py
--rw-rw-rw-   0        0        0     6269 2024-04-28 03:21:27.000000 pih-bonus-0.12/BonusProgramService/service.py
--rw-rw-rw-   0        0        0      275 2024-05-13 01:52:28.297393 pih-bonus-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 01:52:28.219288 pih-bonus-0.12/pih_bonus.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 01:52:28.345301 pih-bonus-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:48:47.136766 pih-bonus-0.13/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:48:46.726855 pih-bonus-0.13/BonusProgramService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-bonus-0.13/BonusProgramService/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-09 22:47:56.000000 pih-bonus-0.13/BonusProgramService/__main__.py
+-rw-rw-rw-   0        0        0     4726 2024-04-22 02:31:18.000000 pih-bonus-0.13/BonusProgramService/api.py
+-rw-rw-rw-   0        0        0      400 2024-05-20 22:33:13.000000 pih-bonus-0.13/BonusProgramService/const.py
+-rw-rw-rw-   0        0        0     6476 2024-05-20 02:47:18.000000 pih-bonus-0.13/BonusProgramService/service.py
+-rw-rw-rw-   0        0        0      275 2024-05-20 22:48:47.105515 pih-bonus-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:48:47.074265 pih-bonus-0.13/pih_bonus.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 22:48:46.000000 pih-bonus-0.13/pih_bonus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-20 22:48:46.000000 pih-bonus-0.13/pih_bonus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:48:46.000000 pih-bonus-0.13/pih_bonus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-20 22:48:46.000000 pih-bonus-0.13/pih_bonus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 22:48:46.000000 pih-bonus-0.13/pih_bonus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-20 22:48:46.000000 pih-bonus-0.13/pih_bonus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:48:47.168030 pih-bonus-0.13/setup.cfg
```

### Comparing `pih-bonus-0.12/BonusProgramService/api.py` & `pih-bonus-0.13/BonusProgramService/api.py`

 * *Files identical despite different names*

### Comparing `pih-bonus-0.12/BonusProgramService/service.py` & `pih-bonus-0.13/BonusProgramService/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import ipih
 
-from pih import A, serve, subscribe_on
+from pih import A, serve, subscribe_on, send_message
 from BonusProgramService.const import SD
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
 
     from BonusProgramService.api import BonusApi as Api
     from pih.tools import ParameterList, js, nn, one, nnt
-    from pih.collections import BonusInformation, PolibasePerson, Message, EventDS
+    from pih.collections import BonusInformation, PolibasePerson, EventDS
 
     from datetime import datetime
 
     api: Api = Api()
 
     class DH:
         timestamp: dict[int, datetime] = {}
 
-    SENDER: str = A.D.get(A.CT_ME_WH_W.Profiles.CALL_CENTRE)
-
     def server_call_handler(sc: SC, pl: ParameterList) -> bool | None:
         if sc == SC.send_event:
             event: A.CT_E = A.D_Ex_E.get(pl)
             if event == A.CT_E.POLIBASE_PERSON_BONUSES_WAS_UPDATED:
                 polibase_person_pin: int = A.D_Ex_E.parameters(pl)[0]
                 bonus_information: BonusInformation | None = one(
                     A.R_P.bonus_information(polibase_person_pin)
@@ -40,27 +38,29 @@
                                 "обновлены бонусы:",
                                 nnt(bonus_information).bonus_last,
                                 "из",
                                 nnt(bonus_information).bonus_active,
                             )
                         )
                     )
-                    if A.S.get(
-                        A.CT_S.BONUS_PROGRAM_IS_ON
-                    ) or polibase_person_pin == A.S.get(
+                    is_on: bool = A.S.get(A.CT_S.BONUS_PROGRAM_IS_ON)
+                    is_test_polibase_person: bool = polibase_person_pin == A.S.get(
                         A.CT_S.BONUS_PROGRAM_TEST_POLIBASE_PERSON_PIN
-                    ):
+                    )
+                    if is_on or is_test_polibase_person:
                         polibase_person: PolibasePerson = A.D_P.person_by_pin(
                             polibase_person_pin
                         )
                         bonus_information: BonusInformation | None = one(
                             A.R_P.bonus_information(polibase_person)
                         )
                         if nn(bonus_information):
-                            if nnt(bonus_information).bonus_active >= A.S.get(
+                            if is_test_polibase_person or nnt(
+                                bonus_information
+                            ).bonus_active >= A.S.get(
                                 A.CT_S.BONUS_PROGRAM_BONUS_MINIMUM
                             ):
                                 link: str | None = None
                                 if api.exists_bonus_card(polibase_person):
                                     if not api.exists_bonus_card(polibase_person, True):
                                         event_ds: EventDS | None = one(
                                             A.R_E.get_last(
@@ -81,18 +81,20 @@
                                             nn(last_timestamp)
                                             and (
                                                 A.D.now() - nnt(last_timestamp)
                                             ).total_seconds()
                                             < 5 * 60
                                         ):
                                             link = None
-                                        if one(A.R_E.get_count(
-                                            A.CT_E.POLIBASE_PERSON_BONUS_CARD_WAS_CREATED,
-                                            (polibase_person_pin,),
-                                        )) > A.S.get(
+                                        if one(
+                                            A.R_E.get_count(
+                                                A.CT_E.POLIBASE_PERSON_BONUS_CARD_WAS_CREATED,
+                                                (polibase_person_pin,),
+                                            )
+                                        ) > A.S.get(
                                             A.CT_S.BONUS_PROGRAM_NOTIFICATION_COUNT_MAX
                                         ):
                                             link = None
                                         DH.timestamp[polibase_person_pin] = A.D.now()
                                     else:
                                         api.update_bonuses(polibase_person)
                                 else:
@@ -103,20 +105,20 @@
                                             (
                                                 polibase_person_pin,
                                                 link,
                                             ),
                                         )
                                         DH.timestamp[polibase_person_pin] = A.D.now()
                                 if nn(link):
-                                    A.ME_WH_W_Q.add_message(
-                                        Message(
-                                            js(("Перейдите по ссылке:", link)),
-                                            polibase_person.telephoneNumber,
-                                            SENDER,
-                                        )
+                                    send_message(
+                                        str(A.S.get(A.CT_S.BONUS_PROGRAM_TEXT)).format(
+                                            link=link
+                                        ),
+                                        polibase_person.telephoneNumber,
+                                        A.CT_ME_WH_W.Profiles.CALL_CENTRE,
                                     )
                                 else:
                                     pass
                         else:
                             pass
         return None
```

