# Comparing `tmp/empower_functions-0.1.2.tar.gz` & `tmp/empower_functions-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empower_functions-0.1.2.tar", last modified: Sat May 18 00:32:45 2024, max compression
+gzip compressed data, was "empower_functions-0.1.3.tar", last modified: Tue May 21 03:50:07 2024, max compression
```

## Comparing `empower_functions-0.1.2.tar` & `empower_functions-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-18 00:32:45.078652 empower_functions-0.1.2/
--rw-r--r--   0 yulong     (501) staff       (20)      763 2024-05-18 00:32:45.078534 empower_functions-0.1.2/PKG-INFO
--rw-r--r--   0 yulong     (501) staff       (20)    12579 2024-05-17 17:17:35.000000 empower_functions-0.1.2/README.md
-drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-18 00:32:45.077501 empower_functions-0.1.2/empower_functions/
--rw-r--r--   0 yulong     (501) staff       (20)      277 2024-05-17 20:27:57.000000 empower_functions-0.1.2/empower_functions/README.md
--rw-r--r--   0 yulong     (501) staff       (20)      173 2024-05-16 16:18:45.000000 empower_functions-0.1.2/empower_functions/__init__.py
--rw-r--r--   0 yulong     (501) staff       (20)    11879 2024-05-17 17:47:18.000000 empower_functions-0.1.2/empower_functions/chat_handler.py
--rw-r--r--   0 yulong     (501) staff       (20)     7058 2024-05-18 00:31:56.000000 empower_functions-0.1.2/empower_functions/prompt.py
--rw-r--r--   0 yulong     (501) staff       (20)     9171 2024-05-16 19:45:02.000000 empower_functions-0.1.2/empower_functions/server.py
-drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-18 00:32:45.078352 empower_functions-0.1.2/empower_functions.egg-info/
--rw-r--r--   0 yulong     (501) staff       (20)      763 2024-05-18 00:32:45.000000 empower_functions-0.1.2/empower_functions.egg-info/PKG-INFO
--rw-r--r--   0 yulong     (501) staff       (20)      387 2024-05-18 00:32:45.000000 empower_functions-0.1.2/empower_functions.egg-info/SOURCES.txt
--rw-r--r--   0 yulong     (501) staff       (20)        1 2024-05-18 00:32:45.000000 empower_functions-0.1.2/empower_functions.egg-info/dependency_links.txt
--rw-r--r--   0 yulong     (501) staff       (20)       41 2024-05-18 00:32:45.000000 empower_functions-0.1.2/empower_functions.egg-info/requires.txt
--rw-r--r--   0 yulong     (501) staff       (20)       18 2024-05-18 00:32:45.000000 empower_functions-0.1.2/empower_functions.egg-info/top_level.txt
--rw-r--r--   0 yulong     (501) staff       (20)      685 2024-05-18 00:32:26.000000 empower_functions-0.1.2/pyproject.toml
--rw-r--r--   0 yulong     (501) staff       (20)       38 2024-05-18 00:32:45.078706 empower_functions-0.1.2/setup.cfg
--rw-r--r--   0 yulong     (501) staff       (20)      629 2024-05-18 00:32:30.000000 empower_functions-0.1.2/setup.py
+drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-21 03:50:07.093479 empower_functions-0.1.3/
+-rw-r--r--   0 yulong     (501) staff       (20)      849 2024-05-21 03:50:07.093264 empower_functions-0.1.3/PKG-INFO
+-rw-r--r--   0 yulong     (501) staff       (20)    13239 2024-05-21 03:49:14.000000 empower_functions-0.1.3/README.md
+drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-21 03:50:07.092294 empower_functions-0.1.3/empower_functions/
+-rw-r--r--   0 yulong     (501) staff       (20)      277 2024-05-17 20:27:57.000000 empower_functions-0.1.3/empower_functions/README.md
+-rw-r--r--   0 yulong     (501) staff       (20)      173 2024-05-16 16:18:45.000000 empower_functions-0.1.3/empower_functions/__init__.py
+-rw-r--r--   0 yulong     (501) staff       (20)    11879 2024-05-17 17:47:18.000000 empower_functions-0.1.3/empower_functions/chat_handler.py
+-rw-r--r--   0 yulong     (501) staff       (20)     7070 2024-05-21 03:49:14.000000 empower_functions-0.1.3/empower_functions/prompt.py
+-rw-r--r--   0 yulong     (501) staff       (20)     9171 2024-05-16 19:45:02.000000 empower_functions-0.1.3/empower_functions/server.py
+drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-21 03:50:07.093013 empower_functions-0.1.3/empower_functions.egg-info/
+-rw-r--r--   0 yulong     (501) staff       (20)      849 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/PKG-INFO
+-rw-r--r--   0 yulong     (501) staff       (20)      387 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 yulong     (501) staff       (20)        1 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 yulong     (501) staff       (20)       41 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/requires.txt
+-rw-r--r--   0 yulong     (501) staff       (20)       18 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/top_level.txt
+-rw-r--r--   0 yulong     (501) staff       (20)      686 2024-05-21 03:49:42.000000 empower_functions-0.1.3/pyproject.toml
+-rw-r--r--   0 yulong     (501) staff       (20)       38 2024-05-21 03:50:07.093533 empower_functions-0.1.3/setup.cfg
+-rw-r--r--   0 yulong     (501) staff       (20)      629 2024-05-21 03:49:35.000000 empower_functions-0.1.3/setup.py
```

### Comparing `empower_functions-0.1.2/PKG-INFO` & `empower_functions-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: empower_functions
-Version: 0.1.2
+Version: 0.1.3
 Summary: The empower_functions package provides a set of utility functions to run the empower-functions model
 Author-email: "empower.dev" <yulong@empower.dev>
 Project-URL: Homepage, https://empower.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: jinja2
+Requires-Dist: llama-cpp-python[server]
+Requires-Dist: pydantic
 
 ## Project Description
 
 This is the pip package for the empower-functions LLMs which offer GPT-4 level capatiblities for real-world "tool-using" use cases.
 
 For more information, please visit the [Empower Functions](https://github.com/empower-ai/empower-functions) Github repo.
```

### Comparing `empower_functions-0.1.2/README.md` & `empower_functions-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 Real-world use cases, particularly those involving conversational agents, often introduce complex requirements for LLMs. Models must be capable of retrieving context from multiple round of conversations([multi-turn](docs/inference/multi-turn.md)), choosing between utilizing tools or engaging in standard dialogue (['auto' mode](docs/inference/introduction.md#tools-parameter)), and asking for clarification if any parameters are missing([clarification](docs/inference/clarification.md)). Furthermore, they should integrate responses with tool outputs in a [streaming](docs/inference/streaming.md) fashion. Additionally, when multiple tools are required to complete a task, models should efficiently execute multiple functions either in parallel ([parallel calling](docs/inference/parallel-calling.md)) or sequentially with dependencies ([sequential calling](docs/inference/sequential-calling.md)).
 
 For example, below is a screenshot demonstrating how the model is used in a medical center coordinator bot. You can explore this further in our [live demo](https://app.empower.dev/chat-demo).
 ![image](assets/demo_screenshot.png)
 
 ## Family of Models
 
-| Model                    | Specs                                                                                             | Links                  |                                     |
-| ------------------------ | ------------------------------------------------------------------------------------------------- | ---------------------- | ----------------------------------- |
-| empower-functions-small  | 8k context, based on [Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B)               | model, GGUF, GGUF 4bit | most cost effective, local runnable |
-| empower-functions-medium | 32k context, based on [Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) | model                  | balance in accuracy and cost        |
-| empower-functions-large  | 65k context, based on [Mixtral 8x22B](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1)        | model                  | best accuracy                       |
+| Model                    | Specs                                                                                             | Links                                                                                                                                                      |                                     |
+| ------------------------ | ------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
+| empower-functions-small  | 8k context, based on [Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B)               | [model](https://huggingface.co/empower-dev/llama3-empower-functions-small), [GGUF](https://huggingface.co/empower-dev/llama3-empower-functions-small-gguf) | most cost effective, local runnable |
+| empower-functions-medium | 32k context, based on [Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) | [model](https://huggingface.co/empower-dev/empower-functions-medium)                                                                                       | balance in accuracy and cost        |
+| empower-functions-large  | 65k context, based on [Mixtral 8x22B](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1)        | model                                                                                                                                                      | best accuracy                       |
 
 #### Hardware Requirement
 
 We have tested and the family of models in following setup:
 
 - empower-functions-small: fp16 on 1xA100 40G, GGUF and 4bit GGUF on Macbook M2 Pro with 32G RAM, in minimal the 4bit GGUF version requires 7.56G RAM.
 - empower-functions-medium: fp16 on 2xA100 80G
```

#### html2text {}

```diff
@@ -24,33 +24,37 @@
 inference/parallel-calling.md)) or sequentially with dependencies ([sequential
 calling](docs/inference/sequential-calling.md)). For example, below is a
 screenshot demonstrating how the model is used in a medical center coordinator
 bot. You can explore this further in our [live demo](https://app.empower.dev/
 chat-demo). ![image](assets/demo_screenshot.png) ## Family of Models | Model |
 Specs | Links | | | ------------------------ | --------------------------------
 ----------------------------------------------------------------- | -----------
------------ | ----------------------------------- | | empower-functions-small |
-8k context, based on [Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-
-3-8B) | model, GGUF, GGUF 4bit | most cost effective, local runnable | |
-empower-functions-medium | 32k context, based on [Mixtral 8x7B](https://
-huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) | model | balance in
-accuracy and cost | | empower-functions-large | 65k context, based on [Mixtral
-8x22B](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1) | model | best
-accuracy | #### Hardware Requirement We have tested and the family of models in
-following setup: - empower-functions-small: fp16 on 1xA100 40G, GGUF and 4bit
-GGUF on Macbook M2 Pro with 32G RAM, in minimal the 4bit GGUF version requires
-7.56G RAM. - empower-functions-medium: fp16 on 2xA100 80G - empower-functions-
-large: fp16 on 4xA100 80G ## How to Use? #### Running Locally > Running locally
-is only supported by empower-functions-small model. To use other models, please
-use our API. Local running is supported through the `empower_functions` pip
-package, make sure you install it first by running `pip install empower-
-functions`. > If you run into errors like RuntimeError: Failed to load shared
-library, (mach-o file, but is an incompatible architecture (have 'x86_64', need
-'arm64')), please re-install the llama-cpp-python package by running
-`CMAKE_ARGS="-DCMAKE_OSX_ARCHITECTURES=arm64 -
+-------------------------------------------------------------------------------
+---------------------------------------------------------------- | ------------
+----------------------- | | empower-functions-small | 8k context, based on
+[Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B) | [model](https:
+//huggingface.co/empower-dev/llama3-empower-functions-small), [GGUF](https://
+huggingface.co/empower-dev/llama3-empower-functions-small-gguf) | most cost
+effective, local runnable | | empower-functions-medium | 32k context, based on
+[Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) |
+[model](https://huggingface.co/empower-dev/empower-functions-medium) | balance
+in accuracy and cost | | empower-functions-large | 65k context, based on
+[Mixtral 8x22B](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1) | model |
+best accuracy | #### Hardware Requirement We have tested and the family of
+models in following setup: - empower-functions-small: fp16 on 1xA100 40G, GGUF
+and 4bit GGUF on Macbook M2 Pro with 32G RAM, in minimal the 4bit GGUF version
+requires 7.56G RAM. - empower-functions-medium: fp16 on 2xA100 80G - empower-
+functions-large: fp16 on 4xA100 80G ## How to Use? #### Running Locally >
+Running locally is only supported by empower-functions-small model. To use
+other models, please use our API. Local running is supported through the
+`empower_functions` pip package, make sure you install it first by running `pip
+install empower-functions`. > If you run into errors like RuntimeError: Failed
+to load shared library, (mach-o file, but is an incompatible architecture (have
+'x86_64', need 'arm64')), please re-install the llama-cpp-python package by
+running `CMAKE_ARGS="-DCMAKE_OSX_ARCHITECTURES=arm64 -
 DCMAKE_APPLE_SILICON_PROCESSOR=arm64 -DLLAMA_METAL=on" pip install --upgrade --
 verbose --force-reinstall --no-cache-dir llama-cpp-python` Using a Local OpenAI
 Compatible Server We leverage the `llama-cpp-python` project to run the model
 locally. To start a local OpenAI compatible server, you'll need to follow the
 steps below: 1. Download the GGUF model from our [huggingface repo](TODO) 2.
 Run the command `python -m empower_functions.server --model --chat_format
 empower-functions` You should see the following output when the server is
```

### Comparing `empower_functions-0.1.2/empower_functions/chat_handler.py` & `empower_functions-0.1.3/empower_functions/chat_handler.py`

 * *Files identical despite different names*

### Comparing `empower_functions-0.1.2/empower_functions/prompt.py` & `empower_functions-0.1.3/empower_functions/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,18 +141,18 @@
 
     if len(functions_def) == 0:
         prompted_messages = [first_user_message]
     else:
         prompted_messages = [{'role': 'user', 'content': (
             system_instruction
             + "\n"
-            + "Functions: "
+            + "Functions:\n"
             + json.dumps(functions_def, indent=2, ensure_ascii=False)
             + "\n\n"
-            + " <u>"
+            + "User Message:\n"
             + first_user_message['content']
         )}]
 
     for message in messages[starting_index:]:
         if message['role'] == 'tool':
             prompted_messages.append({
                 'role': 'user',
```

### Comparing `empower_functions-0.1.2/empower_functions/server.py` & `empower_functions-0.1.3/empower_functions/server.py`

 * *Files identical despite different names*

### Comparing `empower_functions-0.1.2/empower_functions.egg-info/PKG-INFO` & `empower_functions-0.1.3/empower_functions.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
-Name: empower-functions
-Version: 0.1.2
+Name: empower_functions
+Version: 0.1.3
 Summary: The empower_functions package provides a set of utility functions to run the empower-functions model
 Author-email: "empower.dev" <yulong@empower.dev>
 Project-URL: Homepage, https://empower.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: jinja2
+Requires-Dist: llama-cpp-python[server]
+Requires-Dist: pydantic
 
 ## Project Description
 
 This is the pip package for the empower-functions LLMs which offer GPT-4 level capatiblities for real-world "tool-using" use cases.
 
 For more information, please visit the [Empower Functions](https://github.com/empower-ai/empower-functions) Github repo.
```

### Comparing `empower_functions-0.1.2/pyproject.toml` & `empower_functions-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "empower_functions"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="empower.dev", email="yulong@empower.dev" }
 ]
 description = "The empower_functions package provides a set of utility functions to run the empower-functions model"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -19,8 +19,8 @@
 readme = "./empower_functions/README.md"
 
 [project.urls]
 Homepage = "https://empower.dev"
 
 [build-system]
 requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `empower_functions-0.1.2/setup.py` & `empower_functions-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "empower_functions/README.md").read_text()
 
 setup(
     name='empower_functions',  # This is the package name
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),  # This will find the `empower_functions` directory
     install_requires=[
         "jinja2",
         "llama-cpp-python[server]",
         "pydantic"
         # Add your dependencies here
     ],
```

