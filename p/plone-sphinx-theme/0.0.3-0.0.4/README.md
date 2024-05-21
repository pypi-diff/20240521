# Comparing `tmp/plone_sphinx_theme-0.0.3.tar.gz` & `tmp/plone_sphinx_theme-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_sphinx_theme-0.0.3.tar", last modified: Sun May 19 22:31:31 2024, max compression
+gzip compressed data, was "plone_sphinx_theme-0.0.4.tar", last modified: Tue May 21 06:48:23 2024, max compression
```

## Comparing `plone_sphinx_theme-0.0.3.tar` & `plone_sphinx_theme-0.0.4.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.330340 plone_sphinx_theme-0.0.3/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1336 2024-05-19 22:31:31.152678 plone_sphinx_theme-0.0.3/CHANGES.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)    18091 2024-05-19 22:31:31.152958 plone_sphinx_theme-0.0.3/LICENSE
--rw-r--r--   0 stevepiercy   (501) staff       (20)       33 2024-05-19 22:31:31.153073 plone_sphinx_theme-0.0.3/MANIFEST.in
--rw-r--r--   0 stevepiercy   (501) staff       (20)     7914 2024-05-19 22:31:31.153321 plone_sphinx_theme-0.0.3/Makefile
--rw-r--r--   0 stevepiercy   (501) staff       (20)      888 2024-05-19 22:31:31.153412 plone_sphinx_theme-0.0.3/README.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157188 plone_sphinx_theme-0.0.3/docs/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.153771 plone_sphinx_theme-0.0.3/docs/_static/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     5430 2024-05-19 22:31:31.153740 plone_sphinx_theme-0.0.3/docs/_static/favicon.ico
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3775 2024-05-19 22:31:31.153953 plone_sphinx_theme-0.0.3/docs/_static/logo.svg
--rw-r--r--   0 stevepiercy   (501) staff       (20)    16098 2024-05-19 22:31:31.154119 plone_sphinx_theme-0.0.3/docs/conf.py
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2620 2024-05-19 22:31:31.154234 plone_sphinx_theme-0.0.3/docs/glossary.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.154778 plone_sphinx_theme-0.0.3/docs/guides/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3887 2024-05-19 22:31:31.154478 plone_sphinx_theme-0.0.3/docs/guides/contribute.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2177 2024-05-19 22:31:31.154629 plone_sphinx_theme-0.0.3/docs/guides/contributing-policies.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1173 2024-05-19 22:31:31.154747 plone_sphinx_theme-0.0.3/docs/guides/develop.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1885 2024-05-19 22:31:31.154847 plone_sphinx_theme-0.0.3/docs/guides/usage.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1588 2024-05-19 22:31:31.154949 plone_sphinx_theme-0.0.3/docs/index.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157047 plone_sphinx_theme-0.0.3/docs/reference/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     5113 2024-05-19 22:31:31.155104 plone_sphinx_theme-0.0.3/docs/reference/extensions.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3212 2024-05-19 22:31:31.155233 plone_sphinx_theme-0.0.3/docs/reference/file-system-structure.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.156905 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3208 2024-05-19 22:31:31.155420 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/admonitions.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)      980 2024-05-19 22:31:31.155549 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/api.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     8114 2024-05-19 22:31:31.155692 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/blocks.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     8597 2024-05-19 22:31:31.156005 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/generic.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3070 2024-05-19 22:31:31.156219 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/images.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)      576 2024-05-19 22:31:31.156346 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/index.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6150 2024-05-19 22:31:31.156484 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/lists.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)    13453 2024-05-19 22:31:31.156613 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/really-long.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6375 2024-05-19 22:31:31.156742 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/structure.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6705 2024-05-19 22:31:31.156870 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/tables.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2669 2024-05-19 22:31:31.157006 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/typography.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2507 2024-05-19 22:31:31.157158 plone_sphinx_theme-0.0.3/docs/reference/special-theme-elements.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)      260 2024-05-19 22:31:31.157257 plone_sphinx_theme-0.0.3/docs/robots.txt
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157320 plone_sphinx_theme-0.0.3/news/
--rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157318 plone_sphinx_theme-0.0.3/news/.gitkeep
--rw-r--r--   0 stevepiercy   (501) staff       (20)      622 2024-05-19 22:31:31.157706 plone_sphinx_theme-0.0.3/package.json
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3498 2024-05-19 22:31:31.157812 plone_sphinx_theme-0.0.3/pyproject.toml
--rw-r--r--   0 stevepiercy   (501) staff       (20)      302 2024-05-19 22:31:31.157918 plone_sphinx_theme-0.0.3/requirements-docs.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)      133 2024-05-19 22:31:31.158039 plone_sphinx_theme-0.0.3/requirements-initial.txt
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.158362 plone_sphinx_theme-0.0.3/scripts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1195 2024-05-19 22:31:31.158330 plone_sphinx_theme-0.0.3/scripts/kitchen_sink_update.py
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1655 2024-05-19 22:31:31.158448 plone_sphinx_theme-0.0.3/scripts/sbt_styles_update.py
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.158515 plone_sphinx_theme-0.0.3/src/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.163955 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2894 2024-05-19 22:31:31.158631 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/__init__.py
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.159004 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.158750 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/scripts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6353 2024-05-19 22:31:31.158973 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/scripts/index.js
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160436 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.159321 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-19 22:31:31.159284 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-19 22:31:31.159472 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.159767 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-19 22:31:31.159732 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_base.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-19 22:31:31.159955 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_print.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160032 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/components/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      124 2024-05-19 22:31:31.160124 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/components/_title.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160206 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/content/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      197 2024-05-19 22:31:31.160294 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/content/_margin.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      287 2024-05-19 22:31:31.160405 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/index.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.162799 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160650 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-19 22:31:31.160603 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-19 22:31:31.160722 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160981 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-19 22:31:31.160859 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-19 22:31:31.160951 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      517 2024-05-19 22:31:31.161156 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.161636 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      325 2024-05-19 22:31:31.161352 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_back-to-top.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      455 2024-05-19 22:31:31.161476 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_icon-links.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      461 2024-05-19 22:31:31.161605 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_logo.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1059 2024-05-19 22:31:31.161732 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.162249 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      128 2024-05-19 22:31:31.161876 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_code.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      824 2024-05-19 22:31:31.161990 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     4767 2024-05-19 22:31:31.162113 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      250 2024-05-19 22:31:31.162218 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_notebooks.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      364 2024-05-19 22:31:31.162332 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_quotes.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.162554 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      308 2024-05-19 22:31:31.162519 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_comments.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      431 2024-05-19 22:31:31.162648 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_thebe.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1262 2024-05-19 22:31:31.162767 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.163830 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/
--rw-r--r--   0 stevepiercy   (501) staff       (20)       94 2024-05-19 22:31:31.162937 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_announcement.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      746 2024-05-19 22:31:31.163066 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      113 2024-05-19 22:31:31.163170 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      150 2024-05-19 22:31:31.163287 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-article.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      436 2024-05-19 22:31:31.163412 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-content.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     4365 2024-05-19 22:31:31.163557 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      233 2024-05-19 22:31:31.163682 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-primary.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1266 2024-05-19 22:31:31.163799 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2585 2024-05-19 22:31:31.163926 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.163996 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164637 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1305 2024-05-19 22:31:31.164246 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164526 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      142 2024-05-19 22:31:31.164489 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/chapter-title.html
--rw-r--r--   0 stevepiercy   (501) staff       (20)       13 2024-05-19 22:31:31.164606 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/version.html
--rw-r--r--   0 stevepiercy   (501) staff       (20)      349 2024-05-19 22:31:31.164795 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/theme.conf
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164870 plone_sphinx_theme-0.0.3/styles/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165105 plone_sphinx_theme-0.0.3/styles/Vocab/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165034 plone_sphinx_theme-0.0.3/styles/Vocab/Base/
--rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164947 plone_sphinx_theme-0.0.3/styles/Vocab/Base/accept.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165032 plone_sphinx_theme-0.0.3/styles/Vocab/Base/reject.txt
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165271 plone_sphinx_theme-0.0.3/styles/Vocab/Plone/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      564 2024-05-19 22:31:31.165238 plone_sphinx_theme-0.0.3/styles/Vocab/Plone/accept.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)       14 2024-05-19 22:31:31.165427 plone_sphinx_theme-0.0.3/styles/Vocab/Plone/reject.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1628 2024-05-19 22:31:31.165545 plone_sphinx_theme-0.0.3/webpack.config.js
--rw-r--r--   0        0        0    23980 1970-01-01 00:00:00.000000 plone_sphinx_theme-0.0.3/PKG-INFO
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.776104 plone_sphinx_theme-0.0.4/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1617 2024-05-21 06:48:23.603870 plone_sphinx_theme-0.0.4/CHANGES.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)    18091 2024-05-21 06:48:23.604160 plone_sphinx_theme-0.0.4/LICENSE
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       33 2024-05-21 06:48:23.604382 plone_sphinx_theme-0.0.4/MANIFEST.in
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     7914 2024-05-21 06:48:23.604635 plone_sphinx_theme-0.0.4/Makefile
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      888 2024-05-21 06:48:23.604826 plone_sphinx_theme-0.0.4/README.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.608841 plone_sphinx_theme-0.0.4/docs/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.605156 plone_sphinx_theme-0.0.4/docs/_static/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     5430 2024-05-21 06:48:23.605127 plone_sphinx_theme-0.0.4/docs/_static/favicon.ico
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3775 2024-05-21 06:48:23.605328 plone_sphinx_theme-0.0.4/docs/_static/logo.svg
+-rw-r--r--   0 stevepiercy   (501) staff       (20)    16098 2024-05-21 06:48:23.605591 plone_sphinx_theme-0.0.4/docs/conf.py
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2620 2024-05-21 06:48:23.605814 plone_sphinx_theme-0.0.4/docs/glossary.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.606346 plone_sphinx_theme-0.0.4/docs/guides/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3887 2024-05-21 06:48:23.606038 plone_sphinx_theme-0.0.4/docs/guides/contribute.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2177 2024-05-21 06:48:23.606204 plone_sphinx_theme-0.0.4/docs/guides/contributing-policies.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1173 2024-05-21 06:48:23.606315 plone_sphinx_theme-0.0.4/docs/guides/develop.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1885 2024-05-21 06:48:23.606532 plone_sphinx_theme-0.0.4/docs/guides/usage.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1588 2024-05-21 06:48:23.606716 plone_sphinx_theme-0.0.4/docs/index.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.608695 plone_sphinx_theme-0.0.4/docs/reference/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     5113 2024-05-21 06:48:23.606872 plone_sphinx_theme-0.0.4/docs/reference/extensions.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3212 2024-05-21 06:48:23.606990 plone_sphinx_theme-0.0.4/docs/reference/file-system-structure.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.608563 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3208 2024-05-21 06:48:23.607141 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/admonitions.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      980 2024-05-21 06:48:23.607255 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/api.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     8114 2024-05-21 06:48:23.607392 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/blocks.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     8597 2024-05-21 06:48:23.607653 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/generic.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3070 2024-05-21 06:48:23.607822 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/images.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      576 2024-05-21 06:48:23.607954 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/index.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6150 2024-05-21 06:48:23.608106 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/lists.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)    13453 2024-05-21 06:48:23.608249 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/really-long.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6375 2024-05-21 06:48:23.608390 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/structure.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6705 2024-05-21 06:48:23.608527 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/tables.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2669 2024-05-21 06:48:23.608662 plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/typography.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2507 2024-05-21 06:48:23.608806 plone_sphinx_theme-0.0.4/docs/reference/special-theme-elements.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      260 2024-05-21 06:48:23.609040 plone_sphinx_theme-0.0.4/docs/robots.txt
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.609112 plone_sphinx_theme-0.0.4/news/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.609109 plone_sphinx_theme-0.0.4/news/.gitkeep
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      622 2024-05-21 06:48:23.609745 plone_sphinx_theme-0.0.4/package.json
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3620 2024-05-21 06:48:23.609950 plone_sphinx_theme-0.0.4/pyproject.toml
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      302 2024-05-21 06:48:23.610219 plone_sphinx_theme-0.0.4/requirements-docs.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      133 2024-05-21 06:48:23.610458 plone_sphinx_theme-0.0.4/requirements-initial.txt
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.610910 plone_sphinx_theme-0.0.4/scripts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1195 2024-05-21 06:48:23.610737 plone_sphinx_theme-0.0.4/scripts/kitchen_sink_update.py
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1655 2024-05-21 06:48:23.610879 plone_sphinx_theme-0.0.4/scripts/sbt_styles_update.py
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.610951 plone_sphinx_theme-0.0.4/scripts/templates/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      271 2024-05-21 06:48:23.611032 plone_sphinx_theme-0.0.4/scripts/templates/towncrier_template.jinja
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.611108 plone_sphinx_theme-0.0.4/src/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.616389 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2894 2024-05-21 06:48:23.611241 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/__init__.py
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.611603 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.611356 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/scripts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6353 2024-05-21 06:48:23.611575 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/scripts/index.js
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.612917 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.611911 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-21 06:48:23.611875 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-21 06:48:23.612041 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.612296 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-21 06:48:23.612264 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/base/_base.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-21 06:48:23.612470 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/base/_print.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.612542 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      124 2024-05-21 06:48:23.612626 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/components/_title.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.612695 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      197 2024-05-21 06:48:23.612779 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/content/_margin.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      287 2024-05-21 06:48:23.612887 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/index.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.615237 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.613094 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-21 06:48:23.613057 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-21 06:48:23.613171 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.613443 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-21 06:48:23.613319 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-21 06:48:23.613416 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      517 2024-05-21 06:48:23.613626 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.614126 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      325 2024-05-21 06:48:23.613875 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_back-to-top.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      455 2024-05-21 06:48:23.613986 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_icon-links.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      461 2024-05-21 06:48:23.614099 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_logo.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1059 2024-05-21 06:48:23.614208 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.614751 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      128 2024-05-21 06:48:23.614352 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_code.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      824 2024-05-21 06:48:23.614487 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     4767 2024-05-21 06:48:23.614609 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      250 2024-05-21 06:48:23.614724 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_notebooks.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      364 2024-05-21 06:48:23.614831 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_quotes.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.615009 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      308 2024-05-21 06:48:23.614977 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_comments.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      431 2024-05-21 06:48:23.615085 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_thebe.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1262 2024-05-21 06:48:23.615202 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.616258 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       94 2024-05-21 06:48:23.615358 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_announcement.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      746 2024-05-21 06:48:23.615480 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      113 2024-05-21 06:48:23.615589 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      150 2024-05-21 06:48:23.615706 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-article.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      436 2024-05-21 06:48:23.615831 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-content.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     4365 2024-05-21 06:48:23.615964 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      233 2024-05-21 06:48:23.616091 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-primary.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1266 2024-05-21 06:48:23.616225 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2585 2024-05-21 06:48:23.616359 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.616437 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617118 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1305 2024-05-21 06:48:23.616691 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.616999 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      142 2024-05-21 06:48:23.616964 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/chapter-title.html
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       13 2024-05-21 06:48:23.617088 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/version.html
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      349 2024-05-21 06:48:23.617267 plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/theme.conf
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617329 plone_sphinx_theme-0.0.4/styles/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617535 plone_sphinx_theme-0.0.4/styles/Vocab/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617471 plone_sphinx_theme-0.0.4/styles/Vocab/Base/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617397 plone_sphinx_theme-0.0.4/styles/Vocab/Base/accept.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617468 plone_sphinx_theme-0.0.4/styles/Vocab/Base/reject.txt
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-21 06:48:23.617685 plone_sphinx_theme-0.0.4/styles/Vocab/Plone/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      564 2024-05-21 06:48:23.617656 plone_sphinx_theme-0.0.4/styles/Vocab/Plone/accept.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       14 2024-05-21 06:48:23.617836 plone_sphinx_theme-0.0.4/styles/Vocab/Plone/reject.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1628 2024-05-21 06:48:23.617981 plone_sphinx_theme-0.0.4/webpack.config.js
+-rw-r--r--   0        0        0    23980 1970-01-01 00:00:00.000000 plone_sphinx_theme-0.0.4/PKG-INFO
```

### Comparing `plone_sphinx_theme-0.0.3/CHANGES.md` & `plone_sphinx_theme-0.0.4/CHANGES.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,22 @@
      Instead create a file in the news directory.
      For helpful instructions, see:
      https://6.docs.plone.org/contributing/index.html#change-log-entry
 -->
 
 <!-- towncrier release notes start -->
 
-0.0.3 (2024-05-19)
-------------------
+## 0.0.4 (2024-05-20)
+
+### Internal changes
+
+- Steal towncrier config from Volto. Clean up `CHANGES.md`. @stevepiercy [Issue #18](https://github.com/plone/plone-sphinx-theme/issues/18)
+- Fix towncrier template path. @stevepiercy [Issue #19](https://github.com/plone/plone-sphinx-theme/issues/19)
+
+## 0.0.3 (2024-05-19)
 
 ### Internal changes:
 
 - Add .gitkeep to news directory to preserve it upon releases. @stevepiercy ([Issue #garden](https://github.com/plone/plone-sphinx-theme/garden))
 - Fix CHANGES.md content for automatic updates upon releases. @stevepiercy ([Issue #garden1](https://github.com/plone/plone-sphinx-theme/garden1))
 - Add GitHub action to deploy documentation to Read the Docs. @stevepiercy ([Issue #garden2](https://github.com/plone/plone-sphinx-theme/garden2))
 - Add pull request preview on Read the Docs. @stevepiercy ([Issue #garden3](https://github.com/plone/plone-sphinx-theme/garden3))
```

### Comparing `plone_sphinx_theme-0.0.3/LICENSE` & `plone_sphinx_theme-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/Makefile` & `plone_sphinx_theme-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/README.md` & `plone_sphinx_theme-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/_static/favicon.ico` & `plone_sphinx_theme-0.0.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/_static/logo.svg` & `plone_sphinx_theme-0.0.4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/conf.py` & `plone_sphinx_theme-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/glossary.md` & `plone_sphinx_theme-0.0.4/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/guides/contribute.md` & `plone_sphinx_theme-0.0.4/docs/guides/contribute.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/guides/contributing-policies.md` & `plone_sphinx_theme-0.0.4/docs/guides/contributing-policies.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/guides/develop.md` & `plone_sphinx_theme-0.0.4/docs/guides/develop.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/guides/usage.md` & `plone_sphinx_theme-0.0.4/docs/guides/usage.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/index.md` & `plone_sphinx_theme-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/extensions.md` & `plone_sphinx_theme-0.0.4/docs/reference/extensions.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/file-system-structure.md` & `plone_sphinx_theme-0.0.4/docs/reference/file-system-structure.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/admonitions.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/api.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/blocks.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/generic.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/images.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/index.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/index.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/lists.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/really-long.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/really-long.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/structure.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/tables.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/typography.rst` & `plone_sphinx_theme-0.0.4/docs/reference/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/docs/reference/special-theme-elements.md` & `plone_sphinx_theme-0.0.4/docs/reference/special-theme-elements.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/package.json` & `plone_sphinx_theme-0.0.4/package.json`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/pyproject.toml` & `plone_sphinx_theme-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -111,39 +111,41 @@
 #filterwarnings = [
 #]
 
 [tool.zest-releaser]
 python-file-with-version = "src/plone_sphinx_theme/__init__.py"
 
 [tool.towncrier]
-issue_format = "[Issue #{issue}](https://github.com/plone/plone-sphinx-theme/{issue})"
-filename = "CHANGES.md"
 directory = "news/"
-title_format = "{version} ({project_date})"
+filename = "CHANGES.md"
+issue_format = "[Issue #{issue}](https://github.com/plone/plone-sphinx-theme/issues/{issue})"
+start_string = "<!-- towncrier release notes start -->\n"
+template = "scripts/templates/towncrier_template.jinja"
+title_format = "## {version} ({project_date})"
 # First underline is used for version/date header.
 # Second underline is used for the type names (like 'Bug fixes:').
-underlines = ["-", ""]
+underlines = ["", "", ""]
 
 [[tool.towncrier.type]]
 directory = "internal"
-name = "Internal changes:"
+name = "Internal changes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "breaking"
-name = "Breaking changes:"
+name = "Breaking changes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "feature"
-name = "New features:"
+name = "New features"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "bugfix"
-name = "Bug fixes:"
+name = "Bug fixes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "documentation"
-name = "Documentation:"
+name = "Documentation"
 showcontent = true
```

### Comparing `plone_sphinx_theme-0.0.3/scripts/kitchen_sink_update.py` & `plone_sphinx_theme-0.0.4/scripts/kitchen_sink_update.py`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/scripts/sbt_styles_update.py` & `plone_sphinx_theme-0.0.4/scripts/sbt_styles_update.py`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/__init__.py` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 from pathlib import Path
 
 from sphinx.application import Sphinx
 from sphinx.util import logging
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 from sphinx_book_theme import update_context_with_repository_info, update_sourcename
 
 logger = logging.getLogger(__name__)
 
 
 def get_html_theme_path():
```

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/scripts/index.js` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_base.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/base/_base.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_print.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/base/_print.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html` & `plone_sphinx_theme-0.0.4/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/styles/Vocab/Plone/accept.txt` & `plone_sphinx_theme-0.0.4/styles/Vocab/Plone/accept.txt`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/webpack.config.js` & `plone_sphinx_theme-0.0.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.3/PKG-INFO` & `plone_sphinx_theme-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone-sphinx-theme
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plone Sphinx Theme is the official Sphinx theme for Plone 6 Documentation, Plone Conference Training, and documentation of various Plone packages.
 Keywords: Plone,Sphinx,Theme,documentation,training,Diátaxis
 Author-Email: Steve Piercy <spiercy@plone.org>
 Maintainer-Email: Steve Piercy <spiercy@plone.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```

