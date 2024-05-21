# Comparing `tmp/zjbbintest-2.6.tar.gz` & `tmp/zjbbintest-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zjbbintest-2.6.tar", last modified: Tue May 14 06:05:39 2024, max compression
+gzip compressed data, was "dist/zjbbintest-2.7.tar", last modified: Tue May 21 07:48:38 2024, max compression
```

## Comparing `zjbbintest-2.6.tar` & `zjbbintest-2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.640219 zjbbintest-2.6/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-14 06:05:39.640080 zjbbintest-2.6/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.6/README.md
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-14 06:05:39.640261 zjbbintest-2.6/setup.cfg
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      603 2024-05-14 06:05:36.000000 zjbbintest-2.6/setup.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.635841 zjbbintest-2.6/zjbbintest/
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.636679 zjbbintest-2.6/zjbbintest/Actuator/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.6/zjbbintest/Actuator/__init__.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.636854 zjbbintest-2.6/zjbbintest/Actuator/bin_test_case/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.6/zjbbintest/Actuator/bin_test_case/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13666 2024-05-13 14:02:45.000000 zjbbintest-2.6/zjbbintest/Actuator/bin_test_case/bin_test_case.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.637332 zjbbintest-2.6/zjbbintest/Actuator/bin_test_exception/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.6/zjbbintest/Actuator/bin_test_exception/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.6/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.638952 zjbbintest-2.6/zjbbintest/Actuator/utils/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-10 09:44:52.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/action_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6407 2024-05-11 07:03:52.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/assert_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3734 2024-05-12 15:28:29.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/format_check.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/processing_path.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     7611 2024-05-11 07:15:47.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/requestor.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12193 2024-05-10 09:44:52.000000 zjbbintest-2.6/zjbbintest/Actuator/utils/string_dynamic_run.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.639371 zjbbintest-2.6/zjbbintest/Analysis/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.6/zjbbintest/Analysis/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11073 2024-05-13 13:38:33.000000 zjbbintest-2.6/zjbbintest/Analysis/har2json.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11263 2024-05-13 13:52:05.000000 zjbbintest-2.6/zjbbintest/Analysis/replace_values.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.639804 zjbbintest-2.6/zjbbintest/Template/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.6/zjbbintest/Template/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1255 2024-05-10 08:40:52.000000 zjbbintest-2.6/zjbbintest/Template/bintest_template.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.6/zjbbintest/Template/report_template.html
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.6/zjbbintest/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12463 2024-05-13 13:31:46.000000 zjbbintest-2.6/zjbbintest/bintest.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.6/zjbbintest/bintest_data.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-14 06:05:39.636576 zjbbintest-2.6/zjbbintest.egg-info/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-14 06:05:39.000000 zjbbintest-2.6/zjbbintest.egg-info/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1019 2024-05-14 06:05:39.000000 zjbbintest-2.6/zjbbintest.egg-info/SOURCES.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-14 06:05:39.000000 zjbbintest-2.6/zjbbintest.egg-info/dependency_links.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-14 06:05:39.000000 zjbbintest-2.6/zjbbintest.egg-info/requires.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-14 06:05:39.000000 zjbbintest-2.6/zjbbintest.egg-info/top_level.txt
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.588231 zjbbintest-2.7/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-21 07:48:38.588108 zjbbintest-2.7/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-20 08:36:59.000000 zjbbintest-2.7/README.md
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-21 07:48:38.588277 zjbbintest-2.7/setup.cfg
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      603 2024-05-21 07:48:21.000000 zjbbintest-2.7/setup.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.583510 zjbbintest-2.7/zjbbintest/
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.584379 zjbbintest-2.7/zjbbintest/Actuator/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.7/zjbbintest/Actuator/__init__.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.584556 zjbbintest-2.7/zjbbintest/Actuator/bin_test_case/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.7/zjbbintest/Actuator/bin_test_case/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13666 2024-05-21 07:47:41.000000 zjbbintest-2.7/zjbbintest/Actuator/bin_test_case/bin_test_case.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.584945 zjbbintest-2.7/zjbbintest/Actuator/bin_test_exception/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.7/zjbbintest/Actuator/bin_test_exception/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.7/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.586804 zjbbintest-2.7/zjbbintest/Actuator/utils/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-10 09:44:52.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/action_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6407 2024-05-11 07:03:52.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/assert_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3863 2024-05-16 12:37:48.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/format_check.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/processing_path.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     7611 2024-05-11 07:15:47.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/requestor.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    10796 2024-05-17 03:22:05.000000 zjbbintest-2.7/zjbbintest/Actuator/utils/string_dynamic_run.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.587333 zjbbintest-2.7/zjbbintest/Analysis/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.7/zjbbintest/Analysis/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11094 2024-05-21 07:47:41.000000 zjbbintest-2.7/zjbbintest/Analysis/har2json.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11425 2024-05-21 07:48:21.000000 zjbbintest-2.7/zjbbintest/Analysis/replace_values.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.587836 zjbbintest-2.7/zjbbintest/Template/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.7/zjbbintest/Template/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1255 2024-05-10 08:40:52.000000 zjbbintest-2.7/zjbbintest/Template/bintest_template.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.7/zjbbintest/Template/report_template.html
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.7/zjbbintest/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11330 2024-05-20 06:33:44.000000 zjbbintest-2.7/zjbbintest/bintest.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.7/zjbbintest/bintest_data.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-21 07:48:38.584276 zjbbintest-2.7/zjbbintest.egg-info/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-21 07:48:38.000000 zjbbintest-2.7/zjbbintest.egg-info/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1019 2024-05-21 07:48:38.000000 zjbbintest-2.7/zjbbintest.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-21 07:48:38.000000 zjbbintest-2.7/zjbbintest.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-21 07:48:38.000000 zjbbintest-2.7/zjbbintest.egg-info/requires.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-21 07:48:38.000000 zjbbintest-2.7/zjbbintest.egg-info/top_level.txt
```

### Comparing `zjbbintest-2.6/setup.py` & `zjbbintest-2.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     for line in file:
         dependencies.append(line.strip())
 
 print(dependencies)
 
 setup(
     name='zjbbintest',
-    version='2.6',
+    version='2.7',
     author="zhangjiabin01",
     author_email="zhangjiabin01@baidu.com",
     description="bintest自动化框架",
     packages=find_packages(),
     package_data={
             'zjbbintest': ['Template/*'],  # 包含my_package中的templates文件夹下的所有文件
         },
```

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/bin_test_case/bin_test_case.py` & `zjbbintest-2.7/zjbbintest/Actuator/bin_test_case/bin_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             check_case(case_space_dict, case_name)
         except bt_exception.FormatCheckException as e:
             case_run_status = CaseRunStatus.CASE_FORMAT_CHECK_ERROR
             case_run_msg = str(e.message)
             return BinTestCase(case_name=case_name, case_run_status=case_run_status, case_run_msg=case_run_msg)
         case_desc = case_space_dict.get("description")
         priority = case_space_dict.get("priority")
-        case_mack_labels = case_space_dict.get("mark")
+        case_mack_labels = case_space_dict.get("tags")
         case_steps = case_space_dict.get("testSteps")
         case_step_list = []
         for case_step in case_steps:
             case_step_obj = CaseStep.create_obj_by_dict(case_step)
             case_step_list.append(case_step_obj)
         return BinTestCase(case_name=case_name, case_desc=case_desc, priority=priority,
                            case_mack_labels=case_mack_labels, case_steps=case_step_list)
```

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py` & `zjbbintest-2.7/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/utils/action_execution.py` & `zjbbintest-2.7/zjbbintest/Actuator/utils/action_execution.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/utils/assert_execution.py` & `zjbbintest-2.7/zjbbintest/Actuator/utils/assert_execution.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/utils/format_check.py` & `zjbbintest-2.7/zjbbintest/Actuator/utils/format_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,20 @@
         },
         "description": {
             "type": "string"
         },
         "priority": {
             "type": "integer",
         },
+        "tags": {
+            "type": "array",
+            "items": {
+                "type": "string"
+            },
+        },
         "testSteps": {
             "type": "array",
             "items": {
                 "type": "object",
                 "properties": {
                     "step": {
                         "type": "integer"
```

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/utils/processing_path.py` & `zjbbintest-2.7/zjbbintest/Actuator/utils/processing_path.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/utils/requestor.py` & `zjbbintest-2.7/zjbbintest/Actuator/utils/requestor.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/Actuator/utils/string_dynamic_run.py` & `zjbbintest-2.7/zjbbintest/Actuator/utils/string_dynamic_run.py`

 * *Files 11% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         """
         self.case_var_dict = case_var_dict
         self.req_dict = req_dict
         self.resp_dict = resp_dict
 
     def run(self, operable_str):
         """
-        传入可以执行的字符串如func()、var()、set()，执行具体动作，返回执行后的字符串和case级变量字典
+        传入可以执行的字符串如func()、var()、set()、action()，执行具体动作，返回执行后的字符串和case级变量字典
         :param operable_str:
         :return:
         """
         logging.debug(f'动态执行字符串：{operable_str}')
         if operable_str is None or operable_str == '':
             return ''
         operable_str = operable_str.strip()
@@ -198,39 +198,14 @@
             elif value_str.startswith("$conf"):
                 # 获取配置文件变量
                 data_source = BinTestData.config_dict
                 json_path = '$' + value_str[5:]
                 logging.debug(f'从配置文件中获取内容，jsonpath为:{json_path}；配置字典为:{data_source}')
             else:
                 return None
-            # value_path = value_str.split('.')
-            # if len(value_path) == 0:
-            #     return None
-            # if value_path[0] == "$var":
-            #     # 获取用户自定义变量
-            #     data_source = self.case_var_dict
-            #     json_path = '$' + value_str[4:]
-            #     logging.debug(f'从变量中获取内容，jsonpath为:{json_path}；变量字典为:{data_source}')
-            # elif value_path[0] == "$req":
-            #     # 获取请求响应变量
-            #     data_source = self.req_list
-            #     json_path = '$' + value_str[4:]
-            #     logging.debug(f'从请求中获取内容，jsonpath为:{json_path}；请求字典为:{data_source}')
-            # elif value_path[0] == "$resp":
-            #     # 获取请求响应变量
-            #     data_source = self.resp_list
-            #     json_path = '$' + value_str[5:]
-            #     logging.debug(f'从响应中获取内容，jsonpath为:{json_path}；响应字典为:{data_source}')
-            # elif value_path[0] == "$conf":
-            #     # 获取配置文件变量
-            #     data_source = BinTestData.config_dict
-            #     json_path = '$' + value_str[5:]
-            #     logging.debug(f'从配置文件中获取内容，jsonpath为:{json_path}；配置字典为:{data_source}')
-            # else:
-            #     return None
             expr = parse(json_path)
             result = expr.find(data_source)
             if result:
                 res_list = []
                 for match in result:
                     res_list.append(match.value)
                 if len(res_list) == 1:
```

### Comparing `zjbbintest-2.6/zjbbintest/Analysis/har2json.py` & `zjbbintest-2.7/zjbbintest/Analysis/har2json.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,22 @@
         step = {
             "step": index,
             "request": {
                 "url": url,
                 "path": path,
                 "method": request['method'],
                 "headers": {header['name']: header['value'] for header in request['headers']},
-                "param": params,
+                "params": params,
                 "body": body
             },
             "action": [],
             "assert": [
                 {
-                    "expect": f"$BT[var($resp['{index}'].status_code)]",
-                    "actual": 200,
+                    "expect": 200,
+                    "actual": f"$BT[var($resp['{index}'].status_code)]",
                     "operator": "=="
                 }
             ]
         }
         json_output['testSteps'].append(step)
         index += 1
 
@@ -297,15 +297,15 @@
 def save_json(dict_data, file_path):
     """
     将数据保存为JSON文件
     :param dict_data: 数据
     :param file_path: 文件路径
     :return: None
     """
-    res_str = json.dumps(dict_data, indent=4)
+    res_str = json.dumps(dict_data, indent=4, ensure_ascii=False)
     if file_path:
         with open(file_path, 'w', encoding='utf-8') as f:
             f.write(res_str)
 
 
 def have_easy_har(har_file_path):
     """
```

### Comparing `zjbbintest-2.6/zjbbintest/Analysis/replace_values.py` & `zjbbintest-2.7/zjbbintest/Analysis/replace_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,16 @@
     :param res_bt_str_map:
     :param resp_bt_str_map:
     :return:
     """
     new_case = {
         'caseName': case_json.get('caseName'),
         'description': case_json.get('description'),
-        'priority': case_json.get('priority')
+        'priority': case_json.get('priority'),
+        'tags': []
     }
     new_case_steps = []
     case_steps = case_json.get('testSteps')
     pre_step_bt_str_map = copy.deepcopy(conf_bt_str_map)
     for step in case_steps:
         step_id = step.get('step')
         # 先处理pre_step_bt_str_map
@@ -184,15 +185,15 @@
             'path': request_json.get('path'),
             'method': request_json.get('method'),
             # 'params': request_json.get('params'),
             'headers': request_json.get('headers')
         }
         new_request_json = replace_nested_values(new_request_json, conf_bt_str_map)
         # param和body和所有做替换
-        param_json = request_json.get('param')
+        param_json = request_json.get('params')
         body_json = request_json.get('body')
         new_param_json = replace_nested_values(param_json, pre_step_bt_str_map)
         new_body_json = replace_nested_values(body_json, pre_step_bt_str_map)
         new_request_json['param'] = new_param_json
         new_request_json['body'] = new_body_json
 
         new_step = {
@@ -245,22 +246,25 @@
             if isinstance(value, dict):
                 new_dict[key] = replace_nested_values(value, replacement_dict)
             elif isinstance(value, list):
                 new_dict[key] = [
                     replace_nested_values(item, replacement_dict) if isinstance(item, (dict, list)) else item for item
                     in value]
             elif value in replacement_dict:
+                if value is None:
+                    new_dict = None
+                    break
                 # 使用整个列表作为替换值
                 # 如果replacement_dict[value]只有一个元素，则直接使用这个元素替换
-                # 如果replacement_dict[value]有多个元素，则使用列表作为替换值，判断是否>10个元素，只取前10个
+                # 如果replacement_dict[value]有多个元素，则使用列表作为替换值，判断是否>10个元素，只取前5个和后5个元素
                 new_values = None
                 if len(replacement_dict[value]) == 1:
                     new_values = replacement_dict[value][0]
                 elif len(replacement_dict[value]) >= 10:
-                    new_values = replacement_dict[value][:10]
+                    new_values = replacement_dict[value][:5] + replacement_dict[value][-5:]
                 else:
                     new_values = replacement_dict[value]
                 new_dict[key] = {
                     value: new_values
                 }
             else:
                 new_dict[key] = value
```

### Comparing `zjbbintest-2.6/zjbbintest/Template/bintest_template.py` & `zjbbintest-2.7/zjbbintest/Template/bintest_template.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/Template/report_template.html` & `zjbbintest-2.7/zjbbintest/Template/report_template.html`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest/bintest.py` & `zjbbintest-2.7/zjbbintest/bintest.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,60 +174,37 @@
     :return:
     """
     for name, obj in getmembers(module):
         if isfunction(obj) and getattr(obj, 'is_bt_assert', False):
             BinTestData.assert_dict[name] = obj
 
 
-def case_load(path_list, mark_labels=[], priority=[]):
+def case_load(path_list, tags=[], priority=[]):
     """
     加载case，只会加载制定case
     :param path_list: 路径列表，支持多个路径，递归加载路径下的所有case
-    :param mark_labels: 加载指定标签的case，支持多个标签，比如['label1', 'label2']代表加载label1和label2的case
+    :param tags: 加载指定标签的case，支持多个标签，比如['label1', 'label2']代表加载label1和label2的case
     :param priority: 加载指定优先级的case，支持多个优先级，比如[1, 2]代表加载1和2的case
     :return: 返回case列表，list中存的是BinTestCase对象
     """
     # 获取case文件
     case_path_list = get_json_files_in_directories(path_list)
-    # 判断标签和优先级
-    # for case_path in case_path_list:
-    #     with open(case_path, 'r') as json_file:
-    #         data = json.load(json_file)
-    #     json_string = json.dumps(data)
-    #     if not mark_labels and not priority:
-    #         BinTestData.run_case_list.append(BinTestCase(json_string))
-    #     elif mark_labels and priority:
-    #         case_mark_labels = data.get('mark_label', [])
-    #         case_priority = data.get('priority', 999)
-    #         if set(case_mark_labels) & set(mark_labels) and case_priority in priority:
-    #             BinTestData.run_case_list.append(BinTestCase(json_string))
-    #     elif mark_labels and not priority:
-    #         case_mark_labels = data.get('mark_label', [])
-    #         if set(case_mark_labels) & set(mark_labels):
-    #             BinTestData.run_case_list.append(BinTestCase(json_string))
-    #     else:
-    #         case_priority = data.get('priority', 999)
-    #         if case_priority in priority:
-    #             BinTestData.run_case_list.append(BinTestCase(json_string))
-    # # 修改状态
-    # BinTestData.case_load_flag = True
-    # return
     for case_path in case_path_list:
         with open(case_path, 'r') as json_file:
             data = json.load(json_file)
-        if not mark_labels and not priority:
+        if not tags and not priority:
             BinTestData.run_case_list.append(BinTestCase.create_obj_by_dict(data))
-        elif mark_labels and priority:
-            case_mark_labels = data.get('mark_label', [])
+        elif tags and priority:
+            case_mark_labels = data.get('tags', [])
             case_priority = data.get('priority', 999)
-            if set(case_mark_labels) & set(mark_labels) and case_priority in priority:
+            if set(case_mark_labels) & set(tags) and case_priority in priority:
                 BinTestData.run_case_list.append(BinTestCase.create_obj_by_dict(data))
-        elif mark_labels and not priority:
-            case_mark_labels = data.get('mark_label', [])
-            if set(case_mark_labels) & set(mark_labels):
+        elif tags and not priority:
+            case_mark_labels = data.get('tags', [])
+            if set(case_mark_labels) & set(tags):
                 BinTestData.run_case_list.append(BinTestCase.create_obj_by_dict(data))
         else:
             case_priority = data.get('priority', 999)
             if case_priority in priority:
                 BinTestData.run_case_list.append(BinTestCase.create_obj_by_dict(data))
     # 修改状态
     BinTestData.case_load_flag = True
@@ -264,42 +241,46 @@
             case_res_list.append(case_res)
         # 生成测试报告
         render_report(case_res_list, now_time, report_path)
     else:
         raise BTCaseNotLoadException()
 
 
-def rebuild(har_file_path, conf_ini_file_path, case_dir_path=''):
+def rebuild(har_file_path, conf_ini_file_path='', case_dir_path=''):
     """
     根据har_file_path重建case，将其放在case_dir_path目录下
     case_dir_path目录下，应该存放三个文件
     1 替换后的case的json形式 xxx_case.json
     2 变量的bt_str映射关系 xxx_bt_str.json
     3 提取的请求和响应信息 xxx_req_resp.json
     :param har_file_path:
     :param conf_ini_file_path
     :param case_dir_path:
     :return: 
     """
     # 判断har_file_path是否存在
     if not os.path.exists(har_file_path):
         raise FileNotFoundError(f"har文件 {har_file_path} 不存在。")
-    if not os.path.exists(conf_ini_file_path):
-        raise FileNotFoundError(f"配置文件 {conf_ini_file_path} 不存在。")
+    if conf_ini_file_path != '':
+        if not os.path.exists(conf_ini_file_path):
+            raise FileNotFoundError(f"配置文件 {conf_ini_file_path} 不存在。")
+        conf_dict = save_conf_var(conf_ini_file_path)
+    else:
+        conf_dict = {}
+
     # 获取文件名
     file_name = os.path.basename(har_file_path)
     # 获取路径
     dir_name = os.path.dirname(har_file_path)
     # 获取基础名（不含后缀）
     base_name, _ = os.path.splitext(file_name)
 
     easy_har_list = have_easy_har(har_file_path)
     case_json = analysis_har_list(easy_har_list)
     req_dict, resp_dict = parse_har_list(easy_har_list)
-    conf_dict = save_conf_var(conf_ini_file_path)
     req_bt_str_map = get_req_bt_str_map(req_dict)
     resp_bt_str_map = get_resp_bt_str_map(resp_dict)
     conf_bt_str_map = get_conf_bt_str_map(conf_dict)
     new_case_json = case_json_replace_bintest_var(case_json, conf_bt_str_map, req_bt_str_map, resp_bt_str_map)
     req_resp_json = {}
     for req_key, req in req_dict.items():
         req_resp_json[req_key] = {
```

### Comparing `zjbbintest-2.6/zjbbintest.egg-info/SOURCES.txt` & `zjbbintest-2.7/zjbbintest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.6/zjbbintest.egg-info/requires.txt` & `zjbbintest-2.7/zjbbintest.egg-info/requires.txt`

 * *Files identical despite different names*

