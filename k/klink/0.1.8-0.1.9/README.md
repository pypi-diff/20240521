# Comparing `tmp/klink-0.1.8.tar.gz` & `tmp/klink-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/klink-0.1.8.tar", last modified: Mon Jul  7 15:17:51 2014, max compression
+gzip compressed data, was "dist/klink-0.1.9.tar", last modified: Tue Jun 16 18:03:46 2015, max compression
```

## Comparing `klink-0.1.8.tar` & `klink-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3847 2014-07-07 14:11:18.000000 klink-0.1.8/README.rst
--rw-rw-r--   0 phil      (1000) phil      (1000)      307 2014-07-07 15:17:51.000000 klink-0.1.8/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)       12 2014-07-01 20:03:33.000000 klink-0.1.8/MANIFEST.in
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1584 2014-07-07 15:17:51.000000 klink-0.1.8/klink.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      307 2014-07-07 15:17:51.000000 klink-0.1.8/klink.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)        6 2014-07-07 15:17:51.000000 klink-0.1.8/klink.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2014-07-07 15:17:51.000000 klink-0.1.8/klink.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       59 2014-07-07 15:17:51.000000 klink-0.1.8/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      382 2014-07-03 12:56:35.000000 klink-0.1.8/setup.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1949 2014-07-04 19:18:04.000000 klink-0.1.8/klink/layout.html
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/less/
--rw-rw-r--   0 phil      (1000) phil      (1000)     6297 2014-07-07 15:14:31.000000 klink-0.1.8/klink/less/klink.less
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/less/vendor/
--rw-rw-r--   0 phil      (1000) phil      (1000)    56552 2014-07-01 20:03:33.000000 klink-0.1.8/klink/less/vendor/3L.less
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/less/vendor/font-awesome/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/
--rw-rw-r--   0 phil      (1000) phil      (1000)      330 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/bordered-pulled.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      699 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/mixins.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      476 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/stacked.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      699 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/path.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      119 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/fixed-width.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      367 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/rotated-flipped.less
--rw-rw-r--   0 phil      (1000) phil      (1000)       40 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/extras.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      270 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/core.less
--rw-rw-r--   0 phil      (1000) phil      (1000)    31652 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/icons.less
--rw-rw-r--   0 phil      (1000) phil      (1000)    14295 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/variables.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      375 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/list.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      465 2014-07-02 17:45:38.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/font-awesome.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      370 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/larger.less
--rw-rw-r--   0 phil      (1000) phil      (1000)      749 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/less/spinning.less
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/less/vendor/font-awesome/fonts/
--rwxrwxr-x   0 phil      (1000) phil      (1000)   253487 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 phil      (1000) phil      (1000)    75188 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/fonts/FontAwesome.otf
--rwxrwxr-x   0 phil      (1000) phil      (1000)    83760 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.woff
--rwxrwxr-x   0 phil      (1000) phil      (1000)   141564 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.ttf
--rwxrwxr-x   0 phil      (1000) phil      (1000)    72449 2014-07-02 17:44:26.000000 klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.eot
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/static/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/static/fonts/
--rwxrwxr-x   0 phil      (1000) phil      (1000)   253487 2014-07-02 17:50:18.000000 klink-0.1.8/klink/static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 phil      (1000) phil      (1000)    75188 2014-07-02 17:50:18.000000 klink-0.1.8/klink/static/fonts/FontAwesome.otf
--rwxrwxr-x   0 phil      (1000) phil      (1000)    83760 2014-07-02 17:50:18.000000 klink-0.1.8/klink/static/fonts/fontawesome-webfont.woff
--rwxrwxr-x   0 phil      (1000) phil      (1000)   141564 2014-07-02 17:50:18.000000 klink-0.1.8/klink/static/fonts/fontawesome-webfont.ttf
--rwxrwxr-x   0 phil      (1000) phil      (1000)    72449 2014-07-02 17:50:18.000000 klink-0.1.8/klink/static/fonts/fontawesome-webfont.eot
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/static/css/
--rw-rw-r--   0 phil      (1000) phil      (1000)    29586 2014-07-07 15:17:20.000000 klink-0.1.8/klink/static/css/klink.css
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2014-07-07 15:17:51.000000 klink-0.1.8/klink/static/img/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3167 2014-07-01 20:03:33.000000 klink-0.1.8/klink/static/img/logo.png
--rw-rw-r--   0 phil      (1000) phil      (1000)     1035 2014-07-01 20:03:33.000000 klink-0.1.8/klink/static/img/favicon.ico
--rw-rw-r--   0 phil      (1000) phil      (1000)     2609 2014-07-07 15:17:12.000000 klink-0.1.8/klink/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1572 2014-07-07 15:09:36.000000 klink-0.1.8/klink/demo.pyc
--rw-rw-r--   0 phil      (1000) phil      (1000)     1002 2014-07-07 15:09:11.000000 klink-0.1.8/klink/demo.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2846 2014-07-07 15:17:20.000000 klink-0.1.8/klink/__init__.pyc
--rw-rw-r--   0 phil      (1000) phil      (1000)      103 2014-07-01 20:03:33.000000 klink-0.1.8/klink/theme.conf
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/
+-rw-rw-r--   0 phil      (1001) phil      (1001)       59 2015-06-16 18:03:46.000000 klink-0.1.9/setup.cfg
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink.egg-info/
+-rw-rw-r--   0 phil      (1001) phil      (1001)        1 2015-06-16 18:03:45.000000 klink-0.1.9/klink.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1001) phil      (1001)        6 2015-06-16 18:03:45.000000 klink-0.1.9/klink.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1001) phil      (1001)      307 2015-06-16 18:03:45.000000 klink-0.1.9/klink.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1001) phil      (1001)     1584 2015-06-16 18:03:45.000000 klink-0.1.9/klink.egg-info/SOURCES.txt
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/
+-rw-rw-r--   0 phil      (1001) phil      (1001)      103 2015-06-15 13:41:19.000000 klink-0.1.9/klink/theme.conf
+-rw-rw-r--   0 phil      (1001) phil      (1001)     2798 2015-06-16 18:01:04.000000 klink-0.1.9/klink/__init__.pyc
+-rw-rw-r--   0 phil      (1001) phil      (1001)     2609 2015-06-16 18:00:38.000000 klink-0.1.9/klink/__init__.py
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/static/
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/static/fonts/
+-rwxrwxr-x   0 phil      (1001) phil      (1001)    83760 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/fonts/fontawesome-webfont.woff
+-rwxrwxr-x   0 phil      (1001) phil      (1001)    72449 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/fonts/fontawesome-webfont.eot
+-rwxrwxr-x   0 phil      (1001) phil      (1001)   253487 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 phil      (1001) phil      (1001)    75188 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/fonts/FontAwesome.otf
+-rwxrwxr-x   0 phil      (1001) phil      (1001)   141564 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/fonts/fontawesome-webfont.ttf
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/static/img/
+-rw-rw-r--   0 phil      (1001) phil      (1001)     1035 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/img/favicon.ico
+-rw-rw-r--   0 phil      (1001) phil      (1001)     3167 2015-06-15 13:41:19.000000 klink-0.1.9/klink/static/img/logo.png
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/static/css/
+-rw-rw-r--   0 phil      (1001) phil      (1001)    36431 2015-06-16 18:01:02.000000 klink-0.1.9/klink/static/css/klink.css
+-rw-rw-r--   0 phil      (1001) phil      (1001)     1967 2015-06-15 15:07:09.000000 klink-0.1.9/klink/layout.html
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/less/
+-rw-rw-r--   0 phil      (1001) phil      (1001)     6456 2015-06-15 18:34:32.000000 klink-0.1.9/klink/less/klink.less
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/less/vendor/
+-rw-rw-r--   0 phil      (1001) phil      (1001)    56552 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/3L.less
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/less/vendor/font-awesome/
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/less/vendor/font-awesome/fonts/
+-rwxrwxr-x   0 phil      (1001) phil      (1001)    83760 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.woff
+-rwxrwxr-x   0 phil      (1001) phil      (1001)    72449 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.eot
+-rwxrwxr-x   0 phil      (1001) phil      (1001)   253487 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 phil      (1001) phil      (1001)    75188 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/fonts/FontAwesome.otf
+-rwxrwxr-x   0 phil      (1001) phil      (1001)   141564 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.ttf
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2015-06-16 18:03:46.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/
+-rw-rw-r--   0 phil      (1001) phil      (1001)      476 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/stacked.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      699 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/path.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      375 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/list.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      330 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/bordered-pulled.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)    14295 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/variables.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      465 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/font-awesome.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      119 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/fixed-width.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)    31652 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/icons.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)       40 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/extras.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      367 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/rotated-flipped.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      270 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/core.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      699 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/mixins.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      370 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/larger.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)      749 2015-06-15 13:41:19.000000 klink-0.1.9/klink/less/vendor/font-awesome/less/spinning.less
+-rw-rw-r--   0 phil      (1001) phil      (1001)     1524 2015-06-15 13:44:07.000000 klink-0.1.9/klink/demo.pyc
+-rw-rw-r--   0 phil      (1001) phil      (1001)     1002 2015-06-15 13:41:19.000000 klink-0.1.9/klink/demo.py
+-rw-rw-r--   0 phil      (1001) phil      (1001)     3847 2015-06-15 13:41:19.000000 klink-0.1.9/README.rst
+-rw-rw-r--   0 phil      (1001) phil      (1001)      307 2015-06-16 18:03:46.000000 klink-0.1.9/PKG-INFO
+-rw-rw-r--   0 phil      (1001) phil      (1001)      527 2015-06-16 18:00:03.000000 klink-0.1.9/setup.py
+-rw-rw-r--   0 phil      (1001) phil      (1001)       12 2015-06-15 13:41:19.000000 klink-0.1.9/MANIFEST.in
```

### Comparing `klink-0.1.8/README.rst` & `klink-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink.egg-info/SOURCES.txt` & `klink-0.1.9/klink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/layout.html` & `klink-0.1.9/klink/layout.html`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     {%- block sidebar2 %}
         <aside>
 
             {% if theme_logo %}
             <a href="{{ pathto('index') }}" id="logo" title={{project}}><img class="logo" src="{{ pathto('_static/' + theme_logo, 1) }}" width="150px" height="150px" title={{project}} /></a>
             {% endif %}
             
-            {{ toctree() }}
+            {{ toctree(includehidden=True) }}
 
             {% if theme_github %}
             <ul>
                 <li><a href="https://github.com/{{theme_github}}">Github</a></li>
             </ul>
             {% endif %}
```

### Comparing `klink-0.1.8/klink/less/klink.less` & `klink-0.1.9/klink/less/klink.less`

 * *Files 2% similar despite different names*

```diff
@@ -366,14 +366,24 @@
     font-size: 0.9em;
     max-width: 98%;
     margin: 0 auto;
     
     table, p {
         margin-left: 20px;
     }
+
+    .highlight {
+        background: inherit;
+        border: none;
+
+        pre {
+            background: inherit;
+            border: none;
+        }
+    }
 }
 
 div#searchbox {
     padding-top: 10px;
 }
 
 @media (max-width: 800px) {
```

### Comparing `klink-0.1.8/klink/less/vendor/3L.less` & `klink-0.1.9/klink/less/vendor/3L.less`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/less/mixins.less` & `klink-0.1.9/klink/less/vendor/font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/less/path.less` & `klink-0.1.9/klink/less/vendor/font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/less/icons.less` & `klink-0.1.9/klink/less/vendor/font-awesome/less/icons.less`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/less/variables.less` & `klink-0.1.9/klink/less/vendor/font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/less/spinning.less` & `klink-0.1.9/klink/less/vendor/font-awesome/less/spinning.less`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.svg` & `klink-0.1.9/klink/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/fonts/FontAwesome.otf` & `klink-0.1.9/klink/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.woff` & `klink-0.1.9/klink/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.ttf` & `klink-0.1.9/klink/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.eot` & `klink-0.1.9/klink/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/fonts/fontawesome-webfont.svg` & `klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/fonts/FontAwesome.otf` & `klink-0.1.9/klink/less/vendor/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/fonts/fontawesome-webfont.woff` & `klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/fonts/fontawesome-webfont.ttf` & `klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/fonts/fontawesome-webfont.eot` & `klink-0.1.9/klink/less/vendor/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/img/logo.png` & `klink-0.1.9/klink/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/static/img/favicon.ico` & `klink-0.1.9/klink/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/__init__.py` & `klink-0.1.9/klink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,10 +78,10 @@
 
 def get_html_theme_path():
     """Returns list of HTML theme paths."""
     cur_dir = os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
     return cur_dir
 
 
-VERSION = (0, 1, 8)
+VERSION = (0, 1, 9)
 __version__ = '.'.join(str(v) for v in VERSION)
 __version_full__ = __version__
```

### Comparing `klink-0.1.8/klink/demo.py` & `klink-0.1.9/klink/demo.py`

 * *Files identical despite different names*

### Comparing `klink-0.1.8/klink/__init__.pyc` & `klink-0.1.9/klink/__init__.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a f8b9 ba53 6300 0000 0000 0000  .......Sc.......
+00000000: 03f3 0d0a 4664 8055 6300 0000 0000 0000  ....Fd.Uc.......
 00000010: 0003 0000 0040 0000 0073 6f00 0000 6400  .....@...so...d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
 00000030: 6c01 006d 0200 5a02 0001 6400 0064 0100  l..m..Z...d..d..
 00000040: 6c03 005a 0300 6400 0064 0100 6c04 005a  l..Z..d..d..l..Z
 00000050: 0400 6403 0084 0000 5a05 0064 0400 8400  ..d.....Z..d....
 00000060: 005a 0600 640a 005a 0700 6408 006a 0800  .Z..d..Z..d..j..
 00000070: 6409 0084 0000 6507 0044 8301 0083 0100  d.....e..D......
@@ -114,65 +114,62 @@
 00000710: 0000 6e61 6d65 7408 0000 006e 6f74 6562  ..namet....noteb
 00000720: 6f6f 6b74 0400 0000 7364 6972 7407 0000  ookt....sdirt...
 00000730: 0073 7461 7469 6373 7408 0000 0072 7374  .staticst....rst
 00000740: 5f66 696c 6574 0400 0000 6461 7461 7401  _filet....datat.
 00000750: 0000 0066 7405 0000 006c 696e 6573 7401  ...ft....linest.
 00000760: 0000 006e 7408 0000 0072 6177 5761 7463  ...nt....rawWatc
 00000770: 6874 0400 0000 6c69 6e65 2800 0000 0028  ht....line(....(
-00000780: 0000 0000 7339 0000 002f 686f 6d65 2f70  ....s9.../home/p
-00000790: 6869 6c2f 4472 6f70 626f 782f 6465 762f  hil/Dropbox/dev/
-000007a0: 7264 612f 7079 7468 6f6e 2f6b 6c69 6e6b  rda/python/klink
-000007b0: 2f6b 6c69 6e6b 2f5f 5f69 6e69 745f 5f2e  /klink/__init__.
-000007c0: 7079 7411 0000 0063 6f6e 7665 7274 5f6e  pyt....convert_n
-000007d0: 6f74 6562 6f6f 6b73 0700 0000 7362 0000  otebooks....sb..
-000007e0: 0000 051b 010c 0113 0219 0127 0129 0219  ...........'.)..
-000007f0: 010a 010a 020f 030a 010f 0128 0123 010d  ...........(.#..
-00000800: 030a 0109 0106 0112 0112 020c 0112 0119  ................
-00000810: 0116 0306 0112 0112 020c 010c 0106 0106  ................
-00000820: 020f 010a 020c 0114 010d 010c 0114 010d  ................
-00000830: 010c 0109 0206 010c 0112 010a 010c 020e  ................
-00000840: 0212 0163 0000 0000 0100 0000 0400 0000  ...c............
-00000850: 4300 0000 732e 0000 0074 0000 6a01 006a  C...s....t..j..j
-00000860: 0200 7400 006a 0100 6a03 0074 0000 6a01  ..t..j..j..t..j.
-00000870: 006a 0300 7404 0083 0100 8301 0083 0100  .j..t...........
-00000880: 7d00 007c 0000 5328 0100 0000 7321 0000  }..|..S(....s!..
-00000890: 0052 6574 7572 6e73 206c 6973 7420 6f66  .Returns list of
-000008a0: 2048 544d 4c20 7468 656d 6520 7061 7468   HTML theme path
-000008b0: 732e 2805 0000 0052 0900 0000 520b 0000  s.(....R....R...
-000008c0: 0074 0700 0000 6162 7370 6174 6874 0700  .t....abspatht..
-000008d0: 0000 6469 726e 616d 6574 0800 0000 5f5f  ..dirnamet....__
-000008e0: 6669 6c65 5f5f 2801 0000 0074 0700 0000  file__(....t....
-000008f0: 6375 725f 6469 7228 0000 0000 2800 0000  cur_dir(....(...
-00000900: 0073 3900 0000 2f68 6f6d 652f 7068 696c  .s9.../home/phil
-00000910: 2f44 726f 7062 6f78 2f64 6576 2f72 6461  /Dropbox/dev/rda
-00000920: 2f70 7974 686f 6e2f 6b6c 696e 6b2f 6b6c  /python/klink/kl
-00000930: 696e 6b2f 5f5f 696e 6974 5f5f 2e70 7974  ink/__init__.pyt
-00000940: 1300 0000 6765 745f 6874 6d6c 5f74 6865  ....get_html_the
-00000950: 6d65 5f70 6174 684f 0000 0073 0400 0000  me_pathO...s....
-00000960: 0002 2a01 6900 0000 0069 0100 0000 6908  ..*.i....i....i.
-00000970: 0000 0052 0400 0000 6301 0000 0002 0000  ...R....c.......
-00000980: 0003 0000 0063 0000 0073 1b00 0000 7c00  .....c...s....|.
-00000990: 005d 1100 7d01 0074 0000 7c01 0083 0100  .]..}..t..|.....
-000009a0: 5601 7103 0064 0000 5328 0100 0000 4e28  V.q..d..S(....N(
-000009b0: 0100 0000 7403 0000 0073 7472 2802 0000  ....t....str(...
-000009c0: 0074 0200 0000 2e30 7401 0000 0076 2800  .t.....0t....v(.
-000009d0: 0000 0028 0000 0000 7339 0000 002f 686f  ...(....s9.../ho
-000009e0: 6d65 2f70 6869 6c2f 4472 6f70 626f 782f  me/phil/Dropbox/
-000009f0: 6465 762f 7264 612f 7079 7468 6f6e 2f6b  dev/rda/python/k
-00000a00: 6c69 6e6b 2f6b 6c69 6e6b 2f5f 5f69 6e69  link/klink/__ini
-00000a10: 745f 5f2e 7079 7309 0000 003c 6765 6e65  t__.pys....<gene
-00000a20: 7870 723e 5600 0000 7302 0000 0006 0028  xpr>V...s......(
-00000a30: 0300 0000 6900 0000 0069 0100 0000 6908  ....i....i....i.
-00000a40: 0000 0028 0b00 0000 5209 0000 0074 0a00  ...(....R....t..
-00000a50: 0000 7375 6270 726f 6365 7373 5200 0000  ..subprocessR...
-00000a60: 0052 1100 0000 5217 0000 0052 3000 0000  .R....R....R0...
-00000a70: 5235 0000 0074 0700 0000 5645 5253 494f  R5...t....VERSIO
-00000a80: 4e52 1000 0000 740b 0000 005f 5f76 6572  NR....t....__ver
-00000a90: 7369 6f6e 5f5f 7410 0000 005f 5f76 6572  sion__t....__ver
-00000aa0: 7369 6f6e 5f66 756c 6c5f 5f28 0000 0000  sion_full__(....
-00000ab0: 2800 0000 0028 0000 0000 7339 0000 002f  (....(....s9.../
-00000ac0: 686f 6d65 2f70 6869 6c2f 4472 6f70 626f  home/phil/Dropbo
-00000ad0: 782f 6465 762f 7264 612f 7079 7468 6f6e  x/dev/rda/python
-00000ae0: 2f6b 6c69 6e6b 2f6b 6c69 6e6b 2f5f 5f69  /klink/klink/__i
-00000af0: 6e69 745f 5f2e 7079 7408 0000 003c 6d6f  nit__.pyt....<mo
-00000b00: 6475 6c65 3e01 0000 0073 1000 0000 0c01  dule>....s......
-00000b10: 1001 0c01 0c03 0948 0906 0601 1901       .......H......
+00000780: 0000 0000 732d 0000 002f 686f 6d65 2f70  ....s-.../home/p
+00000790: 6869 6c2f 6465 762f 7079 7468 6f6e 2f6b  hil/dev/python/k
+000007a0: 6c69 6e6b 2f6b 6c69 6e6b 2f5f 5f69 6e69  link/klink/__ini
+000007b0: 745f 5f2e 7079 7411 0000 0063 6f6e 7665  t__.pyt....conve
+000007c0: 7274 5f6e 6f74 6562 6f6f 6b73 0700 0000  rt_notebooks....
+000007d0: 7362 0000 0000 051b 010c 0113 0219 0127  sb.............'
+000007e0: 0129 0219 010a 010a 020f 030a 010f 0128  .).............(
+000007f0: 0123 010d 030a 0109 0106 0112 0112 020c  .#..............
+00000800: 0112 0119 0116 0306 0112 0112 020c 010c  ................
+00000810: 0106 0106 020f 010a 020c 0114 010d 010c  ................
+00000820: 0114 010d 010c 0109 0206 010c 0112 010a  ................
+00000830: 010c 020e 0212 0163 0000 0000 0100 0000  .......c........
+00000840: 0400 0000 4300 0000 732e 0000 0074 0000  ....C...s....t..
+00000850: 6a01 006a 0200 7400 006a 0100 6a03 0074  j..j..t..j..j..t
+00000860: 0000 6a01 006a 0300 7404 0083 0100 8301  ..j..j..t.......
+00000870: 0083 0100 7d00 007c 0000 5328 0100 0000  ....}..|..S(....
+00000880: 7321 0000 0052 6574 7572 6e73 206c 6973  s!...Returns lis
+00000890: 7420 6f66 2048 544d 4c20 7468 656d 6520  t of HTML theme 
+000008a0: 7061 7468 732e 2805 0000 0052 0900 0000  paths.(....R....
+000008b0: 520b 0000 0074 0700 0000 6162 7370 6174  R....t....abspat
+000008c0: 6874 0700 0000 6469 726e 616d 6574 0800  ht....dirnamet..
+000008d0: 0000 5f5f 6669 6c65 5f5f 2801 0000 0074  ..__file__(....t
+000008e0: 0700 0000 6375 725f 6469 7228 0000 0000  ....cur_dir(....
+000008f0: 2800 0000 0073 2d00 0000 2f68 6f6d 652f  (....s-.../home/
+00000900: 7068 696c 2f64 6576 2f70 7974 686f 6e2f  phil/dev/python/
+00000910: 6b6c 696e 6b2f 6b6c 696e 6b2f 5f5f 696e  klink/klink/__in
+00000920: 6974 5f5f 2e70 7974 1300 0000 6765 745f  it__.pyt....get_
+00000930: 6874 6d6c 5f74 6865 6d65 5f70 6174 684f  html_theme_pathO
+00000940: 0000 0073 0400 0000 0002 2a01 6900 0000  ...s......*.i...
+00000950: 0069 0100 0000 6909 0000 0052 0400 0000  .i....i....R....
+00000960: 6301 0000 0002 0000 0003 0000 0063 0000  c............c..
+00000970: 0073 1b00 0000 7c00 005d 1100 7d01 0074  .s....|..]..}..t
+00000980: 0000 7c01 0083 0100 5601 7103 0064 0000  ..|.....V.q..d..
+00000990: 5328 0100 0000 4e28 0100 0000 7403 0000  S(....N(....t...
+000009a0: 0073 7472 2802 0000 0074 0200 0000 2e30  .str(....t.....0
+000009b0: 7401 0000 0076 2800 0000 0028 0000 0000  t....v(....(....
+000009c0: 732d 0000 002f 686f 6d65 2f70 6869 6c2f  s-.../home/phil/
+000009d0: 6465 762f 7079 7468 6f6e 2f6b 6c69 6e6b  dev/python/klink
+000009e0: 2f6b 6c69 6e6b 2f5f 5f69 6e69 745f 5f2e  /klink/__init__.
+000009f0: 7079 7309 0000 003c 6765 6e65 7870 723e  pys....<genexpr>
+00000a00: 5600 0000 7302 0000 0006 0028 0300 0000  V...s......(....
+00000a10: 6900 0000 0069 0100 0000 6909 0000 0028  i....i....i....(
+00000a20: 0b00 0000 5209 0000 0074 0a00 0000 7375  ....R....t....su
+00000a30: 6270 726f 6365 7373 5200 0000 0052 1100  bprocessR....R..
+00000a40: 0000 5217 0000 0052 3000 0000 5235 0000  ..R....R0...R5..
+00000a50: 0074 0700 0000 5645 5253 494f 4e52 1000  .t....VERSIONR..
+00000a60: 0000 740b 0000 005f 5f76 6572 7369 6f6e  ..t....__version
+00000a70: 5f5f 7410 0000 005f 5f76 6572 7369 6f6e  __t....__version
+00000a80: 5f66 756c 6c5f 5f28 0000 0000 2800 0000  _full__(....(...
+00000a90: 0028 0000 0000 732d 0000 002f 686f 6d65  .(....s-.../home
+00000aa0: 2f70 6869 6c2f 6465 762f 7079 7468 6f6e  /phil/dev/python
+00000ab0: 2f6b 6c69 6e6b 2f6b 6c69 6e6b 2f5f 5f69  /klink/klink/__i
+00000ac0: 6e69 745f 5f2e 7079 7408 0000 003c 6d6f  nit__.pyt....<mo
+00000ad0: 6475 6c65 3e01 0000 0073 1000 0000 0c01  dule>....s......
+00000ae0: 1001 0c01 0c03 0948 0906 0601 1901       .......H......
```

