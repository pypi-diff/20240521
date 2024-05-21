# Comparing `tmp/revampdeployer-0.1.0.tar.gz` & `tmp/revampdeployer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revampdeployer-0.1.0.tar", last modified: Tue May 21 11:42:15 2024, max compression
+gzip compressed data, was "revampdeployer-0.1.1.tar", last modified: Tue May 21 12:09:18 2024, max compression
```

## Comparing `revampdeployer-0.1.0.tar` & `revampdeployer-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 11:42:15.355085 revampdeployer-0.1.0/
--rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.0/LICENSE
--rw-r--r--   0 evsi       (501) staff       (20)       80 2024-05-21 11:42:15.354848 revampdeployer-0.1.0/PKG-INFO
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 11:42:15.353685 revampdeployer-0.1.0/revampdeployer/
--rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.0/revampdeployer/__init__.py
--rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.0/revampdeployer/__main__.py
--rw-r--r--   0 evsi       (501) staff       (20)     6284 2024-05-21 11:39:44.000000 revampdeployer-0.1.0/revampdeployer/deployer.py
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 11:42:15.354604 revampdeployer-0.1.0/revampdeployer.egg-info/
--rw-r--r--   0 evsi       (501) staff       (20)       80 2024-05-21 11:42:15.000000 revampdeployer-0.1.0/revampdeployer.egg-info/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)      290 2024-05-21 11:42:15.000000 revampdeployer-0.1.0/revampdeployer.egg-info/SOURCES.txt
--rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 11:42:15.000000 revampdeployer-0.1.0/revampdeployer.egg-info/dependency_links.txt
--rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 11:42:15.000000 revampdeployer-0.1.0/revampdeployer.egg-info/entry_points.txt
--rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 11:42:15.000000 revampdeployer-0.1.0/revampdeployer.egg-info/top_level.txt
--rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 11:42:15.355130 revampdeployer-0.1.0/setup.cfg
--rw-r--r--   0 evsi       (501) staff       (20)      257 2024-05-21 11:41:38.000000 revampdeployer-0.1.0/setup.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:09:18.637691 revampdeployer-0.1.1/
+-rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.1/LICENSE
+-rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:09:18.637272 revampdeployer-0.1.1/PKG-INFO
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:09:18.636231 revampdeployer-0.1.1/revampdeployer/
+-rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.1/revampdeployer/__init__.py
+-rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.1/revampdeployer/__main__.py
+-rw-r--r--   0 evsi       (501) staff       (20)     6289 2024-05-21 12:07:09.000000 revampdeployer-0.1.1/revampdeployer/deployer.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:09:18.636993 revampdeployer-0.1.1/revampdeployer.egg-info/
+-rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)      290 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/SOURCES.txt
+-rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/dependency_links.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/entry_points.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/top_level.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 12:09:18.637740 revampdeployer-0.1.1/setup.cfg
+-rw-r--r--   0 evsi       (501) staff       (20)      558 2024-05-21 12:09:17.000000 revampdeployer-0.1.1/setup.py
```

### Comparing `revampdeployer-0.1.0/LICENSE` & `revampdeployer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revampdeployer-0.1.0/revampdeployer/deployer.py` & `revampdeployer-0.1.1/revampdeployer/deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         logger.success(f"Successfully connected to {remote_host}.")
         await print_os_info(conn)  # Вызываем функцию для вывода информации об ОС
         return conn
     except Exception as e:
         logger.error(f"Failed to connect to {remote_host}: {e}")
         return None
 
-
 async def print_os_info(conn):
     # Вывод информации об операционной системе
     try:
         result = await conn.run('uname -a')
         logger.info(f"Operating System Information:\n{result.stdout.strip()}")
     except Exception as e:
         logger.error(f"An error occurred while getting OS info: {e}")
@@ -108,15 +107,15 @@
 
     for f in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Post-deployment Configuration"):
         await f
 
 
 async def deploy_to_server(remote_host, port, username, password, scripts_dir, input_dir, output_dir, scripts_dir_deploy):
     # Подключение к серверу
-    conn = await connect_to_server(remote_host, port, username, password)
+    conn = await connect_to_server(remote_host, username, password, port)
     if conn is None:
         return
 
     # Установка и настройка окружения на удаленном сервере
     await install_configure_environment(conn, scripts_dir)
 
     # Отправка файлов на сервер
@@ -130,15 +129,15 @@
 
 
 def parse_server_string(server_string):
     # Парсинг строки подключения в формате 192.168.1.0@root:password
     try:
         address, credentials = server_string.split('@')
         username, password = credentials.split(':')
-        return address, username, password
+        return str(address), username, password
     except ValueError:
         raise ValueError("Server string must be in the format 192.168.1.0@root:password")
 
 
 def main():
     # Получаем конфигурации из config.py
     servers = [parse_server_string(server) for server in config.servers]
@@ -149,14 +148,15 @@
 
     # Создаем цикл событий для выполнения асинхронных функций
     loop = asyncio.get_event_loop()
 
     tasks = [deploy_to_server(remote_host, 22, username, password, scripts_dir, input_dir, output_dir, scripts_dir_deploy)
              for remote_host, username, password in servers]
 
+
     loop.run_until_complete(asyncio.gather(*tasks))
 
     # Завершить цикл событий
     loop.close()
 
 
 if __name__ == '__main__':
```

