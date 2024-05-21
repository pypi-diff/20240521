# Comparing `tmp/toui-3.5.0a7.tar.gz` & `tmp/toui-3.5.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.5.0a7.tar", last modified: Sun May 12 06:42:57 2024, max compression
+gzip compressed data, was "toui-3.5.0a8.tar", last modified: Tue May 21 17:23:29 2024, max compression
```

## Comparing `toui-3.5.0a7.tar` & `toui-3.5.0a8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 06:42:57.282803 toui-3.5.0a7/
--rw-rw-rw-   0        0        0     1094 2024-05-10 13:17:12.000000 toui-3.5.0a7/LICENSE
--rw-rw-rw-   0        0        0       16 2024-05-10 13:17:12.000000 toui-3.5.0a7/MANIFEST.in
--rw-rw-rw-   0        0        0     5411 2024-05-12 06:42:57.280788 toui-3.5.0a7/PKG-INFO
--rw-rw-rw-   0        0        0     4975 2024-05-10 13:17:12.000000 toui-3.5.0a7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 06:42:57.233475 toui-3.5.0a7/examples/
--rw-rw-rw-   0        0        0        0 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0     1373 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/advanced_example_2_toui_with_javascript.py
--rw-rw-rw-   0        0        0     2119 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/advanced_example_3_toui_with_google_sign_in.py
--rw-rw-rw-   0        0        0     3663 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/advanced_example_4_toui_with_firebase.py
--rw-rw-rw-   0        0        0     2806 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/advanced_example_5_toui_with_sql_user_database.py
--rw-rw-rw-   0        0        0     7653 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/advanced_example_6_widgets.py
--rw-rw-rw-   0        0        0      556 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2024-05-10 13:17:12.000000 toui-3.5.0a7/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2024-05-12 06:42:57.250308 toui-3.5.0a7/images/
--rw-rw-rw-   0        0        0  2404280 2024-05-10 13:17:12.000000 toui-3.5.0a7/images/calculator.gif
--rw-rw-rw-   0        0        0  2803703 2024-05-10 13:17:12.000000 toui-3.5.0a7/images/home.gif
--rw-rw-rw-   0        0        0    27837 2024-05-10 13:17:12.000000 toui-3.5.0a7/images/icon.png
--rw-rw-rw-   0        0        0    29049 2024-05-10 13:17:12.000000 toui-3.5.0a7/images/logo.png
--rw-rw-rw-   0        0        0       42 2024-05-12 06:42:57.283342 toui-3.5.0a7/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-05-12 06:41:41.000000 toui-3.5.0a7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 06:42:57.266914 toui-3.5.0a7/toui/
--rw-rw-rw-   0        0        0      291 2024-05-12 06:41:45.000000 toui-3.5.0a7/toui/__init__.py
--rw-rw-rw-   0        0        0      379 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/_helpers.py
--rw-rw-rw-   0        0        0    12059 2024-05-12 06:35:52.000000 toui-3.5.0a7/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/_signals.py
--rw-rw-rw-   0        0        0    64448 2024-05-12 06:36:18.000000 toui-3.5.0a7/toui/apps.py
--rw-rw-rw-   0        0        0    27205 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/elements.py
--rw-rw-rw-   0        0        0      451 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/exceptions.py
--rw-rw-rw-   0        0        0    22102 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2024-05-10 13:17:12.000000 toui-3.5.0a7/toui/structure.py
-drwxrwxrwx   0        0        0        0 2024-05-12 06:42:57.275264 toui-3.5.0a7/toui.egg-info/
--rw-rw-rw-   0        0        0     5411 2024-05-12 06:42:57.000000 toui-3.5.0a7/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-05-12 06:42:57.000000 toui-3.5.0a7/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 06:42:57.000000 toui-3.5.0a7/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-12 06:42:57.000000 toui-3.5.0a7/toui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      253 2024-05-12 06:42:57.000000 toui-3.5.0a7/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-12 06:42:57.000000 toui-3.5.0a7/toui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 06:42:57.279782 toui-3.5.0a7/touicmd/
--rw-rw-rw-   0        0        0       18 2024-05-10 13:53:34.000000 toui-3.5.0a7/touicmd/__init__.py
--rw-rw-rw-   0        0        0     2617 2024-05-10 13:17:12.000000 toui-3.5.0a7/touicmd/_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:23:29.511804 toui-3.5.0a8/
+-rw-rw-rw-   0        0        0     1094 2024-05-10 13:17:12.000000 toui-3.5.0a8/LICENSE
+-rw-rw-rw-   0        0        0       16 2024-05-10 13:17:12.000000 toui-3.5.0a8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5411 2024-05-21 17:23:29.509803 toui-3.5.0a8/PKG-INFO
+-rw-rw-rw-   0        0        0     4975 2024-05-10 13:17:12.000000 toui-3.5.0a8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 17:23:29.423196 toui-3.5.0a8/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     2119 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3663 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0     2806 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/advanced_example_5_toui_with_sql_user_database.py
+-rw-rw-rw-   0        0        0     7653 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/advanced_example_6_widgets.py
+-rw-rw-rw-   0        0        0      556 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2024-05-10 13:17:12.000000 toui-3.5.0a8/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:23:29.454524 toui-3.5.0a8/images/
+-rw-rw-rw-   0        0        0  2404280 2024-05-10 13:17:12.000000 toui-3.5.0a8/images/calculator.gif
+-rw-rw-rw-   0        0        0  2803703 2024-05-10 13:17:12.000000 toui-3.5.0a8/images/home.gif
+-rw-rw-rw-   0        0        0    27837 2024-05-10 13:17:12.000000 toui-3.5.0a8/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2024-05-10 13:17:12.000000 toui-3.5.0a8/images/logo.png
+-rw-rw-rw-   0        0        0       42 2024-05-21 17:23:29.511804 toui-3.5.0a8/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-05-12 06:41:41.000000 toui-3.5.0a8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:23:29.487745 toui-3.5.0a8/toui/
+-rw-rw-rw-   0        0        0      291 2024-05-21 17:21:23.000000 toui-3.5.0a8/toui/__init__.py
+-rw-rw-rw-   0        0        0      379 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/_helpers.py
+-rw-rw-rw-   0        0        0    12188 2024-05-20 21:00:47.000000 toui-3.5.0a8/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/_signals.py
+-rw-rw-rw-   0        0        0    64408 2024-05-12 11:50:40.000000 toui-3.5.0a8/toui/apps.py
+-rw-rw-rw-   0        0        0    27205 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/exceptions.py
+-rw-rw-rw-   0        0        0    22102 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2024-05-10 13:17:12.000000 toui-3.5.0a8/toui/structure.py
+drwxrwxrwx   0        0        0        0 2024-05-21 17:23:29.502738 toui-3.5.0a8/toui.egg-info/
+-rw-rw-rw-   0        0        0     5411 2024-05-21 17:23:29.000000 toui-3.5.0a8/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-21 17:23:29.000000 toui-3.5.0a8/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 17:23:29.000000 toui-3.5.0a8/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-21 17:23:29.000000 toui-3.5.0a8/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      253 2024-05-21 17:23:29.000000 toui-3.5.0a8/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-21 17:23:29.000000 toui-3.5.0a8/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 17:23:29.506802 toui-3.5.0a8/touicmd/
+-rw-rw-rw-   0        0        0       18 2024-05-10 13:53:34.000000 toui-3.5.0a8/touicmd/__init__.py
+-rw-rw-rw-   0        0        0     2617 2024-05-10 13:17:12.000000 toui-3.5.0a8/touicmd/_cmd.py
```

### Comparing `toui-3.5.0a7/LICENSE` & `toui-3.5.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/PKG-INFO` & `toui-3.5.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.5.0a7
+Version: 3.5.0a8
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-3.5.0a7/README.md` & `toui-3.5.0a8/README.md`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/advanced_example_1_toui_blueprint.py` & `toui-3.5.0a8/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/advanced_example_2_toui_with_javascript.py` & `toui-3.5.0a8/examples/advanced_example_2_toui_with_javascript.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/advanced_example_3_toui_with_google_sign_in.py` & `toui-3.5.0a8/examples/advanced_example_3_toui_with_google_sign_in.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/advanced_example_4_toui_with_firebase.py` & `toui-3.5.0a8/examples/advanced_example_4_toui_with_firebase.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/advanced_example_5_toui_with_sql_user_database.py` & `toui-3.5.0a8/examples/advanced_example_5_toui_with_sql_user_database.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/advanced_example_6_widgets.py` & `toui-3.5.0a8/examples/advanced_example_6_widgets.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/example_1_simple_website.py` & `toui-3.5.0a8/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/example_2_simple_desktop_app.py` & `toui-3.5.0a8/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/example_3_updating_page.py` & `toui-3.5.0a8/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/example_4_function_with_arg.py` & `toui-3.5.0a8/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/examples/example_5_user_variables.py` & `toui-3.5.0a8/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/images/calculator.gif` & `toui-3.5.0a8/images/calculator.gif`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/images/home.gif` & `toui-3.5.0a8/images/home.gif`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/images/icon.png` & `toui-3.5.0a8/images/icon.png`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/images/logo.png` & `toui-3.5.0a8/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/setup.py` & `toui-3.5.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/toui/_helpers.py` & `toui-3.5.0a8/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/toui/_javascript_templates.py` & `toui-3.5.0a8/toui/_javascript_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,28 +40,30 @@
                 url: urlPath,
                 "outputId": currentOutputId}
     _manageProperties()
     json['html'] = _getDoc()
     json['uid'] = await _getUid()
     var jsonstring = JSON.stringify(json)
     if (socket.readyState === 0) {
-        socket.onopen = async function() {
+        socket.addEventListener("open", async (event) => {
             socket.send(jsonstring);
-        }
+        })
     } else {
         socket.send(jsonstring)
     }
     var timeWaited = 0
     const timeLimit = 10000
     return new Promise(resolve => {
         function checkOutput() {
             if (currentOutputId in _pythonOutputs) {
                 const output = _pythonOutputs[currentOutputId]
+                delete _pythonOutputs[currentOutputId]
                 resolve(output);
             } else if (timeWaited >= timeLimit) {
+                delete _pythonOutputs[currentOutputId]
                 reject()
             } else {
                 window.setTimeout(checkOutput, 150); 
                 timeWaited = timeWaited + 150
             }
         }
         checkOutput();
```

### Comparing `toui-3.5.0a7/toui/_signals.py` & `toui-3.5.0a8/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/toui/apps.py` & `toui-3.5.0a8/toui/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1277,15 +1277,14 @@
                                 args[index] = new_page.get_element_from_selector(arg['selector'])
                 if "uid" in data_dict:
                     new_page._uid = data_dict['uid']
                 session['user page'] = new_page
                 try:
                     if new_page._func_exists(func):
                         output = new_page._call_func(func, *args)
-                        time.sleep(12)
                         ws.send(json.dumps({"python_output": output,"output_id": output_id}))
                     del session['user page']
                 except Exception as e:
                     del session['user page']
                     raise e
                 e = time.time()
                 debug(f"TIME: {e - s}s")
```

### Comparing `toui-3.5.0a7/toui/elements.py` & `toui-3.5.0a8/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/toui/pages.py` & `toui-3.5.0a8/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/toui/structure.py` & `toui-3.5.0a8/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/toui.egg-info/PKG-INFO` & `toui-3.5.0a8/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.5.0a7
+Version: 3.5.0a8
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-3.5.0a7/toui.egg-info/SOURCES.txt` & `toui-3.5.0a8/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a7/touicmd/_cmd.py` & `toui-3.5.0a8/touicmd/_cmd.py`

 * *Files identical despite different names*

