# Comparing `tmp/dungeonmaker-0.6.6.tar.gz` & `tmp/dungeonmaker-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dungeonmaker-0.6.6.tar", last modified: Mon May 20 18:12:41 2024, max compression
+gzip compressed data, was "dungeonmaker-0.6.7.tar", last modified: Mon May 20 18:53:45 2024, max compression
```

## Comparing `dungeonmaker-0.6.6.tar` & `dungeonmaker-0.6.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.338103 dungeonmaker-0.6.6/dungeonmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/dungeonmaker/dm_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/dba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/dba.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/dmtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/room.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/dungeonmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:12:41.000000 dungeonmaker-0.6.6/dungeonmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 18:12:41.000000 dungeonmaker-0.6.6/dungeonmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:12:41.000000 dungeonmaker-0.6.6/dungeonmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 18:12:41.000000 dungeonmaker-0.6.6/dungeonmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 18:12:41.000000 dungeonmaker-0.6.6/dungeonmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:12:41.342103 dungeonmaker-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 18:12:31.000000 dungeonmaker-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.806608 dungeonmaker-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:53:45.806608 dungeonmaker-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/dba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dmtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:53:45.802608 dungeonmaker-0.6.7/dungeonmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 18:53:45.000000 dungeonmaker-0.6.7/dungeonmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:53:45.806608 dungeonmaker-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 18:53:41.000000 dungeonmaker-0.6.7/setup.py
```

### Comparing `dungeonmaker-0.6.6/LICENSE` & `dungeonmaker-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/PKG-INFO` & `dungeonmaker-0.6.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.6
+Version: 0.6.7
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/backend.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,34 +266,45 @@
         
         @self.request_handler.request(name="load_room", allow_python_syntax=True, auto_convert=True)
         def load_room(room_id : RoomId) -> str:
             room : Room
             room = self.dm_session.find(ROOM, room_id)
             return room.content
         
-        @self.request_handler.request(name="like_dungeon")
-        def like_dungeon(dungeon_id : DungeonId):
+        @self.request_handler.request(name="like_dungeon", allow_python_syntax=True, auto_convert=True)
+        def like_dungeon(dungeon_id : DungeonId) -> str:
             dungeon : Dungeon
             user : User
             self.ensure_login()
             dungeon = self.dm_session.find(DUNGEON, dungeon_id)
             user = self.find_current_client_user()
             dungeon.like(user)
             return "Success!"
         
-        @self.request_handler.request(name="unlike_dungeon")
-        def unlike_dungeon(dungeon_id : DungeonId):
+        @self.request_handler.request(name="unlike_dungeon", allow_python_syntax=True, auto_convert=True)
+        def unlike_dungeon(dungeon_id : DungeonId) -> str:
             dungeon : Dungeon
             user : User
             self.ensure_login()
             dungeon = self.dm_session.find(DUNGEON, dungeon_id)
             user = self.find_current_client_user()
             dungeon.unlike(user)
             return "Success!"
         
+        @self.request_handler.request(name="load_tab", allow_python_syntax=True, auto_convert=True)
+        def load_tab(tab : str) -> json.dumps:
+            if tab == "popular":
+                data = self.dm_session.get_popular_tab()
+            elif tab == "random":
+                data = self.dm_session.get_default_tab()
+            elif tab == "new":
+                data = self.dm_session.get_newest_tab()
+            data = [dungeon.to_object() for dungeon in data]
+            return data
+        
         self.request_handler.start(thread=thread, duration=duration)
         
     def stop(self):
         """
         Stop the dungeon maker backend.
         """
         self.request_handler.stop()
```

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/basetypes.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/connection.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/connection.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/database/dba.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/database/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/dba.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/dmtypes.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dmtypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,37 +93,37 @@
 @dataclass
 class BaseDMSession:
     database_abstractions : list[BaseDatabaseAbstraction] = field(default_factory=list, kw_only=True)
     database_abstraction : BaseDatabaseAbstraction = field(init=False)
 
 
 @dataclass(slots=True)
-class Permition:
+class Permission:
     """
-    Class for permitions.
+    Class for permissions.
     """
     type: Literal[
         "read", 
         "edit_rooms", 
         "edit_room", 
-        "edit_permitions", 
+        "edit_permissions", 
         "edit_infos", 
-        "permition_level"
+        "permission_level"
         ] = field(kw_only=True)
     value: Any = field(kw_only=True)
 
 
 
-class Permitions(list[Permition]):
+class Permissions(list[Permission]):
     """
-    Class for containing a list of permitions.
+    Class for containing a list of permissions.
     """
-    def get(self, __type : Any) -> Permition:
+    def get(self, __type : Any) -> Permission:
         try:
-            return ([i for i in self if i.type == __type] + [Permition(type=__type, value=None)])[0]
+            return ([i for i in self if i.type == __type] + [Permission(type=__type, value=None)])[0]
         except IndexError:
             pass
 
 
 
 class Stats(dict):
     """
@@ -152,15 +152,15 @@
 class BaseDungeon:
     """
     Base class for dungeons.
     """
     rooms : list[RoomId] = field(kw_only=True, default_factory=list)
     owner : UserId = field(kw_only=True)
     owner_name : str = field(kw_only=True)
-    permitions : dict[UserId, Permitions] = field(kw_only=True, default_factory=dict)
+    permissions : dict[UserId, Permissions] = field(kw_only=True, default_factory=dict)
     views : int = field(kw_only=True, default=0)
     likers : list[UserId] = field(kw_only=True, default_factory=list)
     new : bool = field(kw_only=True, default=True)
     dungeon_id : DungeonId = field(kw_only=True, default_factory=lambda : secrets.randbits(32))
     name : str = field(kw_only=True)
     description : str = field(kw_only=True)
     creation_time : float = field(kw_only=True, default_factory=time.time)
@@ -177,15 +177,15 @@
 @dataclass(slots=True)
 class BaseDungeonUser:
     """
     Base class for dungeon users.
     """
     user_id : UserId = field(kw_only=True)
     dungeon : BaseDungeon = field(kw_only=True)
-    permitions : Permitions = field(kw_only=True)
+    permissions : Permissions = field(kw_only=True)
     owner : bool = field(kw_only=True)
 
 
 @dataclass(slots=True)
 class BaseUser:
     """
     Base class for users.
```

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/dungeon.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/dungeon.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 from typing import Self
 from .dmtypes import (
     DungeonId, 
     BaseDungeon, 
     BaseRoom, 
     UserId, 
     RoomId, 
-    Permition, 
+    Permission, 
     BaseDungeonUser, 
-    Permitions
+    Permissions
 )
 from .room import Room
 from .user import User
 from . import room
 from . import session as _session
 from .utils import s_vars
 from .selectors import ROOM
 
 class Dungeon(BaseDungeon):
     """
     Class for dungeons.
     """
     def __init__(self, *args, **kwargs):
-        kwargs.setdefault("permitions", {})
-        kwargs["permitions"][kwargs["owner"]] = Permitions([
-            Permition(type="read", value=True),
-            Permition(type="edit_rooms", value=True),
-            Permition(type="edit_infos", value=True),
-            Permition(type="edit_permitions", value=True),
-            Permition(type="permition_level", value=999),
+        kwargs.setdefault("permissions", {})
+        kwargs["permissions"][kwargs["owner"]] = Permissions([
+            Permission(type="read", value=True),
+            Permission(type="edit_rooms", value=True),
+            Permission(type="edit_infos", value=True),
+            Permission(type="edit_permissions", value=True),
+            Permission(type="permission_level", value=999),
         ])
         kwargs["owner_name"] = User.read(kwargs["owner"], session=kwargs["session"]).username
         super().__init__(*args, **kwargs)
     
     @property
     def likes(self) -> int:
         """
@@ -50,18 +50,18 @@
         return [room.Room.read(room_id=room_id) for room_id in self.rooms]
     
     def get_user(self, username : str = None, *, user_id : UserId = None) -> BaseDungeonUser:
         """
         Get a user of the dungeon.
         """
         user_id = user_id or User.lookup_user(username=username, session=self.session).user_id
-        permitions = self.permitions.get(user_id, Permitions([Permition(type="read", value=True)]))
+        permissions = self.permissions.get(user_id, Permissions([Permission(type="read", value=True)]))
         owner = self.owner == user_id
-        d_user = DungeonUser(user_id=user_id, permitions=permitions, owner=owner, dungeon=self)
-        self.permitions[user_id] = d_user
+        d_user = DungeonUser(user_id=user_id, permissions=permissions, owner=owner, dungeon=self)
+        self.permissions[user_id] = d_user
         return d_user
         
     
     @classmethod
     def read(cls, dungeon_id : DungeonId, *, session : _session.DMSession) -> Self:
         """
         Method for reading a dungeon.
@@ -71,15 +71,15 @@
     
     def write(self):
         """
         Method for writing a dungeon.
         """
         data = copy.deepcopy(s_vars(self))
         data["new"] = False
-        for _, perms in (data["permitions"]).items():
+        for _, perms in (data["permissions"]).items():
             perms[:] = [{"type": perm.type, "value": perm.value} for perm in perms]
         if self.new:
             self.new = False
             self.session.database_abstraction.insert_dungeon(data=data)
             return
         self.session.database_abstraction.update_dungeon(dungeon_id=self.dungeon_id, updator={"$set": data})
         
@@ -114,14 +114,32 @@
         self.likers.remove(user.user_id)
         
     def view(self):
         """
         Register a view.
         """
         self.views += 1
+        
+    def to_object(self) -> dict:
+        """
+        Convert to an object.
+        """
+        data = copy.deepcopy(s_vars(self))
+        data.pop("rooms")
+        data.pop("permissions")
+        data.pop("new")
+        data.pop("creation_time")
+        data.pop("update_time")
+        data.pop("score")
+        data.pop("stats")
+        data.pop("start")
+        data.pop("likers")
+        data["likes"] = self.likes
+        return data
+        
 
 class DungeonUser(BaseDungeonUser):
     """
     Class for handling users in the context of a dungeon.
     """
```

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/room.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/room.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/session.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/session.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker/dm_backend/modules/dm/user.py` & `dungeonmaker-0.6.7/dungeonmaker/dm_backend/modules/dm/user.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/dungeonmaker.egg-info/PKG-INFO` & `dungeonmaker-0.6.7/dungeonmaker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.6
+Version: 0.6.7
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.6/dungeonmaker.egg-info/SOURCES.txt` & `dungeonmaker-0.6.7/dungeonmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.6/setup.py` & `dungeonmaker-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dungeonmaker',
-    version='0.6.6',
+    version='0.6.7',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='Dungeon maker backend and other things',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/dungeon-maker-reinvented',
     packages=find_packages(),
```

