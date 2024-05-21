# Comparing `tmp/mircheck-0.1.0.tar.gz` & `tmp/mircheck-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mircheck-0.1.0.tar", last modified: Tue May 21 19:40:11 2024, max compression
+gzip compressed data, was "mircheck-0.1.1.tar", last modified: Tue May 21 20:00:42 2024, max compression
```

## Comparing `mircheck-0.1.0.tar` & `mircheck-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:40:11.914208 mircheck-0.1.0/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     1071 2024-05-21 19:27:54.000000 mircheck-0.1.0/LICENSE
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2851 2024-05-21 19:40:11.914208 mircheck-0.1.0/PKG-INFO
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2388 2024-05-21 19:27:54.000000 mircheck-0.1.0/README.md
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:40:11.914208 mircheck-0.1.0/mircheck/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:27:54.000000 mircheck-0.1.0/mircheck/__init__.py
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     5056 2024-05-21 19:27:54.000000 mircheck-0.1.0/mircheck/main.py
-drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:40:11.914208 mircheck-0.1.0/mircheck.egg-info/
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2851 2024-05-21 19:40:11.000000 mircheck-0.1.0/mircheck.egg-info/PKG-INFO
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      258 2024-05-21 19:40:11.000000 mircheck-0.1.0/mircheck.egg-info/SOURCES.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        1 2024-05-21 19:40:11.000000 mircheck-0.1.0/mircheck.egg-info/dependency_links.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       48 2024-05-21 19:40:11.000000 mircheck-0.1.0/mircheck.egg-info/entry_points.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 19:40:11.000000 mircheck-0.1.0/mircheck.egg-info/requires.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 19:40:11.000000 mircheck-0.1.0/mircheck.egg-info/top_level.txt
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       38 2024-05-21 19:40:11.914208 mircheck-0.1.0/setup.cfg
--rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      842 2024-05-21 19:27:54.000000 mircheck-0.1.0/setup.py
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:00:42.451156 mircheck-0.1.1/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     1071 2024-05-21 19:27:54.000000 mircheck-0.1.1/LICENSE
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2882 2024-05-21 20:00:42.451156 mircheck-0.1.1/PKG-INFO
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2418 2024-05-21 19:50:01.000000 mircheck-0.1.1/README.md
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:00:42.451156 mircheck-0.1.1/mircheck/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 19:27:54.000000 mircheck-0.1.1/mircheck/__init__.py
+-rwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)     5056 2024-05-21 19:27:54.000000 mircheck-0.1.1/mircheck/mircheck.py
+drwxrwxr-x   0 kimbozy   (1000) kimbozy   (1000)        0 2024-05-21 20:00:42.451156 mircheck-0.1.1/mircheck.egg-info/
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)     2882 2024-05-21 20:00:42.000000 mircheck-0.1.1/mircheck.egg-info/PKG-INFO
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      262 2024-05-21 20:00:42.000000 mircheck-0.1.1/mircheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        1 2024-05-21 20:00:42.000000 mircheck-0.1.1/mircheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       43 2024-05-21 20:00:42.000000 mircheck-0.1.1/mircheck.egg-info/entry_points.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       14 2024-05-21 20:00:42.000000 mircheck-0.1.1/mircheck.egg-info/requires.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)        9 2024-05-21 20:00:42.000000 mircheck-0.1.1/mircheck.egg-info/top_level.txt
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)       38 2024-05-21 20:00:42.451156 mircheck-0.1.1/setup.cfg
+-rw-rw-r--   0 kimbozy   (1000) kimbozy   (1000)      853 2024-05-21 19:59:22.000000 mircheck-0.1.1/setup.py
```

### Comparing `mircheck-0.1.0/LICENSE` & `mircheck-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mircheck-0.1.0/PKG-INFO` & `mircheck-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,38 @@
-Metadata-Version: 2.1
-Name: mircheck
-Version: 0.1.0
-Summary: A tool to find the fastest mirror for Ubuntu and it's derivative
-Home-page: https://github.com/arkrwn/mircheck
-Author: Arie Kurniawan
-Author-email: hubungi.aja@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # Mircheck - Fastest Mirror Selector for Ubuntu and it's derivatives
 
 This script helps you find the fastest mirror for your Ubuntu and it's derivatives and generates a `sources.list` file accordingly. 
 It downloads the `Release` file from each mirror to measure the speed and identifies the fastest one.
 
 ## Requirements
 
 - Python 3.6 or higher
 - `requests` library
 
 ## Installation
 
-1. **Clone the repository:**
+1. **Recommended - Using PIP**
    ```sh
-   git clone https://github.com/arkrwn/mircheck.git
-   cd mircheck
+   pip install mircheck
    ```
-
-2. **Install the required libraries:**
+   
+2. **Clone the repository:**
    ```sh
-   pip install requests
+   git clone https://github.com/arkrwn/mircheck.git
+   cd mircheck/mircheck
+   pip install -r ../requirements.txt
+   chmod +x main.py
    ```
 
 ## Usage
 
 ```sh
-python3 mircheck.py [options] <distribution> <country>
+Install using pip: `mircheck [options] <distribution> <country>`
+Install using git: `./mircheck [options] <distribution> <country>`
 ```
 
 ### Positional Arguments
 
 - `distribution`: Distribution code name (e.g., jammy, bionic).
 - `country`: Country code or name.
 
@@ -55,25 +44,25 @@
 - `-n, --nonfree`: Include non-free section in the generated `sources.list`.
 - `-d, --distribution_type {stable, testing, unstable, experimental, release_codename, sid}`: Specify which distribution of Debian to use. Default is `stable`.
 
 ### Examples
 
 1. **Find the fastest mirror for Ubuntu `jammy` in Indonesia and save to the current directory:**
    ```sh
-   python3 mircheck.py jammy id
+   mircheck jammy id
    ```
 
 2. **Find the fastest mirror for Debian `stable` in Germany and include source lines:**
    ```sh
-   python3 mircheck.py stable germany -s
+   mircheck stable germany -s
    ```
 
 3. **Find the fastest mirror for Ubuntu `bionic` in the USA and save to a custom path:**
    ```sh
-   python3 mircheck.py bionic us -o /path/to/custom/sources.list
+   mircheck bionic us -o /path/to/custom/sources.list
    ```
 
 ## Output
 
 The script will test each mirror's speed and display the results in kilobytes per second (KB/s). It will identify the fastest mirror and generate a `sources.list` file with the appropriate entries.
 
 ## License
@@ -82,10 +71,9 @@
 
 ## Contributing
 
 Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Acknowledgements
 
-- The `requests` library for handling HTTP requests.
-- The Ubuntu and Debian communities for providing mirror lists.
+- The Ubuntu for providing mirror lists.
```

### Comparing `mircheck-0.1.0/README.md` & `mircheck-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,52 @@
+Metadata-Version: 2.1
+Name: mircheck
+Version: 0.1.1
+Summary: A tool to find the fastest mirror for Ubuntu and it's derivatives
+Home-page: https://github.com/arkrwn/mircheck
+Author: Arie Kurniawan
+Author-email: hubungi.aja@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Mircheck - Fastest Mirror Selector for Ubuntu and it's derivatives
 
 This script helps you find the fastest mirror for your Ubuntu and it's derivatives and generates a `sources.list` file accordingly. 
 It downloads the `Release` file from each mirror to measure the speed and identifies the fastest one.
 
 ## Requirements
 
 - Python 3.6 or higher
 - `requests` library
 
 ## Installation
 
-1. **Clone the repository:**
+1. **Recommended - Using PIP**
    ```sh
-   git clone https://github.com/arkrwn/mircheck.git
-   cd mircheck
+   pip install mircheck
    ```
-
-2. **Install the required libraries:**
+   
+2. **Clone the repository:**
    ```sh
-   pip install requests
+   git clone https://github.com/arkrwn/mircheck.git
+   cd mircheck/mircheck
+   pip install -r ../requirements.txt
+   chmod +x main.py
    ```
 
 ## Usage
 
 ```sh
-python3 mircheck.py [options] <distribution> <country>
+Install using pip: `mircheck [options] <distribution> <country>`
+Install using git: `./mircheck [options] <distribution> <country>`
 ```
 
 ### Positional Arguments
 
 - `distribution`: Distribution code name (e.g., jammy, bionic).
 - `country`: Country code or name.
 
@@ -41,25 +58,25 @@
 - `-n, --nonfree`: Include non-free section in the generated `sources.list`.
 - `-d, --distribution_type {stable, testing, unstable, experimental, release_codename, sid}`: Specify which distribution of Debian to use. Default is `stable`.
 
 ### Examples
 
 1. **Find the fastest mirror for Ubuntu `jammy` in Indonesia and save to the current directory:**
    ```sh
-   python3 mircheck.py jammy id
+   mircheck jammy id
    ```
 
 2. **Find the fastest mirror for Debian `stable` in Germany and include source lines:**
    ```sh
-   python3 mircheck.py stable germany -s
+   mircheck stable germany -s
    ```
 
 3. **Find the fastest mirror for Ubuntu `bionic` in the USA and save to a custom path:**
    ```sh
-   python3 mircheck.py bionic us -o /path/to/custom/sources.list
+   mircheck bionic us -o /path/to/custom/sources.list
    ```
 
 ## Output
 
 The script will test each mirror's speed and display the results in kilobytes per second (KB/s). It will identify the fastest mirror and generate a `sources.list` file with the appropriate entries.
 
 ## License
@@ -68,10 +85,9 @@
 
 ## Contributing
 
 Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Acknowledgements
 
-- The `requests` library for handling HTTP requests.
-- The Ubuntu and Debian communities for providing mirror lists.
+- The Ubuntu for providing mirror lists.
```

### Comparing `mircheck-0.1.0/mircheck/main.py` & `mircheck-0.1.1/mircheck/mircheck.py`

 * *Files identical despite different names*

### Comparing `mircheck-0.1.0/mircheck.egg-info/PKG-INFO` & `mircheck-0.1.1/mircheck.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mircheck
-Version: 0.1.0
-Summary: A tool to find the fastest mirror for Ubuntu and it's derivative
+Version: 0.1.1
+Summary: A tool to find the fastest mirror for Ubuntu and it's derivatives
 Home-page: https://github.com/arkrwn/mircheck
 Author: Arie Kurniawan
 Author-email: hubungi.aja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -21,29 +21,32 @@
 ## Requirements
 
 - Python 3.6 or higher
 - `requests` library
 
 ## Installation
 
-1. **Clone the repository:**
+1. **Recommended - Using PIP**
    ```sh
-   git clone https://github.com/arkrwn/mircheck.git
-   cd mircheck
+   pip install mircheck
    ```
-
-2. **Install the required libraries:**
+   
+2. **Clone the repository:**
    ```sh
-   pip install requests
+   git clone https://github.com/arkrwn/mircheck.git
+   cd mircheck/mircheck
+   pip install -r ../requirements.txt
+   chmod +x main.py
    ```
 
 ## Usage
 
 ```sh
-python3 mircheck.py [options] <distribution> <country>
+Install using pip: `mircheck [options] <distribution> <country>`
+Install using git: `./mircheck [options] <distribution> <country>`
 ```
 
 ### Positional Arguments
 
 - `distribution`: Distribution code name (e.g., jammy, bionic).
 - `country`: Country code or name.
 
@@ -55,25 +58,25 @@
 - `-n, --nonfree`: Include non-free section in the generated `sources.list`.
 - `-d, --distribution_type {stable, testing, unstable, experimental, release_codename, sid}`: Specify which distribution of Debian to use. Default is `stable`.
 
 ### Examples
 
 1. **Find the fastest mirror for Ubuntu `jammy` in Indonesia and save to the current directory:**
    ```sh
-   python3 mircheck.py jammy id
+   mircheck jammy id
    ```
 
 2. **Find the fastest mirror for Debian `stable` in Germany and include source lines:**
    ```sh
-   python3 mircheck.py stable germany -s
+   mircheck stable germany -s
    ```
 
 3. **Find the fastest mirror for Ubuntu `bionic` in the USA and save to a custom path:**
    ```sh
-   python3 mircheck.py bionic us -o /path/to/custom/sources.list
+   mircheck bionic us -o /path/to/custom/sources.list
    ```
 
 ## Output
 
 The script will test each mirror's speed and display the results in kilobytes per second (KB/s). It will identify the fastest mirror and generate a `sources.list` file with the appropriate entries.
 
 ## License
@@ -82,10 +85,9 @@
 
 ## Contributing
 
 Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Acknowledgements
 
-- The `requests` library for handling HTTP requests.
-- The Ubuntu and Debian communities for providing mirror lists.
+- The Ubuntu for providing mirror lists.
```

### Comparing `mircheck-0.1.0/setup.py` & `mircheck-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mircheck",
-    version="0.1.0",
+    version="0.1.1",
     author="Arie Kurniawan",
     author_email="hubungi.aja@gmail.com",
-    description="A tool to find the fastest mirror for Ubuntu and it's derivative",
+    description="A tool to find the fastest mirror for Ubuntu and it's derivatives",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arkrwn/mircheck",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         "requests",
+        "json"
     ],
     entry_points={
         'console_scripts': [
-            'mircheck=mircheck.main:main',
+            'mircheck=mircheck:main',
         ],
     },
 )
```

