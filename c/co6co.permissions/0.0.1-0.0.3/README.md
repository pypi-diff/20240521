# Comparing `tmp/co6co.permissions-0.0.1.tar.gz` & `tmp/co6co.permissions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co6co.permissions-0.0.1.tar", last modified: Mon May 13 01:23:59 2024, max compression
+gzip compressed data, was "co6co.permissions-0.0.3.tar", last modified: Tue May 21 08:51:27 2024, max compression
```

## Comparing `co6co.permissions-0.0.1.tar` & `co6co.permissions-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.613930 co6co.permissions-0.0.1/
--rw-rw-rw-   0        0        0      447 2024-05-13 01:23:59.612930 co6co.permissions-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-04-15 02:48:28.000000 co6co.permissions-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.566218 co6co.permissions-0.0.1/co6co.permissions.egg-info/
--rw-rw-rw-   0        0        0      447 2024-05-13 01:23:58.000000 co6co.permissions-0.0.1/co6co.permissions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1423 2024-05-13 01:23:58.000000 co6co.permissions-0.0.1/co6co.permissions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:23:58.000000 co6co.permissions-0.0.1/co6co.permissions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-13 01:23:58.000000 co6co.permissions-0.0.1/co6co.permissions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-13 01:23:58.000000 co6co.permissions-0.0.1/co6co.permissions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 07:53:56.000000 co6co.permissions-0.0.1/co6co.permissions.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.568572 co6co.permissions-0.0.1/co6co_permissions/
--rw-rw-rw-   0        0        0      110 2024-04-15 02:47:00.000000 co6co.permissions-0.0.1/co6co_permissions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.576904 co6co.permissions-0.0.1/co6co_permissions/api/
--rw-rw-rw-   0        0        0      286 2024-05-07 09:17:40.000000 co6co.permissions-0.0.1/co6co_permissions/api/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-30 09:20:19.000000 co6co.permissions-0.0.1/co6co_permissions/api/menu.py
--rw-rw-rw-   0        0        0      447 2024-04-30 09:20:15.000000 co6co.permissions-0.0.1/co6co_permissions/api/role.py
--rw-rw-rw-   0        0        0      501 2024-05-07 04:15:39.000000 co6co.permissions-0.0.1/co6co_permissions/api/user.py
--rw-rw-rw-   0        0        0      791 2024-05-07 04:00:45.000000 co6co.permissions-0.0.1/co6co_permissions/api/userGroup.py
--rw-rw-rw-   0        0        0      523 2024-05-07 09:17:33.000000 co6co.permissions-0.0.1/co6co_permissions/api/view.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.579904 co6co.permissions-0.0.1/co6co_permissions/model/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:58:55.000000 co6co.permissions-0.0.1/co6co_permissions/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.581903 co6co.permissions-0.0.1/co6co_permissions/model/enum/
--rw-rw-rw-   0        0        0      626 2024-05-06 07:52:27.000000 co6co.permissions-0.0.1/co6co_permissions/model/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.588797 co6co.permissions-0.0.1/co6co_permissions/model/filters/
--rw-rw-rw-   0        0        0        0 2024-04-22 08:05:26.000000 co6co.permissions-0.0.1/co6co_permissions/model/filters/__init__.py
--rw-rw-rw-   0        0        0     1095 2024-04-28 08:19:29.000000 co6co.permissions-0.0.1/co6co_permissions/model/filters/menu_filter.py
--rw-rw-rw-   0        0        0      974 2024-04-29 06:30:07.000000 co6co.permissions-0.0.1/co6co_permissions/model/filters/role_filter.py
--rw-rw-rw-   0        0        0     1603 2024-05-07 02:26:49.000000 co6co.permissions-0.0.1/co6co_permissions/model/filters/user_filter.py
--rw-rw-rw-   0        0        0     1131 2024-04-29 06:29:27.000000 co6co.permissions-0.0.1/co6co_permissions/model/filters/user_group_filter.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.589555 co6co.permissions-0.0.1/co6co_permissions/model/pos/
--rw-rw-rw-   0        0        0        0 2024-04-22 08:05:20.000000 co6co.permissions-0.0.1/co6co_permissions/model/pos/__init__.py
--rw-rw-rw-   0        0        0     8855 2024-05-07 09:07:05.000000 co6co.permissions-0.0.1/co6co_permissions/model/pos/right.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.605033 co6co.permissions-0.0.1/co6co_permissions/view_model/
--rw-rw-rw-   0        0        0     2262 2024-05-07 05:49:07.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.608931 co6co.permissions-0.0.1/co6co_permissions/view_model/aop/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:59:08.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/aop/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-05-13 01:23:49.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/aop/api_auth.py
--rw-rw-rw-   0        0        0     1617 2024-05-07 09:00:17.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/aop/login_log.py
--rw-rw-rw-   0        0        0      771 2024-05-07 08:10:06.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/base_view.py
--rw-rw-rw-   0        0        0     2011 2024-05-07 04:15:05.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/currentUser.py
--rw-rw-rw-   0        0        0     2310 2024-05-07 09:12:40.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/login.py
--rw-rw-rw-   0        0        0     4104 2024-04-30 09:09:15.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/menu_view.py
--rw-rw-rw-   0        0        0     4681 2024-05-06 06:43:21.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/role_view.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:23:59.610931 co6co.permissions-0.0.1/co6co_permissions/view_model/ui/
--rw-rw-rw-   0        0        0        0 2024-05-07 09:18:17.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/ui/__init__.py
--rw-rw-rw-   0        0        0     1675 2024-05-07 09:43:57.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/ui/menu_view.py
--rw-rw-rw-   0        0        0     5372 2024-05-07 07:32:14.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/user.py
--rw-rw-rw-   0        0        0     5718 2024-05-07 04:01:52.000000 co6co.permissions-0.0.1/co6co_permissions/view_model/user_group.py
--rw-rw-rw-   0        0        0       42 2024-05-13 01:23:59.614928 co6co.permissions-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1151 2024-04-22 08:03:57.000000 co6co.permissions-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.889019 co6co.permissions-0.0.3/
+-rw-rw-rw-   0        0        0      506 2024-05-21 08:51:27.887020 co6co.permissions-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2024-05-21 06:53:23.000000 co6co.permissions-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.830037 co6co.permissions-0.0.3/co6co.permissions.egg-info/
+-rw-rw-rw-   0        0        0      506 2024-05-21 08:51:27.000000 co6co.permissions-0.0.3/co6co.permissions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1517 2024-05-21 08:51:27.000000 co6co.permissions-0.0.3/co6co.permissions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:51:27.000000 co6co.permissions-0.0.3/co6co.permissions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-21 08:51:27.000000 co6co.permissions-0.0.3/co6co.permissions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-21 08:51:27.000000 co6co.permissions-0.0.3/co6co.permissions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 07:53:56.000000 co6co.permissions-0.0.3/co6co.permissions.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.831037 co6co.permissions-0.0.3/co6co_permissions/
+-rw-rw-rw-   0        0        0      110 2024-05-21 06:53:42.000000 co6co.permissions-0.0.3/co6co_permissions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.840034 co6co.permissions-0.0.3/co6co_permissions/api/
+-rw-rw-rw-   0        0        0      286 2024-05-07 09:17:40.000000 co6co.permissions-0.0.3/co6co_permissions/api/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-30 09:20:19.000000 co6co.permissions-0.0.3/co6co_permissions/api/menu.py
+-rw-rw-rw-   0        0        0      447 2024-04-30 09:20:15.000000 co6co.permissions-0.0.3/co6co_permissions/api/role.py
+-rw-rw-rw-   0        0        0      501 2024-05-07 04:15:39.000000 co6co.permissions-0.0.3/co6co_permissions/api/user.py
+-rw-rw-rw-   0        0        0      791 2024-05-07 04:00:45.000000 co6co.permissions-0.0.3/co6co_permissions/api/userGroup.py
+-rw-rw-rw-   0        0        0      480 2024-05-14 04:09:43.000000 co6co.permissions-0.0.3/co6co_permissions/api/view.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.841034 co6co.permissions-0.0.3/co6co_permissions/model/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:58:55.000000 co6co.permissions-0.0.3/co6co_permissions/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.843034 co6co.permissions-0.0.3/co6co_permissions/model/enum/
+-rw-rw-rw-   0        0        0      684 2024-05-15 06:14:49.000000 co6co.permissions-0.0.3/co6co_permissions/model/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.851031 co6co.permissions-0.0.3/co6co_permissions/model/filters/
+-rw-rw-rw-   0        0        0        0 2024-04-22 08:05:26.000000 co6co.permissions-0.0.3/co6co_permissions/model/filters/__init__.py
+-rw-rw-rw-   0        0        0     1095 2024-04-28 08:19:29.000000 co6co.permissions-0.0.3/co6co_permissions/model/filters/menu_filter.py
+-rw-rw-rw-   0        0        0     1428 2024-05-21 06:33:42.000000 co6co.permissions-0.0.3/co6co_permissions/model/filters/role_filter.py
+-rw-rw-rw-   0        0        0     1734 2024-05-16 08:18:51.000000 co6co.permissions-0.0.3/co6co_permissions/model/filters/user_filter.py
+-rw-rw-rw-   0        0        0     1131 2024-04-29 06:29:27.000000 co6co.permissions-0.0.3/co6co_permissions/model/filters/user_group_filter.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.853030 co6co.permissions-0.0.3/co6co_permissions/model/pos/
+-rw-rw-rw-   0        0        0        0 2024-04-22 08:05:20.000000 co6co.permissions-0.0.3/co6co_permissions/model/pos/__init__.py
+-rw-rw-rw-   0        0        0     8855 2024-05-07 09:07:05.000000 co6co.permissions-0.0.3/co6co_permissions/model/pos/right.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.873024 co6co.permissions-0.0.3/co6co_permissions/view_model/
+-rw-rw-rw-   0        0        0     2262 2024-05-07 05:49:07.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.884020 co6co.permissions-0.0.3/co6co_permissions/view_model/aop/
+-rw-rw-rw-   0        0        0      376 2024-05-20 08:10:27.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/aop/__init__.py
+-rw-rw-rw-   0        0        0     3075 2024-05-21 03:04:51.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/aop/api_auth.py
+-rw-rw-rw-   0        0        0     2141 2024-05-21 05:51:57.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/aop/api_check.py
+-rw-rw-rw-   0        0        0     4000 2024-05-21 05:50:47.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/aop/authonCache.py
+-rw-rw-rw-   0        0        0     1615 2024-05-20 06:32:01.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/aop/login_log.py
+-rw-rw-rw-   0        0        0      581 2024-05-20 06:19:13.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/base_view.py
+-rw-rw-rw-   0        0        0     2144 2024-05-21 08:51:25.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/currentUser.py
+-rw-rw-rw-   0        0        0     2303 2024-05-20 08:52:00.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/login.py
+-rw-rw-rw-   0        0        0     4225 2024-05-20 08:44:58.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/menu_view.py
+-rw-rw-rw-   0        0        0     4785 2024-05-21 06:34:02.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/role_view.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:51:27.885020 co6co.permissions-0.0.3/co6co_permissions/view_model/ui/
+-rw-rw-rw-   0        0        0        0 2024-05-07 09:18:17.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/ui/__init__.py
+-rw-rw-rw-   0        0        0     3068 2024-05-20 06:31:35.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/ui/menu_view.py
+-rw-rw-rw-   0        0        0     5443 2024-05-20 08:47:29.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/user.py
+-rw-rw-rw-   0        0        0     5791 2024-05-20 08:46:58.000000 co6co.permissions-0.0.3/co6co_permissions/view_model/user_group.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 08:51:27.889019 co6co.permissions-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2024-04-22 08:03:57.000000 co6co.permissions-0.0.3/setup.py
```

### Comparing `co6co.permissions-0.0.1/co6co.permissions.egg-info/SOURCES.txt` & `co6co.permissions-0.0.3/co6co.permissions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,10 +28,12 @@
 co6co_permissions/view_model/login.py
 co6co_permissions/view_model/menu_view.py
 co6co_permissions/view_model/role_view.py
 co6co_permissions/view_model/user.py
 co6co_permissions/view_model/user_group.py
 co6co_permissions/view_model/aop/__init__.py
 co6co_permissions/view_model/aop/api_auth.py
+co6co_permissions/view_model/aop/api_check.py
+co6co_permissions/view_model/aop/authonCache.py
 co6co_permissions/view_model/aop/login_log.py
 co6co_permissions/view_model/ui/__init__.py
 co6co_permissions/view_model/ui/menu_view.py
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/api/menu.py` & `co6co.permissions-0.0.3/co6co_permissions/api/menu.py`

 * *Files identical despite different names*

### Comparing `co6co.permissions-0.0.1/co6co_permissions/api/userGroup.py` & `co6co.permissions-0.0.3/co6co_permissions/api/userGroup.py`

 * *Files identical despite different names*

### Comparing `co6co.permissions-0.0.1/co6co_permissions/model/enum/__init__.py` & `co6co.permissions-0.0.3/co6co_permissions/model/enum/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 class menu_type(Base_EC_Enum):
     """
     菜单类型 
     """
     group = "group","分组", 0  # 分组菜单
     api = "api","API接口", 1   # api
     view = "view", "页面视图",2  # a视图
-    button = "button","视图功能", 3  # 视图中的按钮等。
+    subView = "subView", "页面子视图",3  # a视图
+    button = "button","视图功能", 10  # 视图中的按钮等。
    
 
 class menu_state(Base_EC_Enum):
     """
     菜单类型 
     """
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/model/filters/menu_filter.py` & `co6co.permissions-0.0.3/co6co_permissions/model/filters/menu_filter.py`

 * *Files identical despite different names*

### Comparing `co6co.permissions-0.0.1/co6co_permissions/model/filters/role_filter.py` & `co6co.permissions-0.0.3/co6co_permissions/model/filters/user_group_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 
 
-from ..pos.right import RolePO
+from ..pos.right import UserGroupPO
 from sqlalchemy .orm.attributes import InstrumentedAttribute
 from typing import Tuple
 from co6co_db_ext.db_filter import absFilterItems
 from co6co.utils import log
 from sqlalchemy import func, or_, and_, Select
 
 
-class role_filter(absFilterItems): 
+class user_group_filter(absFilterItems): 
     """
-    角色 filter
-    """ 
+    用户组 filter
+    """
+    pid:int=None
     name: str = None
     code: str = None 
 
     def __init__(self): 
-        super().__init__(RolePO) 
+        super().__init__(UserGroupPO) 
  
     def filter(self) -> list:
         """
         过滤条件
         """
         filters_arr = []
-        
+        if self.checkFieldValue(self.pid) :
+            filters_arr.append(UserGroupPO.parentId.__eq__(self.pid))
         if self.checkFieldValue(self.name)  : 
-            filters_arr.append(RolePO.name.like(f"%{self.name}%"))
+            filters_arr.append(UserGroupPO.name.like(f"%{self.name}%"))
         if self.checkFieldValue(self.code):
-            filters_arr.append(RolePO.code.like(f"%{self.code}%")) 
+            filters_arr.append(UserGroupPO.code.like(f"%{self.code}%")) 
         return filters_arr
 
    
     def getDefaultOrderBy(self) -> Tuple[InstrumentedAttribute]:
         """
         默认排序
         """
-        return (RolePO.order.asc(),)
+        return (UserGroupPO.order.asc(),)
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/model/filters/user_filter.py` & `co6co.permissions-0.0.3/co6co_permissions/model/filters/user_filter.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class user_filter(absFilterItems):
     """
         用户表过滤器
     """
     name: str = None
     userGroupId: int = None
+    state:int=None
 
     def __init__(self, userName=None, userGroupId: int = None):
         super().__init__(UserPO)
         self.name = userName
         self.userGroupId = userGroupId
         self.listSelectFields=[UserPO.id,UserPO.userGroupId,UserPO.state,UserPO.createTime, UserPO.userName]
          
@@ -24,14 +25,16 @@
     def filter(self) -> list:
         """
         过滤条件
         """
         filters_arr = []
         if self.checkFieldValue(self.userGroupId):
             filters_arr.append(UserPO.userGroupId.__eq__(self.userGroupId))
+        if self.checkFieldValue(self.state):
+            filters_arr.append(UserPO.state.__eq__(self.state))
         if self.checkFieldValue(self.name):
             filters_arr.append(UserPO.userName.like(f"%{self.name}%"))
         return filters_arr
 
     def create_List_select(self):
         select=(
 				Select(UserPO.id,UserPO.userGroupId,UserPO.state,UserPO.createTime, UserPO.userName,UserGroupPO.name.label("groupName"),UserGroupPO.id.label("groupId"))
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/model/filters/user_group_filter.py` & `co6co.permissions-0.0.3/co6co_permissions/model/filters/role_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,48 @@
+from sanic.request import Request
 
 
-from ..pos.right import UserGroupPO
 from sqlalchemy .orm.attributes import InstrumentedAttribute
 from typing import Tuple
 from co6co_db_ext.db_filter import absFilterItems
 from co6co.utils import log
 from sqlalchemy import func, or_, and_, Select
+from ..pos.right import RolePO
+from ...view_model.aop.authonCache import AuthonCacheManage
 
 
-class user_group_filter(absFilterItems): 
+class role_filter(absFilterItems): 
     """
-    用户组 filter
-    """
-    pid:int=None
+    角色 filter
+    """ 
     name: str = None
     code: str = None 
-
-    def __init__(self): 
-        super().__init__(UserGroupPO) 
+    request:Request=None
+    currentRoles:list=None
+    def __init__(self,request:Request): 
+        super().__init__(RolePO) 
+        self.request=request
+    async def init(self):
+        cache=AuthonCacheManage(self.request)
+        self.currentRoles=await cache.currentRoles
  
     def filter(self) -> list:
         """
         过滤条件
         """
-        filters_arr = []
-        if self.checkFieldValue(self.pid) :
-            filters_arr.append(UserGroupPO.parentId.__eq__(self.pid))
+        filters_arr = [] 
+       
         if self.checkFieldValue(self.name)  : 
-            filters_arr.append(UserGroupPO.name.like(f"%{self.name}%"))
+            filters_arr.append(RolePO.name.like(f"%{self.name}%"))
         if self.checkFieldValue(self.code):
-            filters_arr.append(UserGroupPO.code.like(f"%{self.code}%")) 
+            filters_arr.append(RolePO.code.like(f"%{self.code}%"))
+        if  self.currentRoles!=None and len(self.currentRoles)>0:
+            filters_arr.append(RolePO.id.in_(self.currentRoles))
+
         return filters_arr
 
    
     def getDefaultOrderBy(self) -> Tuple[InstrumentedAttribute]:
         """
         默认排序
         """
-        return (UserGroupPO.order.asc(),)
+        return (RolePO.order.asc(),)
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/model/pos/right.py` & `co6co.permissions-0.0.3/co6co_permissions/model/pos/right.py`

 * *Files identical despite different names*

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/__init__.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/__init__.py`

 * *Files identical despite different names*

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/aop/login_log.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/aop/login_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from functools import wraps 
 from sanic.request import Request  
 from ...model.pos.right import LoginLogPO
-from ..base_view import getCtxUserId
+from .api_auth import getCtxUserId
 
 from datetime import datetime
 from sanic.response import JSONResponse
 
 from co6co.utils import log
 from co6co_sanic_ext.model.res.result import Result
 from co6co_db_ext.db_utils import db_tools,InsertCallable
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/base_view.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/base_view.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 from co6co_web_db.view_model import BaseMethodView,Request
-from ..model.pos.right import UserPO
-
-from .aop.api_auth import authorized
-
-
-def getCtxUserId(request:Request):
-   return request.ctx.current_user["id"]  
-
-def getCtxData(user:UserPO):
-   """
-   通过user获取 dict 保存在 request.ctx.current_user 中 
-   """
-   return user.to_jwt_dict()
+from .aop.api_auth import authorized,ctx,getCtxUserId
+ 
+class CtxMethodView(BaseMethodView): 
+   decorators=[ctx]  
 
 class AuthMethodView(BaseMethodView): 
    decorators=[authorized] 
    
    def getUserId(self, request: Request):
       """
       获取用户ID
@@ -24,8 +15,8 @@
    
    def getUserName(self, request: Request): 
        """
        获取当前用户名
        """
        current_user=request.ctx.current_user  
        return current_user.get("userName") 
-      
+
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/currentUser.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/currentUser.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,23 +21,26 @@
         修改密码：
         {
                oldPassword:""
                newPassword:""
         }
         """ 
         data=request.json
-        current_user=request.ctx.current_user 
-        self.getUserId()
-        userName=current_user.get("userName") 
+       
+        userId=self.getUserId(request)
+        userName=self.getUserName(request)
+
         oldPassword=data["oldPassword"]
         password=data["newPassword"] 
         select=(Select(UserPO).filter(UserPO.userName==userName))
         async def edit(_,one:UserPO): 
             if one!=None:
                 if one.password!=one.encrypt(oldPassword) :return JSON_util.response(Result.fail(message="输入的旧密码不正确！"))
+                if one.encrypt(password)==one.encrypt(oldPassword):return JSON_util.response(Result.fail(message="输入的旧密码与新密码一样！"))
+
                 one.password=one.encrypt(password)
             return JSON_util.response(Result.success()) 
         return await self.update_one(request,select,edit) 
 
 class user_info_view(AuthMethodView):
     routePath="/currentUser" 
     async def get(self, request:Request):
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/login.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 from co6co_web_db.view_model import BaseMethodView
-from .base_view import getCtxData
 
 from sanic.response import text
 from sanic import  Request  
 from co6co_sanic_ext.utils import JSON_util
 from co6co_sanic_ext.model.res.result import  Result   
 from sqlalchemy.ext.asyncio import AsyncSession 
 
@@ -12,14 +11,15 @@
 from co6co_db_ext.db_utils  import db_tools 
 from co6co_web_db.services.jwt_service import createToken,setCurrentUser
 from co6co.utils import log
 
 from co6co_web_db.view_model import get_one
 from ..model.pos.right import UserPO, RolePO,UserRolePO,AccountPO 
 from .aop.login_log import loginLog
+from .aop import getCtxData
 
 async def generateUserToken(request:Result,sessionId:str,data=None,userId:int=None,userOpenId:str=None,expire_seconds:int=86400): 
     token=""  
     SECRET=request.app.config.SECRET 
     if data!=None:
         token=await createToken(SECRET,data,expire_seconds)
     else: 
@@ -43,11 +43,11 @@
         select=Select(UserPO ).filter(UserPO.userName.__eq__(where.userName)) 
         user:UserPO= await self.get_one(request,select)
         if user !=None:
             if user.password==user.encrypt(where.password):   
                 token=await generateUserToken(request,user.id,user.to_jwt_dict(),expire_seconds=86400,userOpenId=user.userGroupId)
                 await setCurrentUser(request,user.to_jwt_dict()) # loginLog 获取登录ID等
                 return  JSON_util.response(Result.success(data=token, message="登录成功"))
-            else :return JSON_util.response(Result.fail(message="登录用户名或者密码不正确!"))
+            else:return JSON_util.response(Result.fail(message="登录用户名或者密码不正确!"))
         else:
             log.warn(f"未找到用户名[{where.userName}]。")
             return JSON_util.response(Result.fail(message="登录用户名或者密码不正确!"))
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/menu_view.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/menu_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from sqlalchemy.sql import Select
 from co6co_db_ext.db_utils import db_tools
 from .base_view import AuthMethodView
 from ..model.pos.right import menuPO 
 from ..model.filters.menu_filter import menu_filter
+from .aop.api_auth import menuChanged
+
   
 class menu_tree_view(AuthMethodView):
     routePath="/tree"
     
     async def get(self, request: Request):
         """
         树形选择下拉框数据
@@ -44,64 +46,69 @@
         selectTree :  el-Tree
         """
         select = (
             Select(menuPO.id, menuPO.name, menuPO.code, menuPO.parentId)
             .order_by(menuPO.parentId.asc())
         )
         return await self.query_list(request, select,  isPO=False)
-
+    
+    
     async def post(self, request: Request):
         """
         树形 table数据
         tree 形状 table
         """
         param = menu_filter()
         param.__dict__.update(request.json)
 
         return await self.query_list(request, param.list_select)
-
+    
+    @menuChanged
     async def put(self, request: Request):
         """
         增加
         """
         po = menuPO()
         userId = self.getUserId(request)
         po.__dict__.update(request.json)
         if type(po.methods) == list:
             po.methods = ",".join(po.methods)
         async def before(po: menuPO, session: AsyncSession, request):
             exist = await db_tools.exist(session,  menuPO.code.__eq__(po.code), column=menuPO.id)
             if exist:
                 return JSON_util.response(Result.fail(message=f"'{po.code}'已存在！")) 
+ 
         return await self.add(request, po, json2Po=False, userId= userId, beforeFun= before)
 
     def patch(self, request: Request):
         return text("I am patch method")
 
 
 class menu_view(AuthMethodView):
     routePath="/<pk:int>"
+    
+    @menuChanged
     async def put(self, request: Request, pk: int):
         """
         编辑
         """
         po = menuPO()
         po.__dict__.update(request.json)
         if type(po.methods) == list:
                 po.methods = ",".join(po.methods)
                 
         async def before(oldPo: menuPO, po: menuPO, session: AsyncSession, request):
             exist = await db_tools.exist(session, menuPO.id != oldPo.id, menuPO.code.__eq__(po.code), column=menuPO.id)
             if exist:
                 return JSON_util.response(Result.fail(message=f"'{po.code}'已存在！"))
             if po.parentId == oldPo.id:
-                return JSON_util.response(Result.fail(message=f"'父节点选择错误！")) 
-
+                return JSON_util.response(Result.fail(message=f"'父节点选择错误！"))  
         return await self.edit(request,pk,menuPO,po=po,userId=self.getUserId(request), fun= before)
-
+    
+    @menuChanged
     async def delete(self, request: Request, pk: int):
         """
         删除
         """
         async def before(po: menuPO, session: AsyncSession):
             count = await db_tools.count( session, menuPO.parentId == po.id, column=menuPO.id)
             if count > 0:
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/role_view.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/role_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,31 @@
 from co6co_web_db.model.params import associationParam
  
 from datetime import datetime
 from .base_view import AuthMethodView
 from ..model.pos.right import RolePO,MenuRolePO,UserRolePO,UserGroupRolePO
 from ..model.filters.role_filter import role_filter
 from ..model.pos.right import menuPO 
+from .aop.api_auth import userRoleChanged
 
 class roles_ass_view(AuthMethodView) :
     routePath="/association/<roleId:int>"
     async def post(self, request:Request,roleId:int): 
         """
         获取角色关联菜单
         """
         subSelect=Select(MenuRolePO.menuId,MenuRolePO.roleId).filter(MenuRolePO.roleId==roleId).subquery() 
         select = (
             Select(menuPO.id, menuPO.name, menuPO.code, menuPO.parentId,subSelect.c.roleId.label("associatedValue"))
             .outerjoin_from(menuPO,subSelect,onclause=subSelect.c.menuId==menuPO.id,full=False) 
             .order_by(menuPO.parentId.asc())
         ) 
         return await self.query_tree(request, select, rootValue=0, pid_field='parentId', id_field="id", isPO=False)
-
+    
+    @userRoleChanged
     async def put(self, request:Request,roleId:int):
         """
         保存角色关联菜单
         """
         param=associationParam()
         param.__dict__.update(request.json)   
         userId=self.getUserId(request)
@@ -60,15 +62,16 @@
         ) 
         return await self.query_list(request,select,  isPO=False) 
     
     async def post(self, request:Request):
         """
         table数据 
         """ 
-        param=role_filter()
+        param=role_filter(request)
+        await param.init()
         param.__dict__.update(request.json)   
         return await self.query_page(request,param ) 
     
     async def put(self,request:Request):  
         """
         增加
         """
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/user.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 from co6co_db_ext.db_utils  import db_tools
 from co6co_web_db.model.params import associationParam
 from co6co.utils import getRandomStr
 
 from .base_view import AuthMethodView
 from ..model.pos.right import UserPO, RolePO,UserRolePO,AccountPO
 from ..model.filters.user_filter import user_filter
+from .aop.api_auth import userRoleChanged
 
 class user_ass_view(AuthMethodView) :
     routePath="/association/<userId:int>"
     async def post(self, request:Request,userId:int): 
         """
         获取用户关联的角色
         """
         subSelect=Select(UserRolePO.roleId,UserRolePO.userId).filter(UserRolePO.userId==userId).subquery() 
         select = (
             Select(RolePO.id, RolePO.name, RolePO.code,subSelect.c.userId.label("associatedValue"))
             .outerjoin_from(RolePO,subSelect,onclause=subSelect.c.roleId==RolePO.id,full=False) 
             .order_by(RolePO.id.asc())
         ) 
         return await self.query_list(request, select, isPO=False)
+    
+    @userRoleChanged
     async def put(self, request:Request,userId:int):
         """
         保存用户关联角色
         """ 
         param=associationParam()
         param.__dict__.update(request.json)   
         currentUserId=self.getUserId(request)
```

### Comparing `co6co.permissions-0.0.1/co6co_permissions/view_model/user_group.py` & `co6co.permissions-0.0.3/co6co_permissions/view_model/user_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 from co6co_db_ext.db_utils  import db_tools
 from co6co_web_db.model.params import associationParam
 
 from .base_view import AuthMethodView
 from ..model.pos.right import UserGroupPO,RolePO,UserGroupRolePO
 from ..model.filters.user_group_filter import user_group_filter
 from co6co.utils import log
+from .aop.api_auth import userRoleChanged
+
 class user_group_ass_view(AuthMethodView) :
     routePath="/association/<userGroupId:int>"
     async def post(self, request:Request,userGroupId:int): 
         """
         获取用户组关联的角色
         """
         subSelect=Select(UserGroupRolePO.roleId,UserGroupRolePO.userGroupId).filter(UserGroupRolePO.userGroupId==userGroupId).subquery() 
         select = (
             Select(RolePO.id, RolePO.name, RolePO.code,subSelect.c.roleId.label("associatedValue"))
             .outerjoin_from(RolePO,subSelect,onclause=subSelect.c.roleId==RolePO.id,full=False) 
             .order_by(RolePO.name.asc())
         ) 
         return await self.query_list(request, select, isPO=False)
+    
+    @userRoleChanged
     async def put(self, request:Request,userGroupId:int):
         """
         保存角色关联菜单
         """ 
         param=associationParam()
         param.__dict__.update(request.json)   
         userId=self.getUserId(request)
```

### Comparing `co6co.permissions-0.0.1/setup.py` & `co6co.permissions-0.0.3/setup.py`

 * *Files identical despite different names*

