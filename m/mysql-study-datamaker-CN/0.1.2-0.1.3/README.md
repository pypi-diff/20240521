# Comparing `tmp/mysql_study_datamaker_cn-0.1.2.tar.gz` & `tmp/mysql_study_datamaker_cn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_study_datamaker_cn-0.1.2.tar", last modified: Sat May 11 20:25:46 2024, max compression
+gzip compressed data, was "mysql_study_datamaker_cn-0.1.3.tar", last modified: Tue May 21 04:59:19 2024, max compression
```

## Comparing `mysql_study_datamaker_cn-0.1.2.tar` & `mysql_study_datamaker_cn-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.536629 mysql_study_datamaker_cn-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      860 2024-05-11 20:25:46.532049 mysql_study_datamaker_cn-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      443 2024-05-11 20:23:35.000000 mysql_study_datamaker_cn-0.1.2/README.md
--rw-rw-rw-   0        0        0      425 2024-05-11 20:25:36.000000 mysql_study_datamaker_cn-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 20:25:46.536629 mysql_study_datamaker_cn-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.505002 mysql_study_datamaker_cn-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.517342 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/
--rw-rw-rw-   0        0        0      147 2024-05-11 20:18:58.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/__init__.py
--rw-rw-rw-   0        0        0    19927 2024-05-11 20:23:35.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/datamaker.py
--rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_family.txt
--rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_names.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 20:25:46.532049 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/
--rw-rw-rw-   0        0        0      860 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-11 20:25:46.000000 mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 04:59:19.700561 mysql_study_datamaker_cn-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      860 2024-05-21 04:59:19.694893 mysql_study_datamaker_cn-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-05-11 20:23:35.000000 mysql_study_datamaker_cn-0.1.3/README.md
+-rw-rw-rw-   0        0        0      425 2024-05-21 04:58:47.000000 mysql_study_datamaker_cn-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:59:19.700561 mysql_study_datamaker_cn-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 04:59:19.629252 mysql_study_datamaker_cn-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 04:59:19.662362 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/
+-rw-rw-rw-   0        0        0      147 2024-05-11 20:18:58.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/__init__.py
+-rw-rw-rw-   0        0        0    19958 2024-05-21 04:57:58.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/datamaker.py
+-rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/new_family.txt
+-rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/new_names.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 04:59:19.691881 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN.egg-info/
+-rw-rw-rw-   0        0        0      860 2024-05-21 04:59:19.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-05-21 04:59:19.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:59:19.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-21 04:59:19.000000 mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN.egg-info/top_level.txt
```

### Comparing `mysql_study_datamaker_cn-0.1.2/LICENSE` & `mysql_study_datamaker_cn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.1.2/PKG-INFO` & `mysql_study_datamaker_cn-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_study_datamaker_CN
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate some data and convert it to MySQL language.
 Author-email: Kavin <scratch_test@126.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/datamaker.py` & `mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/datamaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -278,53 +278,64 @@
             elif item == "日期":
                 self.__informations[item] = self.__get_random_date()
 
 
     def __iter__(self):
         return self
 
+
     def __next__(self):
 
         result = ""
-        for k, v in self.__informations.items():
-            if k == "DATE":
-                temp = next(v)
-                for item in self.__args:
-                    if item == "生日":
-                        result += temp[0] + ","
-                    elif item == "年龄":
-                        result += temp[1] + ","
-                    elif item == "身份证":
-                        result += temp[2] + ","
+        if "DATE" in self.__informations:
+            temp = next(self.__informations["DATE"])
 
+        for item in self.__args:
+            if item == "生日":
+                result += temp[0] + ","
+            elif item == "年龄":
+                result += temp[1] + ","
+            elif item == "身份证":
+                result += temp[2] + ","
             else:
-                result += next(v) + ","
+                result += next(self.__informations[item]) + ","
+
+
         result = result[:-1]
         if not result:
             raise StopIteration
         return result
 
-    def create_insertinto(self):
+    def create(self, code="insert_into"):
         """
         需要先生成一个DataMaker对象，来创建指定数量和字段，再调用该方法，写入到一个txt文本中；
         :param self: 生成的对象
         :param file: txt文件名
         :return: None
         """
-        with open("insert_into_" + self.file, "x", encoding="utf-8") as f:
-            f.write(f"insert into xxx values {('PRIMARYKEY_ID',) + self.__args} \n")
-            id = 1
-            for line in self:
-                comment = "(" + str(id) + "," + line + "),\n"
-                id += 1
-                f.write(comment)
+        if code == "insert_into":
+            with open("insert_into_" + self.file, "x", encoding="utf-8") as f:
+                f.write(f"insert into xxx values {('PRIMARYKEY_ID',) + self.__args} \n")
+                id = 1
+                for line in self:
+                    comment = "(" + str(id) + "," + line + "),\n"
+                    id += 1
+                    f.write(comment)
                 
     
 def get_help():
     content = """
+    
+    --- ver 0.1.3 ---
+    更改内容：
+        | -- create_insertinto() 方法 更名为 create方法，需要传递 code 参数来生成指定的 Mysql语法信息，默认”insert_into“；
+    bug修复：
+        | -- 修复了 年龄、身份证、生日与其他字段顺序不统一的录入问题
+        
+        
     --- ver 0.1.2 ---
     增加内容：
         | -- 增加了 get_demo() 函数，查看详细的案例演示；
     
     bug修复：
         | -- 修复了 电话/手机 的不统一问题，只能用 手机；
         
@@ -392,19 +403,12 @@
         one = DataMaker(100, ("姓名", "性别", "生日", "年龄", "身份证", "部门", "手机"))
         one.create_insertinto()
     """
     print(content)
 
 if __name__ == '__main__':
     """
-    下面是案例，直接运行可以获得测试代码，生成15个随机数据；
+    下面是案例，直接运行可以获得测试代码，生成50个随机数据；
     """
-    get_demo()
-    # args = ("姓名", "性别", "工号", "分数语文", "分数数学", "分数英语")
-    # one = DataMaker(33, args, left=2010, gender="cn", file='date')
-    # one.create_insertinto()
-
-    # one = DataMaker(50, ("姓名", "性别", "工号", "分数语文", "分数数学", "分数英语"), work_head="2024.三班", work_numwidth=2)
-    # one.create_insertinto()
-
-    # one = DataMaker(100, ("姓名", "性别", "生日", "年龄", "身份证", "部门", "手机"))
-    # one.create_insertinto()
+    one = DataMaker(50, ("姓名", "年龄", "性别", "生日", "部门", "身份证"),
+                    work_head="2024.三班", work_numwidth=2, file='date')
+    one.create()
```

### Comparing `mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_family.txt` & `mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/new_family.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN/new_names.txt` & `mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN/new_names.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.1.2/src/mysql_study_datamaker_CN.egg-info/PKG-INFO` & `mysql_study_datamaker_cn-0.1.3/src/mysql_study_datamaker_CN.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_study_datamaker_CN
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate some data and convert it to MySQL language.
 Author-email: Kavin <scratch_test@126.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

