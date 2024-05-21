# Comparing `tmp/krules-dev-support-0.9.1.tar.gz` & `tmp/krules-dev-support-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krules-dev-support-0.9.1.tar", last modified: Thu Aug 26 09:33:43 2021, max compression
+gzip compressed data, was "dist/krules-dev-support-0.9.2.tar", last modified: Sat Oct  9 15:44:47 2021, max compression
```

## Comparing `krules-dev-support-0.9.1.tar` & `krules-dev-support-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 ade       (1000) ade       (1000)        0 2021-08-26 09:33:43.234072 krules-dev-support-0.9.1/
--rw-rw-r--   0 ade       (1000) ade       (1000)      225 2021-06-17 15:55:01.000000 krules-dev-support-0.9.1/AUTHORS
--rw-rw-r--   0 ade       (1000) ade       (1000)    11341 2021-06-17 15:55:01.000000 krules-dev-support-0.9.1/LICENSE
--rw-rw-r--   0 ade       (1000) ade       (1000)      668 2021-08-26 09:33:43.234072 krules-dev-support-0.9.1/PKG-INFO
--rw-rw-r--   0 ade       (1000) ade       (1000)      199 2021-06-17 15:55:01.000000 krules-dev-support-0.9.1/README.md
-drwxrwxr-x   0 ade       (1000) ade       (1000)        0 2021-08-26 09:33:43.234072 krules-dev-support-0.9.1/krules_dev/
--rw-rw-r--   0 ade       (1000) ade       (1000)        0 2021-07-07 08:53:15.000000 krules-dev-support-0.9.1/krules_dev/__init__.py
--rw-rw-r--   0 ade       (1000) ade       (1000)    23139 2021-08-26 08:17:25.000000 krules-dev-support-0.9.1/krules_dev/sane_utils.py
-drwxrwxr-x   0 ade       (1000) ade       (1000)        0 2021-08-26 09:33:43.234072 krules-dev-support-0.9.1/krules_dev_support.egg-info/
--rw-rw-r--   0 ade       (1000) ade       (1000)      668 2021-08-26 09:33:43.000000 krules-dev-support-0.9.1/krules_dev_support.egg-info/PKG-INFO
--rw-rw-r--   0 ade       (1000) ade       (1000)      291 2021-08-26 09:33:43.000000 krules-dev-support-0.9.1/krules_dev_support.egg-info/SOURCES.txt
--rw-rw-r--   0 ade       (1000) ade       (1000)        1 2021-08-26 09:33:43.000000 krules-dev-support-0.9.1/krules_dev_support.egg-info/dependency_links.txt
--rw-rw-r--   0 ade       (1000) ade       (1000)       84 2021-08-26 09:33:43.000000 krules-dev-support-0.9.1/krules_dev_support.egg-info/requires.txt
--rw-rw-r--   0 ade       (1000) ade       (1000)       11 2021-08-26 09:33:43.000000 krules-dev-support-0.9.1/krules_dev_support.egg-info/top_level.txt
--rw-rw-r--   0 ade       (1000) ade       (1000)       38 2021-08-26 09:33:43.234072 krules-dev-support-0.9.1/setup.cfg
--rw-rw-r--   0 ade       (1000) ade       (1000)      947 2021-08-26 08:53:35.000000 krules-dev-support-0.9.1/setup.py
+drwxrwxr-x   0 ade       (1000) ade       (1000)        0 2021-10-09 15:44:47.243261 krules-dev-support-0.9.2/
+-rw-rw-r--   0 ade       (1000) ade       (1000)      225 2021-06-17 15:55:01.000000 krules-dev-support-0.9.2/AUTHORS
+-rw-rw-r--   0 ade       (1000) ade       (1000)    11341 2021-06-17 15:55:01.000000 krules-dev-support-0.9.2/LICENSE
+-rw-rw-r--   0 ade       (1000) ade       (1000)      669 2021-10-09 15:44:47.243261 krules-dev-support-0.9.2/PKG-INFO
+-rw-rw-r--   0 ade       (1000) ade       (1000)      199 2021-06-17 15:55:01.000000 krules-dev-support-0.9.2/README.md
+drwxrwxr-x   0 ade       (1000) ade       (1000)        0 2021-10-09 15:44:47.243261 krules-dev-support-0.9.2/krules_dev/
+-rw-rw-r--   0 ade       (1000) ade       (1000)        0 2021-07-07 08:53:15.000000 krules-dev-support-0.9.2/krules_dev/__init__.py
+-rw-rw-r--   0 ade       (1000) ade       (1000)    24410 2021-10-08 09:53:32.000000 krules-dev-support-0.9.2/krules_dev/sane_utils.py
+drwxrwxr-x   0 ade       (1000) ade       (1000)        0 2021-10-09 15:44:47.243261 krules-dev-support-0.9.2/krules_dev_support.egg-info/
+-rw-rw-r--   0 ade       (1000) ade       (1000)      669 2021-10-09 15:44:46.000000 krules-dev-support-0.9.2/krules_dev_support.egg-info/PKG-INFO
+-rw-rw-r--   0 ade       (1000) ade       (1000)      306 2021-10-09 15:44:46.000000 krules-dev-support-0.9.2/krules_dev_support.egg-info/SOURCES.txt
+-rw-rw-r--   0 ade       (1000) ade       (1000)        1 2021-10-09 15:44:46.000000 krules-dev-support-0.9.2/krules_dev_support.egg-info/dependency_links.txt
+-rw-rw-r--   0 ade       (1000) ade       (1000)       84 2021-10-09 15:44:46.000000 krules-dev-support-0.9.2/krules_dev_support.egg-info/requires.txt
+-rw-rw-r--   0 ade       (1000) ade       (1000)       11 2021-10-09 15:44:46.000000 krules-dev-support-0.9.2/krules_dev_support.egg-info/top_level.txt
+-rw-rw-r--   0 ade       (1000) ade       (1000)      100 2021-10-08 09:53:32.000000 krules-dev-support-0.9.2/pyproject.toml
+-rw-rw-r--   0 ade       (1000) ade       (1000)       38 2021-10-09 15:44:47.243261 krules-dev-support-0.9.2/setup.cfg
+-rw-rw-r--   0 ade       (1000) ade       (1000)      948 2021-10-09 15:44:32.000000 krules-dev-support-0.9.2/setup.py
```

### Comparing `krules-dev-support-0.9.1/LICENSE` & `krules-dev-support-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krules-dev-support-0.9.1/PKG-INFO` & `krules-dev-support-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: krules-dev-support
-Version: 0.9.1
+Version: 0.9.2
 Summary: KRules dev utilities
 Home-page: https://github.com/airspot-dev/krules
 Author: Alberto Degli Esposti
 Author-email: alberto@arispot.tech
 License: Apache Licence 2.0
 Keywords: krules rules engine sane-build
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >3.8
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 
 This module contains shared code used by make.py files contained in the different modules of the project
 
 For a better understanding take a look at [sane project](https://github.com/mikeevmm/sane)
```

### Comparing `krules-dev-support-0.9.1/krules_dev/sane_utils.py` & `krules-dev-support-0.9.2/krules_dev/sane_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,21 +63,23 @@
     _load_dir_env(cur_dir)
 
 
 def get_buildable_image(location: str,
                         dir_name: str,
                         name=None,
                         use_release_version=True,
+                        docker_registry=None,
                         environ_override: typing.Optional[str] = None,
                         push_cmd: str = "push",
                         digest_file: str = ".digest"):
     if environ_override is not None and environ_override in os.environ:
         return os.environ[environ_override]
     if use_release_version and 'RELEASE_VERSION' in os.environ:
-        docker_registry = check_envvar_exists("DOCKER_REGISTRY")
+        if docker_registry is None:
+            docker_registry = check_envvar_exists("DOCKER_REGISTRY")
         if name is None:
             name = f'krules-{dir_name}'
         return f'{docker_registry}/{name}:{os.environ["RELEASE_VERSION"]}'
     try:
         build_dir = os.path.join(location, dir_name)
         Help.log(f"Ensuring {digest_file} in {dir_name}")
         run([
@@ -92,47 +94,50 @@
 def get_image(image, environ_override: typing.Optional[str] = None):
     """
     Convenient method for guessing the image name if we have a RELEASE_VERSION defined
     or using the KRrules source repo located in KRULES_ROOT_DIR.
     It is a wrapper for the more specialized get_buildable_image function
     """
     if "RELEASE_VERSION" in os.environ:
+        docker_registry = check_envvar_exists("RELEASE_DOCKER_REGISTRY")
         return get_buildable_image(
             location="",
             dir_name=image,
             environ_override=environ_override,
+            docker_registry=docker_registry,
         )
     if "KRULES_ROOT_DIR" in os.environ:
         return get_buildable_image(
             location=os.path.join(os.environ["KRULES_ROOT_DIR"], "images"),
             dir_name=image,
             environ_override=environ_override,
         )
     if environ_override is not None and environ_override in os.environ:
         return os.environ[environ_override]
     Help.error("One of RELEASE_VERSION or KRULES_ROOT_DIR needed")
 
 
-def get_project_base(image):
+def get_project_base(location):
     """
     Get and eventually build the image from the specified folder contained in the project root
     It is a wrapper for the more specialized get_buildable_image function
 
-    :param image: a folder whit that name is expected in the project root to build image from
+    :param location: a folder with that name is expected in the project root to build image from
     :return image digest
     """
     if "KRULES_PROJECT_DIR" not in os.environ:
         Help.error("Cannot guess project root directory")
-    target_dir = os.path.join(os.environ["KRULES_PROJECT_DIR"], image)
+    target_dir = os.path.join(os.environ["KRULES_PROJECT_DIR"], location)
     if not os.path.exists(target_dir) or not os.path.isdir(target_dir):
         Help.error(f"{target_dir} does not exists or is not a directory")
     return get_buildable_image(
         location=os.environ["KRULES_PROJECT_DIR"],
-        dir_name=image,
-        environ_override=None
+        dir_name=location,
+        environ_override=None,
+        use_release_version=False,
     )
 
 
 def update_code_hash(globs: list,
                      output_file: str = ".code.digest"):
 
     abs_path = os.path.abspath(inspect.stack()[-1].filename)
@@ -405,22 +410,22 @@
             try:
                 if service_api == "base":
                     out = run([
                         kubectl_cmd, *kubectl_opts, "-n", namespace, "get", "deployments",
                         "-o", "jsonpath=\"{{.items[?(@.metadata.name=='{}')]}}\"".format(app_name)
                     ], check=True, capture_output=True).stdout
                     if len(out) > len('""'):  # found
-                        Help.log(f"updating deployment '{app_name}")
+                        Help.log(f"updating deployment {app_name}")
                         out = run([
                             kubectl_cmd, *kubectl_opts, "-n", namespace, "set", "image", f"deployment/{app_name}",
                             f"{app_name}={_image}", "--record"
                         ], check=True, capture_output=True).stdout
                         [Help.log(f"> {l}") for l in out.decode().splitlines()]
                     else:
-                        Help.log(f"creating deployment '{app_name}")
+                        Help.log(f"creating deployment {app_name}")
                         deployment = {
                             "apiVersion": "apps/v1",
                             "kind": "Deployment",
                             "metadata": {
                                 "name": app_name,
                                 "labels": _labels,
                             },
@@ -526,40 +531,62 @@
     os.chdir(new_dir)
     try:
         yield
     finally:
         os.chdir(old_dir)
 
 
-
-
-def copy_dirs(src: typing.Iterable[str], dst: str,
-              override: bool = True,
-              make_recipes: typing.Iterable = (),
-              workdir: str = None):
+def copy_resources(src: typing.Iterable[str], dst: str,
+                   override: bool = True,
+                   make_recipes_before: typing.Iterable = (),
+                   make_recipes_after: typing.Iterable = (),
+                   workdir: str = None):
+
+    for recipe in make_recipes_before:
+        for f in src:
+            fname=os.path.basename(f)
+            fdir=os.path.dirname(f)
+            make_py = os.path.join(fdir, "make.py")
+            if os.path.exists(make_py):
+                cmd = " ".join((make_py, recipe.format(src=fname)))
+                Help.log(f"Invoking [before] {cmd}")
+                try:
+                    run(cmd, shell=True, check=True, capture_output=True)
+                except CalledProcessError as err:
+                    Help.error(err.stderr.decode())
 
     if workdir is None:
         workdir = os.path.abspath(inspect.stack()[1].filename)
-    root_dir = os.path.dirname(workdir)
+    dest_dir = os.path.dirname(workdir)
 
-    with pushd(root_dir):
+    # wi pushd(src_base_dir):
+    #       _recipe_before:
+    #         run(f"make
+    #         y {r)}", shell=True, check=True, capture_output=True)
+    with pushd(dest_dir):
         os.makedirs(dst, exist_ok=True)
         for p in src:
             to_path = os.path.join(dst, os.path.basename(p))
             if os.path.exists(to_path):
                 if override:
-                    shutil.rmtree(to_path)
+                    if os.path.isdir(to_path):
+                        shutil.rmtree(to_path)
+                    else:
+                        os.unlink(to_path)
                 else:
                     Help.error(f"Destination path {to_path} already exists")
-            shutil.copytree(p, to_path)
-            for recipe in make_recipes:
+            if os.path.isdir(p):
+                shutil.copytree(p, to_path)
+            else:
+                shutil.copyfile(p, to_path)
+            for recipe in make_recipes_after:
                 make_py = os.path.join(to_path, "make.py")
                 if os.path.exists(make_py):
                     cmd = " ".join((make_py, recipe))
-                    Help.log(f"Invoking {cmd}")
+                    Help.log(f"Invoking [after] {cmd}")
                     try:
                         run(cmd, shell=True, check=True, capture_output=True)
                     except CalledProcessError as err:
                         Help.error(err.stderr.decode())
 
 
 def copy_source(src: typing.Union[typing.Iterable[str], str],
@@ -582,13 +609,13 @@
     if not condition():
         return
     if isinstance(src, str):
         src = [src]
     src = list(map(lambda x: os.path.join(os.environ["KRULES_ROOT_DIR"], x), src))
 
     workdir = os.path.abspath(inspect.stack()[1].filename)
-    copy_dirs(
+    copy_resources(
         src, dst, override, make_recipes,
         workdir
     )
```

### Comparing `krules-dev-support-0.9.1/krules_dev_support.egg-info/PKG-INFO` & `krules-dev-support-0.9.2/krules_dev_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: krules-dev-support
-Version: 0.9.1
+Version: 0.9.2
 Summary: KRules dev utilities
 Home-page: https://github.com/airspot-dev/krules
 Author: Alberto Degli Esposti
 Author-email: alberto@arispot.tech
 License: Apache Licence 2.0
 Keywords: krules rules engine sane-build
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >3.8
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 
 This module contains shared code used by make.py files contained in the different modules of the project
 
 For a better understanding take a look at [sane project](https://github.com/mikeevmm/sane)
```

### Comparing `krules-dev-support-0.9.1/setup.py` & `krules-dev-support-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='krules-dev-support',
-    version="0.9.1",
+    version="0.9.2",
     author="Alberto Degli Esposti",
     author_email="alberto@arispot.tech",
     description="KRules dev utilities",
     license="Apache Licence 2.0",
     keywords="krules rules engine sane-build",
     url="https://github.com/airspot-dev/krules",
     packages=find_packages(),
     long_description=read('README.md'),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
     ],
-    python_requires='>3.8',
+    python_requires='>=3.8',
     install_requires=[
         'Jinja2==3.0.1',
         'sane-build==7.2',
         'python-dotenv==0.19.0',
         'PyYAML==5.4.1',
         'MarkupSafe==2.0.1',
     ],
```

