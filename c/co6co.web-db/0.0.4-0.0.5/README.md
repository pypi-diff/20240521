# Comparing `tmp/co6co.web_db-0.0.4.tar.gz` & `tmp/co6co.web_db-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co6co.web_db-0.0.4.tar", last modified: Sat May 11 06:44:59 2024, max compression
+gzip compressed data, was "co6co.web_db-0.0.5.tar", last modified: Tue May 21 06:57:42 2024, max compression
```

## Comparing `co6co.web_db-0.0.4.tar` & `co6co.web_db-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.449331 co6co.web_db-0.0.4/
--rw-rw-rw-   0        0        0      482 2024-05-11 06:44:59.448331 co6co.web_db-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-11-24 08:37:18.000000 co6co.web_db-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.438254 co6co.web_db-0.0.4/co6co.web_db.egg-info/
--rw-rw-rw-   0        0        0      482 2024-05-11 06:44:59.000000 co6co.web_db-0.0.4/co6co.web_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2024-05-11 06:44:59.000000 co6co.web_db-0.0.4/co6co.web_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 06:44:59.000000 co6co.web_db-0.0.4/co6co.web_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-11 06:44:59.000000 co6co.web_db-0.0.4/co6co.web_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-11 06:44:59.000000 co6co.web_db-0.0.4/co6co.web_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-11-24 08:37:22.000000 co6co.web_db-0.0.4/co6co.web_db.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.441215 co6co.web_db-0.0.4/co6co_web_db/
--rw-rw-rw-   0        0        0      110 2024-05-11 06:44:57.000000 co6co.web_db-0.0.4/co6co_web_db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.442215 co6co.web_db-0.0.4/co6co_web_db/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 03:39:27.000000 co6co.web_db-0.0.4/co6co_web_db/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.443215 co6co.web_db-0.0.4/co6co_web_db/model/params/
--rw-rw-rw-   0        0        0      134 2024-05-06 03:39:23.000000 co6co.web_db-0.0.4/co6co_web_db/model/params/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.446332 co6co.web_db-0.0.4/co6co_web_db/services/
--rw-rw-rw-   0        0        0        0 2023-11-24 08:42:41.000000 co6co.web_db-0.0.4/co6co_web_db/services/__init__.py
--rw-rw-rw-   0        0        0     2580 2024-03-07 07:44:43.000000 co6co.web_db-0.0.4/co6co_web_db/services/db_service.py
--rw-rw-rw-   0        0        0     1801 2024-05-07 09:03:52.000000 co6co.web_db-0.0.4/co6co_web_db/services/jwt_service.py
--rw-rw-rw-   0        0        0      656 2023-12-15 03:30:50.000000 co6co.web_db-0.0.4/co6co_web_db/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:44:59.447332 co6co.web_db-0.0.4/co6co_web_db/view_model/
--rw-rw-rw-   0        0        0    15108 2024-05-11 06:34:40.000000 co6co.web_db-0.0.4/co6co_web_db/view_model/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-11 06:44:59.449331 co6co.web_db-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1162 2023-11-30 06:28:05.000000 co6co.web_db-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.145102 co6co.web_db-0.0.5/
+-rw-rw-rw-   0        0        0      482 2024-05-21 06:57:42.143103 co6co.web_db-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-11-24 08:37:18.000000 co6co.web_db-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.132107 co6co.web_db-0.0.5/co6co.web_db.egg-info/
+-rw-rw-rw-   0        0        0      482 2024-05-21 06:57:42.000000 co6co.web_db-0.0.5/co6co.web_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2024-05-21 06:57:42.000000 co6co.web_db-0.0.5/co6co.web_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:57:42.000000 co6co.web_db-0.0.5/co6co.web_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-21 06:57:42.000000 co6co.web_db-0.0.5/co6co.web_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 06:57:42.000000 co6co.web_db-0.0.5/co6co.web_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-11-24 08:37:22.000000 co6co.web_db-0.0.5/co6co.web_db.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.135107 co6co.web_db-0.0.5/co6co_web_db/
+-rw-rw-rw-   0        0        0      110 2024-05-21 06:57:40.000000 co6co.web_db-0.0.5/co6co_web_db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.136106 co6co.web_db-0.0.5/co6co_web_db/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 03:39:27.000000 co6co.web_db-0.0.5/co6co_web_db/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.137105 co6co.web_db-0.0.5/co6co_web_db/model/params/
+-rw-rw-rw-   0        0        0      134 2024-05-06 03:39:23.000000 co6co.web_db-0.0.5/co6co_web_db/model/params/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.141104 co6co.web_db-0.0.5/co6co_web_db/services/
+-rw-rw-rw-   0        0        0        0 2023-11-24 08:42:41.000000 co6co.web_db-0.0.5/co6co_web_db/services/__init__.py
+-rw-rw-rw-   0        0        0     2541 2024-05-20 07:43:06.000000 co6co.web_db-0.0.5/co6co_web_db/services/db_service.py
+-rw-rw-rw-   0        0        0     1934 2024-05-20 02:45:01.000000 co6co.web_db-0.0.5/co6co_web_db/services/jwt_service.py
+-rw-rw-rw-   0        0        0      656 2023-12-15 03:30:50.000000 co6co.web_db-0.0.5/co6co_web_db/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:57:42.142104 co6co.web_db-0.0.5/co6co_web_db/view_model/
+-rw-rw-rw-   0        0        0    15509 2024-05-14 07:46:21.000000 co6co.web_db-0.0.5/co6co_web_db/view_model/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:57:42.145102 co6co.web_db-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-11-30 06:28:05.000000 co6co.web_db-0.0.5/setup.py
```

### Comparing `co6co.web_db-0.0.4/co6co_web_db/services/db_service.py` & `co6co.web_db-0.0.5/co6co_web_db/services/db_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 from sanic import Sanic,Blueprint 
 from sanic.blueprint_group import BlueprintGroup
 import asyncio,time ,typing
 from sanic.log import logger  
 from sanic import Blueprint,Request
 from typing import TypeVar
 from co6co_db_ext.db_session import db_service 
+import multiprocessing
 
 def injectDbSessionFactory(app:Sanic,settings:dict={},engineUrl:str=None,sessionApi:list=["/api"] ):
     """
     挂在 DBSession_factory
     """
     service:db_service=None
     if settings !=None or engineUrl !=None:
         service=db_service(settings,engineUrl)
         app.ctx.service=service
         service.sync_init_tables() 
-    '''
+     
     @app.main_process_start
-    async def inject_session_factory(app:Sanic):
-        logger.info("挂在db_session_factory。。。")  
+    async def inject_session_factory(app:Sanic): 
         app.shared_ctx.cache=multiprocessing.Manager().dict()
-        app.shared_ctx.cache["db_session_factory"]=_async_session_factory 
+        #app.shared_ctx.cache["db_session_factory"]=_async_session_factory 
 
-    '''
+    
     def checkApi(request:Request):
         for api in sessionApi:
            if api in request.path:return True
         return False
```

### Comparing `co6co.web_db-0.0.4/co6co_web_db/services/jwt_service.py` & `co6co.web_db-0.0.5/co6co_web_db/services/jwt_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,17 +19,20 @@
             'iss':self._issuer,# 签名
             'data':data # 内容一般放用户ID 和开始时间 
         }
         return jwt.encode(dic,self._secret, algorithm="HS256") # 加密字符
 
     def decode(self,token:str)->Any|None: 
         try:
+            if token==None or token =="":
+                log.warn("token is None!")
+                return None
             return jwt.decode(token,self._secret,issuer=self._issuer,algorithms=['HS256']) # 解密签名  //
         except Exception as e:
-            log.err(e)
+            log.warn("校验失败:",e)
             return None
 
 async def createToken(SECRET:str,data:dict,expire_seconds:int=86400):
     """
     登录时生成tooken
     """
     svc=JWT_service(SECRET)
```

### Comparing `co6co.web_db-0.0.4/co6co_web_db/utils.py` & `co6co.web_db-0.0.5/co6co_web_db/utils.py`

 * *Files identical despite different names*

### Comparing `co6co.web_db-0.0.4/co6co_web_db/view_model/__init__.py` & `co6co.web_db-0.0.5/co6co_web_db/view_model/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,47 +100,47 @@
                     result = executer.mappings().all()
                     result = Result.success(db_tools.list2Dict(result))
                     return JSON_util.response(result)
         except Exception as e:
             errorLog(request,self.__class__,get_current_function_name())
             return Result.fail(message=f"请求失败：{e}")
 
-    async def _query(self, request: Request, select: Select  , isPO: bool = True, remove_db_instance: bool = True):
+    async def _query(self, request: Request, select: Select  , isPO: bool = True, remove_db_instance: bool = True,param:Dict|List|Tuple=None):
         """
         执行查询: 列表 
         """
         try:
             session: AsyncSession = request.ctx.session
             query = QueryListCallable(session)
-            data = await query(select, isPO, remove_db_instance)
+            data = await query(select, isPO, remove_db_instance,param)
             result = db_tools.list2Dict(data)
             return result 
         except Exception as e:
             errorLog(request,self.__class__,get_current_function_name())
             return None 
 
-    async def query_list(self, request: Request, select: Select,   isPO: bool = True, remove_db_instance: bool = True):
+    async def query_list(self, request: Request, select: Select,   isPO: bool = True, remove_db_instance: bool = True,param:Dict|List|Tuple=None):
         """
         执行查询:  列表 
         """
         try:
-            result=await self._query(request, select,   isPO , remove_db_instance)  
+            result=await self._query(request, select,   isPO , remove_db_instance,param)  
             return JSON_util.response(Result.success(data=result))
         except Exception as e:
             errorLog(request,self.__class__,get_current_function_name())
             result = Result.fail(message=f"请求失败：{e}")
             return JSON_util.response(Result.success(data=result))
 
 
-    async def query_tree(self, request: Request, select: Select, rootValue: any = None, pid_field: str = "pid", id_field: str = "id", isPO: bool = True, remove_db_instance: bool = True):
+    async def query_tree(self, request: Request, select: Select, rootValue: any = None, pid_field: str = "pid", id_field: str = "id", isPO: bool = True, remove_db_instance: bool = True,param:Dict|List|Tuple=None):
         """
         执行查询: tree列表 
         """
         try: 
-            result =   await self._query(request, select,   isPO , remove_db_instance)  
+            result =   await self._query(request, select,   isPO , remove_db_instance,param)  
             if result ==None:treeList=[]
             else :treeList = list_to_tree(result, rootValue, pid_field, id_field)
             if len(treeList) == 0:
                 return JSON_util.response(Result.success(data=[]))
             return JSON_util.response(Result.success(data=treeList))
         except Exception as e:
             errorLog(request,self.__class__,get_current_function_name())
@@ -158,22 +158,27 @@
             pageList = Page_Result.success(result, total=total)
             return JSON_util.response(pageList) 
         except Exception as e:
             errorLog(request,self.__class__,get_current_function_name())
             pageList = Page_Result.fail(message=f"请求失败：{e}")
             return JSON_util.response(pageList)
         
-    async def execSqls(self, request: Request,*sml:Update|Delete|Insert,callBck=None):
+    async def execSqls(self, request: Request,*sml:Update|Delete|Insert,callBck=None,smlParamList:List[Dict|Tuple|List]=None):
         callable = DbCallable(self.get_db_session(request))
         async def exec(session:AsyncSession):
             try:
                 result=[]
-                for sql in sml:  
-                    r=await db_tools.execSQL(session,sql) 
+                index=0
+                for sql in sml: 
+                     
+                    param= None
+                    if smlParamList!=None and len(smlParamList)==len(sml):param=smlParamList[index]
+                    r=await db_tools.execSQL(session,sql,param) 
                     result.append(r) 
+                    index+=1
                 if callBck!=None: 
                     return await callBck(*result)
             except Exception as e:
                 await session.rollback()
                 errorLog(request,self.__class__,get_current_function_name())
                 return JSON_util.response(Result.fail(e))
 
@@ -290,15 +295,15 @@
                         return result
                 return JSON_util.response(Result.success())
         except Exception as e:
             await session.rollback()
             errorLog(request,self.__class__,get_current_function_name()) 
             return JSON_util.response(Result.fail(message=e))
     
-    async def save_association(self, request: Request, currentUser:int,delSml:Delete,createPo:any,param:associationParam=None):
+    async def save_association(self, request: Request, currentUser:int,delSml:Delete,createPo:any,param:associationParam=None,delSmlParam:Dict|List|Tuple=None):
         """
         保存关联菜单
         delSml:Delete 删除语句
         createPo:(id)=>basePO
         """
         if param==None:
             param=associationParam()
@@ -306,15 +311,15 @@
         session:AsyncSession=self.get_db_session(request)
         callable=DbCallable(session) 
         async def exec(session:AsyncSession): 
             try: 
                 isChanged=False
                 # 移除
                 if(param.remove!=None and len(param.remove)>0): 
-                    result= await db_tools.execSQL(session,delSml)
+                    result= await db_tools.execSQL(session,delSml,delSmlParam)
                     if result>0:
                         isChanged=True
                 # 增加
                 if(param.add!=None and len(param.add)>0):
                     addpoList=[]
                     for id in param.add: 
                         po=await createPo(session,id)
```

### Comparing `co6co.web_db-0.0.4/setup.py` & `co6co.web_db-0.0.5/setup.py`

 * *Files identical despite different names*

