# Comparing `tmp/amphi-etl-0.3.7.tar.gz` & `tmp/amphi-etl-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amphi-etl-0.3.7.tar", last modified: Tue May 21 05:35:04 2024, max compression
+gzip compressed data, was "amphi-etl-0.3.8.tar", last modified: Tue May 21 05:59:07 2024, max compression
```

## Comparing `amphi-etl-0.3.7.tar` & `amphi-etl-0.3.8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.931077 amphi-etl-0.3.7/
--rw-r--r--   0 thibaut    (501) staff       (20)     3795 2024-03-22 17:55:16.000000 amphi-etl-0.3.7/LICENSE
--rw-r--r--   0 thibaut    (501) staff       (20)      646 2024-05-17 20:22:58.000000 amphi-etl-0.3.7/MANIFEST.in
--rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-21 05:35:04.930777 amphi-etl-0.3.7/PKG-INFO
--rw-r--r--   0 thibaut    (501) staff       (20)     1770 2024-03-22 18:05:50.000000 amphi-etl-0.3.7/README.md
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.911344 amphi-etl-0.3.7/amphi/
--rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-15 18:36:08.000000 amphi-etl-0.3.7/amphi/__init__.py
--rw-r--r--   0 thibaut    (501) staff       (20)      171 2024-05-21 05:32:46.000000 amphi-etl-0.3.7/amphi/_version.py
--rw-r--r--   0 thibaut    (501) staff       (20)     1007 2024-05-21 05:31:35.000000 amphi-etl-0.3.7/amphi/main.py
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.911923 amphi-etl-0.3.7/amphi/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)    23618 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/build_log.json
--rw-r--r--   0 thibaut    (501) staff       (20)     2699 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.913253 amphi-etl-0.3.7/amphi/theme-light/static/
--rw-r--r--   0 thibaut    (501) staff       (20)     1584 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js
--rw-r--r--   0 thibaut    (501) staff       (20)      933 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)    27264 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js
--rw-r--r--   0 thibaut    (501) staff       (20)    25995 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)      118 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/static/style.js
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.905404 amphi-etl-0.3.7/amphi/theme-light/themes/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.905486 amphi-etl-0.3.7/amphi/theme-light/themes/@amphi/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.913699 amphi-etl-0.3.7/amphi/theme-light/themes/@amphi/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)    37650 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/themes/@amphi/theme-light/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)        0 2024-05-21 05:32:29.000000 amphi-etl-0.3.7/amphi/theme-light/themes/@amphi/theme-light/index.js
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.914054 amphi-etl-0.3.7/amphi/ui-component/
--rw-r--r--   0 thibaut    (501) staff       (20)    22518 2024-05-21 05:32:32.000000 amphi-etl-0.3.7/amphi/ui-component/build_log.json
--rw-r--r--   0 thibaut    (501) staff       (20)     2764 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.916408 amphi-etl-0.3.7/amphi/ui-component/static/
--rw-r--r--   0 thibaut    (501) staff       (20)    64203 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js
--rw-r--r--   0 thibaut    (501) staff       (20)    37982 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)    58944 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js
--rw-r--r--   0 thibaut    (501) staff       (20)    73309 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)    30264 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js
--rw-r--r--   0 thibaut    (501) staff       (20)    29057 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)      162 2024-05-21 05:32:32.000000 amphi-etl-0.3.7/amphi/ui-component/static/style.js
--rw-r--r--   0 thibaut    (501) staff       (20)    14477 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js
--rw-r--r--   0 thibaut    (501) staff       (20)     5614 2024-05-21 05:32:33.000000 amphi-etl-0.3.7/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.917586 amphi-etl-0.3.7/amphi_etl.egg-info/
--rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-21 05:35:04.000000 amphi-etl-0.3.7/amphi_etl.egg-info/PKG-INFO
--rw-r--r--   0 thibaut    (501) staff       (20)     3816 2024-05-21 05:35:04.000000 amphi-etl-0.3.7/amphi_etl.egg-info/SOURCES.txt
--rw-r--r--   0 thibaut    (501) staff       (20)        1 2024-05-21 05:35:04.000000 amphi-etl-0.3.7/amphi_etl.egg-info/dependency_links.txt
--rw-r--r--   0 thibaut    (501) staff       (20)       42 2024-05-21 05:35:04.000000 amphi-etl-0.3.7/amphi_etl.egg-info/entry_points.txt
--rw-r--r--   0 thibaut    (501) staff       (20)       57 2024-05-21 05:35:04.000000 amphi-etl-0.3.7/amphi_etl.egg-info/requires.txt
--rw-r--r--   0 thibaut    (501) staff       (20)        6 2024-05-21 05:35:04.000000 amphi-etl-0.3.7/amphi_etl.egg-info/top_level.txt
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.906102 amphi-etl-0.3.7/config/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.917756 amphi-etl-0.3.7/config/labconfig/
--rw-r--r--   0 thibaut    (501) staff       (20)      680 2024-05-15 22:02:31.000000 amphi-etl-0.3.7/config/labconfig/page_config.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.917953 amphi-etl-0.3.7/config/settings/
--rw-r--r--   0 thibaut    (501) staff       (20)     2679 2024-05-15 22:26:33.000000 amphi-etl-0.3.7/config/settings/overrides.json
--rw-r--r--   0 thibaut    (501) staff       (20)     3187 2024-05-21 05:32:16.000000 amphi-etl-0.3.7/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.906628 amphi-etl-0.3.7/packages/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.918548 amphi-etl-0.3.7/packages/theme-light/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.919450 amphi-etl-0.3.7/packages/theme-light/lib/
--rw-r--r--   0 thibaut    (501) staff       (20)      214 2024-05-20 16:47:00.000000 amphi-etl-0.3.7/packages/theme-light/lib/index.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)      584 2024-05-20 16:47:00.000000 amphi-etl-0.3.7/packages/theme-light/lib/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)     2583 2024-05-17 20:42:53.000000 amphi-etl-0.3.7/packages/theme-light/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.919684 amphi-etl-0.3.7/packages/theme-light/src/
--rw-r--r--   0 thibaut    (501) staff       (20)      683 2024-03-22 18:05:01.000000 amphi-etl-0.3.7/packages/theme-light/src/index.ts
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.920371 amphi-etl-0.3.7/packages/theme-light/style/
--rw-r--r--   0 thibaut    (501) staff       (20)    23012 2024-05-20 20:54:31.000000 amphi-etl-0.3.7/packages/theme-light/style/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)    14663 2024-05-20 17:28:49.000000 amphi-etl-0.3.7/packages/theme-light/style/variables.css
--rw-r--r--   0 thibaut    (501) staff       (20)      135 2024-03-22 18:05:01.000000 amphi-etl-0.3.7/packages/theme-light/tsconfig.json
--rw-r--r--   0 thibaut    (501) staff       (20)    62340 2024-05-20 16:47:00.000000 amphi-etl-0.3.7/packages/theme-light/tsconfig.tsbuildinfo
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.921194 amphi-etl-0.3.7/packages/ui-component/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.923618 amphi-etl-0.3.7/packages/ui-component/lib/
--rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/BrowseFileDialog.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     6922 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/BrowseFileDialog.js
--rw-r--r--   0 thibaut    (501) staff       (20)      729 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/Dropzone.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     2229 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/Dropzone.js
--rw-r--r--   0 thibaut    (501) staff       (20)      529 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/icons.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     1861 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/icons.js
--rw-r--r--   0 thibaut    (501) staff       (20)      255 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/index.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     5217 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)     1127 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/launcher.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)    13920 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/lib/launcher.js
--rw-r--r--   0 thibaut    (501) staff       (20)     2622 2024-05-17 20:42:59.000000 amphi-etl-0.3.7/packages/ui-component/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.924842 amphi-etl-0.3.7/packages/ui-component/src/
--rw-r--r--   0 thibaut    (501) staff       (20)     7188 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/src/BrowseFileDialog.tsx
--rw-r--r--   0 thibaut    (501) staff       (20)     2814 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/src/Dropzone.tsx
--rw-r--r--   0 thibaut    (501) staff       (20)       74 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/src/declarations.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     1831 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/src/icons.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     5084 2024-05-15 17:04:08.000000 amphi-etl-0.3.7/packages/ui-component/src/index.ts
--rw-r--r--   0 thibaut    (501) staff       (20)    12567 2024-05-15 16:58:31.000000 amphi-etl-0.3.7/packages/ui-component/src/launcher.tsx
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.925622 amphi-etl-0.3.7/packages/ui-component/style/
--rw-r--r--   0 thibaut    (501) staff       (20)      403 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/base.css
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:35:04.930407 amphi-etl-0.3.7/packages/ui-component/style/icons/
--rw-r--r--   0 thibaut    (501) staff       (20)     2857 2024-03-22 20:46:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/amphi-square-logo.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     3001 2024-03-22 20:45:41.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2838 2024-03-22 20:46:22.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/amphi.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     1227 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/bug-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     1204 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/bug-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/code-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      496 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/code-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      432 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/docs-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      479 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/docs-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      924 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/network-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      330 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/p5-asterisk.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2895 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/p5-square-logo.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      687 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      702 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2703 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2717 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline_negative.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      845 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/shield-check-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      472 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/icons/upload-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      289 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)      307 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/style/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)    18439 2024-05-15 17:05:28.000000 amphi-etl-0.3.7/packages/ui-component/style/output.css
--rw-r--r--   0 thibaut    (501) staff       (20)      277 2024-05-15 16:52:04.000000 amphi-etl-0.3.7/packages/ui-component/tailwind.config.js
--rw-r--r--   0 thibaut    (501) staff       (20)      620 2024-03-22 18:05:02.000000 amphi-etl-0.3.7/packages/ui-component/tsconfig.json
--rw-r--r--   0 thibaut    (501) staff       (20)    70461 2024-05-20 16:47:05.000000 amphi-etl-0.3.7/packages/ui-component/tsconfig.tsbuildinfo
--rw-r--r--   0 thibaut    (501) staff       (20)     2603 2024-05-17 20:43:36.000000 amphi-etl-0.3.7/pyproject.toml
--rw-r--r--   0 thibaut    (501) staff       (20)       38 2024-05-21 05:35:04.931157 amphi-etl-0.3.7/setup.cfg
--rw-r--r--   0 thibaut    (501) staff       (20)     1745 2024-05-21 05:32:16.000000 amphi-etl-0.3.7/setup.py
--rw-r--r--   0 thibaut    (501) staff       (20)       66 2024-03-22 17:55:16.000000 amphi-etl-0.3.7/tsconfig.eslint.json
--rw-r--r--   0 thibaut    (501) staff       (20)      513 2024-03-22 17:55:16.000000 amphi-etl-0.3.7/tsconfigbase.json
--rw-r--r--   0 thibaut    (501) staff       (20)   363863 2024-05-20 16:46:47.000000 amphi-etl-0.3.7/yarn.lock
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.644932 amphi-etl-0.3.8/
+-rw-r--r--   0 thibaut    (501) staff       (20)     3795 2024-03-22 17:55:16.000000 amphi-etl-0.3.8/LICENSE
+-rw-r--r--   0 thibaut    (501) staff       (20)      646 2024-05-17 20:22:58.000000 amphi-etl-0.3.8/MANIFEST.in
+-rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-21 05:59:07.644642 amphi-etl-0.3.8/PKG-INFO
+-rw-r--r--   0 thibaut    (501) staff       (20)     1770 2024-03-22 18:05:50.000000 amphi-etl-0.3.8/README.md
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.630527 amphi-etl-0.3.8/amphi/
+-rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-15 18:36:08.000000 amphi-etl-0.3.8/amphi/__init__.py
+-rw-r--r--   0 thibaut    (501) staff       (20)      171 2024-05-21 05:58:39.000000 amphi-etl-0.3.8/amphi/_version.py
+-rw-r--r--   0 thibaut    (501) staff       (20)     1196 2024-05-21 05:56:13.000000 amphi-etl-0.3.8/amphi/main.py
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.630893 amphi-etl-0.3.8/amphi/theme-light/
+-rw-r--r--   0 thibaut    (501) staff       (20)    23618 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/build_log.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     2699 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.631737 amphi-etl-0.3.8/amphi/theme-light/static/
+-rw-r--r--   0 thibaut    (501) staff       (20)     1584 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      933 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)    27264 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    25995 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)      118 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/static/style.js
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.626497 amphi-etl-0.3.8/amphi/theme-light/themes/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.626566 amphi-etl-0.3.8/amphi/theme-light/themes/@amphi/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.632119 amphi-etl-0.3.8/amphi/theme-light/themes/@amphi/theme-light/
+-rw-r--r--   0 thibaut    (501) staff       (20)    37650 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/themes/@amphi/theme-light/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)        0 2024-05-21 05:58:24.000000 amphi-etl-0.3.8/amphi/theme-light/themes/@amphi/theme-light/index.js
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.632716 amphi-etl-0.3.8/amphi/ui-component/
+-rw-r--r--   0 thibaut    (501) staff       (20)    22518 2024-05-21 05:58:26.000000 amphi-etl-0.3.8/amphi/ui-component/build_log.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     2764 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.634644 amphi-etl-0.3.8/amphi/ui-component/static/
+-rw-r--r--   0 thibaut    (501) staff       (20)    64203 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    37982 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)    58944 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    73309 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)    30264 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    29057 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)      162 2024-05-21 05:58:26.000000 amphi-etl-0.3.8/amphi/ui-component/static/style.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    14477 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     5614 2024-05-21 05:58:27.000000 amphi-etl-0.3.8/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.635741 amphi-etl-0.3.8/amphi_etl.egg-info/
+-rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-21 05:59:07.000000 amphi-etl-0.3.8/amphi_etl.egg-info/PKG-INFO
+-rw-r--r--   0 thibaut    (501) staff       (20)     3816 2024-05-21 05:59:07.000000 amphi-etl-0.3.8/amphi_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)        1 2024-05-21 05:59:07.000000 amphi-etl-0.3.8/amphi_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)       42 2024-05-21 05:59:07.000000 amphi-etl-0.3.8/amphi_etl.egg-info/entry_points.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)       57 2024-05-21 05:59:07.000000 amphi-etl-0.3.8/amphi_etl.egg-info/requires.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)        6 2024-05-21 05:59:07.000000 amphi-etl-0.3.8/amphi_etl.egg-info/top_level.txt
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.627156 amphi-etl-0.3.8/config/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.635947 amphi-etl-0.3.8/config/labconfig/
+-rw-r--r--   0 thibaut    (501) staff       (20)      680 2024-05-15 22:02:31.000000 amphi-etl-0.3.8/config/labconfig/page_config.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.636148 amphi-etl-0.3.8/config/settings/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2679 2024-05-15 22:26:33.000000 amphi-etl-0.3.8/config/settings/overrides.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     3187 2024-05-21 05:55:37.000000 amphi-etl-0.3.8/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.627690 amphi-etl-0.3.8/packages/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.636735 amphi-etl-0.3.8/packages/theme-light/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.637112 amphi-etl-0.3.8/packages/theme-light/lib/
+-rw-r--r--   0 thibaut    (501) staff       (20)      214 2024-05-20 16:47:00.000000 amphi-etl-0.3.8/packages/theme-light/lib/index.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)      584 2024-05-20 16:47:00.000000 amphi-etl-0.3.8/packages/theme-light/lib/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2583 2024-05-17 20:42:53.000000 amphi-etl-0.3.8/packages/theme-light/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.637295 amphi-etl-0.3.8/packages/theme-light/src/
+-rw-r--r--   0 thibaut    (501) staff       (20)      683 2024-03-22 18:05:01.000000 amphi-etl-0.3.8/packages/theme-light/src/index.ts
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.637643 amphi-etl-0.3.8/packages/theme-light/style/
+-rw-r--r--   0 thibaut    (501) staff       (20)    23012 2024-05-20 20:54:31.000000 amphi-etl-0.3.8/packages/theme-light/style/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)    14663 2024-05-20 17:28:49.000000 amphi-etl-0.3.8/packages/theme-light/style/variables.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      135 2024-03-22 18:05:01.000000 amphi-etl-0.3.8/packages/theme-light/tsconfig.json
+-rw-r--r--   0 thibaut    (501) staff       (20)    62340 2024-05-20 16:47:00.000000 amphi-etl-0.3.8/packages/theme-light/tsconfig.tsbuildinfo
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.638326 amphi-etl-0.3.8/packages/ui-component/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.639957 amphi-etl-0.3.8/packages/ui-component/lib/
+-rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/BrowseFileDialog.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     6922 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/BrowseFileDialog.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      729 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/Dropzone.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     2229 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/Dropzone.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      529 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/icons.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     1861 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/icons.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      255 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/index.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     5217 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     1127 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/launcher.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)    13920 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/lib/launcher.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2622 2024-05-17 20:42:59.000000 amphi-etl-0.3.8/packages/ui-component/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.640939 amphi-etl-0.3.8/packages/ui-component/src/
+-rw-r--r--   0 thibaut    (501) staff       (20)     7188 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/src/BrowseFileDialog.tsx
+-rw-r--r--   0 thibaut    (501) staff       (20)     2814 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/src/Dropzone.tsx
+-rw-r--r--   0 thibaut    (501) staff       (20)       74 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/src/declarations.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     1831 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/src/icons.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     5084 2024-05-15 17:04:08.000000 amphi-etl-0.3.8/packages/ui-component/src/index.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)    12567 2024-05-15 16:58:31.000000 amphi-etl-0.3.8/packages/ui-component/src/launcher.tsx
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.641543 amphi-etl-0.3.8/packages/ui-component/style/
+-rw-r--r--   0 thibaut    (501) staff       (20)      403 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/base.css
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-21 05:59:07.644246 amphi-etl-0.3.8/packages/ui-component/style/icons/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2857 2024-03-22 20:46:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/amphi-square-logo.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     3001 2024-03-22 20:45:41.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2838 2024-03-22 20:46:22.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/amphi.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1227 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/bug-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1204 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/bug-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/code-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      496 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/code-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      432 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/docs-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      479 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/docs-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      924 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/network-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      330 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/p5-asterisk.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2895 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/p5-square-logo.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      687 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      702 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2703 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2717 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline_negative.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      845 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/shield-check-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      472 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/icons/upload-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      289 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      307 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/style/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    18439 2024-05-15 17:05:28.000000 amphi-etl-0.3.8/packages/ui-component/style/output.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      277 2024-05-15 16:52:04.000000 amphi-etl-0.3.8/packages/ui-component/tailwind.config.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      620 2024-03-22 18:05:02.000000 amphi-etl-0.3.8/packages/ui-component/tsconfig.json
+-rw-r--r--   0 thibaut    (501) staff       (20)    70461 2024-05-20 16:47:05.000000 amphi-etl-0.3.8/packages/ui-component/tsconfig.tsbuildinfo
+-rw-r--r--   0 thibaut    (501) staff       (20)     2603 2024-05-17 20:43:36.000000 amphi-etl-0.3.8/pyproject.toml
+-rw-r--r--   0 thibaut    (501) staff       (20)       38 2024-05-21 05:59:07.644982 amphi-etl-0.3.8/setup.cfg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1745 2024-05-21 05:58:13.000000 amphi-etl-0.3.8/setup.py
+-rw-r--r--   0 thibaut    (501) staff       (20)       66 2024-03-22 17:55:16.000000 amphi-etl-0.3.8/tsconfig.eslint.json
+-rw-r--r--   0 thibaut    (501) staff       (20)      513 2024-03-22 17:55:16.000000 amphi-etl-0.3.8/tsconfigbase.json
+-rw-r--r--   0 thibaut    (501) staff       (20)   363863 2024-05-20 16:46:47.000000 amphi-etl-0.3.8/yarn.lock
```

### Comparing `amphi-etl-0.3.7/LICENSE` & `amphi-etl-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/MANIFEST.in` & `amphi-etl-0.3.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/PKG-INFO` & `amphi-etl-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amphi-etl
-Version: 0.3.7
+Version: 0.3.8
 Summary: Amphi is a python-based ETL
 Author: Thibaut Gourdel
 Author-email: tgourdel@amphi.ai
 License: Elastic License 2.0 \(ELv2\)
         
         **Acceptance** By using the software, you agree to all of the terms and conditions below.
```

### Comparing `amphi-etl-0.3.7/README.md` & `amphi-etl-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/main.py` & `amphi-etl-0.3.8/amphi/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import subprocess
 import sys
 import argparse
 import os
 
 def main():
     parser = argparse.ArgumentParser(description='Amphi ETL Command Line Interface')
-    parser.add_argument('command', choices=['start'], help='Command to execute')
-    parser.add_argument('-w', '--workspace', default='.', help='Workspace directory for JupyterLab')
+    parser.add_argument('command', choices=['start'], help='Command to start Amphi ETL')
+    parser.add_argument('-w', '--workspace', default='.', help='Workspace directory for Amphi ETL')
+    parser.add_argument('-p', '--port', type=int, default=8888, help='Port for Amphi ETL')
 
     args = parser.parse_args()
 
     # Debugging logs
     print(f"Received command: {args.command}")
     print(f"Workspace directory: {args.workspace}")
+    print(f"Port: {args.port}")
     print(f"Python executable: {sys.executable}")
     print(f"Environment PATH: {os.environ.get('PATH')}")
 
     if args.command == 'start':
-        jupyter_command = [sys.executable, '-m', 'jupyter', 'lab', f'--notebook-dir={args.workspace}']
+        jupyter_command = [
+            sys.executable, '-m', 'jupyter', 'lab', 
+            f'--notebook-dir={args.workspace}', f'--port={args.port}'
+        ]
         print(f"Running JupyterLab command: {' '.join(jupyter_command)}")
         try:
             subprocess.check_call(jupyter_command)
         except subprocess.CalledProcessError as e:
             print(f"Failed to start Amphi: {e}")
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `amphi-etl-0.3.7/amphi/theme-light/build_log.json` & `amphi-etl-0.3.8/amphi/theme-light/build_log.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/theme-light/package.json` & `amphi-etl-0.3.8/amphi/theme-light/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js` & `amphi-etl-0.3.8/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map` & `amphi-etl-0.3.8/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js` & `amphi-etl-0.3.8/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map` & `amphi-etl-0.3.8/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/theme-light/themes/@amphi/theme-light/index.css` & `amphi-etl-0.3.8/amphi/theme-light/themes/@amphi/theme-light/index.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/build_log.json` & `amphi-etl-0.3.8/amphi/ui-component/build_log.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/package.json` & `amphi-etl-0.3.8/amphi/ui-component/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js` & `amphi-etl-0.3.8/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map` & `amphi-etl-0.3.8/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js` & `amphi-etl-0.3.8/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map` & `amphi-etl-0.3.8/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js` & `amphi-etl-0.3.8/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map` & `amphi-etl-0.3.8/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js` & `amphi-etl-0.3.8/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map` & `amphi-etl-0.3.8/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/amphi_etl.egg-info/PKG-INFO` & `amphi-etl-0.3.8/amphi_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amphi-etl
-Version: 0.3.7
+Version: 0.3.8
 Summary: Amphi is a python-based ETL
 Author: Thibaut Gourdel
 Author-email: tgourdel@amphi.ai
 License: Elastic License 2.0 \(ELv2\)
         
         **Acceptance** By using the software, you agree to all of the terms and conditions below.
```

### Comparing `amphi-etl-0.3.7/amphi_etl.egg-info/SOURCES.txt` & `amphi-etl-0.3.8/amphi_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/config/labconfig/page_config.json` & `amphi-etl-0.3.8/config/labconfig/page_config.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/config/settings/overrides.json` & `amphi-etl-0.3.8/config/settings/overrides.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/package.json` & `amphi-etl-0.3.8/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.8'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.7",
+    "version": "0.3.8",
     "workspaces": {
         "packages": [
             "packages/theme-light",
             "packages/ui-component"
         ]
     }
 }
```

### Comparing `amphi-etl-0.3.7/packages/theme-light/lib/index.js` & `amphi-etl-0.3.8/packages/theme-light/lib/index.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/theme-light/package.json` & `amphi-etl-0.3.8/packages/theme-light/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/theme-light/src/index.ts` & `amphi-etl-0.3.8/packages/theme-light/src/index.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/theme-light/style/index.css` & `amphi-etl-0.3.8/packages/theme-light/style/index.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/theme-light/style/variables.css` & `amphi-etl-0.3.8/packages/theme-light/style/variables.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/theme-light/tsconfig.tsbuildinfo` & `amphi-etl-0.3.8/packages/theme-light/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/BrowseFileDialog.js` & `amphi-etl-0.3.8/packages/ui-component/lib/BrowseFileDialog.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/Dropzone.d.ts` & `amphi-etl-0.3.8/packages/ui-component/lib/Dropzone.d.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/Dropzone.js` & `amphi-etl-0.3.8/packages/ui-component/lib/Dropzone.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/icons.d.ts` & `amphi-etl-0.3.8/packages/ui-component/lib/icons.d.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/icons.js` & `amphi-etl-0.3.8/packages/ui-component/lib/icons.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/index.js` & `amphi-etl-0.3.8/packages/ui-component/lib/index.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/launcher.d.ts` & `amphi-etl-0.3.8/packages/ui-component/lib/launcher.d.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/lib/launcher.js` & `amphi-etl-0.3.8/packages/ui-component/lib/launcher.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/package.json` & `amphi-etl-0.3.8/packages/ui-component/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/src/BrowseFileDialog.tsx` & `amphi-etl-0.3.8/packages/ui-component/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/src/Dropzone.tsx` & `amphi-etl-0.3.8/packages/ui-component/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/src/icons.ts` & `amphi-etl-0.3.8/packages/ui-component/src/icons.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/src/index.ts` & `amphi-etl-0.3.8/packages/ui-component/src/index.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/src/launcher.tsx` & `amphi-etl-0.3.8/packages/ui-component/src/launcher.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/amphi-square-logo.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/amphi-square-logo.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/amphi.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/amphi.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/bug-16.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/bug-16.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/bug-24.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/bug-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/network-24.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/network-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/p5-square-logo.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/p5-square-logo.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline-16.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline-24.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/pipeline_negative.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/pipeline_negative.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/icons/shield-check-24.svg` & `amphi-etl-0.3.8/packages/ui-component/style/icons/shield-check-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/style/output.css` & `amphi-etl-0.3.8/packages/ui-component/style/output.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/tsconfig.json` & `amphi-etl-0.3.8/packages/ui-component/tsconfig.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/packages/ui-component/tsconfig.tsbuildinfo` & `amphi-etl-0.3.8/packages/ui-component/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/pyproject.toml` & `amphi-etl-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/setup.py` & `amphi-etl-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     collect_files('amphi', 'share/jupyter/labextensions/@amphi') +
     collect_files('config/labconfig', 'etc/jupyter/labconfig') +
     collect_files('config/settings', 'share/jupyter/lab/settings')
 )
 
 setup(
     name='amphi-etl',
-    version='0.3.7',
+    version='0.3.8',
     description='Open-source and Python-based ETL',
     author='Thibaut Gourdel',
     author_email='tgourdel@amphi.ai',
     license='ELv2',
     install_requires=[
         'jupyterlab>=4.1.5',
         'jupyterlab-amphi>=0.3.1',
```

### Comparing `amphi-etl-0.3.7/tsconfigbase.json` & `amphi-etl-0.3.8/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.7/yarn.lock` & `amphi-etl-0.3.8/yarn.lock`

 * *Files identical despite different names*

