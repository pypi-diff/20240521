# Comparing `tmp/deltachat2-0.6.1.tar.gz` & `tmp/deltachat2-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat2-0.6.1.tar", last modified: Mon May 20 20:47:51 2024, max compression
+gzip compressed data, was "deltachat2-0.6.2.tar", last modified: Tue May 21 11:18:55 2024, max compression
```

## Comparing `deltachat2-0.6.1.tar` & `deltachat2-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:47:51.402936 deltachat2-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:47:51.398935 deltachat2-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:47:51.398935 deltachat2-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 20:47:40.000000 deltachat2-0.6.1/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 20:47:40.000000 deltachat2-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-20 20:47:40.000000 deltachat2-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-20 20:47:51.402936 deltachat2-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-20 20:47:40.000000 deltachat2-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:47:51.398935 deltachat2-0.6.1/deltachat2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-20 20:47:40.000000 deltachat2-0.6.1/deltachat2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:47:51.402936 deltachat2-0.6.1/deltachat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-20 20:47:51.000000 deltachat2-0.6.1/deltachat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-20 20:47:51.000000 deltachat2-0.6.1/deltachat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:47:51.000000 deltachat2-0.6.1/deltachat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 20:47:51.000000 deltachat2-0.6.1/deltachat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 20:47:51.000000 deltachat2-0.6.1/deltachat2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:47:51.402936 deltachat2-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-20 20:47:40.000000 deltachat2-0.6.1/examples/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-05-20 20:47:40.000000 deltachat2-0.6.1/examples/echobot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-20 20:47:40.000000 deltachat2-0.6.1/examples/echobot_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 20:47:40.000000 deltachat2-0.6.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-20 20:47:40.000000 deltachat2-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:47:51.402936 deltachat2-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:55.663164 deltachat2-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:55.659164 deltachat2-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:55.659164 deltachat2-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-21 11:18:45.000000 deltachat2-0.6.2/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 11:18:45.000000 deltachat2-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-21 11:18:45.000000 deltachat2-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-21 11:18:55.663164 deltachat2-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-21 11:18:45.000000 deltachat2-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:55.663164 deltachat2-0.6.2/deltachat2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-21 11:18:45.000000 deltachat2-0.6.2/deltachat2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:55.663164 deltachat2-0.6.2/deltachat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-21 11:18:55.000000 deltachat2-0.6.2/deltachat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 11:18:55.000000 deltachat2-0.6.2/deltachat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:18:55.000000 deltachat2-0.6.2/deltachat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 11:18:55.000000 deltachat2-0.6.2/deltachat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 11:18:55.000000 deltachat2-0.6.2/deltachat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:55.663164 deltachat2-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-21 11:18:45.000000 deltachat2-0.6.2/examples/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-05-21 11:18:45.000000 deltachat2-0.6.2/examples/echobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-21 11:18:45.000000 deltachat2-0.6.2/examples/echobot_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 11:18:45.000000 deltachat2-0.6.2/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-21 11:18:45.000000 deltachat2-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:18:55.663164 deltachat2-0.6.2/setup.cfg
```

### Comparing `deltachat2-0.6.1/.github/workflows/python-ci.yml` & `deltachat2-0.6.2/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/LICENSE` & `deltachat2-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/PKG-INFO` & `deltachat2-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.6.1
+Version: 0.6.2
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.6.1/README.md` & `deltachat2-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/_utils.py` & `deltachat2-0.6.2/deltachat2/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/bot.py` & `deltachat2-0.6.2/deltachat2/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         if msg.from_id > SpecialContactId.LAST_SPECIAL:
             return True
         if msg.from_id == SpecialContactId.SELF:
             try:
                 community = self.rpc.get_config(accid, "is_community")
                 if community:
                     name = self.rpc.get_config(accid, "ui.community.selfname")
-                    if name and name != msg.override_sender_name:
+                    if name and name != msg.get("override_sender_name"):
                         return True
             except JsonRpcError:
                 pass
         return False
 
     def _process_messages(self, accid: int, retry=True) -> None:
         try:
```

### Comparing `deltachat2-0.6.1/deltachat2/client.py` & `deltachat2-0.6.2/deltachat2/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/events.py` & `deltachat2-0.6.2/deltachat2/events.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/rpc.py` & `deltachat2-0.6.2/deltachat2/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/transport.py` & `deltachat2-0.6.2/deltachat2/transport.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/types.py` & `deltachat2-0.6.2/deltachat2/types.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2/util.py` & `deltachat2-0.6.2/deltachat2/util.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/deltachat2.egg-info/PKG-INFO` & `deltachat2-0.6.2/deltachat2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.6.1
+Version: 0.6.2
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.6.1/examples/client.py` & `deltachat2-0.6.2/examples/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/examples/echobot.py` & `deltachat2-0.6.2/examples/echobot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/examples/echobot_advanced.py` & `deltachat2-0.6.2/examples/echobot_advanced.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.6.1/pyproject.toml` & `deltachat2-0.6.2/pyproject.toml`

 * *Files identical despite different names*

