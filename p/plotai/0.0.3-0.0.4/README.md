# Comparing `tmp/plotai-0.0.3.tar.gz` & `tmp/plotai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotai-0.0.3.tar", last modified: Mon Mar 18 07:09:52 2024, max compression
+gzip compressed data, was "plotai-0.0.4.tar", last modified: Tue May 21 06:55:19 2024, max compression
```

## Comparing `plotai-0.0.3.tar` & `plotai-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-18 07:09:52.380556 plotai-0.0.3/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11357 2023-08-23 12:51:16.000000 plotai-0.0.3/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2023-08-25 11:55:20.000000 plotai-0.0.3/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6639 2024-03-18 07:09:52.380556 plotai-0.0.3/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4893 2024-03-18 07:09:26.000000 plotai-0.0.3/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-18 07:09:52.376556 plotai-0.0.3/plotai/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       27 2023-08-23 13:30:24.000000 plotai-0.0.3/plotai/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-18 07:09:52.380556 plotai-0.0.3/plotai/code/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-08-24 06:39:30.000000 plotai-0.0.3/plotai/code/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      417 2023-08-24 11:40:05.000000 plotai-0.0.3/plotai/code/executor.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      991 2023-08-24 13:52:56.000000 plotai-0.0.3/plotai/code/logger.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-18 07:09:52.380556 plotai-0.0.3/plotai/llm/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-08-23 13:17:40.000000 plotai-0.0.3/plotai/llm/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1334 2024-03-18 07:09:26.000000 plotai-0.0.3/plotai/llm/openai.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2219 2024-03-18 07:09:26.000000 plotai-0.0.3/plotai/plotai.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-18 07:09:52.380556 plotai-0.0.3/plotai/prompt/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-08-23 13:20:56.000000 plotai-0.0.3/plotai/prompt/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1236 2023-08-24 14:26:38.000000 plotai-0.0.3/plotai/prompt/prompt.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-03-18 07:09:52.376556 plotai-0.0.3/plotai.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6639 2024-03-18 07:09:52.000000 plotai-0.0.3/plotai.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      425 2024-03-18 07:09:52.000000 plotai-0.0.3/plotai.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-03-18 07:09:52.000000 plotai-0.0.3/plotai.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       82 2024-03-18 07:09:52.000000 plotai-0.0.3/plotai.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        7 2024-03-18 07:09:52.000000 plotai-0.0.3/plotai.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       12 2023-08-23 13:30:13.000000 plotai-0.0.3/requirements-dev.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       82 2024-03-18 07:09:26.000000 plotai-0.0.3/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-03-18 07:09:52.380556 plotai-0.0.3/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1276 2024-03-18 07:09:26.000000 plotai-0.0.3/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-21 06:55:19.590058 plotai-0.0.4/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11357 2023-08-23 12:51:16.000000 plotai-0.0.4/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2023-08-25 11:55:20.000000 plotai-0.0.4/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6639 2024-05-21 06:55:19.590058 plotai-0.0.4/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4893 2024-03-18 07:09:26.000000 plotai-0.0.4/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-21 06:55:19.590058 plotai-0.0.4/plotai/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       27 2023-08-23 13:30:24.000000 plotai-0.0.4/plotai/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-21 06:55:19.590058 plotai-0.0.4/plotai/code/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-08-24 06:39:30.000000 plotai-0.0.4/plotai/code/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      417 2023-08-24 11:40:05.000000 plotai-0.0.4/plotai/code/executor.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      991 2023-08-24 13:52:56.000000 plotai-0.0.4/plotai/code/logger.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-21 06:55:19.590058 plotai-0.0.4/plotai/llm/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-08-23 13:17:40.000000 plotai-0.0.4/plotai/llm/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1334 2024-03-18 07:09:26.000000 plotai-0.0.4/plotai/llm/openai.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1827 2024-05-21 06:53:43.000000 plotai-0.0.4/plotai/plotai.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-21 06:55:19.590058 plotai-0.0.4/plotai/prompt/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-08-23 13:20:56.000000 plotai-0.0.4/plotai/prompt/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1236 2023-08-24 14:26:38.000000 plotai-0.0.4/plotai/prompt/prompt.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-21 06:55:19.590058 plotai-0.0.4/plotai.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6639 2024-05-21 06:55:19.000000 plotai-0.0.4/plotai.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      425 2024-05-21 06:55:19.000000 plotai-0.0.4/plotai.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-05-21 06:55:19.000000 plotai-0.0.4/plotai.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       45 2024-05-21 06:55:19.000000 plotai-0.0.4/plotai.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        7 2024-05-21 06:55:19.000000 plotai-0.0.4/plotai.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       12 2023-08-23 13:30:13.000000 plotai-0.0.4/requirements-dev.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       45 2024-05-21 06:47:01.000000 plotai-0.0.4/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-05-21 06:55:19.590058 plotai-0.0.4/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1276 2024-05-21 06:54:48.000000 plotai-0.0.4/setup.py
```

### Comparing `plotai-0.0.3/LICENSE` & `plotai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plotai-0.0.3/PKG-INFO` & `plotai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create plots in Python with AI
 Home-page: https://github.com/mljar/plotai
 Author: MLJAR Sp. z o.o.
 Author-email: contact@mljar.com
 License: Apache 2.0
 Description: 
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plotai Version: 0.0.3 Summary: Create plots in
+Metadata-Version: 2.1 Name: plotai Version: 0.0.4 Summary: Create plots in
 Python with AI Home-page: https://github.com/mljar/plotai Author: MLJAR Sp. z
 o.o. Author-email: contact@mljar.com License: Apache 2.0 Description:
                                  [PlotAI logo]
          ?ð???¨?ð??¤? CCrreeaattee PPyytthhoonn pplloottss iinn mmaattpplloottlliibb wwiitthh LLLLMM ?ð???¨?ð??¤?
  _ð____ _G_e_t_ _S_t_a_r_t_e_d   â¢   _ð__¤__ _I_s_s_u_e_s   â¢   _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___©_â___ð___¼
                                    _L_i_n_k_e_d_I_n
 # PlotAI ð¨ð¤ The easiest way to create plots in Python and Matplotlib. The
```

### Comparing `plotai-0.0.3/README.md` & `plotai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `plotai-0.0.3/plotai/code/logger.py` & `plotai-0.0.4/plotai/code/logger.py`

 * *Files identical despite different names*

### Comparing `plotai-0.0.3/plotai/llm/openai.py` & `plotai-0.0.4/plotai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `plotai-0.0.3/plotai/plotai.py` & `plotai-0.0.4/plotai/plotai.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,54 +4,40 @@
 from plotai.llm.openai import ChatGPT
 from plotai.code.executor import Executor
 from plotai.code.logger import Logger
 
 
 class PlotAI:
 
-    def __init__(self, model_version: str = "gpt-3.5-turbo", *args, **kwargs):
-
-        # OpenAI Model Version
-        self.model_version = model_version
+    def __init__(self, *args, **kwargs):
+        self.model_version = "gpt-3.5-turbo"
         # DataFrame to plot
         self.df, self.x, self.y, self.z = None, None, None, None
-        if len(args) > 1:
-            for i in range(len(args)):
-                if isinstance(args[i], pd.DataFrame):
-                    raise Exception("You can pass only one DataFrame")
-
-        if len(args) == 1:
-            if isinstance(args[0], pd.DataFrame):
-                self.df = args[0]
-            else:
-                self.x = args[0]
-        elif len(args) == 2:
-            self.x = args[0]
-            self.y = args[1]
-        elif len(args) == 3:
-            self.x = args[0]
-            self.y = args[1]
-            self.z = args[2]
-
-        for k in kwargs:
-            for expected_k in ["x", "y", "z", "df"]:
-                if k == expected_k:
-                    setattr(self, k, kwargs[k])
+        
+        for expected_k in ["x", "y", "z", "df", "model_version"]:
+            if expected_k in kwargs:
+                setattr(self, expected_k, kwargs[expected_k])
+        
+        if self.df is None:
+            for arg in args:
+                if isinstance(arg, pd.DataFrame):
+                    self.df = arg
+                    break
 
     def make(self, prompt):
         p = Prompt(prompt, self.df, self.x, self.y, self.z)
 
         Logger().log({"title": "Prompt", "details": p.value})
 
         response = ChatGPT(model=self.model_version).chat(p.value)
 
         Logger().log({"title": "Response", "details": response})
 
         executor = Executor()
-        error = executor.run(response, globals(), locals())
+        error = executor.run(response, globals(), {"df":self.df, "x": self.x, "y": self.y, "z": self.z})
         if error is not None:
             Logger().log({"title": "Error in code execution", "details": error})
 
             # p_again = Prompt(prompt, self.df, self.x, self.y, self.z, previous_code=response, previous_error=error)
 
             # Logger().log({"title": "Prompt with fix", "details": p_again.value})
```

### Comparing `plotai-0.0.3/plotai/prompt/prompt.py` & `plotai-0.0.4/plotai/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `plotai-0.0.3/plotai.egg-info/PKG-INFO` & `plotai-0.0.4/plotai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create plots in Python with AI
 Home-page: https://github.com/mljar/plotai
 Author: MLJAR Sp. z o.o.
 Author-email: contact@mljar.com
 License: Apache 2.0
 Description: 
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plotai Version: 0.0.3 Summary: Create plots in
+Metadata-Version: 2.1 Name: plotai Version: 0.0.4 Summary: Create plots in
 Python with AI Home-page: https://github.com/mljar/plotai Author: MLJAR Sp. z
 o.o. Author-email: contact@mljar.com License: Apache 2.0 Description:
                                  [PlotAI logo]
          ?ð???¨?ð??¤? CCrreeaattee PPyytthhoonn pplloottss iinn mmaattpplloottlliibb wwiitthh LLLLMM ?ð???¨?ð??¤?
  _ð____ _G_e_t_ _S_t_a_r_t_e_d   â¢   _ð__¤__ _I_s_s_u_e_s   â¢   _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___©_â___ð___¼
                                    _L_i_n_k_e_d_I_n
 # PlotAI ð¨ð¤ The easiest way to create plots in Python and Matplotlib. The
```

### Comparing `plotai-0.0.3/setup.py` & `plotai-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="plotai",
-    version="0.0.3",
+    version="0.0.4",
     description="Create plots in Python with AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mljar/plotai",
     author="MLJAR Sp. z o.o.",
     author_email="contact@mljar.com",
     license="Apache 2.0",
```

