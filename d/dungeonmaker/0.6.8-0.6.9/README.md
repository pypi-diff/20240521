# Comparing `tmp/dungeonmaker-0.6.8.tar.gz` & `tmp/dungeonmaker-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dungeonmaker-0.6.8.tar", last modified: Tue May 21 06:58:44 2024, max compression
+gzip compressed data, was "dungeonmaker-0.6.9.tar", last modified: Tue May 21 07:08:53 2024, max compression
```

## Comparing `dungeonmaker-0.6.8.tar` & `dungeonmaker-0.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.186410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/dba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dba.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dmtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/room.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/dungeonmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 06:58:44.000000 dungeonmaker-0.6.8/dungeonmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:58:44.190410 dungeonmaker-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 06:58:40.000000 dungeonmaker-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.725279 dungeonmaker-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 07:08:53.725279 dungeonmaker-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.721279 dungeonmaker-0.6.9/dungeonmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.721279 dungeonmaker-0.6.9/dungeonmaker/dm_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.721279 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.721279 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/dba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.721279 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/dba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/dmtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:08:53.725279 dungeonmaker-0.6.9/dungeonmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 07:08:53.000000 dungeonmaker-0.6.9/dungeonmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-21 07:08:53.000000 dungeonmaker-0.6.9/dungeonmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:08:53.000000 dungeonmaker-0.6.9/dungeonmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 07:08:53.000000 dungeonmaker-0.6.9/dungeonmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 07:08:53.000000 dungeonmaker-0.6.9/dungeonmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:08:53.725279 dungeonmaker-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 07:08:49.000000 dungeonmaker-0.6.9/setup.py
```

### Comparing `dungeonmaker-0.6.8/LICENSE` & `dungeonmaker-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.8/PKG-INFO` & `dungeonmaker-0.6.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.8
+Version: 0.6.9
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/backend.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/backend.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/basetypes.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/connection.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/connection.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/database/dba.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/database/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dba.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/dba.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Submodule for database abstractions.
 """
+from __future__ import annotations
 from .dmtypes import UserId, DungeonId, RoomId, BaseDatabaseAbstraction
 
 
     
 class DatabaseAbstractionSelector(BaseDatabaseAbstraction):
     """
     Class for selecting a database abstraction.
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dmtypes.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/dmtypes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Types used in the dm library
 """
-from typing import Literal, Any, Union
+from __future__ import annotations
+from typing import Literal, Any, Union, Sequence, Mapping
 from dataclasses import dataclass, field
 import secrets, time
 
 
 
 RoomId = int
 
@@ -86,18 +87,16 @@
         aggregation : list[dict] = [{"$addFields":{"score": {"$add": [{"$multiply": [20,{"$size": "$likers"},]},"$views"]}}}]
     ) -> list[dict]:
         """
         Do not use.
         """
         raise NotImplementedError
 
-@dataclass
-class BaseDMSession:
-    database_abstractions : list[BaseDatabaseAbstraction] = field(default_factory=list, kw_only=True)
-    database_abstraction : BaseDatabaseAbstraction = field(init=False)
+
+
 
 
 @dataclass(slots=True)
 class Permission:
     """
     Class for permissions.
     """
@@ -144,37 +143,14 @@
     new : bool = field(kw_only=True, default=True)
     _id : Any = field(kw_only=True, default=None)
     session : BaseDMSession = field(kw_only=True)
 
 
 
 
-@dataclass(slots=True)
-class BaseDungeon:
-    """
-    Base class for dungeons.
-    """
-    rooms : list[RoomId] = field(kw_only=True, default_factory=list)
-    owner : UserId = field(kw_only=True)
-    owner_name : str = field(kw_only=True)
-    permissions : dict[UserId, Permissions] = field(kw_only=True, default_factory=dict)
-    views : int = field(kw_only=True, default=0)
-    likers : list[UserId] = field(kw_only=True, default_factory=list)
-    new : bool = field(kw_only=True, default=True)
-    dungeon_id : DungeonId = field(kw_only=True, default_factory=lambda : secrets.randbits(32))
-    name : str = field(kw_only=True)
-    description : str = field(kw_only=True)
-    creation_time : float = field(kw_only=True, default_factory=time.time)
-    update_time : float = field(kw_only=True, default_factory=time.time)
-    _id : Any = field(kw_only=True, default=None)
-    score : Any = field(kw_only=True, default=None)
-    session : BaseDMSession = field(kw_only=True)
-    stats : Stats = field(kw_only=True, default_factory=Stats)
-    start : tuple = field(kw_only=True)
-
 
 
 
 @dataclass(slots=True)
 class BaseDungeonUser:
     """
     Base class for dungeon users.
@@ -201,16 +177,92 @@
     session : BaseDMSession = field(kw_only=True)
     passdata : bytes = field(kw_only=True)
     linked_user : Union[str, None] = field(kw_only=True, default=None)
     stats : Stats = field(kw_only=True, default_factory=Stats)
 
 
 
+@dataclass(slots=True)
+class BaseDungeon:
+    """
+    Base class for dungeons.
+    """
+    rooms : list[RoomId] = field(kw_only=True, default_factory=list)
+    owner : UserId = field(kw_only=True)
+    owner_name : str = field(kw_only=True)
+    permissions : dict[UserId, Permissions] = field(kw_only=True, default_factory=dict)
+    views : int = field(kw_only=True, default=0)
+    likers : list[UserId] = field(kw_only=True, default_factory=list)
+    new : bool = field(kw_only=True, default=True)
+    dungeon_id : DungeonId = field(kw_only=True, default_factory=lambda : secrets.randbits(32))
+    name : str = field(kw_only=True)
+    description : str = field(kw_only=True)
+    creation_time : float = field(kw_only=True, default_factory=time.time)
+    update_time : float = field(kw_only=True, default_factory=time.time)
+    _id : Any = field(kw_only=True, default=None)
+    score : Any = field(kw_only=True, default=None)
+    session : BaseDMSession = field(kw_only=True)
+    stats : Stats = field(kw_only=True, default_factory=Stats)
+    start : tuple = field(kw_only=True)
+
+
+
+@dataclass
+class BaseDMSession:
+    database_abstractions : list[BaseDatabaseAbstraction] = field(default_factory=list, kw_only=True)
+    database_abstraction : BaseDatabaseAbstraction = field(init=False)
+    
+    def add_database_abstraction(self, dba : BaseDatabaseAbstraction):
+        """
+        Add a database abstraction.
+        """
+        raise NotImplementedError
+
+
+    def get_popular_tab(self, *, offset : int = 0, amount : int = 20) -> list[BaseDungeon]:
+        """
+        Get a default of 20 dungeons with no offset from the most popular dungeons.
+        """
+        raise NotImplementedError
 
+    def get_random_tab(self, *, offset : int = 0, amount : int = 20) -> list[BaseDungeon]:
+        """
+        Get a default of 20 dungeons of random dungeons. 
+        """
+        raise NotImplementedError
+
+    def get_default_tab(self, *, offset : int = 0, amount : int = 20) -> list[BaseDungeon]:
+        """
+        Get a default of 20 dungeons of random dungeons. 
+        """
+        raise NotImplementedError
+
+    def get_newest_tab(self, *, offset : int = 0, amount : int = 20) -> list[BaseDungeon]:
+        """
+        Get a default of 20 dungeons of the newest dungeons. 
+        """
+        raise NotImplementedError
 
+    def search_for_term(self, term : str, *, amount : int = 10) -> list[BaseDungeon]:
+        """
+        Searches for terms.
+        """
+        raise NotImplementedError
+
+    def find(self, type : Literal["dungeon", "room", "user"], id : Union[DungeonId, RoomId, UserId] = None, *, name : str = None) -> Union[BaseDungeon, BaseRoom, BaseUser]:
+        """
+        Finds something.
+        """
+        raise NotImplementedError
+
+    def create(self, type : Literal["dungeon", "room", "user"], *, args : Sequence = (), kwargs : Mapping = {}) -> Union[BaseDungeon, BaseRoom, BaseUser]:
+        """
+        Creates something.
+        """
+        raise NotImplementedError
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/dungeon.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/dungeon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Submodule for dungeons.
 """
+from __future__ import annotations
 import time, copy, secrets
 from typing import Self
 from .dmtypes import (
     DungeonId, 
     BaseDungeon, 
     BaseRoom, 
     UserId,
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/room.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/room.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Submodule for dungeons.
 """
+from __future__ import annotations
 from typing import Self
 from .dmtypes import RoomId, BaseDungeon, BaseRoom
 from . import dungeon
 from . import session as _session
 from .utils import s_vars
 
 class Room(BaseRoom):
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/session.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Submodule for database connection.
 """
+from __future__ import annotations
 import random
 from typing import Literal, Union, assert_never, Sequence, Mapping
-
 from dataclasses import dataclass, field
 from . import dungeon, user, room
 from . import dba as _dba
 from .dmtypes import DungeonId, RoomId, UserId, BaseDatabaseAbstraction
 from .selectors import DUNGEON, ROOM, USER
 
 @dataclass
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker/dm_backend/modules/dm/user.py` & `dungeonmaker-0.6.9/dungeonmaker/dm_backend/modules/dm/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 Submodule for handling users.
 """
+from __future__ import annotations
 from typing import Self
-from .dmtypes import BaseUser, UserId
-from . import session as _session
+from .dmtypes import BaseUser, UserId, BaseDMSession
 from .utils import s_vars
 
 
 
 class User(BaseUser):
     """
     Class for handling users.
     """
     @classmethod
-    def lookup_user(cls, *, username : str = None, user_id : UserId = None, session : _session.DMSession) -> Self:
+    def lookup_user(cls, *, username : str = None, user_id : UserId = None, session : BaseDMSession) -> Self:
         """
         Find a user based on its username or user id.
         """
         return cls(**session.database_abstraction.select_user(user_id=user_id, fields={"username": username} if username else {}))
     
     @classmethod
-    def read(cls, user_id : UserId, *, session : _session.DMSession) -> Self:
+    def read(cls, user_id : UserId, *, session : BaseDMSession) -> Self:
         """
         Read a user based on its user_id.
         """
         return cls(**session.database_abstraction.select_user(user_id=user_id))
     
     def write(self):
         """
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker.egg-info/PKG-INFO` & `dungeonmaker-0.6.9/dungeonmaker.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.8
+Version: 0.6.9
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.8/dungeonmaker.egg-info/SOURCES.txt` & `dungeonmaker-0.6.9/dungeonmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.8/setup.py` & `dungeonmaker-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dungeonmaker',
-    version='0.6.8',
+    version='0.6.9',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='Dungeon maker backend and other things',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/dungeon-maker-reinvented',
     packages=find_packages(),
```

