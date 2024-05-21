# Comparing `tmp/jzai-59.83.49.tar.gz` & `tmp/jzai-59.83.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.49.tar", last modified: Mon May 20 08:36:47 2024, max compression
+gzip compressed data, was "jzai-59.83.50.tar", last modified: Mon May 20 08:52:45 2024, max compression
```

## Comparing `jzai-59.83.49.tar` & `jzai-59.83.50.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:36:47.660839 jzai-59.83.49/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:36:47.659633 jzai-59.83.49/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.49/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:36:47.640960 jzai-59.83.49/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.49/jzai/__init__.py
--rw-rw-rw-   0        0        0     9373 2024-05-20 08:33:38.000000 jzai-59.83.49/jzai/bot.py
--rw-rw-rw-   0        0        0      199 2024-05-20 08:36:28.000000 jzai-59.83.49/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.49/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.49/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:36:47.657635 jzai-59.83.49/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 08:36:47.660839 jzai-59.83.49/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-20 08:36:45.000000 jzai-59.83.49/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:52:45.271365 jzai-59.83.50/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:52:45.270159 jzai-59.83.50/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.50/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:52:45.250546 jzai-59.83.50/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.50/jzai/__init__.py
+-rw-rw-rw-   0        0        0     9473 2024-05-20 08:51:50.000000 jzai-59.83.50/jzai/bot.py
+-rw-rw-rw-   0        0        0      199 2024-05-20 08:52:30.000000 jzai-59.83.50/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.50/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.50/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:52:45.268808 jzai-59.83.50/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:52:45.000000 jzai-59.83.50/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 08:52:45.000000 jzai-59.83.50/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:52:45.000000 jzai-59.83.50/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:52:45.000000 jzai-59.83.50/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-20 08:52:45.000000 jzai-59.83.50/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 08:52:45.000000 jzai-59.83.50/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:52:45.272832 jzai-59.83.50/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-20 08:52:38.000000 jzai-59.83.50/setup.py
```

### Comparing `jzai-59.83.49/jzai/bot.py` & `jzai-59.83.50/jzai/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,21 +141,23 @@
         elif user_input_lower.startswith("view chat log for "):
             username = user_input[18:].strip()
             if self.is_admin(self.current_user):
                 self.view_chat(username)
             else:
                 print("You do not have permission to view chats.")
         else:
-            bot_response = self.generate_response(user_input)
-            print(f"{self.name}: {bot_response}")
-            self.speak(bot_response)
             if self.current_user:
+                bot_response = self.generate_response(user_input)
+                print(f"{self.name}: {bot_response}")
+                self.speak(bot_response)
                 chat_log = asyncio.run(self.load_chat_logs(self.current_user))
                 chat_log.append({'user': user_input, 'bot': bot_response})
                 asyncio.run(self.save_chat_log(self.current_user, chat_log))
+            else:
+                print("Invalid command. Please log in or sign up.")
 
     def login(self):
         username = input("Username: ")
         password = pw.pwinput(prompt="Password: ", mask="*")
         password_hash = hashlib.sha256(password.encode()).hexdigest()
         if username in self.users and self.users[username]['password'] == password_hash:
             print(f"Welcome back, {username}!")
```

### Comparing `jzai-59.83.49/jzai/db.py` & `jzai-59.83.50/jzai/db.py`

 * *Files identical despite different names*

