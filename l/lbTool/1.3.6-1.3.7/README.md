# Comparing `tmp/lbtool-1.3.6.tar.gz` & `tmp/lbtool-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbtool-1.3.6.tar", last modified: Mon May 20 14:11:33 2024, max compression
+gzip compressed data, was "lbtool-1.3.7.tar", last modified: Tue May 21 06:13:08 2024, max compression
```

## Comparing `lbtool-1.3.6.tar` & `lbtool-1.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 14:11:33.948184 lbtool-1.3.6/
--rw-rw-rw-   0        0        0     6018 2024-05-20 14:11:33.946702 lbtool-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     5505 2024-05-20 14:03:32.000000 lbtool-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 14:11:33.934388 lbtool-1.3.6/lbTool/
--rw-rw-rw-   0        0        0     4492 2024-01-25 15:49:04.000000 lbtool-1.3.6/lbTool/Common.py
--rw-rw-rw-   0        0        0     1075 2024-01-25 15:49:04.000000 lbtool-1.3.6/lbTool/ConfigManager.py
--rw-rw-rw-   0        0        0    10446 2024-05-16 15:08:28.000000 lbtool-1.3.6/lbTool/Db.py
--rw-rw-rw-   0        0        0    18181 2024-05-16 15:08:28.000000 lbtool-1.3.6/lbTool/DmDb.py
--rw-rw-rw-   0        0        0     4063 2024-01-25 15:49:04.000000 lbtool-1.3.6/lbTool/EnCipher.py
--rw-rw-rw-   0        0        0     2280 2024-01-25 15:49:04.000000 lbtool-1.3.6/lbTool/FileUtil.py
--rw-rw-rw-   0        0        0     3140 2024-05-16 15:08:28.000000 lbtool-1.3.6/lbTool/Logging.py
--rw-rw-rw-   0        0        0        0 2024-01-25 15:49:04.000000 lbtool-1.3.6/lbTool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:11:33.944744 lbtool-1.3.6/lbTool.egg-info/
--rw-rw-rw-   0        0        0     6018 2024-05-20 14:11:33.000000 lbtool-1.3.6/lbTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-05-20 14:11:33.000000 lbtool-1.3.6/lbTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 14:11:33.000000 lbtool-1.3.6/lbTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2024-05-20 14:11:33.000000 lbtool-1.3.6/lbTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 14:11:33.000000 lbtool-1.3.6/lbTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 14:11:33.948184 lbtool-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1064 2024-05-20 14:11:25.000000 lbtool-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:13:08.315133 lbtool-1.3.7/
+-rw-rw-rw-   0        0        0     6088 2024-05-21 06:13:08.314135 lbtool-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5575 2024-05-21 06:11:39.000000 lbtool-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:13:08.307153 lbtool-1.3.7/lbTool/
+-rw-rw-rw-   0        0        0     4492 2023-12-04 07:29:53.000000 lbtool-1.3.7/lbTool/Common.py
+-rw-rw-rw-   0        0        0     1075 2023-11-08 02:54:21.000000 lbtool-1.3.7/lbTool/ConfigManager.py
+-rw-rw-rw-   0        0        0    10446 2024-05-16 08:08:55.000000 lbtool-1.3.7/lbTool/Db.py
+-rw-rw-rw-   0        0        0    18814 2024-05-21 06:04:53.000000 lbtool-1.3.7/lbTool/DmDb.py
+-rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbtool-1.3.7/lbTool/EnCipher.py
+-rw-rw-rw-   0        0        0     2280 2023-08-22 15:07:22.000000 lbtool-1.3.7/lbTool/FileUtil.py
+-rw-rw-rw-   0        0        0     3140 2024-05-20 01:50:21.000000 lbtool-1.3.7/lbTool/Logging.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbtool-1.3.7/lbTool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:13:08.313138 lbtool-1.3.7/lbTool.egg-info/
+-rw-rw-rw-   0        0        0     6088 2024-05-21 06:13:08.000000 lbtool-1.3.7/lbTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-05-21 06:13:08.000000 lbtool-1.3.7/lbTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:13:08.000000 lbtool-1.3.7/lbTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-05-21 06:13:08.000000 lbtool-1.3.7/lbTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 06:13:08.000000 lbtool-1.3.7/lbTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:13:08.315133 lbtool-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-05-21 06:12:44.000000 lbtool-1.3.7/setup.py
```

### Comparing `lbtool-1.3.6/PKG-INFO` & `lbtool-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbTool
-Version: 1.3.6
+Version: 1.3.7
 Summary: Multifunctional Toolset
 Author: lb
 Author-email: lcoolb@163.com
 Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: gmSsl==3.2.2
@@ -63,14 +63,16 @@
 
 # 依靠config.yml配置文件获取连接参数，可查看下方配置文件区域
 # 添加自动生成实体，便捷使用增删查改
 # 获取数据库连接1
 # db = DmDatabase('ip:port', 'user', 'password')
 # 获取数据库连接2
 db = get_dm_con()
+# 控制台不显示执行sql,设置False关闭
+db.show_sql = False
 
 # 1.语句方式使用
 # 查询
 sql = "select * from test where id=1"
 data = db.query(sql)
 sql1 = "select * from test where id=?"
 data1 = db.query(sql1, 1)
```

### Comparing `lbtool-1.3.6/README.md` & `lbtool-1.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 # 依靠config.yml配置文件获取连接参数，可查看下方配置文件区域
 # 添加自动生成实体，便捷使用增删查改
 # 获取数据库连接1
 # db = DmDatabase('ip:port', 'user', 'password')
 # 获取数据库连接2
 db = get_dm_con()
+# 控制台不显示执行sql,设置False关闭
+db.show_sql = False
 
 # 1.语句方式使用
 # 查询
 sql = "select * from test where id=1"
 data = db.query(sql)
 sql1 = "select * from test where id=?"
 data1 = db.query(sql1, 1)
```

### Comparing `lbtool-1.3.6/lbTool/Common.py` & `lbtool-1.3.7/lbTool/Common.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.6/lbTool/ConfigManager.py` & `lbtool-1.3.7/lbTool/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.6/lbTool/Db.py` & `lbtool-1.3.7/lbTool/Db.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.6/lbTool/DmDb.py` & `lbtool-1.3.7/lbTool/DmDb.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,14 @@
         where_condition = []
         for key, value in kwargs.items():
             if key.lower() not in cls._columns_:
                 raise KeyError(key)
             where_condition.append(f"{key.upper()}=:{key}")
         sql += " AND ".join(where_condition)
         result = cls._database_.query_sql(sql, **kwargs)
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         if result is None:
             return None
         for key, value in result.items():
             if key.lower() == cls._pk_column_:
                 setattr(cls, "_pk_", value)  # 设置主键值
             setattr(cls, key.lower(), value)
         return cls
@@ -128,17 +125,14 @@
         where_condition = []
         for key, value in kwargs.items():
             if key.lower() not in cls._columns_:
                 raise KeyError(key)
             where_condition.append(f"{key.upper()}=:{key}")
         sql += " AND ".join(where_condition)
         result = cls._database_.query_sql_list(sql, **kwargs)
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         if len(result) == 0:
             return result
         end_data = []
         for item in result:
             new_entity = type(cls._class_name_, (cls,), {})  # 生成对象新实例
             for key, value in item.items():
                 if key.lower() == cls._pk_column_:
@@ -162,17 +156,14 @@
             if key.lower() not in cls._columns_:
                 raise KeyError(key)
             where_condition.append(f"{key.upper()}=:{key}")
         sql += " AND ".join(where_condition)
         # 拼接分页sql
         page_sql = f"SELECT * FROM (SELECT TMP_PAGE.*, ROWNUM AS RN FROM ({sql}) TMP_PAGE WHERE ROWNUM <= {page_num * page_size}) WHERE RN > {(page_num - 1) * page_size}"
         result = cls._database_.query_sql_list(page_sql, **kwargs)
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         if len(result) == 0:
             return result
         end_data = []
         for item in result:
             new_entity = type(cls._class_name_, (cls,), {})  # 生成对象新实例
             for key, value in item.items():
                 if key != "RN":  # 行号不赋值
@@ -193,17 +184,14 @@
         where_condition = []
         for key, value in kwargs.items():
             if key.lower() not in cls._columns_:
                 raise KeyError(key)
             where_condition.append(f"{key.upper()}=:{key}")
         sql += " AND ".join(where_condition)
         result = cls._database_.query_sql(sql, **kwargs)
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         return result['TOTAL_COUNT']
 
     def insert(cls, **kwargs):
         """
         新增数据
         :param kwargs: 参数字典
         :return:
@@ -211,17 +199,14 @@
         table_name = cls.__get_table_name()
         for key, value in kwargs.items():
             if key.lower() not in cls._columns_:
                 raise KeyError(key)
         fields = ",".join(item.upper() for item in kwargs.keys())
         values = ",".join(f":{item}" for item in kwargs.keys())
         sql = f"INSERT INTO {table_name}({fields}) VALUES ({values})"
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         affect_rows = cls._database_.execute(sql, **kwargs)
         return affect_rows
 
     def update_dict(cls, **kwargs):
         """
         修改数据
         :param kwargs: 参数字典
@@ -238,17 +223,14 @@
                 raise RuntimeError(f"数据表{table_name}主键为空或未传入主键参数！")
             if key == cls._pk_column_:
                 key_str = key.upper() + f"=:{key}"
             else:
                 update_data.append(f"{key.upper()}=:{key}")
         update_str = ",".join(update_data)
         sql = f"UPDATE {table_name} SET {update_str} WHERE {key_str}"
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         affect_rows = cls._database_.execute(sql, **kwargs)
         return affect_rows
 
     def update(cls, entity_data):
         """
         修改数据
         :param entity_data: 实体
@@ -263,17 +245,14 @@
         for key, value in dict_data.items():
             if key == cls._pk_column_:
                 key_str = key.upper() + f"=:{key}"
             else:
                 update_data.append(f"{key.upper()}=:{key}")
         update_str = ",".join(update_data)
         sql = f"UPDATE {table_name} SET {update_str} WHERE {key_str}"
-        # 打印语句和参数
-        print(sql)
-        print(dict_data)
         affect_rows = cls._database_.execute(sql, **dict_data)
         return affect_rows
 
     def delete(cls, **kwargs):
         """
         删除数据
         :param kwargs: 参数字典
@@ -283,17 +262,14 @@
         delete_condition = []
         for key, value in kwargs.items():
             if key.lower() not in cls._columns_:
                 raise KeyError(key)
             delete_condition.append(f"{key.upper()}=:{key}")
         delete_str = " AND ".join(delete_condition)
         sql = f"DELETE FROM {table_name} where {delete_str}"
-        # 打印语句和参数
-        print(sql)
-        print(kwargs)
         affect_rows = cls._database_.execute(sql, **kwargs)
         return affect_rows
 
 
 class DmDatabase:
     """
     达梦操作类
@@ -303,14 +279,15 @@
         """
         初始化
         :param dsn: 连接描述
         :param user: 用户名
         :param password: 密码
         :param contextmanager: 是否使用上下文管理器标识
         """
+        self.show_sql = True  # 是否展示语句，默认为True
         self.conn = None
         self.dsn = dsn
         self.user = user
         self.password = password
         self.contextmanager = contextmanager
         if not self.contextmanager:
             # 不使用上下文管理器时直接连接
@@ -421,18 +398,29 @@
             raise ex
 
     def query_sql(self, sql, *args, **kwargs):
         try:
             cursor = self.conn.cursor()
             if args:
                 cursor.execute(sql, *args)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
+                    print(args)
             elif kwargs:
                 cursor.execute(sql, **kwargs)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
+                    print(kwargs)
             else:
                 cursor.execute(sql)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
             result = cursor.fetchone()
             if result is None:
                 return None
             # 查出当前查询的列名，保存到columns
             columns = [column[0] for column in cursor.description]
             # 组合字典形式{"name":"test","age":18}
             res_data = dict(zip(columns, result))
@@ -443,18 +431,29 @@
             return None
 
     def query_sql_list(self, sql, *args, **kwargs):
         try:
             cursor = self.conn.cursor()
             if args:
                 cursor.execute(sql, *args)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
+                    print(args)
             elif kwargs:
                 cursor.execute(sql, **kwargs)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
+                    print(kwargs)
             else:
                 cursor.execute(sql)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
             result = cursor.fetchall()
             # 查出当前查询的列名，保存到columns
             columns = [column[0] for column in cursor.description]
             # 定义一个数组，用来保存每一组的数组，格式为字典形式{"name":"test","age":18}
             sub_resdata = []
             for row in result:
                 # 循环遍历查询出来的结果，然后生成字典
@@ -467,18 +466,29 @@
             return None
 
     def execute(self, sql, *args, **kwargs):
         try:
             cursor = self.conn.cursor()
             if args:
                 cursor.execute(sql, *args)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
+                    print(args)
             elif kwargs:
                 cursor.execute(sql, **kwargs)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
+                    print(kwargs)
             else:
                 cursor.execute(sql)
+                # 打印语句和参数
+                if self.show_sql:
+                    print(sql)
             result = cursor.rowcount  # 返回影响行数
             cursor.close()
             return result
         except dmPython.Error as ex:
             raise RuntimeError(ex)
```

### Comparing `lbtool-1.3.6/lbTool/EnCipher.py` & `lbtool-1.3.7/lbTool/EnCipher.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.6/lbTool/FileUtil.py` & `lbtool-1.3.7/lbTool/FileUtil.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.6/lbTool/Logging.py` & `lbtool-1.3.7/lbTool/Logging.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.6/lbTool.egg-info/PKG-INFO` & `lbtool-1.3.7/lbTool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbTool
-Version: 1.3.6
+Version: 1.3.7
 Summary: Multifunctional Toolset
 Author: lb
 Author-email: lcoolb@163.com
 Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: gmSsl==3.2.2
@@ -63,14 +63,16 @@
 
 # 依靠config.yml配置文件获取连接参数，可查看下方配置文件区域
 # 添加自动生成实体，便捷使用增删查改
 # 获取数据库连接1
 # db = DmDatabase('ip:port', 'user', 'password')
 # 获取数据库连接2
 db = get_dm_con()
+# 控制台不显示执行sql,设置False关闭
+db.show_sql = False
 
 # 1.语句方式使用
 # 查询
 sql = "select * from test where id=1"
 data = db.query(sql)
 sql1 = "select * from test where id=?"
 data1 = db.query(sql1, 1)
```

### Comparing `lbtool-1.3.6/setup.py` & `lbtool-1.3.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lbTool',  # 包的名称
-    version='1.3.6',  # 版本号
+    version='1.3.7',  # 版本号
     author='lb',  # 作者名
     author_email='lcoolb@163.com',
     description='Multifunctional Toolset',  # 包的描述信息
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # 包含的所有包
     install_requires=[  # 依赖的其他包
```

