# Comparing `tmp/tg_signer-0.1.3.tar.gz` & `tmp/tg_signer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_signer-0.1.3.tar", last modified: Thu May 16 09:35:34 2024, max compression
+gzip compressed data, was "tg_signer-0.1.4.tar", last modified: Tue May 21 02:03:27 2024, max compression
```

## Comparing `tg_signer-0.1.3.tar` & `tg_signer-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 09:35:34.973740 tg_signer-0.1.3/
--rw-r--r--   0 luming     (501) staff       (20)     1493 2024-01-07 10:02:22.000000 tg_signer-0.1.3/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)     1206 2024-05-16 09:35:34.973678 tg_signer-0.1.3/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      607 2024-05-16 07:49:00.000000 tg_signer-0.1.3/README.md
--rw-r--r--   0 luming     (501) staff       (20)     1017 2024-05-16 09:35:34.974450 tg_signer-0.1.3/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2024-01-07 10:02:22.000000 tg_signer-0.1.3/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 09:35:34.972322 tg_signer-0.1.3/tg_signer/
--rw-r--r--   0 luming     (501) staff       (20)       22 2024-05-16 08:34:11.000000 tg_signer-0.1.3/tg_signer/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       66 2024-05-16 07:03:40.000000 tg_signer-0.1.3/tg_signer/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)     8896 2024-05-16 08:48:02.000000 tg_signer-0.1.3/tg_signer/signer.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 09:35:34.973405 tg_signer-0.1.3/tg_signer.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     1206 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      300 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       53 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)       30 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)       10 2024-05-16 09:35:34.000000 tg_signer-0.1.3/tg_signer.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-21 02:03:27.271078 tg_signer-0.1.4/
+-rw-r--r--   0 luming     (501) staff       (20)     1493 2024-01-07 10:02:22.000000 tg_signer-0.1.4/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)     1309 2024-05-21 02:03:27.271014 tg_signer-0.1.4/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      710 2024-05-17 08:18:22.000000 tg_signer-0.1.4/README.md
+-rw-r--r--   0 luming     (501) staff       (20)     1017 2024-05-21 02:03:27.273015 tg_signer-0.1.4/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2024-01-07 10:02:22.000000 tg_signer-0.1.4/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-21 02:03:27.269629 tg_signer-0.1.4/tg_signer/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2024-05-20 03:13:53.000000 tg_signer-0.1.4/tg_signer/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       66 2024-05-16 07:03:40.000000 tg_signer-0.1.4/tg_signer/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)     9007 2024-05-20 03:11:57.000000 tg_signer-0.1.4/tg_signer/signer.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-21 02:03:27.270754 tg_signer-0.1.4/tg_signer.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     1309 2024-05-21 02:03:27.000000 tg_signer-0.1.4/tg_signer.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      300 2024-05-21 02:03:27.000000 tg_signer-0.1.4/tg_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2024-05-21 02:03:27.000000 tg_signer-0.1.4/tg_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       53 2024-05-21 02:03:27.000000 tg_signer-0.1.4/tg_signer.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)       30 2024-05-21 02:03:27.000000 tg_signer-0.1.4/tg_signer.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)       10 2024-05-21 02:03:27.000000 tg_signer-0.1.4/tg_signer.egg-info/top_level.txt
```

### Comparing `tg_signer-0.1.3/LICENSE` & `tg_signer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_signer-0.1.3/PKG-INFO` & `tg_signer-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-signer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Telegram signer
 Home-page: https://github.com/amchii/tg-signer
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/tg-signer
 Classifier: Intended Audience :: Developers
@@ -19,37 +19,41 @@
 
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
 ```
 pip install -U tg-signer
 ```
+or for speedup:
+```
+pip install "tg-signer[tgcrypto]"
+```
 
 ## Usage
 ```
 Usage: tg-signer <command>
 Available commands: list, login, run, reconfig
 e.g. tg-signer run
 ```
 #### Configure proxy(if necessary)
-use `TG_PROXY`
+use env `TG_PROXY`
 
 e.g.:
 ```
 export TG_PROXY=socks5://127.0.0.1:7890
 ```
 
 #### Run
 `tg-signer run`
 
 run `tree .signer` you will see:
 ```
 .signer
-├── latest_chats.json
-├── me.json
+├── latest_chats.json  # 获取的最近对话
+├── me.json  # 个人信息
 └── signs
     └── openai  # 签到任务名
         ├── config.json  # 签到配置
         └── sign_record.json  # 签到记录
 
 3 directories, 4 files
 ```
```

### Comparing `tg_signer-0.1.3/setup.cfg` & `tg_signer-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tg_signer-0.1.3/tg_signer/signer.py` & `tg_signer-0.1.4/tg_signer/signer.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pathlib
 import random
 import sys
 from datetime import datetime, time, timedelta, timezone
 from logging.handlers import RotatingFileHandler
 from urllib import parse
 
-from pyrogram import Client, errors
+from pyrogram import Client as BaseClient, errors
 from pyrogram.types import Object, User
 
 format_str = (
     "[%(levelname)s] [%(name)s] %(asctime)s %(filename)s %(lineno)s %(message)s"
 )
 logging.basicConfig(
     level=logging.INFO,
@@ -31,14 +31,22 @@
 )
 file_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 root_dir = pathlib.Path(".").absolute()
 local_dir = root_dir / ".signer"
 
 
+class Client(BaseClient):
+    async def __aenter__(self):
+        try:
+            return await self.start()
+        except ConnectionError:
+            pass
+
+
 def get_api_config():
     api_id = int(os.environ.get("TG_API_ID", 611335))
     api_hash = os.environ.get("TG_API_HASH", "d524b414d21f4d37f08684c1df41ac9c")
     return api_id, api_hash
 
 
 def get_proxy():
@@ -242,26 +250,27 @@
                     logger.info(f"当前时间: {now}")
                     if str(now.date()) not in sign_record:
                         await self.sign(config.chat_id, config.sign_text)
                         sign_record[str(now.date())] = now.isoformat()
                         with open(self.sign_record_file, "w", encoding="utf-8") as fp:
                             json.dump(sign_record, fp)
 
-                    next_run = (now + timedelta(days=1)).replace(
-                        hour=sign_at.hour,
-                        minute=sign_at.minute,
-                        second=sign_at.second,
-                        microsecond=sign_at.microsecond,
-                    ) + timedelta(seconds=random.randint(0, int(config.random_seconds)))
-                    logger.info(f"下次运行时间: {next_run}")
-                    await asyncio.sleep((next_run - now).total_seconds())
             except (OSError, errors.Unauthorized) as e:
                 logger.exception(e)
                 await asyncio.sleep(30)
 
+            next_run = (now + timedelta(days=1)).replace(
+                hour=sign_at.hour,
+                minute=sign_at.minute,
+                second=sign_at.second,
+                microsecond=sign_at.microsecond,
+            ) + timedelta(seconds=random.randint(0, int(config.random_seconds)))
+            logger.info(f"下次运行时间: {next_run}")
+            await asyncio.sleep((next_run - now).total_seconds())
+
 
 async def main():
     help_text = (
         "Usage: tg-signer <command>\n"
         "Available commands: list, login, run, reconfig\n\n"
         "e.g. tg-signer run"
     )
```

### Comparing `tg_signer-0.1.3/tg_signer.egg-info/PKG-INFO` & `tg_signer-0.1.4/tg_signer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-signer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Telegram signer
 Home-page: https://github.com/amchii/tg-signer
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/tg-signer
 Classifier: Intended Audience :: Developers
@@ -19,37 +19,41 @@
 
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
 ```
 pip install -U tg-signer
 ```
+or for speedup:
+```
+pip install "tg-signer[tgcrypto]"
+```
 
 ## Usage
 ```
 Usage: tg-signer <command>
 Available commands: list, login, run, reconfig
 e.g. tg-signer run
 ```
 #### Configure proxy(if necessary)
-use `TG_PROXY`
+use env `TG_PROXY`
 
 e.g.:
 ```
 export TG_PROXY=socks5://127.0.0.1:7890
 ```
 
 #### Run
 `tg-signer run`
 
 run `tree .signer` you will see:
 ```
 .signer
-├── latest_chats.json
-├── me.json
+├── latest_chats.json  # 获取的最近对话
+├── me.json  # 个人信息
 └── signs
     └── openai  # 签到任务名
         ├── config.json  # 签到配置
         └── sign_record.json  # 签到记录
 
 3 directories, 4 files
 ```
```

