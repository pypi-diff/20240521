# Comparing `tmp/easy-xedu-0.1.9.tar.gz` & `tmp/easy-xedu-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easy-xedu-0.1.9.tar", last modified: Tue May 21 07:53:49 2024, max compression
+gzip compressed data, was "dist\easy-xedu-0.2.1.tar", last modified: Tue May 21 08:31:14 2024, max compression
```

## Comparing `easy-xedu-0.1.9.tar` & `easy-xedu-0.2.1.tar`

### file list

```diff
@@ -1,326 +1,328 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:49.305792 easy-xedu-0.1.9/
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.433242 easy-xedu-0.1.9/EasyConvert/
--rw-rw-rw-   0        0        0        0 2023-12-25 15:57:21.000000 easy-xedu-0.1.9/EasyConvert/__init__.py
--rw-rw-rw-   0        0        0     6351 2023-12-25 15:57:21.000000 easy-xedu-0.1.9/EasyConvert/easyconvert.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.452220 easy-xedu-0.1.9/EasyTrain/
--rw-rw-rw-   0        0        0        0 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.456222 easy-xedu-0.1.9/EasyTrain/apis/
--rw-rw-rw-   0        0        0        0 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.466922 easy-xedu-0.1.9/EasyTrain/apis/baseml/
--rw-rw-rw-   0        0        0      115 2024-05-17 11:59:45.000000 easy-xedu-0.1.9/EasyTrain/apis/baseml/__init__.py
--rw-rw-rw-   0        0        0     3790 2024-05-21 06:13:01.000000 easy-xedu-0.1.9/EasyTrain/apis/baseml/baseml.py
--rw-rw-rw-   0        0        0     6412 2024-05-21 06:13:57.000000 easy-xedu-0.1.9/EasyTrain/apis/baseml/config.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.478958 easy-xedu-0.1.9/EasyTrain/apis/basenn/
--rw-rw-rw-   0        0        0      115 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/apis/basenn/__init__.py
--rw-rw-rw-   0        0        0     5362 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/apis/basenn/basenn.py
--rw-rw-rw-   0        0        0     8924 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/apis/basenn/config.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.490402 easy-xedu-0.1.9/EasyTrain/apis/mmedu/
--rw-rw-rw-   0        0        0      111 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/apis/mmedu/__init__.py
--rw-rw-rw-   0        0        0    10751 2024-05-21 03:41:38.000000 easy-xedu-0.1.9/EasyTrain/apis/mmedu/config.py
--rw-rw-rw-   0        0        0     8135 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/apis/mmedu/mmedu.py
--rw-rw-rw-   0        0        0      662 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/basenn_code.py
--rw-rw-rw-   0        0        0      636 2024-05-17 10:07:08.000000 easy-xedu-0.1.9/EasyTrain/extensions.py
--rw-rw-rw-   0        0        0      502 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/mmedu_code.py
--rw-rw-rw-   0        0        0    15938 2024-05-21 06:09:34.000000 easy-xedu-0.1.9/EasyTrain/run.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.400673 easy-xedu-0.1.9/EasyTrain/static/
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.502010 easy-xedu-0.1.9/EasyTrain/static/assets/
--rw-rw-rw-   0        0        0      643 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/assets/clipboard-plus.svg
--rw-rw-rw-   0        0        0      935 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/assets/question-diamond.svg
--rw-rw-rw-   0        0        0      497 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/assets/x-square.svg
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.517782 easy-xedu-0.1.9/EasyTrain/static/css/
--rw-rw-rw-   0        0        0     2357 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/css/basenn.css
--rw-rw-rw-   0        0        0   162264 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1309 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/css/github.min.css
--rw-rw-rw-   0        0        0     8039 2024-05-21 06:58:15.000000 easy-xedu-0.1.9/EasyTrain/static/css/style.css
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.551790 easy-xedu-0.1.9/EasyTrain/static/js/
--rw-rw-rw-   0        0        0    42085 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/basenn.js
--rw-rw-rw-   0        0        0    83376 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0     9160 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/clipboard.min.js
--rw-rw-rw-   0        0        0   491315 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/echarts.min.js
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.576789 easy-xedu-0.1.9/EasyTrain/static/js/highlight/
--rw-rw-rw-   0        0        0    38854 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/DIGESTS.md
--rw-rw-rw-   0        0        0     1514 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/LICENSE
--rw-rw-rw-   0        0        0     1717 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.597787 easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/
--rw-rw-rw-   0        0        0    76121 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/core.js
--rw-rw-rw-   0        0        0    20322 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/core.min.js
--rw-rw-rw-   0        0        0    76121 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/highlight.js
--rw-rw-rw-   0        0        0    20322 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/highlight.min.js
--rw-rw-rw-   0        0        0       20 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/package.json
--rw-rw-rw-   0        0        0    80817 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/highlight.js
--rw-rw-rw-   0        0        0    23953 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/highlight.min.js
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.600788 easy-xedu-0.1.9/EasyTrain/static/js/highlight/languages/
--rw-rw-rw-   0        0        0     3529 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/languages/python.min.js
--rw-rw-rw-   0        0        0     2903 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/package.json
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:47.994814 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/
--rw-rw-rw-   0        0        0     1158 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/a11y-dark.min.css
--rw-rw-rw-   0        0        0     1146 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/a11y-light.min.css
--rw-rw-rw-   0        0        0     1357 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/agate.min.css
--rw-rw-rw-   0        0        0      961 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/an-old-hope.min.css
--rw-rw-rw-   0        0        0      611 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/androidstudio.min.css
--rw-rw-rw-   0        0        0      844 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/arduino-light.min.css
--rw-rw-rw-   0        0        0      673 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/arta.min.css
--rw-rw-rw-   0        0        0      454 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/ascetic.min.css
--rw-rw-rw-   0        0        0     1193 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/atom-one-dark-reasonable.min.css
--rw-rw-rw-   0        0        0      856 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/atom-one-dark.min.css
--rw-rw-rw-   0        0        0      856 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/atom-one-light.min.css
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:49.256791 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/3024.min.css
--rw-rw-rw-   0        0        0     1403 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/apathy.min.css
--rw-rw-rw-   0        0        0     1368 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/apprentice.min.css
--rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ashes.min.css
--rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-cave-light.min.css
--rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-cave.min.css
--rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-dune-light.min.css
--rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-dune.min.css
--rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-estuary-light.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-estuary.min.css
--rw-rw-rw-   0        0        0     1416 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-forest-light.min.css
--rw-rw-rw-   0        0        0     1410 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-forest.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-heath-light.min.css
--rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-heath.min.css
--rw-rw-rw-   0        0        0     1418 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside-light.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside.min.css
--rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-plateau-light.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-plateau.min.css
--rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-savanna-light.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-savanna.min.css
--rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-seaside-light.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-seaside.min.css
--rw-rw-rw-   0        0        0     1421 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool-light.min.css
--rw-rw-rw-   0        0        0     1415 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool.min.css
--rw-rw-rw-   0        0        0     1391 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atlas.min.css
--rw-rw-rw-   0        0        0     1368 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/bespin.min.css
--rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-bathory.min.css
--rw-rw-rw-   0        0        0     1375 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-burzum.min.css
--rw-rw-rw-   0        0        0     1390 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-dark-funeral.min.css
--rw-rw-rw-   0        0        0     1387 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-gorgoroth.min.css
--rw-rw-rw-   0        0        0     1377 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-immortal.min.css
--rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-khold.min.css
--rw-rw-rw-   0        0        0     1384 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-marduk.min.css
--rw-rw-rw-   0        0        0     1384 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-mayhem.min.css
--rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-nile.min.css
--rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-venom.min.css
--rw-rw-rw-   0        0        0     1372 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal.min.css
--rw-rw-rw-   0        0        0     1404 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brewer.min.css
--rw-rw-rw-   0        0        0     1396 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/bright.min.css
--rw-rw-rw-   0        0        0     1407 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brogrammer.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brush-trees-dark.min.css
--rw-rw-rw-   0        0        0     1407 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brush-trees.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/chalk.min.css
--rw-rw-rw-   0        0        0     1451 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/circus.min.css
--rw-rw-rw-   0        0        0     1400 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/classic-dark.min.css
--rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/classic-light.min.css
--rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/codeschool.min.css
--rw-rw-rw-   0        0        0     1361 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/colors.min.css
--rw-rw-rw-   0        0        0     1400 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/cupcake.min.css
--rw-rw-rw-   0        0        0     1347 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/cupertino.min.css
--rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/danqing.min.css
--rw-rw-rw-   0        0        0     1367 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/darcula.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/dark-violet.min.css
--rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/darkmoss.min.css
--rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/darktooth.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/decaf.min.css
--rw-rw-rw-   0        0        0     1405 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/default-dark.min.css
--rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/default-light.min.css
--rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/dirtysea.min.css
--rw-rw-rw-   0        0        0     1456 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/dracula.min.css
--rw-rw-rw-   0        0        0     1387 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/edge-dark.min.css
--rw-rw-rw-   0        0        0     1388 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/edge-light.min.css
--rw-rw-rw-   0        0        0     1380 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/eighties.min.css
--rw-rw-rw-   0        0        0     1403 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/embers.min.css
--rw-rw-rw-   0        0        0     1382 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-dark.min.css
--rw-rw-rw-   0        0        0     1381 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-dark.min.css
--rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-light.min.css
--rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-light.min.css
--rw-rw-rw-   0        0        0     1424 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/espresso.min.css
--rw-rw-rw-   0        0        0     1396 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/eva-dim.min.css
--rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/eva.min.css
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/flat.min.css
--rw-rw-rw-   0        0        0     1394 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/framer.min.css
--rw-rw-rw-   0        0        0     1369 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/fruit-soda.min.css
--rw-rw-rw-   0        0        0     1404 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gigavolt.min.css
--rw-rw-rw-   0        0        0     1339 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/github.min.css
--rw-rw-rw-   0        0        0     1387 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/google-dark.min.css
--rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/google-light.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/grayscale-dark.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/grayscale-light.min.css
--rw-rw-rw-   0        0        0     1354 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/green-screen.min.css
--rw-rw-rw-   0        0        0     1449 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-hard.min.css
--rw-rw-rw-   0        0        0     1451 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-medium.min.css
--rw-rw-rw-   0        0        0     1449 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-pale.min.css
--rw-rw-rw-   0        0        0     1449 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-soft.min.css
--rw-rw-rw-   0        0        0     1450 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-hard.min.css
--rw-rw-rw-   0        0        0     1452 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-medium.min.css
--rw-rw-rw-   0        0        0     1450 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-soft.min.css
--rw-rw-rw-   0        0        0     1374 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/hardcore.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/harmonic16-dark.min.css
--rw-rw-rw-   0        0        0     1413 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/harmonic16-light.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/heetch-dark.min.css
--rw-rw-rw-   0        0        0     1399 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/heetch-light.min.css
--rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/helios.min.css
--rw-rw-rw-   0        0        0     1374 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/hopscotch.min.css
--rw-rw-rw-   0        0        0     1413 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/horizon-dark.min.css
--rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/horizon-light.min.css
--rw-rw-rw-   0        0        0     1388 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/humanoid-dark.min.css
--rw-rw-rw-   0        0        0     1389 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/humanoid-light.min.css
--rw-rw-rw-   0        0        0     1386 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ia-dark.min.css
--rw-rw-rw-   0        0        0     1396 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ia-light.min.css
--rw-rw-rw-   0        0        0     1390 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/icy-dark.min.css
--rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ir-black.min.css
--rw-rw-rw-   0        0        0     1334 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/isotope.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/kimber.min.css
--rw-rw-rw-   0        0        0     1376 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/london-tube.min.css
--rw-rw-rw-   0        0        0     1389 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/macintosh.min.css
--rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/marrakesh.min.css
--rw-rw-rw-   0        0        0     1363 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/materia.min.css
--rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-darker.min.css
--rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-lighter.min.css
--rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-palenight.min.css
--rw-rw-rw-   0        0        0     1378 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-vivid.min.css
--rw-rw-rw-   0        0        0     1366 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material.min.css
--rw-rw-rw-   0        0        0     1363 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/mellow-purple.min.css
--rw-rw-rw-   0        0        0     1381 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/mexico-light.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/mocha.min.css
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/monokai.min.css
--rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/nebula.min.css
--rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/nord.min.css
--rw-rw-rw-   0        0        0     1430 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/nova.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ocean.min.css
--rw-rw-rw-   0        0        0     1418 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/oceanicnext.min.css
--rw-rw-rw-   0        0        0     1410 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/one-light.min.css
--rw-rw-rw-   0        0        0     1403 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/onedark.min.css
--rw-rw-rw-   0        0        0     1416 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/outrun-dark.min.css
--rw-rw-rw-   0        0        0     1476 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/papercolor-dark.min.css
--rw-rw-rw-   0        0        0     1460 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/papercolor-light.min.css
--rw-rw-rw-   0        0        0     1372 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/paraiso.min.css
--rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/pasque.min.css
--rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/phd.min.css
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/pico.min.css
--rw-rw-rw-   0        0        0     1390 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/pop.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/porple.min.css
--rw-rw-rw-   0        0        0     1363 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/qualia.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/railscasts.min.css
--rw-rw-rw-   0        0        0     1455 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/rebecca.min.css
--rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ros-pine-dawn.min.css
--rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ros-pine-moon.min.css
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ros-pine.min.css
--rw-rw-rw-   0        0        0     1380 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/sagelight.min.css
--rw-rw-rw-   0        0        0     1376 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/sandcastle.min.css
--rw-rw-rw-   0        0        0     1361 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/seti-ui.min.css
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/shapeshifter.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/silk-dark.min.css
--rw-rw-rw-   0        0        0     1410 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/silk-light.min.css
--rw-rw-rw-   0        0        0     1476 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/snazzy.min.css
--rw-rw-rw-   0        0        0     1413 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solar-flare-light.min.css
--rw-rw-rw-   0        0        0     1407 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solar-flare.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solarized-dark.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solarized-light.min.css
--rw-rw-rw-   0        0        0     1425 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/spacemacs.min.css
--rw-rw-rw-   0        0        0     1392 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/summercamp.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/summerfruit-dark.min.css
--rw-rw-rw-   0        0        0     1404 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/summerfruit-light.min.css
--rw-rw-rw-   0        0        0     1429 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-dark.min.css
--rw-rw-rw-   0        0        0     1430 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-light.min.css
--rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tango.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tender.min.css
--rw-rw-rw-   0        0        0     1374 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tomorrow-night.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tomorrow.min.css
--rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/twilight.min.css
--rw-rw-rw-   0        0        0     1393 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/unikitty-dark.min.css
--rw-rw-rw-   0        0        0     1391 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/unikitty-light.min.css
--rw-rw-rw-   0        0        0     1350 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/vulcan.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-10-light.min.css
--rw-rw-rw-   0        0        0     1399 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-10.min.css
--rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-95-light.min.css
--rw-rw-rw-   0        0        0     1405 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-95.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast-light.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast.min.css
--rw-rw-rw-   0        0        0     1380 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-nt-light.min.css
--rw-rw-rw-   0        0        0     1367 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-nt.min.css
--rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/woodland.min.css
--rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/xcode-dusk.min.css
--rw-rw-rw-   0        0        0     1361 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/zenburn.min.css
--rw-rw-rw-   0        0        0      656 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/brown-paper.min.css
--rw-rw-rw-   0        0        0    18198 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/brown-papersq.png
--rw-rw-rw-   0        0        0      600 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/codepen-embed.min.css
--rw-rw-rw-   0        0        0      631 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/color-brewer.min.css
--rw-rw-rw-   0        0        0      625 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/dark.min.css
--rw-rw-rw-   0        0        0     1144 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/default.min.css
--rw-rw-rw-   0        0        0     1080 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/devibeans.min.css
--rw-rw-rw-   0        0        0      837 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/docco.min.css
--rw-rw-rw-   0        0        0      669 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/far.min.css
--rw-rw-rw-   0        0        0     1169 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/felipec.min.css
--rw-rw-rw-   0        0        0      779 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/foundation.min.css
--rw-rw-rw-   0        0        0     1251 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/github-dark-dimmed.min.css
--rw-rw-rw-   0        0        0     1315 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/github-dark.min.css
--rw-rw-rw-   0        0        0     1309 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/github.min.css
--rw-rw-rw-   0        0        0      787 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/gml.min.css
--rw-rw-rw-   0        0        0      835 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/googlecode.min.css
--rw-rw-rw-   0        0        0     1089 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/gradient-dark.min.css
--rw-rw-rw-   0        0        0     1112 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/gradient-light.min.css
--rw-rw-rw-   0        0        0     1674 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/grayscale.min.css
--rw-rw-rw-   0        0        0      897 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/hybrid.min.css
--rw-rw-rw-   0        0        0      906 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/idea.min.css
--rw-rw-rw-   0        0        0     1051 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/intellij-light.min.css
--rw-rw-rw-   0        0        0      694 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/ir-black.min.css
--rw-rw-rw-   0        0        0      971 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/isbl-editor-dark.min.css
--rw-rw-rw-   0        0        0      952 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/isbl-editor-light.min.css
--rw-rw-rw-   0        0        0      652 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/kimbie-dark.min.css
--rw-rw-rw-   0        0        0      652 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/kimbie-light.min.css
--rw-rw-rw-   0        0        0      831 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/lightfair.min.css
--rw-rw-rw-   0        0        0      715 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/lioshi.min.css
--rw-rw-rw-   0        0        0      642 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/magula.min.css
--rw-rw-rw-   0        0        0      631 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/mono-blue.min.css
--rw-rw-rw-   0        0        0      826 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/monokai-sublime.min.css
--rw-rw-rw-   0        0        0      790 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/monokai.min.css
--rw-rw-rw-   0        0        0     1421 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/night-owl.min.css
--rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/nnfx-dark.min.css
--rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/nnfx-light.min.css
--rw-rw-rw-   0        0        0     2684 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/nord.min.css
--rw-rw-rw-   0        0        0      882 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/obsidian.min.css
--rw-rw-rw-   0        0        0     1095 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/panda-syntax-dark.min.css
--rw-rw-rw-   0        0        0     1069 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/panda-syntax-light.min.css
--rw-rw-rw-   0        0        0      637 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/paraiso-dark.min.css
--rw-rw-rw-   0        0        0      637 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/paraiso-light.min.css
--rw-rw-rw-   0        0        0     1186 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/pojoaque.jpg
--rw-rw-rw-   0        0        0      814 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/pojoaque.min.css
--rw-rw-rw-   0        0        0      734 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/purebasic.min.css
--rw-rw-rw-   0        0        0      815 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/qtcreator-dark.min.css
--rw-rw-rw-   0        0        0      810 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/qtcreator-light.min.css
--rw-rw-rw-   0        0        0      826 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/rainbow.min.css
--rw-rw-rw-   0        0        0      862 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/routeros.min.css
--rw-rw-rw-   0        0        0      664 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/school-book.min.css
--rw-rw-rw-   0        0        0      854 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/shades-of-purple.min.css
--rw-rw-rw-   0        0        0      795 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/srcery.min.css
--rw-rw-rw-   0        0        0     1271 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/stackoverflow-dark.min.css
--rw-rw-rw-   0        0        0     1285 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/stackoverflow-light.min.css
--rw-rw-rw-   0        0        0      950 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/sunburst.min.css
--rw-rw-rw-   0        0        0     1234 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tokyo-night-dark.min.css
--rw-rw-rw-   0        0        0     1235 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tokyo-night-light.min.css
--rw-rw-rw-   0        0        0      648 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tomorrow-night-blue.min.css
--rw-rw-rw-   0        0        0      648 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tomorrow-night-bright.min.css
--rw-rw-rw-   0        0        0      640 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/vs.min.css
--rw-rw-rw-   0        0        0     1088 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/vs2015.min.css
--rw-rw-rw-   0        0        0      945 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/xcode.min.css
--rw-rw-rw-   0        0        0      765 2024-05-17 09:30:32.000000 easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/xt256.min.css
--rw-rw-rw-   0        0        0    87532 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/jquery-3.7.1.slim.min.js
--rw-rw-rw-   0        0        0   100167 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/leader-line.min.js
--rw-rw-rw-   0        0        0    29906 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/mmedu.js
--rw-rw-rw-   0        0        0   184698 2024-05-17 09:30:31.000000 easy-xedu-0.1.9/EasyTrain/static/js/socket.io.js
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:49.265789 easy-xedu-0.1.9/EasyTrain/templates/
--rw-rw-rw-   0        0        0    30149 2024-05-21 07:41:46.000000 easy-xedu-0.1.9/EasyTrain/templates/basennPage.html
--rw-rw-rw-   0        0        0    35705 2024-05-21 07:42:34.000000 easy-xedu-0.1.9/EasyTrain/templates/mmeduPage.html
--rw-rw-rw-   0        0        0     1080 2023-12-25 15:57:21.000000 easy-xedu-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0      330 2024-05-21 07:53:49.303792 easy-xedu-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-12-25 15:57:21.000000 easy-xedu-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 07:53:49.298790 easy-xedu-0.1.9/easy_xedu.egg-info/
--rw-rw-rw-   0        0        0      330 2024-05-21 07:53:47.000000 easy-xedu-0.1.9/easy_xedu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17502 2024-05-21 07:53:47.000000 easy-xedu-0.1.9/easy_xedu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 07:53:47.000000 easy-xedu-0.1.9/easy_xedu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-05-21 07:53:47.000000 easy-xedu-0.1.9/easy_xedu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-12-25 15:57:21.000000 easy-xedu-0.1.9/easy_xedu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2024-05-21 07:53:47.000000 easy-xedu-0.1.9/easy_xedu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-21 07:53:47.000000 easy-xedu-0.1.9/easy_xedu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 07:53:49.307788 easy-xedu-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      574 2024-05-21 07:50:52.000000 easy-xedu-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:14.819298 easy-xedu-0.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.326983 easy-xedu-0.2.1/EasyConvert/
+-rw-rw-rw-   0        0        0        0 2023-12-25 15:57:21.000000 easy-xedu-0.2.1/EasyConvert/__init__.py
+-rw-rw-rw-   0        0        0     6351 2023-12-25 15:57:21.000000 easy-xedu-0.2.1/EasyConvert/easyconvert.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.341984 easy-xedu-0.2.1/EasyTrain/
+-rw-rw-rw-   0        0        0        0 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.344982 easy-xedu-0.2.1/EasyTrain/apis/
+-rw-rw-rw-   0        0        0        0 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.353982 easy-xedu-0.2.1/EasyTrain/apis/baseml/
+-rw-rw-rw-   0        0        0      115 2024-05-17 11:59:45.000000 easy-xedu-0.2.1/EasyTrain/apis/baseml/__init__.py
+-rw-rw-rw-   0        0        0     3790 2024-05-21 06:13:01.000000 easy-xedu-0.2.1/EasyTrain/apis/baseml/baseml.py
+-rw-rw-rw-   0        0        0     6412 2024-05-21 06:13:57.000000 easy-xedu-0.2.1/EasyTrain/apis/baseml/config.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.362983 easy-xedu-0.2.1/EasyTrain/apis/basenn/
+-rw-rw-rw-   0        0        0      115 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/apis/basenn/__init__.py
+-rw-rw-rw-   0        0        0     5362 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/apis/basenn/basenn.py
+-rw-rw-rw-   0        0        0     8924 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/apis/basenn/config.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.370983 easy-xedu-0.2.1/EasyTrain/apis/mmedu/
+-rw-rw-rw-   0        0        0      111 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/apis/mmedu/__init__.py
+-rw-rw-rw-   0        0        0    10751 2024-05-21 03:41:38.000000 easy-xedu-0.2.1/EasyTrain/apis/mmedu/config.py
+-rw-rw-rw-   0        0        0     8135 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/apis/mmedu/mmedu.py
+-rw-rw-rw-   0        0        0      662 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/basenn_code.py
+-rw-rw-rw-   0        0        0      636 2024-05-17 10:07:08.000000 easy-xedu-0.2.1/EasyTrain/extensions.py
+-rw-rw-rw-   0        0        0      502 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/mmedu_code.py
+-rw-rw-rw-   0        0        0    15938 2024-05-21 06:09:34.000000 easy-xedu-0.2.1/EasyTrain/run.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.308026 easy-xedu-0.2.1/EasyTrain/static/
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.380987 easy-xedu-0.2.1/EasyTrain/static/assets/
+-rw-rw-rw-   0        0        0      643 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/assets/clipboard-plus.svg
+-rw-rw-rw-   0        0        0      935 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/assets/question-diamond.svg
+-rw-rw-rw-   0        0        0      497 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/assets/x-square.svg
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.397988 easy-xedu-0.2.1/EasyTrain/static/css/
+-rw-rw-rw-   0        0        0      113 2024-05-21 06:23:13.000000 easy-xedu-0.2.1/EasyTrain/static/css/baseml.css
+-rw-rw-rw-   0        0        0     2357 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/css/basenn.css
+-rw-rw-rw-   0        0        0   162264 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1309 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/css/github.min.css
+-rw-rw-rw-   0        0        0     8039 2024-05-21 06:58:15.000000 easy-xedu-0.2.1/EasyTrain/static/css/style.css
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.429023 easy-xedu-0.2.1/EasyTrain/static/js/
+-rw-rw-rw-   0        0        0    17598 2024-05-21 06:12:02.000000 easy-xedu-0.2.1/EasyTrain/static/js/baseml.js
+-rw-rw-rw-   0        0        0    42085 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/basenn.js
+-rw-rw-rw-   0        0        0    83376 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0     9160 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/clipboard.min.js
+-rw-rw-rw-   0        0        0   491315 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/echarts.min.js
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.450862 easy-xedu-0.2.1/EasyTrain/static/js/highlight/
+-rw-rw-rw-   0        0        0    38854 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/DIGESTS.md
+-rw-rw-rw-   0        0        0     1514 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/LICENSE
+-rw-rw-rw-   0        0        0     1717 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.468873 easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/
+-rw-rw-rw-   0        0        0    76121 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/core.js
+-rw-rw-rw-   0        0        0    20322 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/core.min.js
+-rw-rw-rw-   0        0        0    76121 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/highlight.js
+-rw-rw-rw-   0        0        0    20322 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/highlight.min.js
+-rw-rw-rw-   0        0        0       20 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/package.json
+-rw-rw-rw-   0        0        0    80817 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/highlight.js
+-rw-rw-rw-   0        0        0    23953 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/highlight.min.js
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.472874 easy-xedu-0.2.1/EasyTrain/static/js/highlight/languages/
+-rw-rw-rw-   0        0        0     3529 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/languages/python.min.js
+-rw-rw-rw-   0        0        0     2903 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/package.json
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:13.730977 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/
+-rw-rw-rw-   0        0        0     1158 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/a11y-dark.min.css
+-rw-rw-rw-   0        0        0     1146 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/a11y-light.min.css
+-rw-rw-rw-   0        0        0     1357 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/agate.min.css
+-rw-rw-rw-   0        0        0      961 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/an-old-hope.min.css
+-rw-rw-rw-   0        0        0      611 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/androidstudio.min.css
+-rw-rw-rw-   0        0        0      844 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/arduino-light.min.css
+-rw-rw-rw-   0        0        0      673 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/arta.min.css
+-rw-rw-rw-   0        0        0      454 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/ascetic.min.css
+-rw-rw-rw-   0        0        0     1193 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/atom-one-dark-reasonable.min.css
+-rw-rw-rw-   0        0        0      856 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/atom-one-dark.min.css
+-rw-rw-rw-   0        0        0      856 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/atom-one-light.min.css
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:14.756298 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/3024.min.css
+-rw-rw-rw-   0        0        0     1403 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/apathy.min.css
+-rw-rw-rw-   0        0        0     1368 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/apprentice.min.css
+-rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ashes.min.css
+-rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-cave-light.min.css
+-rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-cave.min.css
+-rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-dune-light.min.css
+-rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-dune.min.css
+-rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-estuary-light.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-estuary.min.css
+-rw-rw-rw-   0        0        0     1416 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-forest-light.min.css
+-rw-rw-rw-   0        0        0     1410 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-forest.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-heath-light.min.css
+-rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-heath.min.css
+-rw-rw-rw-   0        0        0     1418 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside-light.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside.min.css
+-rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-plateau-light.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-plateau.min.css
+-rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-savanna-light.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-savanna.min.css
+-rw-rw-rw-   0        0        0     1417 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-seaside-light.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-seaside.min.css
+-rw-rw-rw-   0        0        0     1421 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool-light.min.css
+-rw-rw-rw-   0        0        0     1415 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool.min.css
+-rw-rw-rw-   0        0        0     1391 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atlas.min.css
+-rw-rw-rw-   0        0        0     1368 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/bespin.min.css
+-rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-bathory.min.css
+-rw-rw-rw-   0        0        0     1375 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-burzum.min.css
+-rw-rw-rw-   0        0        0     1390 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-dark-funeral.min.css
+-rw-rw-rw-   0        0        0     1387 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-gorgoroth.min.css
+-rw-rw-rw-   0        0        0     1377 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-immortal.min.css
+-rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-khold.min.css
+-rw-rw-rw-   0        0        0     1384 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-marduk.min.css
+-rw-rw-rw-   0        0        0     1384 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-mayhem.min.css
+-rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-nile.min.css
+-rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-venom.min.css
+-rw-rw-rw-   0        0        0     1372 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal.min.css
+-rw-rw-rw-   0        0        0     1404 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brewer.min.css
+-rw-rw-rw-   0        0        0     1396 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/bright.min.css
+-rw-rw-rw-   0        0        0     1407 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brogrammer.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brush-trees-dark.min.css
+-rw-rw-rw-   0        0        0     1407 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brush-trees.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/chalk.min.css
+-rw-rw-rw-   0        0        0     1451 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/circus.min.css
+-rw-rw-rw-   0        0        0     1400 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/classic-dark.min.css
+-rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/classic-light.min.css
+-rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/codeschool.min.css
+-rw-rw-rw-   0        0        0     1361 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/colors.min.css
+-rw-rw-rw-   0        0        0     1400 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/cupcake.min.css
+-rw-rw-rw-   0        0        0     1347 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/cupertino.min.css
+-rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/danqing.min.css
+-rw-rw-rw-   0        0        0     1367 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/darcula.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/dark-violet.min.css
+-rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/darkmoss.min.css
+-rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/darktooth.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/decaf.min.css
+-rw-rw-rw-   0        0        0     1405 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/default-dark.min.css
+-rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/default-light.min.css
+-rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/dirtysea.min.css
+-rw-rw-rw-   0        0        0     1456 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/dracula.min.css
+-rw-rw-rw-   0        0        0     1387 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/edge-dark.min.css
+-rw-rw-rw-   0        0        0     1388 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/edge-light.min.css
+-rw-rw-rw-   0        0        0     1380 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/eighties.min.css
+-rw-rw-rw-   0        0        0     1403 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/embers.min.css
+-rw-rw-rw-   0        0        0     1382 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-dark.min.css
+-rw-rw-rw-   0        0        0     1381 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-dark.min.css
+-rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-light.min.css
+-rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-light.min.css
+-rw-rw-rw-   0        0        0     1424 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/espresso.min.css
+-rw-rw-rw-   0        0        0     1396 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/eva-dim.min.css
+-rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/eva.min.css
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/flat.min.css
+-rw-rw-rw-   0        0        0     1394 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/framer.min.css
+-rw-rw-rw-   0        0        0     1369 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/fruit-soda.min.css
+-rw-rw-rw-   0        0        0     1404 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gigavolt.min.css
+-rw-rw-rw-   0        0        0     1339 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/github.min.css
+-rw-rw-rw-   0        0        0     1387 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/google-dark.min.css
+-rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/google-light.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/grayscale-dark.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/grayscale-light.min.css
+-rw-rw-rw-   0        0        0     1354 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/green-screen.min.css
+-rw-rw-rw-   0        0        0     1449 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-hard.min.css
+-rw-rw-rw-   0        0        0     1451 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-medium.min.css
+-rw-rw-rw-   0        0        0     1449 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-pale.min.css
+-rw-rw-rw-   0        0        0     1449 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-soft.min.css
+-rw-rw-rw-   0        0        0     1450 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-hard.min.css
+-rw-rw-rw-   0        0        0     1452 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-medium.min.css
+-rw-rw-rw-   0        0        0     1450 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-soft.min.css
+-rw-rw-rw-   0        0        0     1374 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/hardcore.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/harmonic16-dark.min.css
+-rw-rw-rw-   0        0        0     1413 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/harmonic16-light.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/heetch-dark.min.css
+-rw-rw-rw-   0        0        0     1399 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/heetch-light.min.css
+-rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/helios.min.css
+-rw-rw-rw-   0        0        0     1374 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/hopscotch.min.css
+-rw-rw-rw-   0        0        0     1413 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/horizon-dark.min.css
+-rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/horizon-light.min.css
+-rw-rw-rw-   0        0        0     1388 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/humanoid-dark.min.css
+-rw-rw-rw-   0        0        0     1389 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/humanoid-light.min.css
+-rw-rw-rw-   0        0        0     1386 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ia-dark.min.css
+-rw-rw-rw-   0        0        0     1396 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ia-light.min.css
+-rw-rw-rw-   0        0        0     1390 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/icy-dark.min.css
+-rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ir-black.min.css
+-rw-rw-rw-   0        0        0     1334 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/isotope.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/kimber.min.css
+-rw-rw-rw-   0        0        0     1376 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/london-tube.min.css
+-rw-rw-rw-   0        0        0     1389 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/macintosh.min.css
+-rw-rw-rw-   0        0        0     1408 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/marrakesh.min.css
+-rw-rw-rw-   0        0        0     1363 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/materia.min.css
+-rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-darker.min.css
+-rw-rw-rw-   0        0        0     1383 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-lighter.min.css
+-rw-rw-rw-   0        0        0     1385 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-palenight.min.css
+-rw-rw-rw-   0        0        0     1378 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-vivid.min.css
+-rw-rw-rw-   0        0        0     1366 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material.min.css
+-rw-rw-rw-   0        0        0     1363 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/mellow-purple.min.css
+-rw-rw-rw-   0        0        0     1381 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/mexico-light.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/mocha.min.css
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/monokai.min.css
+-rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/nebula.min.css
+-rw-rw-rw-   0        0        0     1373 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/nord.min.css
+-rw-rw-rw-   0        0        0     1430 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/nova.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ocean.min.css
+-rw-rw-rw-   0        0        0     1418 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/oceanicnext.min.css
+-rw-rw-rw-   0        0        0     1410 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/one-light.min.css
+-rw-rw-rw-   0        0        0     1403 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/onedark.min.css
+-rw-rw-rw-   0        0        0     1416 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/outrun-dark.min.css
+-rw-rw-rw-   0        0        0     1476 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/papercolor-dark.min.css
+-rw-rw-rw-   0        0        0     1460 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/papercolor-light.min.css
+-rw-rw-rw-   0        0        0     1372 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/paraiso.min.css
+-rw-rw-rw-   0        0        0     1406 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/pasque.min.css
+-rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/phd.min.css
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/pico.min.css
+-rw-rw-rw-   0        0        0     1390 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/pop.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/porple.min.css
+-rw-rw-rw-   0        0        0     1363 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/qualia.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/railscasts.min.css
+-rw-rw-rw-   0        0        0     1455 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/rebecca.min.css
+-rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ros-pine-dawn.min.css
+-rw-rw-rw-   0        0        0     1402 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ros-pine-moon.min.css
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ros-pine.min.css
+-rw-rw-rw-   0        0        0     1380 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/sagelight.min.css
+-rw-rw-rw-   0        0        0     1376 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/sandcastle.min.css
+-rw-rw-rw-   0        0        0     1361 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/seti-ui.min.css
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/shapeshifter.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/silk-dark.min.css
+-rw-rw-rw-   0        0        0     1410 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/silk-light.min.css
+-rw-rw-rw-   0        0        0     1476 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/snazzy.min.css
+-rw-rw-rw-   0        0        0     1413 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solar-flare-light.min.css
+-rw-rw-rw-   0        0        0     1407 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solar-flare.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solarized-dark.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solarized-light.min.css
+-rw-rw-rw-   0        0        0     1425 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/spacemacs.min.css
+-rw-rw-rw-   0        0        0     1392 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/summercamp.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/summerfruit-dark.min.css
+-rw-rw-rw-   0        0        0     1404 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/summerfruit-light.min.css
+-rw-rw-rw-   0        0        0     1429 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-dark.min.css
+-rw-rw-rw-   0        0        0     1430 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-light.min.css
+-rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tango.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tender.min.css
+-rw-rw-rw-   0        0        0     1374 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tomorrow-night.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tomorrow.min.css
+-rw-rw-rw-   0        0        0     1401 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/twilight.min.css
+-rw-rw-rw-   0        0        0     1393 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/unikitty-dark.min.css
+-rw-rw-rw-   0        0        0     1391 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/unikitty-light.min.css
+-rw-rw-rw-   0        0        0     1350 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/vulcan.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-10-light.min.css
+-rw-rw-rw-   0        0        0     1399 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-10.min.css
+-rw-rw-rw-   0        0        0     1414 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-95-light.min.css
+-rw-rw-rw-   0        0        0     1405 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-95.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast-light.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast.min.css
+-rw-rw-rw-   0        0        0     1380 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-nt-light.min.css
+-rw-rw-rw-   0        0        0     1367 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-nt.min.css
+-rw-rw-rw-   0        0        0     1398 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/woodland.min.css
+-rw-rw-rw-   0        0        0     1409 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/xcode-dusk.min.css
+-rw-rw-rw-   0        0        0     1361 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/zenburn.min.css
+-rw-rw-rw-   0        0        0      656 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/brown-paper.min.css
+-rw-rw-rw-   0        0        0    18198 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/brown-papersq.png
+-rw-rw-rw-   0        0        0      600 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/codepen-embed.min.css
+-rw-rw-rw-   0        0        0      631 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/color-brewer.min.css
+-rw-rw-rw-   0        0        0      625 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/dark.min.css
+-rw-rw-rw-   0        0        0     1144 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/default.min.css
+-rw-rw-rw-   0        0        0     1080 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/devibeans.min.css
+-rw-rw-rw-   0        0        0      837 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/docco.min.css
+-rw-rw-rw-   0        0        0      669 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/far.min.css
+-rw-rw-rw-   0        0        0     1169 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/felipec.min.css
+-rw-rw-rw-   0        0        0      779 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/foundation.min.css
+-rw-rw-rw-   0        0        0     1251 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/github-dark-dimmed.min.css
+-rw-rw-rw-   0        0        0     1315 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/github-dark.min.css
+-rw-rw-rw-   0        0        0     1309 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/github.min.css
+-rw-rw-rw-   0        0        0      787 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/gml.min.css
+-rw-rw-rw-   0        0        0      835 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/googlecode.min.css
+-rw-rw-rw-   0        0        0     1089 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/gradient-dark.min.css
+-rw-rw-rw-   0        0        0     1112 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/gradient-light.min.css
+-rw-rw-rw-   0        0        0     1674 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/grayscale.min.css
+-rw-rw-rw-   0        0        0      897 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/hybrid.min.css
+-rw-rw-rw-   0        0        0      906 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/idea.min.css
+-rw-rw-rw-   0        0        0     1051 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/intellij-light.min.css
+-rw-rw-rw-   0        0        0      694 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/ir-black.min.css
+-rw-rw-rw-   0        0        0      971 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/isbl-editor-dark.min.css
+-rw-rw-rw-   0        0        0      952 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/isbl-editor-light.min.css
+-rw-rw-rw-   0        0        0      652 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/kimbie-dark.min.css
+-rw-rw-rw-   0        0        0      652 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/kimbie-light.min.css
+-rw-rw-rw-   0        0        0      831 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/lightfair.min.css
+-rw-rw-rw-   0        0        0      715 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/lioshi.min.css
+-rw-rw-rw-   0        0        0      642 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/magula.min.css
+-rw-rw-rw-   0        0        0      631 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/mono-blue.min.css
+-rw-rw-rw-   0        0        0      826 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/monokai-sublime.min.css
+-rw-rw-rw-   0        0        0      790 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/monokai.min.css
+-rw-rw-rw-   0        0        0     1421 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/night-owl.min.css
+-rw-rw-rw-   0        0        0     1411 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/nnfx-dark.min.css
+-rw-rw-rw-   0        0        0     1412 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/nnfx-light.min.css
+-rw-rw-rw-   0        0        0     2684 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/nord.min.css
+-rw-rw-rw-   0        0        0      882 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/obsidian.min.css
+-rw-rw-rw-   0        0        0     1095 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/panda-syntax-dark.min.css
+-rw-rw-rw-   0        0        0     1069 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/panda-syntax-light.min.css
+-rw-rw-rw-   0        0        0      637 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/paraiso-dark.min.css
+-rw-rw-rw-   0        0        0      637 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/paraiso-light.min.css
+-rw-rw-rw-   0        0        0     1186 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/pojoaque.jpg
+-rw-rw-rw-   0        0        0      814 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/pojoaque.min.css
+-rw-rw-rw-   0        0        0      734 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/purebasic.min.css
+-rw-rw-rw-   0        0        0      815 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/qtcreator-dark.min.css
+-rw-rw-rw-   0        0        0      810 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/qtcreator-light.min.css
+-rw-rw-rw-   0        0        0      826 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/rainbow.min.css
+-rw-rw-rw-   0        0        0      862 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/routeros.min.css
+-rw-rw-rw-   0        0        0      664 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/school-book.min.css
+-rw-rw-rw-   0        0        0      854 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/shades-of-purple.min.css
+-rw-rw-rw-   0        0        0      795 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/srcery.min.css
+-rw-rw-rw-   0        0        0     1271 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/stackoverflow-dark.min.css
+-rw-rw-rw-   0        0        0     1285 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/stackoverflow-light.min.css
+-rw-rw-rw-   0        0        0      950 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/sunburst.min.css
+-rw-rw-rw-   0        0        0     1234 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tokyo-night-dark.min.css
+-rw-rw-rw-   0        0        0     1235 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tokyo-night-light.min.css
+-rw-rw-rw-   0        0        0      648 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tomorrow-night-blue.min.css
+-rw-rw-rw-   0        0        0      648 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tomorrow-night-bright.min.css
+-rw-rw-rw-   0        0        0      640 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/vs.min.css
+-rw-rw-rw-   0        0        0     1088 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/vs2015.min.css
+-rw-rw-rw-   0        0        0      945 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/xcode.min.css
+-rw-rw-rw-   0        0        0      765 2024-05-17 09:30:32.000000 easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/xt256.min.css
+-rw-rw-rw-   0        0        0    87532 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/jquery-3.7.1.slim.min.js
+-rw-rw-rw-   0        0        0   100167 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/leader-line.min.js
+-rw-rw-rw-   0        0        0    29906 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/mmedu.js
+-rw-rw-rw-   0        0        0   184698 2024-05-17 09:30:31.000000 easy-xedu-0.2.1/EasyTrain/static/js/socket.io.js
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:14.772298 easy-xedu-0.2.1/EasyTrain/templates/
+-rw-rw-rw-   0        0        0    36471 2024-05-21 07:29:37.000000 easy-xedu-0.2.1/EasyTrain/templates/basemlPage.html
+-rw-rw-rw-   0        0        0    30149 2024-05-21 07:41:46.000000 easy-xedu-0.2.1/EasyTrain/templates/basennPage.html
+-rw-rw-rw-   0        0        0    35705 2024-05-21 07:42:34.000000 easy-xedu-0.2.1/EasyTrain/templates/mmeduPage.html
+-rw-rw-rw-   0        0        0      303 2024-05-21 08:31:14.815297 easy-xedu-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-12-25 15:57:21.000000 easy-xedu-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 08:31:14.811298 easy-xedu-0.2.1/easy_xedu.egg-info/
+-rw-rw-rw-   0        0        0      303 2024-05-21 08:31:12.000000 easy-xedu-0.2.1/easy_xedu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17578 2024-05-21 08:31:13.000000 easy-xedu-0.2.1/easy_xedu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:31:12.000000 easy-xedu-0.2.1/easy_xedu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-05-21 08:31:13.000000 easy-xedu-0.2.1/easy_xedu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2023-12-25 15:57:21.000000 easy-xedu-0.2.1/easy_xedu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2024-05-21 08:31:13.000000 easy-xedu-0.2.1/easy_xedu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-21 08:31:13.000000 easy-xedu-0.2.1/easy_xedu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 08:31:14.820300 easy-xedu-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      574 2024-05-21 08:20:59.000000 easy-xedu-0.2.1/setup.py
```

### Comparing `easy-xedu-0.1.9/EasyConvert/easyconvert.py` & `easy-xedu-0.2.1/EasyConvert/easyconvert.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/apis/baseml/baseml.py` & `easy-xedu-0.2.1/EasyTrain/apis/baseml/baseml.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/apis/baseml/config.py` & `easy-xedu-0.2.1/EasyTrain/apis/baseml/config.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/apis/basenn/basenn.py` & `easy-xedu-0.2.1/EasyTrain/apis/basenn/basenn.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/apis/basenn/config.py` & `easy-xedu-0.2.1/EasyTrain/apis/basenn/config.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/apis/mmedu/config.py` & `easy-xedu-0.2.1/EasyTrain/apis/mmedu/config.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/apis/mmedu/mmedu.py` & `easy-xedu-0.2.1/EasyTrain/apis/mmedu/mmedu.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/basenn_code.py` & `easy-xedu-0.2.1/EasyTrain/basenn_code.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/extensions.py` & `easy-xedu-0.2.1/EasyTrain/extensions.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/run.py` & `easy-xedu-0.2.1/EasyTrain/run.py`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/assets/clipboard-plus.svg` & `easy-xedu-0.2.1/EasyTrain/static/assets/clipboard-plus.svg`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/assets/question-diamond.svg` & `easy-xedu-0.2.1/EasyTrain/static/assets/question-diamond.svg`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/css/basenn.css` & `easy-xedu-0.2.1/EasyTrain/static/css/basenn.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/css/bootstrap.min.css` & `easy-xedu-0.2.1/EasyTrain/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/css/github.min.css` & `easy-xedu-0.2.1/EasyTrain/static/css/github.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/css/style.css` & `easy-xedu-0.2.1/EasyTrain/static/css/style.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/basenn.js` & `easy-xedu-0.2.1/EasyTrain/static/js/basenn.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/bootstrap.bundle.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/clipboard.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/echarts.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/DIGESTS.md` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/DIGESTS.md`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/LICENSE` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/README.md` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/README.md`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/core.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/core.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/core.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/core.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/highlight.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/highlight.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/es/highlight.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/es/highlight.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/highlight.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/highlight.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/highlight.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/highlight.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/languages/python.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/languages/python.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/package.json` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/package.json`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/a11y-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/a11y-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/a11y-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/a11y-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/agate.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/agate.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/an-old-hope.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/an-old-hope.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/androidstudio.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/androidstudio.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/arduino-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/arduino-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/arta.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/arta.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/atom-one-dark-reasonable.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/atom-one-dark-reasonable.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/atom-one-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/atom-one-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/atom-one-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/atom-one-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/3024.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/3024.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/apathy.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/apathy.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/apprentice.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/apprentice.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ashes.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ashes.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-cave-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-cave-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-cave.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-cave.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-dune-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-dune-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-dune.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-dune.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-estuary-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-estuary-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-estuary.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-estuary.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-forest-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-forest-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-forest.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-forest.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-heath-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-heath-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-heath.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-heath.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-lakeside.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-plateau-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-plateau-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-plateau.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-plateau.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-savanna-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-savanna-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-savanna.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-savanna.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-seaside-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-seaside-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-seaside.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-seaside.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atelier-sulphurpool.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/atlas.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/atlas.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/bespin.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/bespin.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-bathory.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-bathory.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-burzum.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-burzum.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-dark-funeral.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-dark-funeral.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-gorgoroth.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-gorgoroth.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-immortal.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-immortal.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-khold.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-khold.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-marduk.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-marduk.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-mayhem.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-mayhem.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-nile.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-nile.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal-venom.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal-venom.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/black-metal.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/black-metal.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brewer.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brewer.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/bright.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/bright.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brogrammer.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brogrammer.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brush-trees-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brush-trees-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/brush-trees.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/brush-trees.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/chalk.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/chalk.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/circus.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/circus.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/classic-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/classic-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/classic-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/classic-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/codeschool.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/codeschool.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/colors.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/colors.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/cupcake.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/cupcake.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/cupertino.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/cupertino.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/danqing.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/danqing.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/darcula.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/darcula.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/dark-violet.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/dark-violet.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/darkmoss.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/darkmoss.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/darktooth.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/darktooth.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/decaf.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/decaf.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/default-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/default-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/default-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/default-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/dirtysea.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/dirtysea.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/dracula.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/dracula.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/edge-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/edge-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/edge-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/edge-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/eighties.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/eighties.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/embers.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/embers.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-gray-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/equilibrium-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/equilibrium-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/espresso.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/espresso.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/eva-dim.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/eva-dim.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/eva.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/eva.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/flat.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/flat.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/framer.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/framer.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/fruit-soda.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/fruit-soda.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gigavolt.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gigavolt.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/github.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/github.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/google-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/google-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/google-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/google-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/grayscale-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/grayscale-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/grayscale-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/grayscale-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/green-screen.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/green-screen.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-hard.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-hard.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-medium.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-medium.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-pale.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-pale.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-soft.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-dark-soft.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-hard.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-hard.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-medium.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-medium.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-soft.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/gruvbox-light-soft.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/hardcore.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/hardcore.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/harmonic16-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/harmonic16-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/harmonic16-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/harmonic16-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/heetch-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/heetch-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/heetch-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/heetch-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/helios.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/helios.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/hopscotch.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/hopscotch.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/horizon-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/horizon-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/horizon-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/horizon-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/humanoid-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/humanoid-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/humanoid-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/humanoid-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ia-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ia-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ia-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ia-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/icy-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/icy-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ir-black.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ir-black.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/isotope.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/isotope.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/kimber.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/kimber.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/london-tube.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/london-tube.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/macintosh.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/macintosh.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/marrakesh.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/marrakesh.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/materia.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/materia.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-darker.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-darker.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-lighter.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-lighter.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-palenight.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-palenight.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material-vivid.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material-vivid.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/material.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/material.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/mellow-purple.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/mellow-purple.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/mexico-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/mexico-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/mocha.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/mocha.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/monokai.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/monokai.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/nebula.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/nebula.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/nord.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/nord.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/nova.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/nova.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ocean.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ocean.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/oceanicnext.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/oceanicnext.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/one-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/one-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/onedark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/onedark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/outrun-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/outrun-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/papercolor-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/papercolor-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/papercolor-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/papercolor-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/paraiso.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/paraiso.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/pasque.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/pasque.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/phd.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/phd.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/pico.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/pico.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/pop.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/pop.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/porple.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/porple.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/qualia.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/qualia.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/railscasts.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/railscasts.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/rebecca.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/rebecca.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ros-pine-dawn.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ros-pine-dawn.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ros-pine-moon.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ros-pine-moon.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/ros-pine.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/ros-pine.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/sagelight.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/sagelight.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/sandcastle.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/sandcastle.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/seti-ui.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/seti-ui.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/shapeshifter.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/shapeshifter.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/silk-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/silk-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/silk-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/silk-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/snazzy.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/snazzy.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solar-flare-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solar-flare-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solar-flare.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solar-flare.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solarized-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solarized-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/solarized-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/solarized-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/spacemacs.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/spacemacs.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/summercamp.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/summercamp.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/summerfruit-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/summerfruit-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/summerfruit-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/summerfruit-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/synth-midnight-terminal-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tango.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tango.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tender.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tender.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tomorrow-night.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tomorrow-night.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/tomorrow.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/tomorrow.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/twilight.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/twilight.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/unikitty-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/unikitty-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/unikitty-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/unikitty-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/vulcan.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/vulcan.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-10-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-10-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-10.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-10.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-95-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-95-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-95.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-95.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-high-contrast.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-nt-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-nt-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/windows-nt.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/windows-nt.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/woodland.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/woodland.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/xcode-dusk.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/xcode-dusk.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/base16/zenburn.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/base16/zenburn.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/brown-paper.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/brown-paper.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/brown-papersq.png` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/brown-papersq.png`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/codepen-embed.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/codepen-embed.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/color-brewer.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/color-brewer.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/default.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/default.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/devibeans.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/devibeans.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/docco.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/docco.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/far.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/far.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/felipec.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/felipec.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/foundation.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/foundation.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/github-dark-dimmed.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/github-dark-dimmed.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/github-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/github-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/github.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/github.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/gml.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/gml.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/googlecode.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/googlecode.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/gradient-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/gradient-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/gradient-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/gradient-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/grayscale.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/grayscale.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/hybrid.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/hybrid.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/idea.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/idea.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/intellij-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/intellij-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/ir-black.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/ir-black.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/isbl-editor-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/isbl-editor-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/isbl-editor-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/isbl-editor-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/kimbie-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/kimbie-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/kimbie-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/kimbie-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/lightfair.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/lightfair.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/lioshi.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/lioshi.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/magula.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/magula.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/mono-blue.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/mono-blue.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/monokai-sublime.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/monokai-sublime.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/monokai.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/monokai.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/night-owl.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/night-owl.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/nnfx-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/nnfx-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/nnfx-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/nnfx-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/nord.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/nord.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/obsidian.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/obsidian.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/panda-syntax-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/panda-syntax-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/panda-syntax-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/panda-syntax-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/paraiso-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/paraiso-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/paraiso-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/paraiso-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/pojoaque.jpg` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/pojoaque.jpg`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/pojoaque.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/pojoaque.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/purebasic.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/purebasic.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/qtcreator-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/qtcreator-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/qtcreator-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/qtcreator-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/rainbow.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/rainbow.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/routeros.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/routeros.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/school-book.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/school-book.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/shades-of-purple.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/shades-of-purple.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/srcery.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/srcery.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/stackoverflow-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/stackoverflow-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/stackoverflow-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/stackoverflow-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/sunburst.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/sunburst.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tokyo-night-dark.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tokyo-night-dark.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tokyo-night-light.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tokyo-night-light.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tomorrow-night-blue.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tomorrow-night-blue.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/tomorrow-night-bright.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/tomorrow-night-bright.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/vs.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/vs.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/vs2015.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/vs2015.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/xcode.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/xcode.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/highlight/styles/xt256.min.css` & `easy-xedu-0.2.1/EasyTrain/static/js/highlight/styles/xt256.min.css`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/jquery-3.7.1.slim.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/jquery-3.7.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/leader-line.min.js` & `easy-xedu-0.2.1/EasyTrain/static/js/leader-line.min.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/mmedu.js` & `easy-xedu-0.2.1/EasyTrain/static/js/mmedu.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/static/js/socket.io.js` & `easy-xedu-0.2.1/EasyTrain/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/templates/basennPage.html` & `easy-xedu-0.2.1/EasyTrain/templates/basennPage.html`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/EasyTrain/templates/mmeduPage.html` & `easy-xedu-0.2.1/EasyTrain/templates/mmeduPage.html`

 * *Files identical despite different names*

### Comparing `easy-xedu-0.1.9/easy_xedu.egg-info/SOURCES.txt` & `easy-xedu-0.2.1/easy_xedu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-LICENSE.txt
 README.md
-setup.cfg
 setup.py
 EasyConvert/__init__.py
 EasyConvert/easyconvert.py
 EasyTrain/__init__.py
 EasyTrain/basenn_code.py
 EasyTrain/extensions.py
 EasyTrain/mmedu_code.py
@@ -18,18 +16,20 @@
 EasyTrain/apis/basenn/config.py
 EasyTrain/apis/mmedu/__init__.py
 EasyTrain/apis/mmedu/config.py
 EasyTrain/apis/mmedu/mmedu.py
 EasyTrain/static/assets/clipboard-plus.svg
 EasyTrain/static/assets/question-diamond.svg
 EasyTrain/static/assets/x-square.svg
+EasyTrain/static/css/baseml.css
 EasyTrain/static/css/basenn.css
 EasyTrain/static/css/bootstrap.min.css
 EasyTrain/static/css/github.min.css
 EasyTrain/static/css/style.css
+EasyTrain/static/js/baseml.js
 EasyTrain/static/js/basenn.js
 EasyTrain/static/js/bootstrap.bundle.min.js
 EasyTrain/static/js/clipboard.min.js
 EasyTrain/static/js/echarts.min.js
 EasyTrain/static/js/jquery-3.7.1.slim.min.js
 EasyTrain/static/js/leader-line.min.js
 EasyTrain/static/js/mmedu.js
@@ -292,14 +292,15 @@
 EasyTrain/static/js/highlight/styles/base16/windows-high-contrast-light.min.css
 EasyTrain/static/js/highlight/styles/base16/windows-high-contrast.min.css
 EasyTrain/static/js/highlight/styles/base16/windows-nt-light.min.css
 EasyTrain/static/js/highlight/styles/base16/windows-nt.min.css
 EasyTrain/static/js/highlight/styles/base16/woodland.min.css
 EasyTrain/static/js/highlight/styles/base16/xcode-dusk.min.css
 EasyTrain/static/js/highlight/styles/base16/zenburn.min.css
+EasyTrain/templates/basemlPage.html
 EasyTrain/templates/basennPage.html
 EasyTrain/templates/mmeduPage.html
 easy_xedu.egg-info/PKG-INFO
 easy_xedu.egg-info/SOURCES.txt
 easy_xedu.egg-info/dependency_links.txt
 easy_xedu.egg-info/entry_points.txt
 easy_xedu.egg-info/not-zip-safe
```

### Comparing `easy-xedu-0.1.9/setup.py` & `easy-xedu-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="easy-xedu",
-    version="0.1.9",
+    version="0.2.1",
     packages = find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "flask",
         "flask-cors",
         "flask-socketio",
```

