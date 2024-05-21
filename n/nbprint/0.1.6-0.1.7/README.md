# Comparing `tmp/nbprint-0.1.6.tar.gz` & `tmp/nbprint-0.1.7.tar.gz`

## Comparing `nbprint-0.1.6.tar` & `nbprint-0.1.7.tar`

### file list

```diff
@@ -1,94 +1,105 @@
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/.eslintrc.js
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/build.mjs
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/package.json
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/playwright.config.js
--rw-r--r--   0        0        0    55380 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/yarn.lock
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/css/embedded.css
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/css/table-of-content.css
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/embedded.js
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/index.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/nbconvert.js
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/nbprint.js
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/components/table-of-content.js
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/less/index.less
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/tests/index.spec.js
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/__main__.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/cli.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/__init__.py
--rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/base.py
--rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/page.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/border.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/common.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/css.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/display.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/spacing.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/style.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/text.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/__init__.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/base.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/common.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/cover.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/image.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/page.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/pagebreak.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/table_of_contents.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/__init__.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/config.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/context.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/exceptions.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/outputs.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/parameters.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/__init__.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/code.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/context.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/cover.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/markdown.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/page.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/parameters.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/__init__.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/content.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/context.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/parameters.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/research/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/research/content.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/research/context.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/embedded.css
--rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/embedded.js
--rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/embedded.js.map
--rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/fontawesome.min.css
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/index.css
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/index.js
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/index.js.map
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/table-of-content.css
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/conf.json
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/index.html.j2
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.css
--rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js
--rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js.map
--rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/fontawesome.min.css
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/index.js
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/index.js.map
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/nbprint.css
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/table-of-content.css
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/tests/test_all.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/tests/test_e2e.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/tests/config/common/test_styles.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/format.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/image.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/ipython.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/base.html.j2
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/browser-open.html
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/error.html
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/index.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/mathjax.html.j2
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/mermaidjs.html.j2
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/page.html
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nbprint-0.1.6/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nbprint-0.1.6/LICENSE
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 nbprint-0.1.6/README.md
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 nbprint-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 nbprint-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/.eslintrc.js
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/build.mjs
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/package.json
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/playwright.config.js
+-rw-r--r--   0        0        0    55380 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/yarn.lock
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/css/embedded.css
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/css/table-of-content.css
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/js/embedded.js
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/js/index.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/js/nbconvert.js
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/js/nbprint.js
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/js/components/table-of-content.js
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/src/less/index.less
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbprint-0.1.7/js/tests/index.spec.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/__main__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/cli.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/__init__.py
+-rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/base.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/page.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/border.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/common.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/css.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/display.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/spacing.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/style.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/common/text.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/__init__.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/base.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/common.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/cover.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/image.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/page.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/pagebreak.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/content/table_of_contents.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/core/__init__.py
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/core/config.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/core/context.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/core/exceptions.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/core/outputs.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/core/parameters.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/conf.yaml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/config/default.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/context/default.yaml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/hydra/hydra_logging/custom.yaml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/outputs/nbconvert.yaml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/page/default.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/config/hydra/parameters/default.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/code.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/context.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/cover.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/markdown.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/page.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/basic/parameters.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/finance/__init__.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/finance/content.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/finance/context.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/finance/parameters.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/research/__init__.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/research/content.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/example/research/context.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/embedded.css
+-rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/embedded.js
+-rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/embedded.js.map
+-rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/fontawesome.min.css
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/index.css
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/index.js
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/index.js.map
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/extension/table-of-content.css
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/models/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/models/pandas.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/models/seaborn.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/conf.json
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/index.html.j2
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/embedded.css
+-rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/embedded.js
+-rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/embedded.js.map
+-rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/fontawesome.min.css
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/index.js
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/index.js.map
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/nbprint.css
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/templates/nbprint/static/table-of-content.css
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/tests/test_all.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/tests/test_e2e.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/tests/config/common/test_styles.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/utils/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/utils/format.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/utils/image.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/utils/ipython.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/base.html.j2
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/browser-open.html
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/error.html
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/index.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/mathjax.html.j2
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/mermaidjs.html.j2
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 nbprint-0.1.7/nbprint/voila/page.html
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nbprint-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nbprint-0.1.7/LICENSE
+-rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 nbprint-0.1.7/README.md
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 nbprint-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    22609 2020-02-02 00:00:00.000000 nbprint-0.1.7/PKG-INFO
```

### Comparing `nbprint-0.1.6/js/.eslintrc.js` & `nbprint-0.1.7/js/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/build.mjs` & `nbprint-0.1.7/js/build.mjs`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/package.json` & `nbprint-0.1.7/js/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'repository'": "'git@github.com:nbprint/nbprint.git'", "'version'": "'0.1.7'"}*

```diff
@@ -21,21 +21,21 @@
         "index.d.ts"
     ],
     "license": "Apache-2.0",
     "name": "nbprint",
     "publishConfig": {
         "access": "public"
     },
-    "repository": "git@github.com:timkpaine/nbprint.git",
+    "repository": "git@github.com:nbprint/nbprint.git",
     "scripts": {
         "build": "node build.mjs",
         "clean": "rm -rf dist playwright-report ../nbprint/extension",
         "fix": "prettier --write  \"src/js/*.js\" \"src/less/*.less\" \"tests/*.spec.js\" \"*.js\" \"*.json\"",
         "lint": "prettier --check \"src/js/*.js\" \"src/less/*.less\" \"tests/*.spec.js\" \"*.js\" \"*.json\"",
         "prepack": "npm run build",
         "start:examples": "http-server -p 3000 -o examples/",
         "start:tests": "http-server -p 3000 ",
         "test": "TZ=UTC playwright test"
     },
     "types": "index.d.ts",
-    "version": "0.1.6"
+    "version": "0.1.7"
 }
```

### Comparing `nbprint-0.1.6/js/playwright.config.js` & `nbprint-0.1.7/js/playwright.config.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/yarn.lock` & `nbprint-0.1.7/js/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1110,17 +1110,17 @@
   version "7.2.0"
   resolved "https://registry.yarnpkg.com/supports-color/-/supports-color-7.2.0.tgz#1b7dcdcb32b8138801b3e478ba6a51caa89648da"
   integrity sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==
   dependencies:
     has-flag "^4.0.0"
 
 tar@^6.1.11:
-  version "6.2.0"
-  resolved "https://registry.yarnpkg.com/tar/-/tar-6.2.0.tgz#b14ce49a79cb1cd23bc9b016302dea5474493f73"
-  integrity sha512-/Wo7DcT0u5HUV486xg675HtjNd3BXZ6xDbzsCUZPt5iw8bTQ63bP0Raut3mvro9u+CUyq7YQd8Cx55fsZXxqLQ==
+  version "6.2.1"
+  resolved "https://registry.yarnpkg.com/tar/-/tar-6.2.1.tgz#717549c541bc3c2af15751bea94b1dd068d4b03a"
+  integrity sha512-DZ4yORTwrbTj/7MZYq2w+/ZFdI6OZ/f9SFHR+71gIVUZhOQPHzVCLpvRnPgyaMpfWxxk/4ONva3GQSyNIKRv6A==
   dependencies:
     chownr "^2.0.0"
     fs-minipass "^2.0.0"
     minipass "^5.0.0"
     minizlib "^2.1.1"
     mkdirp "^1.0.3"
     yallist "^4.0.0"
```

### Comparing `nbprint-0.1.6/js/src/css/embedded.css` & `nbprint-0.1.7/js/src/css/embedded.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/src/css/table-of-content.css` & `nbprint-0.1.7/js/src/css/table-of-content.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/src/js/embedded.js` & `nbprint-0.1.7/js/src/js/embedded.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/src/js/nbconvert.js` & `nbprint-0.1.7/js/src/js/nbconvert.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/src/js/nbprint.js` & `nbprint-0.1.7/js/src/js/nbprint.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/src/js/components/table-of-content.js` & `nbprint-0.1.7/js/src/js/components/table-of-content.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/js/src/less/index.less` & `nbprint-0.1.7/js/src/less/index.less`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/base.py` & `nbprint-0.1.7/nbprint/config/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 from importlib import import_module
 from IPython.display import DisplayObject
 from json import dumps, loads
 from nbformat import NotebookNode
 from nbformat.v4 import new_code_cell, new_markdown_cell
 from pathlib import Path
-from pydantic import BaseModel, Field, PrivateAttr, SerializeAsAny, validator
+from pydantic import BaseModel, Field, PrivateAttr, SerializeAsAny, field_validator
 from pydantic._internal._model_construction import ModelMetaclass
 from strenum import StrEnum
 from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple, Type, Union
 from uuid import uuid4
 
 if TYPE_CHECKING:
     from ..config import Configuration
@@ -94,32 +94,32 @@
         validate_assignment: bool = True
 
     def __init__(self, **kwargs):
         if "_target_" not in kwargs:
             kwargs["_target_"] = Type(module=self.__class__.__module__, name=self.__class__.__name__)
         super().__init__(**kwargs)
 
-    @validator("css", pre=True)
+    @field_validator("css", mode="before")
     def convert_css_string_or_path_to_string_or_path(cls, v):
         if isinstance(v, str):
             if v.strip().endswith(".css"):
                 # TODO resolve relative to class?
                 v = Path(v).resolve().read_text()
         return v
 
-    @validator("esm", pre=True)
+    @field_validator("esm", mode="before")
     def convert_esm_string_or_path_to_string_or_path(cls, v):
         if isinstance(v, str):
             v = v.strip()
             if v.endswith(".js") or v.endswith(".mjs"):
                 # TODO resolve relative to class?
                 v = Path(v).resolve().read_text()
         return v
 
-    @validator("type", pre=True)
+    @field_validator("type", mode="before")
     def convert_type_string_to_module_and_name(cls, v):
         if isinstance(v, str):
             return Type.from_string(v)
         return v
 
     @property
     def nb_var_name(self):
@@ -190,14 +190,29 @@
         return self._base_generate(metadata=metadata, config=config, parent=parent, attr=attr, counter=counter)
 
     def _base_set_nbprint_metadata(self, cell: NotebookNode):
         cell.metadata.nbprint.id = self._id
         cell.metadata.nbprint.role = self.role or "undefined"
         cell.metadata.nbprint.type = self.type.to_string()
         cell.metadata.nbprint.ignore = self.ignore or False
+        if cell.metadata.nbprint.ignore and self.role in (Role.PARAMETERS,):
+            # Don't collapse
+            ...
+        elif cell.metadata.nbprint.ignore or self.role in (
+            Role.CONFIGURATION,
+            Role.CONTEXT,
+            Role.PAGE,
+            Role.UNDEFINED,
+        ):
+            # Collapse cell by default
+            cell.metadata["jupyter"] = {
+                "source_hidden": True,
+                "outputs_hidden": True,
+            }
+            cell.metadata.collapsed = True
         cell.metadata.nbprint.css = self.css or ""
         cell.metadata.nbprint.esm = self.esm or ""
         cell.metadata.nbprint.class_selector = f'{cell.metadata.nbprint.type.replace(":", "-").replace(".", "-")}'
         cell.metadata.nbprint.element_selector = f"{cell.metadata.nbprint.class_selector}-{self._id}"
         cell.metadata.nbprint["class"] = (
             f"nbprint {cell.metadata.nbprint.class_selector} {cell.metadata.nbprint.element_selector} "
             + (" ".join(self.classname) if isinstance(self.classname, list) else self.classname or "")
```

### Comparing `nbprint-0.1.6/nbprint/config/page.py` & `nbprint-0.1.7/nbprint/config/page.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from nbformat import NotebookNode
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from .base import BaseModel, Role, Type, _append_or_extend
 from .common import Style
 
 if TYPE_CHECKING:
     from .core.config import Configuration
@@ -78,59 +78,59 @@
     def convert_region_from_obj(cls, v, region):
         ret = BaseModel._to_type(v, PageRegion)
         ret._region = region
         base_css_scope = "@page {{ @{region} {{ {content} }} }}".format(region=region, content=str(ret.content or ""))
         ret.css += base_css_scope
         return ret
 
-    @validator("top", pre=True)
+    @field_validator("top", mode="before")
     def convert_top_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "top-center")
 
-    @validator("top_left", pre=True)
+    @field_validator("top_left", mode="before")
     def convert_top_left_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "top-left")
 
-    @validator("top_right", pre=True)
+    @field_validator("top_right", mode="before")
     def convert_top_right_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "top-right")
 
-    @validator("bottom", pre=True)
+    @field_validator("bottom", mode="before")
     def convert_bottom_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "bottom-center")
 
-    @validator("bottom_left", pre=True)
+    @field_validator("bottom_left", mode="before")
     def convert_bottom_left_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "bottom-left")
 
-    @validator("bottom_right", pre=True)
+    @field_validator("bottom_right", mode="before")
     def convert_bottom_right_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "bottom-right")
 
-    @validator("left", pre=True)
+    @field_validator("left", mode="before")
     def convert_left_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "left-center")
 
-    @validator("left_top", pre=True)
+    @field_validator("left_top", mode="before")
     def convert_left_top_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "left-top")
 
-    @validator("left_bottom", pre=True)
+    @field_validator("left_bottom", mode="before")
     def convert_left_bottom_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "left-bottom")
 
-    @validator("right", pre=True)
+    @field_validator("right", mode="before")
     def convert_right_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "right-center")
 
-    @validator("right_top", pre=True)
+    @field_validator("right_top", mode="before")
     def convert_right_top_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "right-top")
 
-    @validator("right_bottom", pre=True)
+    @field_validator("right_bottom", mode="before")
     def convert_right_bottom_from_obj(cls, v):
         return Page.convert_region_from_obj(v, "right-bottom")
 
     def generate(
         self, metadata: dict, config: "Configuration", parent: "BaseModel", attr: str = "page", *args, **kwargs
     ) -> Optional[Union[NotebookNode, List[NotebookNode]]]:
         cells = []
@@ -169,15 +169,15 @@
                 cell.generate(metadata=metadata, config=config, parent=self, attr="pages", counter=i),
             )
         for cell in cells:
             if cell is None:
                 raise Exception("got null cell, investigate!")
         return cells
 
-    @validator("pages", pre=True)
+    @field_validator("pages", mode="before")
     def convert_pages_from_obj(cls, v):
         if v is None:
             return []
         if isinstance(v, list):
             for i, element in enumerate(v):
                 if isinstance(element, str):
                     v[i] = Page(type=Type.from_string(element))
```

### Comparing `nbprint-0.1.6/nbprint/config/common/border.py` & `nbprint-0.1.7/nbprint/config/common/border.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/common/common.py` & `nbprint-0.1.7/nbprint/config/common/common.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/common/display.py` & `nbprint-0.1.7/nbprint/config/common/display.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/common/spacing.py` & `nbprint-0.1.7/nbprint/config/common/spacing.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/common/style.py` & `nbprint-0.1.7/nbprint/config/common/style.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/common/text.py` & `nbprint-0.1.7/nbprint/config/common/text.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/content/base.py` & `nbprint-0.1.7/nbprint/config/content/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from IPython.display import HTML
 from nbformat import NotebookNode
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from ..base import BaseModel, Role, SerializeAsAny, Type, _append_or_extend
 from ..common import Style
 
 if TYPE_CHECKING:
     from ..core import Configuration
@@ -49,26 +50,29 @@
                     cell.generate(metadata=metadata, config=config, parent=self, attr=attr or "content", counter=i),
                 )
         for cell in cells:
             if cell is None:
                 raise Exception("got null cell, investigate!")
         return cells
 
-    @validator("content", pre=True)
+    @field_validator("content", mode="before")
     def convert_content_from_obj(cls, v):
         if v is None:
             return []
         if isinstance(v, list):
             for i, element in enumerate(v):
                 if isinstance(element, str):
                     v[i] = Content(type=Type.from_string(element))
                 elif isinstance(element, dict):
                     v[i] = BaseModel._to_type(element)
         return v
 
+    def __call__(self, *args, **kwargs):
+        return HTML("")
+
 
 class ContentMarkdown(Content):
     content: Optional[str] = ""
 
     def generate(
         self,
         metadata: Optional[dict] = None,
```

### Comparing `nbprint-0.1.6/nbprint/config/content/common.py` & `nbprint-0.1.7/nbprint/config/content/common.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/content/image.py` & `nbprint-0.1.7/nbprint/config/content/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from IPython.display import HTML, Image
 from pathlib import Path
-from pydantic import Field, FilePath, validator
+from pydantic import Field, FilePath, field_validator
 from typing import List, Optional
 
 from .base import Content
 
 
 class ContentImage(Content):
     path: Optional[FilePath] = None
     content: Optional[bytes] = b""
     tags: List[str] = Field(default=["nbprint:content", "nbprint:content:image"])
 
-    @validator("path", pre=True)
+    @field_validator("path", mode="before")
     def convert_path_from_obj(cls, v):
         if isinstance(v, str):
             v = Path(v).resolve()
         return v
 
-    @validator("content", pre=True)
+    @field_validator("content", mode="before")
     def convert_content_from_obj(cls, v):
         if v is None:
             return b""
         if v and isinstance(v, str):
             v = Path(v).resolve()
         if v and isinstance(v, Path):
             v = v.read_bytes()
         return v
 
-    def __call__(self, ctx=None, *args, **kwargs):
+    def as_base64(self):
         if self.path:
             img = Image(filename=self.path)
         else:
             img = Image(data=self.content)
-        return HTML(f"""<img src="data:image/png;base64,{img._repr_png_()}">""")
+        return img._repr_png_()
+
+    def __call__(self, ctx=None, *args, **kwargs):
+        return HTML(f"""<img src="data:image/png;base64,{self.as_base64()}">""")
 
     def __repr__(self) -> str:
         return f"Image(path='{self.path}', content=[{len(self.content)} bytes])"
```

### Comparing `nbprint-0.1.6/nbprint/config/content/page.py` & `nbprint-0.1.7/nbprint/config/content/page.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/core/config.py` & `nbprint-0.1.7/nbprint/config/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from hydra import compose, initialize_config_dir
 from hydra.utils import instantiate
 from nbformat import NotebookNode
 from nbformat.v4 import new_notebook
-from omegaconf import DictConfig, OmegaConf
 from pathlib import Path
 from pprint import pprint
-from pydantic import Field, PrivateAttr, validator
+from pydantic import Field, PrivateAttr, field_validator
 from sys import version_info
 from typing import Dict, List, Union
 
 from ... import __version__
 from ..base import BaseModel, Role, Type, _append_or_extend
 from ..content import Content
 from ..page import Page
@@ -38,40 +37,40 @@
     ignore: bool = True
     debug: bool = True
 
     # internals
     _nb_var_name: str = PrivateAttr(default="nbprint_config")
     _nb_vars: set = PrivateAttr(default_factory=set)
 
-    @validator("resources", pre=True)
+    @field_validator("resources", mode="before")
     def convert_resources_from_obj(cls, value):
         if value is None:
             value = {}
         if isinstance(value, dict):
             for k, v in value.items():
                 value[k] = BaseModel._to_type(v)
         return value
 
-    @validator("outputs", pre=True)
+    @field_validator("outputs", mode="before")
     def convert_outputs_from_obj(cls, v):
         return BaseModel._to_type(v, Outputs)
 
-    @validator("parameters", pre=True)
+    @field_validator("parameters", mode="before")
     def convert_parameters_from_obj(cls, v):
         return BaseModel._to_type(v, Parameters)
 
-    @validator("page", pre=True)
+    @field_validator("page", mode="before")
     def convert_page_from_obj(cls, v):
         return BaseModel._to_type(v, Page)
 
-    @validator("context", pre=True)
+    @field_validator("context", mode="before")
     def convert_context_from_obj(cls, v):
         return BaseModel._to_type(v, Context)
 
-    @validator("content", pre=True)
+    @field_validator("content", mode="before")
     def convert_content_from_obj(cls, v):
         if v is None:
             return []
         if isinstance(v, list):
             for i, element in enumerate(v):
                 if isinstance(element, str):
                     v[i] = Content(type=Type.from_string(element))
@@ -163,29 +162,26 @@
         if isinstance(path_or_model, Configuration):
             return path_or_model
 
         if isinstance(path_or_model, str) and (path_or_model.endswith(".yml") or path_or_model.endswith(".yaml")):
             path_or_model = Path(path_or_model).resolve()
 
         if isinstance(path_or_model, Path):
-            path_or_model = OmegaConf.load(path_or_model)
-
-        if isinstance(path_or_model, DictConfig):
-            container = OmegaConf.to_container(path_or_model, resolve=True, throw_on_missing=True)
-            return Configuration(name=name, **container)
-
+            path_or_model = path_or_model.resolve()
+            folder = str(path_or_model.parent)
+            file = str(path_or_model.name)
+
+            with initialize_config_dir(version_base=None, config_dir=folder, job_name=name):
+                cfg = compose(config_name=file, overrides=[f"+name={name}"])
+                config = instantiate(cfg)
+                if not isinstance(config, Configuration):
+                    config = Configuration(**config)
+                return config
         raise TypeError(f"Path or model malformed: {path_or_model} {type(path_or_model)}")
 
-    @staticmethod
-    def load_hydra(folder, file, name):
-        with initialize_config_dir(version_base=None, config_dir=folder, job_name=name):
-            cfg = compose(config_name=file, overrides=[f"+name={name}"])
-            config = instantiate(cfg)
-            return config
-
     def run(self):
         gen = self.generate(self)
         if self.debug:
             pprint(gen)
         self.outputs.run(self, gen)
```

### Comparing `nbprint-0.1.6/nbprint/config/core/context.py` & `nbprint-0.1.7/nbprint/config/core/context.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/config/core/outputs.py` & `nbprint-0.1.7/nbprint/config/core/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 from nbformat import NotebookNode, write
 from pathlib import Path
-from pydantic import DirectoryPath, Field, validator
+from pydantic import DirectoryPath, Field, field_validator
 from strenum import StrEnum
 from typing import TYPE_CHECKING, List, Literal, Optional, Union
 from uuid import uuid4
 
 from ..base import BaseModel, Role
 
 if TYPE_CHECKING:
@@ -26,15 +26,15 @@
     path_root: DirectoryPath
     naming: List[Union[OutputNaming, str]] = [OutputNaming.name, "-", OutputNaming.date]
 
     tags: List[str] = Field(default=["nbprint:outputs"])
     role: Role = Role.OUTPUTS
     ignore: bool = True
 
-    @validator("path_root", pre=True)
+    @field_validator("path_root", mode="before")
     def convert_str_to_path(cls, v):
         if isinstance(v, str):
             v = Path(v)
         if isinstance(v, Path):
             v.resolve().mkdir(parents=True, exist_ok=True)
             return v
         raise TypeError
```

### Comparing `nbprint-0.1.6/nbprint/config/core/parameters.py` & `nbprint-0.1.7/nbprint/config/core/parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from .config import Configuration
 
 __all__ = ("Parameters",)
 
 
 class Parameters(BaseModel):
     tags: List[str] = Field(default=["parameters", "nbprint:parameters"])
-    role: Role = Role.CONTENT
+    role: Role = Role.PARAMETERS
     ignore: bool = True
 
     def generate(self, metadata: dict, config: "Configuration", *args, **kwargs) -> NotebookNode:
         cell = self._base_generate_meta(metadata=metadata)
         # if nb_vars:
         #     # add parameter variable
         #     nb_vars.add(k)
```

### Comparing `nbprint-0.1.6/nbprint/example/basic/cover.py` & `nbprint-0.1.7/nbprint/example/basic/cover.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 class ExampleCoverPageContent(ContentCover):
     logo: Optional[ContentImage]
     title: Optional[str] = ""
     subtitle: Optional[str] = ""
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, ctx=None, *args, **kwargs):
         return HTML(f"""
             {self.logo()._repr_html_()}
             <h1>{self.title}</h1>
             <h2>{self.subtitle}</h2>
+            <h3>{ctx.string}</h3>
             <p class="pagebreak"></p>
         """)
```

### Comparing `nbprint-0.1.6/nbprint/example/basic/markdown.py` & `nbprint-0.1.7/nbprint/example/basic/markdown.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/example/finance/content.py` & `nbprint-0.1.7/nbprint/example/finance/content.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/example/research/content.py` & `nbprint-0.1.7/nbprint/example/research/content.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/embedded.css` & `nbprint-0.1.7/nbprint/extension/embedded.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/embedded.js` & `nbprint-0.1.7/nbprint/extension/embedded.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/embedded.js.map` & `nbprint-0.1.7/nbprint/extension/embedded.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/fontawesome.min.css` & `nbprint-0.1.7/nbprint/extension/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/index.css` & `nbprint-0.1.7/nbprint/extension/index.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/index.js` & `nbprint-0.1.7/nbprint/extension/index.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/index.js.map` & `nbprint-0.1.7/nbprint/extension/index.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/extension/table-of-content.css` & `nbprint-0.1.7/nbprint/extension/table-of-content.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/index.html.j2` & `nbprint-0.1.7/nbprint/templates/nbprint/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.css` & `nbprint-0.1.7/nbprint/templates/nbprint/static/embedded.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js` & `nbprint-0.1.7/nbprint/templates/nbprint/static/embedded.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js.map` & `nbprint-0.1.7/nbprint/templates/nbprint/static/embedded.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/fontawesome.min.css` & `nbprint-0.1.7/nbprint/templates/nbprint/static/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/index.js` & `nbprint-0.1.7/nbprint/templates/nbprint/static/index.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/index.js.map` & `nbprint-0.1.7/nbprint/templates/nbprint/static/index.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/nbprint.css` & `nbprint-0.1.7/nbprint/templates/nbprint/static/nbprint.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/templates/nbprint/static/table-of-content.css` & `nbprint-0.1.7/nbprint/templates/nbprint/static/table-of-content.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/tests/config/common/test_styles.py` & `nbprint-0.1.7/nbprint/tests/config/common/test_styles.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/utils/format.py` & `nbprint-0.1.7/nbprint/utils/format.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,25 +40,14 @@
 def newpage():
     """make a new page. in html, this just does a horizontal rule"""
     p = dt.p()
     p.attributes["style"] = "page-break-before: always;"
     return _html(str(p))
 
 
-def table(df, title="", footnote=""):
-    """helper to display a table"""
-    ret = ""
-    if title:
-        ret += "### {}\n".format(title)
-    ret += df.to_html()
-    if footnote:
-        ret += "\n" + footnote + "\n"
-    return _html(ret)
-
-
 def pagenum():
     """display a page number (latex only)"""
     # TODO
     return "[pagenum]"
 
 
 def _make(text, h_type, **kwargs):
```

### Comparing `nbprint-0.1.6/nbprint/utils/image.py` & `nbprint-0.1.7/nbprint/utils/image.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/voila/base.html.j2` & `nbprint-0.1.7/nbprint/voila/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/voila/browser-open.html` & `nbprint-0.1.7/nbprint/voila/browser-open.html`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/voila/index.html.j2` & `nbprint-0.1.7/nbprint/voila/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/voila/mathjax.html.j2` & `nbprint-0.1.7/nbprint/voila/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/nbprint/voila/mermaidjs.html.j2` & `nbprint-0.1.7/nbprint/voila/mermaidjs.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/.gitignore` & `nbprint-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/LICENSE` & `nbprint-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.6/README.md` & `nbprint-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-<a href="https://github.com/timkpaine/nbprint#gh-light-mode-only">
-  <img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/logo-light.png?raw=true#gh-light-mode-only" alt="nbprint" width="400"></a>
+<a href="https://github.com/nbprint/nbprint#gh-light-mode-only">
+  <img src="https://github.com/nbprint/nbprint/raw/main/docs/img/logo-light.png?raw=true#gh-light-mode-only" alt="nbprint" width="400"></a>
 </a>
-<a href="https://github.com/timkpaine/nbprint#gh-dark-mode-only">
-  <img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/logo-dark.png?raw=true#gh-dark-mode-only" alt="nbprint" width="400"></a>
+<a href="https://github.com/nbprint/nbprint#gh-dark-mode-only">
+  <img src="https://github.com/nbprint/nbprint/raw/main/docs/img/logo-dark.png?raw=true#gh-dark-mode-only" alt="nbprint" width="400"></a>
 </a>
 <br/>
 
 A framework for building print media with [nbconvert](https://nbconvert.readthedocs.io).
 
-[![Build Status](https://github.com/timkpaine/nbprint/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/timkpaine/nbprint/actions?query=workflow%3A%22Build+Status%22)
-[![Coverage](https://codecov.io/gh/timkpaine/nbprint/branch/main/graph/badge.svg?token=ag2j2TV2wE)](https://codecov.io/gh/timkpaine/nbprint)
-[![GitHub issues](https://img.shields.io/github/issues/timkpaine/nbprint.svg)](https://github.com/timkpaine/nbprint/issues)
+[![Build Status](https://github.com/nbprint/nbprint/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/nbprint/nbprint/actions?query=workflow%3A%22Build+Status%22)
+[![Coverage](https://codecov.io/gh/nbprint/nbprint/branch/main/graph/badge.svg?token=ag2j2TV2wE)](https://codecov.io/gh/nbprint/nbprint)
+[![GitHub issues](https://img.shields.io/github/issues/nbprint/nbprint.svg)](https://github.com/nbprint/nbprint/issues)
 [![PyPI](https://img.shields.io/pypi/l/nbprint.svg)](https://pypi.python.org/pypi/nbprint)
 [![PyPI](https://img.shields.io/pypi/v/nbprint.svg)](https://pypi.python.org/pypi/nbprint)
 
 ## Installation
 Install with `pip`:
 
 ```bash
@@ -114,21 +114,21 @@
 
 ```bash
 nbprint examples/basic.yaml basic
 ```
 
 This will create a Notebook output in our specified folder `examples/output`, as well as an html asset (since that is what we specified in the yaml file). Both will have the date as a suffix, which is also configureable in our yaml. We see the generated report notebook, which we can open and use for further experimentation or to investigate the report itself.
 
-<img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/example-notebook.png?raw=true" alt="example notebook output" width="800"></a>
+<img src="https://github.com/nbprint/nbprint/raw/main/docs/img/example-notebook.png?raw=true" alt="example notebook output" width="800"></a>
 
 We also see the html document itself, which will be rendered via [`pagedjs`](https://pagedjs.org) print preview.
 
-<img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/example-basic.png?raw=true" alt="example basic output" width="800"></a>
+<img src="https://github.com/nbprint/nbprint/raw/main/docs/img/example-basic.png?raw=true" alt="example basic output" width="800"></a>
 
-You can find a pdf form of this document [here](https://github.com/timkpaine/nbprint/raw/main/docs/img/example-basic.pdf?raw=true).
+You can find a pdf form of this document [here](https://github.com/nbprint/nbprint/raw/main/docs/img/example-basic.pdf?raw=true).
 
 
 ## Development
 **Warning**: This project is under active development, so all APIs are subject to change!
 
 ## Related Projects
 - [nbconvert](https://nbconvert.readthedocs.io/en/latest/): Convert Notebooks to other formats
```

#### html2text {}

```diff
@@ -1,54 +1,53 @@
 _[_n_b_p_r_i_n_t_]
 _[_n_b_p_r_i_n_t_]
 
 A framework for building print media with [nbconvert](https://
-nbconvert.readthedocs.io). [![Build Status](https://github.com/timkpaine/
-nbprint/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/
-timkpaine/nbprint/actions?query=workflow%3A%22Build+Status%22) [![Coverage]
-(https://codecov.io/gh/timkpaine/nbprint/branch/main/graph/
-badge.svg?token=ag2j2TV2wE)](https://codecov.io/gh/timkpaine/nbprint) [![GitHub
-issues](https://img.shields.io/github/issues/timkpaine/nbprint.svg)](https://
-github.com/timkpaine/nbprint/issues) [![PyPI](https://img.shields.io/pypi/l/
-nbprint.svg)](https://pypi.python.org/pypi/nbprint) [![PyPI](https://
-img.shields.io/pypi/v/nbprint.svg)](https://pypi.python.org/pypi/nbprint) ##
-Installation Install with `pip`: ```bash pip install nbprint ``` Install with
-`conda` ```bash conda install nbprint -c conda-forge ``` ## Background Jupyter
-Notebooks are widely used for reports via [`nbconvert`](https://
-nbconvert.readthedocs.io/en/latest/). Most efforts focus on building web
-reports / websites from notebooks, including [`VoilÃ `](https://github.com/
-voila-dashboards/voila) and [`Jupyter Book`](https://jupyterbook.org/en/stable/
-intro.html). Despite being the primary goal of early notebook conversion
-efforts, in recent years much less focus has been spent on print media - PDFs
-for reports, academic papers, newspapers, etc. There are many examples of
-`nbconvert` templates for academic papers, as well as projects like
-[`ipypublish`](https://github.com/chrisjsewell/ipypublish/tree/develop). Most
-of these efforts focus on $\LaTeX$, and indeed `nbprint` itself started as
-convenience framework for formatting charts and tables similarly between html
-and pdf outputs. However, with recent releases to `nbconvert`, which now
-supports `webpdf` (printing as pdf from within a headless web browser), and
-with advances to the `@media print` CSS directive spearheaded by the lovely
-folks at [`pagedjs`](https://pagedjs.org), it is now much easier to build
-publication ready print-oriented media on the web. This is the goal of
-`nbprint`. Using [`pagedjs`](https://pagedjs.org), `nbprint` provides templates
-and utilities for building web reports targetting print media. Beyong that, it
-provides infrastructure for parameterizing and configuring documents via
-[`pydantic`](https://docs.pydantic.dev/latest/), which makes designing and
-generating reports a breeze, even without knowledge of Python. ## Quickstart
-`nbprint` can be used purely via notebook metadata, but it also provides a
-`yaml`-based framework for configuration (via [`pydantic`](https://
-docs.pydantic.dev/latest/) and [`omegaconf`](https://github.com/omry/
-omegaconf)). This is particularly convenient when generating parameterized
-reports, for example when configuring a large number of hyperparameters for a
-model's evaluation report. This configuration also allows for easier iteration
-on a report's design and content. ### Configuration Let's take a simple
-placeholder report. ```yaml --- debug: false outputs: type: nbprint:
-NBConvertOutputs path_root: ./examples/output target: "html" content: - type:
-nbprint:ContentMarkdown content: | # A Generic Report ## A Subtitle css: ":
-scope { text-align: center; }" - type: nbprint:ContentPageBreak - type:
+nbconvert.readthedocs.io). [![Build Status](https://github.com/nbprint/nbprint/
+actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/nbprint/
+nbprint/actions?query=workflow%3A%22Build+Status%22) [![Coverage](https://
+codecov.io/gh/nbprint/nbprint/branch/main/graph/badge.svg?token=ag2j2TV2wE)]
+(https://codecov.io/gh/nbprint/nbprint) [![GitHub issues](https://
+img.shields.io/github/issues/nbprint/nbprint.svg)](https://github.com/nbprint/
+nbprint/issues) [![PyPI](https://img.shields.io/pypi/l/nbprint.svg)](https://
+pypi.python.org/pypi/nbprint) [![PyPI](https://img.shields.io/pypi/v/
+nbprint.svg)](https://pypi.python.org/pypi/nbprint) ## Installation Install
+with `pip`: ```bash pip install nbprint ``` Install with `conda` ```bash conda
+install nbprint -c conda-forge ``` ## Background Jupyter Notebooks are widely
+used for reports via [`nbconvert`](https://nbconvert.readthedocs.io/en/latest/
+). Most efforts focus on building web reports / websites from notebooks,
+including [`VoilÃ `](https://github.com/voila-dashboards/voila) and [`Jupyter
+Book`](https://jupyterbook.org/en/stable/intro.html). Despite being the primary
+goal of early notebook conversion efforts, in recent years much less focus has
+been spent on print media - PDFs for reports, academic papers, newspapers, etc.
+There are many examples of `nbconvert` templates for academic papers, as well
+as projects like [`ipypublish`](https://github.com/chrisjsewell/ipypublish/
+tree/develop). Most of these efforts focus on $\LaTeX$, and indeed `nbprint`
+itself started as convenience framework for formatting charts and tables
+similarly between html and pdf outputs. However, with recent releases to
+`nbconvert`, which now supports `webpdf` (printing as pdf from within a
+headless web browser), and with advances to the `@media print` CSS directive
+spearheaded by the lovely folks at [`pagedjs`](https://pagedjs.org), it is now
+much easier to build publication ready print-oriented media on the web. This is
+the goal of `nbprint`. Using [`pagedjs`](https://pagedjs.org), `nbprint`
+provides templates and utilities for building web reports targetting print
+media. Beyong that, it provides infrastructure for parameterizing and
+configuring documents via [`pydantic`](https://docs.pydantic.dev/latest/),
+which makes designing and generating reports a breeze, even without knowledge
+of Python. ## Quickstart `nbprint` can be used purely via notebook metadata,
+but it also provides a `yaml`-based framework for configuration (via
+[`pydantic`](https://docs.pydantic.dev/latest/) and [`omegaconf`](https://
+github.com/omry/omegaconf)). This is particularly convenient when generating
+parameterized reports, for example when configuring a large number of
+hyperparameters for a model's evaluation report. This configuration also allows
+for easier iteration on a report's design and content. ### Configuration Let's
+take a simple placeholder report. ```yaml --- debug: false outputs: type:
+nbprint:NBConvertOutputs path_root: ./examples/output target: "html" content: -
+type: nbprint:ContentMarkdown content: | # A Generic Report ## A Subtitle css:
+":scope { text-align: center; }" - type: nbprint:ContentPageBreak - type:
 nbprint:ContentTableOfContents - type: nbprint:ContentPageBreak - type:
 nbprint:ContentMarkdown content: | # Section One Lorem ipsum dolor sit amet. ##
 Subsection One Consectetur adipiscing elit, sed do eiusmod tempor incididunt.
 ## Subsection Two Ut labore et dolore magna aliqua. - type: nbprint:
 ContentPageBreak - type: nbprint:ContentFlexRowLayout sizes: [1, 1] content: -
 type: nbprint:ContentFlexColumnLayout content: - type: nbprint:ContentMarkdown
 content: | # Section Two Lorem ipsum dolor sit amet. ## Subsection One
@@ -68,15 +67,15 @@
 Notebook output in our specified folder `examples/output`, as well as an html
 asset (since that is what we specified in the yaml file). Both will have the
 date as a suffix, which is also configureable in our yaml. We see the generated
 report notebook, which we can open and use for further experimentation or to
 investigate the report itself. [example notebook output]
 We also see the html document itself, which will be rendered via [`pagedjs`]
 (https://pagedjs.org) print preview. [example basic output]
-You can find a pdf form of this document [here](https://github.com/timkpaine/
+You can find a pdf form of this document [here](https://github.com/nbprint/
 nbprint/raw/main/docs/img/example-basic.pdf?raw=true). ## Development
 **Warning**: This project is under active development, so all APIs are subject
 to change! ## Related Projects - [nbconvert](https://nbconvert.readthedocs.io/
 en/latest/): Convert Notebooks to other formats - [pagedjs](https://
 pagedjs.org): Paged.js is a free and open-source library that paginates any
 HTML content to produce beautiful print-ready PDF - [VoilÃ ](https://
 github.com/voila-dashboards/voila): VoilÃ  turns Jupyter notebooks into
```

### Comparing `nbprint-0.1.6/pyproject.toml` & `nbprint-0.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "jupyterlab>=4,<5",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "nbprint"
 description = "A framework for customizing NBConvert templates and building reports"
-version = "0.1.6"
+version = "0.1.7"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 authors = [
     { name = "Tim Paine", email = "t.paine154@gmail.com" },
 ]
 keywords = [
@@ -36,57 +36,53 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 dependencies = [
     "dominate",
+    "hydra-core",
     "ipywidgets",
     "nbconvert>=7.11.0",
     "nbformat",
     "notebook",
     "omegaconf",
     "pydantic>=2,<3",
     "pydantic_extra_types",
     "strenum",
     "typer",
 ]
 
 [project.optional-dependencies]
-hydra = [
-    "hydra-core",
-]
 develop = [
     "check-manifest",
     "isort>=5,<6",
     "ruff>=0.3,<0.4",
     # test
     "pytest",
     "pytest-cov",
-    # hydra
-    "hydra-core",
     # notebook deps
+    "great_tables",
     "matplotlib",
     "pandas",
     "perspective-python",
     "seaborn",
     "superstore",
 ]
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 [project.scripts]
 nbprint = "nbprint.cli:main"
-nbprint-hydra = "nbprint.cli:main_hydra"
 
 [project.urls]
-repository = "https://github.com/timkpaine/nbprint"
-homepage = "https://github.com/timkpaine/nbprint"
+repository = "https://github.com/nbprint/nbprint"
+homepage = "https://github.com/nbprint/nbprint"
 
 [tool.hatch.build]
 artifacts = [
     "nbprint/templates",
     "nbprint/extension",
 ]
```

### Comparing `nbprint-0.1.6/PKG-INFO` & `nbprint-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: nbprint
-Version: 0.1.6
+Version: 0.1.7
 Summary: A framework for customizing NBConvert templates and building reports
-Project-URL: repository, https://github.com/timkpaine/nbprint
-Project-URL: homepage, https://github.com/timkpaine/nbprint
+Project-URL: repository, https://github.com/nbprint/nbprint
+Project-URL: homepage, https://github.com/nbprint/nbprint
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -216,55 +216,54 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: dominate
+Requires-Dist: hydra-core
 Requires-Dist: ipywidgets
 Requires-Dist: nbconvert>=7.11.0
 Requires-Dist: nbformat
 Requires-Dist: notebook
 Requires-Dist: omegaconf
 Requires-Dist: pydantic-extra-types
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: strenum
 Requires-Dist: typer
 Provides-Extra: develop
 Requires-Dist: check-manifest; extra == 'develop'
-Requires-Dist: hydra-core; extra == 'develop'
+Requires-Dist: great-tables; extra == 'develop'
 Requires-Dist: isort<6,>=5; extra == 'develop'
 Requires-Dist: matplotlib; extra == 'develop'
 Requires-Dist: pandas; extra == 'develop'
 Requires-Dist: perspective-python; extra == 'develop'
 Requires-Dist: pytest; extra == 'develop'
 Requires-Dist: pytest-cov; extra == 'develop'
 Requires-Dist: ruff<0.4,>=0.3; extra == 'develop'
 Requires-Dist: seaborn; extra == 'develop'
 Requires-Dist: superstore; extra == 'develop'
-Provides-Extra: hydra
-Requires-Dist: hydra-core; extra == 'hydra'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
-<a href="https://github.com/timkpaine/nbprint#gh-light-mode-only">
-  <img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/logo-light.png?raw=true#gh-light-mode-only" alt="nbprint" width="400"></a>
+<a href="https://github.com/nbprint/nbprint#gh-light-mode-only">
+  <img src="https://github.com/nbprint/nbprint/raw/main/docs/img/logo-light.png?raw=true#gh-light-mode-only" alt="nbprint" width="400"></a>
 </a>
-<a href="https://github.com/timkpaine/nbprint#gh-dark-mode-only">
-  <img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/logo-dark.png?raw=true#gh-dark-mode-only" alt="nbprint" width="400"></a>
+<a href="https://github.com/nbprint/nbprint#gh-dark-mode-only">
+  <img src="https://github.com/nbprint/nbprint/raw/main/docs/img/logo-dark.png?raw=true#gh-dark-mode-only" alt="nbprint" width="400"></a>
 </a>
 <br/>
 
 A framework for building print media with [nbconvert](https://nbconvert.readthedocs.io).
 
-[![Build Status](https://github.com/timkpaine/nbprint/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/timkpaine/nbprint/actions?query=workflow%3A%22Build+Status%22)
-[![Coverage](https://codecov.io/gh/timkpaine/nbprint/branch/main/graph/badge.svg?token=ag2j2TV2wE)](https://codecov.io/gh/timkpaine/nbprint)
-[![GitHub issues](https://img.shields.io/github/issues/timkpaine/nbprint.svg)](https://github.com/timkpaine/nbprint/issues)
+[![Build Status](https://github.com/nbprint/nbprint/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/nbprint/nbprint/actions?query=workflow%3A%22Build+Status%22)
+[![Coverage](https://codecov.io/gh/nbprint/nbprint/branch/main/graph/badge.svg?token=ag2j2TV2wE)](https://codecov.io/gh/nbprint/nbprint)
+[![GitHub issues](https://img.shields.io/github/issues/nbprint/nbprint.svg)](https://github.com/nbprint/nbprint/issues)
 [![PyPI](https://img.shields.io/pypi/l/nbprint.svg)](https://pypi.python.org/pypi/nbprint)
 [![PyPI](https://img.shields.io/pypi/v/nbprint.svg)](https://pypi.python.org/pypi/nbprint)
 
 ## Installation
 Install with `pip`:
 
 ```bash
@@ -364,21 +363,21 @@
 
 ```bash
 nbprint examples/basic.yaml basic
 ```
 
 This will create a Notebook output in our specified folder `examples/output`, as well as an html asset (since that is what we specified in the yaml file). Both will have the date as a suffix, which is also configureable in our yaml. We see the generated report notebook, which we can open and use for further experimentation or to investigate the report itself.
 
-<img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/example-notebook.png?raw=true" alt="example notebook output" width="800"></a>
+<img src="https://github.com/nbprint/nbprint/raw/main/docs/img/example-notebook.png?raw=true" alt="example notebook output" width="800"></a>
 
 We also see the html document itself, which will be rendered via [`pagedjs`](https://pagedjs.org) print preview.
 
-<img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/example-basic.png?raw=true" alt="example basic output" width="800"></a>
+<img src="https://github.com/nbprint/nbprint/raw/main/docs/img/example-basic.png?raw=true" alt="example basic output" width="800"></a>
 
-You can find a pdf form of this document [here](https://github.com/timkpaine/nbprint/raw/main/docs/img/example-basic.pdf?raw=true).
+You can find a pdf form of this document [here](https://github.com/nbprint/nbprint/raw/main/docs/img/example-basic.pdf?raw=true).
 
 
 ## Development
 **Warning**: This project is under active development, so all APIs are subject to change!
 
 ## Related Projects
 - [nbconvert](https://nbconvert.readthedocs.io/en/latest/): Convert Notebooks to other formats
```

