# Comparing `tmp/process_boss-0.0.1.tar.gz` & `tmp/process_boss-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process_boss-0.0.1.tar", last modified: Sun May 19 19:05:36 2024, max compression
+gzip compressed data, was "process_boss-0.0.2.tar", last modified: Tue May 21 10:13:08 2024, max compression
```

## Comparing `process_boss-0.0.1.tar` & `process_boss-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.048205 process_boss-0.0.1/
--rw-rw-rw-   0        0        0     1089 2024-05-19 18:17:43.000000 process_boss-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2219 2024-05-19 19:05:36.048205 process_boss-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2024-05-19 18:56:57.000000 process_boss-0.0.1/README.md
--rw-rw-rw-   0        0        0      740 2024-05-19 19:03:48.000000 process_boss-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 19:05:36.048205 process_boss-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.028098 process_boss-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.031099 process_boss-0.0.1/src/process-boss/
--rw-rw-rw-   0        0        0        0 2024-05-02 14:45:02.000000 process_boss-0.0.1/src/process-boss/__init__.py
--rw-rw-rw-   0        0        0      321 2024-05-19 18:41:31.000000 process_boss-0.0.1/src/process-boss/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.032098 process_boss-0.0.1/src/process-boss/domain/
--rw-rw-rw-   0        0        0     1968 2024-05-07 16:32:41.000000 process_boss-0.0.1/src/process-boss/domain/Config.py
--rw-rw-rw-   0        0        0     1225 2024-05-07 16:36:47.000000 process_boss-0.0.1/src/process-boss/domain/State.py
--rw-rw-rw-   0        0        0        0 2024-05-02 14:45:02.000000 process_boss-0.0.1/src/process-boss/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.033098 process_boss-0.0.1/src/process-boss/service/
--rw-rw-rw-   0        0        0     4087 2024-05-07 16:46:29.000000 process_boss-0.0.1/src/process-boss/service/ProcessScheduler.py
--rw-rw-rw-   0        0        0        0 2024-05-02 14:45:02.000000 process_boss-0.0.1/src/process-boss/service/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.039188 process_boss-0.0.1/src/process-boss/util/
--rw-rw-rw-   0        0        0      524 2024-05-07 16:30:26.000000 process_boss-0.0.1/src/process-boss/util/ConfigHandler.py
--rw-rw-rw-   0        0        0     1181 2024-05-02 16:00:45.000000 process_boss-0.0.1/src/process-boss/util/FileHandler.py
--rw-rw-rw-   0        0        0     1333 2024-05-02 14:41:22.000000 process_boss-0.0.1/src/process-boss/util/LogHandler.py
--rw-rw-rw-   0        0        0        0 2024-05-02 14:45:02.000000 process_boss-0.0.1/src/process-boss/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:05:36.048205 process_boss-0.0.1/src/process_boss.egg-info/
--rw-rw-rw-   0        0        0     2219 2024-05-19 19:05:36.000000 process_boss-0.0.1/src/process_boss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2024-05-19 19:05:36.000000 process_boss-0.0.1/src/process_boss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:05:36.000000 process_boss-0.0.1/src/process_boss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-19 19:05:36.000000 process_boss-0.0.1/src/process_boss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.900035 process_boss-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 10:12:59.000000 process_boss-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 10:13:08.900035 process_boss-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-21 10:12:59.000000 process_boss-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-21 10:12:59.000000 process_boss-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:13:08.900035 process_boss-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.896035 process_boss-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.896035 process_boss-0.0.2/src/process-boss/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.896035 process_boss-0.0.2/src/process-boss/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/domain/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/domain/State.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.896035 process_boss-0.0.2/src/process-boss/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/service/ProcessScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.900035 process_boss-0.0.2/src/process-boss/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/util/ConfigHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/util/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/util/LogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:12:59.000000 process_boss-0.0.2/src/process-boss/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:13:08.900035 process_boss-0.0.2/src/process_boss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 10:13:08.000000 process_boss-0.0.2/src/process_boss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-21 10:13:08.000000 process_boss-0.0.2/src/process_boss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:13:08.000000 process_boss-0.0.2/src/process_boss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:13:08.000000 process_boss-0.0.2/src/process_boss.egg-info/top_level.txt
```

### Comparing `process_boss-0.0.1/LICENSE` & `process_boss-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 kristof9851
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 kristof9851
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `process_boss-0.0.1/PKG-INFO` & `process_boss-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: process-boss
-Version: 0.0.1
-Summary: A python implementation of a cron job scheduler
-Author: kristof9851
-Project-URL: Homepage, https://github.com/kristof9851/process-boss
-Project-URL: Issues, https://github.com/kristof9851/process-boss/issues
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Process Scheduler
-
-A python implementation of a cron job scheduler.
-
-## 1. Install from source then activate venv
-
-Install `venv` to set up your virtual environment
-```bash
-pip install --upgrade pip setuptools wheel venv
-```
-
-Go to project root and create your virtual environment
-```bash
-cd <PROJECT_ROOT>
-python -m venv venv
-```
-
-Activate your virtual environment
-```bash
-.\venv\Scripts\activate
-```
-
-Install project dependencies
-```bash
-pip install -r requirements.txt
-```
-
-Install module locally, so you can import it as a module
-```bash
-pip install -e .
-```
-
-## 2. Run it
-
-First install from source (see above), then define your configuration in a YAML file
-```yaml
-loopRefreshSeconds: 15
-maxWorkers: 10
-schedulerLogDir: "C:\\Desktop\\apps\\process-scheduler\\logs\\scheduler"
-processLogDir: "C:\\Desktop\\apps\\process-scheduler\\logs\\process"
-processes:
-  - id: test-job
-    cron: "0 7 * * mon"                          # == 7:00 AM every Monday
-    command: "python C:\\Desktop\\my-process.py" # Invoke my python script
-    runAtStartup: true                           # Run immediately when scheduler starts, then follow cron definition
-```
-
-Run it
-```bash
-python -m process-scheduler C:\\Desktop\\config.yaml
-```
-
-## 3. Test
-
-TODO
-
-## 4. Build and upload
-
-Install dependencies
-
-```bash
-pip install --upgrade setuptools wheel build twine
-```
-
-Build the package (wheel and sdist)
-```bash
-python -m build 
-```
-
-Ensure `.pypirc` in user folder is correct, then upload
-```bash
-twine upload dist/*
-```
+Metadata-Version: 2.1
+Name: process-boss
+Version: 0.0.2
+Summary: A python implementation of a cron job scheduler
+Author: kristof9851
+Project-URL: Homepage, https://github.com/kristof9851/process-boss
+Project-URL: Issues, https://github.com/kristof9851/process-boss/issues
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Process Scheduler
+
+A python implementation of a cron job scheduler.
+
+## 1. Install from source then activate venv
+
+Install `venv` to set up your virtual environment
+```bash
+pip install --upgrade venv
+```
+
+Go to project root and create your virtual environment
+```bash
+cd <PROJECT_ROOT>
+python -m venv venv
+```
+
+Activate your virtual environment
+```bash
+.\venv\Scripts\activate
+```
+
+Install project dependencies
+```bash
+pip install -r requirements.txt
+```
+
+Install module locally, so you can import it as a module
+```bash
+pip install -e .
+```
+
+## 2. Run it
+
+First install from source (see above), then define your configuration in a YAML file
+```yaml
+loopRefreshSeconds: 15
+maxWorkers: 10
+schedulerLogDir: "C:\\Desktop\\apps\\process-boss\\logs\\scheduler"
+processLogDir: "C:\\Desktop\\apps\\process-boss\\logs\\process"
+processes:
+  - id: test-job
+    cron: "0 7 * * mon"                          # == 7:00 AM every Monday
+    command: "python C:\\Desktop\\my-process.py" # Invoke my python script
+    runAtStartup: true                           # Run immediately when scheduler starts, then follow cron definition
+```
+
+Run it
+```bash
+python -m process-boss C:\\Desktop\\config.yaml
+```
+
+## 3. Test
+
+TODO
+
+## 4. Build and upload
+
+Install dependencies
+
+```bash
+pip install --upgrade setuptools wheel build twine
+```
+
+Build the package (wheel and sdist)
+```bash
+python -m build 
+```
+
+Ensure `.pypirc` in user folder is correct, then upload
+```bash
+python -m twine upload dist/*
+```
```

### Comparing `process_boss-0.0.1/README.md` & `process_boss-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# Process Scheduler
-
-A python implementation of a cron job scheduler.
-
-## 1. Install from source then activate venv
-
-Install `venv` to set up your virtual environment
-```bash
-pip install --upgrade pip setuptools wheel venv
-```
-
-Go to project root and create your virtual environment
-```bash
-cd <PROJECT_ROOT>
-python -m venv venv
-```
-
-Activate your virtual environment
-```bash
-.\venv\Scripts\activate
-```
-
-Install project dependencies
-```bash
-pip install -r requirements.txt
-```
-
-Install module locally, so you can import it as a module
-```bash
-pip install -e .
-```
-
-## 2. Run it
-
-First install from source (see above), then define your configuration in a YAML file
-```yaml
-loopRefreshSeconds: 15
-maxWorkers: 10
-schedulerLogDir: "C:\\Desktop\\apps\\process-scheduler\\logs\\scheduler"
-processLogDir: "C:\\Desktop\\apps\\process-scheduler\\logs\\process"
-processes:
-  - id: test-job
-    cron: "0 7 * * mon"                          # == 7:00 AM every Monday
-    command: "python C:\\Desktop\\my-process.py" # Invoke my python script
-    runAtStartup: true                           # Run immediately when scheduler starts, then follow cron definition
-```
-
-Run it
-```bash
-python -m process-scheduler C:\\Desktop\\config.yaml
-```
-
-## 3. Test
-
-TODO
-
-## 4. Build and upload
-
-Install dependencies
-
-```bash
-pip install --upgrade setuptools wheel build twine
-```
-
-Build the package (wheel and sdist)
-```bash
-python -m build 
-```
-
-Ensure `.pypirc` in user folder is correct, then upload
-```bash
-twine upload dist/*
-```
+# Process Scheduler
+
+A python implementation of a cron job scheduler.
+
+## 1. Install from source then activate venv
+
+Install `venv` to set up your virtual environment
+```bash
+pip install --upgrade venv
+```
+
+Go to project root and create your virtual environment
+```bash
+cd <PROJECT_ROOT>
+python -m venv venv
+```
+
+Activate your virtual environment
+```bash
+.\venv\Scripts\activate
+```
+
+Install project dependencies
+```bash
+pip install -r requirements.txt
+```
+
+Install module locally, so you can import it as a module
+```bash
+pip install -e .
+```
+
+## 2. Run it
+
+First install from source (see above), then define your configuration in a YAML file
+```yaml
+loopRefreshSeconds: 15
+maxWorkers: 10
+schedulerLogDir: "C:\\Desktop\\apps\\process-boss\\logs\\scheduler"
+processLogDir: "C:\\Desktop\\apps\\process-boss\\logs\\process"
+processes:
+  - id: test-job
+    cron: "0 7 * * mon"                          # == 7:00 AM every Monday
+    command: "python C:\\Desktop\\my-process.py" # Invoke my python script
+    runAtStartup: true                           # Run immediately when scheduler starts, then follow cron definition
+```
+
+Run it
+```bash
+python -m process-boss C:\\Desktop\\config.yaml
+```
+
+## 3. Test
+
+TODO
+
+## 4. Build and upload
+
+Install dependencies
+
+```bash
+pip install --upgrade setuptools wheel build twine
+```
+
+Build the package (wheel and sdist)
+```bash
+python -m build 
+```
+
+Ensure `.pypirc` in user folder is correct, then upload
+```bash
+python -m twine upload dist/*
+```
```

### Comparing `process_boss-0.0.1/pyproject.toml` & `process_boss-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[build-system]
-requires = ["setuptools >= 61.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "process-boss"
-version = "0.0.1"
-description = "A python implementation of a cron job scheduler"
-authors = [ { name="kristof9851" } ]
-readme = "README.md"
-license = {file = "LICENSE.md"}
-classifiers=[
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Intended Audience :: Developers",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.10",
-    "License :: OSI Approved :: MIT License"
-]
-requires-python = ">=3.10"
-
-[project.urls]
-Homepage = "https://github.com/kristof9851/process-boss"
-Issues = "https://github.com/kristof9851/process-boss/issues"
+[build-system]
+requires = ["setuptools >= 61.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "process-boss"
+version = "0.0.2"
+description = "A python implementation of a cron job scheduler"
+authors = [ { name="kristof9851" } ]
+readme = "README.md"
+license = {file = "LICENSE.md"}
+classifiers=[
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Intended Audience :: Developers",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.10",
+    "License :: OSI Approved :: MIT License"
+]
+requires-python = ">=3.10"
+
+[project.urls]
+Homepage = "https://github.com/kristof9851/process-boss"
+Issues = "https://github.com/kristof9851/process-boss/issues"
```

### Comparing `process_boss-0.0.1/src/process-boss/service/ProcessScheduler.py` & `process_boss-0.0.2/src/process-boss/service/ProcessScheduler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import json
-import sys
-import time
-import os
-import pytz
-import logging
-from subprocess import Popen, PIPE, STDOUT
-from croniter import croniter
-from datetime import datetime
-from concurrent.futures import ThreadPoolExecutor
-
-from ..util.ConfigHandler import ConfigHandler 
-from ..util.LogHandler import LogHandler 
-from ..domain.State import State
-
-class ProcessScheduler:
-
-    def __init__(self, configPath):
-        logging.debug(f"configPath={configPath}")
-
-        self.configPath = configPath
-        self.startupDatetime = datetime.now(pytz.timezone('Europe/London'))
-        self.configHandler = ConfigHandler()
-        self.logHandler = LogHandler()
-        self.state = State()
-
-    def loop(self):
-        while(True):
-            logging.info("Starting new loop")
-            logging.debug(self.state)
-
-            config = self.configHandler.read(self.configPath)
-            self.runAll(config)
-            self.wait(config.loopRefreshSeconds)
-            
-    def runAll(self, config):
-        logging.debug(f"config={config}")
-
-        with ThreadPoolExecutor (max_workers=config.maxWorkers) as executor:
-            for processConfig in config.processesConfig.processList:
-                slog = self.logHandler.createSchedulerLogger (processConfig, config.schedulerLogDir) 
-                slog.info(f"[{processConfig.id}] processConfig={processConfig}")
-
-                processRegistered = self.state.get(processConfig.id) != False
-                processFinished = processRegistered and self.state.get(processConfig.id).future.done()
-                slog.debug(f"[{processConfig.id}] processRegistered={processRegistered}, processFinished={processFinished}")
-
-                if processRegistered:
-                    if not processFinished:
-                        slog.info(f"[{processConfig.id}] Process is still running. Skipping...")
-                        continue
-                    else:
-                        nextRunBaseDate = self.state.get(processConfig.id).startDatetime 
-                        slog.info(f"[{processConfig.id}] Process ran before: {nextRunBaseDate}")
-                else:
-                    nextRunBaseDate = self.startupDatetime
-                    slog.info(f"[{processConfig.id}] Process has not run before")
-
-                slog.debug(f"[{processConfig.id}] nextRunBaseDate={nextRunBaseDate}")
-
-                nextRunTimestamp = croniter (processConfig.cron, nextRunBaseDate).get_next() 
-                nowDatetime = datetime.now(pytz.timezone('Europe/London'))
-                nowTimestamp = nowDatetime.timestamp()
-                scheduledToRun = nextRunTimestamp < nowTimestamp
-                slog.debug(f"[{processConfig.id}] scheduledToRun={scheduledToRun}, processConfig.runAtStartup={processConfig.runAtStartup}")
-
-                if (scheduledToRun or (not processRegistered and processConfig.runAtStartup)):
-                    slog.info(f"[{processConfig.id}] Process is scheduled to run NOW: {datetime.fromtimestamp (nowTimestamp)}")
-                    self.state.set( processConfig, nowDatetime, executor.submit(self.run, processConfig, config.processLogDir, nowDatetime) )
-                else:
-                    slog.info(f"[{processConfig.id}] Process is scheduled to run on: {datetime.fromtimestamp (nextRunTimestamp)}")
-
-    def run(self, processConfig, processLogDir, nowDatetime):
-        plog = self.logHandler.createProcessLogger(processConfig, processLogDir, nowDatetime)
-        plog.debug(f"processConfig={processConfig}, processLogDir={processLogDir}, nowDatetime={nowDatetime}")
-
-        with Popen(
-            processConfig.command,
-            stdout=PIPE,
-            stderr=STDOUT
-        ) as p:
-            for line in iter (p.stdout.readline, b""):
-                plog.info(f"[{processConfig.id}] ... {line.decode(sys.stdout.encoding).rstrip()}")
-
-    def wait(self, loopRefreshSeconds):
-        logging.info(f"Waiting for: {loopRefreshSeconds} seconds")
-
-        time.sleep(loopRefreshSeconds)
+import json
+import sys
+import time
+import os
+import pytz
+import logging
+from subprocess import Popen, PIPE, STDOUT
+from croniter import croniter
+from datetime import datetime
+from concurrent.futures import ThreadPoolExecutor
+
+from ..util.ConfigHandler import ConfigHandler 
+from ..util.LogHandler import LogHandler 
+from ..domain.State import State
+
+class ProcessScheduler:
+
+    def __init__(self, configPath):
+        logging.debug(f"configPath={configPath}")
+
+        self.configPath = configPath
+        self.startupDatetime = datetime.now(pytz.timezone('Europe/London'))
+        self.configHandler = ConfigHandler()
+        self.logHandler = LogHandler()
+        self.state = State()
+
+    def loop(self):
+        while(True):
+            logging.info("Starting new loop")
+            logging.debug(self.state)
+
+            config = self.configHandler.read(self.configPath)
+            self.runAll(config)
+            self.wait(config.loopRefreshSeconds)
+            
+    def runAll(self, config):
+        logging.debug(f"config={config}")
+
+        with ThreadPoolExecutor (max_workers=config.maxWorkers) as executor:
+            for processConfig in config.processesConfig.processList:
+                slog = self.logHandler.createSchedulerLogger (processConfig, config.schedulerLogDir) 
+                slog.info(f"[{processConfig.id}] processConfig={processConfig}")
+
+                processRegistered = self.state.get(processConfig.id) != False
+                processFinished = processRegistered and self.state.get(processConfig.id).future.done()
+                slog.debug(f"[{processConfig.id}] processRegistered={processRegistered}, processFinished={processFinished}")
+
+                if processRegistered:
+                    if not processFinished:
+                        slog.info(f"[{processConfig.id}] Process is still running. Skipping...")
+                        continue
+                    else:
+                        nextRunBaseDate = self.state.get(processConfig.id).startDatetime 
+                        slog.info(f"[{processConfig.id}] Process ran before: {nextRunBaseDate}")
+                else:
+                    nextRunBaseDate = self.startupDatetime
+                    slog.info(f"[{processConfig.id}] Process has not run before")
+
+                slog.debug(f"[{processConfig.id}] nextRunBaseDate={nextRunBaseDate}")
+
+                nextRunTimestamp = croniter(processConfig.cron, nextRunBaseDate).get_next() 
+                nowDatetime = datetime.now(pytz.timezone('Europe/London'))
+                nowTimestamp = nowDatetime.timestamp()
+                scheduledToRun = nextRunTimestamp < nowTimestamp
+                slog.debug(f"[{processConfig.id}] scheduledToRun={scheduledToRun}, processConfig.runAtStartup={processConfig.runAtStartup}")
+
+                if (scheduledToRun or (not processRegistered and processConfig.runAtStartup)):
+                    slog.info(f"[{processConfig.id}] Process is scheduled to run NOW: {datetime.fromtimestamp (nowTimestamp)}")
+                    self.state.set( processConfig, nowDatetime, executor.submit(self.run, processConfig, config.processLogDir, nowDatetime) )
+                else:
+                    slog.info(f"[{processConfig.id}] Process is scheduled to run on: {datetime.fromtimestamp (nextRunTimestamp)}")
+
+    def run(self, processConfig, processLogDir, nowDatetime):
+        plog = self.logHandler.createProcessLogger(processConfig, processLogDir, nowDatetime)
+        plog.debug(f"processConfig={processConfig}, processLogDir={processLogDir}, nowDatetime={nowDatetime}")
+
+        with Popen(
+            processConfig.command,
+            stdout=PIPE,
+            stderr=STDOUT
+        ) as p:
+            for line in iter (p.stdout.readline, b""):
+                plog.info(f"[{processConfig.id}] ... {line.decode(sys.stdout.encoding).rstrip()}")
+
+    def wait(self, loopRefreshSeconds):
+        logging.info(f"Waiting for: {loopRefreshSeconds} seconds")
+
+        time.sleep(loopRefreshSeconds)
```

### Comparing `process_boss-0.0.1/src/process-boss/util/LogHandler.py` & `process_boss-0.0.2/src/process-boss/util/LogHandler.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import logging
-import os
-
-class LogHandler:
-    LEVEL = os.environ.get('LOGLEVEL', 'DEBUG').upper()
-    FORMAT = '%(asctime)s [%(levelname)5s] %(filename)s :: %(funcName)s() - %(message)s'
-
-    def createSchedulerLogger(self, processConfig, schedulerLogDir):
-        loggerName = f'{processConfig.id}_SCHEDULER'
-        fileName = f'{processConfig.id}.txt'
-        filePath = os.path.join(schedulerLogDir, fileName)
-        return self.createLogger(loggerName, filePath)
-
-    def createProcessLogger(self, processConfig, processLogDir, nowDatetime): 
-        loggerName = f'{processConfig.id}_PROCESS'
-        fileName = f'{nowDatetime.strftime("%Y%m%d-%H%M%S")}_{processConfig.id}.txt'
-        filePath = os.path.join(processLogDir, fileName)
-        return self.createLogger(loggerName, filePath)
-
-    def createLogger(self, name, filePath):
-        logger = logging.getLogger(name)
-        logger.setLevel(LogHandler.LEVEL)
-        fh = logging.FileHandler(filePath)
-        fh.setFormatter( logging.Formatter(LogHandler.FORMAT) )
-        if logger.hasHandlers():
-            for h in list (logger.handlers):
-                logger.removeHandler(h)
-        logger.addHandler(fh)
-
-        logging.debug(f'name={logger.name}, level={logger.level}, handlers={logger.handlers}')
-
-        return logger
+import logging
+import os
+
+class LogHandler:
+    LEVEL = os.environ.get('LOGLEVEL', 'DEBUG').upper()
+    FORMAT = '%(asctime)s [%(levelname)5s] %(filename)s :: %(funcName)s() - %(message)s'
+
+    def createSchedulerLogger(self, processConfig, schedulerLogDir):
+        loggerName = f'{processConfig.id}_SCHEDULER'
+        fileName = f'{processConfig.id}.txt'
+        filePath = os.path.join(schedulerLogDir, fileName)
+        return self.createLogger(loggerName, filePath)
+
+    def createProcessLogger(self, processConfig, processLogDir, nowDatetime): 
+        loggerName = f'{processConfig.id}_PROCESS'
+        fileName = f'{nowDatetime.strftime("%Y%m%d-%H%M%S")}_{processConfig.id}.txt'
+        filePath = os.path.join(processLogDir, fileName)
+        return self.createLogger(loggerName, filePath)
+
+    def createLogger(self, name, filePath):
+        logger = logging.getLogger(name)
+        logger.setLevel(LogHandler.LEVEL)
+        fh = logging.FileHandler(filePath)
+        fh.setFormatter( logging.Formatter(LogHandler.FORMAT) )
+        if logger.hasHandlers():
+            for h in list (logger.handlers):
+                logger.removeHandler(h)
+        logger.addHandler(fh)
+
+        logging.debug(f'name={logger.name}, level={logger.level}, handlers={logger.handlers}')
+
+        return logger
```

### Comparing `process_boss-0.0.1/src/process_boss.egg-info/PKG-INFO` & `process_boss-0.0.2/src/process_boss.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: process-boss
-Version: 0.0.1
-Summary: A python implementation of a cron job scheduler
-Author: kristof9851
-Project-URL: Homepage, https://github.com/kristof9851/process-boss
-Project-URL: Issues, https://github.com/kristof9851/process-boss/issues
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Process Scheduler
-
-A python implementation of a cron job scheduler.
-
-## 1. Install from source then activate venv
-
-Install `venv` to set up your virtual environment
-```bash
-pip install --upgrade pip setuptools wheel venv
-```
-
-Go to project root and create your virtual environment
-```bash
-cd <PROJECT_ROOT>
-python -m venv venv
-```
-
-Activate your virtual environment
-```bash
-.\venv\Scripts\activate
-```
-
-Install project dependencies
-```bash
-pip install -r requirements.txt
-```
-
-Install module locally, so you can import it as a module
-```bash
-pip install -e .
-```
-
-## 2. Run it
-
-First install from source (see above), then define your configuration in a YAML file
-```yaml
-loopRefreshSeconds: 15
-maxWorkers: 10
-schedulerLogDir: "C:\\Desktop\\apps\\process-scheduler\\logs\\scheduler"
-processLogDir: "C:\\Desktop\\apps\\process-scheduler\\logs\\process"
-processes:
-  - id: test-job
-    cron: "0 7 * * mon"                          # == 7:00 AM every Monday
-    command: "python C:\\Desktop\\my-process.py" # Invoke my python script
-    runAtStartup: true                           # Run immediately when scheduler starts, then follow cron definition
-```
-
-Run it
-```bash
-python -m process-scheduler C:\\Desktop\\config.yaml
-```
-
-## 3. Test
-
-TODO
-
-## 4. Build and upload
-
-Install dependencies
-
-```bash
-pip install --upgrade setuptools wheel build twine
-```
-
-Build the package (wheel and sdist)
-```bash
-python -m build 
-```
-
-Ensure `.pypirc` in user folder is correct, then upload
-```bash
-twine upload dist/*
-```
+Metadata-Version: 2.1
+Name: process-boss
+Version: 0.0.2
+Summary: A python implementation of a cron job scheduler
+Author: kristof9851
+Project-URL: Homepage, https://github.com/kristof9851/process-boss
+Project-URL: Issues, https://github.com/kristof9851/process-boss/issues
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Process Scheduler
+
+A python implementation of a cron job scheduler.
+
+## 1. Install from source then activate venv
+
+Install `venv` to set up your virtual environment
+```bash
+pip install --upgrade venv
+```
+
+Go to project root and create your virtual environment
+```bash
+cd <PROJECT_ROOT>
+python -m venv venv
+```
+
+Activate your virtual environment
+```bash
+.\venv\Scripts\activate
+```
+
+Install project dependencies
+```bash
+pip install -r requirements.txt
+```
+
+Install module locally, so you can import it as a module
+```bash
+pip install -e .
+```
+
+## 2. Run it
+
+First install from source (see above), then define your configuration in a YAML file
+```yaml
+loopRefreshSeconds: 15
+maxWorkers: 10
+schedulerLogDir: "C:\\Desktop\\apps\\process-boss\\logs\\scheduler"
+processLogDir: "C:\\Desktop\\apps\\process-boss\\logs\\process"
+processes:
+  - id: test-job
+    cron: "0 7 * * mon"                          # == 7:00 AM every Monday
+    command: "python C:\\Desktop\\my-process.py" # Invoke my python script
+    runAtStartup: true                           # Run immediately when scheduler starts, then follow cron definition
+```
+
+Run it
+```bash
+python -m process-boss C:\\Desktop\\config.yaml
+```
+
+## 3. Test
+
+TODO
+
+## 4. Build and upload
+
+Install dependencies
+
+```bash
+pip install --upgrade setuptools wheel build twine
+```
+
+Build the package (wheel and sdist)
+```bash
+python -m build 
+```
+
+Ensure `.pypirc` in user folder is correct, then upload
+```bash
+python -m twine upload dist/*
+```
```

### Comparing `process_boss-0.0.1/src/process_boss.egg-info/SOURCES.txt` & `process_boss-0.0.2/src/process_boss.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-src/process-boss/__init__.py
 src/process-boss/__main__.py
 src/process-boss/domain/Config.py
 src/process-boss/domain/State.py
 src/process-boss/domain/__init__.py
 src/process-boss/service/ProcessScheduler.py
 src/process-boss/service/__init__.py
 src/process-boss/util/ConfigHandler.py
```

