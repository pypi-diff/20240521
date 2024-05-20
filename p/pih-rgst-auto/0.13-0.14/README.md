# Comparing `tmp/pih-rgst_auto-0.13.tar.gz` & `tmp/pih-rgst_auto-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rgst_auto-0.13.tar", last modified: Wed Apr 10 02:28:53 2024, max compression
+gzip compressed data, was "pih-rgst_auto-0.14.tar", last modified: Mon May 20 23:14:24 2024, max compression
```

## Comparing `pih-rgst_auto-0.13.tar` & `pih-rgst_auto-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:28:53.484466 pih-rgst_auto-0.13/
--rw-rw-rw-   0        0        0      336 2024-04-10 02:28:53.453219 pih-rgst_auto-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:28:53.057573 pih-rgst_auto-0.13/RegistratorAutomationService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-rgst_auto-0.13/RegistratorAutomationService/__init__.py
--rw-rw-rw-   0        0        0      155 2024-04-10 01:34:06.000000 pih-rgst_auto-0.13/RegistratorAutomationService/__main__.py
--rw-rw-rw-   0        0        0      551 2024-04-10 01:32:40.000000 pih-rgst_auto-0.13/RegistratorAutomationService/const.py
--rw-rw-rw-   0        0        0    19908 2024-04-10 01:34:06.000000 pih-rgst_auto-0.13/RegistratorAutomationService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:28:53.421972 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/
--rw-rw-rw-   0        0        0      336 2024-04-10 02:28:52.000000 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-04-10 02:28:52.000000 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:28:52.000000 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-04-10 02:28:52.000000 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-04-10 02:28:52.000000 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-10 02:28:52.000000 pih-rgst_auto-0.13/pih_rgst_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:28:53.484466 pih-rgst_auto-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:14:24.623075 pih-rgst_auto-0.14/
+-rw-rw-rw-   0        0        0      336 2024-05-20 23:14:24.591826 pih-rgst_auto-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:14:24.238287 pih-rgst_auto-0.14/RegistratorAutomationService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-rgst_auto-0.14/RegistratorAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      155 2024-04-10 01:34:06.000000 pih-rgst_auto-0.14/RegistratorAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      551 2024-05-20 22:40:33.000000 pih-rgst_auto-0.14/RegistratorAutomationService/const.py
+-rw-rw-rw-   0        0        0    19677 2024-05-19 13:13:03.000000 pih-rgst_auto-0.14/RegistratorAutomationService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 23:14:24.520225 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/
+-rw-rw-rw-   0        0        0      336 2024-05-20 23:14:23.000000 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-05-20 23:14:24.000000 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:14:23.000000 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-20 23:14:23.000000 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-05-20 23:14:23.000000 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 23:14:23.000000 pih-rgst_auto-0.14/pih_rgst_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:14:24.623075 pih-rgst_auto-0.14/setup.cfg
```

### Comparing `pih-rgst_auto-0.13/RegistratorAutomationService/const.py` & `pih-rgst_auto-0.14/RegistratorAutomationService/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 HOST = A.CT_H.BACKUP_WORKER
 
 
 PACKAGES: tuple[str, ...] = (
     A.PTH_FCD_DIST.NAME(A.CT_SR.MOBILE_HELPER.standalone_name),  # type: ignore
 )
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Registrator Automation service",
     host=HOST.NAME,
     version=VERSION,
     standalone_name="rgst_auto",
```

### Comparing `pih-rgst_auto-0.13/RegistratorAutomationService/service.py` & `pih-rgst_auto-0.14/RegistratorAutomationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 import ipih
 
-from pih import A
+from pih import A, send_message
 from pih.consts.errors import NotFound
 from pih.collections import (
     User,
     EventDS,
     Message,
     NewMailMessage,
     PolibasePerson,
@@ -27,18 +27,21 @@
     print(as_standalone)
     from MobileHelperService.api import MobileOutput
     from MobileHelperService.client import Client as MIO
 
     email_control_output: MobileOutput = MIO.create_output(
         A.CT_ME_WH.GROUP.EMAIL_CONTROL
     )
-    sender_profile: A.CT_ME_WH_W.Profiles = A.CT_ME_WH_W.Profiles.CALL_CENTRE
 
-    def mio_write(telephone_number: str, message: str) -> None:
-        A.A_MIO.write(telephone_number, message, sender_profile)
+    def _send_message(
+        telephone_number: str, message: str, queued: bool = False
+    ) -> None:
+        send_message(
+            message, telephone_number, A.CT_ME_WH_W.Profiles.CALL_CENTRE, queued
+        )
 
     def service_call_handler(_, pl: ParameterList) -> Any:
         if A.D_Ex.subscribtion_result(pl).result:
             event: A.CT_E | None = None
             parameters: list[Any] | None = None
             event, parameters = A.D_Ex_E.with_parameters(pl)
             if event in [
@@ -80,15 +83,15 @@
                 eventDS: EventDS | None = one(
                     A.R_E.get_last_by_key(
                         *A.E_B.ask_for_polibase_person_email(polibase_person)
                     )
                 )
                 telephone_number: str = polibase_person.telephoneNumber
                 if nn(eventDS):
-                    mio_write(
+                    _send_message(
                         telephone_number,
                         j(
                             (
                                 "День добрый, ",
                                 b(A.D.to_given_name(polibase_person)),
                                 ".",
                                 nl(),
@@ -98,19 +101,19 @@
                                 nl(),
                                 "Для этого - скопируйте код ",
                                 A.CT_V.HAND_DOWN,
                                 ":",
                             )
                         ),
                     )
-                    mio_write(
+                    _send_message(
                         telephone_number,
                         str(eventDS.parameters[A.CT_PI.SECRET.name]),
                     )
-                    mio_write(
+                    _send_message(
                         telephone_number,
                         j(
                             (
                                 "И отправьте этот код в теме или теле письма на почту: ",
                                 nl(),
                                 A.CT_EML.ADD_EMAIL,
                                 nl(),
@@ -144,15 +147,15 @@
                             polibase_person: PolibasePerson = A.D_P.person_by_pin(
                                 polibase_person_pin
                             )
                             telephone_number: str = polibase_person.telephoneNumber
                             current_email: str = polibase_person.email
                             if lw(current_email) != from_:
                                 if A.A_P.email(from_, polibase_person):
-                                    mio_write(
+                                    _send_message(
                                         telephone_number,
                                         j(
                                             (
                                                 "День добрый, ",
                                                 b(A.D.to_given_name(polibase_person)),
                                                 ", ",
                                                 "адресс электронной почты была добавлена в Вашу карту",
@@ -300,41 +303,37 @@
                         if not allow_for_notification:
                             allow_for_notification = A.C.email(
                                 polibase_person.email, check_accesability=True
                             )
 
                     polibase_note_title: str = A.D_P.note_title(polibase_note_id)
                     if allow_for_notification:
-                        A.ME_WH_W_Q.add_message(
-                            Message(
-                                j(
-                                    (
-                                        A.S.get(
-                                            A.CT_S.PERSON_VISIT_NOTIFICATION_HEADER
-                                        ),
-                                        b(
-                                            A.D.to_given_name(
-                                                polibase_person.FullName  # type: ignore
-                                            )
-                                        ),
-                                        ", на Вашу электронную почту отправлено письмо с медицинской записью ",
-                                        esc(
-                                            polibase_note_title,
-                                        ),
-                                        ".",
-                                        nl(count=2),
-                                        b("Важно:"),
-                                        " если письма нет на почте, посмотрите в папке ",
-                                        b("Спам"),
-                                        ".",
-                                    )
-                                ),
-                                polibase_person.telephoneNumber,  # type: ignore
-                                A.D.get(sender_profile),
-                            )
+                        _send_message(
+                            j(
+                                (
+                                    A.S.get(A.CT_S.PERSON_VISIT_NOTIFICATION_HEADER),
+                                    b(
+                                        A.D.to_given_name(
+                                            polibase_person.FullName  # type: ignore
+                                        )
+                                    ),
+                                    ", на Вашу электронную почту отправлено письмо с медицинской записью ",
+                                    esc(
+                                        polibase_note_title,
+                                    ),
+                                    ".",
+                                    nl(count=2),
+                                    b("Важно:"),
+                                    " если письма нет на почте, посмотрите в папке ",
+                                    b("Спам"),
+                                    ".",
+                                )
+                            ),
+                            polibase_person.telephoneNumber,  # type: ignore
+                            True,
                         )
                     else:
                         email_address = polibase_person.email
                         email_control_output.write_line(
                             j(
                                 (
                                     js(
```

