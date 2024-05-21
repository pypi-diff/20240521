# Comparing `tmp/infolab_common_lib-1.0.3.tar.gz` & `tmp/infolab_common_lib-1.0.4.tar.gz`

## Comparing `infolab_common_lib-1.0.3.tar` & `infolab_common_lib-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/common_lib/__init__.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/common_lib/http_client.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/common_lib/__init__.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/common_lib/http_client.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/LICENSE
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/README.md
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.4/PKG-INFO
```

### Comparing `infolab_common_lib-1.0.3/common_lib/http_client.py` & `infolab_common_lib-1.0.4/common_lib/http_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,18 @@
             return {}
 
         proxy = random.choice(self.proxies)
         return {"http": proxy, "https": proxy}
 
     def get(self, url, **kwargs):
         return self.get_client().get(
-            url, proxies=self.get_proxies(url), timeout=self.timeout, **kwargs
+            url,
+            proxies=self.get_proxies(url),
+            timeout=self.timeout,
+            **kwargs
         )
 
     def post(self, url, data=None, json=None, **kwargs):
         return self.get_client().post(
             url,
             data=data,
             json=json,
```

### Comparing `infolab_common_lib-1.0.3/.gitignore` & `infolab_common_lib-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `infolab_common_lib-1.0.3/LICENSE` & `infolab_common_lib-1.0.4/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2024 Infolab Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `infolab_common_lib-1.0.3/PKG-INFO` & `infolab_common_lib-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: infolab-common-lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Infolab Common Lib
 Project-URL: Homepage, https://zalogit2.zing.vn/infolab/infolab-common-lib
-Project-URL: Bug Tracker, https://zalogit2.zing.vn/infolab/infolab-common-lib/-/issues
+Project-URL: BugTracker, https://zalogit2.zing.vn/infolab/infolab-common-lib/-/issues
 Author-email: anhnd15 <anhnd15@vng.com.vn>
-License: Copyright (c) 2018 The Python Packaging Authority
+License: Copyright (c) 2024 Infolab Team
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -26,7 +26,24 @@
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: requests>=2.27.1
+Description-Content-Type: text/markdown
+
+# infolab-common-lib
+
+## Description
+The `infolab-common-lib` provides common functionalities for projects within the Infolab team.
+
+## Requirements
+
+- Python >= 3.8
+
+## Installation
+
+To install the library, you can use pip. Run the following command in your terminal:
+
+```bash
+pip install infolab-common-lib
```

