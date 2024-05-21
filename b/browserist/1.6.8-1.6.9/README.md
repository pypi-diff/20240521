# Comparing `tmp/browserist-1.6.8.tar.gz` & `tmp/browserist-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserist-1.6.8.tar", last modified: Tue Feb  6 06:46:50 2024, max compression
+gzip compressed data, was "browserist-1.6.9.tar", last modified: Mon Apr  8 23:37:53 2024, max compression
```

## Comparing `browserist-1.6.8.tar` & `browserist-1.6.9.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.809389 browserist-1.6.8/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)    11343 2023-11-08 10:32:02.000000 browserist-1.6.8/LICENSE.md
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      193 2024-01-20 05:30:48.000000 browserist-1.6.8/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (502) staff       (20)    17322 2024-02-06 06:46:50.807991 browserist-1.6.8/PKG-INFO
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4095 2024-02-06 06:38:37.000000 browserist-1.6.8/README.md
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      140 2024-01-20 05:30:48.000000 browserist-1.6.8/pyproject.toml
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2162 2024-02-06 06:46:50.811835 browserist-1.6.8/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.219487 browserist-1.6.8/src/
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.242345 browserist-1.6.8/src/browserist/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1016 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.251809 browserist-1.6.8/src/browserist/browser/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4953 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/__main__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.261259 browserist-1.6.8/src/browserist/browser/check_if/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/check_if/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     5058 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/check_if/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      431 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/check_if/contains_any_text.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      574 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/check_if/contains_text.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      400 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/check_if/does_exist.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      501 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/check_if/is_clickable.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      299 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/check_if/is_disabled.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      411 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/check_if/is_displayed.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      407 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/check_if/is_enabled.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      504 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/check_if/is_image_loaded.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      999 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/check_if/is_in_viewport.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      409 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/check_if/is_selected.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.265880 browserist-1.6.8/src/browserist/browser/click/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/click/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     7179 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/click/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      705 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/click/button.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1094 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/click/button_if_contains_text.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      997 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/click/download.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      815 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/click/download_and_get_file_path.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.271426 browserist-1.6.8/src/browserist/browser/combo/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/combo/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     7856 2024-02-06 06:04:44.000000 browserist-1.6.8/src/browserist/browser/combo/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4279 2024-02-05 19:24:18.000000 browserist-1.6.8/src/browserist/browser/combo/cookie_banner.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     5396 2024-02-06 06:04:44.000000 browserist-1.6.8/src/browserist/browser/combo/log_in.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1370 2024-02-02 09:43:57.000000 browserist-1.6.8/src/browserist/browser/combo/search.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.278350 browserist-1.6.8/src/browserist/browser/get/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/get/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     5230 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/__main__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.281553 browserist-1.6.8/src/browserist/browser/get/attribute/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/get/attribute/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2268 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/attribute/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      496 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/attribute/value.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      533 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/attribute/values.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      623 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/dimensions.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      784 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/element.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      801 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/elements.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      464 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/elements_by_tag.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      183 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/page_title.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      709 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/text.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      475 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/texts.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.289405 browserist-1.6.8/src/browserist/browser/get/url/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/get/url/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4436 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/current.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      270 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/current_domain.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      697 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/from_image.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      349 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/from_images.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      699 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/from_link.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      349 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/get/url/from_links.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.292314 browserist-1.6.8/src/browserist/browser/iframe/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/iframe/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1084 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/iframe/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      517 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/iframe/switch_to.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      208 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/iframe/switch_to_original_page.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.296423 browserist-1.6.8/src/browserist/browser/input/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/input/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2472 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/input/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      479 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/input/clear.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      445 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/input/select.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      572 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/input/value.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.298741 browserist-1.6.8/src/browserist/browser/mouse/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/mouse/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      818 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/mouse/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      610 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/mouse/hover.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.304727 browserist-1.6.8/src/browserist/browser/open/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/open/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1671 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/open/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      237 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/open/url.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      986 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/open/url_if_not_current.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.308647 browserist-1.6.8/src/browserist/browser/prompt/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/prompt/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1588 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/prompt/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      474 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/prompt/input_value.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      647 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/prompt/proceed_yes_or_no.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.318617 browserist-1.6.8/src/browserist/browser/screenshot/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/screenshot/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4911 2024-01-20 05:30:48.000000 browserist-1.6.8/src/browserist/browser/screenshot/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1116 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/screenshot/complete_page.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      992 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/screenshot/element.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      796 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/screenshot/visible_portion.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.326593 browserist-1.6.8/src/browserist/browser/scroll/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     5798 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/scroll/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      373 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/by.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.329223 browserist-1.6.8/src/browserist/browser/scroll/check_if/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/check_if/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1122 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/scroll/check_if/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      725 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/check_if/is_end_of_page.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      245 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/check_if/is_top_of_page.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      238 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/down_by.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.336248 browserist-1.6.8/src/browserist/browser/scroll/get/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/get/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1055 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/scroll/get/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      347 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/get/position.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      545 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/get/total_height.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      681 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/into_view.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      483 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/into_view_if_not_visible.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      239 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/left_by.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.339675 browserist-1.6.8/src/browserist/browser/scroll/page/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/page/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1875 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/scroll/page/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      384 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/page/down.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1338 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/scroll/page/to_end.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      251 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/page/to_top.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      385 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/page/up.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      239 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/right_by.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      382 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/to_position.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      237 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/scroll/up_by.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.343026 browserist-1.6.8/src/browserist/browser/tool/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/tool/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2902 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/tool/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      454 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/tool/count_elements.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      412 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/tool/execute_script.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      216 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/tool/is_input_valid.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.344252 browserist-1.6.8/src/browserist/browser/viewport/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      561 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/__main__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.350046 browserist-1.6.8/src/browserist/browser/viewport/get/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/get/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1377 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/viewport/get/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      248 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/get/height.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      330 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/get/size.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      246 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/get/width.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.355900 browserist-1.6.8/src/browserist/browser/viewport/set/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/set/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1852 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/viewport/set/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      982 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/set/size.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      318 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/viewport/set/size_by_device.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.359926 browserist-1.6.8/src/browserist/browser/wait/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2351 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1648 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/wait/for_element.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      158 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/random_seconds.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       80 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/seconds.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.372609 browserist-1.6.8/src/browserist/browser/wait/until/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4815 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      467 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/contains_any_text.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.376624 browserist-1.6.8/src/browserist/browser/wait/until/download_file/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/download_file/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2978 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/download_file/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      506 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/download_file/does_not_exist.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      497 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/download_file/exists.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1499 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/download_file/size_does_not_increase.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      446 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/element_disappears.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      894 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/images_have_loaded.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      438 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/is_clickable.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1212 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/wait/until/number_of_window_handles_is.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.380356 browserist-1.6.8/src/browserist/browser/wait/until/page_title/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/page_title/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2500 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/page_title/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      542 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/page_title/changes.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1197 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/wait/until/page_title/contains.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1153 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/wait/until/page_title/equals.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.387720 browserist-1.6.8/src/browserist/browser/wait/until/text/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/text/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2666 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/text/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      722 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/text/changes.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      789 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/text/contains.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      742 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/text/equals.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.390823 browserist-1.6.8/src/browserist/browser/wait/until/url/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/url/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3491 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/wait/until/url/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      593 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/wait/until/url/changes.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1118 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/wait/until/url/contains.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1134 2024-02-06 06:04:35.000000 browserist-1.6.8/src/browserist/browser/wait/until/url/equals.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.475407 browserist-1.6.8/src/browserist/browser/window/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3670 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      463 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/close.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      194 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/fullscreen.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.488245 browserist-1.6.8/src/browserist/browser/window/get/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/get/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2017 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/get/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      234 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/get/height.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      327 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/get/position.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      320 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/get/size.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      232 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/get/width.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.492085 browserist-1.6.8/src/browserist/browser/window/handle/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/handle/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1929 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/handle/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      433 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/handle/all.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      403 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/handle/count.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      211 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/handle/current.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      190 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/maximize.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      190 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/minimize.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.495253 browserist-1.6.8/src/browserist/browser/window/open/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/open/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2921 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/open/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1291 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/open/new_tab_or_window.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.569732 browserist-1.6.8/src/browserist/browser/window/set/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/browser/window/set/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1365 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/set/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      219 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/set/position.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      229 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/set/size.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      541 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/browser/window/switch_to.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.576393 browserist-1.6.8/src/browserist/constant/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      147 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/constant/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      184 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/constant/directory.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      247 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/constant/idle_timeout.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      170 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/constant/interval.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       48 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/constant/screenshot.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      249 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/constant/timeout.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.613226 browserist-1.6.8/src/browserist/exception/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      732 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/exception/download.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1392 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/element.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      273 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/file_png.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      723 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/headless.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      437 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/retry.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      250 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/scroll.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1821 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/timeout.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      254 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/url.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1762 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/window_handle.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      262 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/exception/xpath.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.620061 browserist-1.6.8/src/browserist/factory/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      129 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/factory/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1405 2024-02-02 09:30:34.000000 browserist-1.6.8/src/browserist/factory/chromium.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2442 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/factory/get.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1382 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/factory/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      887 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/factory/safari.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      717 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/factory/set.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.641547 browserist-1.6.8/src/browserist/helper/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      331 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      416 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/helper/date_time.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1364 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/directory.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1756 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/file.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1551 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/image.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1212 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/internet.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      155 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/operating_system.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/regex.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      468 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/terminal.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      768 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/timeout.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1595 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/url.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      272 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/helper/viewport.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      626 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/window_handle.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      476 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper/xpath.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.643680 browserist-1.6.8/src/browserist/helper_download/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1098 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper_download/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.645228 browserist-1.6.8/src/browserist/helper_iteration/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       41 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/helper_iteration/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3428 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper_iteration/retry.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.652635 browserist-1.6.8/src/browserist/helper_screenshot/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1008 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper_screenshot/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3489 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/helper_screenshot/complete_page.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1422 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper_screenshot/controller.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1420 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/helper_screenshot/file.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.655387 browserist-1.6.8/src/browserist/model/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.663685 browserist-1.6.8/src/browserist/model/browser/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      608 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/README.md
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.674816 browserist-1.6.8/src/browserist/model/browser/base/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/base/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4907 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/base/driver.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      459 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/base/page_load_strategy.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3215 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/base/settings.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.694998 browserist-1.6.8/src/browserist/model/browser/base/timeout/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/base/timeout/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1057 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/base/timeout/settings.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      261 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/base/timeout/strategy.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      263 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/base/type.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1239 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/chrome.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1646 2024-02-02 09:30:34.000000 browserist-1.6.8/src/browserist/model/browser/edge.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.697752 browserist-1.6.8/src/browserist/model/browser/extension/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/extension/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      601 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/extension/__main__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      439 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/extension/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      407 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/browser/extension/safari.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1777 2024-02-02 09:30:34.000000 browserist-1.6.8/src/browserist/model/browser/firefox.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1250 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1288 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/browser/safari.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.730073 browserist-1.6.8/src/browserist/model/combo_settings/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/combo_settings/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     2066 2024-02-02 09:43:57.000000 browserist-1.6.8/src/browserist/model/combo_settings/cookie_banner.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1145 2024-02-04 09:41:30.000000 browserist-1.6.8/src/browserist/model/combo_settings/handling_state.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      399 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/combo_settings/login_credentials.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4734 2024-02-06 06:04:44.000000 browserist-1.6.8/src/browserist/model/combo_settings/login_form.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1274 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/combo_settings/search.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.747377 browserist-1.6.8/src/browserist/model/download/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1634 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/chrome.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1262 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/edge.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1153 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/firefox.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)    13274 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/handler.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1386 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1364 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/download/safari.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1287 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/driver_methods.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3215 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/screenshot.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.772148 browserist-1.6.8/src/browserist/model/type/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/type/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      514 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/type/callable.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      823 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/type/file_png.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      968 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/type/path.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      773 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/type/url.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      811 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/type/xpath.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.775135 browserist-1.6.8/src/browserist/model/viewport/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/viewport/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.798769 browserist-1.6.8/src/browserist/model/viewport/collection/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/viewport/collection/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4202 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/apple.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1220 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/google.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1727 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/huawei.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1186 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/microsoft.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1106 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/oneplus.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      947 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/oppo.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1170 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/samsung.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      647 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/vivo.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1401 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/collection/xiaomi.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      613 2024-01-20 05:30:49.000000 browserist-1.6.8/src/browserist/model/viewport/common_devices.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      208 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/viewport/device.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.804027 browserist-1.6.8/src/browserist/model/window/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/window/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     3231 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/window/controller.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      261 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/window/handle.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      212 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/model/window/tab_or_window.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-11-08 10:32:02.000000 browserist-1.6.8/src/browserist/py.typed
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       80 2024-02-06 06:38:57.000000 browserist-1.6.8/src/browserist/version.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2024-02-06 06:46:50.805070 browserist-1.6.8/src/browserist.egg-info/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)    17322 2024-02-06 06:46:50.000000 browserist-1.6.8/src/browserist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (502) staff       (20)    12347 2024-02-06 06:46:50.000000 browserist-1.6.8/src/browserist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2024-02-06 06:46:50.000000 browserist-1.6.8/src/browserist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2023-12-02 08:00:31.000000 browserist-1.6.8/src/browserist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      187 2024-02-06 06:46:50.000000 browserist-1.6.8/src/browserist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       11 2024-02-06 06:46:50.000000 browserist-1.6.8/src/browserist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.526709 browserist-1.6.9/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    11343 2023-01-25 13:58:31.000000 browserist-1.6.9/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      193 2024-02-17 10:06:41.000000 browserist-1.6.9/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    17322 2024-04-08 23:37:53.526542 browserist-1.6.9/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4095 2024-04-08 23:32:04.000000 browserist-1.6.9/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      140 2024-02-17 10:06:41.000000 browserist-1.6.9/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2162 2024-04-08 23:37:53.527237 browserist-1.6.9/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.451449 browserist-1.6.9/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.456309 browserist-1.6.9/src/browserist/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1016 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.457555 browserist-1.6.9/src/browserist/browser/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4953 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/__main__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.460060 browserist-1.6.9/src/browserist/browser/check_if/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/check_if/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     5058 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/check_if/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      431 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/check_if/contains_any_text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      574 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/check_if/contains_text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      400 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/check_if/does_exist.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      501 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/check_if/is_clickable.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      299 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/check_if/is_disabled.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      411 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/check_if/is_displayed.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      407 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/check_if/is_enabled.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      504 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/check_if/is_image_loaded.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      999 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/check_if/is_in_viewport.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      409 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/check_if/is_selected.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.461254 browserist-1.6.9/src/browserist/browser/click/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/click/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     7163 2024-02-20 14:03:31.000000 browserist-1.6.9/src/browserist/browser/click/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      705 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/click/button.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1094 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/click/button_if_contains_text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      997 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/click/download.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      815 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/click/download_and_get_file_path.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.462517 browserist-1.6.9/src/browserist/browser/combo/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/combo/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     7856 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/combo/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4279 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/combo/cookie_banner.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     5396 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/combo/log_in.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1370 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/combo/search.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.464163 browserist-1.6.9/src/browserist/browser/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     5230 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/__main__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.464741 browserist-1.6.9/src/browserist/browser/get/attribute/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/get/attribute/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2268 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/attribute/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      496 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/attribute/value.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      533 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/attribute/values.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      623 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/dimensions.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      784 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      801 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/elements.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      464 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/elements_by_tag.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      183 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/page_title.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      709 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      475 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/texts.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.466261 browserist-1.6.9/src/browserist/browser/get/url/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/get/url/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4436 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/current.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      270 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/current_domain.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      697 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/from_image.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      349 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/from_images.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      699 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/from_link.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      349 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/get/url/from_links.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.466863 browserist-1.6.9/src/browserist/browser/iframe/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/iframe/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1084 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/iframe/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      517 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/iframe/switch_to.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      208 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/iframe/switch_to_original_page.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.467632 browserist-1.6.9/src/browserist/browser/input/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/input/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2472 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/input/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      479 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/input/clear.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      445 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/input/select.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/input/value.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.468093 browserist-1.6.9/src/browserist/browser/mouse/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/mouse/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      818 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/mouse/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      610 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/mouse/hover.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.468791 browserist-1.6.9/src/browserist/browser/open/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/open/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1671 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/open/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      237 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/open/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      986 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/open/url_if_not_current.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.469725 browserist-1.6.9/src/browserist/browser/prompt/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/prompt/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1588 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/prompt/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      474 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/prompt/input_value.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      647 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/prompt/proceed_yes_or_no.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.470641 browserist-1.6.9/src/browserist/browser/screenshot/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/screenshot/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4911 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/screenshot/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1116 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/screenshot/complete_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      992 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/screenshot/element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      796 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/screenshot/visible_portion.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.472346 browserist-1.6.9/src/browserist/browser/scroll/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     5798 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/scroll/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      373 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.472874 browserist-1.6.9/src/browserist/browser/scroll/check_if/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/check_if/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1122 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/scroll/check_if/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      725 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/check_if/is_end_of_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/check_if/is_top_of_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      238 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/down_by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.473401 browserist-1.6.9/src/browserist/browser/scroll/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1055 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/scroll/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/get/position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      545 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/get/total_height.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/into_view.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      483 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/into_view_if_not_visible.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/left_by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.474211 browserist-1.6.9/src/browserist/browser/scroll/page/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/page/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1875 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/scroll/page/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      384 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/page/down.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1338 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/scroll/page/to_end.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      251 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/page/to_top.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      385 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/page/up.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/right_by.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      382 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/to_position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      237 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/scroll/up_by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.474913 browserist-1.6.9/src/browserist/browser/tool/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/tool/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2902 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/tool/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      454 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/tool/count_elements.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      412 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/tool/execute_script.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      216 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/tool/is_input_valid.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.475265 browserist-1.6.9/src/browserist/browser/viewport/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      561 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/__main__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.476120 browserist-1.6.9/src/browserist/browser/viewport/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1377 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/viewport/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      248 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/get/height.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      330 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/get/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      246 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/get/width.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.476819 browserist-1.6.9/src/browserist/browser/viewport/set/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/set/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1852 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/viewport/set/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      982 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/set/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      318 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/viewport/set/size_by_device.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.477738 browserist-1.6.9/src/browserist/browser/wait/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2351 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1648 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/wait/for_element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      158 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/random_seconds.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/seconds.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.479266 browserist-1.6.9/src/browserist/browser/wait/until/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4815 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      467 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/contains_any_text.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.480407 browserist-1.6.9/src/browserist/browser/wait/until/download_file/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/download_file/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2978 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/download_file/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      506 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/download_file/does_not_exist.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      497 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/download_file/exists.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1499 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/download_file/size_does_not_increase.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      446 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/element_disappears.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      894 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/images_have_loaded.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      438 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/is_clickable.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1212 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/wait/until/number_of_window_handles_is.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.482358 browserist-1.6.9/src/browserist/browser/wait/until/page_title/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/page_title/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2500 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/page_title/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/page_title/changes.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1197 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/wait/until/page_title/contains.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1153 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/wait/until/page_title/equals.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.484328 browserist-1.6.9/src/browserist/browser/wait/until/text/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/text/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2666 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/text/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      722 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/text/changes.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/text/contains.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      742 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/text/equals.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.485495 browserist-1.6.9/src/browserist/browser/wait/until/url/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/url/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3491 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/wait/until/url/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/wait/until/url/changes.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1118 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/wait/until/url/contains.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1134 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/browser/wait/until/url/equals.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.486915 browserist-1.6.9/src/browserist/browser/window/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3670 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      463 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/close.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      194 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/fullscreen.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.488075 browserist-1.6.9/src/browserist/browser/window/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2017 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/get/height.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      327 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/get/position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      320 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/get/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      232 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/get/width.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.488990 browserist-1.6.9/src/browserist/browser/window/handle/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/handle/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1929 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/handle/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      433 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/handle/all.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      403 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/handle/count.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      211 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/handle/current.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      190 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/maximize.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      190 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/minimize.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.489467 browserist-1.6.9/src/browserist/browser/window/open/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/open/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2921 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/open/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1291 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/open/new_tab_or_window.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.490088 browserist-1.6.9/src/browserist/browser/window/set/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/browser/window/set/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1365 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/set/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      219 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/set/position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      229 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/set/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      541 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/browser/window/switch_to.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.491424 browserist-1.6.9/src/browserist/constant/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      147 2024-04-08 22:22:43.000000 browserist-1.6.9/src/browserist/constant/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      184 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/constant/directory.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      247 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/constant/idle_timeout.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      170 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/constant/interval.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       48 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/constant/screenshot.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      249 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/constant/timeout.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.493393 browserist-1.6.9/src/browserist/exception/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      732 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/exception/download.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1392 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      273 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/file_png.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      723 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/headless.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      437 2023-12-15 23:10:12.000000 browserist-1.6.9/src/browserist/exception/retry.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      250 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/scroll.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1821 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/timeout.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      254 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1762 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/window_handle.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      262 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/exception/xpath.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.494382 browserist-1.6.9/src/browserist/factory/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      129 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/factory/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1405 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/factory/chromium.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2442 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/factory/get.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1382 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/factory/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      887 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/factory/safari.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      717 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/factory/set.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.497365 browserist-1.6.9/src/browserist/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      331 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/helper/date_time.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1364 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/directory.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1756 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/file.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1540 2024-04-08 23:32:00.000000 browserist-1.6.9/src/browserist/helper/image.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1212 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/internet.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      155 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/operating_system.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/regex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      468 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/terminal.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      768 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/timeout.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1595 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      272 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/helper/viewport.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      626 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper/window_handle.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      460 2024-04-08 23:32:00.000000 browserist-1.6.9/src/browserist/helper/xpath.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.497612 browserist-1.6.9/src/browserist/helper_download/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1060 2024-04-08 23:32:00.000000 browserist-1.6.9/src/browserist/helper_download/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.497985 browserist-1.6.9/src/browserist/helper_iteration/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       41 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/helper_iteration/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3428 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper_iteration/retry.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.499068 browserist-1.6.9/src/browserist/helper_screenshot/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1007 2024-04-08 23:32:00.000000 browserist-1.6.9/src/browserist/helper_screenshot/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3489 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/helper_screenshot/complete_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1422 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper_screenshot/controller.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1420 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/helper_screenshot/file.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.499705 browserist-1.6.9/src/browserist/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.501659 browserist-1.6.9/src/browserist/model/browser/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      608 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.503944 browserist-1.6.9/src/browserist/model/browser/base/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/base/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4907 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/base/driver.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      459 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/base/page_load_strategy.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3215 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/base/settings.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.504589 browserist-1.6.9/src/browserist/model/browser/base/timeout/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/base/timeout/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1057 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/base/timeout/settings.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/base/timeout/strategy.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      263 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/base/type.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1239 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/chrome.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1646 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/model/browser/edge.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.506512 browserist-1.6.9/src/browserist/model/browser/extension/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/extension/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      601 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/extension/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      439 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/extension/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      407 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/browser/extension/safari.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1777 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/model/browser/firefox.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1250 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1288 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/browser/safari.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.510597 browserist-1.6.9/src/browserist/model/combo_settings/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/combo_settings/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2066 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/model/combo_settings/cookie_banner.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1145 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/model/combo_settings/handling_state.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      399 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/combo_settings/login_credentials.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4734 2024-02-17 10:06:47.000000 browserist-1.6.9/src/browserist/model/combo_settings/login_form.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1274 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/combo_settings/search.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.512259 browserist-1.6.9/src/browserist/model/download/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1634 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/chrome.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1262 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/edge.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1153 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/firefox.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    13274 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/handler.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1386 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1364 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/download/safari.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1287 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/driver_methods.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3206 2024-04-08 23:32:00.000000 browserist-1.6.9/src/browserist/model/screenshot.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.515538 browserist-1.6.9/src/browserist/model/type/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/type/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      514 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/type/callable.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      823 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/type/file_png.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      968 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/type/path.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      773 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/type/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      811 2023-02-01 06:40:45.000000 browserist-1.6.9/src/browserist/model/type/xpath.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.517112 browserist-1.6.9/src/browserist/model/viewport/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/viewport/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.523009 browserist-1.6.9/src/browserist/model/viewport/collection/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/viewport/collection/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4202 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/apple.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/google.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1727 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/huawei.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1186 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/microsoft.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1106 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/oneplus.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      947 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/oppo.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1170 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/samsung.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      647 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/vivo.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1401 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/collection/xiaomi.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      613 2024-02-17 10:06:41.000000 browserist-1.6.9/src/browserist/model/viewport/common_devices.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      208 2023-02-03 11:49:45.000000 browserist-1.6.9/src/browserist/model/viewport/device.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.524596 browserist-1.6.9/src/browserist/model/window/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/window/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3231 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/window/controller.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/window/handle.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      212 2023-01-25 13:58:31.000000 browserist-1.6.9/src/browserist/model/window/tab_or_window.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 15:16:10.000000 browserist-1.6.9/src/browserist/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2024-04-08 23:32:04.000000 browserist-1.6.9/src/browserist/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:53.525451 browserist-1.6.9/src/browserist.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    17322 2024-04-08 23:37:53.000000 browserist-1.6.9/src/browserist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    12347 2024-04-08 23:37:53.000000 browserist-1.6.9/src/browserist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2024-04-08 23:37:53.000000 browserist-1.6.9/src/browserist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-25 15:10:37.000000 browserist-1.6.9/src/browserist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      187 2024-04-08 23:37:53.000000 browserist-1.6.9/src/browserist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       11 2024-04-08 23:37:53.000000 browserist-1.6.9/src/browserist.egg-info/top_level.txt
```

### Comparing `browserist-1.6.8/LICENSE.md` & `browserist-1.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/PKG-INFO` & `browserist-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserist
-Version: 1.6.8
+Version: 1.6.9
 Summary: Extension for the Selenium web driver that makes browser automation even easier
 Home-page: https://jakob-bagterp.github.io/browserist/
 Download-URL: https://pypi.org/project/browserist/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
@@ -27,28 +27,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: chromedriver
-Requires-Dist: lxml==5.1.0
-Requires-Dist: pillow==10.2.0
+Requires-Dist: lxml==5.2.1
+Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: selenium==4.17.2
+Requires-Dist: selenium==4.19.0
 Provides-Extra: testing
-Requires-Dist: coverage==7.4.1; extra == "testing"
+Requires-Dist: coverage==7.4.4; extra == "testing"
 Requires-Dist: flake8==7.0.0; extra == "testing"
-Requires-Dist: keyring==24.3.0; extra == "testing"
-Requires-Dist: mypy==1.8.0; extra == "testing"
-Requires-Dist: pytest==8.0.0; extra == "testing"
-Requires-Dist: pytest-cov==4.1.0; extra == "testing"
-Requires-Dist: tox==4.12.1; extra == "testing"
+Requires-Dist: keyring==25.1.0; extra == "testing"
+Requires-Dist: mypy==1.9.0; extra == "testing"
+Requires-Dist: pytest==8.1.1; extra == "testing"
+Requires-Dist: pytest-cov==5.0.0; extra == "testing"
+Requires-Dist: tox==4.14.2; extra == "testing"
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.8&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.9&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 [![Python 3.10 | 3.11 | 3.12+](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
```

### Comparing `browserist-1.6.8/README.md` & `browserist-1.6.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.8&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.9&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 [![Python 3.10 | 3.11 | 3.12+](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
```

### Comparing `browserist-1.6.8/setup.cfg` & `browserist-1.6.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = browserist
-version = 1.6.8
+version = 1.6.9
 author = Jakob Bagterp
 author_email = jakob_bagterp@hotmail.com
 maintainer = Jakob Bagterp
 maintainer_email = jakob_bagterp@hotmail.com
 description = Extension for the Selenium web driver that makes browser automation even easier
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
@@ -35,36 +35,36 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 setup_requires = 
-	lxml==5.1.0
-	pillow==10.2.0
+	lxml==5.2.1
+	pillow==10.3.0
 	requests==2.31.0
-	selenium==4.17.2
+	selenium==4.19.0
 install_requires = 
 	chromedriver
-	lxml==5.1.0
-	pillow==10.2.0
+	lxml==5.2.1
+	pillow==10.3.0
 	requests==2.31.0
-	selenium==4.17.2
+	selenium==4.19.0
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage==7.4.1
+	coverage==7.4.4
 	flake8==7.0.0
-	keyring==24.3.0
-	mypy==1.8.0
-	pytest==8.0.0
-	pytest-cov==4.1.0
-	tox==4.12.1
+	keyring==25.1.0
+	mypy==1.9.0
+	pytest==8.1.1
+	pytest-cov==5.0.0
+	tox==4.14.2
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 browserist = py.typed
```

### Comparing `browserist-1.6.8/src/browserist/__init__.py` & `browserist-1.6.9/src/browserist/__init__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/__main__.py` & `browserist-1.6.9/src/browserist/browser/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/check_if/__main__.py` & `browserist-1.6.9/src/browserist/browser/check_if/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/check_if/contains_text.py` & `browserist-1.6.9/src/browserist/browser/check_if/contains_text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/check_if/is_in_viewport.py` & `browserist-1.6.9/src/browserist/browser/check_if/is_in_viewport.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/click/__main__.py` & `browserist-1.6.9/src/browserist/browser/click/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             expected_file_name (str | None, optional): Expected file name to determine when the download is complete. If `None`, this may be slower as Browserist will attempt to guess the file name by monitoring changes in the download directory.
             idle_download_timeout (float | None, optional): In seconds. Timeout to wait for file size to not increase, which is constantly renewed as long as the file size increases. If `None`, the global idle download timeout setting is used (default 3 seconds).
 
         Example:
             ```python title="" linenums="1"
             from browserist import Browser
 
-            with Browser(settings) as browser:
+            with Browser() as browser:
                 browser.open.url("https://example.com")
 
                 # Download file in background without waiting
                 # If the browser quits during a download, the download may be cancelled or left uncomplete
                 browser.click.download("//xpath/to/button")
 
                 # Download file and wait for download to complete
@@ -91,15 +91,15 @@
             Path: Path to the downloaded file. Return type is the standard library `pathlib.Path`.
 
         Example:
             ```python title="" linenums="1"
             from pathlib import Path
             from browserist import Browser
 
-            with Browser(settings) as browser:
+            with Browser() as browser:
                 browser.open.url("https://example.com")
                 file_path = browser.click.download_and_get_file_path("//xpath/to/button")
                 print("File name:", file_path.name)
                 # File name: file.zip
                 print("Absolute file path:", file_path.absolute())
                 # Absolute path: /home/user/downloads/file.zip
             ```
```

### Comparing `browserist-1.6.8/src/browserist/browser/click/button.py` & `browserist-1.6.9/src/browserist/browser/click/button.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/click/button_if_contains_text.py` & `browserist-1.6.9/src/browserist/browser/click/button_if_contains_text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/click/download.py` & `browserist-1.6.9/src/browserist/browser/click/download.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/click/download_and_get_file_path.py` & `browserist-1.6.9/src/browserist/browser/click/download_and_get_file_path.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/combo/__main__.py` & `browserist-1.6.9/src/browserist/browser/combo/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/combo/cookie_banner.py` & `browserist-1.6.9/src/browserist/browser/combo/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/combo/log_in.py` & `browserist-1.6.9/src/browserist/browser/combo/log_in.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/combo/search.py` & `browserist-1.6.9/src/browserist/browser/combo/search.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/__main__.py` & `browserist-1.6.9/src/browserist/browser/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/attribute/__main__.py` & `browserist-1.6.9/src/browserist/browser/get/attribute/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/attribute/values.py` & `browserist-1.6.9/src/browserist/browser/get/attribute/values.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/dimensions.py` & `browserist-1.6.9/src/browserist/browser/get/dimensions.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/element.py` & `browserist-1.6.9/src/browserist/browser/get/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/elements.py` & `browserist-1.6.9/src/browserist/browser/get/elements.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/text.py` & `browserist-1.6.9/src/browserist/browser/get/text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/url/__main__.py` & `browserist-1.6.9/src/browserist/browser/get/url/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/url/from_image.py` & `browserist-1.6.9/src/browserist/browser/get/url/from_image.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/get/url/from_link.py` & `browserist-1.6.9/src/browserist/browser/get/url/from_link.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/iframe/__main__.py` & `browserist-1.6.9/src/browserist/browser/iframe/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/iframe/switch_to.py` & `browserist-1.6.9/src/browserist/browser/iframe/switch_to.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/input/__main__.py` & `browserist-1.6.9/src/browserist/browser/input/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/input/value.py` & `browserist-1.6.9/src/browserist/browser/input/value.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/mouse/__main__.py` & `browserist-1.6.9/src/browserist/browser/mouse/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/mouse/hover.py` & `browserist-1.6.9/src/browserist/browser/mouse/hover.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/open/__main__.py` & `browserist-1.6.9/src/browserist/browser/open/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/open/url_if_not_current.py` & `browserist-1.6.9/src/browserist/browser/open/url_if_not_current.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/prompt/__main__.py` & `browserist-1.6.9/src/browserist/browser/prompt/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/prompt/proceed_yes_or_no.py` & `browserist-1.6.9/src/browserist/browser/prompt/proceed_yes_or_no.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/screenshot/__main__.py` & `browserist-1.6.9/src/browserist/browser/screenshot/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/screenshot/complete_page.py` & `browserist-1.6.9/src/browserist/browser/screenshot/complete_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/screenshot/element.py` & `browserist-1.6.9/src/browserist/browser/screenshot/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/screenshot/visible_portion.py` & `browserist-1.6.9/src/browserist/browser/screenshot/visible_portion.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/__main__.py` & `browserist-1.6.9/src/browserist/browser/scroll/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/check_if/__main__.py` & `browserist-1.6.9/src/browserist/browser/scroll/check_if/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/check_if/is_end_of_page.py` & `browserist-1.6.9/src/browserist/browser/scroll/check_if/is_end_of_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/get/__main__.py` & `browserist-1.6.9/src/browserist/browser/scroll/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/get/total_height.py` & `browserist-1.6.9/src/browserist/browser/scroll/get/total_height.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/into_view.py` & `browserist-1.6.9/src/browserist/browser/scroll/into_view.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/page/__main__.py` & `browserist-1.6.9/src/browserist/browser/scroll/page/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/scroll/page/to_end.py` & `browserist-1.6.9/src/browserist/browser/scroll/page/to_end.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/tool/__main__.py` & `browserist-1.6.9/src/browserist/browser/tool/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/viewport/__main__.py` & `browserist-1.6.9/src/browserist/browser/viewport/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/viewport/get/__main__.py` & `browserist-1.6.9/src/browserist/browser/viewport/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/viewport/set/__main__.py` & `browserist-1.6.9/src/browserist/browser/viewport/set/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/viewport/set/size.py` & `browserist-1.6.9/src/browserist/browser/viewport/set/size.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/__main__.py` & `browserist-1.6.9/src/browserist/browser/wait/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/for_element.py` & `browserist-1.6.9/src/browserist/browser/wait/for_element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/__main__.py` & `browserist-1.6.9/src/browserist/browser/wait/until/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/download_file/__main__.py` & `browserist-1.6.9/src/browserist/browser/wait/until/download_file/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/download_file/size_does_not_increase.py` & `browserist-1.6.9/src/browserist/browser/wait/until/download_file/size_does_not_increase.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/images_have_loaded.py` & `browserist-1.6.9/src/browserist/browser/wait/until/images_have_loaded.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/number_of_window_handles_is.py` & `browserist-1.6.9/src/browserist/browser/wait/until/number_of_window_handles_is.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/page_title/__main__.py` & `browserist-1.6.9/src/browserist/browser/wait/until/page_title/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/page_title/changes.py` & `browserist-1.6.9/src/browserist/browser/wait/until/page_title/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/page_title/contains.py` & `browserist-1.6.9/src/browserist/browser/wait/until/page_title/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/page_title/equals.py` & `browserist-1.6.9/src/browserist/browser/wait/until/page_title/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/text/__main__.py` & `browserist-1.6.9/src/browserist/browser/wait/until/text/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/text/changes.py` & `browserist-1.6.9/src/browserist/browser/wait/until/text/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/text/contains.py` & `browserist-1.6.9/src/browserist/browser/wait/until/text/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/text/equals.py` & `browserist-1.6.9/src/browserist/browser/wait/until/text/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/url/__main__.py` & `browserist-1.6.9/src/browserist/browser/wait/until/url/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/url/changes.py` & `browserist-1.6.9/src/browserist/browser/wait/until/url/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/url/contains.py` & `browserist-1.6.9/src/browserist/browser/wait/until/url/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/wait/until/url/equals.py` & `browserist-1.6.9/src/browserist/browser/wait/until/url/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/__main__.py` & `browserist-1.6.9/src/browserist/browser/window/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/get/__main__.py` & `browserist-1.6.9/src/browserist/browser/window/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/handle/__main__.py` & `browserist-1.6.9/src/browserist/browser/window/handle/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/open/__main__.py` & `browserist-1.6.9/src/browserist/browser/window/open/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/open/new_tab_or_window.py` & `browserist-1.6.9/src/browserist/browser/window/open/new_tab_or_window.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/set/__main__.py` & `browserist-1.6.9/src/browserist/browser/window/set/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/browser/window/switch_to.py` & `browserist-1.6.9/src/browserist/browser/window/switch_to.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/exception/download.py` & `browserist-1.6.9/src/browserist/exception/download.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/exception/element.py` & `browserist-1.6.9/src/browserist/exception/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/exception/headless.py` & `browserist-1.6.9/src/browserist/exception/headless.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/exception/timeout.py` & `browserist-1.6.9/src/browserist/exception/timeout.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/exception/window_handle.py` & `browserist-1.6.9/src/browserist/exception/window_handle.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/factory/chromium.py` & `browserist-1.6.9/src/browserist/factory/chromium.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/factory/get.py` & `browserist-1.6.9/src/browserist/factory/get.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/factory/internet_explorer.py` & `browserist-1.6.9/src/browserist/factory/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/factory/safari.py` & `browserist-1.6.9/src/browserist/factory/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/factory/set.py` & `browserist-1.6.9/src/browserist/factory/set.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper/directory.py` & `browserist-1.6.9/src/browserist/helper/directory.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper/file.py` & `browserist-1.6.9/src/browserist/helper/file.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper/image.py` & `browserist-1.6.9/src/browserist/helper/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from PIL import Image  # type: ignore
+from PIL import Image
+from PIL.Image import Image as ImageType
 from selenium.webdriver.remote.webdriver import BaseWebDriver
 from selenium.webdriver.remote.webelement import WebElement
 
 from ..model.type.path import FilePath
 
 
 def is_element_loaded(driver: BaseWebDriver, element: WebElement) -> bool:
@@ -10,31 +11,31 @@
 
     is_image_loaded: bool = driver.execute_script(  # type: ignore
         "return arguments[0].complete && typeof arguments[0].naturalWidth != 'undefined' && arguments[0].naturalWidth > 0;",
         element)
     return is_image_loaded or False
 
 
-def merge_vertically(image_base: Image, image_add: Image) -> Image:  # type: ignore
+def merge_vertically(image_base: ImageType, image_add: ImageType) -> ImageType:
     """Merge two images vertically. Assumes both images have the same width. "image_add" will be added below "image_base"."""
 
     merged_image_width: int = image_base.width
     merged_image_height: int = image_base.height + image_add.height
     merged_image = Image.new("RGB", (merged_image_width, merged_image_height))
     merged_image.paste(image_base, (0, 0))
     merged_image.paste(image_add, (0, image_base.height))
     # Rememeber to close images so we avoid PermissionError on especially Windows when trying to remove temporary files:
     image_base.close()
     image_add.close()
     return merged_image
 
 
-def open(file_path: str) -> Image:  # type: ignore
+def open(file_path: str) -> ImageType:
     """Open image from file path."""
 
     return Image.open(file_path)
 
 
-def save(image: Image, file_path: FilePath) -> Image:  # type: ignore
+def save(image: ImageType, file_path: FilePath) -> None:
     """Save image to file path."""
 
-    return image.save(file_path)
+    image.save(file_path)
```

### Comparing `browserist-1.6.8/src/browserist/helper/internet.py` & `browserist-1.6.9/src/browserist/helper/internet.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper/timeout.py` & `browserist-1.6.9/src/browserist/helper/timeout.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper/url.py` & `browserist-1.6.9/src/browserist/helper/url.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper/window_handle.py` & `browserist-1.6.9/src/browserist/helper/window_handle.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper_download/__init__.py` & `browserist-1.6.9/src/browserist/helper_download/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-__all__ = ["get_absolute_file_path"]
-
 import os
 from pathlib import Path
 
 from ..model.browser.base.driver import BrowserDriver
 from ..model.type.path import FilePath
```

### Comparing `browserist-1.6.8/src/browserist/helper_iteration/retry.py` & `browserist-1.6.9/src/browserist/helper_iteration/retry.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper_screenshot/__init__.py` & `browserist-1.6.9/src/browserist/helper_screenshot/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __all__ = ["complete_page", "controller", "file", "save", "save_element", "merge_two_images_without_save"]
 
 
-from PIL import Image  # type: ignore
+from PIL.Image import Image as ImageType
 from selenium.webdriver.remote.webelement import WebElement
 
 from .. import helper
 from ..model.browser.base.driver import BrowserDriver
 from . import complete_page, controller, file
 
 
@@ -18,9 +18,9 @@
 
 def save_element(element: WebElement, file_path: str) -> None:
     """Take screenshot of element. Reference: https://www.selenium.dev/documentation/webdriver/browser/windows/#takeelementscreenshot"""
 
     element.screenshot(file_path)
 
 
-def merge_two_images_without_save(image_1: Image, image_2: Image) -> Image:  # type: ignore
+def merge_two_images_without_save(image_1: ImageType, image_2: ImageType) -> ImageType:
     return helper.image.merge_vertically(image_1, image_2)
```

### Comparing `browserist-1.6.8/src/browserist/helper_screenshot/complete_page.py` & `browserist-1.6.9/src/browserist/helper_screenshot/complete_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper_screenshot/controller.py` & `browserist-1.6.9/src/browserist/helper_screenshot/controller.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/helper_screenshot/file.py` & `browserist-1.6.9/src/browserist/helper_screenshot/file.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/README.md` & `browserist-1.6.9/src/browserist/model/browser/README.md`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/base/driver.py` & `browserist-1.6.9/src/browserist/model/browser/base/driver.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/base/settings.py` & `browserist-1.6.9/src/browserist/model/browser/base/settings.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/base/timeout/settings.py` & `browserist-1.6.9/src/browserist/model/browser/base/timeout/settings.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/chrome.py` & `browserist-1.6.9/src/browserist/model/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/edge.py` & `browserist-1.6.9/src/browserist/model/browser/edge.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/extension/__main__.py` & `browserist-1.6.9/src/browserist/model/browser/extension/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/firefox.py` & `browserist-1.6.9/src/browserist/model/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/internet_explorer.py` & `browserist-1.6.9/src/browserist/model/browser/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/browser/safari.py` & `browserist-1.6.9/src/browserist/model/browser/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/combo_settings/cookie_banner.py` & `browserist-1.6.9/src/browserist/model/combo_settings/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/combo_settings/handling_state.py` & `browserist-1.6.9/src/browserist/model/combo_settings/handling_state.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/combo_settings/login_form.py` & `browserist-1.6.9/src/browserist/model/combo_settings/login_form.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/combo_settings/search.py` & `browserist-1.6.9/src/browserist/model/combo_settings/search.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/download/chrome.py` & `browserist-1.6.9/src/browserist/model/download/chrome.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/download/edge.py` & `browserist-1.6.9/src/browserist/model/download/edge.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/download/firefox.py` & `browserist-1.6.9/src/browserist/model/download/firefox.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/download/handler.py` & `browserist-1.6.9/src/browserist/model/download/handler.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/download/internet_explorer.py` & `browserist-1.6.9/src/browserist/model/download/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/download/safari.py` & `browserist-1.6.9/src/browserist/model/download/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/driver_methods.py` & `browserist-1.6.9/src/browserist/model/driver_methods.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/screenshot.py` & `browserist-1.6.9/src/browserist/model/screenshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 
-from PIL import Image  # type: ignore
+from PIL.Image import Image as ImageType
 
 from .. import helper, helper_screenshot
 from ..model.browser.base.driver import BrowserDriver
 from .type.file_png import FilePNG
 from .type.path import FilePath
 
 
@@ -30,15 +30,15 @@
 
     def __post_init__(self) -> None:
         self._destination_file_path: FilePath = helper_screenshot.file.get_path(self.file_name, self.destination_dir)
         self._temp_dir: FilePath = helper_screenshot.controller.mediate_temp_dir(self.destination_dir)
         self._all_temp_file_paths: list[FilePath] = []
         self._temp_file_prefix: str = helper_screenshot.file.get_temp_prefix_without_iterator_and_file_type()
         self._iteration: int = 1
-        self._screenshot: Image  # type: ignore
+        self._screenshot: ImageType
 
     def get_temp_file_name(self) -> FilePNG:
         return FilePNG(f"{self._temp_file_prefix}_{self._iteration}.png")
 
     def get_temp_file_path(self) -> FilePath:
         temp_file_name = self.get_temp_file_name()
         return helper_screenshot.file.get_path(temp_file_name, self._temp_dir)
```

### Comparing `browserist-1.6.8/src/browserist/model/type/callable.py` & `browserist-1.6.9/src/browserist/model/type/callable.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/type/file_png.py` & `browserist-1.6.9/src/browserist/model/type/file_png.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/type/path.py` & `browserist-1.6.9/src/browserist/model/type/path.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/type/url.py` & `browserist-1.6.9/src/browserist/model/type/url.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/type/xpath.py` & `browserist-1.6.9/src/browserist/model/type/xpath.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/apple.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/apple.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/google.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/google.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/huawei.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/huawei.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/microsoft.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/microsoft.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/oneplus.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/oneplus.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/oppo.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/oppo.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/samsung.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/samsung.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/vivo.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/vivo.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/collection/xiaomi.py` & `browserist-1.6.9/src/browserist/model/viewport/collection/xiaomi.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/viewport/common_devices.py` & `browserist-1.6.9/src/browserist/model/viewport/common_devices.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist/model/window/controller.py` & `browserist-1.6.9/src/browserist/model/window/controller.py`

 * *Files identical despite different names*

### Comparing `browserist-1.6.8/src/browserist.egg-info/PKG-INFO` & `browserist-1.6.9/src/browserist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserist
-Version: 1.6.8
+Version: 1.6.9
 Summary: Extension for the Selenium web driver that makes browser automation even easier
 Home-page: https://jakob-bagterp.github.io/browserist/
 Download-URL: https://pypi.org/project/browserist/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
@@ -27,28 +27,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: chromedriver
-Requires-Dist: lxml==5.1.0
-Requires-Dist: pillow==10.2.0
+Requires-Dist: lxml==5.2.1
+Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: selenium==4.17.2
+Requires-Dist: selenium==4.19.0
 Provides-Extra: testing
-Requires-Dist: coverage==7.4.1; extra == "testing"
+Requires-Dist: coverage==7.4.4; extra == "testing"
 Requires-Dist: flake8==7.0.0; extra == "testing"
-Requires-Dist: keyring==24.3.0; extra == "testing"
-Requires-Dist: mypy==1.8.0; extra == "testing"
-Requires-Dist: pytest==8.0.0; extra == "testing"
-Requires-Dist: pytest-cov==4.1.0; extra == "testing"
-Requires-Dist: tox==4.12.1; extra == "testing"
+Requires-Dist: keyring==25.1.0; extra == "testing"
+Requires-Dist: mypy==1.9.0; extra == "testing"
+Requires-Dist: pytest==8.1.1; extra == "testing"
+Requires-Dist: pytest-cov==5.0.0; extra == "testing"
+Requires-Dist: tox==4.14.2; extra == "testing"
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.8&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.9&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 [![Python 3.10 | 3.11 | 3.12+](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
```

### Comparing `browserist-1.6.8/src/browserist.egg-info/SOURCES.txt` & `browserist-1.6.9/src/browserist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

