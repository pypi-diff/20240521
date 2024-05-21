# Comparing `tmp/life360-7.0.0b5.tar.gz` & `tmp/life360-7.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-7.0.0b5.tar", last modified: Sun Apr 28 18:28:02 2024, max compression
+gzip compressed data, was "life360-7.0.0b6.tar", last modified: Mon Apr 29 20:11:52 2024, max compression
```

## Comparing `life360-7.0.0b5.tar` & `life360-7.0.0b6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:28:01.996330 life360-7.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 18:27:59.000000 life360-7.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-28 18:28:01.996330 life360-7.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-28 18:27:59.000000 life360-7.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:28:01.996330 life360-7.0.0b5/life360/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-28 18:27:59.000000 life360-7.0.0b5/life360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-04-28 18:27:59.000000 life360-7.0.0b5/life360/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-28 18:27:59.000000 life360-7.0.0b5/life360/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-28 18:27:59.000000 life360-7.0.0b5/life360/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-28 18:27:59.000000 life360-7.0.0b5/life360/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:28:01.996330 life360-7.0.0b5/life360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-28 18:28:01.000000 life360-7.0.0b5/life360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-28 18:28:01.000000 life360-7.0.0b5/life360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:28:01.000000 life360-7.0.0b5/life360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 18:28:01.000000 life360-7.0.0b5/life360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 18:28:01.000000 life360-7.0.0b5/life360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:28:01.996330 life360-7.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-28 18:27:59.000000 life360-7.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:11:52.252387 life360-7.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 20:11:49.000000 life360-7.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 20:11:52.252387 life360-7.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 20:11:49.000000 life360-7.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:11:52.252387 life360-7.0.0b6/life360/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:11:52.252387 life360-7.0.0b6/life360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:11:52.252387 life360-7.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 20:11:49.000000 life360-7.0.0b6/setup.py
```

### Comparing `life360-7.0.0b5/LICENSE` & `life360-7.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b5/PKG-INFO` & `life360-7.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b5
+Version: 7.0.0b6
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b5/README.md` & `life360-7.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b5/life360/__init__.py` & `life360-7.0.0b6/life360/__init__.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b5/life360/api.py` & `life360-7.0.0b6/life360/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 _BASE_CMD_FMT = f"{_BASE_URL}/v{{}}/"
 _TOKEN_URL = f"{_BASE_CMD_FMT.format(3)}oauth2/token"
 _ME_URL = f"{_BASE_CMD_FMT.format(3)}users/me"
 _CIRCLES_URL = f"{_BASE_CMD_FMT.format(4)}circles"
 _CIRCLE_URL_FMT = f"{_BASE_CMD_FMT.format(3)}circles/{{cid}}"
 _CIRCLE_MEMBERS_URL_FMT = f"{_CIRCLE_URL_FMT}/members"
 _MEMBER_URL_FMT = f"{_CIRCLE_MEMBERS_URL_FMT}/{{mid}}"
+_MEMBER_REQUEST_URL_FMT = f"{_MEMBER_URL_FMT}/request"
 
 _HEADERS = {
     "accept": "application/json",
     "cache-control": "no-cache",
     "user-agent": USER_AGENT,
 }
 
@@ -221,14 +222,37 @@
         return cast(
             dict[str, Any],
             await self._request(
                 _MEMBER_URL_FMT.format(cid=cid, mid=mid), raise_not_modified
             ),
         )
 
+    async def send_circle_member_request(
+        self, cid: str, mid: str, request: dict[str, Any]
+    ) -> dict[str, Any]:
+        """Send a request to a Circle's Member."""
+        return cast(
+            dict[str, Any],
+            await self._request(
+                _MEMBER_REQUEST_URL_FMT.format(cid=cid, mid=mid),
+                method="post",
+                raise_not_modified=False,
+                data=request,
+            ),
+        )
+
+    async def request_circle_member_location_update(
+        self, cid: str, mid: str
+    ) -> dict[str, Any]:
+        """Send a request to a Circle's Member to update their location.
+
+        Seems to cause updates every five seconds for a minute (after request is seen.)
+        """
+        return await self.send_circle_member_request(cid, mid, {"type": "location"})
+
     async def _request(
         self,
         url: str,
         /,
         raise_not_modified: bool,
         method: str = "get",
         *,
```

### Comparing `life360-7.0.0b5/life360/const.py` & `life360-7.0.0b6/life360/const.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b5/life360/exceptions.py` & `life360-7.0.0b6/life360/exceptions.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b5/life360.egg-info/PKG-INFO` & `life360-7.0.0b6/life360.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b5
+Version: 7.0.0b6
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b5/setup.py` & `life360-7.0.0b6/setup.py`

 * *Files identical despite different names*

