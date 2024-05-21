# Comparing `tmp/pih-0.37.tar.gz` & `tmp/pih-0.37.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.37.tar", last modified: Mon May 20 23:05:23 2024, max compression
+gzip compressed data, was "pih-0.37.1.tar", last modified: Tue May 21 13:51:29 2024, max compression
```

## Comparing `pih-0.37.tar` & `pih-0.37.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.483360 pih-0.37/
--rw-rw-rw-   0        0        0      247 2024-05-20 23:05:23.436483 pih-0.37/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:20.538872 pih-0.37/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:21.285612 pih-0.37/pih/collections/
--rw-rw-rw-   0        0        0    30339 2024-05-17 03:55:00.000000 pih-0.37/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37/pih/collections/service.py
--rw-rw-rw-   0        0        0   104237 2024-05-17 04:58:32.000000 pih-0.37/pih/console_api.py
--rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:22.951668 pih-0.37/pih/consts/
--rw-rw-rw-   0        0        0    26747 2024-05-20 22:38:29.000000 pih-0.37/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37/pih/consts/errors.py
--rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37/pih/consts/hosts.py
--rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37/pih/consts/iot.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.37/pih/consts/password.py
--rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37/pih/consts/paths.py
--rw-rw-rw-   0        0        0    16020 2024-05-20 22:44:51.000000 pih-0.37/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37/pih/consts/service.py
--rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    17765 2024-05-20 04:39:33.000000 pih-0.37/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37/pih/consts/style.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   572231 2024-05-20 02:59:52.000000 pih-0.37/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.186465 pih-0.37/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.342733 pih-0.37/pih/tools/
--rw-rw-rw-   0        0        0    59031 2024-05-20 00:30:59.000000 pih-0.37/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:05:23.405234 pih-0.37/pih.egg-info/
--rw-rw-rw-   0        0        0      247 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-20 23:05:19.000000 pih-0.37/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 23:05:23.498986 pih-0.37/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:30.024561 pih-0.37.1/
+-rw-rw-rw-   0        0        0      249 2024-05-21 13:51:29.993310 pih-0.37.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:27.660863 pih-0.37.1/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37.1/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:28.070881 pih-0.37.1/pih/collections/
+-rw-rw-rw-   0        0        0    30339 2024-05-17 03:55:00.000000 pih-0.37.1/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37.1/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104226 2024-05-20 23:34:54.000000 pih-0.37.1/pih/console_api.py
+-rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37.1/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.566558 pih-0.37.1/pih/consts/
+-rw-rw-rw-   0        0        0    26749 2024-05-21 13:50:32.000000 pih-0.37.1/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37.1/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37.1/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37.1/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37.1/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37.1/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37.1/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37.1/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37.1/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37.1/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37.1/pih/consts/iot.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37.1/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.37.1/pih/consts/password.py
+-rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37.1/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    16022 2024-05-21 01:27:45.000000 pih-0.37.1/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37.1/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37.1/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37.1/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37.1/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37.1/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37.1/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    17771 2024-05-20 23:11:31.000000 pih-0.37.1/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37.1/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37.1/pih/consts/style.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37.1/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   572567 2024-05-21 13:46:27.000000 pih-0.37.1/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.756851 pih-0.37.1/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37.1/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37.1/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37.1/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37.1/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.898522 pih-0.37.1/pih/tools/
+-rw-rw-rw-   0        0        0    59031 2024-05-20 00:30:59.000000 pih-0.37.1/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37.1/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37.1/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:51:29.962041 pih-0.37.1/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-05-21 13:51:26.000000 pih-0.37.1/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2024-05-21 13:51:27.000000 pih-0.37.1/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:51:26.000000 pih-0.37.1/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 13:51:26.000000 pih-0.37.1/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-21 13:51:26.000000 pih-0.37.1/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:51:30.040185 pih-0.37.1/setup.cfg
```

### Comparing `pih-0.37/pih/collections/__init__.py` & `pih-0.37.1/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/collections/service.py` & `pih-0.37.1/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/console_api.py` & `pih-0.37.1/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1473,15 +1473,15 @@
                 if A.C_WS.name(value):
                     if A.C_WS.exists(value):
                         recipient = A.R_WS.by_name(value).data
                         break
                 if recipient is None:
                     recipient_name = None
                     self.output.error(error.get_details())
-        if isinstance(recipient, User) and A.R.is_empty(
+        if isinstance(recipient, User) and e(
             A.R_WS.by_login(recipient.samAccountName)
         ):
             self.output.error(
                 js(
                     (
                         "Пользователь ",
                         recipient.name,
@@ -1511,15 +1511,15 @@
                                 A.D.to_given_name(recipient),
                                 ", ",
                             )
                         )
                         message = message or self.input.message(
                             js(
                                 (
-                                    "введите сообщение для пользователя",
+                                    "Введите сообщение для пользователя",
                                     self.get_formatted_given_name(
                                         A.D.to_given_name(recipient)
                                     ),
                                 )
                             ),
                             None if self.session.is_mobile else prefix,
                         )
```

### Comparing `pih-0.37/pih/console_api_wrapper.py` & `pih-0.37.1/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/__init__.py` & `pih-0.37.1/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ZabbixResourceDescriptionDelegated,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.37"
+VERSION: str = "0.37.1"
 
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
```

### Comparing `pih-0.37/pih/consts/ad.py` & `pih-0.37.1/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/addresses.py` & `pih-0.37.1/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/date_time.py` & `pih-0.37.1/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/errors.py` & `pih-0.37.1/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/events.py` & `pih-0.37.1/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/hosts.py` & `pih-0.37.1/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/names.py` & `pih-0.37.1/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/password.py` & `pih-0.37.1/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/paths.py` & `pih-0.37.1/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/polibase.py` & `pih-0.37.1/pih/consts/polibase.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,16 +95,16 @@
         AppointmentServiceGroupId.MRI: "МРТ исследование",
         AppointmentServiceGroupId.CT: "КТ исследование",
         AppointmentServiceGroupId.X_RAY: "рентген исследование",
     }
 
     # BONUS_PROGRAM_INFORMATION_URL: str = "https://pacifichosp.com/legal-information/polozhenie-o-bonusnoi-programme-loialnosti"
 
-    BONUS_PROGRAM_TEXT: str = """*Предлагаем вам стать участником бонусной программы Пасифик Хоспитал! Получайте кэшбэк бонусами на ваш личный счет.
-Краткие условия бонусной программы:*
+    BONUS_PROGRAM_TEXT: str = """*Предлагаем вам стать участником бонусной программы Пасифик Хоспитал! Получайте кэшбэк бонусами на ваш личный счет.*
+*Краткие условия бонусной программы:*
  • Кэшбэк 3% от стоимости приёма специалистов зачисляется в виде бонусов на ваш личный бонусный счет
  • 1 бонус = 1 рубль
  • Бонусами можно оплатить до 50% от стоимости любой услуги
  • Бонусы можно использовать при оплате услуг, оказанных владельцу карты
  • Для списания бонусных баллов участник должен уведомить администратора медицинского центра о желании оплатить частично медицинские услуги с помощью накопленных бонусных балов
  • Бонусы не подлежат обмену на денежные средства
  • Скидка по бонусам не суммируется с другими акционными предложениями
```

### Comparing `pih-0.37/pih/consts/service.py` & `pih-0.37.1/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/service_commands.py` & `pih-0.37.1/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/service_roles.py` & `pih-0.37.1/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/consts/settings.py` & `pih-0.37.1/pih/consts/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         "RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME", "8:00"
     )
     #
     POLIBASE_CREATION_DB_DUMP_START_TIME = TimeStorageVariableHolder(
         "POLIBASE_CREATION_DB_DUMP_START_TIME", "20:30"
     )
     POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL = IntVariantableStorageVariableHolder(
-        "POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL", 5, variants=(0, 1, 3, 5, 7, 9)
+        "POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL", 5, variants=(None, 0, 1, 3, 5, 7, 9)
     )
     POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS = StorageVariableHolder(
         "POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS", None
     )
     #
     RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES = IntStorageVariableHolder(
         "RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES", 15
```

### Comparing `pih-0.37/pih/pih.py` & `pih-0.37.1/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -8822,24 +8822,29 @@
                     PIH.RESULT.NOTES._all(
                         cached,
                         local,
                         CONST.FILES.SECTION,
                         Events.SAVE_FILE_FROM_KNOWLEDGE_BASE,
                     ),
                 )
+                
+            @staticmethod
+            def by_name(value: str) -> Result[File]:
+                return PIH.RESULT.FILES.find(value, strict_equality=True)
 
             @staticmethod
             def find(
                 value: str | None = None,
                 command_type: CommandTypes | None = None,
                 exclude_private_files: bool = False,
+                strict_equality: bool = False,
             ) -> Result[list[File]]:
                 value = lw(value)
                 search_function: Callable[[File], bool] = (
-                    lambda item: StringTool.full_right_intersection_by_tokens(
+                    lambda item: StringTool.contains(nns(item.title), nns(value)) if strict_equality else StringTool.full_right_intersection_by_tokens(
                         nns(item.title),
                         nns(value),
                         (" ", CONST.NAME_SPLITTER, CONST.SPLITTER, ","),
                     )
                 )
                 was_updated: bool = False
                 section: str = CONST.FILES.SECTION
@@ -8917,19 +8922,19 @@
             def execute(
                 file_search_request: str,
                 parameters: strdict | None = None,
                 stdout_redirect: bool | None = True,
                 catch_exceptions: bool = False,
                 use_default_stdout: bool = False,
             ) -> str | strdict | None:
-                file: File | None = one(PIH.RESULT.FILES.find(file_search_request))
+                file: File | None = one(PIH.RESULT.FILES.by_name(file_search_request))
                 if n(file):
                     return None
                 return PIH.EXECUTOR.execute_python_localy(
-                    file.text,  # type: ignore
+                    nnt(file).text,  
                     parameters,
                     stdout_redirect,
                     catch_exceptions,
                     use_default_stdout,
                 )
 
             @staticmethod
@@ -12308,15 +12313,15 @@
 
             @staticmethod
             def send_to_user(
                 user: User,
                 message: Any,
                 via_wappi: bool = True,
                 use_alternative: bool = True,
-                wappi_profile: Any = None,
+                wappi_profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
             ) -> bool:
                 return PIH.MESSAGE.WHATSAPP.send(
                     user.telephoneNumber,
                     message,
                     via_wappi,
                     use_alternative,
                     EnumTool.get_value(
```

### Comparing `pih-0.37/pih/rpc/__init__.py` & `pih-0.37.1/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.37.1/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.37.1/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/tools/__init__.py` & `pih-0.37.1/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/tools/service.py` & `pih-0.37.1/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih/widgets.py` & `pih-0.37.1/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.37/pih.egg-info/SOURCES.txt` & `pih-0.37.1/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

