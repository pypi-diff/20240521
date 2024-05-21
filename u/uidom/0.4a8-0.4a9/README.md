# Comparing `tmp/uidom-0.4a8.tar.gz` & `tmp/uidom-0.4a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uidom-0.4a8.tar", max compression
+gzip compressed data, was "uidom-0.4a9.tar", max compression
```

## Comparing `uidom-0.4a8.tar` & `uidom-0.4a9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1062 2023-10-03 09:38:59.997740 uidom-0.4a8/LICENSE
--rw-r--r--   0        0        0     5845 2023-10-03 09:38:59.997740 uidom-0.4a8/README.md
--rw-r--r--   0        0        0     1277 2023-10-11 19:46:05.093662 uidom-0.4a8/pyproject.toml
--rw-r--r--   0        0        0      218 2023-10-11 19:45:48.474821 uidom-0.4a8/uidom/__init__.py
--rw-r--r--   0        0        0      142 2023-10-03 09:39:00.009740 uidom-0.4a8/uidom/alpinejs/__init__.py
--rw-r--r--   0        0        0     9154 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/alpinejs/dataset.py
--rw-r--r--   0        0        0     1224 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/alpinejs/ripple_btn.py
--rw-r--r--   0        0        0     1067 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/cli/__init__.py
--rw-r--r--   0        0        0    12108 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/cli/_cli.py
--rw-r--r--   0        0        0    10362 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/cli/cli.py
--rw-r--r--   0        0        0      729 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/dom/__init__.py
--rw-r--r--   0        0        0     6059 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/dom/htmldocument.py
--rw-r--r--   0        0        0     6179 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/dom/htmlelement.py
--rw-r--r--   0        0        0    42988 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/dom/icons.py
--rw-r--r--   0        0        0     1363 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/dom/jinja.py
--rwxr-xr-x   0        0        0      350 2023-10-03 09:39:00.013740 uidom-0.4a8/uidom/dom/src/__init__.py
--rw-r--r--   0        0        0    20976 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/component.py
--rw-r--r--   0        0        0     3607 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/csstags.py
--rw-r--r--   0        0        0     3926 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/dom1core.py
--rw-r--r--   0        0        0    18412 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/dom_tag.py
--rw-r--r--   0        0        0    31873 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/ext.py
--rw-r--r--   0        0        0     7544 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/html_string.py
--rw-r--r--   0        0        0    31434 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/htmltags.py
--rw-r--r--   0        0        0     5072 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/jinjatags.py
--rw-r--r--   0        0        0      164 2023-10-03 09:39:00.017740 uidom-0.4a8/uidom/dom/src/main.py
--rw-r--r--   0        0        0    13731 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/parse_html.py
--rw-r--r--   0        0        0     2836 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/pythontags.py
--rw-r--r--   0        0        0     1729 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/sphinxtags.py
--rw-r--r--   0        0        0    10753 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/svgtags.py
--rw-r--r--   0        0        0      144 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/utils/__init__.py
--rw-r--r--   0        0        0     4481 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/utils/dom_util.py
--rw-r--r--   0        0        0     5091 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/utils/sheets.py
--rw-r--r--   0        0        0     6623 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/src/ws_rpc.py
--rw-r--r--   0        0        0    16753 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/ui.py
--rw-r--r--   0        0        0     3921 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/dom/uniqueid.py
--rw-r--r--   0        0        0      121 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/edge_db/__init__.py
--rw-r--r--   0        0        0     9912 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/edge_db/ql.py
--rw-r--r--   0        0        0      277 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/elements/__init__.py
--rw-r--r--   0        0        0     5996 2023-10-10 14:35:54.655928 uidom-0.4a8/uidom/elements/booleans.py
--rw-r--r--   0        0        0     6617 2023-10-10 16:29:40.123626 uidom-0.4a8/uidom/elements/buttons.py
--rw-r--r--   0        0        0    12880 2023-10-10 13:23:04.259466 uidom-0.4a8/uidom/elements/chars.py
--rw-r--r--   0        0        0     1830 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/elements/dates.py
--rw-r--r--   0        0        0     1947 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/elements/enums.py
--rw-r--r--   0        0        0     5497 2023-10-11 03:56:00.915289 uidom-0.4a8/uidom/elements/floats.py
--rw-r--r--   0        0        0     9891 2023-10-10 17:27:17.723558 uidom-0.4a8/uidom/elements/integers.py
--rw-r--r--   0        0        0      908 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/examples/links.py
--rw-r--r--   0        0        0     2685 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/examples/toggle.py
--rw-r--r--   0        0        0     1915 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/htmx/__init__.py
--rw-r--r--   0        0        0     2153 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/htmx/middleware.py
--rw-r--r--   0        0        0      157 2023-10-03 09:39:00.021740 uidom-0.4a8/uidom/reloader/__init__.py
--rw-r--r--   0        0        0     3945 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/reloader/_app.py
--rw-r--r--   0        0        0      158 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/reloader/_models.py
--rw-r--r--   0        0        0     1320 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/reloader/_notify.py
--rw-r--r--   0        0        0       83 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/reloader/_types.py
--rw-r--r--   0        0        0     2031 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/reloader/_watch.py
--rw-r--r--   0        0        0     2027 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/reloader/script/reloader.js
--rw-r--r--   0        0        0      118 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/response/__init__.py
--rw-r--r--   0        0        0     3264 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/response/starlette.py
--rw-r--r--   0        0        0      118 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/routing/__init__.py
--rw-r--r--   0        0        0    19108 2023-10-10 10:08:59.228611 uidom-0.4a8/uidom/routing/fastapi.py
--rw-r--r--   0        0        0      723 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/scripts/__init__.py
--rw-r--r--   0        0        0    12124 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/scripts/xcomponent.js
--rw-r--r--   0        0        0      197 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/settings/__init__.py
--rw-r--r--   0        0        0     9472 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/settings/commands.py
--rw-r--r--   0        0        0     8599 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/settings/document.py
--rw-r--r--   0        0        0     4201 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/settings/paths.py
--rw-r--r--   0        0        0      255 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/slots/__init__.py
--rw-r--r--   0        0        0     1968 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/slots/custom_element_slot.py
--rw-r--r--   0        0        0     1597 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/slots/slots.py
--rw-r--r--   0        0        0     1594 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/slots/web_component_slot.py
--rw-r--r--   0        0        0      118 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/utils/__init__.py
--rwxr-xr-x   0        0        0     5295 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/utils/functional.py
--rw-r--r--   0        0        0     1320 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/utils/logger.py
--rw-r--r--   0        0        0     6458 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/utils/parameters.py
--rw-r--r--   0        0        0      337 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/web_io/__init__.py
--rw-r--r--   0        0        0    12444 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/web_io/_adapter.py
--rw-r--r--   0        0        0     7496 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/web_io/_events.py
--rw-r--r--   0        0        0     1467 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/web_io/_protocol.py
--rw-r--r--   0        0        0      353 2023-10-03 09:39:00.025740 uidom-0.4a8/uidom/web_io/_types.py
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 uidom-0.4a8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-10-03 09:38:59.997740 uidom-0.4a9/LICENSE
+-rw-r--r--   0        0        0     5845 2023-10-03 09:38:59.997740 uidom-0.4a9/README.md
+-rw-r--r--   0        0        0     1277 2023-12-11 00:26:47.872701 uidom-0.4a9/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-12-11 00:23:39.596954 uidom-0.4a9/uidom/__init__.py
+-rw-r--r--   0        0        0      142 2023-10-03 09:39:00.009740 uidom-0.4a9/uidom/alpinejs/__init__.py
+-rw-r--r--   0        0        0     9154 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/alpinejs/dataset.py
+-rw-r--r--   0        0        0     1224 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/alpinejs/ripple_btn.py
+-rw-r--r--   0        0        0     1067 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/cli/__init__.py
+-rw-r--r--   0        0        0    12108 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/cli/_cli.py
+-rw-r--r--   0        0        0    10362 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/cli/cli.py
+-rw-r--r--   0        0        0      729 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/dom/__init__.py
+-rw-r--r--   0        0        0     6059 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/dom/htmldocument.py
+-rw-r--r--   0        0        0     6179 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/dom/htmlelement.py
+-rw-r--r--   0        0        0    42988 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/dom/icons.py
+-rw-r--r--   0        0        0     1363 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/dom/jinja.py
+-rwxr-xr-x   0        0        0      350 2023-10-03 09:39:00.013740 uidom-0.4a9/uidom/dom/src/__init__.py
+-rw-r--r--   0        0        0    20976 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/component.py
+-rw-r--r--   0        0        0     3607 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/csstags.py
+-rw-r--r--   0        0        0     3926 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/dom1core.py
+-rw-r--r--   0        0        0    18412 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/dom_tag.py
+-rw-r--r--   0        0        0    31873 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/ext.py
+-rw-r--r--   0        0        0     7544 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/html_string.py
+-rw-r--r--   0        0        0    31434 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/htmltags.py
+-rw-r--r--   0        0        0     5072 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/jinjatags.py
+-rw-r--r--   0        0        0      164 2023-10-03 09:39:00.017740 uidom-0.4a9/uidom/dom/src/main.py
+-rw-r--r--   0        0        0    13731 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/parse_html.py
+-rw-r--r--   0        0        0     2836 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/pythontags.py
+-rw-r--r--   0        0        0     1729 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/sphinxtags.py
+-rw-r--r--   0        0        0    10753 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/svgtags.py
+-rw-r--r--   0        0        0      144 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/utils/__init__.py
+-rw-r--r--   0        0        0     4481 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/utils/dom_util.py
+-rw-r--r--   0        0        0     5091 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/utils/sheets.py
+-rw-r--r--   0        0        0     6623 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/src/ws_rpc.py
+-rw-r--r--   0        0        0    16753 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/ui.py
+-rw-r--r--   0        0        0     3921 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/dom/uniqueid.py
+-rw-r--r--   0        0        0      121 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/edge_db/__init__.py
+-rw-r--r--   0        0        0     9912 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/edge_db/ql.py
+-rw-r--r--   0        0        0      277 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/elements/__init__.py
+-rw-r--r--   0        0        0     5996 2023-10-10 14:35:54.655928 uidom-0.4a9/uidom/elements/booleans.py
+-rw-r--r--   0        0        0     6617 2023-10-10 16:29:40.123626 uidom-0.4a9/uidom/elements/buttons.py
+-rw-r--r--   0        0        0    12880 2023-10-10 13:23:04.259466 uidom-0.4a9/uidom/elements/chars.py
+-rw-r--r--   0        0        0     1830 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/elements/dates.py
+-rw-r--r--   0        0        0     1947 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/elements/enums.py
+-rw-r--r--   0        0        0     5497 2023-10-11 03:56:00.915289 uidom-0.4a9/uidom/elements/floats.py
+-rw-r--r--   0        0        0     9891 2023-10-10 17:27:17.723558 uidom-0.4a9/uidom/elements/integers.py
+-rw-r--r--   0        0        0      908 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/examples/links.py
+-rw-r--r--   0        0        0     2685 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/examples/toggle.py
+-rw-r--r--   0        0        0     1915 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/htmx/__init__.py
+-rw-r--r--   0        0        0     2153 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/htmx/middleware.py
+-rw-r--r--   0        0        0      157 2023-10-03 09:39:00.021740 uidom-0.4a9/uidom/reloader/__init__.py
+-rw-r--r--   0        0        0     3945 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/reloader/_app.py
+-rw-r--r--   0        0        0      158 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/reloader/_models.py
+-rw-r--r--   0        0        0     1320 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/reloader/_notify.py
+-rw-r--r--   0        0        0       83 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/reloader/_types.py
+-rw-r--r--   0        0        0     2031 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/reloader/_watch.py
+-rw-r--r--   0        0        0     2027 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/reloader/script/reloader.js
+-rw-r--r--   0        0        0      118 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/response/__init__.py
+-rw-r--r--   0        0        0     3308 2023-12-10 22:33:09.334228 uidom-0.4a9/uidom/response/starlette.py
+-rw-r--r--   0        0        0      118 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/routing/__init__.py
+-rw-r--r--   0        0        0    20518 2023-12-11 00:26:43.536800 uidom-0.4a9/uidom/routing/fastapi.py
+-rw-r--r--   0        0        0      723 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/scripts/__init__.py
+-rw-r--r--   0        0        0    12175 2023-12-11 00:11:31.013401 uidom-0.4a9/uidom/scripts/xcomponent.js
+-rw-r--r--   0        0        0      197 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/settings/__init__.py
+-rw-r--r--   0        0        0     9472 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/settings/commands.py
+-rw-r--r--   0        0        0     8599 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/settings/document.py
+-rw-r--r--   0        0        0     4201 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/settings/paths.py
+-rw-r--r--   0        0        0      255 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/slots/__init__.py
+-rw-r--r--   0        0        0     1968 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/slots/custom_element_slot.py
+-rw-r--r--   0        0        0     1597 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/slots/slots.py
+-rw-r--r--   0        0        0     1594 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/slots/web_component_slot.py
+-rw-r--r--   0        0        0      118 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/utils/__init__.py
+-rwxr-xr-x   0        0        0     5295 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/utils/functional.py
+-rw-r--r--   0        0        0     1320 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/utils/logger.py
+-rw-r--r--   0        0        0     6458 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/utils/parameters.py
+-rw-r--r--   0        0        0      337 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/web_io/__init__.py
+-rw-r--r--   0        0        0    12444 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/web_io/_adapter.py
+-rw-r--r--   0        0        0     7496 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/web_io/_events.py
+-rw-r--r--   0        0        0     1467 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/web_io/_protocol.py
+-rw-r--r--   0        0        0      353 2023-10-03 09:39:00.025740 uidom-0.4a9/uidom/web_io/_types.py
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 uidom-0.4a9/PKG-INFO
```

### Comparing `uidom-0.4a8/LICENSE` & `uidom-0.4a9/LICENSE`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/README.md` & `uidom-0.4a9/README.md`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/pyproject.toml` & `uidom-0.4a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uidom"
-version = "0.4a8"
+version = "0.4a9"
 description = "HTML library"
 authors = ["bitplorer <bitplorer@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uidom-0.4a8/uidom/alpinejs/dataset.py` & `uidom-0.4a9/uidom/alpinejs/dataset.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/alpinejs/ripple_btn.py` & `uidom-0.4a9/uidom/alpinejs/ripple_btn.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/cli/__init__.py` & `uidom-0.4a9/uidom/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/cli/_cli.py` & `uidom-0.4a9/uidom/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/cli/cli.py` & `uidom-0.4a9/uidom/cli/cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/__init__.py` & `uidom-0.4a9/uidom/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/htmldocument.py` & `uidom-0.4a9/uidom/dom/htmldocument.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/htmlelement.py` & `uidom-0.4a9/uidom/dom/htmlelement.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/icons.py` & `uidom-0.4a9/uidom/dom/icons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/jinja.py` & `uidom-0.4a9/uidom/dom/jinja.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/component.py` & `uidom-0.4a9/uidom/dom/src/component.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/csstags.py` & `uidom-0.4a9/uidom/dom/src/csstags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/dom1core.py` & `uidom-0.4a9/uidom/dom/src/dom1core.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/dom_tag.py` & `uidom-0.4a9/uidom/dom/src/dom_tag.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/ext.py` & `uidom-0.4a9/uidom/dom/src/ext.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/html_string.py` & `uidom-0.4a9/uidom/dom/src/html_string.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/htmltags.py` & `uidom-0.4a9/uidom/dom/src/htmltags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/jinjatags.py` & `uidom-0.4a9/uidom/dom/src/jinjatags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/parse_html.py` & `uidom-0.4a9/uidom/dom/src/parse_html.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/pythontags.py` & `uidom-0.4a9/uidom/dom/src/pythontags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/sphinxtags.py` & `uidom-0.4a9/uidom/dom/src/sphinxtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/svgtags.py` & `uidom-0.4a9/uidom/dom/src/svgtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/utils/dom_util.py` & `uidom-0.4a9/uidom/dom/src/utils/dom_util.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/utils/sheets.py` & `uidom-0.4a9/uidom/dom/src/utils/sheets.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/src/ws_rpc.py` & `uidom-0.4a9/uidom/dom/src/ws_rpc.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/ui.py` & `uidom-0.4a9/uidom/dom/ui.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/dom/uniqueid.py` & `uidom-0.4a9/uidom/dom/uniqueid.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/edge_db/ql.py` & `uidom-0.4a9/uidom/edge_db/ql.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/booleans.py` & `uidom-0.4a9/uidom/elements/booleans.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/buttons.py` & `uidom-0.4a9/uidom/elements/buttons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/chars.py` & `uidom-0.4a9/uidom/elements/chars.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/dates.py` & `uidom-0.4a9/uidom/elements/dates.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/enums.py` & `uidom-0.4a9/uidom/elements/enums.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/floats.py` & `uidom-0.4a9/uidom/elements/floats.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/elements/integers.py` & `uidom-0.4a9/uidom/elements/integers.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/examples/links.py` & `uidom-0.4a9/uidom/examples/links.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/examples/toggle.py` & `uidom-0.4a9/uidom/examples/toggle.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/htmx/__init__.py` & `uidom-0.4a9/uidom/htmx/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/htmx/middleware.py` & `uidom-0.4a9/uidom/htmx/middleware.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/reloader/_app.py` & `uidom-0.4a9/uidom/reloader/_app.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/reloader/_notify.py` & `uidom-0.4a9/uidom/reloader/_notify.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/reloader/_watch.py` & `uidom-0.4a9/uidom/reloader/_watch.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/reloader/script/reloader.js` & `uidom-0.4a9/uidom/reloader/script/reloader.js`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/response/starlette.py` & `uidom-0.4a9/uidom/response/starlette.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from starlette.background import BackgroundTask
 from starlette.responses import HTMLResponse as StarletteHTMLResponse
 from starlette.responses import StreamingResponse as StarletteStreamingResponse
 
 from uidom.dom.src import ext
 
-__all__ = ["HTMLResponse", "html_response", "StreamingResponse", "async_html_response"]
+__all__ = ["HTMLResponse", "html_response", "StreamingResponse", "streaming_response"]
 
 CallableType = T.TypeVar("CallableType", bound=T.Callable[..., T.Any])
 
 
 class HTMLResponse(StarletteHTMLResponse):
     media_type = "text/html"
 
@@ -26,15 +26,14 @@
         self,
         html_content: ext.Tags,
         status_code: int = 200,
         headers: dict = None,
         media_type: str = None,
         background: BackgroundTask = None,
     ) -> None:
-        
         super().__init__(html_content, status_code, headers, media_type, background)
 
     def render(self, content: T.Any) -> bytes:
         if hasattr(content, "__render__"):
             content = content.__render__()
         return super().render(content=content)
 
@@ -47,14 +46,15 @@
 
             @wraps(endpoint)
             async def decorated(*args, **kwargs) -> HTMLResponse:
                 content = await endpoint(*args, **kwargs)
                 if isinstance(content, ext.Tags):
                     return HTMLResponse(content)
                 return content
+
         else:
 
             @wraps(endpoint)
             def decorated(*args, **kwargs) -> HTMLResponse:
                 content = endpoint(*args, **kwargs)
                 if isinstance(content, ext.Tags):
                     return HTMLResponse(content)
@@ -72,36 +72,41 @@
         self,
         html_content: ext.Tags,
         status_code: int = 200,
         headers: dict = None,
         media_type: str = None,
         background: BackgroundTask = None,
     ) -> None:
-        
-        super().__init__(html_content.__async_render__(), status_code, headers, media_type, background)
-        
+        super().__init__(
+            html_content.__async_render__(),
+            status_code,
+            headers,
+            media_type,
+            background,
+        )
+
 
-def async_html_response(
+def streaming_response(
     endpoint: T.Optional[CallableType] = None,
 ) -> T.Callable[..., StreamingResponse]:
     def decorate_sync_async(endpoint):
         if iscoroutinefunction(endpoint):
 
             @wraps(endpoint)
             async def decorated(*args, **kwargs) -> StreamingResponse:
                 content = await endpoint(*args, **kwargs)
                 if isinstance(content, ext.Tags):
                     return StreamingResponse(content)
                 return content
+
         else:
 
             @wraps(endpoint)
             def decorated(*args, **kwargs) -> StreamingResponse:
                 content = endpoint(*args, **kwargs)
                 if isinstance(content, ext.Tags):
                     return StreamingResponse(content)
                 return content
 
         return decorated
 
     return decorate_sync_async(endpoint)
-
```

### Comparing `uidom-0.4a8/uidom/routing/fastapi.py` & `uidom-0.4a9/uidom/routing/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from starlette.responses import JSONResponse, Response
 from starlette.routing import BaseRoute
 from starlette.types import ASGIApp, Lifespan
 
 from uidom.response.starlette import (
     HTMLResponse,
     StreamingResponse,
-    async_html_response,
     html_response,
+    streaming_response,
 )
 
 
 class HTMLRoute(routing.APIRoute):
     def __init__(
         self,
         path: str,
@@ -129,15 +129,15 @@
         openapi_extra: Optional[Dict[str, Any]] = None,
         generate_unique_id_function: Union[
             Callable[["routing.APIRoute"], str], DefaultPlaceholder
         ] = Default(generate_unique_id),
     ) -> None:
         super().__init__(
             path=path,
-            endpoint=async_html_response(endpoint),
+            endpoint=streaming_response(endpoint),
             response_model=response_model,
             status_code=status_code,
             tags=tags,
             dependencies=dependencies,
             summary=summary,
             description=description,
             response_description=response_description,
@@ -261,17 +261,30 @@
             # example: package/app/module/ -> package.app.module
             module = file_package_path.replace("/", ".") + "." + file.stem
             # Import route file
             route_file = importlib.import_module(module)
 
             # Find routes
             if file.stem == self.route_file_name:
-                route_methods = [
-                    r for r in dir(route_file) if r.lower() in self._METHODS
-                ]
+                # first we will search the declared functions in __all__
+                # if we don't find any we will proceed to scan CRUD methods
+                # like in self._METHODS and add them to routes
+                # for example:
+                #
+                # app/login/route.py
+                #
+                # def get():...
+                #
+                # def post():...
+                #
+                route_methods = getattr(
+                    route_file,
+                    "__all__",
+                    [r for r in dir(route_file) if r.lower() in self._METHODS],
+                )
             else:
                 # if the file name is NOT "route.py" and we want to include method from that
                 # file in router, we can scan __all__ variable in directory for pyobjects
                 # that declare route methods, for example
                 #
                 # shoppers.py
                 #
@@ -280,45 +293,54 @@
                 #   class Shoppers(Component):
                 #       routes = ["get", "post", "cart", etc...]
                 #
                 #       def get(self, ...):...
                 #
                 route_methods = defaultdict(dict)
 
-                for klass_name in getattr(route_file, "__all__", []):
+                for klass_name in getattr(
+                    route_file,
+                    "__all__",
+                    [r for r in dir(route_file) if r.lower() in self._METHODS],
+                ):
                     klass = getattr(route_file, klass_name)
-                    for mthd in getattr(klass, "routes", []):
-                        route_methods[klass_name.lower()][mthd] = getattr(klass, mthd)
+                    if getattr(klass, "routes", []):
+                        for mthd in getattr(klass, "routes"):
+                            route_methods[klass_name.lower()][mthd] = getattr(
+                                klass, mthd
+                            )
+                    else:
+                        route_methods["_DIRECT_ROUTES"][klass_name] = klass
 
             if route_methods:
                 # braces_or_brackets = self._find_braces_or_brackets(
                 #     relative_path_to_file_module
                 # )
                 # TODO: make a {items}, tags parsed well in advance
                 # tag_string = ""
                 # for str_to_remove in braces_or_brackets:
                 #     tag_string = relative_path_to_file_module.replace(
                 #         "/" + str_to_remove, ""
                 #     )
 
-                # Making "app" prefix as default
-                if relative_file_folder.startswith("app"):
+                # Making "base_directory" prefix as default
+                if relative_file_folder.startswith(self.base_directory):
                     tags = ["default"]
                 else:
                     tags = relative_file_folder.split("/")
 
-                if relative_file_folder.startswith("app"):
-                    # remove "app" prefix from path as "app" is default
-                    # folder.
-                    rel_path_without_app_prefix = relative_file_folder.replace(
-                        "app", ""
+                if relative_file_folder.startswith(self.base_directory):
+                    # remove base_directory prefix from path as "base_directory"
+                    # is default folder.
+                    rel_path_without_base_directory_prefix = (
+                        relative_file_folder.replace(self.base_directory, "")
                     )
                     prefix = (
-                        rel_path_without_app_prefix
-                        if rel_path_without_app_prefix
+                        rel_path_without_base_directory_prefix
+                        if rel_path_without_base_directory_prefix
                         else ""
                     )
                 else:
                     prefix = "/" + relative_file_folder
 
                 if prefix:
                     # remove private folders starting with "_" i.e. underscore
@@ -342,36 +364,46 @@
 
                 if isinstance(route_methods, list):
                     # these are methods inside normal route.py files
                     for method in route_methods:
                         _method_attr = getattr(route_file, method)
                         name = f"{module}:{_method}"
                         _method_attr.__dict__["name"] = name
-                        _router.add_api_route(
-                            "/",
-                            _method_attr,
-                            name=_method_attr.name,
-                            methods=[method.lower()],
-                            description=_method_attr.__doc__,
-                        )
+                        if method in self._METHODS:
+                            _router.add_api_route(
+                                "/",
+                                _method_attr,
+                                name=_method_attr.name,
+                                methods=[method.lower()],
+                                description=_method_attr.__doc__,
+                            )
+                        else:
+                            _router.add_api_route(
+                                method.lower(),
+                                _method_attr,
+                                name=_method_attr.name,
+                                methods=["get"],
+                                description=_method_attr.__doc__,
+                            )
+
                 else:
                     # these are methods inside non route.py files
                     # with __all__ variable declared, important thing to
                     # note is that all methods inside class MUST BE
                     # classmethod or staticmethod
                     for klass_name in route_methods:
                         for _method in route_methods[klass_name]:
                             _method_attr = route_methods[klass_name][_method]
                             # here we set .name attribute to method because we want
                             # htmx to use the route via hx_get=url_for(klass.method.name)
                             name = f"{module}.{klass_name}:{_method}"
                             _method_attr.__dict__["name"] = name
 
                             if _method.lower() in self._METHODS:
-                                # case for [get, post, path, delete, etc] CRUD methods
+                                # case for [get, post, patch, delete, etc] CRUD methods
                                 _router.tags.extend([file.stem, klass_name])
                                 if not file.stem.startswith("_"):
                                     _route_ = (
                                         f"/{file.stem}/{klass_name}"
                                         if not klass_name.startswith("_")
                                         else f"/{file.stem}"
                                     )
```

### Comparing `uidom-0.4a8/uidom/scripts/__init__.py` & `uidom-0.4a9/uidom/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/scripts/xcomponent.js` & `uidom-0.4a9/uidom/scripts/xcomponent.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -214,15 +214,15 @@
                 this.ws = document.setUpOrGetWebSocket(this.id, messageHandler, this._dataState.get('ws'));
                 this.waitForConnection = document.waitForConnection[`${this._dataState.get('ws')}`]
             }
 
 
             this.observer = observeAttrChange(this, (attr, oldVal, newVal) => {
                 // slice :attr to remove leading '_' (underscore) to check in this._dataState
-                console.log('from observer', attr, oldVal, newVal);
+                // console.log('from observer',attr, oldVal, newVal);
                 //console.log(attr, this._dataState.get(attr.replace('_data_', '')));
                 if (this._dataState.get(attr.replace('_data_', ''))) {
                     this.attributeChangedCallback(attr.replace('_data_', ''), oldVal, newVal);
                 }
             });
 
             //setTimeout(() => {this.ws.send(JSON.stringify(this.data()));}, 300);
@@ -258,16 +258,18 @@
             }
         }
 
         disconnectedCallback() {
             //super.disconnectedCallback();
             this.observer.disconnect();
             this.observer = null;
-            this.ws.close();
-            this.ws = null;
+            if (this.ws) {
+                this.ws.close();
+                this.ws = null;
+            }
         }
 
         send(data, retries = 4) {
             try {
                 this.ws.send(data);
                 return data;
             } catch (error) {
```

### Comparing `uidom-0.4a8/uidom/settings/commands.py` & `uidom-0.4a9/uidom/settings/commands.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/settings/document.py` & `uidom-0.4a9/uidom/settings/document.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/settings/paths.py` & `uidom-0.4a9/uidom/settings/paths.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/slots/custom_element_slot.py` & `uidom-0.4a9/uidom/slots/custom_element_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/slots/slots.py` & `uidom-0.4a9/uidom/slots/slots.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/slots/web_component_slot.py` & `uidom-0.4a9/uidom/slots/web_component_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/utils/functional.py` & `uidom-0.4a9/uidom/utils/functional.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/utils/logger.py` & `uidom-0.4a9/uidom/utils/logger.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/utils/parameters.py` & `uidom-0.4a9/uidom/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/web_io/_adapter.py` & `uidom-0.4a9/uidom/web_io/_adapter.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/web_io/_events.py` & `uidom-0.4a9/uidom/web_io/_events.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/uidom/web_io/_protocol.py` & `uidom-0.4a9/uidom/web_io/_protocol.py`

 * *Files identical despite different names*

### Comparing `uidom-0.4a8/PKG-INFO` & `uidom-0.4a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uidom
-Version: 0.4a8
+Version: 0.4a9
 Summary: HTML library
 License: MIT
 Author: bitplorer
 Author-email: bitplorer@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

