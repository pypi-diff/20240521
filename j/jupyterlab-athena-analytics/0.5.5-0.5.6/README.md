# Comparing `tmp/jupyterlab_athena_analytics-0.5.5.tar.gz` & `tmp/jupyterlab_athena_analytics-0.5.6.tar.gz`

## Comparing `jupyterlab_athena_analytics-0.5.5.tar` & `jupyterlab_athena_analytics-0.5.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/CHANGELOG.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/babel.config.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/build.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jest.config.js
--rw-r--r--   0        0        0   357048 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/package-lock.json
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/setup.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/test.ipynb
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/tsconfig.test.json
--rw-r--r--   0        0        0   374390 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/yarn.lock
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/_version.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/package.json
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/509.68053d43f01f7d268d38.js
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/remoteEntry.d43dde86f53fb87db6c8.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/scripts/build.sh
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/.gitignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/.yarnrc.yml
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/index.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/__tests__/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/yarn.lock
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/LICENSE
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/README.md
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/CHANGELOG.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/babel.config.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/build.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jest.config.js
+-rw-r--r--   0        0        0   357048 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/package-lock.json
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/setup.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/test.ipynb
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/tsconfig.test.json
+-rw-r--r--   0        0        0   373470 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/yarn.lock
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/_version.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/package.json
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/509.ffcf5195228912dc474b.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/remoteEntry.f65916be0fb99f932ce1.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/scripts/build.sh
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/scripts/deploy-full.sh
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/.gitignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/.yarnrc.yml
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/index.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/__tests__/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/LICENSE
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/README.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/PKG-INFO
```

### Comparing `jupyterlab_athena_analytics-0.5.5/RELEASE.md` & `jupyterlab_athena_analytics-0.5.6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/jest.config.js` & `jupyterlab_athena_analytics-0.5.6/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/package-lock.json` & `jupyterlab_athena_analytics-0.5.6/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/package.json` & `jupyterlab_athena_analytics-0.5.6/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'0.5.6'"}*

```diff
@@ -173,12 +173,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.5",
+    "version": "0.5.6",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.5/test.ipynb` & `jupyterlab_athena_analytics-0.5.6/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/tsconfig.json` & `jupyterlab_athena_analytics-0.5.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/yarn.lock` & `jupyterlab_athena_analytics-0.5.6/yarn.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1368,15 +1368,15 @@
 "@bcoe/v8-coverage@npm:^0.2.3":
   version: 0.2.3
   resolution: "@bcoe/v8-coverage@npm:0.2.3"
   checksum: 850f9305536d0f2bd13e9e0881cb5f02e4f93fad1189f7b2d4bebf694e3206924eadee1068130d43c11b750efcc9405f88a8e42ef098b6d75239c0f047de1a27
   languageName: node
   linkType: hard
 
-"@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
+"@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.15.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.7.1":
   version: 6.16.0
   resolution: "@codemirror/autocomplete@npm:6.16.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
@@ -1385,15 +1385,15 @@
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
   checksum: e33d3d8c961c03dc4a70d1ac6f01aee5362d778da9d873a8335aed47f7de9430eab083589736e7922464b941d5da23c51ab6af05400413a8d1a07604ffcb99f7
   languageName: node
   linkType: hard
 
-"@codemirror/commands@npm:^6.2.3":
+"@codemirror/commands@npm:^6.3.3":
   version: 6.5.0
   resolution: "@codemirror/commands@npm:6.5.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.4.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.1.0
@@ -1407,28 +1407,28 @@
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/cpp": ^1.0.0
   checksum: bb9eba482cca80037ce30c7b193cf45eff19ccbb773764fddf2071756468ecc25aa53c777c943635054f89095b0247b9b50c339e107e41e68d34d12a7295f9a9
   languageName: node
   linkType: hard
 
-"@codemirror/lang-css@npm:^6.0.0, @codemirror/lang-css@npm:^6.1.1":
+"@codemirror/lang-css@npm:^6.0.0, @codemirror/lang-css@npm:^6.2.1":
   version: 6.2.1
   resolution: "@codemirror/lang-css@npm:6.2.1"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
   checksum: 5a8457ee8a4310030a969f2d3128429f549c4dc9b7907ee8888b42119c80b65af99093801432efdf659b8ec36a147d2a947bc1ecbbf69a759395214e3f4834a8
   languageName: node
   linkType: hard
 
-"@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
+"@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.8":
   version: 6.4.9
   resolution: "@codemirror/lang-html@npm:6.4.9"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
@@ -1447,15 +1447,15 @@
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
-"@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
+"@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.2.2":
   version: 6.2.2
   resolution: "@codemirror/lang-javascript@npm:6.2.2"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
@@ -1472,15 +1472,15 @@
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/json": ^1.0.0
   checksum: e9e87d50ff7b81bd56a6ab50740b1dd54e9a93f1be585e1d59d0642e2148842ea1528ac7b7221eb4ddc7fe84bbc28065144cc3ab86f6e06c6aeb2d4b4e62acf1
   languageName: node
   linkType: hard
 
-"@codemirror/lang-markdown@npm:^6.1.1":
+"@codemirror/lang-markdown@npm:^6.2.4":
   version: 6.2.5
   resolution: "@codemirror/lang-markdown@npm:6.2.5"
   dependencies:
     "@codemirror/autocomplete": ^6.7.1
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
@@ -1500,15 +1500,15 @@
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
-"@codemirror/lang-python@npm:^6.1.3":
+"@codemirror/lang-python@npm:^6.1.4":
   version: 6.1.6
   resolution: "@codemirror/lang-python@npm:6.1.6"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.8.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.1
@@ -1523,107 +1523,107 @@
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
-"@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.6.3
-  resolution: "@codemirror/lang-sql@npm:6.6.3"
+"@codemirror/lang-sql@npm:^6.6.1":
+  version: 6.6.4
+  resolution: "@codemirror/lang-sql@npm:6.6.4"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: b8e554bda9107107283674a6397cdb4816ad8bb429afd739fdc5e0339ef60170f09bdd93e7dc3eaf7f24ffaec5c7477ee42af7c05cb471990657014fac2fea1e
+  checksum: ae7c498d08c118d8f1751c28d12c54f45cacd589f6adb56216d44eb14abc0e436dcefe675d50bd02a242426327384cbcafa8c35098aa63384570a33c4cf27038
   languageName: node
   linkType: hard
 
-"@codemirror/lang-wast@npm:^6.0.1":
+"@codemirror/lang-wast@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 72119d4a7d726c54167aa227c982ae9fa785c8ad97a158d8350ae95eecfbd8028a803eef939f7e6c5c6e626fcecda1dc37e9dffc6d5d6ec105f686aeda6b2c24
   languageName: node
   linkType: hard
 
-"@codemirror/lang-xml@npm:^6.0.2":
+"@codemirror/lang-xml@npm:^6.1.0":
   version: 6.1.0
   resolution: "@codemirror/lang-xml@npm:6.1.0"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
   checksum: 3a1b7af07b29ad7e53b77bf584245580b613bc92256059f175f2b1d7c28c4e39b75654fe169b9a8a330a60164b53ff5254bdb5b8ee8c6e6766427ee115c4e229
   languageName: node
   linkType: hard
 
-"@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
+"@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.10.1, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
   version: 6.10.1
   resolution: "@codemirror/language@npm:6.10.1"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.23.0
     "@lezer/common": ^1.1.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
   checksum: 453bbe122a84795752f29261412b69a8dcfdd7e4369eb7e112bffba36b9e527ad21adff1d3845e0dc44c9ab44eb0c6f823eb6ba790ddd00cc749847574eda779
   languageName: node
   linkType: hard
 
-"@codemirror/legacy-modes@npm:^6.3.2":
+"@codemirror/legacy-modes@npm:^6.3.3":
   version: 6.4.0
   resolution: "@codemirror/legacy-modes@npm:6.4.0"
   dependencies:
     "@codemirror/language": ^6.0.0
   checksum: d382aa6f640a67418bd209e1e4b395340f96aac1b0cf185927fc2c7f98b62cfd0c59ef0f7048148ce8771622003ca844c78c2d18548235ecc57d0bcbfbbfe091
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.6.0
-  resolution: "@codemirror/lint@npm:6.6.0"
+  version: 6.7.1
+  resolution: "@codemirror/lint@npm:6.7.1"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: e68b53b051742143b50067663af8b0fe88615d5cdaa18497f888b3ea0e130c1af47525821a5a81efc45f828dbf15bb56348de1ec329f411bdd0ba3b000846555
+  checksum: b3f52b16367abe150c734b75fd9224132a06c83ebc8148724acd1352fa27d4565a3b29dbdf31d5e27a9232d595fc32c23d68321391e7345d13937ad88b48a87f
   languageName: node
   linkType: hard
 
-"@codemirror/search@npm:^6.3.0":
+"@codemirror/search@npm:^6.5.6":
   version: 6.5.6
   resolution: "@codemirror/search@npm:6.5.6"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 19dc88d09fc750563347001e83c6194bbb2a25c874bd919d2d81809e1f98d6330222ddbd284aa9758a09eeb41fd153ec7c2cf810b2ee51452c25963d7f5833d5
   languageName: node
   linkType: hard
 
-"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
+"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.4.0, @codemirror/state@npm:^6.4.1":
   version: 6.4.1
   resolution: "@codemirror/state@npm:6.4.1"
   checksum: b81b55574091349eed4d32fc0eadb0c9688f1f7c98b681318f59138ee0f527cb4c4a97831b70547c0640f02f3127647838ae6730782de4a3dd2cc58836125d01
   languageName: node
   linkType: hard
 
-"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
+"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.26.0":
   version: 6.26.3
   resolution: "@codemirror/view@npm:6.26.3"
   dependencies:
     "@codemirror/state": ^6.4.0
     style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
   checksum: fdee35fb5e0bbba7b6f1a9b43a865880911bbfafd30360da5dda21b35f81ba2d080ff66b6c3d94dbe946b6b7ec98a76208786360b8f030ef10bcb054b816de05
@@ -2032,138 +2032,138 @@
   dependencies:
     "@jridgewell/resolve-uri": ^3.1.0
     "@jridgewell/sourcemap-codec": ^1.4.14
   checksum: 9d3c40d225e139987b50c48988f8717a54a8c994d8a948ee42e1412e08988761d0754d7d10b803061cc3aebf35f92a5dbbab493bd0e1a9ef9e89a2130e83ba34
   languageName: node
   linkType: hard
 
-"@jupyter/react-components@npm:^0.15.2":
+"@jupyter/react-components@npm:^0.15.3":
   version: 0.15.3
   resolution: "@jupyter/react-components@npm:0.15.3"
   dependencies:
     "@jupyter/web-components": ^0.15.3
     "@microsoft/fast-react-wrapper": ^0.3.22
     react: ">=17.0.0 <19.0.0"
   checksum: 1a6b256314259c6465c4b6d958575710536b82234a7bf0fba3e889a07e1f19ff8ab321450be354359876f92c45dbcc9d21a840237ff4a619806d9de696f55496
   languageName: node
   linkType: hard
 
-"@jupyter/web-components@npm:^0.15.2, @jupyter/web-components@npm:^0.15.3":
+"@jupyter/web-components@npm:^0.15.3":
   version: 0.15.3
   resolution: "@jupyter/web-components@npm:0.15.3"
   dependencies:
     "@microsoft/fast-colors": ^5.3.1
     "@microsoft/fast-element": ^1.12.0
     "@microsoft/fast-foundation": ^2.49.4
     "@microsoft/fast-web-utilities": ^5.4.1
   checksum: a0980af934157bfdbdb6cc169c0816c1b2e57602d524c56bdcef746a4c25dfeb8f505150d83207c8695ed89b5486cf53d35a3382584d25ef64db666e4e16e45b
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^1.1.1":
-  version: 1.1.1
-  resolution: "@jupyter/ydoc@npm:1.1.1"
+"@jupyter/ydoc@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@jupyter/ydoc@npm:2.0.1"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
-  checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
+  checksum: f5f29e1ff3327ebc1cf326f53634e03c4c7bf7733d235087fe26975c16eebd404f23c2f3ba88b6e04b1927846be7162b09b8b8719a4b29e51d0299c745018cbb
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/application@npm:4.1.8"
+"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/application@npm:4.2.0"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/docregistry": ^4.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/statedb": ^4.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
-    "@lumino/application": ^2.3.0
-    "@lumino/commands": ^2.2.0
+    "@lumino/application": ^2.3.1
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
-  checksum: 33c57c7e825f72f8aca146bfb2ade9c91e55ac5218410ff4472b0e4cf0de0305ec34f94a9ff3ab5e8982c37a170225dbfe47b4ac900980837ecaf00b7effb0fc
+    "@lumino/widgets": ^2.3.2
+  checksum: 74811d63ddf4e6628c2467659ca1b0c39bba271689cff05925efbd3529bf4c771d41f42b04a458d1acdb0ced87b5fee5fb31d315a5b45e3449bd5f581f3be377
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.2.8":
-  version: 4.2.8
-  resolution: "@jupyterlab/apputils@npm:4.2.8"
+"@jupyterlab/apputils@npm:^4.3.0":
+  version: 4.3.0
+  resolution: "@jupyterlab/apputils@npm:4.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/settingregistry": ^4.1.8
-    "@jupyterlab/statedb": ^4.1.8
-    "@jupyterlab/statusbar": ^4.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/settingregistry": ^4.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     "@types/react": ^18.0.26
     react: ^18.2.0
-    sanitize-html: ~2.7.3
-  checksum: 253b3a21f292b19791e149926014e90eb0e6e074b86422a63ce2fbfaebc53c6e16c6cd628f79d91eb7e66b60357df79b9dc6de683b5293562f9fcbe39bcd0522
+    sanitize-html: ~2.12.1
+  checksum: 96f4f9055c464fb6f0e2545d21623b9500936da44cd7bafa9c1154164f6fc1846a518bc637ef46d6a082d208d12acf737d8aa679ce5546427ac04f068cf10cd5
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/attachments@npm:4.1.8"
+"@jupyterlab/attachments@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/attachments@npm:4.2.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-  checksum: 496eb41e8335d237f7c88b5ce7d1194292d4e6ab8952a3a62883bf4daea36dc6e426ce97b039583ea0e9b9a3ec72e755b2d842e3fc562747efe517e34930f25e
+  checksum: 1224fe573aadeaf09f803d7619d3ecadc5b8f8d85ae76abb1cbd09a12be7a55f1f84ce29f576eb4bb8f806e28a412edce26fbae7fb841e9cb7fbcce1f5cf4bf4
   languageName: node
   linkType: hard
 
 "@jupyterlab/builder@npm:^4.0.0":
-  version: 4.1.8
-  resolution: "@jupyterlab/builder@npm:4.1.8"
+  version: 4.2.0
+  resolution: "@jupyterlab/builder@npm:4.2.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
-    "@lumino/application": ^2.3.0
-    "@lumino/commands": ^2.2.0
+    "@lumino/application": ^2.3.1
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     ajv: ^8.12.0
     commander: ^9.4.1
     css-loader: ^6.7.1
     duplicate-package-checker-webpack-plugin: ^3.0.0
     fs-extra: ^10.1.0
     glob: ~7.1.6
     license-webpack-plugin: ^2.3.14
@@ -2177,532 +2177,533 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: e727e4fddbfd4e8f7d4c83e5c5aaf9be41b67771f6a4ef10b44bbc0e51bb21966b2fa1ad33eacf58420ca3a2cda2ab410331a1543e6f945b9ca0a59e109f240b
+  checksum: 9b8be036d7ad63981081f10c5aae5e33f3e4358e68774a3497ffb28dab199a2eb98994653420f46bf169af8200a57c6a9ab47529cd634c70a49d27504afbed91
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/cells@npm:4.1.8"
-  dependencies:
-    "@codemirror/state": ^6.2.0
-    "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/attachments": ^4.1.8
-    "@jupyterlab/codeeditor": ^4.1.8
-    "@jupyterlab/codemirror": ^4.1.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/documentsearch": ^4.1.8
-    "@jupyterlab/filebrowser": ^4.1.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/outputarea": ^4.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/toc": ^6.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+"@jupyterlab/cells@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/cells@npm:4.2.0"
+  dependencies:
+    "@codemirror/state": ^6.4.1
+    "@codemirror/view": ^6.26.0
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/attachments": ^4.2.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/codemirror": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/documentsearch": ^4.2.0
+    "@jupyterlab/filebrowser": ^4.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/outputarea": ^4.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/toc": ^6.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: feb2aa9b681acaae78aadffce6d9c61c6b7d4c15da23f11accf98a5d36891918a7304260f73e6b39512fadb8cc31b433bf8619cbb8d7c5c410d5c14b78558364
+  checksum: 444ddf33c9ecda1880af67cd163a6b0416f761e5e454b4fe6dc36dc9b7f39f0deaca063bfd17de6312a2627f38a44645599d9a42501e2e2790d45a395e149a9a
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/codeeditor@npm:4.1.8"
-  dependencies:
-    "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/statusbar": ^4.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+"@jupyterlab/codeeditor@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/codeeditor@npm:4.2.0"
+  dependencies:
+    "@codemirror/state": ^6.4.1
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: e5d3b0f5c94775017b044528843596ce7f5616cede5555a6a32b3a8e9ae583775f83a6448717fd15e2cf254ef50209861da06821f67267ebe2ef67b34860f7d6
+  checksum: a6e2b1cf7e46ae86154b20bd4a3c29c7c4bb0feb7b0cf6461470db99f2d6f4df13084f861fad7de9409a040191f075dcb3f148328eff419a2494cd84326749b2
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/codemirror@npm:4.1.8"
+"@jupyterlab/codemirror@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/codemirror@npm:4.2.0"
   dependencies:
-    "@codemirror/autocomplete": ^6.5.1
-    "@codemirror/commands": ^6.2.3
+    "@codemirror/autocomplete": ^6.15.0
+    "@codemirror/commands": ^6.3.3
     "@codemirror/lang-cpp": ^6.0.2
-    "@codemirror/lang-css": ^6.1.1
-    "@codemirror/lang-html": ^6.4.3
+    "@codemirror/lang-css": ^6.2.1
+    "@codemirror/lang-html": ^6.4.8
     "@codemirror/lang-java": ^6.0.1
-    "@codemirror/lang-javascript": ^6.1.7
+    "@codemirror/lang-javascript": ^6.2.2
     "@codemirror/lang-json": ^6.0.1
-    "@codemirror/lang-markdown": ^6.1.1
+    "@codemirror/lang-markdown": ^6.2.4
     "@codemirror/lang-php": ^6.0.1
-    "@codemirror/lang-python": ^6.1.3
+    "@codemirror/lang-python": ^6.1.4
     "@codemirror/lang-rust": ^6.0.1
-    "@codemirror/lang-sql": ^6.4.1
-    "@codemirror/lang-wast": ^6.0.1
-    "@codemirror/lang-xml": ^6.0.2
-    "@codemirror/language": ^6.6.0
-    "@codemirror/legacy-modes": ^6.3.2
-    "@codemirror/search": ^6.3.0
-    "@codemirror/state": ^6.2.0
-    "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/codeeditor": ^4.1.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/documentsearch": ^4.1.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@lezer/common": ^1.0.2
-    "@lezer/generator": ^1.2.2
-    "@lezer/highlight": ^1.1.4
-    "@lezer/markdown": ^1.0.2
+    "@codemirror/lang-sql": ^6.6.1
+    "@codemirror/lang-wast": ^6.0.2
+    "@codemirror/lang-xml": ^6.1.0
+    "@codemirror/language": ^6.10.1
+    "@codemirror/legacy-modes": ^6.3.3
+    "@codemirror/search": ^6.5.6
+    "@codemirror/state": ^6.4.1
+    "@codemirror/view": ^6.26.0
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/documentsearch": ^4.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@lezer/common": ^1.2.1
+    "@lezer/generator": ^1.7.0
+    "@lezer/highlight": ^1.2.0
+    "@lezer/markdown": ^1.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 0a56b6855b6dd4999e9816938f7546c2f1c46c629f05cf246813d58700f3c283e068b9c86dba275374756536472b598a19a0e5e12cfffd365817fbcc8333c795
+  checksum: 5fa46acd267dbd2e555250256a7e7820ccf9f931dfcf6a41bf15f71ed220ac317d386d81fe7ca55eb7c6136bc4e715fe086421296eb6e8fbe992b12e4b7d1be6
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.1.8":
-  version: 6.1.8
-  resolution: "@jupyterlab/coreutils@npm:6.1.8"
+"@jupyterlab/coreutils@npm:^6.2.0":
+  version: 6.2.0
+  resolution: "@jupyterlab/coreutils@npm:6.2.0"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: 1049c78bdbffb247fe7e7be4e082fe15711ca0d8da997d6da7042e0299d7ebbf1d0341d830ae0ab451bf8dfbfc30027bf3f063fc7e35210409a7aa56fe94cee9
+  checksum: 1975f19f567b63484055b0d1d10757b2bf66274814083e50702bb6017af22341cc3f5924d0ec7da408feacd652120b476aaaf50286a5401f798f257e899aed91
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/docmanager@npm:4.1.8"
+"@jupyterlab/docmanager@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/docmanager@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/docregistry": ^4.1.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/statusbar": ^4.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: d0d1316a885d1e72891d9b9cd61c36c7f8db4a4e53ae4cc8f105931e0dcdc262ebd5e76d3a145517bcc009cb3f8ab23e4e4ce84191f2f09c5df3d2a3294cfe9a
+  checksum: 63e461bf75ce4b12ada41cf727b11f956c62312b2e017fdaf9979ba16a86cb5078e7eed4f508e122afc3718d1ee18548c8ec6a1bb50f4a95a2217a77a8e0b1c3
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/docregistry@npm:4.1.8"
-  dependencies:
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/codeeditor": ^4.1.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+"@jupyterlab/docregistry@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/docregistry@npm:4.2.0"
+  dependencies:
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: d65aef500ab8d9d761490cf2a6902e897475173727cd3676691789e6d2609aefc8c98c0a4d4e57c670721409cb58925eeb162dbd101c9b6a473ecd20cf7efe78
+  checksum: ef616ca11a07a5a2d8865d909499662e8c37b19e9487081682c47808becb5d87fe09a4d1c0175ea8afd3c96a255a437b8d762e990c81d71cf9cc13cf99fe3c3b
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/documentsearch@npm:4.1.8"
+"@jupyterlab/documentsearch@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/documentsearch@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
-    "@lumino/commands": ^2.2.0
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: c8f05403435c8613c599ea54512f4a8bb865e3836f336e2258cba60291b101f35515eb6e8a33d88973d22fffe2b9772d1b0d9d177a5b7a396ff64b046b211580
+  checksum: c49919b3094390c6cefdf66c2d13baf6e7a387e087a75090cd04e65bda593bf3e9afc91307b80b851e41544ba22eae766bcacfa63480738f3f54b43f6f111c8e
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/filebrowser@npm:4.1.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/docmanager": ^4.1.8
-    "@jupyterlab/docregistry": ^4.1.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/statedb": ^4.1.8
-    "@jupyterlab/statusbar": ^4.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+"@jupyterlab/filebrowser@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/filebrowser@npm:4.2.0"
+  dependencies:
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docmanager": ^4.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 51ae88c5fabb2fad341cd3ea7b94750c373d5b3d251287f0bcbc7f1357b11f7a4e9ec08ee92512a46435fccee0c7c647cdf2185db9459a55845d15410f0dcf1c
+  checksum: d80fdb55c25472cae56852c6ce8633a9899430e784ff60fbac956c17db60bc3eb92fdc5cf4e7b1c06e1fd5b7e37c3c4f9992e4ed7d4d800cd5c65eac43d5ac08
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/lsp@npm:4.1.8"
+"@jupyterlab/lsp@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/lsp@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/codeeditor": ^4.1.8
-    "@jupyterlab/codemirror": ^4.1.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/docregistry": ^4.1.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/codemirror": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 535786735c28c8cd6b3a39c2ae0d8e7b4d7b39c96346595fea6c39f4c81b55c986025e27b6a5f874d16319eab09022eb3d9ae7114ecbdcf688712838858f1590
+  checksum: e016ed7efb6c664eb386d6036e601fd603ad34232cb11c40c5c35fe32710cdfa55346ae33759fc1006428f6e7dcadb0a371e0907a872519cedc123779770dc67
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/nbformat@npm:4.1.8"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/nbformat@npm:4.2.0"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: 11d89ae6fb2385a00e60ab84defc61e3cf28510b029ffbe9ffe27a75bc84f85e64a0d0d16b6deb7b57256fdd651d842a0626128def511e7755121a5a0a71f078
+  checksum: adecadcb63de48f09aeb54eebfed8b77ab322c478fd903001e09780a01e7cf68f93716a2598631d4426d8ad9d3dc6349e8892db12575f74c8daea33f63b9c111
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/notebook@npm:4.1.8"
-  dependencies:
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/cells": ^4.1.8
-    "@jupyterlab/codeeditor": ^4.1.8
-    "@jupyterlab/codemirror": ^4.1.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/docregistry": ^4.1.8
-    "@jupyterlab/documentsearch": ^4.1.8
-    "@jupyterlab/lsp": ^4.1.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/settingregistry": ^4.1.8
-    "@jupyterlab/statusbar": ^4.1.8
-    "@jupyterlab/toc": ^6.1.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+"@jupyterlab/notebook@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/notebook@npm:4.2.0"
+  dependencies:
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/cells": ^4.2.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/codemirror": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/documentsearch": ^4.2.0
+    "@jupyterlab/lsp": ^4.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/settingregistry": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/toc": ^6.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: ec1044f23cbbcaa5a6d1057f2f26640630a3c31f4d2fc9930da5dc6665fcf041ab4472952f13dd863eb29a91ed3af2e8a4eee5eff2d329b381b8f0a5865f52ef
+  checksum: 2f4bcc4edde849a77b3a257c1920ca03dc666ec442acdf56e4e5acb4d4ff81231fc065cc753f07f91010e08f1c888f49d4813eaef6bc5b444f5d4d85dfb93f98
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.1.8":
-  version: 5.1.8
-  resolution: "@jupyterlab/observables@npm:5.1.8"
+"@jupyterlab/observables@npm:^5.2.0":
+  version: 5.2.0
+  resolution: "@jupyterlab/observables@npm:5.2.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: c349b4fea92ef28019c0b3f5a100abdd4384554188d6741234e90e03f3f18b343a22ea8560f9d2eea1a00d4cd9514074d195ec850e930785f28a2f8a624a0f4d
+  checksum: 98460d55d8ac559c79be87fe5e105cc200556e87276daed739fd89e8393c74ba9b03f67c8ecf7a02e8d8ee1fd8a60031ced6c1b7884ab5f10c8bdb876f150c5f
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/outputarea@npm:4.1.8"
+"@jupyterlab/outputarea@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/outputarea@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
-  checksum: deb86addc7c43794442cdec2097946be949accd081aec51029cf0c6b53e4a950be1cfd9d9621059e580b9e45255a8bf971966ae8ecebec2358579462f7396b8b
+    "@lumino/widgets": ^2.3.2
+  checksum: 79403a2a27bf608a453f907c270afd0df822b398460cf5e435fcf938111201f35a1fc298a93be7e5386d5d38f9431a90a9c451f8f1255c8169d6aea7c3391163
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.9.8":
-  version: 3.9.8
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.8"
+"@jupyterlab/rendermime-interfaces@npm:^3.10.0":
+  version: 3.10.0
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.10.0"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
-    "@lumino/widgets": ^1.37.2 || ^2.3.1
-  checksum: d08bcecdf37a48de5c22bbb5b62a4ebe756408aaa27ae18b3a99d13863e5776c861db69ee1066b2262a1a93ce59f475b549a8d56fe5bc087d4a6ba27afbc168a
+    "@lumino/widgets": ^1.37.2 || ^2.3.2
+  checksum: 08999b64a6896a4d58869ec00ca64a1b3931e01b438d471a0ad1404407f6231667f686b823a9cb482349f3d774693368320d2d4463c23fdd1de81cb4ddf34f20
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/rendermime@npm:4.1.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/translation": ^4.1.8
+"@jupyterlab/rendermime@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/rendermime@npm:4.2.0"
+  dependencies:
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     lodash.escape: ^4.0.1
-  checksum: 3c750598c212e2df43f45c32deba9d4b96dd676781e348771dd7d18c4c23e64e9bf3d25906a68be5368d898a4c81e48ff4215607c46df7934b17dc1ba672a697
+  checksum: 296eba0721a2900cb960fbdb99e98f82999e982f4332f6be8af7ccbb7055b9bcb1517a2b24e5c3b6759c722d5f06f9a68d6a61c8cb59c40855b7852a45aca2bd
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.1.8":
-  version: 7.1.8
-  resolution: "@jupyterlab/services@npm:7.1.8"
+"@jupyterlab/services@npm:^7.2.0":
+  version: 7.2.0
+  resolution: "@jupyterlab/services@npm:7.2.0"
   dependencies:
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/settingregistry": ^4.1.8
-    "@jupyterlab/statedb": ^4.1.8
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/settingregistry": ^4.2.0
+    "@jupyterlab/statedb": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: 56143631829ee1081f6ad2f03343a47d83549d2463f9c4bfddb34e4770c74cf78cbcc5f54aca5338a0d5ce4d28e9b8d8301e6e04b4fb7f66570c49d1ceaf19e5
+  checksum: edc93389913d792841b615cd0a317e16c77621cd5cb35e67c40f7a58bcf0e31c77718ae7abcf643621ba86ce78c795d6008a9413d84ecad2b42e39bd52db1447
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/settingregistry@npm:4.1.8"
+"@jupyterlab/settingregistry@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/settingregistry@npm:4.2.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.8
-    "@jupyterlab/statedb": ^4.1.8
-    "@lumino/commands": ^2.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@rjsf/utils": ^5.13.4
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: 90067142211fdaf6e9a6e0029fe1bc4c9ae05fa8e88e37f912373a0365bc8d507ef44e0bf83deb1e0bd0855a2cf05b0f541db38fafe3bc37d83422df8671e56a
+  checksum: fc60490e9e977e38b14b27a9e3896b47a28930a76a84888dd86180105b9ab6d1e68544f1184bdba72b4c5aa003cb13f10c8e5ca60685827fe6f893302483a109
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/statedb@npm:4.1.8"
+"@jupyterlab/statedb@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/statedb@npm:4.2.0"
   dependencies:
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 28983e98affec8b8d6bb8e0cbacfe2c74d1ae48af8e69fddc7f457dcd87210adf5e39dafd21bcad24cfe572f45758c7531cd8d991e9eda894e63392b544bf09d
+  checksum: 69620478aa7bf452d7440b9433b6411edef537cd7d9f72f87f70bd6fc0c8fc50003d02ab8d9d4b0746383f98cb7035b093ce5e596e6560e3c35c5a0fe434dce4
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/statusbar@npm:4.1.8"
+"@jupyterlab/statusbar@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/statusbar@npm:4.2.0"
   dependencies:
-    "@jupyterlab/ui-components": ^4.1.8
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: eb3094b9511334a82b92686ad7010763fc8c101a9631ee558462cc71d6ca3e7ad485a927e777da1f2c1aba8398c5c2d1ec65c48daae69317267944255197dbe7
+  checksum: 1ab4bfab3d6b37f0ff93ffd8b747b90ec7e532c554c8203716931923bcd97c61ad1b34c07b9973517022f022879014b57614a27f7417996697a5c97cad814c3b
   languageName: node
   linkType: hard
 
-"@jupyterlab/testing@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/testing@npm:4.1.8"
+"@jupyterlab/testing@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/testing@npm:4.2.0"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
-    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/coreutils": ^6.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    child_process: ~1.0.2
     deepmerge: ^4.2.2
     fs-extra: ^10.1.0
     identity-obj-proxy: ^3.0.0
     jest: ^29.2.0
     jest-environment-jsdom: ^29.3.0
     jest-junit: ^15.0.0
-    node-fetch: ^2.6.0
     simulate-event: ~1.4.0
     ts-jest: ^29.1.0
   peerDependencies:
     typescript: ">=4.3"
-  checksum: 8bb3e0e3ee9722fc36993fbba5252627ff9080045d1ddecc196a5df13e84b64cb1d65ded0cf567bcf275207c014a812cca4910be88f2f35fc52d91c45123d5be
+  checksum: 65ef38d488ba6cab82602d733f72e5492ba0ec9e67f8cb91d68a012e455a9abd0538962f6bfe422c4ec44954005c7da90f13851866366f45833a11107b27fb80
   languageName: node
   linkType: hard
 
 "@jupyterlab/testutils@npm:^4.0.0":
-  version: 4.1.8
-  resolution: "@jupyterlab/testutils@npm:4.1.8"
+  version: 4.2.0
+  resolution: "@jupyterlab/testutils@npm:4.2.0"
   dependencies:
-    "@jupyterlab/application": ^4.1.8
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/notebook": ^4.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/testing": ^4.1.8
-  checksum: efabbdd60565a76cf7c17ef05ae73956f5955bbe943430c64ff9985677cadbfdc35eb79f20ea5e4ae5227fdcb397e8920a71e8b0f9b60a5c31dc6a9a4815fa11
+    "@jupyterlab/application": ^4.2.0
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/notebook": ^4.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/testing": ^4.2.0
+  checksum: e8ba4a3db75e014932b2bf48283a49bb587ef8acf9bc6c283a3f9da0c0557cfbe3dab0241da2dd1203ff3bbd2f0be71da7271c8164babfcae6d750c4bf9389de
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.1.8":
-  version: 6.1.8
-  resolution: "@jupyterlab/toc@npm:6.1.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.8
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/docregistry": ^4.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime": ^4.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/translation": ^4.1.8
-    "@jupyterlab/ui-components": ^4.1.8
+"@jupyterlab/toc@npm:^6.2.0":
+  version: 6.2.0
+  resolution: "@jupyterlab/toc@npm:6.2.0"
+  dependencies:
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 6dadf19c32fadeccc19df6ba31287c929a7a09ac41ecaf53fbc88471d4c62a16193555c3fb391ecc4e495c9f6cdde7d0519c77ed0b69fbc90da9e5b16bb924d3
+  checksum: 68906012ba858d33587ce28e7a9785af4ff61cf119ed34bdfaceb48201ba56a941e2df0d722cb48f5ae2b541397fc7cea79509c388c762dccff20916d5dfdc2b
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/translation@npm:4.1.8"
+"@jupyterlab/translation@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/translation@npm:4.2.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/services": ^7.1.8
-    "@jupyterlab/statedb": ^4.1.8
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
     "@lumino/coreutils": ^2.1.2
-  checksum: 7de872e52ffa0d2e4579c26b906ae7f98fcab6767ff85a4ce157f70be26d9edcf3410e94931ea9c8c1a1c48f4fc5f5e410b396761164dc8314ec1157314bcb9e
+  checksum: 0b2d4d3827946bf5b12db5e98356d15dc7721279bb791a46f2927b20b49b597fd717b0d24b84ae4c7b96540f99a0eed82ba0609c186675daf80b343df9792a21
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/ui-components@npm:4.1.8"
+"@jupyterlab/ui-components@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/ui-components@npm:4.2.0"
   dependencies:
-    "@jupyter/react-components": ^0.15.2
-    "@jupyter/web-components": ^0.15.2
-    "@jupyterlab/coreutils": ^6.1.8
-    "@jupyterlab/observables": ^5.1.8
-    "@jupyterlab/rendermime-interfaces": ^3.9.8
-    "@jupyterlab/translation": ^4.1.8
+    "@jupyter/react-components": ^0.15.3
+    "@jupyter/web-components": ^0.15.3
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     "@rjsf/core": ^5.13.4
     "@rjsf/utils": ^5.13.4
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: 6a95597b8c71cd31b3f7a39cc61dc094fc6fede5b0b6bac61ff9df0a5757542d419e653f3a2527a15cb0dc9e7b7fcd2568101e9063878ce260f6adb486787e69
+  checksum: 9352c9d5d4df2671999a79bcc0434c50731bc78e89b5d94cfcf1e91f55fb14dbe4670576f49b8c53f9c7bb3995e72455c9062ad6953411c188c8bb85edee0a00
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
   version: 1.2.1
   resolution: "@lezer/common@npm:1.2.1"
   checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
@@ -2727,27 +2728,27 @@
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 1f5968360dbac7ba27f0c2a194143769f7b01824715274dd8507dacf13cc790bb8c48ce95de355e9c58be93bb3e271bf98b9fc51213f79e4ce918e7c7ebbef04
   languageName: node
   linkType: hard
 
-"@lezer/generator@npm:^1.2.2":
+"@lezer/generator@npm:^1.7.0":
   version: 1.7.0
   resolution: "@lezer/generator@npm:1.7.0"
   dependencies:
     "@lezer/common": ^1.1.0
     "@lezer/lr": ^1.3.0
   bin:
     lezer-generator: src/lezer-generator.cjs
   checksum: 69f4c6625446cb65adaa509480ec67502f27651707a8e45e99373e682d7f66f8842205669f174bcb138eade72c64ded0b54d6de6aa5af995ac1f1e805ef021fd
   languageName: node
   linkType: hard
 
-"@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
+"@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.2.0":
   version: 1.2.0
   resolution: "@lezer/highlight@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
@@ -2771,21 +2772,21 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 752e8c9b99cccf022669a702016e0c3a793d8326e043b1d053159f5de4d222cd188e8e31e1427cbe6a8ed8e53de3977ab551c64cbd5a76a12eb3a1da5e18b6a5
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.15
-  resolution: "@lezer/javascript@npm:1.4.15"
+  version: 1.4.16
+  resolution: "@lezer/javascript@npm:1.4.16"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: e0322ec70231a1beb6652f0883d62371297f37783a774ad011a3c7d4acaf066f4bcd6c0b83b34cef0893766ae730ab29efee7a11d67d66e8c5f8d4dea3c46172
+  checksum: 20fcf5ad95d3cf0155af8a060045d1c14609e1178669e087f246854d1ef7e7326e512cc05f90db1bcbd58ce229fcc7aa8600c7f757580c5f980c420835a2cd3c
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/json@npm:1.0.2"
   dependencies:
@@ -2801,15 +2802,15 @@
   resolution: "@lezer/lr@npm:1.4.0"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 4c8517017e9803415c6c5cb8230d8764107eafd7d0b847676cd1023abb863a4b268d0d01c7ce3cf1702c4749527c68f0a26b07c329cb7b68c36ed88362d7b193
   languageName: node
   linkType: hard
 
-"@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
+"@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.2.0":
   version: 1.3.0
   resolution: "@lezer/markdown@npm:1.3.0"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
   checksum: 13eb2720e4cb84278349bad8af116f748813094f99fad02680010c3a8c5985e0358c344487990f87a31ef0d6c1a2be582301f914c0e4a6e9cfa22647b6cd6545
   languageName: node
@@ -2862,15 +2863,15 @@
 "@lumino/algorithm@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/algorithm@npm:2.0.1"
   checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^2.3.0":
+"@lumino/application@npm:^2.3.1":
   version: 2.3.1
   resolution: "@lumino/application@npm:2.3.1"
   dependencies:
     "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/widgets": ^2.3.2
   checksum: c112789d99baf62e5c2cee98834bc3efb5027bbca1aac81f10ea8855c0cd2538ec0a7c56c3f5dd42dce244e6892ef5bf8ef356f97e1cd4c161b99eb2068c195c
@@ -2882,15 +2883,15 @@
   resolution: "@lumino/collections@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.2.0, @lumino/commands@npm:^2.3.0":
+"@lumino/commands@npm:^2.3.0":
   version: 2.3.0
   resolution: "@lumino/commands@npm:2.3.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
@@ -2984,15 +2985,15 @@
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^2.3.1, @lumino/widgets@npm:^2.3.2":
+"@lumino/widgets@npm:^1.37.2 || ^2.3.2, @lumino/widgets@npm:^2.3.2":
   version: 2.3.2
   resolution: "@lumino/widgets@npm:2.3.2"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
@@ -3091,57 +3092,57 @@
     lru-cache: ^10.0.1
     socks-proxy-agent: ^8.0.3
   checksum: 67de7b88cc627a79743c88bab35e023e23daf13831a8aa4e15f998b92f5507b644d8ffc3788afc8e64423c612e0785a6a92b74782ce368f49a6746084b50d874
   languageName: node
   linkType: hard
 
 "@npmcli/fs@npm:^3.1.0":
-  version: 3.1.0
-  resolution: "@npmcli/fs@npm:3.1.0"
+  version: 3.1.1
+  resolution: "@npmcli/fs@npm:3.1.1"
   dependencies:
     semver: ^7.3.5
-  checksum: a50a6818de5fc557d0b0e6f50ec780a7a02ab8ad07e5ac8b16bf519e0ad60a144ac64f97d05c443c3367235d337182e1d012bbac0eb8dbae8dc7b40b193efd0e
+  checksum: d960cab4b93adcb31ce223bfb75c5714edbd55747342efb67dcc2f25e023d930a7af6ece3e75f2f459b6f38fc14d031c766f116cd124fdc937fd33112579e820
   languageName: node
   linkType: hard
 
 "@pkgjs/parseargs@npm:^0.11.0":
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.13.4":
-  version: 5.18.3
-  resolution: "@rjsf/core@npm:5.18.3"
+  version: 5.18.4
+  resolution: "@rjsf/core@npm:5.18.4"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.4.1
     nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
     "@rjsf/utils": ^5.18.x
     react: ^16.14.0 || >=17
-  checksum: 370586a38e6557367281cd3e6292abf4391a24ed3d7c19b02478a45ca5aeb337363f54d841a7077b1403a24014bb1969d568976f12220b3ccd1a076ed4875397
+  checksum: 8c3f49914be396595ce67dc4c36ac25c5cb6673917ec82c47f79321f5bb78d02741e8dca39287d0435270e7c9ccb06f7d40e396bdf71a3e9eb1371ef16954817
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.13.4":
-  version: 5.18.3
-  resolution: "@rjsf/utils@npm:5.18.3"
+  version: 5.18.4
+  resolution: "@rjsf/utils@npm:5.18.4"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 36f6574836e8ccad27b8215f940cb86b1a02939d325e0223a8d8e70b9ae65245e6649dd4835a40e628153f26d961a5cfbdd6c0bdd7b70a80f7cb1911357f78ff
+  checksum: d7cf514527ec50a94751c5ec1f9e5eafd89d0c56441a22ae28a4e667aaa7c60447e1e1ccf8355c5be5b97e9a1163853c116816b13307e3463433d50f6b89bb3e
   languageName: node
   linkType: hard
 
 "@sinclair/typebox@npm:^0.27.8":
   version: 0.27.8
   resolution: "@sinclair/typebox@npm:0.27.8"
   checksum: 00bd7362a3439021aa1ea51b0e0d0a0e8ca1351a3d54c606b115fdcc49b51b16db6e5f43b4fe7a28c38688523e22a94d49dd31168868b655f0d4d50f032d07a1
@@ -3307,19 +3308,19 @@
   version: 1.2.5
   resolution: "@types/minimist@npm:1.2.5"
   checksum: 477047b606005058ab0263c4f58097136268007f320003c348794f74adedc3166ffc47c80ec3e94687787f2ab7f4e72c468223946e79892cf0fd9e25e9970a90
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.12.7
-  resolution: "@types/node@npm:20.12.7"
+  version: 20.12.12
+  resolution: "@types/node@npm:20.12.12"
   dependencies:
     undici-types: ~5.26.4
-  checksum: 7cc979f7e2ca9a339ec71318c3901b9978555257929ef3666987f3e447123bc6dc92afcc89f6347e09e07d602fde7d51bcddea626c23aa2bb74aeaacfd1e1686
+  checksum: 5373983874b9af7c216e7ca5d26b32a8d9829c703a69f1e66f2113598b5be8582c0e009ca97369f1ec9a6282b3f92812208d06eb1e9fc3bd9b939b022303d042
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.4
   resolution: "@types/normalize-package-data@npm:2.4.4"
   checksum: 65dff72b543997b7be8b0265eca7ace0e34b75c3e5fee31de11179d08fa7124a7a5587265d53d0409532ecb7f7fba662c2012807963e1f9b059653ec2c83ee05
@@ -3337,20 +3338,20 @@
   version: 15.7.12
   resolution: "@types/prop-types@npm:15.7.12"
   checksum: ac16cc3d0a84431ffa5cfdf89579ad1e2269549f32ce0c769321fdd078f84db4fbe1b461ed5a1a496caf09e637c0e367d600c541435716a55b1d9713f5035dfe
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.3.1
-  resolution: "@types/react@npm:18.3.1"
+  version: 18.3.2
+  resolution: "@types/react@npm:18.3.2"
   dependencies:
     "@types/prop-types": "*"
     csstype: ^3.0.2
-  checksum: 9224ef319a0c2b7f66e7e7f06012aa5eb638a6c76c9742843eab1a5d243f2bed5ff829ddbb41efd60d33a266420528adfcb84cb93f238b00e905f98c3a355768
+  checksum: d0b8b9d0ede6cd28dbbe34106d914b5e3652d9d7aa9d0f32fe6171506b6fc7c826d9d6571642976a5422bd29c5022fd893a710ed59a1177a0c1df8e02cf17ffe
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.3.12":
   version: 7.5.8
   resolution: "@types/semver@npm:7.5.8"
   checksum: ea6f5276f5b84c55921785a3a27a3cd37afee0111dfe2bcb3e03c31819c197c782598f17f0b150a69d453c9584cd14c4c4d7b9a55d2c5e6cacd4d66fdb3b3663
@@ -3860,22 +3861,22 @@
     json-schema-traverse: ^0.4.1
     uri-js: ^4.2.2
   checksum: 874972efe5c4202ab0a68379481fbd3d1b5d0a7bd6d3cc21d40d3536ebff3352a2a1fabb632d4fd2cc7fe4cbdcd5ed6782084c9bbf7f32a1536d18f9da5007d4
   languageName: node
   linkType: hard
 
 "ajv@npm:^8.0.0, ajv@npm:^8.0.1, ajv@npm:^8.12.0, ajv@npm:^8.9.0":
-  version: 8.12.0
-  resolution: "ajv@npm:8.12.0"
+  version: 8.13.0
+  resolution: "ajv@npm:8.13.0"
   dependencies:
-    fast-deep-equal: ^3.1.1
+    fast-deep-equal: ^3.1.3
     json-schema-traverse: ^1.0.0
     require-from-string: ^2.0.2
-    uri-js: ^4.2.2
-  checksum: 4dc13714e316e67537c8b31bc063f99a1d9d9a497eb4bbd55191ac0dcd5e4985bbb71570352ad6f1e76684fb6d790928f96ba3b2d4fd6e10024be9612fe3f001
+    uri-js: ^4.4.1
+  checksum: 6de82d0b2073e645ca3300561356ddda0234f39b35d2125a8700b650509b296f41c00ab69f53178bbe25ad688bd6ac3747ab44101f2f4bd245952e8fd6ccc3c1
   languageName: node
   linkType: hard
 
 "ansi-escapes@npm:^4.2.1":
   version: 4.3.2
   resolution: "ansi-escapes@npm:4.3.2"
   dependencies:
@@ -4167,20 +4168,20 @@
   resolution: "brace-expansion@npm:2.0.1"
   dependencies:
     balanced-match: ^1.0.0
   checksum: a61e7cd2e8a8505e9f0036b3b6108ba5e926b4b55089eeb5550cd04a471fe216c96d4fe7e4c7f995c728c554ae20ddfc4244cad10aef255e72b62930afd233d1
   languageName: node
   linkType: hard
 
-"braces@npm:^3.0.2":
-  version: 3.0.2
-  resolution: "braces@npm:3.0.2"
+"braces@npm:^3.0.3":
+  version: 3.0.3
+  resolution: "braces@npm:3.0.3"
   dependencies:
-    fill-range: ^7.0.1
-  checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
+    fill-range: ^7.1.1
+  checksum: b95aa0b3bd909f6cd1720ffcf031aeaf46154dd88b4da01f9a1d3f7ea866a79eba76a6d01cbc3c422b2ee5cdc39a4f02491058d5df0d7bf6e6a162a832df1f69
   languageName: node
   linkType: hard
 
 "browserslist@npm:^4.21.10, browserslist@npm:^4.22.2, browserslist@npm:^4.23.0":
   version: 4.23.0
   resolution: "browserslist@npm:4.23.0"
   dependencies:
@@ -4216,30 +4217,30 @@
   version: 1.1.2
   resolution: "buffer-from@npm:1.1.2"
   checksum: 0448524a562b37d4d7ed9efd91685a5b77a50672c556ea254ac9a6d30e3403a517d8981f10e565db24e8339413b43c97ca2951f10e399c6125a0d8911f5679bb
   languageName: node
   linkType: hard
 
 "cacache@npm:^18.0.0":
-  version: 18.0.2
-  resolution: "cacache@npm:18.0.2"
+  version: 18.0.3
+  resolution: "cacache@npm:18.0.3"
   dependencies:
     "@npmcli/fs": ^3.1.0
     fs-minipass: ^3.0.0
     glob: ^10.2.2
     lru-cache: ^10.0.1
     minipass: ^7.0.3
     minipass-collect: ^2.0.1
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     p-map: ^4.0.0
     ssri: ^10.0.0
     tar: ^6.1.11
     unique-filename: ^3.0.0
-  checksum: 0250df80e1ad0c828c956744850c5f742c24244e9deb5b7dc81bca90f8c10e011e132ecc58b64497cc1cad9a98968676147fb6575f4f94722f7619757b17a11b
+  checksum: b717fd9b36e9c3279bfde4545c3a8f6d5a539b084ee26a9504d48f83694beb724057d26e090b97540f9cc62bea18b9f6cf671c50e18fb7dac60eda9db691714f
   languageName: node
   linkType: hard
 
 "call-bind@npm:^1.0.2, call-bind@npm:^1.0.5, call-bind@npm:^1.0.6, call-bind@npm:^1.0.7":
   version: 1.0.7
   resolution: "call-bind@npm:1.0.7"
   dependencies:
@@ -4281,17 +4282,17 @@
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001587":
-  version: 1.0.30001614
-  resolution: "caniuse-lite@npm:1.0.30001614"
-  checksum: 1b695625f9a1b08584c3c229d4b8deaebb89e7901a2a2ffe599a6250c0a79fc61afc49c374c32a76dbf593a5dedac3229bb0140bbacd438276211bdd1d7c4958
+  version: 1.0.30001620
+  resolution: "caniuse-lite@npm:1.0.30001620"
+  checksum: 1831e519c29ce6971bc50d56bab196a307fcb4181e7deaa80df314b035b87b3912b8626b4e87adc301d0bfe6a90b99814101b1cb28114b96e720f996f19bdc0d
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.3.0, chalk@npm:^2.4.1, chalk@npm:^2.4.2":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -4315,21 +4316,14 @@
 "char-regex@npm:^1.0.2":
   version: 1.0.2
   resolution: "char-regex@npm:1.0.2"
   checksum: b563e4b6039b15213114626621e7a3d12f31008bdce20f9c741d69987f62aeaace7ec30f6018890ad77b2e9b4d95324c9f5acfca58a9441e3b1dcdd1e2525d17
   languageName: node
   linkType: hard
 
-"child_process@npm:~1.0.2":
-  version: 1.0.2
-  resolution: "child_process@npm:1.0.2"
-  checksum: bd814d82bc8c6e85ed6fb157878978121cd03b5296c09f6135fa3d081fd9a6a617a6d509c50397711df713af403331241a9c0397a7fad30672051485e156c2a1
-  languageName: node
-  linkType: hard
-
 "chownr@npm:^2.0.0":
   version: 2.0.0
   resolution: "chownr@npm:2.0.0"
   checksum: c57cf9dd0791e2f18a5ee9c1a299ae6e801ff58fee96dc8bfd0dcb4738a6ce58dd252a3605b1c93c6418fe4f9d5093b28ffbf4d66648cb2a9c67eaef9679be2f
   languageName: node
   linkType: hard
 
@@ -4507,19 +4501,19 @@
   version: 2.0.0
   resolution: "convert-source-map@npm:2.0.0"
   checksum: 63ae9933be5a2b8d4509daca5124e20c14d023c820258e484e32dc324d34c2754e71297c94a05784064ad27615037ef677e3f0c00469fb55f409d2bb21261035
   languageName: node
   linkType: hard
 
 "core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.36.1":
-  version: 3.37.0
-  resolution: "core-js-compat@npm:3.37.0"
+  version: 3.37.1
+  resolution: "core-js-compat@npm:3.37.1"
   dependencies:
     browserslist: ^4.23.0
-  checksum: cab5078e98625f889fd9bbbb19e84cb408f31c87e68302d380db0d26ae8e35c1b38cde084358ff345d4aa461af5f3c60d8a913a5b30bff3a83b4b7859374db36
+  checksum: 5e7430329358bced08c30950512d2081aea0a5652b4c5892cbb3c4a6db05b0d3893a191a955162a07fdb5f4fe74e61b6429fdb503f54e062336d76e43c9555d9
   languageName: node
   linkType: hard
 
 "cosmiconfig@npm:^7.1.0":
   version: 7.1.0
   resolution: "cosmiconfig@npm:7.1.0"
   dependencies:
@@ -4781,15 +4775,15 @@
     es-define-property: ^1.0.0
     es-errors: ^1.3.0
     gopd: ^1.0.1
   checksum: 8068ee6cab694d409ac25936eb861eea704b7763f7f342adbdfe337fc27c78d7ae0eff2364b2917b58c508d723c7a074326d068eef2e45c4edcd85cf94d0313b
   languageName: node
   linkType: hard
 
-"define-properties@npm:^1.1.3, define-properties@npm:^1.2.0, define-properties@npm:^1.2.1":
+"define-properties@npm:^1.2.0, define-properties@npm:^1.2.1":
   version: 1.2.1
   resolution: "define-properties@npm:1.2.1"
   dependencies:
     define-data-property: ^1.0.1
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
   checksum: b4ccd00597dd46cb2d4a379398f5b19fca84a16f3374e2249201992f36b30f6835949a9429669ee6b41b6e837205a163eadd745e472069e70dfc10f03e5fcc12
@@ -4831,26 +4825,26 @@
   resolution: "doctrine@npm:3.0.0"
   dependencies:
     esutils: ^2.0.2
   checksum: fd7673ca77fe26cd5cba38d816bc72d641f500f1f9b25b83e8ce28827fe2da7ad583a8da26ab6af85f834138cf8dae9f69b0cd6ab925f52ddab1754db44d99ce
   languageName: node
   linkType: hard
 
-"dom-serializer@npm:^1.0.1":
-  version: 1.4.1
-  resolution: "dom-serializer@npm:1.4.1"
+"dom-serializer@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "dom-serializer@npm:2.0.0"
   dependencies:
-    domelementtype: ^2.0.1
-    domhandler: ^4.2.0
-    entities: ^2.0.0
-  checksum: fbb0b01f87a8a2d18e6e5a388ad0f7ec4a5c05c06d219377da1abc7bb0f674d804f4a8a94e3f71ff15f6cb7dcfc75704a54b261db672b9b3ab03da6b758b0b22
+    domelementtype: ^2.3.0
+    domhandler: ^5.0.2
+    entities: ^4.2.0
+  checksum: cd1810544fd8cdfbd51fa2c0c1128ec3a13ba92f14e61b7650b5de421b88205fd2e3f0cc6ace82f13334114addb90ed1c2f23074a51770a8e9c1273acbc7f3e6
   languageName: node
   linkType: hard
 
-"domelementtype@npm:^2.0.1, domelementtype@npm:^2.2.0":
+"domelementtype@npm:^2.3.0":
   version: 2.3.0
   resolution: "domelementtype@npm:2.3.0"
   checksum: ee837a318ff702622f383409d1f5b25dd1024b692ef64d3096ff702e26339f8e345820f29a68bcdcea8cfee3531776b3382651232fbeae95612d6f0a75efb4f6
   languageName: node
   linkType: hard
 
 "domexception@npm:^4.0.0":
@@ -4858,31 +4852,31 @@
   resolution: "domexception@npm:4.0.0"
   dependencies:
     webidl-conversions: ^7.0.0
   checksum: ddbc1268edf33a8ba02ccc596735ede80375ee0cf124b30d2f05df5b464ba78ef4f49889b6391df4a04954e63d42d5631c7fcf8b1c4f12bc531252977a5f13d5
   languageName: node
   linkType: hard
 
-"domhandler@npm:^4.0.0, domhandler@npm:^4.2.0":
-  version: 4.3.1
-  resolution: "domhandler@npm:4.3.1"
+"domhandler@npm:^5.0.2, domhandler@npm:^5.0.3":
+  version: 5.0.3
+  resolution: "domhandler@npm:5.0.3"
   dependencies:
-    domelementtype: ^2.2.0
-  checksum: 4c665ceed016e1911bf7d1dadc09dc888090b64dee7851cccd2fcf5442747ec39c647bb1cb8c8919f8bbdd0f0c625a6bafeeed4b2d656bbecdbae893f43ffaaa
+    domelementtype: ^2.3.0
+  checksum: 0f58f4a6af63e6f3a4320aa446d28b5790a009018707bce2859dcb1d21144c7876482b5188395a188dfa974238c019e0a1e610d2fc269a12b2c192ea2b0b131c
   languageName: node
   linkType: hard
 
-"domutils@npm:^2.5.2":
-  version: 2.8.0
-  resolution: "domutils@npm:2.8.0"
+"domutils@npm:^3.0.1":
+  version: 3.1.0
+  resolution: "domutils@npm:3.1.0"
   dependencies:
-    dom-serializer: ^1.0.1
-    domelementtype: ^2.2.0
-    domhandler: ^4.2.0
-  checksum: abf7434315283e9aadc2a24bac0e00eab07ae4313b40cc239f89d84d7315ebdfd2fb1b5bf750a96bc1b4403d7237c7b2ebf60459be394d625ead4ca89b934391
+    dom-serializer: ^2.0.0
+    domelementtype: ^2.3.0
+    domhandler: ^5.0.3
+  checksum: e5757456ddd173caa411cfc02c2bb64133c65546d2c4081381a3bafc8a57411a41eed70494551aa58030be9e58574fcc489828bebd673863d39924fb4878f416
   languageName: node
   linkType: hard
 
 "duplicate-package-checker-webpack-plugin@npm:^3.0.0":
   version: 3.0.0
   resolution: "duplicate-package-checker-webpack-plugin@npm:3.0.0"
   dependencies:
@@ -4898,17 +4892,17 @@
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.668":
-  version: 1.4.751
-  resolution: "electron-to-chromium@npm:1.4.751"
-  checksum: 7d8fce48b7b9997eee6bbef136044702f3fcf959a05a143e8818e4f36106024df86ed6e3aaaf83455cd1d83f5f180c8281c7cef645b798cd7a9424b2847ca15d
+  version: 1.4.777
+  resolution: "electron-to-chromium@npm:1.4.777"
+  checksum: e4a53b204003b36e1c6453ec83f260251df45d475840e2e390a94f7e8873ce5b790e719b2fbf72aa42e1b8d75247706428593bc7c0156c5ce2f9adc9ad714b84
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -4942,31 +4936,24 @@
   dependencies:
     iconv-lite: ^0.6.2
   checksum: bb98632f8ffa823996e508ce6a58ffcf5856330fde839ae42c9e1f436cc3b5cc651d4aeae72222916545428e54fd0f6aa8862fd8d25bdbcc4589f1e3f3715e7f
   languageName: node
   linkType: hard
 
 "enhanced-resolve@npm:^5.16.0":
-  version: 5.16.0
-  resolution: "enhanced-resolve@npm:5.16.0"
+  version: 5.16.1
+  resolution: "enhanced-resolve@npm:5.16.1"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: ccfd01850ecf2aa51e8554d539973319ff7d8a539ef1e0ba3460a0ccad6223c4ef6e19165ee64161b459cd8a48df10f52af4434c60023c65fde6afa32d475f7e
-  languageName: node
-  linkType: hard
-
-"entities@npm:^2.0.0":
-  version: 2.2.0
-  resolution: "entities@npm:2.2.0"
-  checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
+  checksum: 6e4c166fef72ef231455f9119686d93ecccb11874f8256d73a42de5b293cb2536050849382468864b25973514ca4fa4cb13c37be2ff857a211e2aca3ff05bb6c
   languageName: node
   linkType: hard
 
-"entities@npm:^4.4.0":
+"entities@npm:^4.2.0, entities@npm:^4.4.0":
   version: 4.5.0
   resolution: "entities@npm:4.5.0"
   checksum: 853f8ebd5b425d350bffa97dd6958143179a5938352ccae092c62d1267c4e392a039be1bae7d51b6e4ffad25f51f9617531fedf5237f15df302ccfb452cbf2d7
   languageName: node
   linkType: hard
 
 "env-paths@npm:^2.2.0":
@@ -5068,17 +5055,17 @@
   version: 1.3.0
   resolution: "es-errors@npm:1.3.0"
   checksum: ec1414527a0ccacd7f15f4a3bc66e215f04f595ba23ca75cdae0927af099b5ec865f9f4d33e9d7e86f512f252876ac77d4281a7871531a50678132429b1271b5
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^1.2.1":
-  version: 1.5.2
-  resolution: "es-module-lexer@npm:1.5.2"
-  checksum: 59c47109eca80b93dda2418337b4308c194c578704dc57d5aa54973b196e378d31e92f258e5525655b99b3de8a84dda2debb9646cddf6fe8830f1bfca95ee060
+  version: 1.5.3
+  resolution: "es-module-lexer@npm:1.5.3"
+  checksum: 2e0a0936fb49ca072d438128f588d5b46974035f7a1362bdb26447868016243cfd1c5ec8f12e80d273749e8c603f5aba5a828d5c2d95c07f61fbe77ab4fce4af
   languageName: node
   linkType: hard
 
 "es-object-atoms@npm:^1.0.0":
   version: 1.0.0
   resolution: "es-object-atoms@npm:1.0.0"
   dependencies:
@@ -5105,15 +5092,15 @@
     is-callable: ^1.1.4
     is-date-object: ^1.0.1
     is-symbol: ^1.0.2
   checksum: 4ead6671a2c1402619bdd77f3503991232ca15e17e46222b0a41a5d81aebc8740a77822f5b3c965008e631153e9ef0580540007744521e72de8e33599fca2eed
   languageName: node
   linkType: hard
 
-"escalade@npm:^3.1.1":
+"escalade@npm:^3.1.1, escalade@npm:^3.1.2":
   version: 3.1.2
   resolution: "escalade@npm:3.1.2"
   checksum: 1ec0977aa2772075493002bdbd549d595ff6e9393b1cb0d7d6fcaf78c750da0c158f180938365486f75cb69fba20294351caddfce1b46552a7b6c3cde52eaa02
   languageName: node
   linkType: hard
 
 "escape-string-regexp@npm:^1.0.5":
@@ -5452,20 +5439,20 @@
   resolution: "file-entry-cache@npm:6.0.1"
   dependencies:
     flat-cache: ^3.0.4
   checksum: f49701feaa6314c8127c3c2f6173cfefff17612f5ed2daaafc6da13b5c91fd43e3b2a58fd0d63f9f94478a501b167615931e7200e31485e320f74a33885a9c74
   languageName: node
   linkType: hard
 
-"fill-range@npm:^7.0.1":
-  version: 7.0.1
-  resolution: "fill-range@npm:7.0.1"
+"fill-range@npm:^7.1.1":
+  version: 7.1.1
+  resolution: "fill-range@npm:7.1.1"
   dependencies:
     to-regex-range: ^5.0.1
-  checksum: cc283f4e65b504259e64fd969bcf4def4eb08d85565e906b7d36516e87819db52029a76b6363d0f02d0d532f0033c9603b9e2d943d56ee3b0d4f7ad3328ff917
+  checksum: b4abfbca3839a3d55e4ae5ec62e131e2e356bf4859ce8480c64c4876100f4df292a63e5bb1618e1d7460282ca2b305653064f01654474aa35c68000980f17798
   languageName: node
   linkType: hard
 
 "find-root@npm:^1.0.0":
   version: 1.1.0
   resolution: "find-root@npm:1.1.0"
   checksum: b2a59fe4b6c932eef36c45a048ae8f93c85640212ebe8363164814990ee20f154197505965f3f4f102efc33bfb1cbc26fd17c4a2fc739ebc51b886b137cbefaf
@@ -5711,25 +5698,25 @@
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
 "glob@npm:^10.2.2, glob@npm:^10.3.10":
-  version: 10.3.12
-  resolution: "glob@npm:10.3.12"
+  version: 10.3.16
+  resolution: "glob@npm:10.3.16"
   dependencies:
     foreground-child: ^3.1.0
-    jackspeak: ^2.3.6
+    jackspeak: ^3.1.2
     minimatch: ^9.0.1
     minipass: ^7.0.4
-    path-scurry: ^1.10.2
+    path-scurry: ^1.11.0
   bin:
     glob: dist/esm/bin.mjs
-  checksum: 2b0949d6363021aaa561b108ac317bf5a97271b8a5d7a5fac1a176e40e8068ecdcccc992f8a7e958593d501103ac06d673de92adc1efcbdab45edefe35f8d7c6
+  checksum: 3cc49a0700fde72a1669ed587d167bb6921e23cd43fa3f03729794df6719a4188e0a5f3520a6d27b7762bd6b634a275fa6f400298b1559633d2e51bab8096c2e
   languageName: node
   linkType: hard
 
 "glob@npm:^7.1.3, glob@npm:^7.1.4":
   version: 7.2.3
   resolution: "glob@npm:7.2.3"
   dependencies:
@@ -5802,19 +5789,20 @@
   dependencies:
     type-fest: ^0.20.2
   checksum: 56066ef058f6867c04ff203b8a44c15b038346a62efbc3060052a1016be9f56f4cf0b2cd45b74b22b81e521a889fc7786c73691b0549c2f3a6e825b3d394f43c
   languageName: node
   linkType: hard
 
 "globalthis@npm:^1.0.3":
-  version: 1.0.3
-  resolution: "globalthis@npm:1.0.3"
+  version: 1.0.4
+  resolution: "globalthis@npm:1.0.4"
   dependencies:
-    define-properties: ^1.1.3
-  checksum: fbd7d760dc464c886d0196166d92e5ffb4c84d0730846d6621a39fbbc068aeeb9c8d1421ad330e94b7bca4bb4ea092f5f21f3d36077812af5d098b4dc006c998
+    define-properties: ^1.2.1
+    gopd: ^1.0.1
+  checksum: 39ad667ad9f01476474633a1834a70842041f70a55571e8dcef5fb957980a92da5022db5430fca8aecc5d47704ae30618c0bc877a579c70710c904e9ef06108a
   languageName: node
   linkType: hard
 
 "globby@npm:^11.1.0":
   version: 11.1.0
   resolution: "globby@npm:11.1.0"
   dependencies:
@@ -5979,23 +5967,23 @@
 "html-tags@npm:^3.2.0":
   version: 3.3.1
   resolution: "html-tags@npm:3.3.1"
   checksum: b4ef1d5a76b678e43cce46e3783d563607b1d550cab30b4f511211564574770aa8c658a400b100e588bc60b8234e59b35ff72c7851cc28f3b5403b13a2c6cbce
   languageName: node
   linkType: hard
 
-"htmlparser2@npm:^6.0.0":
-  version: 6.1.0
-  resolution: "htmlparser2@npm:6.1.0"
+"htmlparser2@npm:^8.0.0":
+  version: 8.0.2
+  resolution: "htmlparser2@npm:8.0.2"
   dependencies:
-    domelementtype: ^2.0.1
-    domhandler: ^4.0.0
-    domutils: ^2.5.2
-    entities: ^2.0.0
-  checksum: 81a7b3d9c3bb9acb568a02fc9b1b81ffbfa55eae7f1c41ae0bf840006d1dbf54cb3aa245b2553e2c94db674840a9f0fdad7027c9a9d01a062065314039058c4e
+    domelementtype: ^2.3.0
+    domhandler: ^5.0.3
+    domutils: ^3.0.1
+    entities: ^4.4.0
+  checksum: 29167a0f9282f181da8a6d0311b76820c8a59bc9e3c87009e21968264c2987d2723d6fde5a964d4b7b6cba663fca96ffb373c06d8223a85f52a6089ced942700
   languageName: node
   linkType: hard
 
 "http-cache-semantics@npm:^4.1.1":
   version: 4.1.1
   resolution: "http-cache-semantics@npm:4.1.1"
   checksum: 83ac0bc60b17a3a36f9953e7be55e5c8f41acc61b22583060e8dedc9dd5e3607c823a88d0926f9150e571f90946835c7fe150732801010845c72cd8bbff1a236
@@ -6504,24 +6492,24 @@
   dependencies:
     html-escaper: ^2.0.0
     istanbul-lib-report: ^3.0.0
   checksum: 2072db6e07bfbb4d0eb30e2700250636182398c1af811aea5032acb219d2080f7586923c09fa194029efd6b92361afb3dcbe1ebcc3ee6651d13340f7c6c4ed95
   languageName: node
   linkType: hard
 
-"jackspeak@npm:^2.3.6":
-  version: 2.3.6
-  resolution: "jackspeak@npm:2.3.6"
+"jackspeak@npm:^3.1.2":
+  version: 3.1.2
+  resolution: "jackspeak@npm:3.1.2"
   dependencies:
     "@isaacs/cliui": ^8.0.2
     "@pkgjs/parseargs": ^0.11.0
   dependenciesMeta:
     "@pkgjs/parseargs":
       optional: true
-  checksum: 57d43ad11eadc98cdfe7496612f6bbb5255ea69fe51ea431162db302c2a11011642f50cfad57288bd0aea78384a0612b16e131944ad8ecd09d619041c8531b54
+  checksum: 134276d5f785c518930701a0dcba1f3b0e9ce3e5b1c3e300898e2ae0bbd9b5195088b77252bf2110768de072c426e9e39f47e13912b0b002da4a3f4ff6e16eac
   languageName: node
   linkType: hard
 
 "jest-changed-files@npm:^29.7.0":
   version: 29.7.0
   resolution: "jest-changed-files@npm:29.7.0"
   dependencies:
@@ -7266,23 +7254,23 @@
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
 "lib0@npm:^0.2.85, lib0@npm:^0.2.86":
-  version: 0.2.93
-  resolution: "lib0@npm:0.2.93"
+  version: 0.2.94
+  resolution: "lib0@npm:0.2.94"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
     0ecdsa-generate-keypair: bin/0ecdsa-generate-keypair.js
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: 4c482aba249c471316fdec360ee4ace2a70ae42faad5fb6862aebb6786e187de9470eb082a5675489c59ffe54b005a15711a3d7dba33764bcab56349e61a1520
+  checksum: b091c7b39875a58d92ae6dcb014a42b56caf1336e03d310403c47a2fcea079eba92ffb43da90eaff9d010f08bcd20de35fffed7c655c83312ff4e3477f5dc261
   languageName: node
   linkType: hard
 
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
@@ -7455,29 +7443,30 @@
   version: 1.3.6
   resolution: "make-error@npm:1.3.6"
   checksum: b86e5e0e25f7f777b77fabd8e2cbf15737972869d852a22b7e73c17623928fccb826d8e46b9951501d3f20e51ad74ba8c59ed584f610526a48f8ccf88aaec402
   languageName: node
   linkType: hard
 
 "make-fetch-happen@npm:^13.0.0":
-  version: 13.0.0
-  resolution: "make-fetch-happen@npm:13.0.0"
+  version: 13.0.1
+  resolution: "make-fetch-happen@npm:13.0.1"
   dependencies:
     "@npmcli/agent": ^2.0.0
     cacache: ^18.0.0
     http-cache-semantics: ^4.1.1
     is-lambda: ^1.0.1
     minipass: ^7.0.2
     minipass-fetch: ^3.0.0
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     negotiator: ^0.6.3
+    proc-log: ^4.2.0
     promise-retry: ^2.0.1
     ssri: ^10.0.0
-  checksum: 7c7a6d381ce919dd83af398b66459a10e2fe8f4504f340d1d090d3fa3d1b0c93750220e1d898114c64467223504bd258612ba83efbc16f31b075cd56de24b4af
+  checksum: 5c9fad695579b79488fa100da05777213dd9365222f85e4757630f8dd2a21a79ddd3206c78cfd6f9b37346819681782b67900ac847a57cf04190f52dda5343fd
   languageName: node
   linkType: hard
 
 "makeerror@npm:1.0.12":
   version: 1.0.12
   resolution: "makeerror@npm:1.0.12"
   dependencies:
@@ -7554,20 +7543,20 @@
   version: 1.4.1
   resolution: "merge2@npm:1.4.1"
   checksum: 7268db63ed5169466540b6fb947aec313200bcf6d40c5ab722c22e242f651994619bcd85601602972d3c85bd2cc45a358a4c61937e9f11a061919a1da569b0c2
   languageName: node
   linkType: hard
 
 "micromatch@npm:^4.0.4, micromatch@npm:^4.0.5":
-  version: 4.0.5
-  resolution: "micromatch@npm:4.0.5"
+  version: 4.0.6
+  resolution: "micromatch@npm:4.0.6"
   dependencies:
-    braces: ^3.0.2
-    picomatch: ^2.3.1
-  checksum: 02a17b671c06e8fefeeb6ef996119c1e597c942e632a21ef589154f23898c9c6a9858526246abb14f8bca6e77734aa9dcf65476fca47cedfb80d9577d52843fc
+    braces: ^3.0.3
+    picomatch: ^4.0.2
+  checksum: cd44a850c638d82232608e2a03677c5828b9faf35bacfd4817ae232208e2a56bac97bceb67da6a5d4d5a603c1cc88f65ecae3af6be11b5a8c10c995515231e78
   languageName: node
   linkType: hard
 
 "mime-db@npm:1.52.0":
   version: 1.52.0
   resolution: "mime-db@npm:1.52.0"
   checksum: 0d99a03585f8b39d68182803b12ac601d9c01abfa28ec56204fa330bc9f3d1c5e14beb049bafadb3dbdf646dfb94b87e24d4ec7b31b7279ef906a8ea9b6a513f
@@ -7669,25 +7658,25 @@
   dependencies:
     minipass: ^7.0.3
   checksum: b251bceea62090f67a6cced7a446a36f4cd61ee2d5cea9aee7fff79ba8030e416327a1c5aa2908dc22629d06214b46d88fdab8c51ac76bacbf5703851b5ad342
   languageName: node
   linkType: hard
 
 "minipass-fetch@npm:^3.0.0":
-  version: 3.0.4
-  resolution: "minipass-fetch@npm:3.0.4"
+  version: 3.0.5
+  resolution: "minipass-fetch@npm:3.0.5"
   dependencies:
     encoding: ^0.1.13
     minipass: ^7.0.3
     minipass-sized: ^1.0.3
     minizlib: ^2.1.2
   dependenciesMeta:
     encoding:
       optional: true
-  checksum: af7aad15d5c128ab1ebe52e043bdf7d62c3c6f0cecb9285b40d7b395e1375b45dcdfd40e63e93d26a0e8249c9efd5c325c65575aceee192883970ff8cb11364a
+  checksum: 8047d273236157aab27ab7cd8eab7ea79e6ecd63e8f80c3366ec076cb9a0fed550a6935bab51764369027c414647fd8256c2a20c5445fb250c483de43350de83
   languageName: node
   linkType: hard
 
 "minipass-flush@npm:^1.0.5":
   version: 1.0.5
   resolution: "minipass-flush@npm:1.0.5"
   dependencies:
@@ -7734,17 +7723,17 @@
   version: 5.0.0
   resolution: "minipass@npm:5.0.0"
   checksum: 425dab288738853fded43da3314a0b5c035844d6f3097a8e3b5b29b328da8f3c1af6fc70618b32c29ff906284cf6406b6841376f21caaadd0793c1d5a6a620ea
   languageName: node
   linkType: hard
 
 "minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.2, minipass@npm:^7.0.3, minipass@npm:^7.0.4":
-  version: 7.0.4
-  resolution: "minipass@npm:7.0.4"
-  checksum: 87585e258b9488caf2e7acea242fd7856bbe9a2c84a7807643513a338d66f368c7d518200ad7b70a508664d408aa000517647b2930c259a8b1f9f0984f344a21
+  version: 7.1.1
+  resolution: "minipass@npm:7.1.1"
+  checksum: d2c461947a7530f93de4162aa3ca0a1bed1f121626906f6ec63a5ba05fd7b1d9bee4fe89a37a43db7241c2416be98a799c1796abae583c7180be37be5c392ef6
   languageName: node
   linkType: hard
 
 "minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
   version: 2.1.2
   resolution: "minizlib@npm:2.1.2"
   dependencies:
@@ -7810,28 +7799,14 @@
 "nice-try@npm:^1.0.4":
   version: 1.0.5
   resolution: "nice-try@npm:1.0.5"
   checksum: 0b4af3b5bb5d86c289f7a026303d192a7eb4417231fe47245c460baeabae7277bcd8fd9c728fb6bd62c30b3e15cd6620373e2cf33353b095d8b403d3e8a15aff
   languageName: node
   linkType: hard
 
-"node-fetch@npm:^2.6.0":
-  version: 2.7.0
-  resolution: "node-fetch@npm:2.7.0"
-  dependencies:
-    whatwg-url: ^5.0.0
-  peerDependencies:
-    encoding: ^0.1.0
-  peerDependenciesMeta:
-    encoding:
-      optional: true
-  checksum: d76d2f5edb451a3f05b15115ec89fc6be39de37c6089f1b6368df03b91e1633fd379a7e01b7ab05089a25034b2023d959b47e59759cb38d88341b2459e89d6e5
-  languageName: node
-  linkType: hard
-
 "node-gyp@npm:latest":
   version: 10.1.0
   resolution: "node-gyp@npm:10.1.0"
   dependencies:
     env-paths: ^2.2.0
     exponential-backoff: ^3.1.1
     glob: ^10.3.10
@@ -7859,21 +7834,21 @@
   version: 2.0.14
   resolution: "node-releases@npm:2.0.14"
   checksum: 59443a2f77acac854c42d321bf1b43dea0aef55cd544c6a686e9816a697300458d4e82239e2d794ea05f7bbbc8a94500332e2d3ac3f11f52e4b16cbe638b3c41
   languageName: node
   linkType: hard
 
 "nopt@npm:^7.0.0":
-  version: 7.2.0
-  resolution: "nopt@npm:7.2.0"
+  version: 7.2.1
+  resolution: "nopt@npm:7.2.1"
   dependencies:
     abbrev: ^2.0.0
   bin:
     nopt: bin/nopt.js
-  checksum: a9c0f57fb8cb9cc82ae47192ca2b7ef00e199b9480eed202482c962d61b59a7fbe7541920b2a5839a97b42ee39e288c0aed770e38057a608d7f579389dfde410
+  checksum: 6fa729cc77ce4162cfad8abbc9ba31d4a0ff6850c3af61d59b505653bef4781ec059f8890ecfe93ee8aa0c511093369cca88bfc998101616a2904e715bbbb7c9
   languageName: node
   linkType: hard
 
 "normalize-package-data@npm:^2.3.2, normalize-package-data@npm:^2.5.0":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
@@ -7931,17 +7906,17 @@
   dependencies:
     path-key: ^3.0.0
   checksum: 5374c0cea4b0bbfdfae62da7bbdf1e1558d338335f4cacf2515c282ff358ff27b2ecb91ffa5330a8b14390ac66a1e146e10700440c1ab868208430f56b5f4d23
   languageName: node
   linkType: hard
 
 "nwsapi@npm:^2.2.2":
-  version: 2.2.9
-  resolution: "nwsapi@npm:2.2.9"
-  checksum: 3ab2bc47d5507a76e2fdee5aae7ea2875c6def912d0401126cad3e39825a7decb7a02622810c855a7902bd31e917e606b37882dca12b0ae54b4d3b70275de927
+  version: 2.2.10
+  resolution: "nwsapi@npm:2.2.10"
+  checksum: 5f1d361b38c47ab49727d5ea8bbfeb5867ae6de0e538eec9a8b77c88005ddde36d8b930e0730b50ee5e5dda949112c0f9ffed1bf15e7e1b3cd9cfa319f5a9b6f
   languageName: node
   linkType: hard
 
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
@@ -8143,21 +8118,21 @@
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
-"path-scurry@npm:^1.10.2, path-scurry@npm:^1.6.1":
-  version: 1.10.2
-  resolution: "path-scurry@npm:1.10.2"
+"path-scurry@npm:^1.11.0, path-scurry@npm:^1.6.1":
+  version: 1.11.1
+  resolution: "path-scurry@npm:1.11.1"
   dependencies:
     lru-cache: ^10.2.0
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-  checksum: 6739b4290f7d1a949c61c758b481c07ac7d1a841964c68cf5e1fa153d7e18cbde4872b37aadf9c5173c800d627f219c47945859159de36c977dd82419997b9b8
+  checksum: 890d5abcd593a7912dcce7cf7c6bf7a0b5648e3dee6caf0712c126ca0a65c7f3d7b9d769072a4d1baf370f61ce493ab5b038d59988688e0c5f3f646ee3c69023
   languageName: node
   linkType: hard
 
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
@@ -8169,28 +8144,35 @@
 "path-type@npm:^4.0.0":
   version: 4.0.0
   resolution: "path-type@npm:4.0.0"
   checksum: 5b1e2daa247062061325b8fdbfd1fb56dde0a448fb1455453276ea18c60685bdad23a445dc148cf87bc216be1573357509b7d4060494a6fd768c7efad833ee45
   languageName: node
   linkType: hard
 
-"picocolors@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "picocolors@npm:1.0.0"
-  checksum: a2e8092dd86c8396bdba9f2b5481032848525b3dc295ce9b57896f931e63fc16f79805144321f72976383fc249584672a75cc18d6777c6b757603f372f745981
+"picocolors@npm:^1.0.0, picocolors@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "picocolors@npm:1.0.1"
+  checksum: fa68166d1f56009fc02a34cdfd112b0dd3cf1ef57667ac57281f714065558c01828cdf4f18600ad6851cbe0093952ed0660b1e0156bddf2184b6aaf5817553a5
   languageName: node
   linkType: hard
 
-"picomatch@npm:^2.0.4, picomatch@npm:^2.2.3, picomatch@npm:^2.3.1":
+"picomatch@npm:^2.0.4, picomatch@npm:^2.2.3":
   version: 2.3.1
   resolution: "picomatch@npm:2.3.1"
   checksum: 050c865ce81119c4822c45d3c84f1ced46f93a0126febae20737bd05ca20589c564d6e9226977df859ed5e03dc73f02584a2b0faad36e896936238238b0446cf
   languageName: node
   linkType: hard
 
+"picomatch@npm:^4.0.2":
+  version: 4.0.2
+  resolution: "picomatch@npm:4.0.2"
+  checksum: a7a5188c954f82c6585720e9143297ccd0e35ad8072231608086ca950bee672d51b0ef676254af0788205e59bd4e4deb4e7708769226bed725bf13370a7d1464
+  languageName: node
+  linkType: hard
+
 "pidtree@npm:^0.3.0":
   version: 0.3.1
   resolution: "pidtree@npm:0.3.1"
   bin:
     pidtree: bin/pidtree.js
   checksum: eb49025099f1af89a4696f7673351421f13420f3397b963c901fe23a1c9c2ff50f4750321970d4472c0ffbb065e4a6c3c27f75e226cc62284b19e21d32ce7012
   languageName: node
@@ -8360,14 +8342,21 @@
 "proc-log@npm:^3.0.0":
   version: 3.0.0
   resolution: "proc-log@npm:3.0.0"
   checksum: 02b64e1b3919e63df06f836b98d3af002b5cd92655cab18b5746e37374bfb73e03b84fe305454614b34c25b485cc687a9eebdccf0242cda8fda2475dd2c97e02
   languageName: node
   linkType: hard
 
+"proc-log@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "proc-log@npm:4.2.0"
+  checksum: 98f6cd012d54b5334144c5255ecb941ee171744f45fca8b43b58ae5a0c1af07352475f481cadd9848e7f0250376ee584f6aa0951a856ff8f021bdfbff4eb33fc
+  languageName: node
+  linkType: hard
+
 "process@npm:^0.11.10":
   version: 0.11.10
   resolution: "process@npm:0.11.10"
   checksum: bfcce49814f7d172a6e6a14d5fa3ac92cc3d0c3b9feb1279774708a719e19acd673995226351a082a9ae99978254e320ccda4240ddc474ba31a76c79491ca7c3
   languageName: node
   linkType: hard
 
@@ -8765,25 +8754,25 @@
 "safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
   languageName: node
   linkType: hard
 
-"sanitize-html@npm:~2.7.3":
-  version: 2.7.3
-  resolution: "sanitize-html@npm:2.7.3"
+"sanitize-html@npm:~2.12.1":
+  version: 2.12.1
+  resolution: "sanitize-html@npm:2.12.1"
   dependencies:
     deepmerge: ^4.2.2
     escape-string-regexp: ^4.0.0
-    htmlparser2: ^6.0.0
+    htmlparser2: ^8.0.0
     is-plain-object: ^5.0.0
     parse-srcset: ^1.0.2
     postcss: ^8.3.11
-  checksum: 2399d1fdbbc3a263fb413c1fe1971b3dc2b51abc6cc5cb49490624539d1c57a8fe31e2b21408c118e2a957f4e673e3169b1f9a5807654408f17b130a9d78aed7
+  checksum: fb96ea7170d51b5af2607f5cfd84464c78fc6f47e339407f55783e781c6a0288a8d40bbf97ea6a8758924ba9b2d33dcc4846bb94caacacd90d7f2de10ed8541a
   languageName: node
   linkType: hard
 
 "saxes@npm:^6.0.0":
   version: 6.0.0
   resolution: "saxes@npm:6.0.0"
   dependencies:
@@ -8850,21 +8839,19 @@
   bin:
     semver: bin/semver.js
   checksum: ae47d06de28836adb9d3e25f22a92943477371292d9b665fb023fae278d345d508ca1958232af086d85e0155aee22e313e100971898bbb8d5d89b8b1d4054ca2
   languageName: node
   linkType: hard
 
 "semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.5.3, semver@npm:^7.5.4":
-  version: 7.6.0
-  resolution: "semver@npm:7.6.0"
-  dependencies:
-    lru-cache: ^6.0.0
+  version: 7.6.2
+  resolution: "semver@npm:7.6.2"
   bin:
     semver: bin/semver.js
-  checksum: 7427f05b70786c696640edc29fdd4bc33b2acf3bbe1740b955029044f80575fc664e1a512e4113c3af21e767154a94b4aa214bf6cd6e42a1f6dba5914e0b208c
+  checksum: 40f6a95101e8d854357a644da1b8dd9d93ce786d5c6a77227bc69dbb17bea83d0d1d1d7c4cd5920a6df909f48e8bd8a5909869535007f90278289f2451d0292d
   languageName: node
   linkType: hard
 
 "serialize-javascript@npm:^6.0.1":
   version: 6.0.2
   resolution: "serialize-javascript@npm:6.0.2"
   dependencies:
@@ -9152,19 +9139,19 @@
   version: 1.0.3
   resolution: "sprintf-js@npm:1.0.3"
   checksum: 19d79aec211f09b99ec3099b5b2ae2f6e9cdefe50bc91ac4c69144b6d3928a640bb6ae5b3def70c2e85a2c3d9f5ec2719921e3a59d3ca3ef4b2fd1a4656a0df3
   languageName: node
   linkType: hard
 
 "ssri@npm:^10.0.0":
-  version: 10.0.5
-  resolution: "ssri@npm:10.0.5"
+  version: 10.0.6
+  resolution: "ssri@npm:10.0.6"
   dependencies:
     minipass: ^7.0.3
-  checksum: 0a31b65f21872dea1ed3f7c200d7bc1c1b91c15e419deca14f282508ba917cbb342c08a6814c7f68ca4ca4116dd1a85da2bbf39227480e50125a1ceffeecb750
+  checksum: 4603d53a05bcd44188747d38f1cc43833b9951b5a1ee43ba50535bdfc5fe4a0897472dbe69837570a5417c3c073377ef4f8c1a272683b401857f72738ee57299
   languageName: node
   linkType: hard
 
 "stack-utils@npm:^2.0.3":
   version: 2.0.6
   resolution: "stack-utils@npm:2.0.6"
   dependencies:
@@ -9623,58 +9610,54 @@
   resolution: "tr46@npm:3.0.0"
   dependencies:
     punycode: ^2.1.1
   checksum: 44c3cc6767fb800490e6e9fd64fd49041aa4e49e1f6a012b34a75de739cc9ed3a6405296072c1df8b6389ae139c5e7c6496f659cfe13a04a4bff3a1422981270
   languageName: node
   linkType: hard
 
-"tr46@npm:~0.0.3":
-  version: 0.0.3
-  resolution: "tr46@npm:0.0.3"
-  checksum: 726321c5eaf41b5002e17ffbd1fb7245999a073e8979085dacd47c4b4e8068ff5777142fc6726d6ca1fd2ff16921b48788b87225cbc57c72636f6efa8efbffe3
-  languageName: node
-  linkType: hard
-
 "trim-newlines@npm:^3.0.0":
   version: 3.0.1
   resolution: "trim-newlines@npm:3.0.1"
   checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
   languageName: node
   linkType: hard
 
 "ts-jest@npm:^29.1.0":
-  version: 29.1.2
-  resolution: "ts-jest@npm:29.1.2"
+  version: 29.1.3
+  resolution: "ts-jest@npm:29.1.3"
   dependencies:
     bs-logger: 0.x
     fast-json-stable-stringify: 2.x
     jest-util: ^29.0.0
     json5: ^2.2.3
     lodash.memoize: 4.x
     make-error: 1.x
     semver: ^7.5.3
     yargs-parser: ^21.0.1
   peerDependencies:
     "@babel/core": ">=7.0.0-beta.0 <8"
+    "@jest/transform": ^29.0.0
     "@jest/types": ^29.0.0
     babel-jest: ^29.0.0
     jest: ^29.0.0
     typescript: ">=4.3 <6"
   peerDependenciesMeta:
     "@babel/core":
       optional: true
+    "@jest/transform":
+      optional: true
     "@jest/types":
       optional: true
     babel-jest:
       optional: true
     esbuild:
       optional: true
   bin:
     ts-jest: cli.js
-  checksum: a0ce0affc1b716c78c9ab55837829c42cb04b753d174a5c796bb1ddf9f0379fc20647b76fbe30edb30d9b23181908138d6b4c51ef2ae5e187b66635c295cefd5
+  checksum: c5b2c0501680a9056c50541a3315de7b3b85a611056b978062b4defc96fb0066d12bf1e15715021799a3779723343fb98a9a4ba01dc01709f274899b6c28453d
   languageName: node
   linkType: hard
 
 "tslib@npm:^1.13.0, tslib@npm:^1.8.1":
   version: 1.14.1
   resolution: "tslib@npm:1.14.1"
   checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
@@ -9904,28 +9887,28 @@
   version: 2.0.1
   resolution: "universalify@npm:2.0.1"
   checksum: ecd8469fe0db28e7de9e5289d32bd1b6ba8f7183db34f3bfc4ca53c49891c2d6aa05f3fb3936a81285a905cc509fb641a0c3fc131ec786167eff41236ae32e60
   languageName: node
   linkType: hard
 
 "update-browserslist-db@npm:^1.0.13":
-  version: 1.0.13
-  resolution: "update-browserslist-db@npm:1.0.13"
+  version: 1.0.16
+  resolution: "update-browserslist-db@npm:1.0.16"
   dependencies:
-    escalade: ^3.1.1
-    picocolors: ^1.0.0
+    escalade: ^3.1.2
+    picocolors: ^1.0.1
   peerDependencies:
     browserslist: ">= 4.21.0"
   bin:
     update-browserslist-db: cli.js
-  checksum: 1e47d80182ab6e4ad35396ad8b61008ae2a1330221175d0abd37689658bdb61af9b705bfc41057fd16682474d79944fb2d86767c5ed5ae34b6276b9bed353322
+  checksum: 51b1f7189c9ea5925c80154b0a6fd3ec36106d07858d8f69826427d8edb4735d1801512c69eade38ba0814d7407d11f400d74440bbf3da0309f3d788017f35b2
   languageName: node
   linkType: hard
 
-"uri-js@npm:^4.2.2":
+"uri-js@npm:^4.2.2, uri-js@npm:^4.4.1":
   version: 4.4.1
   resolution: "uri-js@npm:4.4.1"
   dependencies:
     punycode: ^2.1.0
   checksum: 7167432de6817fe8e9e0c9684f1d2de2bb688c94388f7569f7dbdb1587c9f4ca2a77962f134ec90be0cc4d004c939ff0d05acc9f34a0db39a3c797dada262633
   languageName: node
   linkType: hard
@@ -10020,28 +10003,35 @@
 "validate.io-number@npm:^1.0.3":
   version: 1.0.3
   resolution: "validate.io-number@npm:1.0.3"
   checksum: 42418aeb6c969efa745475154fe576809b02eccd0961aad0421b090d6e7a12d23a3e28b0d5dddd2c6347c1a6bdccb82bba5048c716131cd20207244d50e07282
   languageName: node
   linkType: hard
 
-"vscode-jsonrpc@npm:8.2.0, vscode-jsonrpc@npm:^8.0.2":
+"vscode-jsonrpc@npm:8.2.0":
   version: 8.2.0
   resolution: "vscode-jsonrpc@npm:8.2.0"
   checksum: f302a01e59272adc1ae6494581fa31c15499f9278df76366e3b97b2236c7c53ebfc71efbace9041cfd2caa7f91675b9e56f2407871a1b3c7f760a2e2ee61484a
   languageName: node
   linkType: hard
 
 "vscode-jsonrpc@npm:^6.0.0":
   version: 6.0.0
   resolution: "vscode-jsonrpc@npm:6.0.0"
   checksum: 3a67a56f287e8c449f2d9752eedf91e704dc7b9a326f47fb56ac07667631deb45ca52192e9bccb2ab108764e48409d70fa64b930d46fc3822f75270b111c5f53
   languageName: node
   linkType: hard
 
+"vscode-jsonrpc@npm:^8.0.2":
+  version: 8.2.1
+  resolution: "vscode-jsonrpc@npm:8.2.1"
+  checksum: 2af2c333d73f6587896a7077978b8d4b430e55c674d5dbb90597a84a6647057c1655a3bff398a9b08f1f8ba57dbd2deabf05164315829c297b0debba3b8bc19e
+  languageName: node
+  linkType: hard
+
 "vscode-languageserver-protocol@npm:^3.17.0":
   version: 3.17.5
   resolution: "vscode-languageserver-protocol@npm:3.17.5"
   dependencies:
     vscode-jsonrpc: 8.2.0
     vscode-languageserver-types: 3.17.5
   checksum: dfb42d276df5dfea728267885b99872ecff62f6c20448b8539fae71bb196b420f5351c5aca7c1047bf8fb1f89fa94a961dce2bc5bf7e726198f4be0bb86a1e71
@@ -10095,21 +10085,14 @@
   dependencies:
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.1.2
   checksum: 5b0179348655dcdf19cac7cb4ff923fdc024d630650c0bf6bec8899cf47c60e19d4f810a88dba692ed0e7f684cf0fcffea86efdbf6c35d81f031e328043b7fab
   languageName: node
   linkType: hard
 
-"webidl-conversions@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "webidl-conversions@npm:3.0.1"
-  checksum: c92a0a6ab95314bde9c32e1d0a6dfac83b578f8fa5f21e675bc2706ed6981bc26b7eb7e6a1fab158e5ce4adf9caa4a0aee49a52505d4d13c7be545f15021b17c
-  languageName: node
-  linkType: hard
-
 "webidl-conversions@npm:^6.1.0":
   version: 6.1.0
   resolution: "webidl-conversions@npm:6.1.0"
   checksum: 1f526507aa491f972a0c1409d07f8444e1d28778dfa269a9971f2e157182f3d496dc33296e4ed45b157fdb3bf535bb90c90bf10c50dcf1dd6caacb2a34cc84fb
   languageName: node
   linkType: hard
 
@@ -10246,24 +10229,14 @@
   dependencies:
     tr46: ^3.0.0
     webidl-conversions: ^7.0.0
   checksum: ed4826aaa57e66bb3488a4b25c9cd476c46ba96052747388b5801f137dd740b73fde91ad207d96baf9f17fbcc80fc1a477ad65181b5eb5fa718d27c69501d7af
   languageName: node
   linkType: hard
 
-"whatwg-url@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "whatwg-url@npm:5.0.0"
-  dependencies:
-    tr46: ~0.0.3
-    webidl-conversions: ^3.0.0
-  checksum: b8daed4ad3356cc4899048a15b2c143a9aed0dfae1f611ebd55073310c7b910f522ad75d727346ad64203d7e6c79ef25eafd465f4d12775ca44b90fa82ed9e2c
-  languageName: node
-  linkType: hard
-
 "whatwg-url@npm:^8.0.0":
   version: 8.7.0
   resolution: "whatwg-url@npm:8.7.0"
   dependencies:
     lodash: ^4.7.0
     tr46: ^2.1.0
     webidl-conversions: ^6.1.0
```

### Comparing `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/package.json` & `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802350427350427%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f65916be0fb99f932ce1.js'}}",*

 * * "'version'": "'0.5.6'"}*

```diff
@@ -104,15 +104,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_athena_analytics",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d43dde86f53fb87db6c8.js",
+            "load": "static/remoteEntry.f65916be0fb99f932ce1.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_athena_analytics/labextension"
     },
     "keywords": [
         "jupyter",
@@ -178,12 +178,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.5",
+    "version": "0.5.6",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/509.68053d43f01f7d268d38.js` & `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/509.ffcf5195228912dc474b.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunkjupyterlab_athena_analytics = self.webpackChunkjupyterlab_athena_analytics || []).push([
     [509], {
         509: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => r
             });
-            var n = o(506),
-                a = o(242);
+            var n = o(291),
+                a = o(899);
 
             function c(e) {
                 e.widgets.forEach((e => {
                     e.model.contentChanged.connect((() => function(e) {
                         const t = e.toJSON();
                         window.parent.postMessage({
                             type: "cellContentChange",
@@ -84,16 +84,27 @@
                                     o && o.model.sharedModel.setSource(t)
                                 }(c.content, a.data);
                                 break;
                             case "executeActiveCell":
                                 ! function(e) {
                                     e && e.content ? n.NotebookActions.run(e.content, e.sessionContext).then((() => {
                                         console.log("Cell executed successfully")
-                                    }), (e => {
-                                        console.error("Error executing cell:", e)
+                                    }), (t => {
+                                        console.error("Error executing cell:", t),
+                                            function(e, t) {
+                                                const o = e.content.activeCell,
+                                                    n = null == o ? void 0 : o.model.toJSON();
+                                                window.parent.postMessage({
+                                                    type: "cellExecutionError",
+                                                    data: {
+                                                        cellData: n,
+                                                        error: t.message
+                                                    }
+                                                }, "*")
+                                            }(e, t)
                                     })) : console.error("Invalid notebook panel")
                                 }(c);
                                 break;
                             case "createNewNotebook":
                                 ! function(e, t) {
                                     const o = `${t}.ipynb`,
                                         n = e.createNew(o, "notebook");
```

### Comparing `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js` & `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/remoteEntry.d43dde86f53fb87db6c8.js` & `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/remoteEntry.f65916be0fb99f932ce1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, a, o, i, u, l, s, f, c, d, p, h, v, b, y = {
-            98: (e, r, t) => {
+            363: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(509).then((() => () => t(509))),
                         "./extension": () => t.e(509).then((() => () => t(509))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -43,18 +43,18 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        509: "68053d43f01f7d268d38",
+        509: "ffcf5195228912dc474b",
         728: "c9fba78fc7d4a52b2765"
     } [e] + ".js?v=" + {
-        509: "68053d43f01f7d268d38",
+        509: "ffcf5195228912dc474b",
         728: "c9fba78fc7d4a52b2765"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(509).then((() => () => m(509))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab_athena_analytics", "0.5.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab_athena_analytics", "0.5.6"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -208,18 +208,18 @@
         return o(n, a) || f(l(e, t, a, n)), c(e[t][a])
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, h = {
-        242: () => d("default", "@jupyterlab/docmanager", [1, 4, 1, 8]),
-        506: () => d("default", "@jupyterlab/notebook", [1, 4, 1, 8])
+        291: () => d("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
+        899: () => d("default", "@jupyterlab/docmanager", [1, 4, 2, 0])
     }, v = {
-        509: [242, 506]
+        509: [291, 899]
     }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(p, e)) return r.push(p[e]);
             if (!b[e]) {
                 var t = r => {
                     p[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
@@ -269,10 +269,10 @@
                     u && u(m)
                 }
                 for (r && r(t); l < o.length; l++) a = o[l], m.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkjupyterlab_athena_analytics = self.webpackChunkjupyterlab_athena_analytics || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), m.nc = void 0;
-    var w = m(98);
+    var w = m(363);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_athena_analytics = w
 })();
```

### Comparing `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json` & `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/src/index.ts` & `jupyterlab_athena_analytics-0.5.6/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,27 @@
   const cellData = cellModel.toJSON();
   window.parent.postMessage({
     type: 'cellContentChange',
     data: cellData
   }, '*');
 }
 
+// Function to handle cell execution errors
+function onCellExecutionError(notebookPanel: NotebookPanel, error: any): void {
+  const activeCell = notebookPanel.content.activeCell;
+  const cellData = activeCell?.model.toJSON();
+  window.parent.postMessage({
+    type: 'cellExecutionError',
+    data: {
+      cellData,
+      error: error.message
+    }
+  }, '*');
+}
+
 // Function to add listeners to each cell in the notebook
 function addCellListeners(notebook: Notebook): void {
   notebook.widgets.forEach(cell => {
     cell.model.contentChanged.connect(() => onCellModelChange(cell.model));
   });
 }
 
@@ -78,80 +91,81 @@
   const activeCell = notebook.activeCell;
   if (activeCell) {
     activeCell.model.sharedModel.setSource(code);
   }
 }
 
 function selectOrInsertBelowCell(notebookPanel: NotebookPanel): void {
-    if (!notebookPanel || !notebookPanel.content) {
-        console.error('Invalid notebook panel');
-        return;
-    }
-    // Save the current active cell index
-    const currentActiveCellIndex = notebookPanel.content.activeCellIndex;
-    // Try to select the cell below
+  if (!notebookPanel || !notebookPanel.content) {
+    console.error('Invalid notebook panel');
+    return;
+  }
+  // Save the current active cell index
+  const currentActiveCellIndex = notebookPanel.content.activeCellIndex;
+  // Try to select the cell below
 
-    const numCells = notebookPanel.model?.cells.length;    
+  const numCells = notebookPanel.model?.cells.length;
 
-    if (numCells && currentActiveCellIndex === numCells-1) {
-      NotebookActions.insertBelow(notebookPanel.content);
-    }
-    else {
-      NotebookActions.selectBelow(notebookPanel.content);
-    }
-    // Check if the active cell index has changed
+  if (numCells && currentActiveCellIndex === numCells - 1) {
+    NotebookActions.insertBelow(notebookPanel.content);
+  }
+  else {
+    NotebookActions.selectBelow(notebookPanel.content);
+  }
+  // Check if the active cell index has changed
 }
 
 function selectOrInsertAboveCell(notebookPanel: NotebookPanel): void {
-    if (!notebookPanel || !notebookPanel.content) {
-        console.error('Invalid notebook panel');
-        return;
-    }
-    // Save the current active cell index
-    const currentActiveCellIndex = notebookPanel.content.activeCellIndex;
-    // Try to select the cell above
-    console.log("current active cell index :", currentActiveCellIndex)
-    // if (currentActiveCellIndex === 0) {
-    //   NotebookActions.insertAbove(notebookPanel.content);
-    // }
-    NotebookActions.selectAbove(notebookPanel.content);
-    // Check if the active cell index has changed
+  if (!notebookPanel || !notebookPanel.content) {
+    console.error('Invalid notebook panel');
+    return;
+  }
+  // Save the current active cell index
+  const currentActiveCellIndex = notebookPanel.content.activeCellIndex;
+  // Try to select the cell above
+  console.log("current active cell index :", currentActiveCellIndex)
+  // if (currentActiveCellIndex === 0) {
+  //   NotebookActions.insertAbove(notebookPanel.content);
+  // }
+  NotebookActions.selectAbove(notebookPanel.content);
+  // Check if the active cell index has changed
 }
 
 
 function executeActiveCell(notebookPanel: NotebookPanel) {
   if (!notebookPanel || !notebookPanel.content) {
-      console.error('Invalid notebook panel');
-      return;
+    console.error('Invalid notebook panel');
+    return;
   }
   // Execute the active cell
   NotebookActions.run(notebookPanel.content, notebookPanel.sessionContext).then(
     () => {
       console.log('Cell executed successfully');
     },
     (reason) => {
       console.error('Error executing cell:', reason);
+      onCellExecutionError(notebookPanel, reason);
     }
   );
 }
 
 function createNewNotebook(documentManager: IDocumentManager, notebookName: string): void {
   // Define the full path for the new notebook
   const path = `${notebookName}.ipynb`;
 
   // Create a new notebook
   const widget = documentManager.createNew(path, 'notebook');
 
   if (widget) {
     // Wait for the notebook to be fully loaded
-      widget.activate();
+    widget.activate();
 
-} else {
+  } else {
     console.error('Failed to create a new notebook');
-} 
+  }
 }
 
 
 function openExistingNotebook(documentManager: IDocumentManager, notebookName: string): void {
   // Define the full path for the notebook
   const path = `${notebookName}.ipynb`;
   const widget = documentManager.openOrReveal(path);
@@ -186,15 +200,15 @@
       if (notebookPanel) {
         onTabChange(notebookPanel);
       }
     });
 
     window.addEventListener('message', (event: MessageEvent) => {
       // Always check the origin for security reasons
-    
+
       const message = event.data;
       console.log(message);
       const notebookPanel = tracker.currentWidget;
 
       if (notebookPanel) {
         switch (message.type) {
           case 'selectOrInsertBelowCell':
@@ -212,17 +226,17 @@
             createNewNotebook(docManager, message.data);
             break;
           case 'openExistingNotebook':
             openExistingNotebook(docManager, message.data);
             break;
           default:
             console.log('Unknown message type:', message.type);
-          }
+        }
       }
-    }); 
+    });
 
 
     // Dynamically inject the PostHog analytics script into the document
     const script = document.createElement('script');
     script.type = 'text/javascript';
     script.async = true;
     script.innerHTML = `!function(t,e){var o,n,p,r;e._SV||(window.posthog=e,e._i=[],e.init=function(i,s,a){function g(t,e){var o=e.split(".");2==o.length&&(t=t[o[0]],e=o[1]),t[e]=function(){t.push([e].concat(Array.prototype.slice.call(arguments,0)))}}(p=t.createElement("script")).type="text/javascript",p.async=!0,p.src=s.api_host+"/static/array.js",(r=t.getElementsByTagName("script")[0]).parentNode.insertBefore(p,r);var u=e;for(void 0!==a?u=e[a]=[]:a="posthog",u.people=u.people||[],u.toString=function(t){var e="posthog";return"posthog"!==a&&(e+="."+a),t||(e+=" (stub)"),e},u.people.toString=function(){return u.toString(1)+".people (stub)"},o="capture identify alias people.set people.set_once set_config register register_once unregister opt_out_capturing has_opted_out_capturing opt_in_capturing reset isFeatureEnabled onFeatureFlags getFeatureFlag getFeatureFlagPayload reloadFeatureFlags group updateEarlyAccessFeatureEnrollment getEarlyAccessFeatures getActiveMatchingSurveys getSurveys onSessionId".split(" "),n=0;n<o.length;n++)g(u,o[n]);e._i.push([i,s,a])},e._SV=1)}(document,window.posthog||[]);
```

### Comparing `jupyterlab_athena_analytics-0.5.5/ui-tests/README.md` & `jupyterlab_athena_analytics-0.5.6/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/ui-tests/tests/jupyterlab_athena_analytics.spec.ts` & `jupyterlab_athena_analytics-0.5.6/ui-tests/tests/jupyterlab_athena_analytics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/.gitignore` & `jupyterlab_athena_analytics-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/LICENSE` & `jupyterlab_athena_analytics-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/README.md` & `jupyterlab_athena_analytics-0.5.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -62,19 +62,14 @@
 
 ## Publish
 ```bash
 hatch publish
 ```
 For username just click enter and for Credentials put in your token from the pypi website or as follows: 
 
-### token
-```
-pypi-AgEIcHlwaS5vcmcCJDIxOTBlNmFjLWY0YzItNDMwMy1hYTgwLTc4ZmM0MjJjMGI1MgACI1sxLFsianVweXRlcmxhYi1hdGhlbmEtYW5hbHl0aWNzIl1dAAIsWzIsWyJiZWY1ZGM2Ny02NGE4LTQ4ODYtOWM2ZC02M2M1YzVmNWVmNGEiXV0AAAYgxX-0Ec9kVZAAr47iGSGFdxTW6ev0PY1iuO3ZMt1ssyo
-```
-
 Sample output:
 ```bash
 dist/jupyterlab_athena_analytics-0.3.0-py3-none-any.whl ...
 success
 dist/jupyterlab_athena_analytics-0.2.0.tar.gz ... already exists
 dist/jupyterlab_athena_analytics-0.3.0.tar.gz ... success
 dist/jupyterlab_athena_analytics-0.2.0-py3-none-any.whl ... already exists
```

### Comparing `jupyterlab_athena_analytics-0.5.5/pyproject.toml` & `jupyterlab_athena_analytics-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.5/PKG-INFO` & `jupyterlab_athena_analytics-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_athena_analytics
-Version: 0.5.5
+Version: 0.5.6
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_athena_analytics
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_athena_analytics/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_athena_analytics.git
 Author-email: Athena Intelligence <team@athenaintelligence.ai>
 License: BSD 3-Clause License
         
@@ -115,19 +115,14 @@
 
 ## Publish
 ```bash
 hatch publish
 ```
 For username just click enter and for Credentials put in your token from the pypi website or as follows: 
 
-### token
-```
-pypi-AgEIcHlwaS5vcmcCJDIxOTBlNmFjLWY0YzItNDMwMy1hYTgwLTc4ZmM0MjJjMGI1MgACI1sxLFsianVweXRlcmxhYi1hdGhlbmEtYW5hbHl0aWNzIl1dAAIsWzIsWyJiZWY1ZGM2Ny02NGE4LTQ4ODYtOWM2ZC02M2M1YzVmNWVmNGEiXV0AAAYgxX-0Ec9kVZAAr47iGSGFdxTW6ev0PY1iuO3ZMt1ssyo
-```
-
 Sample output:
 ```bash
 dist/jupyterlab_athena_analytics-0.3.0-py3-none-any.whl ...
 success
 dist/jupyterlab_athena_analytics-0.2.0.tar.gz ... already exists
 dist/jupyterlab_athena_analytics-0.3.0.tar.gz ... success
 dist/jupyterlab_athena_analytics-0.2.0-py3-none-any.whl ... already exists
```

