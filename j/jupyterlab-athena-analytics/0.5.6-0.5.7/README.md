# Comparing `tmp/jupyterlab_athena_analytics-0.5.6.tar.gz` & `tmp/jupyterlab_athena_analytics-0.5.7.tar.gz`

## Comparing `jupyterlab_athena_analytics-0.5.6.tar` & `jupyterlab_athena_analytics-0.5.7.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/CHANGELOG.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/babel.config.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/build.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jest.config.js
--rw-r--r--   0        0        0   357048 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/package-lock.json
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/setup.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/test.ipynb
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/tsconfig.test.json
--rw-r--r--   0        0        0   373470 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/yarn.lock
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/_version.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/package.json
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/509.ffcf5195228912dc474b.js
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/remoteEntry.f65916be0fb99f932ce1.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/scripts/build.sh
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/scripts/deploy-full.sh
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/.gitignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/.yarnrc.yml
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/index.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/src/__tests__/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/yarn.lock
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/LICENSE
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/README.md
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/CHANGELOG.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/babel.config.js
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jest.config.js
+-rw-r--r--   0        0        0   357048 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/package-lock.json
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/setup.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/test.ipynb
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/tsconfig.test.json
+-rw-r--r--   0        0        0   373470 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/yarn.lock
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/_version.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/package.json
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/509.1866d2287dc3dd54b397.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/remoteEntry.6897030c3ef7f0bc60a2.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0       15 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/scripts/build.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/scripts/deploy-full.sh
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/src/.gitignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/src/.yarnrc.yml
+-rw-r--r--   0        0        0     9291 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/src/index.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/src/__tests__/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/LICENSE
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/README.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.7/PKG-INFO
```

### Comparing `jupyterlab_athena_analytics-0.5.6/RELEASE.md` & `jupyterlab_athena_analytics-0.5.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/jest.config.js` & `jupyterlab_athena_analytics-0.5.7/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/package-lock.json` & `jupyterlab_athena_analytics-0.5.7/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/package.json` & `jupyterlab_athena_analytics-0.5.7/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'0.5.7'"}*

```diff
@@ -173,12 +173,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.6",
+    "version": "0.5.7",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.6/test.ipynb` & `jupyterlab_athena_analytics-0.5.7/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/tsconfig.json` & `jupyterlab_athena_analytics-0.5.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/yarn.lock` & `jupyterlab_athena_analytics-0.5.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/package.json` & `jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802350427350427%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6897030c3ef7f0bc60a2.js'}}",*

 * * "'version'": "'0.5.7'"}*

```diff
@@ -104,15 +104,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_athena_analytics",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f65916be0fb99f932ce1.js",
+            "load": "static/remoteEntry.6897030c3ef7f0bc60a2.js",
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
-    "version": "0.5.6",
+    "version": "0.5.7",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/509.ffcf5195228912dc474b.js` & `jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/509.1866d2287dc3dd54b397.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -84,27 +84,16 @@
                                     o && o.model.sharedModel.setSource(t)
                                 }(c.content, a.data);
                                 break;
                             case "executeActiveCell":
                                 ! function(e) {
                                     e && e.content ? n.NotebookActions.run(e.content, e.sessionContext).then((() => {
                                         console.log("Cell executed successfully")
-                                    }), (t => {
-                                        console.error("Error executing cell:", t),
-                                            function(e, t) {
-                                                const o = e.content.activeCell,
-                                                    n = null == o ? void 0 : o.model.toJSON();
-                                                window.parent.postMessage({
-                                                    type: "cellExecutionError",
-                                                    data: {
-                                                        cellData: n,
-                                                        error: t.message
-                                                    }
-                                                }, "*")
-                                            }(e, t)
+                                    }), (e => {
+                                        console.error("Error executing cell:", e)
                                     })) : console.error("Invalid notebook panel")
                                 }(c);
                                 break;
                             case "createNewNotebook":
                                 ! function(e, t) {
                                     const o = `${t}.ipynb`,
                                         n = e.createNew(o, "notebook");
```

### Comparing `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js` & `jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/remoteEntry.f65916be0fb99f932ce1.js` & `jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/remoteEntry.6897030c3ef7f0bc60a2.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, c, d, p, h, v, b, y = {
+    var e, r, t, n, a, o, i, u, l, s, c, f, d, p, h, v, b, y = {
             363: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(509).then((() => () => t(509))),
                         "./extension": () => t.e(509).then((() => () => t(509))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        509: "ffcf5195228912dc474b",
+        509: "1866d2287dc3dd54b397",
         728: "c9fba78fc7d4a52b2765"
     } [e] + ".js?v=" + {
-        509: "ffcf5195228912dc474b",
+        509: "1866d2287dc3dd54b397",
         728: "c9fba78fc7d4a52b2765"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab_athena_analytics:", m.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+                    var c = l[s];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + a) {
+                        i = c;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var c = (r, n) => {
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(d);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(c.bind(null, void 0, {
+                d = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(509).then((() => () => m(509))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab_athena_analytics", "0.5.6"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab_athena_analytics", "0.5.7"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,33 +164,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, c = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == c ? u > n && !a : "" == c != a);
-                if ("u" == f) {
-                    if (!l || "u" != c) return !1
+                var s, c, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (c = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
+                if ("u" == c) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (c == f)
+                    if (f == c)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (a ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != f && "n" != f) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < c != a) return !1;
+                    if (u <= n || c < f != a) return !1;
                     l = !1
-                } else "s" != c && "n" != c && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var d = [],
             p = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -201,18 +201,18 @@
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || f(l(e, t, a, n)), c(e[t][a])
-    }, f = e => {
+        return o(n, a) || c(l(e, t, a, n)), f(e[t][a])
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
+    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, h = {
         291: () => d("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
         899: () => d("default", "@jupyterlab/docmanager", [1, 4, 2, 0])
     }, v = {
         509: [291, 899]
```

### Comparing `jupyterlab_athena_analytics-0.5.6/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json` & `jupyterlab_athena_analytics-0.5.7/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/src/index.ts` & `jupyterlab_athena_analytics-0.5.7/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -46,26 +46,26 @@
   const cellData = cellModel.toJSON();
   window.parent.postMessage({
     type: 'cellContentChange',
     data: cellData
   }, '*');
 }
 
-// Function to handle cell execution errors
-function onCellExecutionError(notebookPanel: NotebookPanel, error: any): void {
-  const activeCell = notebookPanel.content.activeCell;
-  const cellData = activeCell?.model.toJSON();
-  window.parent.postMessage({
-    type: 'cellExecutionError',
-    data: {
-      cellData,
-      error: error.message
-    }
-  }, '*');
-}
+// // Function to handle cell execution errors
+// function onCellExecutionError(notebookPanel: NotebookPanel, error: any): void {
+//   const activeCell = notebookPanel.content.activeCell;
+//   const cellData = activeCell?.model.toJSON();
+//   window.parent.postMessage({
+//     type: 'cellExecutionError',
+//     data: {
+//       cellData,
+//       error
+//     }
+//   }, '*');
+// }
 
 // Function to add listeners to each cell in the notebook
 function addCellListeners(notebook: Notebook): void {
   notebook.widgets.forEach(cell => {
     cell.model.contentChanged.connect(() => onCellModelChange(cell.model));
   });
 }
@@ -76,18 +76,27 @@
   notebookPanel.content.modelContentChanged.connect(() => onNotebookChange(notebookPanel.content));
   notebookPanel.content.activeCellChanged.connect(() => onActiveCellChange(notebookPanel.content));
 
   // Add listeners to each cell for content changes
   addCellListeners(notebookPanel.content);
 
   if (!notebookPanel?.content?.model) return;
-  // Listen for when new cells are added to the notebook
+  // Listen for when new cells are axdded to the notebook
   notebookPanel.content.model.cells.changed.connect(() => {
     addCellListeners(notebookPanel.content);
   });
+
+  // Listen for cell execution events
+  // notebookPanel.sessionContext.session?.kernel?.anyMessage.connect((_, data) => {
+  //   console.log('msg', data)
+  //   console.log(isErrorMsg(data.msg))
+  //   if (isErrorMsg(data.msg)) {
+  //     onCellExecutionError(notebookPanel, data.msg.content);
+  //   }
+  // });
 }
 
 
 function addCodeToActiveCell(notebook: Notebook, code: string) {
   const activeCell = notebook.activeCell;
   if (activeCell) {
     activeCell.model.sharedModel.setSource(code);
@@ -139,15 +148,15 @@
   // Execute the active cell
   NotebookActions.run(notebookPanel.content, notebookPanel.sessionContext).then(
     () => {
       console.log('Cell executed successfully');
     },
     (reason) => {
       console.error('Error executing cell:', reason);
-      onCellExecutionError(notebookPanel, reason);
+      // onCellExecutionError(notebookPanel, reason);
     }
   );
 }
 
 function createNewNotebook(documentManager: IDocumentManager, notebookName: string): void {
   // Define the full path for the new notebook
   const path = `${notebookName}.ipynb`;
```

### Comparing `jupyterlab_athena_analytics-0.5.6/ui-tests/README.md` & `jupyterlab_athena_analytics-0.5.7/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/ui-tests/tests/jupyterlab_athena_analytics.spec.ts` & `jupyterlab_athena_analytics-0.5.7/ui-tests/tests/jupyterlab_athena_analytics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/.gitignore` & `jupyterlab_athena_analytics-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/LICENSE` & `jupyterlab_athena_analytics-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/README.md` & `jupyterlab_athena_analytics-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/pyproject.toml` & `jupyterlab_athena_analytics-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.6/PKG-INFO` & `jupyterlab_athena_analytics-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_athena_analytics
-Version: 0.5.6
+Version: 0.5.7
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_athena_analytics
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_athena_analytics/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_athena_analytics.git
 Author-email: Athena Intelligence <team@athenaintelligence.ai>
 License: BSD 3-Clause License
```

