# Comparing `tmp/jzai-59.83.56.tar.gz` & `tmp/jzai-59.83.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.56.tar", last modified: Tue May 21 04:08:29 2024, max compression
+gzip compressed data, was "jzai-59.83.57.tar", last modified: Tue May 21 04:19:54 2024, max compression
```

## Comparing `jzai-59.83.56.tar` & `jzai-59.83.57.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 04:08:29.308411 jzai-59.83.56/
--rw-rw-rw-   0        0        0      275 2024-05-21 04:08:29.307402 jzai-59.83.56/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.56/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 04:08:29.252652 jzai-59.83.56/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.56/jzai/__init__.py
--rw-rw-rw-   0        0        0     7750 2024-05-21 04:08:11.000000 jzai-59.83.56/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.56/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.56/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.56/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 04:08:29.304865 jzai-59.83.56/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 04:08:29.000000 jzai-59.83.56/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 04:08:29.309836 jzai-59.83.56/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-21 04:08:23.000000 jzai-59.83.56/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:19:54.944679 jzai-59.83.57/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:19:54.942664 jzai-59.83.57/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.57/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 04:19:54.909671 jzai-59.83.57/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.57/jzai/__init__.py
+-rw-rw-rw-   0        0        0     8546 2024-05-21 04:17:35.000000 jzai-59.83.57/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-20 09:00:13.000000 jzai-59.83.57/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.57/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.57/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:19:54.940168 jzai-59.83.57/jzai.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 04:19:54.000000 jzai-59.83.57/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:19:54.944679 jzai-59.83.57/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-21 04:19:47.000000 jzai-59.83.57/setup.py
```

### Comparing `jzai-59.83.56/jzai/bot.py` & `jzai-59.83.57/jzai/bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import speech_recognition as sr
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
 from textblob import TextBlob
 import nltk
 import random
 import pwinput as pw
+import pkg_resources
 
 # Ensure necessary NLTK data is downloaded
 nltk.download('punkt')
 nltk.download('stopwords')
 
 
 class Bot:
@@ -69,24 +70,31 @@
             return f"Error: {e}"
 
     def speak(self, text):
         self.engine.say(text)
         self.engine.runAndWait()
 
     def load_users(self):
+        users_file_name = "users.json"
         try:
-            with open("users.json", 'r') as file:
-                self.users = json.load(file)
+            file_content = pkg_resources.resource_string("jzai", users_file_name)
+            self.users = json.loads(file_content)
         except FileNotFoundError:
             pass
+        except Exception as e:
+            print(f"Error loading users: {e}")
 
     def save_users(self):
-        with open("users.json", 'w') as file:
-            json.dump(self.users, file, indent=4)
-
+        users_file_name = "users.json"
+        try:
+            with open(users_file_name, 'w') as file:
+                json.dump(self.users, file, indent=4)
+        except Exception as e:
+            print(f"Error saving users: {e}")
+            
     def is_admin(self, username):
         if username in self.users:
             return self.users[username].get('is_admin', False)
         return False
 
     def edit_username(self, username, new_name):
         if username in self.users:
@@ -100,44 +108,47 @@
         if self.is_admin(username):
             # Access all chat logs or perform other admin actions
             print("Admin access granted. You can manage chats here.")
         else:
             print("You do not have permission to manage chats.")
 
     def load_chat_logs(self, username):
-        chat_log_file = os.path.join("chat_logs", f"{username}.json")
-        if os.path.exists(chat_log_file):
-            with open(chat_log_file, 'r') as file:
-                try:
-                    return json.load(file)
-                except json.decoder.JSONDecodeError:
-                    return []
-        else:
+        chat_log_file_name = f"{username}.json"
+        try:
+            file_content = pkg_resources.resource_string("jzai", f"chat_logs/{chat_log_file_name}")
+            return json.loads(file_content)
+        except Exception as e:
+            print(f"Error loading chat log for {username}: {e}")
             return []
 
 
 
     def save_chat_log(self, username, chat_log):
-        chat_log_file = os.path.join("chat_logs", f"{username}.json")
-        with open(chat_log_file, 'w') as file:
-            json.dump(chat_log, file, indent=4)
+        chat_log_file_name = f"{username}.json"
+        chat_log_file_path = pkg_resources.resource_filename("jzai", f"chat_logs/{chat_log_file_name}")
+        try:
+            with open(chat_log_file_path, 'w') as file:
+                json.dump(chat_log, file, indent=4)
+        except Exception as e:
+            print(f"Error saving chat log for {username}: {e}")
 
     def view_chat(self, username):
-        chat_log_file = os.path.join("chat_logs", f"{username}.json")
-        if os.path.exists(chat_log_file):
-            with open(chat_log_file, 'r') as file:
+        chat_log_file_name = f"{username}.json"
+        chat_log_file_path = pkg_resources.resource_filename("jzai", f"chat_logs/{chat_log_file_name}")
+        if os.path.exists(chat_log_file_path):
+            with open(chat_log_file_path, 'r') as file:
                 chat_log = json.load(file)
                 print(f"Chat log for {username}:")
                 for entry in chat_log:
                     print(f"User: {entry['user']}")
                     print(f"Bot: {entry['bot']}")
                     print("-" * 20)
         else:
             print(f"No chat log found for {username}.")
-
+            
     def process_input(self, user_input):
         user_input_lower = user_input.lower()
         if user_input_lower == "login":
             self.login()
         elif user_input_lower == "signup":
             self.signup()
         elif user_input_lower == "what's my name?":
@@ -179,17 +190,21 @@
         if username not in self.users:
             self.users[username] = {'password': password_hash}
             self.save_users()
             print(f"Account created successfully for {username}.")
         else:
             print("Username already exists. Please choose another one.")
 
-    def load_conversations(self, file_path):
-        with open(file_path, 'r') as file:
-            return json.load(file)
+    def load_conversations(self, file_name):
+        try:
+            file_content = pkg_resources.resource_string("jzai", file_name)
+            return json.loads(file_content)
+        except Exception as e:
+            print(f"Error loading conversations.json: {e}")
+            return None
 
 
 bot = Bot(name="JZ")
 bot.load_users()
 
 try:
     while True:
```

### Comparing `jzai-59.83.56/jzai/db.py` & `jzai-59.83.57/jzai/db.py`

 * *Files identical despite different names*

