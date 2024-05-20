# Comparing `tmp/pih-mio-0.29.8.tar.gz` & `tmp/pih-mio-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.29.8.tar", last modified: Thu May  9 23:26:41 2024, max compression
+gzip compressed data, was "pih-mio-0.30.tar", last modified: Mon May 20 23:01:03 2024, max compression
```

## Comparing `pih-mio-0.29.8.tar` & `pih-mio-0.30.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 23:26:41.639765 pih-mio-0.29.8/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:26:40.894905 pih-mio-0.29.8/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.8/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.8/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   372866 2024-05-08 14:50:01.000000 pih-mio-0.29.8/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.8/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.8/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4462 2024-05-09 23:22:09.000000 pih-mio-0.29.8/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      910 2024-05-09 23:19:54.000000 pih-mio-0.29.8/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    17628 2024-05-09 23:18:14.000000 pih-mio-0.29.8/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      331 2024-05-09 23:26:41.624127 pih-mio-0.29.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 23:26:41.558324 pih-mio-0.29.8/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      331 2024-05-09 23:26:39.000000 pih-mio-0.29.8/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-09 23:26:40.000000 pih-mio-0.29.8/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 23:26:41.655391 pih-mio-0.29.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 23:01:03.881865 pih-mio-0.30/
+drwxrwxrwx   0        0        0        0 2024-05-20 23:01:03.267936 pih-mio-0.30/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.30/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.30/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   377214 2024-05-18 23:08:47.000000 pih-mio-0.30/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5930 2024-05-18 23:10:23.000000 pih-mio-0.30/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      303 2024-05-17 06:23:22.000000 pih-mio-0.30/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4470 2024-05-20 22:38:29.000000 pih-mio-0.30/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0     1011 2024-05-19 12:04:05.000000 pih-mio-0.30/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    18213 2024-05-20 00:19:11.000000 pih-mio-0.30/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      381 2024-05-17 06:41:58.000000 pih-mio-0.30/MobileHelperService/tools.py
+-rw-rw-rw-   0        0        0      329 2024-05-20 23:01:03.834971 pih-mio-0.30/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 23:01:03.770983 pih-mio-0.30/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-05-20 23:00:59.000000 pih-mio-0.30/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-20 23:01:00.000000 pih-mio-0.30/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 23:00:59.000000 pih-mio-0.30/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-20 23:00:59.000000 pih-mio-0.30/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 23:00:59.000000 pih-mio-0.30/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-20 23:00:59.000000 pih-mio-0.30/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 23:01:03.881865 pih-mio-0.30/setup.cfg
```

### Comparing `pih-mio-0.29.8/MobileHelperService/api.py` & `pih-mio-0.30/MobileHelperService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import requests
 import calendar
 import shlex
 import json
 import re
 
 from MobileHelperContent.content import MEDIA_CONTENT  # type: ignore
+from MobileHelperService.tools import *
 
 from pih.collections import (
     User,
     Mark,
     Note,
     File,
     Result,
@@ -45,17 +46,17 @@
     CardRegistryFolderStatistics,
     IconedOrderedNameCaptionDescription,
 )
 
 from pih.console_api import ConsoleAppsApi
 from pih.tools import (
     BitMask as BM,
+    n,
     i,
     b,
-    n,
     e,
     j,
     jp,
     nl,
     lw,
     js,
     nn,
@@ -73,38 +74,45 @@
 )
 from pih.consts import (
     Tags,
     Actions,
     JournalType,
     CheckableSections,
     EmailVerificationMethods,
+    INPUT_TYPE,
 )
 from MobileHelperService.collection import MobileHelperUserSettings
 from pih.consts.polibase import PolibaseDocumentTypes
 from pih.consts.ssh_hosts import SSHHosts
 from MobileHelperService.const import *
+from pih.consts import SESSION_TYPE
 
 from pih.consts.errors import BarcodeNotFound, NotFound, Error
 from pih import (
     A,
     PIH,
     Input,
     Stdin,
     Output,
+    strdict,
     Session,
     PIHThread,
     MarkInput,
     UserInput,
     UserOutput,
     MarkOutput,
     OutputStub,
     SessionBase,
 )
 from pih.console_api import LINE
 
+def arg_value_is_file(value: str) -> bool:    
+    return value.startswith(FILE_PATTERN_LIST)
+
+
 
 class MobileOutputBase(OutputStub):
 
     def b(self, value: str) -> str:
         return b(value)
 
     def i(self, value: str) -> str:
@@ -126,33 +134,35 @@
             j((" ", A.CT_V.BLUE_ROMB, " ", lines[0])),
             jnl((A.D.map(lambda item: js((space, item)), lines[1:]))),  # type: ignore
         )
     )
 
 
 class MobileHelperUserSettiongsHolder:
+    
     @staticmethod
-    def get(login: str) -> MobileHelperUserSettings:
+    def get(login_holder: str | User) -> MobileHelperUserSettings:
+        login_holder = login_holder.login if isinstance(login_holder, User) else login_holder
         value: MobileHelperUserSettings = MobileHelperUserSettings()
         result: MobileHelperUserSettings | None = A.S_U.get(
-            login, MOBILE_HELPER_USER_SETTINGS_NAME, value
+            login_holder, MOBILE_HELPER_USER_SETTINGS_NAME, value
         )
         if n(result):
-            MobileHelperUserSettiongsHolder.set(login, value)
-            result = value
+            if MobileHelperUserSettiongsHolder.set(login_holder, value):
+                result = value
         return result  # type: ignore
 
     @staticmethod
     def set(login: str, value: MobileHelperUserSettings) -> bool:
         return A.S_U.set(login, MOBILE_HELPER_USER_SETTINGS_NAME, value)
 
 
 class UserSettings:
-    def __init__(self, login: str):
-        self.login: str = login
+    def __init__(self, login_holder:  str | User):
+        self.login: str = login_holder.login if isinstance(login_holder, User) else login_holder
 
     def get(self) -> MobileHelperUserSettings:
         return MobileHelperUserSettiongsHolder.get(self.login)
 
     def set(self, value: int) -> bool:
         return MobileHelperUserSettiongsHolder.set(
             self.login, MobileHelperUserSettings(value)
@@ -164,35 +174,33 @@
     def remove(self, value: int) -> bool:
         return self.set(BM.remove(self.get().flags, value))
 
     def add(self, value: int) -> bool:
         return self.set(BM.add(self.get().flags, value))
 
 
-def get_command_base_name(value: str) -> str:
-    return value.split(COMMAND_NAME_VARIANT_SPLITTER)[0]
 
 
 def get_command_variant_name(value: str | None) -> str:
     if n(value):
         return ""
     return nns(value).replace(COMMAND_NAME_VARIANT_SPLITTER, "")
 
 
-def command_node_name_equal(value1: str, value2: str) -> bool:
-    return A.D.equal(value1, get_command_base_name(value2)) or A.D.equal(
-        value1, get_command_variant_name(value2)
+def command_node_name_equals_to(name: str, value: str, ) -> bool:
+    command_node_name_variant_index: int = name.find(
+        COMMAND_NAME_VARIANT_SPLITTER
     )
-
-
-def mio_command(value: list[str] | str) -> str:
-    if isinstance(value, str):
-        return get_command_base_name(value)
-    return mio_command(nnt(one(value)))
-
+    if command_node_name_variant_index != -1:
+        name = name[0:command_node_name_variant_index]
+        command_node_name_length: int = len(name)
+        if len(value) < command_node_name_length:
+            return False
+        value = value[0:command_node_name_length]
+    return A.D.equal(value, name)
 
 def flag_name_list(value: Flags, all: bool = False) -> list[str]:
     result: list[str] = [
         item[0]
         for item in A.D.filter(lambda item: item[1] == value, list(FLAG_MAP.items()))
     ]
     return result if all else [result[0]]
@@ -227,37 +235,37 @@
         self,
         result: Result[list[User]],
         caption: str | None = None,
         use_index: bool = False,
         root_location: str = A.CT_AD.ACTIVE_USERS_CONTAINER_DN,
     ) -> None:
         if ne(caption):
-            self.parent.write_line(self.parent.bold(caption))
+            self.parent.write_line(b(caption))
         self.parent.write_result(result, use_index=use_index)
 
     def get_formatted_given_name(self, value: str | None = None) -> str:
-        return self.parent.bold(value)
+        return b(value)
 
 
 class MobileSession(SessionBase):
     def __init__(self, recipient: str, flags: int | None = 0):
-        super().__init__(name="mobile", flags=flags)  # type: ignore
+        super().__init__(name=SESSION_TYPE.OUTSIDE if BM.has(flags, Flags.OUTSIDE) else SESSION_TYPE.MOBILE, flags=flags)  # type: ignore
         self.recipient: str = recipient
         self.user: User | None = None
         self.arg_list: list[str] | None = None
 
     def say_hello(self, telephone_number: str | None = None) -> None:
         self.get_user(telephone_number)
 
     def get_login(self, telephone_number: str | None = None) -> str:
         if n(self.user):
             self.start(
                 A.R_U.by_telephone_number(telephone_number or self.recipient).data  # type: ignore
             )
-            self.login = self.user.samAccountName  # type: ignore
+            self.login = self.user.login  # type: ignore
         return self.login  # type: ignore
 
     def get_user(self, telephone_number: str | None = None) -> User:
         if n(self.user):
             user = A.R_U.by_login(self.get_login(telephone_number), True, True).data
         else:
             user = self.user
@@ -294,36 +302,48 @@
 
 @dataclass
 class MessageHolder:
     body: str | None = None
     text_before: str = ""
 
     def to_string(self) -> str:
-        return j((self.text_before, self.body))  # type: ignore
+        return j((self.text_before, self.body))
 
 
 class MobileOutput(MobileOutputBase, Output):
+
+    @property
+    def choose_menu_item_str(self) -> str:
+        return "Пожалуйста, выберите пункт меню"
+
+    @property
+    def use_instance_mode(self) -> bool:
+        return self.session.is_outside
+
     def __init__(self, session: MobileSession):
         super().__init__(MobileUserOutput(), MobileMarkOutput())
+        self.session: MobileSession = session
         self.message_buffer: list[MessageHolder] = []
+        self.max_lines: int | None = (
+            None if self.use_instance_mode else MAX_MESSAGE_LINE_LENGTH
+        )
         self.thread_started: bool = False
-        self.session: MobileSession = session
         self.type: int = 0
-        self.instant_mode: bool = False
+        self.instant_mode: bool = self.use_instance_mode
         self.redirection: bool = False
         self.redirected_text_list: list[str] = []
         self.write_line_delay: float = 0.2
         self.recipient: str | None = None
         self.profile: A.CT.MESSAGE.WHATSAPP.WAPPI.Profiles = (
             A.CT.MESSAGE.WHATSAPP.WAPPI.Profiles.IT
         )
         self.flags: int = 0
         self.locked: bool = False
         self.show_exit_message: bool = True
-        self.exit_line: str | None = None
+        self.exit_message: str | None = None
         self.show_error: bool = True
 
     @contextmanager
     def make_exit_message_visibility(self, value: bool):
         value_before: bool = self.show_exit_message
         try:
             self.show_exit_message = value
@@ -362,23 +382,25 @@
         color: int,
         text: str,
         text_before: str | None = None,
         text_after: str | None = None,
     ) -> str:
         return text
 
-    def whatsapp_send(self, text: str) -> bool:
-        # A.L.debug_bot(text)
+    def break_line(self) -> None:
+        pass
+
+    def message_send(self, value: str) -> bool:
+        return self.message_send_to_whatsapp(value)
+
+    def message_send_to_whatsapp(self, value: str) -> bool:
         return A.ME_WH_W.send(
-            self.get_recipient(), A.D_F.whatsapp_message(text), self.profile
+            self.get_recipient(), A.D_F.whatsapp_message(value), self.profile
         )
 
-    def index_str(self, index: int, text: str, max_index: int | None = None) -> str:
-        return j(("<li>", super().index_str(index, text, max_index), "</li>"))
-
     @contextmanager
     def make_send_to_group(self, group: A.CT.MESSAGE.WHATSAPP.GROUP):
         try:
             while_not_do(lambda: e(self.message_buffer))
             self.recipient = A.D.get(group)
             yield True
         finally:
@@ -389,42 +411,48 @@
         try:
             self.type = BM.add(self.type, MessageType.SEPARATED)
             yield True
         finally:
             self.type = BM.remove(self.type, MessageType.SEPARATED)
 
     @contextmanager
-    def make_exit_line(self, value: str | None = None):
+    def make_(self, value: int, additional: bool = False):
+        indent: int = self.indent
+        try:
+            self.set_indent([0, indent][additional] + value)
+            yield True
+        finally:
+            self.set_indent(indent)
+
+    @contextmanager
+    def make_exit_message(self, value: str | None = None):
         if nn(value):
-            value = self.create_exit_line(
-                j((value, ": ")),
-                self.keywords.command.BACK,
-            )
+            value = self.create_exit_message(j((value, CONST.SPLITTER, " ")))
         try:
-            self.exit_line = (
-                j((nl(self.create_exit_line())))
+            self.exit_message = (
+                nl(self.create_exit_message())
                 if n(value)
                 else j(
                     (
                         nl("Отправьте:"),
                         " ",
                         A.CT_V.BULLET,
                         " ",
-                        self.create_exit_line("для выхода"),
+                        self.create_exit_message("для выхода"),
                         nl("или", reversed=None),
                         " ",
                         A.CT_V.BULLET,
                         " ",
                         value,
                     )
                 )
             )
             yield True
         finally:
-            self.exit_line = None
+            self.exit_message = None
 
     @contextmanager
     def make_personalized(self, enter: bool = True):
         if enter:
             try:
                 while_not_do(lambda: e(self.message_buffer))
                 self.personalize = True
@@ -458,16 +486,22 @@
         thread: PIHThread | None = None
 
         try:
 
             def show_loading() -> None:
                 sleep(loading_timeout)
                 if nn(thread):
-                    self.whatsapp_send(
-                        js(("", A.CT_V.WAIT, i(j((text or "Идёт загрузка", "...")))))
+                    self.message_send(
+                        js(
+                            (
+                                "",
+                                A.CT_V.WAIT,
+                                self.italics(j((text or "Идёт загрузка", "..."))),
+                            )
+                        )
                     )
 
             thread = PIHThread(show_loading)
             self.locked = True
             yield True
         finally:
             self.locked = False
@@ -477,28 +511,28 @@
         while self.locked:
             pass
         if not self.instant_mode:
             sleep(self.write_line_delay)
         message_list: list[MessageHolder] | None = None
 
         def get_next_part_messages() -> list[MessageHolder]:
-            max_lines: int = MAX_MESSAGE_LINE_LENGTH
+            max_lines: int | None = self.max_lines
             return (
                 self.message_buffer
-                if len(self.message_buffer) < max_lines
+                if n(max_lines) or len(self.message_buffer) < max_lines
                 else self.message_buffer[0:max_lines]
             )
 
         message_list = get_next_part_messages()
         while len(self.message_buffer) > 0:
             self.message_buffer = [
                 item for item in self.message_buffer if item not in message_list
             ]
             while_not_do(
-                lambda: self.whatsapp_send(
+                lambda: self.message_send(
                     jnl(A.D.map(self.add_text_before, message_list))
                 )
             )
             message_list = get_next_part_messages()
         self.thread_started = False
 
     def add_text_before(self, message_holder: MessageHolder) -> str:
@@ -510,85 +544,92 @@
                 message_holder.body.splitlines(),
             )
         )
 
     def get_recipient(self) -> str:
         return self.recipient or self.session.recipient
 
-    def write_line(self, text: str) -> None:
+    def personalize_text(self, value: str) -> str:
         if self.personalize:
             user_name: str | None = self.user.get_formatted_given_name()
             if ne(user_name):
-                text = j((user_name, ", ", A.D.decapitalize(text)))
+                value = j((user_name, ", ", A.D.decapitalize(value)))
+        return value
+
+    def write_line(self, text: str) -> None:
+        text = self.personalize_text(text)
         if self.redirection:
             self.redirected_text_list.append(text)
         elif ne(text):
             if not self.locked and BM.has(
                 self.type, [MessageType.SEPARATE_ONCE, MessageType.SEPARATED]
             ):
-                message_holder: MessageHolder = MessageHolder(text, self.text_before)
                 self.type = BM.remove(self.type, MessageType.SEPARATE_ONCE)
                 while self.thread_started:
                     pass
-                self.whatsapp_send(self.add_text_before(message_holder))
+                self.message_send(
+                    self.add_text_before(MessageHolder(text, self.text_before))
+                )
             else:
                 self.message_buffer.append(MessageHolder(text, self.text_before))
                 if not self.thread_started:
                     self.thread_started = True
                     PIHThread(self.internal_write_line, name="internal_write_line")
 
     def write_video(self, caption: str, video_content: str) -> None:
         return A.ME_WH_W.send_video(
-            self.session.recipient, caption, video_content, self.profile
+            self.get_recipient(), caption, video_content, self.profile
         )
 
     def write_image(self, caption: str, image_content: str) -> bool:
         return A.ME_WH_W.send_image(
-            self.session.recipient,
+            self.get_recipient(),
             A.D_F.whatsapp_message(j((self.text_before, caption))),
             image_content,
             self.profile,
         )
 
     def write_document(
         self, caption: str, file_name: str, document_content: str
     ) -> None:
         return A.ME_WH_W.send_document(
-            self.session.recipient, caption, file_name, document_content, self.profile
+            self.get_recipient(), caption, file_name, document_content, self.profile
         )
 
-    def create_exit_line(
+    def create_exit_message(
         self,
         title: str = "Для выхода, отправьте:",
-        keywords: list[str] = COMMAND_KEYWORDS.EXIT,
     ) -> str:
-        return i(
+        return self.italics(
             js(
                 (
                     title,
                     j(
                         A.D.map(
                             lambda item: self.bold(A.D.capitalize(item)),
-                            keywords,
+                            COMMAND_KEYWORDS.EXIT,
                         ),
                         " или ",
                     ),
                 )
             )
         )
 
     def input(self, value: str) -> None:
         self.separated_line()
-        with self.make_personalized(True):
-            with self.make_indent(2, True):
-                self.write_line(j((value, A.CT.SPLITTER)))
-                if self.show_exit_message:
-                    with self.make_indent(2):
-                        with self.make_personalized(False):
-                            self.write_line(self.exit_line or self.create_exit_line())
+        with self.make_indent(0):
+            with self.make_personalized(True):
+                with self.make_indent(2, True):
+                    self.write_line(j((value, A.CT.SPLITTER)))
+                    if self.show_exit_message:
+                        with self.make_indent(2):
+                            with self.make_personalized(False):
+                                self.write_line(
+                                    self.exit_message or self.create_exit_message()
+                                )
 
     def value(self, caption: str, value: Any, text_before: str | None = None) -> None:
         self.separated_line()
         self.write_line(j((self.bold(caption), ": ", value)))
 
     def good(self, value: str) -> None:
         self.write_line(nl(js((A.CT_V.GOOD, value))))
@@ -618,35 +659,32 @@
 
     def new_line(self) -> None:
         return
 
     def separated_line(self) -> None:
         self.type = BM.add(self.type, MessageType.SEPARATE_ONCE)
 
-    def header(self, value: str) -> None:
+    def paragraph(self, value: str) -> None:
         self.write_line(js(("", A.CT_V.BULLET, nl(self.bold(value)))))
 
     def bold(self, value: Any) -> str:
-        return j(("<b>", value, "</b>"))
-
-    # b(value)
+        return A.D.bold(value)
 
-    def italic(self, value: Any) -> str:
-        return j(("<i>", value, "</i>"))
-        # i(value)
+    def italics(self, value: Any) -> str:
+        return A.D.italics(value)
 
     def free_marks_by_group_for_result(
         self, group: MarkGroup, result: Result, use_index: bool
     ) -> None:
         group_name: str = nns(group.GroupName)
         self.write_line(
-            js(
+            j(
                 (
-                    "Свободные карты доступа для группы доступа",
-                    j((esc(group_name), ":")),
+                    "Свободные карты доступа для группы доступа ",
+                    esc(group_name), ":",
                 )
             )
         )
         self.write_result(
             result,
             use_index=False,
             data_label_function=lambda index, _, __, data_value: j((index + 1, ". "))
@@ -737,15 +775,15 @@
                                 + len(str(length))
                             )
                             if use_index
                             else ""
                         ),
                         A.D.list_to_string(
                             A.D.map(
-                                lambda item: i(item.caption),
+                                lambda item: self.italics(item.caption),
                                 A.D.filter(
                                     lambda item: item.visible,
                                     (
                                         field_list.get_list()[1:]
                                         if use_index
                                         else field_list.get_list()
                                     ),
@@ -767,19 +805,105 @@
                 )
 
     def free_marks_by_group_for_result(
         self, group: MarkGroup, result: Result, use_index: bool
     ) -> None:
         self.table_with_caption_last_title_is_centered(
             result,
-            f"Свободные карты доступа для группы доступа '{group.GroupName}':",
+            j(
+                (
+                    "Свободные карты доступа для группы доступа ",
+                    escs(group.GroupName),
+                    CONST.SPLITTER,
+                )
+            ),
             use_index,
         )
 
 
+class OutsideOutput(MobileOutput):
+
+    def __init__(self, session: MobileSession):
+        super().__init__(session)
+        self._buffer: list[strdict] = []
+
+    def break_line(self) -> None:
+        self.message_send(
+            {
+                "type": "break",
+                "value": nl(),
+            }
+        )
+
+    def index_str(
+        self,
+        caption: str,
+        min_value: int,
+        max_value: int,
+    ) -> str:
+        return js(
+            (
+                j((caption, ", выбрав")),
+                "(от",
+                min_value,
+                "до",
+                j((max_value, ")")),
+            )
+        )
+
+    def input(self, value: str) -> None:
+        with self.make_personalized(False):
+            self.message_send(
+                {
+                    "type": "input",
+                    "value": A.D.capitalize(value),
+                }
+            )
+            self.message_send(
+                {
+                    "type": "break",
+                    "value": self.exit_message or self.create_exit_message(),
+                },
+            )
+
+    def message_send(self, value: strdict) -> bool:
+        value["recipient"] = self.get_recipient()
+        flush: bool = value["type"] == "break"
+        self._buffer.append(value)
+        if flush:
+            text: str = A.D.rpc_encode(self._buffer, ensure_ascii=False)
+            print(text)
+            A.A._call(A.CT_SR.GATEWAY, text)
+            self._buffer = []
+        return True
+
+    def indexed_item(
+        self,
+        index: int,
+        text: str,
+        min_value: int | None = None,
+        max_value: int | None = None,
+    ) -> None:
+        self.message_send(
+            {
+                "type": "index_item",
+                "value": index,
+                "text": Output.indexed_item_str(self, index, text),
+            }
+        )
+
+    def write_line(self, text: str) -> None:
+        self.message_send(
+            {
+                "type": "text",
+                "value": text,
+            }
+        )
+
+
 class MobileMarkInput(MarkInput):
     pass
 
 
 class MobileUserInput(UserInput):
     def title_any(self, title: str | None = None) -> str:
         return self.parent.input(
@@ -808,23 +932,24 @@
         self.stdin: Stdin = stdin
         self.session = session
         self.data_input_timeout: int | None = (
             None
             if data_input_timeout == -1
             else (data_input_timeout or A.S.get(MOBILE_HELPER_USER_DATA_INPUT_TIMEOUT))
         )
-        self.type: int = 0
+        self.type = INPUT_TYPE.NO
 
     @contextmanager
     def make_type(self, value: int):
         try:
-            self.type = value
+            if self.type == INPUT_TYPE.NO:
+                self.type = value
             yield True
         finally:
-            self.type = 0
+            self.type = INPUT_TYPE.NO
 
     @contextmanager
     def make_input_timeout(self, value: int | None):
         data_input_timeout: int | None = self.data_input_timeout
         try:
             self.data_input_timeout = value
             yield True
@@ -856,105 +981,103 @@
 
     def input(
         self,
         caption: str | None = None,
         _: bool = True,
         check_function: Callable[[str], Any] | None = None,
     ) -> str:
-        input_data: str | None = None
-        while True:
-            if ne(caption):
-                with self.output.make_indent(0):
-                    self.output.input(caption)
-            self.stdin.wait_for_data_input = True
-
-            def internal_input() -> None:
-                start_time: int = 0
-                sleep_time: int = 1
-                while True:
-                    if not self.stdin.is_empty() or self.stdin.interrupt_type > 0:
-                        return
-                    sleep(sleep_time)
-                    start_time += sleep_time
-                    if (
-                        ne(self.data_input_timeout)
-                        and start_time > self.data_input_timeout
-                    ):
-                        self.stdin.interrupt_type = InterruptionTypes.TIMEOUT
-                        return
+        with self.make_type(INPUT_TYPE.NORMAL):
+            input_data: str | None = None
+            while True:
+                if ne(caption):
+                    self.output.input(nns(caption))
+                self.stdin.wait_for_data_input = True
+
+                def internal_input() -> None:
+                    start_time: int = 0
+                    sleep_time: int = 1
+                    while True:
+                        if not self.stdin.is_empty() or self.stdin.interrupt_type > 0:
+                            return
+                        sleep(sleep_time)
+                        start_time += sleep_time
+                        if (
+                            ne(self.data_input_timeout)
+                            and start_time > self.data_input_timeout
+                        ):
+                            self.stdin.interrupt_type = InterruptionTypes.TIMEOUT
+                            return
 
-            action_thread = PIHThread(internal_input, name="input_label")
-            action_thread.join()
+                action_thread = PIHThread(internal_input, name="input_label")
+                action_thread.join()
 
-            self.stdin.wait_for_data_input = False
-            input_data = self.stdin.data
-            if self.stdin.interrupt_type > 0:
-                interrupt_type: int = self.stdin.interrupt_type
+                self.stdin.wait_for_data_input = False
+                input_data = self.stdin.data
+                if self.stdin.interrupt_type > 0:
+                    interrupt_type: int = self.stdin.interrupt_type
+                    self.stdin.set_default_state()
+                    raise InternalInterrupt(interrupt_type)
                 self.stdin.set_default_state()
-                raise InternalInterrupt(interrupt_type)
-            self.stdin.set_default_state()
-            if n(check_function):
-                return input_data
-            else:
-                checked_input_data: str | None = check_function(input_data)
-                if nn(checked_input_data):
-                    return checked_input_data
+                if n(check_function):
+                    return input_data
+                else:
+                    checked_input_data: str | None = check_function(input_data)
+                    if nn(checked_input_data):
+                        return checked_input_data
 
     def yes_no(
         self,
         text: str,
         enter_for_yes: bool = False,
         yes_label: str = YES_LABEL,
         no_label: str = NO_LABEL,
         yes_checker: Callable[[str], bool] | None = None,
     ) -> bool:
         default_yes_label: bool = yes_label == YES_LABEL
         if not default_yes_label:
             yes_label = j((" ", A.CT.VISUAL.BULLET, " ", yes_label))
         if no_label != NO_LABEL:
             no_label = j((" ", A.CT.VISUAL.BULLET, " ", no_label))
-        text = j(
+        text = jnl(
             (
-                nl(j((text, A.CT_V.QUESTION))),
-                nl(LINE),
-                nl(yes_label),
-                nl("или"),
+                j((text, A.CT_V.QUESTION)),
+                LINE,
+                yes_label,
+                "или",
                 no_label,
             )
         )
         self.answer = self.input(text).lower().strip()
         return (
             (
                 self.answer in YES_VARIANTS
                 if default_yes_label
                 else self.answer not in ["0", "no", "нет"]
             )
             if n(yes_checker)
-            else yes_checker(self.answer)
+            else nnt(yes_checker)(self.answer)
         )
 
     def item_by_index(
         self,
         caption: str,
         data: list[Any],
         label_function: Callable[[Any, int], str] | None = None,
         use_zero_index: bool = False,
         allow_choose_all: bool = False,
         sticky_items: tuple[int, ...] | None = None,
-        # simple_integer_parse: bool = True,
     ) -> Any:
         with self.make_type(INPUT_TYPE.INDEX):
             return super().item_by_index(
-                j((caption, ", отправив число")),
+                caption,
                 data,
                 label_function,
                 use_zero_index,
                 allow_choose_all,
                 sticky_items,
-                # simple_integer_parse,
             )
 
     def interrupt_for_new_command(self) -> None:
         self.stdin.interrupt_type = InterruptionTypes.NEW_COMMAND
 
     def interrupt(self) -> None:
         self.stdin.interrupt_type = InterruptionTypes.EXIT
@@ -1146,15 +1269,15 @@
             (
                 "[",
                 j(
                     A.D.map(
                         self.output.bold,
                         flag_name_list(value, all),
                     ),
-                    j((" ", i("или"), " ")),
+                    j((" ", self.output.italics("или"), " ")),
                 ),
                 "]",
             )
         )
 
     def create_study_course_item(
         self,
@@ -1219,21 +1342,23 @@
                 nl(self.output.bold("709")),
                 "Сотовый телефон: ",
                 self.output.bold(A.D_TN.by_login("Administrator")),
             )
         )
 
     def long_operation_handler(self) -> None:
-        self.write_line(i("Ожидайте получения результата..."))
+        self.write_line(self.output.italics("Ожидайте получения результата..."))
 
     @staticmethod
     def polibase_status() -> str:
         resource: ResourceStatus | None = A.R_R.get_resource_status(A.CT_R_D.POLIBASE1)
         return A.D.check_not_none(
-            resource, lambda: j((A.D_F.yes_no(resource.accessable, True), " ")), ""  # type: ignore
+            resource,
+            lambda: j((A.D_F.yes_no(resource.accessable, True), " ")),
+            "",
         )
 
     @property
     def is_person_card_registry_folder(self) -> bool:
         name: str | None = self.arg()
         if n(name):
             return True
@@ -1267,27 +1392,17 @@
                             True,
                         ),
                     )
                 )
             )
 
     @property
-    def am_i_admin(self) -> bool:
-        return Groups.Admin in self.session.allowed_groups
-
-    @property
     def am_i_doctor(self) -> bool:
-        return self.is_doctor(self.session.user) or self.am_i_admin
+        return self.session.am_i_admin or A.C_U.doctor(self.session.user) 
 
-    def is_doctor(self, value: User) -> bool:
-        distinguishedName: str | None = value.distinguishedName
-        return ne(distinguishedName) and not (
-            distinguishedName.find("Доктор") == -1
-            and distinguishedName.find("Оператор") == -1
-        )
 
     def yes_no_adapted(
         self,
         text: str,
         _: bool = False,
         yes_label: str = YES_LABEL,
         no_label: str = NO_LABEL,
@@ -1332,16 +1447,16 @@
         self.language_index: int | None = None
         self.commandless_part_list: list[str] | None
         self.menu = MENU()
         self.keywords = KEYWORDS()
         self.return_result_key: str | None = None
         self.user_settings: UserSettings = UserSettings(self.session.login)
         # output stub rewrite
-        self.b = b
-        self.i = i
+        self.b = A.D.bold
+        self.i = A.D.italics
 
         def get_formatted_given_name(name: str | None = None) -> str | None:
             return self.output.bold(name or self.session.user_given_name)
 
         self.output.user.get_formatted_given_name = get_formatted_given_name
         #######################
         self.study_node: CommandNode = self.create_command_link(
@@ -1637,20 +1752,24 @@
                         lambda: MEDIA_CONTENT.VIDEO.HOLTER_FIX_ON_BODY,
                         title="Закрепление аппарата на теле пациента",
                     ),
                 ],
             ),
             HelpContentHolder(
                 "nn4",
-                [i("Памятка: Установка датчиков, карты и аккумулятора")],
+                [
+                    self.output.italics(
+                        "Памятка: Установка датчиков, карты и аккумулятора"
+                    )
+                ],
                 holter_study_course_help_content_image_list,
             ),
             HelpContentHolder(
                 "nn5",
-                [i("Памятка: Расположение датчиков на теле пациента")],
+                [self.output.italics("Памятка: Расположение датчиков на теле пациента")],
                 [
                     HelpImageContent(
                         lambda: MEDIA_CONTENT.IMAGE.HOLTER_DETECTORS_MAP, title=""
                     )
                 ],
             ),
             HelpContentHolder(
@@ -1743,34 +1862,34 @@
                 "выключить все" + (" компьютеры" if self.is_all else ""),
             ],
             lambda: self.shutdown_workstation_handler(True),
             ADMIN_GROUPS,
             filter_function=lambda: self.is_all,
             help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
-        find_workstation_node: CommandNode = CommandNode(
+        ws_find_node: CommandNode = CommandNode(
             self.keywords.command.FIND,
             lambda: [
                 "Поиск компьютера",
                 "Найти" + (" компьютер" if self.in_choose_command else ""),
             ],
-            self.find_workstation_handler,
+            self.ws_find_handler,
             filter_function=lambda: self.is_not_all or self.in_main_menu,
         )
         find_all_workstations_node: CommandNode = CommandNode(
             self.keywords.command.FIND,
             lambda: [
                 "Весь список компьютеров",
                 (
                     "Показать весь список компьютеров"
                     if self.in_choose_command
                     else "Весь список"
                 ),
             ],
-            lambda: self.find_workstation_handler(True),
+            lambda: self.ws_find_handler(True),
             filter_function=lambda: self.is_all,
             help_text=lambda: self.flag_string_represent(Flags.ALL),
         )
         msg_to_node: CommandNode = CommandNode(
             ["msg", "сообщение", "message"],
             lambda: [
                 "Отправка сообщения пользователю",
@@ -1831,15 +1950,15 @@
         )
         self.menu.workstation = [
             reboot_workstation_node,
             reboot_all_workstations_node,
             shutdown_workstation_node,
             shutdown_all_workstations_node,
             process_kill_node,
-            find_workstation_node,
+            ws_find_node,
             find_all_workstations_node,
             msg_to_node.clone_as(
                 title_and_label=lambda: [
                     "Отправка сообщения компьютеру",
                     "Отправить сообщение"
                     + (" компьютеру" if self.in_choose_command else ""),
                 ],
@@ -1905,15 +2024,15 @@
             self.keywords.command.FIND,
             lambda: [
                 "Поиск заметки",
                 j(("Найти", " заметку" if self.in_choose_command else "")),
             ],
             self.note_find_handler,
             # filter_function=lambda: self.in_choose_command,
-            help_text=lambda: js((" (", i("Название заметки"), ")")),
+            help_text=lambda: js((" (", self.output.italics("Название заметки"), ")")),
         )
         self.show_all_note_node: CommandNode = CommandNode(
             ["show", "показать"],
             lambda: [
                 "",
                 j(
                     (
@@ -1983,18 +2102,18 @@
             lambda: self.menu_handler(self.menu.hr_unit),
             text=lambda: j(
                 (
                     "Руководитель: ",
                     self.output.bold(
                         one(
                             A.R.filter(
-                                lambda item: not item.samAccountName.startswith(
+                                lambda item: not item.login.startswith(
                                     A.CT_AD.TEMPLATED_USER_SERACH_TEMPLATE[0]
                                 )
-                                and not item.samAccountName.endswith(
+                                and not item.login.endswith(
                                     A.CT_AD.TEMPLATED_USER_SERACH_TEMPLATE[-1]
                                 ),
                                 A.R_U.by_job_position(A.CT_AD.JobPositions.HR),
                             )
                         ).name
                     ),
                     nl("."),
@@ -2443,15 +2562,15 @@
                                 " Полибейс"
                                 if self.none_command or self.in_all_commands
                                 else ""
                             ),
                         )
                     ),
                 ]
-                if self.am_i_admin
+                if self.session.am_i_admin
                 else [
                     "Мой пароль Полибейс",
                     j(
                         (
                             "Показать мой пароль",
                             " Полибейс" if self.none_command else "",
                         )
@@ -2587,15 +2706,15 @@
         self.polibase_person_card_add_to_card_registry_folder_node: CommandNode = (
             CommandNode(
                 self.keywords.command.ADD,
                 polibase_person_add_to_card_registry_folder_title_and_label,
                 self.add_polibase_person_to_card_registry_folder_handler,
                 ADMIN_GROUPS + [Groups.CardRegistry],
                 text="Добавляет карту пациента в папку реестра",
-                help_text=lambda: f" {i('название папки')} {i('запрос для поиска пациента')}.\nНапример, {self.current_pih_keyword} + п1к {A.CT.TEST.PIN}",
+                help_text=lambda: f" {self.output.italics('название папки')} {self.output.italics('запрос для поиска пациента')}.\nНапример, {self.current_pih_keyword} + п1к {A.CT.TEST.PIN}",
                 filter_function=lambda: self.is_not_all or self.in_main_menu,
             )
         )
 
         def polibase_person_card_registry_folder_register_title_and_label() -> (
             list[str]
         ):
@@ -2757,42 +2876,42 @@
                 else self.output.bold("Список разделов:")
             ),
         )
         #######################
         self.address_node: CommandNode = self.create_command_link(
             j(("to", FLAG_KEYWORDS.ADDRESS_SYMBOL), "|"),
             FLAG_KEYWORDS.ADDRESS_SYMBOL,
-            i("Адресовать команду"),
+            self.output.italics("Адресовать команду"),
             ADMIN_GROUPS,
             True,
         )
         self.address_node.order = 2
         #######################
         self.address_as_link_node: CommandNode = self.create_command_link(
             j(("link", FLAG_KEYWORDS.LINK_SYMBOL), "|"),
             FLAG_KEYWORDS.LINK_SYMBOL,
-            i("Адресовать ссылку на команду"),
+            self.output.italics("Адресовать ссылку на команду"),
             ADMIN_GROUPS,
             True,
         )
         self.address_as_link_node.order = 3
         #######################
         self.all_commands_node: CommandNode = self.create_command_link(
             j((COMMAND_LINK_SYMBOL, j((self.flag_string_represent(Flags.ALL, True))))),
             FLAG_KEYWORDS.ALL_SYMBOL,
-            [i("Все команды")],
+            [self.output.italics("Все команды")],
             None,
             True,
         )
         self.all_commands_node.order = 1
         self.all_commands_node.filter_function = lambda: not self.in_choose_command
 
         about_pih_node: CommandNode = CommandNode(
             ["about", "o"],
-            [i("О PIH")],
+            [self.output.italics("О PIH")],
             text_decoration_after=lambda: (
                 ""
                 if not self.in_main_menu or self.has_help
                 else nl("...", reversed=True)
             ),
             text=lambda: jnl(
                 (
@@ -2802,30 +2921,30 @@
                             (
                                 nl(
                                     "Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации:"
                                 ),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
-                                self.output.bold("P"),
-                                " acific ",
-                                self.output.bold("I"),
-                                " nternational ",
-                                self.output.bold("H"),
-                                nl(" ospital "),
+                                # self.output.bold("P"),
+                                "Pacific ",
+                                # self.output.bold("I"),
+                                "International ",
+                                # self.output.bold("H"),
+                                nl("Hospital "),
                                 nl("или"),
                                 "   ",
                                 A.CT_V.BULLET,
                                 " ",
-                                self.output.bold("П"),
-                                " асифик ",
-                                self.output.bold("И"),
-                                " нтернешнл ",
+                                # self.output.bold("П"),
+                                "Пасифик ",
+                                # self.output.bold("И"),
+                                "Интернешнл ",
                                 self.output.bold("Х"),
-                                nl(" оспитал.", count=2),
+                                nl("Хоспитал.", count=2),
                                 self.output.bold("Автор"),
                                 ": ",
                                 nl("Караченцев Никита Александрович"),
                                 self.output.bold("Версия"),
                                 ": ",
                                 nl(VERSION),
                                 self.output.bold("Сервер"),
@@ -2849,15 +2968,15 @@
             show_in_main_menu=True,
             wait_for_input=False,
             show_always=True,
             order=4,
         )
         self.exit_node: CommandNode = CommandNode(
             self.keywords.command.EXIT,
-            [None, i(A.D.capitalize(self.keywords.command.EXIT[1]))],
+            [None, self.output.italics(A.D.capitalize(self.keywords.command.EXIT[1]))],
             self.session.exit,
             text_decoration_after=lambda: (
                 ""
                 if self.in_main_menu and not self.has_help
                 else nl("...", reversed=True)
             ),
             wait_for_input=False,
@@ -2868,15 +2987,15 @@
             self.exit_node.name_list,
             self.exit_node.title_and_label,
             self.exit_node.handler,
             wait_for_input=False,
         )
         #######################
         self.ws_node: CommandNode = CommandNode(
-            ["ws", "комп|ьютер"],
+            ["ws", "комп|ьютер", "сomp|uter"],
             ["Компьютер"],
             lambda: self.menu_handler(self.menu.workstation),
             text_decoration_before="🖥️ ",
             show_in_main_menu=True,
             help_text=lambda: (
                 self.flag_string_represent(Flags.ALL) if self.is_all else ""
             ),
@@ -2946,15 +3065,18 @@
             ),
             ADMIN_GROUPS + [Groups.RD, Groups.IndicationWatcher],
             text_decoration_before="☑️ ",
             show_in_main_menu=True,
         )
         polibase_node: CommandNode = CommandNode(
             self.keywords.command.POLIBASE,
-            lambda: [js(("Полибейс", MobileHelper.polibase_status())), "Полибейс"],
+            lambda: [
+                js(("Полибейс", MobileHelper.polibase_status())),
+                "Полибейс",
+            ],
             lambda: self.menu_handler(self.menu.polibase),  # type: ignore
             text_decoration_before=MobileHelper.polibase_status,
             show_in_main_menu=True,
         )
         help_node: CommandNode = CommandNode(
             ["help", "помощь"], [js(("Помощь", A.CT.VISUAL.ARROW))]
         )
@@ -2984,15 +3106,15 @@
                 if self.arg_len == 1
                 else self.menu_handler(self.menu.notes)
             ),
             text_decoration_before="📝 ",
             show_in_main_menu=True,
             filter_function=lambda: self.argless
             or A.C_N.exists(self.arg(), self.arg(), False),
-            help_text=lambda: js((" (", i("Название заметки"), ")")),
+            help_text=lambda: js((" (", self.output.italics("Название заметки"), ")")),
         )
 
         self.journal_node: CommandNode = CommandNode(
             self.keywords.command.JOURNALS,
             self.get_journal_title,
             lambda: (
                 self.show_journal_handler()
@@ -3205,19 +3327,21 @@
                     ),
                     ["Выполнение действия", "Действие"],
                 ),
                 self.create_action_handler,
                 ADMIN_GROUPS,
                 show_in_main_menu=True,
                 text_decoration_before="🎯 ",
-                help_text=lambda: js((" (", i("Название действия"), ")")),
+                help_text=lambda: js(
+                    (" (", self.output.italics("Название действия"), ")")
+                ),
                 # filter_function=lambda: self.argless or ne(A.D_ACT.get(self.arg())),
             ): None,
             CommandNode(
-                ["unit", "отдел"],
+                ["unit", "отдел|ы"],
                 ["Отделы"],
                 lambda: self.menu_handler(self.menu.unit),
                 text_decoration_before="🏥 ",
                 show_in_main_menu=True,
             ): None,
             it_unit_node: None,
             hr_unit_node: None,
@@ -3406,14 +3530,15 @@
                                         nl(),
                                         "     ",
                                         A.CT_V.HAND_INDICATE,
                                         self.output.bold(link_text),
                                     )
                                 )
                             )
+        self.output.break_line()
 
     def choose_file(
         self,
         search_request: str | None = None,
         filter_function: Callable[[str], bool] | None = None,
         command_type: A.CT_CMDT | None = None,
     ) -> File:
@@ -3476,15 +3601,15 @@
         )
         title_list: list[str] = file.title.split(A.CT.SPLITTER)  # type: ignore
         self.output.separated_line()
         if nn(search_request_source) and search_request_source in self.arg_list:
             self.arg_list.remove(search_request_source)
         command_type = command_type or A.D_Ex.command_type(file)
         if not (self.is_silence or self.is_only_result):
-            self.output.head1(
+            self.output.write_line(
                 js(
                     (
                         (
                             None
                             if n(command_type)
                             else j((self.output.bold(A.D.get(command_type)[0]), ": "))
                         ),
@@ -3545,15 +3670,21 @@
 
     def bold(self, value: Any) -> str:
         return self.output.bold(value)
 
     @property
     def arg_list_exclude_file(self) -> list[str]:
         return A.D.filter(
-            lambda item: not item.startswith(FILE_PATTERN_LIST), self.arg_list
+            lambda item: not arg_value_is_file(item), self.arg_list
+        )
+        
+    @property
+    def arg_list_only_file(self) -> list[str]:
+        return A.D.filter(
+            arg_value_is_file, self.arg_list
         )
 
     @property
     def check_for_arg_list_include_file(self) -> bool:
         return (self.arg_len - len(self.arg_list_exclude_file)) != 0
 
     def arg(
@@ -3630,15 +3761,15 @@
         )
 
     def zabbix_command_handler(self) -> None:
         self.console_apps_api.show_zabbix()
 
     def get_joke_handler(self, set_settings: bool = False) -> None:
         if set_settings:
-            if A.C_U.has_property(
+            if A.C_U.property(
                 nnt(self.session.user),
                 A.CT_AD_UP.Jokeless,
             ):
                 self.output.error(
                     j(
                         (
                             "Отправка анегдота при входе или выходе отключена Администратором.",
@@ -3801,15 +3932,15 @@
 
     def create_polibase_db_backup_handler(self) -> None:
         name: str = A.D.now_to_string(A.CT_P.DB_DATETIME_FORMAT)
         answer: bool | None = None
         test: bool = self.is_test
         if test:
             self.write_line(
-                i(
+                self.output.italics(
                     j(
                         (
                             self.user_given_name,
                             ", запущен тестовый процесс создания дампа базы данных",
                         )
                     )
                 )
@@ -3824,15 +3955,15 @@
                         self.output.bold(name),
                         "- отправьте",
                         A.O.get_number(0),
                     )
                 ),
             )
             self.write_line(
-                i(
+                self.output.italics(
                     j(
                         (
                             self.user_given_name,
                             ", ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе: ",
                             self.output.bold("Backup Console"),
                         )
                     )
@@ -3862,15 +3993,15 @@
             )
 
         def get_by_login(value: str) -> dict[str, Any] | None:
             return execute_query_for_password(
                 j(("lower(use_name)=", escs(value.lower())))
             )
 
-        if self.am_i_admin:
+        if self.session.am_i_admin:
             value: str = (
                 self.arg()
                 or self.input.polibase_person_any(
                     f"Введите:\n {A.CT_V.BULLET} персональный номер пользователя\n {A.CT_V.BULLET} часть имени пользователя\n {A.CT_V.BULLET} логин пользователя"
                 )
             ).lower()
             result = execute_query_for_password(
@@ -4074,15 +4205,15 @@
                             A.A_B.start_robocopy_job(
                                 job_status.name,
                                 job_status.source,
                                 job_status.destination,
                                 forced,
                             )
                         self.write_line(
-                            i(
+                            self.output.italics(
                                 js(
                                     (
                                         j((self.user_given_name, ",")),
                                         "ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе",
                                         self.output.bold("Backup Console"),
                                     )
                                 )
@@ -4128,15 +4259,15 @@
                 )
             else:
                 job_item = job_list[0]
             if A.A_B.start_robocopy_job(
                 job_name, job_item.source, job_item.destination, forced
             ):
                 self.write_line(
-                    i(
+                    self.output.italics(
                         j(
                             (
                                 self.user_given_name,
                                 ", ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе ",
                                 self.output.bold("Backup Console"),
                             )
                         )
@@ -4173,15 +4304,15 @@
         if self.is_silence_no:
             return False
         return self.input.yes_no(
             text, yes_label=yes_label, no_label=no_label, yes_checker=yes_checker
         )
 
     def save_media_efilm(self) -> None:
-        self.write_line(i("Идёт загрузка..."))
+        self.write_line(self.output.italics("Идёт загрузка..."))
         self.output.write_video(
             r"Как экспортировать исследование пациента из eFilm. Данные находятся в папке: *C:\Program Files (x86)\Merge Healthcare\eFilm\CD*",
             MEDIA_CONTENT.VIDEO.EXPORT_FROM_EFILM,
         )
 
     def under_construction_handler(self) -> None:
         self.output.error(f"Извините, {self.user_given_name}, раздел в разработке 😞")
@@ -4328,17 +4459,17 @@
                             )
                     else:
                         self.output.error(js(("Компьютер", value, "не найден")))
                 else:
 
                     def every_action(workstation: Workstation):
                         user_string: str = ""
-                        has_user: bool = ne(workstation.samAccountName)
+                        has_user: bool = ne(workstation.login)
                         if has_user:
-                            user_string = f" (им пользуется {A.R_U.by_login(workstation.samAccountName).data.name})"
+                            user_string = f" (им пользуется {A.R_U.by_login(workstation.login).data.name})"
                         if action_index == 0:
                             if all or (
                                 A.C_WS.rebootable(workstation)
                                 or (
                                     self.yes_no(
                                         js(
                                             (
@@ -4464,15 +4595,15 @@
         )
 
     def shutdown_workstation_handler(
         self, all: bool = False, raise_exception: bool = False
     ) -> None:
         self.workstation_action_handler(self.arg(), 1, all, raise_exception)
 
-    def find_workstation_handler(self, all: bool = False) -> None:
+    def ws_find_handler(self, all: bool = False) -> None:
         self.workstation_action_handler(self.arg(), 2, all)
 
     def where_handler(self) -> None:
         was_found: bool = False
         with self.output.make_allow_show_error(False):
             value: str = self.arg() or self.input.input("Введите поисковый запрос")
             if lw(value) == "я":
@@ -4581,33 +4712,29 @@
         def filter_function(item: Note) -> bool:
             title_list: list[str] = item.title.split(A.CT.SPLITTER)  # type: ignore
             if len(title_list) > 1:
                 return title_list[0].lower() in A.D.get(command_type)[1:]
             return True
 
         arg: Any = None
+        self.arg_list = A.D.sort(lambda item: int(not arg_value_is_file(item)), self.arg_list)
         if n(command_type):
             for i in range(max(1, self.arg_len)):
                 arg = self.arg(
                     i,
                     as_file=True,
                     filter_function=None if n(command_type) else filter_function,
                 )
                 if isinstance(arg, File):
                     self.run_command(
                         A.D_Ex.command_type(arg), arg.text, arg.title, test=self.is_test
                     )
                     break
         else:
-            if isinstance(arg, File):
-                self.run_command(
-                    A.D_Ex.command_type(arg), arg.text, arg.title, test=self.is_test
-                )
-            else:
-                self.run_command(command_type, arg, test=self.is_test)
+            self.run_command(command_type, arg, test=self.is_test)
 
     def run_file(
         self, value: File | str, redirect_output: bool = False, test: bool = False
     ) -> str | None:
         if isinstance(value, str):
             value = one(A.R_F.find(value))
 
@@ -5224,15 +5351,15 @@
                                 if len(gkeep_item_list) == 1
                                 else gkeep_item.title.upper()
                             ),
                             separated_all=True,
                         )
                         if ne(note.images):
                             self.write_line(
-                                i(
+                                self.output.italics(
                                     js(
                                         (
                                             "Ожидайте загрузку изображений:",
                                             len(note.images),
                                         )
                                     )
                                 )
@@ -5301,15 +5428,20 @@
                     j(
                         (
                             "Ввести параметры для действия",
                             (
                                 ""
                                 if e(action_description.parameters_description)
                                 else j(
-                                    (": ", i(action_description.parameters_description))
+                                    (
+                                        ": ",
+                                        self.output.italics(
+                                            action_description.parameters_description
+                                        ),
+                                    )
                                 )
                             ),
                         )
                     )
                 ):
                     parameters = [self.input.input("Введите параметры для действия")]
         if not action_description.confirm or self.yes_no(
@@ -5597,16 +5729,16 @@
         )
         report_file_path: str = A.PTH.join(
             A.PTH.MOBILE_HELPER.TIME_TRACKING_REPORT_FOLDER, report_file_name
         )
         allowed_report_for_all_persons: bool = (
             not for_me_report_only
             and not self.is_forced
-            and A.C_A.by_group(
-                Groups.TimeTrackingReport, False, self.session, True, False
+            and A.C_A.action_for_group(
+                Groups.TimeTrackingReport, self.session,  False, True, False
             )
         )
 
         if A.A_TT.save_report(
             report_file_path,
             start_date,
             end_date,
@@ -5867,15 +5999,15 @@
                             if is_video:
                                 loading_text += "видео"
                             else:
                                 loading_text += "изображения"
                             if len_content > 1:
                                 loading_text += f" [{index + 1} из {len_content}]"
                             loading_text += "..."
-                            self.write_line(i(loading_text))
+                            self.write_line(self.output.italics(loading_text))
                         if is_video:
                             self.output.write_video(title, content_body)
                         else:
                             self.output.write_image(title, content_body)
 
     def create_temporary_mark_handler(self) -> None:
         arg: str | None = self.arg()
@@ -5938,15 +6070,15 @@
                 )
         self.output.write_result(
             person_list_result,
             separated_result_item=False,
             data_label_function=lambda *parameters: data_label_function(
                 *parameters, len(person_list_result.data)
             ),
-            empty_result_text=i("Папка с картами пациентов пуста"),
+            empty_result_text=self.output.italics("Папка с картами пациентов пуста"),
             use_index=False,
             title=(
                 js(
                     (
                         "Список карт пациентов в папке ",
                         polibase_person_card_registry_folder,
                         nl(),
@@ -6347,15 +6479,15 @@
                                 if polibase_person.pin not in polibase_person_pin_list:
                                     added_polibase_person_list.append(polibase_person)
                                     registrator_person: PolibasePerson = ()
                                     if A.CR.set_folder_for_person(
                                         polibase_person_card_registry_folder,
                                         polibase_person,
                                         A.R_P.person_by_login(
-                                            self.session.user.samAccountName
+                                            self.session.user.login
                                         ).data,
                                         set_by_polibase=False,
                                     ):
                                         self.drop_args()
                                         self.output.separated_line()
                                         self.write_line(
                                             js(
@@ -6388,15 +6520,15 @@
                                             )
                                         )
                                     )
                                     A.CR.set_folder_for_person(
                                         polibase_person_card_registry_folder,
                                         polibase_person,
                                         A.R_P.person_by_login(
-                                            self.session.user.samAccountName
+                                            self.session.user.login
                                         ).data,
                                         set_by_polibase=False,
                                         already_set_by_polibase=True,
                                     )
                             break
                         except NotFound as error:
                             self.output.error(error)
@@ -6408,17 +6540,17 @@
                         self.output.separated_line()
                         self.write_line(
                             j(
                                 (
                                     nl("  Добавьте следующую карту пациента в папку"),
                                     nl("или"),
                                     "  ",
-                                    self.output.create_exit_line("отправьте"),
+                                    self.output.create_exit_message("отправьте"),
                                     " ",
-                                    i("для завершения"),
+                                    self.output.italics("для завершения"),
                                 )
                             )
                         )
         except InternalInterrupt as _interruption:
             interruption = _interruption
         if (
             ne(added_polibase_person_list)
@@ -6532,15 +6664,15 @@
                     ),
                     timestamp_description,
                 )
                 self.output.good("Временная метка создана")
                 break
         note_name: str | None = None
         if self.yes_no("Создать заметку для временной метки"):
-            self.output.header("Создание заметки для временной метки")
+            self.output.paragraph("Создание заметки для временной метки")
             note_name: str | None = None
             if self.yes_no(
                 js(
                     (
                         "Использовать название",
                         self.output.bold(timestamp_name),
                         "для заметки",
@@ -6582,15 +6714,15 @@
                     ),
                 )
             if n(note_name):
                 self.output.error("Заметка не создана")
             else:
                 self.output.good("Заметка создана")
         if self.yes_no("Сделать временную метку истекающей"):
-            self.output.header("Создание истекающей временной метки")
+            self.output.paragraph("Создание истекающей временной метки")
             life_time_holder: StorageVariableHolder | None = None
             expired_timestamp_name: str | None = None
             with self.output.make_indent(2):
                 life_time_holder = self.input.item_by_index(
                     "Выберите продолжительность (в месяцах)",
                     A.D_V.find("life_time") + A.D_V.find("duration"),
                     lambda item, _: j(
@@ -7132,15 +7264,15 @@
                         )
                     )
                 )
                 timestamp = timestamp + timedelta(hours=PERIOD)
             return timestamp
 
         if n(timestamp) or use_preset:
-            with self.output.make_exit_line():
+            with self.output.make_exit_message():
                 while True:
                     try:
                         if not use_preset:
                             timestamp = datetime(
                                 YEAR or A.D.now().year,
                                 int(
                                     self.input.input(
@@ -7148,18 +7280,20 @@
                                         check_function=lambda item: A.D_Ex.decimal(
                                             item, 1, 12
                                         ),
                                     )
                                 ),
                                 1,
                             )
-                        with self.output.make_exit_line("для выбора месяца"):
+                        with self.output.make_exit_message("для выбора месяца"):
                             while True:
                                 try:
-                                    with self.output.make_exit_line("для выбора дня"):
+                                    with self.output.make_exit_message(
+                                        "для выбора дня"
+                                    ):
                                         if not use_preset:
                                             timestamp = timestamp.replace(
                                                 day=int(
                                                     self.input.input(
                                                         "Введите число",
                                                         check_function=lambda item: A.D_Ex.decimal(
                                                             item,
@@ -7290,15 +7424,17 @@
                 result_label_list.append(
                     if_else(
                         e(polibase_person_pin_list),
                         js(
                             (
                                 "",
                                 A.CT_V.WARNING,
-                                self.output.bold(i(A.CT_FC.POSITION.default_value)),
+                                self.output.bold(
+                                    self.output.italics(A.CT_FC.POSITION.default_value)
+                                ),
                             )
                         ),
                         lambda: j(
                             (
                                 nl(
                                     js(
                                         (
@@ -7551,14 +7687,16 @@
             file_search_request: str,
             parameters: dict[str, Any] | list[tuple[str, Any]] | None = None,
             stdout_redirect: bool = True,
             catch_exceptions: bool = True,
             redirect_to_mobile_output: bool = False,
         ) -> str | None:
             result_parameters: dict[str, Any] = {}
+            if nn(parameters):
+                parameters = A.D.map(A.D.as_value, (parameters or {}))
             if isinstance(parameters, list):
                 for parameter_item in parameters:
                     result_parameters[parameter_item[0]] = parameter_item[1]
             else:
                 result_parameters = parameters or {}
             result_parameters["self"] = self
             if stdout_redirect:
@@ -7719,15 +7857,15 @@
             )
             MobileHelper.allowed_group_collection = allowed_group_set
         self.fill_allowed_group_list()
 
     def fill_allowed_group_list(self, session: Session | None = None) -> None:
         session = session or self.session
         for group in MobileHelper.allowed_group_collection:
-            A.C_A.by_group(group, False, session, False, False)
+            A.C_A.action_for_group(group, session=session,exit_on_access_denied=False,  notify_on_fail=False, notify_on_success=False, cached=True)
 
     def command_sort_function(self, value: list[CommandNode]) -> str:
         name_list: list[str] = []
         for item in value:
             name_list.append(
                 self.get_command_node_label(item) if n(item.order) else chr(item.order)
             )
@@ -7807,23 +7945,16 @@
                     lambda flag_information_item: flag_information_item[1],
                     self.flag_information,
                 )
             ]
         non_command_node_name_list: list[str] = []
         for arg_item in part_list:
             command_node_name_exists: bool = False
-            for command_node_name in MobileHelper.command_node_name_collection:
-                command_node_name_has_variants: bool = (
-                    command_node_name.find(COMMAND_NAME_VARIANT_SPLITTER) != -1
-                )
-                command_node_name_exists = command_node_name_exists or (
-                    (command_node_name_equal(arg_item, command_node_name))
-                    if command_node_name_has_variants
-                    else A.D.equal(arg_item, command_node_name)
-                )
+            for command_node_name_item in MobileHelper.command_node_name_collection:
+                command_node_name_exists = command_node_name_equals_to(command_node_name_item, arg_item)
                 if command_node_name_exists:
                     self.commandless_part_list.remove(arg_item)
                     break
             if not command_node_name_exists:
                 non_command_node_name_list.append(arg_item)
         for arg_item in non_command_node_name_list:
             part_list.remove(arg_item)
@@ -7857,15 +7988,15 @@
                 #
                 part_list: list[str] = self.parse_arguments(line)
                 #
 
                 if nn(arguments):
                     self.session.arg_list.extend(arguments)
 
-                source_part_list: list[str] = A.D.map(str.lower, list(part_list))
+                source_part_list: list[str] = A.D.map(lw, list(part_list))
                 part_list_length: int = len(part_list)
 
                 if part_list_length > 0:
                     filtered_command_list: list[list[CommandNode]] = A.D.filter(
                         self.command_list_filter_function, self.command_list
                     )
                     command_item: list[CommandNode]
@@ -7879,16 +8010,16 @@
 
                         temp_part_list: list[str] = list(source_part_list)
                         for source_part_item in source_part_list:
                             has_result: bool = False
                             for command_node_name in command_node_name_list:
                                 has_result = ne(
                                     command_node_name
-                                ) and command_node_name_equal(
-                                    source_part_item, command_node_name
+                                ) and command_node_name_equals_to(
+                                    command_node_name, source_part_item
                                 )
                                 if has_result:
                                     break
                             if has_result:
                                 temp_part_list.remove(source_part_item)
                                 if source_part_item in part_list:
                                     part_list.remove(source_part_item)
@@ -7905,23 +8036,23 @@
                 is_addressed_as_link: bool = self.has_flag(Flags.ADDRESS_AS_LINK)
                 if is_addressed or is_addressed_as_link:
                     with self.output.make_indent(2):
                         self.write_line(
                             nl(
                                 A.D.check(
                                     is_addressed,
-                                    i(
+                                    self.output.italics(
                                         j(
                                             (
                                                 self.user_given_name,
                                                 ", вы выбрали режим адресации команды пользователю.",
                                             )
                                         )
                                     ),
-                                    i(
+                                    self.output.italics(
                                         j(
                                             (
                                                 self.user_given_name,
                                                 ", вы выбрали режим адресации ссылки на команду пользователю.",
                                             )
                                         )
                                     ),
@@ -7951,39 +8082,39 @@
                             )
                         except NotFound as error:
                             recipient = None
                             self.output.error(error)
                         else:
                             if len(self.recipient_user_list) == 1:
                                 if (
-                                    self.recipient_user_list[0].samAccountName
+                                    self.recipient_user_list[0].login
                                     == self.session.get_login()
                                 ):
                                     self.output.error("Нельзя адресовать самому себе!")
                                     recipient = None
                                 else:
                                     break
                             else:
                                 self.recipient_user_list = A.D.filter(
-                                    lambda item: item.samAccountName
+                                    lambda item: item.login
                                     != self.session.get_login()
                                     and A.C.telephone_number(item.telephoneNumber),
                                     self.recipient_user_list,
                                 )
                                 if len(self.recipient_user_list) == 0:
                                     self.output.error("Нельзя адресовать самому себе!")
                                     recipient = None
                                 else:
                                     break
                 if nn(sender_user):
                     if ne(external_flags):
                         self.session.flags = BM.add(self.session.flags, external_flags)
                     if not BM.has(external_flags, Flags.SILENCE):
                         self.write_line(
-                            i(
+                            self.output.italics(
                                 f"{self.get_user_given_name(A.D.to_given_name(sender_user))}, отправил Вам команду:"
                             )
                         )
                 command_list_len: int = 0
                 if self.none_command:
                     command_list = A.D.filter(
                         lambda value: self.command_list_filter_function(
@@ -8129,15 +8260,15 @@
                 A.D.check(
                     len(name_list) > 1,
                     lambda: j(
                         (
                             "[ ",
                             j(
                                 A.D.map(lambda item: self.output.bold(item), name_list),
-                                j((" ", i("или"), " ")),
+                                j((" ", self.output.italics("или"), " ")),
                             ),
                             " ]",
                         )
                     ),
                     A.D.check(
                         len(name_list) > 0
                         and value.name_list != self.exit_node.name_list,
@@ -8208,30 +8339,30 @@
         command_list: list[list[CommandNode]] = A.D.filter(
             filter_function, self.command_list
         )
         command_list.sort(key=self.command_sort_function)
         session: Session | None = None
         if ne(self.recipient_user_list):
             session = Session()
-            session.login = self.recipient_user_list[0].samAccountName
+            session.login = self.recipient_user_list[0].login
             self.fill_allowed_group_list(session)
 
         def label_function(command: list[CommandNode], _: int) -> str:
             command_node: CommandNode = command[0]
             return j(
                 (
                     A.D.as_value(command_node.text_decoration_before),
                     self.output.bold(self.get_command_label(command)),
                     A.D.as_value(command_node.description),
                     A.D.as_value(command_node.text_decoration_after),
                 )
             )
 
         command: list[CommandNode] = self.command_by_index(
-            "Пожалуйста, выберите пункт меню",
+            self.output.choose_menu_item_str,
             A.D.filter(
                 lambda item: self.command_list_filter_function(item, session),
                 command_list,
             ),
             label_function,
             True,
         )
@@ -8288,15 +8419,15 @@
                         for command_node in value:
                             if not command_node.wait_for_input:
                                 is_cyclic = False
                                 break
                     if is_cyclic:
                         self.output.separated_line()
                         self.write_line(
-                            i(
+                            self.output.italics(
                                 js(
                                     (
                                         self.output.bold(PIH.NAME.upper()),
                                         "будет выполнять команду в зацикленном режиме.",
                                     )
                                 )
                             )
@@ -8350,15 +8481,15 @@
                             nl(),
                             " ",
                             A.CT_V.BULLET,
                             " ",
                             "[ ",
                             j(
                                 A.D.map(b, self.keywords.command.PIH),
-                                j((" ", i("или"), " ")),
+                                j((" ", self.output.italics("или"), " ")),
                             ),
                             " ]",
                             " ",
                             js(
                                 A.D.map(
                                     self.get_command_node_help_label,
                                     A.D.filter(
@@ -8396,39 +8527,39 @@
         )
 
     def wait_for_input(self) -> bool:
         return self.stdin.wait_for_data_input
 
     def do_input(self, line: str):
         line = nns(A.D.space_format(line))
-        data: str | None = None
+        index_data: str | None = None
+        arg_list: list[str] = []
         if self.stdin.wait_for_data_input:
             self.stdin.interrupt_type = 0
             lower_line: str = nns(lw(line))
             if lower_line in self.keywords.command.EXIT:
                 interrupt_type = InterruptionTypes.EXIT
                 self.stdin.interrupt_type = interrupt_type
                 self.return_result(interrupt_type=interrupt_type)
             if lower_line in self.keywords.command.BACK:
                 self.stdin.interrupt_type = InterruptionTypes.BACK
             values: tuple[list[str], tuple[str]] = A.D.separate_unquoted_and_quoted(
                 line.strip()
             )
-            index_input: bool = self.input.type == INPUT_TYPE.INDEX
+            index_input_type: bool = self.input.type == INPUT_TYPE.INDEX
             for index, arg_item in enumerate(
                 A.D.not_empty_items(values[0] + values[1])
             ):
                 if arg_item in FLAG_MAP:
                     flag: Flags = FLAG_MAP[arg_item]
                     self.flags = BM.add(self.flags, flag)
                     self.flag_information.append((index, arg_item, flag))
-                if index_input:
-                    if n(data) and A.D_C.decimal(arg_item):
-                        data = arg_item
+                if index_input_type:
+                    if n(index_data) and A.D_C.decimal(arg_item):
+                        index_data = arg_item
                     else:
-                        self.arg_list.append(arg_item)
-            # if index_input:
-            #    if n(data):
-            #        if ne(self.arg_list):
-            #            self.arg_list[0] = None
-            data = data or line
-            self.stdin.data = data
+                        arg_list.append(arg_item)
+            if index_input_type:
+                if nn(index_data):
+                    self.arg_list.extend(arg_list)
+            index_data = index_data or line
+            self.stdin.data = index_data
```

### Comparing `pih-mio-0.29.8/MobileHelperService/client.py` & `pih-mio-0.30/MobileHelperService/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,29 +64,29 @@
         recipient_as_whatsapp_group: bool = recipient.endswith(A.CT_ME_WH.GROUP_SUFFIX)  # type: ignore
         output: MobileOutput = MobileOutput(session)
         session.output = output
         if not recipient_as_whatsapp_group:
             output.user.get_formatted_given_name = lambda: format_given_name(
                 session, output  # type: ignore
             )  # type: ignore
-            session.say_hello(recipient)  # type: ignore
+            session.hello(recipient)  # type: ignore
         return output
 
     @staticmethod
     def waiting_for_result(
         command: str,
         recipient: str | Enum,
         chat_id: str | Enum | None = None,
         flags: int | None = None,
         args: tuple[Any] | None = None,
     ) -> Any | None:
         recipient = A.D.get(recipient)
         chat_id = A.D.get(chat_id)
         return_result_key: str = A.D.uuid()
-        A.A_MIO.send_command_to(
+        A.A_MIO.send(
             command, recipient, chat_id, flags, return_result_key, args
         )
 
         class DH:
             exception: BaseException | None = None
 
         def internal_handler(pl: ParameterList, listener: IClosable) -> None:
```

### Comparing `pih-mio-0.29.8/MobileHelperService/const.py` & `pih-mio-0.30/MobileHelperService/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum, auto
 
 import ipih
 
 from pih import A
-from pih.tools import j, js, b
+from pih.tools import j, js
 from pih.consts.hosts import Hosts
 from pih.consts import CONST, SessionFlags
 from pih.collections.service import ServiceDescription
 from pih.collections import StorageVariableHolder, IntStorageVariableHolder
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.29.8"
+VERSION: str = "0.30"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
@@ -42,18 +42,14 @@
     NEW_COMMAND = 1
     TIMEOUT = 2
     EXIT = 3
     BACK = 4
     CANCEL = 5
 
 
-class INPUT_TYPE:
-    INDEX: int = 1
-
-
 FROM_FILE_REDIRECT_SYMBOL: str = "<"
 FILE_PATTERN_LIST: tuple[str, ...] = (
     j(("file", CONST.SPLITTER)),
     FROM_FILE_REDIRECT_SYMBOL,
     "file=",
 )  # type: ignore
 PARAMETER_PATTERN: str = r"\B(\$[\w+а-яА-Я]+)(:[\w \(\)\.\,а-яА-Я]+)?"
@@ -89,16 +85,16 @@
     ASK_YES_NO: list[str] = ["ask_yes_no"]
     SCAN: list[str] = ["scan|ed"]
     REGISTRY: list[str] = ["registry", "реестр"]
     CARD: list[str] = ["card", "карт"]
 
 
 YES_VARIANTS: tuple[str, ...] = ("1", "yes", "ok", "да")
-YES_LABEL: str = js(("", A.CT.VISUAL.BULLET, b("Да"), "- отправьте", A.O.get_number(1)))
-NO_LABEL: str = js(("", A.CT.VISUAL.BULLET, b("Нет"), "- отправьте", A.O.get_number(0)))
+YES_LABEL: str = js(("", A.CT.VISUAL.BULLET, A.D.bold("Да"), "- отправьте", A.O.get_number(1)))
+NO_LABEL: str = js(("", A.CT.VISUAL.BULLET, A.D.bold("Нет"), "- отправьте", A.O.get_number(0)))
 
 
 class Flags(Enum):
     CYCLIC = 1
     ADDRESS = 2
     ALL = 4
     ADDRESS_AS_LINK = 8
@@ -107,14 +103,15 @@
     HELP = 64
     SILENCE_NO = 128
     SILENCE_YES = 256
     CLI = SessionFlags.CLI.value
     ONLY_RESULT = 1024
     TEST = 2048
     SETTINGS = 4096
+    OUTSIDE = SessionFlags.OUTSIDE.value
 
 
 class FLAG_KEYWORDS:
     ALL_SYMBOL: str = "*"
     ADDRESS_SYMBOL: str = ">"
     LINK_SYMBOL: str = ADDRESS_SYMBOL * 2
     SILENCE: str = "_"
```

### Comparing `pih-mio-0.29.8/MobileHelperService/service.py` & `pih-mio-0.30/MobileHelperService/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import ipih
 
 from pih import A
 from pih.tools import nn, ne
 
-from MobileHelperService.service_api import MobileHelperService
+from MobileHelperService.service_api import MobileHelperService, sender_is_outside
 
 
-def checker(telephone_number: str) -> bool:
+def checker(telephone_number: str, flags: int | None) -> bool:
+    as_outside: bool = sender_is_outside(flags)
     if ne(A.SRV.get_support_host_list(A.CT_SR.MOBILE_HELPER)):
-        pih_cli_group_name: str = A.D.get(A.CT_ME_WH.GROUP.PIH_CLI) 
-        pih_cli_administator_login: str | None = A.S.get(A.CT_S.PIH_CLI_ADMINISTRATOR_LOGIN)
-        is_alisa: bool = telephone_number.endswith(A.CT_ME_WH.ALISA_SUFFIX)
-        as_administrator: bool = telephone_number == pih_cli_group_name or (
-            nn(pih_cli_administator_login) and telephone_number == A.D_TN.by_login(pih_cli_administator_login)
+        pih_cli_group_name: str = A.D.get(A.CT_ME_WH.GROUP.PIH_CLI)
+        pih_cli_administator_login: str | None = A.S.get(
+            A.CT_S.PIH_CLI_ADMINISTRATOR_LOGIN
+        )
+        
+        serve: bool = (
+            telephone_number == pih_cli_group_name
+            or (
+                nn(pih_cli_administator_login)
+                and telephone_number == A.D_TN.by_login(pih_cli_administator_login)
+            )
+            or as_outside
         )
         if MobileHelperService.as_administator():
-            return as_administrator
-        return not as_administrator
+            return serve
+        return not serve
     return True
 
 
 if __name__ == "__main__":
     MobileHelperService(checker=checker).start()
```

### Comparing `pih-mio-0.29.8/MobileHelperService/service_api.py` & `pih-mio-0.30/MobileHelperService/service_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from MobileHelperService.api import (
     Flags,
+    Output,
+    OutsideOutput,
     MobileInput,
     MobileOutput,
     MobileSession,
     MobileUserInput,
     MobileMarkInput,
     get_wappi_status,
     InternalInterrupt,
     MobileHelper as Api,
     AddressedInterruption,
 )
 from pih.console_api import LINE
 from pih.consts.errors import NotFound
 from MobileHelperService.const import *
-from pih import A, PIH, Stdin, PIHThread
+from pih import A, PIH, Stdin, PIHThread, send_message, isolate
 from pih.tools import (
     j,
-    b,
     n,
-    i,
     e,
     nn,
     nl,
     js,
     ne,
     lw,
     one,
@@ -49,14 +49,18 @@
         A.D.filter(
             lambda item: lw(item[0]).endswith("cli"),
             A.D.to_list(A.CT_ME_WH.GROUP, None),  # type: ignore
         ),
     )
 
 
+def sender_is_outside(flags: int | None) -> bool:
+    return BM.has(flags, Flags.OUTSIDE)
+
+
 class MobileHelperService:
 
     is_administrator: bool = False
 
     @staticmethod
     def as_administator() -> bool:
         return MobileHelperService.is_administrator or not A.D.contains(A.SYS.host(), SD.host)  # type: ignore
@@ -66,19 +70,19 @@
         return A.SE.named_arg(COUNT_ALIAS)  # type: ignore
 
     mobile_helper_client_map: dict[str, Api] = {}
 
     def __init__(
         self,
         max_client_count: int | None = None,
-        checker: Callable[[str], bool] | None = None,
+        checker: Callable[[str, int | None], bool] | None = None,
     ):
         self.max_client_count: int | None = max_client_count or DEFAULT_COUNT
         self.root: str = PIH.NAME
-        self.checker: Callable[[str], bool] | None = checker
+        self.checker: Callable[[str, int | None], bool] | None = checker
         self.service_description: ServiceDescription = SD
         self.allow_send_to_next_service_in_chain: dict[str, bool] = defaultdict(bool)
 
     def start(self, as_standalone: bool = False) -> bool:
         A.SE.add_isolated_arg()
         A.SE.add_arg(ADMIN_ALIAS, nargs="?", const="True", type=str, default="False")
         A.SE.add_arg(COUNT_ALIAS, nargs="?", const=1, type=int, default=DEFAULT_COUNT)
@@ -97,15 +101,15 @@
             MobileHelperService.is_administrator = False
 
         def service_starts_handler() -> None:
             if MobileHelperService.as_administator():
                 self.create_mobile_helper(
                     A.CT_ME_WH_G.PIH_CLI,
                     None,
-                    A.D_U.by_login(A.S.get(A.CT_S.PIH_CLI_ADMINISTRATOR_LOGIN)).telephoneNumber,
+                    A.D_TN.by_login(A.S.get(A.CT_S.PIH_CLI_ADMINISTRATOR_LOGIN)),
                 )
             MobileHelperService.service_starts_handler()
 
         if ne(service_desctiption):
             A.SRV_A.serve(
                 service_desctiption,
                 self.service_call_handler,  # type: ignore
@@ -119,20 +123,25 @@
     def create_mobile_helper(
         self,
         sender: str | A.CT_ME_WH_G,
         external_flags: int | None = None,
         recipient: str | None = None,
     ) -> Api:
         sender_value: str = A.D.get(sender)
+        sender = sender_value
         is_cli: bool = sender_is_cli(sender_value)
         if is_cli:
             external_flags = BM.add(external_flags, Flags.CLI)
         stdin: Stdin = Stdin()
         session: MobileSession = MobileSession(sender_value, external_flags)
-        output: MobileOutput = MobileOutput(session)
+        output: Output = (
+            OutsideOutput(session)
+            if sender_is_outside(external_flags)
+            else MobileOutput(session)
+        )
         try:
             session.say_hello(recipient)
             if not is_cli:
                 output.write_line(
                     j(
                         (
                             (
@@ -153,109 +162,115 @@
                                 )
                                 if not BM.has(session.flags, Flags.ONLY_RESULT)
                                 else None
                             ),
                             " ",
                             A.CT_V.WAIT,
                             " ",
-                            i("Ожидайте..."),
+                            A.D_F.italics("Ожидайте..."),
                         )
                     )
                 )
         except NotFound as error:
             output.error(
                 "К сожалению, не могу идентифицировать Вас. ИТ отдел добавит Вас после окончания процедуры идентификации."
             )
             raise error
         as_administrator: bool = is_cli
         if not as_administrator:
             try:
                 as_administrator = A.C_U.by_group(
-                    nnt(A.R_U.by_telephone_number(sender_value).data), A.CT_AD.Groups.Admin
+                    nnt(A.R_U.by_telephone_number(sender_value).data),
+                    A.CT_AD.Groups.Admin,
                 )
             except NotFound as _:
                 pass
         input: MobileInput = MobileInput(
             stdin,
             MobileUserInput(),
             MobileMarkInput(),
             output,
             session,
             [None, -1][as_administrator],
         )
         api: Api = Api(PIH(input, output, session), stdin)
         if is_cli:
             api.external_flags = external_flags
-        MobileHelperService.mobile_helper_client_map[sender_value] = api
+        MobileHelperService.mobile_helper_client_map[sender] = api
         return api
 
     @staticmethod
-    def say_good_bye(mobile_helper: Api, with_error: bool = False) -> None:
+    def good_bye(mobile_helper: Api, with_error: bool = False) -> None:
         mobile_helper.say_good_bye(with_error=with_error)
         mobile_helper.show_good_bye = False
 
     def pih_handler(
         self,
         sender: str,
         line: str | None = None,
         sender_user: User | None = None,
         external_flags: int | None = None,
         chat_id: str | None = None,
         return_result_key: str | None = None,
         args: tuple[Any] | None = None,
     ) -> None:
         mobile_helper: Api | None = None
-        is_cli: bool = sender_is_cli(sender)
+        no_need_for_pih_keyword: bool = sender_is_cli(sender) or sender_is_outside(
+            external_flags
+        )
         while True:
             try:
                 if MobileHelperService.is_client_new(sender):
                     A.IW.remove(A.CT_P.NAMES.PERSON_PIN, sender)
-                    if is_cli or Api.check_for_starts_with_pih_keyword(line):
+                    if (
+                        no_need_for_pih_keyword
+                        or Api.check_for_starts_with_pih_keyword(line)
+                    ):
                         self.allow_send_to_next_service_in_chain[sender] = (
                             self.is_client_stack_full()
                         )
                         if not self.allow_send_to_next_service_in_chain[sender]:
                             self.create_mobile_helper(sender, external_flags, chat_id)
                     else:
                         self.allow_send_to_next_service_in_chain[sender] = False
                 else:
                     self.allow_send_to_next_service_in_chain[sender] = False
                 if sender in MobileHelperService.mobile_helper_client_map:
                     mobile_helper = MobileHelperService.mobile_helper_client_map[sender]
-                    if is_cli and not mobile_helper.wait_for_input():
+                    if no_need_for_pih_keyword and not mobile_helper.wait_for_input():
                         if not Api.check_for_starts_with_pih_keyword(line):
                             line = js((self.root, line))
                     try:
                         if mobile_helper.do_pih(
                             line, sender_user, external_flags, return_result_key, args  # type: ignore
                         ):
                             if mobile_helper.show_good_bye:
                                 if not mobile_helper.is_only_result:
-                                    MobileHelperService.say_good_bye(mobile_helper)
+                                    MobileHelperService.good_bye(mobile_helper)
                     except BaseException as error:
                         is_error: bool = not isinstance(error, InternalInterrupt)
                         if not mobile_helper.is_only_result and is_error:
-                            MobileHelperService.say_good_bye(
+                            MobileHelperService.good_bye(
                                 mobile_helper, with_error=is_error
                             )
                         raise error
                 break
             except NotFound:
                 break
             except InternalInterrupt as interruption:
                 if interruption.type == InterruptionTypes.NEW_COMMAND:
                     line = nnt(mobile_helper).line
                     if not Api.check_for_starts_with_pih_keyword(line):
-                        MobileHelperService.say_good_bye(nnt(mobile_helper))
+                        MobileHelperService.good_bye(nnt(mobile_helper))
                         break
                 elif interruption.type in (
                     InterruptionTypes.TIMEOUT,
                     InterruptionTypes.EXIT,
                 ):
-                    MobileHelperService.say_good_bye(nnt(mobile_helper))
+                    MobileHelperService.good_bye(nnt(mobile_helper))
                     break
 
     def is_client_stack_full(self) -> bool:
         max_client_count: int | None = self.max_client_count
         if n(max_client_count):
             max_client_count = MobileHelperService.count()
         return len(MobileHelperService.mobile_helper_client_map) == max_client_count
@@ -283,35 +298,35 @@
                         None,
                         external_flags,
                         chat_id,
                         return_result_key,
                         args,
                     )
                 else:
-                    for recipient_user in interruption.recipient_user_list(): # type: ignore
+                    for recipient_user in interruption.recipient_user_list():  # type: ignore
                         recipient_user: User = recipient_user
                         self.pih_handler(
                             nnt(recipient_user.telephoneNumber),
                             js((self.root, nnt(interruption).command_name)),
                             nnt(interruption).sender_user,
                             nnt(interruption).flags,
                         )
                     interruption = None
                 break
             except AddressedInterruption as local_interruption:
                 interruption = local_interruption
 
     def receive_message_handler_thread_handler(self, message: WhatsAppMessage) -> None:
         self.receive_message_handler(
-            nnt(nnt(message).message),
-            nnt(nnt(message).sender),
-            nnt(message).flags,
-            nnt(message).chatId,
-            nnt(message).return_result_key,
-            nnt(message).args,
+            nnt(message.message),
+            nnt(message.sender),
+            message.flags,
+            message.chatId,
+            message.return_result_key,
+            message.args,
         )
 
     def service_call_handler(
         self,
         sc: SC,
         parameter_list: ParameterList,
         subscribtion_result: SubscribtionResult | None,
@@ -320,34 +335,38 @@
             if nn(subscribtion_result) and nnt(subscribtion_result).result:
                 if nnt(subscribtion_result).type == A.CT_SubT.ON_RESULT_SEQUENTIALLY:
                     message: WhatsAppMessage | None = A.D_Ex_E.whatsapp_message(
                         parameter_list
                     )
 
                     if nn(message):
+                        nn_message: WhatsAppMessage = nnt(message)
                         if (
                             A.D.get_by_value(
-                                A.CT_ME_WH_W.Profiles, nnt(message).profile_id # type: ignore
+                                A.CT_ME_WH_W.Profiles, nn_message.profile_id  # type: ignore
                             )
                             == A.CT_ME_WH_W.Profiles.IT
                         ):
-                            sender_as_cli: bool = sender_is_cli(nnt(nnt(message).chatId))
-                            allow_for_group: bool = ne(
-                                nnt(message).chatId
-                            ) and sender_as_cli
-                            if n(nnt(message).chatId) or allow_for_group:
+                            flags: int | None = nn_message.flags
+                            sender_as_cli: bool = sender_is_cli(nnt(nn_message.chatId))
+                            allow_for_group: bool = (
+                                ne(nn_message.chatId) and sender_as_cli
+                            )
+                            if n(nn_message.chatId) or allow_for_group:
                                 telephone_number: str = if_else(
                                     allow_for_group,
-                                    nnt(message).chatId,
-                                    nnt(message).sender,
+                                    nn_message.chatId,
+                                    nn_message.sender,
                                 )
                                 if allow_for_group:
-                                    nnt(message).chatId = nnt(message).sender
-                                    nnt(message).sender = telephone_number
-                                if n(self.checker) or nnt(self.checker)(telephone_number):
+                                    nn_message.chatId = nn_message.sender
+                                    nn_message.sender = telephone_number
+                                if n(self.checker) or nnt(self.checker)(
+                                    telephone_number, flags
+                                ):
                                     if self.is_client_stack_full():
                                         return True
                                     else:
                                         if (
                                             telephone_number
                                             in self.allow_send_to_next_service_in_chain
                                         ):
@@ -377,14 +396,16 @@
                                         ]
                                     return True
             return False
         return None
 
     @staticmethod
     def service_starts_handler() -> None:
+        isolate(A.CT_SR.GATEWAY)
+        
         A.O.write_line(nl())
         A.O.blue("Configuration:")
         as_administrator: bool = MobileHelperService.as_administator()
         with A.O.make_indent(1):
             A.O.value("As admin", str(as_administrator))
             if not as_administrator:
                 A.O.value("Count", str(MobileHelperService.count()))
@@ -393,35 +414,34 @@
             A.CT_SubT.ON_RESULT_SEQUENTIALLY,
             SD.name,
         )
         profile = A.CT_ME_WH_W.Profiles
         if as_administrator:
             space: str = "     "
 
-            A.ME_WH_W_Q.add_message(
-                Message(
-                    j(
-                        (
-                            " ",
-                            A.CT_V.ROBOT,
-                            " ",
-                            nl(b("Pih cli запущен...")),
-                            nl(js((space, b("Сервер:"), A.SYS.host()))),
-                            js((space, b("Версия:"), VERSION_STRING)),
-                            nl(),
-                            space,
-                            LINE,
-                            nl(),
-                            get_wappi_status(space, profile.IT),
-                            nl() * 2,
-                            get_wappi_status(space, profile.CALL_CENTRE),
-                            nl() * 2,
-                            get_wappi_status(space, profile.MARKETER),
-                        )
-                    ),
-                    A.D.get(A.CT_ME_WH.GROUP.PIH_CLI),
-                    A.D.get(profile.IT),
-                )
+            send_message(
+                j(
+                    (
+                        " ",
+                        A.CT_V.ROBOT,
+                        " ",
+                        nl(A.D.bold("Pih cli запущен...")),
+                        nl(js((space, A.D.bold("Сервер:"), A.SYS.host()))),
+                        js((space, A.D.bold("Версия:"), VERSION_STRING)),
+                        nl(),
+                        space,
+                        LINE,
+                        nl(),
+                        get_wappi_status(space, profile.IT),
+                        nl() * 2,
+                        get_wappi_status(space, profile.CALL_CENTRE),
+                        nl() * 2,
+                        get_wappi_status(space, profile.MARKETER),
+                    )
+                ),
+                A.D.get(A.CT_ME_WH.GROUP.PIH_CLI),
+                profile.IT,
+                
             )
 
         for item in one(A.R_F.find("@mobile_helper_import_module_list")).text.splitlines():  # type: ignore
             A.R_F.execute(item)
```

