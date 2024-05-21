# Comparing `tmp/co6co.db_ext-0.0.4.tar.gz` & `tmp/co6co.db_ext-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co6co.db_ext-0.0.4.tar", last modified: Sat May 11 06:45:15 2024, max compression
+gzip compressed data, was "co6co.db_ext-0.0.5.tar", last modified: Tue May 21 09:08:47 2024, max compression
```

## Comparing `co6co.db_ext-0.0.4.tar` & `co6co.db_ext-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.789774 co6co.db_ext-0.0.4/
--rw-rw-rw-   0        0        0      803 2024-05-11 06:45:15.787774 co6co.db_ext-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-01-02 01:24:42.000000 co6co.db_ext-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.651554 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/
--rw-rw-rw-   0        0        0      803 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-11-02 03:04:33.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.741127 co6co.db_ext-0.0.4/co6co_db_ext/
--rw-rw-rw-   0        0        0      107 2024-05-11 06:45:12.000000 co6co.db_ext-0.0.4/co6co_db_ext/__init__.py
--rw-rw-rw-   0        0        0     3496 2024-04-18 06:28:14.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_filter.py
--rw-rw-rw-   0        0        0    10492 2024-04-22 08:45:51.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_operations.py
--rw-rw-rw-   0        0        0     3531 2024-04-25 07:12:39.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_session.py
--rw-rw-rw-   0        0        0     8686 2024-05-07 08:54:23.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_utils.py
--rw-rw-rw-   0        0        0      423 2023-12-19 08:04:36.000000 co6co.db_ext-0.0.4/co6co_db_ext/page_param.py
--rw-rw-rw-   0        0        0     1648 2024-05-06 02:10:40.000000 co6co.db_ext-0.0.4/co6co_db_ext/po.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.785775 co6co.db_ext-0.0.4/co6co_db_ext/res/
--rw-rw-rw-   0        0        0        0 2023-11-27 04:01:15.000000 co6co.db_ext-0.0.4/co6co_db_ext/res/__init__.py
--rw-rw-rw-   0        0        0     2554 2023-12-15 03:43:22.000000 co6co.db_ext-0.0.4/co6co_db_ext/res/result.py
--rw-rw-rw-   0        0        0       42 2024-05-11 06:45:15.789774 co6co.db_ext-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-11-20 01:33:12.000000 co6co.db_ext-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 09:08:47.528699 co6co.db_ext-0.0.5/
+-rw-rw-rw-   0        0        0      803 2024-05-21 09:08:47.526703 co6co.db_ext-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-01-02 01:24:42.000000 co6co.db_ext-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 09:08:47.373471 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/
+-rw-rw-rw-   0        0        0      803 2024-05-21 09:08:47.000000 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-05-21 09:08:47.000000 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 09:08:47.000000 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-21 09:08:47.000000 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 09:08:47.000000 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-11-02 03:04:33.000000 co6co.db_ext-0.0.5/co6co.db_ext.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-21 09:08:47.490706 co6co.db_ext-0.0.5/co6co_db_ext/
+-rw-rw-rw-   0        0        0      107 2024-05-21 09:07:46.000000 co6co.db_ext-0.0.5/co6co_db_ext/__init__.py
+-rw-rw-rw-   0        0        0     3496 2024-04-18 06:28:14.000000 co6co.db_ext-0.0.5/co6co_db_ext/db_filter.py
+-rw-rw-rw-   0        0        0    10492 2024-04-22 08:45:51.000000 co6co.db_ext-0.0.5/co6co_db_ext/db_operations.py
+-rw-rw-rw-   0        0        0     3531 2024-04-25 07:12:39.000000 co6co.db_ext-0.0.5/co6co_db_ext/db_session.py
+-rw-rw-rw-   0        0        0     8993 2024-05-14 07:55:32.000000 co6co.db_ext-0.0.5/co6co_db_ext/db_utils.py
+-rw-rw-rw-   0        0        0      423 2023-12-19 08:04:36.000000 co6co.db_ext-0.0.5/co6co_db_ext/page_param.py
+-rw-rw-rw-   0        0        0     1648 2024-05-06 02:10:40.000000 co6co.db_ext-0.0.5/co6co_db_ext/po.py
+drwxrwxrwx   0        0        0        0 2024-05-21 09:08:47.525712 co6co.db_ext-0.0.5/co6co_db_ext/res/
+-rw-rw-rw-   0        0        0        0 2023-11-27 04:01:15.000000 co6co.db_ext-0.0.5/co6co_db_ext/res/__init__.py
+-rw-rw-rw-   0        0        0     2554 2023-12-15 03:43:22.000000 co6co.db_ext-0.0.5/co6co_db_ext/res/result.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 09:08:47.528699 co6co.db_ext-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-11-20 01:33:12.000000 co6co.db_ext-0.0.5/setup.py
```

### Comparing `co6co.db_ext-0.0.4/PKG-INFO` & `co6co.db_ext-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co6co.db_ext
-Version: 0.0.4
+Version: 0.0.5
 Summary: db 数据库扩展
 Home-page: http://github.com/co6co
 Author: co6co
 Author-email: co6co@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `co6co.db_ext-0.0.4/co6co.db_ext.egg-info/PKG-INFO` & `co6co.db_ext-0.0.5/co6co.db_ext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co6co.db-ext
-Version: 0.0.4
+Version: 0.0.5
 Summary: db 数据库扩展
 Home-page: http://github.com/co6co
 Author: co6co
 Author-email: co6co@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `co6co.db_ext-0.0.4/co6co_db_ext/db_filter.py` & `co6co.db_ext-0.0.5/co6co_db_ext/db_filter.py`

 * *Files identical despite different names*

### Comparing `co6co.db_ext-0.0.4/co6co_db_ext/db_operations.py` & `co6co.db_ext-0.0.5/co6co_db_ext/db_operations.py`

 * *Files identical despite different names*

### Comparing `co6co.db_ext-0.0.4/co6co_db_ext/db_session.py` & `co6co.db_ext-0.0.5/co6co_db_ext/db_session.py`

 * *Files identical despite different names*

### Comparing `co6co.db_ext-0.0.4/co6co_db_ext/db_utils.py` & `co6co.db_ext-0.0.5/co6co_db_ext/db_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,46 +100,46 @@
         """
         exist
         """
         count=await db_tools.count(session,*filters,column=column)
         if count>0:return True
         else:return False 
     
-    async def execForMappings(session:AsyncSession,select:Select):
+    async def execForMappings(session:AsyncSession,select:Select,params: Dict|Tuple|List= None):
         """
         session: AsyncSession
         select:Select 
 
         return list
         """ 
-        exec=await session.execute(select)  
+        exec=await session.execute(select,params)  
         data=  exec.mappings().all()  
         result=db_tools.list2Dict(data)  
         return result
     
-    async def execForPos(session:AsyncSession,select:Select, remove_db_instance_state:bool=True):
+    async def execForPos(session:AsyncSession,select:Select, remove_db_instance_state:bool=True,params:Dict|List|Tuple=None):
         """
         session: AsyncSession
         select:Select
         remove_db_instance_state: bool
 
         return list
         """
 
-        exec:ChunkedIteratorResult=await session.execute(select)
+        exec:ChunkedIteratorResult=await session.execute(select,params)
         if remove_db_instance_state:
             return db_tools.remove_db_instance_state(exec.scalars().fetchall())  
         else:
             return exec.scalars().fetchall() 
         
-    async def execSQL(session:AsyncSession,sql:Update|Insert|Delete)-> int:
+    async def execSQL(session:AsyncSession,sql:Update|Insert|Delete,sqlParam:Dict|List|Tuple=None)-> int:
         """
         执行简单SQL语句
         """
-        data:CursorResult=await session.execute(sql)
+        data:CursorResult=await session.execute(sql,sqlParam)
         return data.rowcount
     
 
     
 
 '''
 exec.fetchone() //None| (data,)
@@ -152,17 +152,17 @@
     def __init__(self,session:AsyncSession):
         self.session=session
     async def __call__(self, func ):
         async with self.session,self.session.begin():
             if func!=None:return await func(self.session)
             
 class QueryOneCallable(DbCallable):  
-    async def __call__(self, select :Select,isPO:bool=True):
+    async def __call__(self, select :Select,isPO:bool=True,param:Dict|List|Tuple=None):
         async def exec(session:AsyncSession):
-            exec=await session.execute(select)  
+            exec=await session.execute(select,param)  
             if isPO:  
                 data=exec.fetchone()
                 # 返回的是元组
                 if data!=None:return data[0]
                 else: return None
             else:
                 data=exec.mappings().fetchone()
@@ -178,18 +178,18 @@
             except Exception as e:
                 await session.rollback()
                 log.warn("执行'InsertOneCallable'异常",e)
                 raise 
         return await super().__call__(exec) 
     
 class UpdateOneCallable(DbCallable):
-    async def __call__(self, queryOneSelect :Select,editFn:None):
+    async def __call__(self, queryOneSelect:Select,editFn:None,param:Dict|List|Tuple=None):
         async def exec(session:AsyncSession):
             try:
-                exec=await session.execute(queryOneSelect)   
+                exec=await session.execute(queryOneSelect,param)   
                 data=exec.fetchone()
                 # 返回的是元组 
                 one=None
                 if data!=None:one= data[0]
                 else: one=  None
                 if editFn!=None:
                     result= await editFn(session,one)  
@@ -200,34 +200,34 @@
                 log.warn("执行'UpdateOneCallable'异常",e)
                 raise
 
         return await super().__call__(exec) 
 
          
 class QueryListCallable(DbCallable):  
-    async def __call__(self, select :Select,isPO:bool=True,remove_db_instance=True):
+    async def __call__(self, select:Select,isPO:bool=True,remove_db_instance=True,param:Dict|List|Tuple=None ):
         async def exec(session:AsyncSession):
             if isPO: 
-               result=await db_tools.execForPos(session,select,remove_db_instance)
+               result=await db_tools.execForPos(session,select,remove_db_instance,params=param)
             else:
-               result=await db_tools.execForMappings(session,select)
+               result=await db_tools.execForMappings(session,select,params=param)
             return result
         #return await super(QueryListCallable,self).__call__(exec) #// 2.x 写法
         return await super().__call__(exec)
 
 class QueryPagedCallable(DbCallable):  
-    async def __call__(self, countSelect:Select, select :Select,isPO:bool=True,remove_db_instance=True) ->Tuple[int,List[dict]]:
+    async def __call__(self, countSelect:Select, select :Select,isPO:bool=True,remove_db_instance=True,param:Dict|List|Tuple=None) ->Tuple[int,List[dict]]:
         async def exec(session:AsyncSession):
-            total=await session.execute(countSelect)
+            total=await session.execute(countSelect,param)
             total=total.scalar()  
             if isPO: 
-                result=await db_tools.execForPos(session,select,remove_db_instance)
+                result=await db_tools.execForPos(session,select,remove_db_instance,param)
             else: 
-                result=await db_tools.execForMappings(session,select) 
+                result=await db_tools.execForMappings(session,select,param) 
 
             return total,result  
         return await super().__call__(exec)
 
 class QueryPagedByFilterCallable(QueryPagedCallable):  
-    async def __call__(self, filter:absFilterItems,isPO:bool=True,remove_db_instance=True) ->Tuple[int,List[dict]]:   
-        return await super().__call__(filter.count_select,filter.list_select,isPO ,remove_db_instance) 
+    async def __call__(self, filter:absFilterItems,isPO:bool=True,remove_db_instance=True,param:Dict|List|Tuple=None) ->Tuple[int,List[dict]]:   
+        return await super().__call__(filter.count_select,filter.list_select,isPO ,remove_db_instance,param)
```

### Comparing `co6co.db_ext-0.0.4/co6co_db_ext/po.py` & `co6co.db_ext-0.0.5/co6co_db_ext/po.py`

 * *Files identical despite different names*

### Comparing `co6co.db_ext-0.0.4/co6co_db_ext/res/result.py` & `co6co.db_ext-0.0.5/co6co_db_ext/res/result.py`

 * *Files identical despite different names*

### Comparing `co6co.db_ext-0.0.4/setup.py` & `co6co.db_ext-0.0.5/setup.py`

 * *Files identical despite different names*

