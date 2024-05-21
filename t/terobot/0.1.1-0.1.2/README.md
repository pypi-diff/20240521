# Comparing `tmp/terobot-0.1.1.tar.gz` & `tmp/terobot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terobot-0.1.1.tar", last modified: Tue May 21 10:43:24 2024, max compression
+gzip compressed data, was "terobot-0.1.2.tar", last modified: Tue May 21 10:53:36 2024, max compression
```

## Comparing `terobot-0.1.1.tar` & `terobot-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:43:24.443594 terobot-0.1.1/
--rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:43:24.443302 terobot-0.1.1/PKG-INFO
--rw-r--r--   0 tvarnier   (501) staff       (20)       34 2024-05-21 09:02:31.000000 terobot-0.1.1/README.md
--rw-r--r--   0 tvarnier   (501) staff       (20)      381 2024-05-21 10:41:58.000000 terobot-0.1.1/pyproject.toml
--rw-r--r--   0 tvarnier   (501) staff       (20)       38 2024-05-21 10:43:24.443655 terobot-0.1.1/setup.cfg
-drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:43:24.429245 terobot-0.1.1/terobot/
--rw-r--r--   0 tvarnier   (501) staff       (20)       27 2024-05-21 10:43:05.000000 terobot-0.1.1/terobot/__init__.py
--rw-r--r--   0 tvarnier   (501) staff       (20)     4642 2024-05-21 10:42:45.000000 terobot-0.1.1/terobot/client.py
-drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:43:24.442896 terobot-0.1.1/terobot.egg-info/
--rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:43:24.000000 terobot-0.1.1/terobot.egg-info/PKG-INFO
--rw-r--r--   0 tvarnier   (501) staff       (20)      216 2024-05-21 10:43:24.000000 terobot-0.1.1/terobot.egg-info/SOURCES.txt
--rw-r--r--   0 tvarnier   (501) staff       (20)        1 2024-05-21 10:43:24.000000 terobot-0.1.1/terobot.egg-info/dependency_links.txt
--rw-r--r--   0 tvarnier   (501) staff       (20)       17 2024-05-21 10:43:24.000000 terobot-0.1.1/terobot.egg-info/requires.txt
--rw-r--r--   0 tvarnier   (501) staff       (20)        8 2024-05-21 10:43:24.000000 terobot-0.1.1/terobot.egg-info/top_level.txt
+drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:53:36.104509 terobot-0.1.2/
+-rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:53:36.104200 terobot-0.1.2/PKG-INFO
+-rw-r--r--   0 tvarnier   (501) staff       (20)       34 2024-05-21 09:02:31.000000 terobot-0.1.2/README.md
+-rw-r--r--   0 tvarnier   (501) staff       (20)      381 2024-05-21 10:53:29.000000 terobot-0.1.2/pyproject.toml
+-rw-r--r--   0 tvarnier   (501) staff       (20)       38 2024-05-21 10:53:36.104584 terobot-0.1.2/setup.cfg
+drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:53:36.094658 terobot-0.1.2/terobot/
+-rw-r--r--   0 tvarnier   (501) staff       (20)       27 2024-05-21 10:43:05.000000 terobot-0.1.2/terobot/__init__.py
+-rw-r--r--   0 tvarnier   (501) staff       (20)     4642 2024-05-21 10:53:17.000000 terobot-0.1.2/terobot/client.py
+drwxr-xr-x   0 tvarnier   (501) staff       (20)        0 2024-05-21 10:53:36.103781 terobot-0.1.2/terobot.egg-info/
+-rw-r--r--   0 tvarnier   (501) staff       (20)      275 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/PKG-INFO
+-rw-r--r--   0 tvarnier   (501) staff       (20)      216 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/SOURCES.txt
+-rw-r--r--   0 tvarnier   (501) staff       (20)        1 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/dependency_links.txt
+-rw-r--r--   0 tvarnier   (501) staff       (20)       17 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/requires.txt
+-rw-r--r--   0 tvarnier   (501) staff       (20)        8 2024-05-21 10:53:36.000000 terobot-0.1.2/terobot.egg-info/top_level.txt
```

### Comparing `terobot-0.1.1/terobot/client.py` & `terobot-0.1.2/terobot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,22 +86,22 @@
                 'isTest': self.isTest,
             }
             self.api.post(f'{self.server}/api/datum', json=datum)
         except Exception as err:
             if options and options.logger:
                 options.logger.error('tero-bot', 'Error sending KPI to TeroBot', {'attach': err})
             else:
-                print(f'{datetime.now(timezone.UTC).isoformat()} Error sending KPI to TeroBot: {str(err)}')
+                print(f'{datetime.now(timezone.utc).isoformat()} Error sending KPI to TeroBot: {str(err)}')
 
     def sendException(self, error: BotError):
         if self.disabled:
             self.logDisabled()
             return
         try:
-            timestamp = (error.timestamp or datetime.now(timezone.UTC)).isoformat()
+            timestamp = (error.timestamp or datetime.now(timezone.utc)).isoformat()
             datum = {
                 'key': error.key,
                 'appInstance': self.appInstance,
                 'appDescription': self.appDescription,
                 'timestamp': timestamp,
                 'type': 'exception',
                 'value': str(error),
```

