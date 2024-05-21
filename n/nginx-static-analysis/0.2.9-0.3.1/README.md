# Comparing `tmp/nginx-static-analysis-0.2.9.tar.gz` & `tmp/nginx_static_analysis-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-static-analysis-0.2.9.tar", last modified: Mon Jul 10 22:18:35 2023, max compression
+gzip compressed data, was "nginx_static_analysis-0.3.1.tar", last modified: Tue May 21 08:59:59 2024, max compression
```

## Comparing `nginx-static-analysis-0.2.9.tar` & `nginx_static_analysis-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/nginx_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 22:18:35.613096 nginx-static-analysis-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:59.217687 nginx_static_analysis-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-21 08:59:59.213687 nginx_static_analysis-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:59.213687 nginx_static_analysis-0.3.1/nginx_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/nginx_analysis/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:59.213687 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-21 08:59:59.000000 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-21 08:59:59.000000 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:59:59.000000 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 08:59:59.000000 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 08:59:59.000000 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 08:59:59.000000 nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 08:59:59.217687 nginx_static_analysis-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:59:59.213687 nginx_static_analysis-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-21 08:59:54.000000 nginx_static_analysis-0.3.1/tests/testcase.py
```

### Comparing `nginx-static-analysis-0.2.9/LICENSE` & `nginx_static_analysis-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.9/PKG-INFO` & `nginx_static_analysis-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-static-analysis
-Version: 0.2.9
+Version: 0.3.1
 Summary: Parse Nginx configurations in a clear manner for debugging purposes
 Home-page: https://github.com/AlexanderGrooff/nginx-static-analysis
 Author: Alexander Grooff
 Author-email: Alexander Grooff <alexandergrooff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexander Grooff
@@ -27,14 +27,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: crossplane==0.5.7
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: loguru==0.5.3
+Requires-Dist: prettytable==2.5.0
 
 # Nginx Static Analysis
 
 [![nginx-static-analysis](https://img.shields.io/pypi/v/nginx-static-analysis)](https://pypi.org/project/nginx-static-analysis/)
 
 Parse Nginx configurations on your host and filter for directives/values.
 
@@ -46,15 +50,15 @@
 
 ```bash
 
 # Pip
 pip install nginx-static-analysis
 
 # Arch
-yay -S nginx-static-analysis
+yay -S nginx-static-analysis-git
 ```
 
 ## Analysing your Nginx configuration
 
 You can list any directive within your Nginx configuration. For example, show all `listen` directives:
 ```
 app@wifbtb-testalex-magweb-cmbl:~$ nginx-static-analysis -d listen
```

### Comparing `nginx-static-analysis-0.2.9/README.md` & `nginx_static_analysis-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ```bash
 
 # Pip
 pip install nginx-static-analysis
 
 # Arch
-yay -S nginx-static-analysis
+yay -S nginx-static-analysis-git
 ```
 
 ## Analysing your Nginx configuration
 
 You can list any directive within your Nginx configuration. For example, show all `listen` directives:
 ```
 app@wifbtb-testalex-magweb-cmbl:~$ nginx-static-analysis -d listen
```

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/analysis.py` & `nginx_static_analysis-0.3.1/nginx_analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import crossplane
 from loguru import logger
 
 from nginx_analysis.dataclasses import (
     DirectiveFilter,
     NginxLineConfig,
     RootNginxConfig,
+    convert_to_abs_path,
     filter_unique,
     get_children_recursive,
     get_parents_recursive,
 )
 
 
 def sort_by_depth(line_configs: List[NginxLineConfig]) -> List[NginxLineConfig]:
@@ -34,15 +35,16 @@
     """
     return nginx.replace("*", r"[^/]*")
 
 
 def set_parents_in_include(root_config: RootNginxConfig, block_config: NginxLineConfig):
     if block_config.directive == "include":
         for file_path in block_config.args:
-            nested_file_configs = root_config.get_files(nginx_to_regex(file_path))
+            abs_path = convert_to_abs_path(root_config.root_dir, file_path)
+            nested_file_configs = root_config.get_files(nginx_to_regex(abs_path))
             for nested_file_config in nested_file_configs:
                 for nested_line_config in nested_file_config.parsed:
                     nested_line_config.parent = block_config
                     block_config.children.append(nested_line_config)
                     set_parents_in_include(root_config, nested_line_config)
```

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/dataclasses.py` & `nginx_static_analysis-0.3.1/nginx_analysis/dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,24 @@
     while current_line.parent:
         parents.append(current_line.parent)
         current_line = current_line.parent
 
     return parents
 
 
+def convert_to_abs_path(root_dir: Path, file_path: str) -> str:
+    """
+    Make a path absolute based on the root directory.
+    """
+    path = Path(file_path)
+    if path.is_absolute():
+        return str(path)
+    return str(root_dir / path)
+
+
 class DirectiveFilter(BaseModel):
     directive: str
     value: Optional[str] = None
 
     def match(self, line: "NginxLineConfig") -> bool:
         """
         A block matches if the block itself matches or all filters apply
@@ -71,20 +81,20 @@
         return self.__repr__()
 
 
 class NginxLineConfig(BaseModel):
     directive: str
     line: int
     args: List[str]
-    file: Optional[Path]  # Only filled in after parsing
-    block: Optional[List["NginxLineConfig"]]
-    parent: Optional["NginxLineConfig"]
+    file: Optional[Path] = None  # Only filled in after parsing
+    block: Optional[List["NginxLineConfig"]] = None
+    parent: Optional["NginxLineConfig"] = None
     children: List["NginxLineConfig"] = []
-    definitely_no_match = False
-    full_match = False
+    definitely_no_match: bool = False
+    full_match: bool = False
 
     @property
     def lineage(self) -> List[str]:
         if not self.parent:
             return [self.directive]
         return self.parent.lineage + [self.directive]
 
@@ -112,15 +122,15 @@
 
 
 class NginxFileConfig(BaseModel):
     file: Path
     status: str
     errors: List[str]
     parsed: List[NginxLineConfig]
-    included_in: Optional[Tuple["NginxFileConfig", NginxLineConfig]]
+    included_in: Optional[Tuple["NginxFileConfig", NginxLineConfig]] = None
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, NginxFileConfig):
             return False
 
         comparison_fields = ["file", "status", "errors", "parsed"]
         return compare_objects(self, other, comparison_fields)
```

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/filter.py` & `nginx_static_analysis-0.3.1/nginx_analysis/filter.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/input.py` & `nginx_static_analysis-0.3.1/nginx_analysis/input.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/log.py` & `nginx_static_analysis-0.3.1/nginx_analysis/log.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/main.py` & `nginx_static_analysis-0.3.1/nginx_analysis/main.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.9/nginx_analysis/output.py` & `nginx_static_analysis-0.3.1/nginx_analysis/output.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/PKG-INFO` & `nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-static-analysis
-Version: 0.2.9
+Version: 0.3.1
 Summary: Parse Nginx configurations in a clear manner for debugging purposes
 Home-page: https://github.com/AlexanderGrooff/nginx-static-analysis
 Author: Alexander Grooff
 Author-email: Alexander Grooff <alexandergrooff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexander Grooff
@@ -27,14 +27,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: crossplane==0.5.7
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: loguru==0.5.3
+Requires-Dist: prettytable==2.5.0
 
 # Nginx Static Analysis
 
 [![nginx-static-analysis](https://img.shields.io/pypi/v/nginx-static-analysis)](https://pypi.org/project/nginx-static-analysis/)
 
 Parse Nginx configurations on your host and filter for directives/values.
 
@@ -46,15 +50,15 @@
 
 ```bash
 
 # Pip
 pip install nginx-static-analysis
 
 # Arch
-yay -S nginx-static-analysis
+yay -S nginx-static-analysis-git
 ```
 
 ## Analysing your Nginx configuration
 
 You can list any directive within your Nginx configuration. For example, show all `listen` directives:
 ```
 app@wifbtb-testalex-magweb-cmbl:~$ nginx-static-analysis -d listen
```

### Comparing `nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/SOURCES.txt` & `nginx_static_analysis-0.3.1/nginx_static_analysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 nginx_analysis/main.py
 nginx_analysis/output.py
 nginx_static_analysis.egg-info/PKG-INFO
 nginx_static_analysis.egg-info/SOURCES.txt
 nginx_static_analysis.egg-info/dependency_links.txt
 nginx_static_analysis.egg-info/entry_points.txt
 nginx_static_analysis.egg-info/requires.txt
-nginx_static_analysis.egg-info/top_level.txt
+nginx_static_analysis.egg-info/top_level.txt
+tests/testcase.py
```

### Comparing `nginx-static-analysis-0.2.9/pyproject.toml` & `nginx_static_analysis-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "nginx-static-analysis"
-version = "0.2.9"
+version = "0.3.1"
 description = "Parse Nginx configurations in a clear manner for debugging purposes"
 authors = [
     {name = "Alexander Grooff", email = "alexandergrooff@gmail.com"},
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 license = {name = "MIT", file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "crossplane==0.5.7",
-    "pydantic==1.8.2",
+    "pydantic==2.7.1",
     "loguru==0.5.3",
     "prettytable==2.5.0",
 ]
 
 [project.scripts]
 nginx-static-analysis = "nginx_analysis.main:main"
```

### Comparing `nginx-static-analysis-0.2.9/setup.py` & `nginx_static_analysis-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 requirements = """
 crossplane==0.5.7
-pydantic==1.8.2
+pydantic==2.7.1
 loguru==0.5.3
 prettytable==2.5.0
 """
 
 
 setup(
     name="nginx-static-analysis",
-    version="0.2.9",
+    version="0.3.1",
     description="Parse Nginx configurations in a clear manner for debugging purposes",
     url="https://github.com/AlexanderGrooff/nginx-static-analysis",
     packages=find_packages(
         include=["nginx_analysis", "requirements/base.txt"], exclude=["tests"]
     ),
     author="Alexander Grooff",
     author_email="alexandergrooff@gmail.com",
```

