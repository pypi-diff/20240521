# Comparing `tmp/revampdeployer-0.1.2.tar.gz` & `tmp/revampdeployer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revampdeployer-0.1.2.tar", last modified: Tue May 21 12:11:50 2024, max compression
+gzip compressed data, was "revampdeployer-0.1.4.tar", last modified: Tue May 21 13:27:45 2024, max compression
```

## Comparing `revampdeployer-0.1.2.tar` & `revampdeployer-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:11:50.005268 revampdeployer-0.1.2/
--rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.2/LICENSE
--rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:11:50.004953 revampdeployer-0.1.2/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)     1999 2024-05-21 11:45:28.000000 revampdeployer-0.1.2/README.md
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:11:50.003793 revampdeployer-0.1.2/revampdeployer/
--rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.2/revampdeployer/__init__.py
--rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.2/revampdeployer/__main__.py
--rw-r--r--   0 evsi       (501) staff       (20)     6289 2024-05-21 12:07:09.000000 revampdeployer-0.1.2/revampdeployer/deployer.py
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:11:50.004686 revampdeployer-0.1.2/revampdeployer.egg-info/
--rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)      300 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/SOURCES.txt
--rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/dependency_links.txt
--rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/entry_points.txt
--rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/top_level.txt
--rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 12:11:50.005313 revampdeployer-0.1.2/setup.cfg
--rw-r--r--   0 evsi       (501) staff       (20)      558 2024-05-21 12:11:36.000000 revampdeployer-0.1.2/setup.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 13:27:45.139808 revampdeployer-0.1.4/
+-rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.4/LICENSE
+-rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 13:27:45.139407 revampdeployer-0.1.4/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)     1999 2024-05-21 11:45:28.000000 revampdeployer-0.1.4/README.md
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 13:27:45.137855 revampdeployer-0.1.4/revampdeployer/
+-rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.4/revampdeployer/__init__.py
+-rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.4/revampdeployer/__main__.py
+-rw-r--r--   0 evsi       (501) staff       (20)     7178 2024-05-21 13:26:49.000000 revampdeployer-0.1.4/revampdeployer/deployer.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 13:27:45.139034 revampdeployer-0.1.4/revampdeployer.egg-info/
+-rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 13:27:45.000000 revampdeployer-0.1.4/revampdeployer.egg-info/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)      300 2024-05-21 13:27:45.000000 revampdeployer-0.1.4/revampdeployer.egg-info/SOURCES.txt
+-rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 13:27:45.000000 revampdeployer-0.1.4/revampdeployer.egg-info/dependency_links.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 13:27:45.000000 revampdeployer-0.1.4/revampdeployer.egg-info/entry_points.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 13:27:45.000000 revampdeployer-0.1.4/revampdeployer.egg-info/top_level.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 13:27:45.139876 revampdeployer-0.1.4/setup.cfg
+-rw-r--r--   0 evsi       (501) staff       (20)      558 2024-05-21 13:27:28.000000 revampdeployer-0.1.4/setup.py
```

### Comparing `revampdeployer-0.1.2/LICENSE` & `revampdeployer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revampdeployer-0.1.2/PKG-INFO` & `revampdeployer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revampdeployer
-Version: 0.1.2
+Version: 0.1.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RevampDeployer
 
 RevampDeployer - это инструмент для управления и автоматизации процесса развёртывания приложений на удалённых серверах.
```

### Comparing `revampdeployer-0.1.2/README.md` & `revampdeployer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `revampdeployer-0.1.2/revampdeployer/deployer.py` & `revampdeployer-0.1.4/revampdeployer/deployer.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,25 +40,46 @@
     # Вывод информации об операционной системе
     try:
         result = await conn.run('uname -a')
         logger.info(f"Operating System Information:\n{result.stdout.strip()}")
     except Exception as e:
         logger.error(f"An error occurred while getting OS info: {e}")
 
+async def execute_local_script(script_path):
+    try:
+        logger.info(f"Executing local script: {script_path}")
+        result = await asyncio.create_subprocess_shell(f'bash {script_path}')
+        await result.communicate()
+        logger.success(f"Local script {script_path} executed successfully.")
+    except Exception as e:
+        logger.error(f"An error occurred while executing local script {script_path}: {e}")
+        sys.exit(1)
 
 async def execute_script(conn, script_path):
     # Выполнение скрипта на удаленном сервере
     try:
         async with conn:
             result = await conn.run(f'bash {script_path}', check=True)
             logger.success(f"Script {script_path} executed successfully.")
     except Exception as e:
         logger.error(f"An error occurred while executing script {script_path}: {e}")
         sys.exit(1)
 
+async def install_local_configure_environment(scripts_dir):
+    # Установка и настройка окружения на удаленном сервере
+    scripts = os.listdir(scripts_dir)
+    if not scripts:
+        logger.info("No scripts found in the specified directory.")
+        return
+
+    tasks = [execute_local_script(os.path.join(scripts_dir, script)) for script in scripts]
+
+    for f in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Installing & Configuring Local Environment"):
+        await f
+
 
 async def install_configure_environment(conn, scripts_dir):
     # Установка и настройка окружения на удаленном сервере
     scripts = os.listdir(scripts_dir)
     if not scripts:
         logger.info("No scripts found in the specified directory.")
         return
@@ -105,59 +126,59 @@
 
     tasks = [execute_script(conn, os.path.join(scripts_dir_deploy, script)) for script in scripts]
 
     for f in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Post-deployment Configuration"):
         await f
 
 
-async def deploy_to_server(remote_host, port, username, password, scripts_dir, input_dir, output_dir, scripts_dir_deploy):
+async def deploy_to_server(server_name, scripts_dir, input_dir, output_dir, scripts_dir_deploy, local_dir):
+    # Поиск параметров сервера по имени
+    if server_name not in config.servers:
+        logger.error(f"Server '{server_name}' is not found in the configuration.")
+        return
+
+    server_info = config.servers[server_name]
+    remote_host = server_info['address']
+    username = server_info['username']
+    password = server_info['password']
+
     # Подключение к серверу
-    conn = await connect_to_server(remote_host, username, password, port)
+    conn = await connect_to_server(remote_host, username, password)
     if conn is None:
         return
 
+    await install_local_configure_environment(local_dir)
+
     # Установка и настройка окружения на удаленном сервере
     await install_configure_environment(conn, scripts_dir)
 
     # Отправка файлов на сервер
     await send_files_to_server(conn, output_dir, input_dir)
 
     # Настройка после развертывания на сервере
     await post_deploy_configuration(conn, scripts_dir_deploy)
 
     # Закрыть соединение
     conn.close()
 
 
-def parse_server_string(server_string):
-    # Парсинг строки подключения в формате 192.168.1.0@root:password
-    try:
-        address, credentials = server_string.split('@')
-        username, password = credentials.split(':')
-        return str(address), username, password
-    except ValueError:
-        raise ValueError("Server string must be in the format 192.168.1.0@root:password")
+def main():
+    # Проверка наличия аргумента с именем сервера
+    if len(sys.argv) != 2:
+        logger.error("Usage: deployer.py <server_name>")
+        sys.exit(1)
 
+    server_name = sys.argv[1]
 
-def main():
     # Получаем конфигурации из config.py
-    servers = [parse_server_string(server) for server in config.servers]
     scripts_dir = config.scripts_dir
     input_dir = config.input_dir
     output_dir = config.output_dir
+    local_dir = config.local_scripts_dir
     scripts_dir_deploy = config.scripts_dir_deploy
 
-    # Создаем цикл событий для выполнения асинхронных функций
-    loop = asyncio.get_event_loop()
-
-    tasks = [deploy_to_server(remote_host, 22, username, password, scripts_dir, input_dir, output_dir, scripts_dir_deploy)
-             for remote_host, username, password in servers]
-
-
-    loop.run_until_complete(asyncio.gather(*tasks))
-
-    # Завершить цикл событий
-    loop.close()
+    # Запуск развертывания на сервере
+    asyncio.run(deploy_to_server(server_name, scripts_dir, input_dir, output_dir, scripts_dir_deploy, local_dir))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `revampdeployer-0.1.2/revampdeployer.egg-info/PKG-INFO` & `revampdeployer-0.1.4/revampdeployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revampdeployer
-Version: 0.1.2
+Version: 0.1.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RevampDeployer
 
 RevampDeployer - это инструмент для управления и автоматизации процесса развёртывания приложений на удалённых серверах.
```

### Comparing `revampdeployer-0.1.2/setup.py` & `revampdeployer-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Читаем содержимое файла README.md
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="revampdeployer",
-    version="0.1.2",
+    version="0.1.4",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "revampdeployer = revampdeployer.__main__:main"
         ]
     },
     # Добавляем описание пакета из README.md
```

