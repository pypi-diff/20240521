# Comparing `tmp/cosmix_launcher-1.0.7.tar.gz` & `tmp/cosmix_launcher-1.0.8.tar.gz`

## Comparing `cosmix_launcher-1.0.7.tar` & `cosmix_launcher-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/license.txt
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/scripts/test.sh
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/config.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/net.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/.gitignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/readme.md
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/license.txt
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/scripts/test.sh
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/.gitignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/readme.md
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.7/license.txt` & `cosmix_launcher-1.0.8/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/requirements.txt` & `cosmix_launcher-1.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/src/cosmix/__init__.py` & `cosmix_launcher-1.0.8/src/cosmix/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     Instance.from_config_file(name).launch(args.split())
 
 
 @cosmix.command()
 def instances():
     if not os.path.exists(paths.INSTANCES) or len(os.listdir(paths.INSTANCES)) <= 0:
         logger.error("No instances found.")
-        exit(0)
+        exit(1)
 
     for instance_name in os.listdir(paths.INSTANCES):
         instance = Instance.get_or_throw(instance_name)
         s = f" - \u001b[1m{instance.display_name}\u001b[0m"
         if instance.display_name != instance.name:
             s += f" ({instance.name})"
         s += f" \u001b[33m(Version: {instance.version})\u001b[0m"
@@ -104,15 +104,15 @@
 
 
 @cosmix.command()
 @click.argument("name")
 def trash(name: str):
     instance = Instance.get_or_throw(name)
     send2trash.send2trash(instance.path)
-    logger.info("Moved " + name + " to trash")
+    logger.info("Moved " + name + " to trash.")
 
 
 @cosmix.command()
 @click.argument("name")
 def info(name: str):
     i = Instance.get_or_throw(name)
     print(i.display_name + ":")
@@ -137,14 +137,16 @@
         logger.error("Instance is not modded")
         exit(1)
 
     path = os.path.join(i.path, "mods")
     os.makedirs(path, exist_ok = True)
     shutil.copyfile(mod, os.path.join(path, os.path.split(mod)[-1]))
 
+    logger.info("Done.")
+
 
 @cosmix.command("add-crm1-mod")
 @click.option("--repo", "-r", default=None, type=str, help="Provide a CRM-1 repo to use to resolve the mod. Dependencies may still be found using default_repos.")
 @click.argument("name")
 @click.argument("mod")
 def add_crm1_mod(repo: Optional[str], name: str, mod: str):
     i = Instance.get_or_throw(name)
@@ -157,11 +159,45 @@
     os.makedirs(path, exist_ok = True)
 
     repos = config.get_config()["crm1"]["default_repos"]
     if repo is not None:
         repos.append(repo)
 
     net.download_crm1_mod(mod, path, repos)
+    logger.info("Done.")
+
+
+@cosmix.command("add-data-mod")
+@click.option("--ignore-global-warning", "-I", is_flag = True, default = False, help = "Ignores the global path warning.")
+@click.argument("name")
+@click.argument("mod", type=click.Path(exists = True))
+def add_crm_mod(ignore_global_warning: bool, name: str, mod):
+    i = Instance.get_or_throw(name)
+
+    if not i.is_modded() and not ignore_global_warning:
+        logger.warn("Instance is not modded, this means the data mod will be installed to the GLOBAL Cosmic Reach directory (~/.local/share/cosmic-reach/)")
+        logger.warn("Use --ignore-global-warning or -I to ignore this warning.")
+        exit(1)
+
+    if i.is_modded():
+        path = os.path.join(i.path_to("mods"), "assets")
+        os.makedirs(path, exist_ok = True)
+        shutil.copytree(mod, path, dirs_exist_ok = True)
+    elif ignore_global_warning:
+        if not os.path.exists(paths.CR_DIR):
+            logger.error("Global Cosmic Reach path does not exist. This should not happen.")
+            exit(1)
+        path = os.path.join(paths.CR_DIR, "mods", "assets")
+        shutil.copytree(mod, path, dirs_exist_ok = True)
+
+    logger.info("Done.")
+
+
+@cosmix.command("whereis")
+@click.argument("name")
+def whereis(name: str):
+    i = Instance.get_or_throw(name)
+    logger.info(i.path)
 
 
 if __name__ == "__main__":
     cosmix()
```

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/config.py` & `cosmix_launcher-1.0.8/src/cosmix/api/config.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.8/src/cosmix/api/instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,26 +42,37 @@
     def is_modded(self) -> bool:
         return self.quilt_version is not None
 
     def path_to(self, path: str) -> str:
         return os.path.join(self.path, path)
 
     def get_classpath(self) -> str:
+        classpath = []
+        cq_path = paths.path_to_cq_deps(self.quilt_version)
         path = self.path_to("deps")
-        return ":".join([os.path.join(path, dep) for dep in os.listdir(path)])
+
+        # Get Cosmic Quilt deps from the global folder
+        if self.is_modded() and os.path.exists(cq_path):
+            classpath.extend([os.path.join(cq_path, dep) for dep in os.listdir(cq_path)])
+
+        # Get per-instance dependencies
+        if os.path.exists(path):
+            classpath.extend([os.path.join(path, dep) for dep in os.listdir(path)])
+
+        return ":".join(classpath)
 
     def launch(self, launch_args: Optional[list[str]] = None):
         os.chdir(self.path)
 
         args = ["java"]
         if not self.is_modded():
             args.extend(["-jar", paths.path_to_cr(self.version)])
         else:
             args.extend([
-                "-Dloader.gameJarPath=" + paths.path_to_cr(self.version),
+                f"-Dloader.gameJarPath={paths.path_to_cr(self.version)}",
                 "-classpath", self.get_classpath(),
                 "org.quiltmc.loader.impl.launch.knot.KnotClient"
             ])
         args.extend(self.args)
         if launch_args is not None:
             args.extend(launch_args)
 
@@ -69,28 +80,23 @@
         os.execvp("java", args)
 
     def download(self, is_updating: bool = False):
         cr_path = paths.path_to_cr(self.version)
         if not os.path.isfile(cr_path):
             net.download(f"{COSMIC_ARCHIVE_RAW_URL}/Cosmic Reach-{self.version}.jar", cr_path)
 
-        if self.is_modded():
+        if self.is_modded() and not os.path.exists(paths.path_to_cq_deps(self.quilt_version)):
             logger.info("Downloading Cosmic Quilt dependencies...")
 
-            pom = self.path_to("pom.xml")
-            deps = self.path_to("deps")
-            had_existing_pom = True
-            if not os.path.isfile(pom):
-                maven.make_pom(pom, self.quilt_version)
-                had_existing_pom = False
-            if is_updating and os.path.exists(deps):
-                shutil.rmtree(deps)
-            maven.copy_deps(self.path, deps)
-            if not had_existing_pom:
-                os.remove(pom)
+            pom = os.path.join(paths.path_to_cq_deps(self.quilt_version), "pom.xml")
+            deps = paths.path_to_cq_deps(self.quilt_version)
+            os.makedirs(deps, exist_ok = True)
+            maven.make_pom(pom, self.quilt_version)
+            maven.copy_deps(deps, deps)
+            os.remove(pom)
 
             self.save()
 
     def save(self):
         os.makedirs(self.path, exist_ok = True)
         with open(self.path_to("config.hjson"), "w") as f:
             hjson.dump(Instance.get_hjson(self), f)
```

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/logger.py` & `cosmix_launcher-1.0.8/src/cosmix/api/logger.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.8/src/cosmix/api/maven.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.8/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/net.py` & `cosmix_launcher-1.0.8/src/cosmix/api/net.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.8/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.7/pyproject.toml` & `cosmix_launcher-1.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmix_launcher-1.0.7/readme.md` & `cosmix_launcher-1.0.8/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,20 @@
 
 cosmix add-mod [instance] [path to mod jar]
     adds a mod jar to an instance
 
 cosmix add-crm1-mod [instance] [mod id]
     adds a mod to an instance via CRM-1. To add repos, see ~/.local/share/cosmix/config.hjson
 
+cosmix add-data-mod [instance] [mod path]
+    adds a data mod to an instance
+
+cosmic whereis [instance]
+    prints the path to a given instance
+
 cosmix trash [instance]
     moves an instance to the system's trash folder
 ```
 
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
@@ -121,14 +127,16 @@
 ```
 cosmix/
     config.hjson - Configs for Cosmix
 
     deps/
         cosmic-reach/
             Contains JARs for each downloaded Cosmic Reach version.
+        cosmic-quilt/
+            Contains the JAR dependencies for each downloaded Cosmic Quilt version.
 
     instances/
         example-instance/
             config.hjson - Configs for the instance.
             deps/
-                If the instance is modded, this folder is used to store Cosmic Quilt and its dependencies.
+                If the instance is modded, this folder is used to store extra dependencies for the classpath. Typically this will be unused.
 ```
```

### Comparing `cosmix_launcher-1.0.7/PKG-INFO` & `cosmix_launcher-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.7
+Version: 1.0.8
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -110,14 +110,20 @@
 
 cosmix add-mod [instance] [path to mod jar]
     adds a mod jar to an instance
 
 cosmix add-crm1-mod [instance] [mod id]
     adds a mod to an instance via CRM-1. To add repos, see ~/.local/share/cosmix/config.hjson
 
+cosmix add-data-mod [instance] [mod path]
+    adds a data mod to an instance
+
+cosmic whereis [instance]
+    prints the path to a given instance
+
 cosmix trash [instance]
     moves an instance to the system's trash folder
 ```
 
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
@@ -140,14 +146,16 @@
 ```
 cosmix/
     config.hjson - Configs for Cosmix
 
     deps/
         cosmic-reach/
             Contains JARs for each downloaded Cosmic Reach version.
+        cosmic-quilt/
+            Contains the JAR dependencies for each downloaded Cosmic Quilt version.
 
     instances/
         example-instance/
             config.hjson - Configs for the instance.
             deps/
-                If the instance is modded, this folder is used to store Cosmic Quilt and its dependencies.
+                If the instance is modded, this folder is used to store extra dependencies for the classpath. Typically this will be unused.
 ```
```

