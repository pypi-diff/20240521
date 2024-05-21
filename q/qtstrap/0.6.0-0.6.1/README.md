# Comparing `tmp/qtstrap-0.6.0.tar.gz` & `tmp/qtstrap-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtstrap-0.6.0.tar", last modified: Tue May 21 21:34:34 2024, max compression
+gzip compressed data, was "qtstrap-0.6.1.tar", last modified: Tue May 21 21:45:43 2024, max compression
```

## Comparing `qtstrap-0.6.0.tar` & `qtstrap-0.6.1.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.738673 qtstrap-0.6.0/
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:31.563301 qtstrap-0.6.0/.github/
--rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.6.0/.github/FUNDING.yml
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:31.603155 qtstrap-0.6.0/.github/workflows/
--rw-rw-rw-   0        0        0     1026 2024-05-08 19:00:02.000000 qtstrap-0.6.0/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      173 2024-04-03 18:10:27.000000 qtstrap-0.6.0/.gitignore
--rw-rw-rw-   0        0        0     1159 2023-09-14 23:58:51.000000 qtstrap-0.6.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      132 2023-09-01 03:46:41.000000 qtstrap-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3048 2024-05-21 21:28:07.000000 qtstrap-0.6.0/Makefile
--rw-rw-rw-   0        0        0     4070 2024-05-21 21:34:34.736673 qtstrap-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2024-05-08 19:00:02.000000 qtstrap-0.6.0/README.md
--rw-rw-rw-   0        0        0      340 2024-05-08 19:00:02.000000 qtstrap-0.6.0/build_docs.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:31.721212 qtstrap-0.6.0/docs/
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:33.441359 qtstrap-0.6.0/docs/api/
--rw-rw-rw-   0        0        0       68 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/.pages
--rw-rw-rw-   0        0        0      395 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/experimental.md
--rw-rw-rw-   0        0        0     5155 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.code_editor.md
--rw-rw-rw-   0        0        0     1469 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.code_line.md
--rw-rw-rw-   0        0        0      489 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.highlighters.md
--rw-rw-rw-   0        0        0     3309 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.highlighters.python.md
--rw-rw-rw-   0        0        0      505 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.md
--rw-rw-rw-   0        0        0     9538 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.command_palette.command_palette.md
--rw-rw-rw-   0        0        0      480 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.command_palette.md
--rw-rw-rw-   0        0        0     2636 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_database_handler.md
--rw-rw-rw-   0        0        0    15224 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_filter_controls.md
--rw-rw-rw-   0        0        0     4096 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_profile.md
--rw-rw-rw-   0        0        0     4743 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_table_view.md
--rw-rw-rw-   0        0        0     5173 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_widget.md
--rw-rw-rw-   0        0        0      969 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.md
--rw-rw-rw-   0        0        0      383 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.md
--rw-rw-rw-   0        0        0      925 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.colors.md
--rw-rw-rw-   0        0        0      854 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.dark_palette.md
--rw-rw-rw-   0        0        0      471 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.md
--rw-rw-rw-   0        0        0     1423 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.themes.md
--rw-rw-rw-   0        0        0      387 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/optional.md
--rw-rw-rw-   0        0        0      628 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/options.md
--rw-rw-rw-   0        0        0    11611 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/overview.md
--rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.6.0/docs/api/settings.md
--rw-rw-rw-   0        0        0     1513 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.adapter.md
--rw-rw-rw-   0        0        0      750 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.call_later.md
--rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.6.0/docs/api/utils.decorators.md
--rw-rw-rw-   0        0        0     1142 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.defer.md
--rw-rw-rw-   0        0        0     1846 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.drag_and_drop.md
--rw-rw-rw-   0        0        0      824 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.get_ip.md
--rw-rw-rw-   0        0        0      500 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.md
--rw-rw-rw-   0        0        0     1069 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.signals.md
--rw-rw-rw-   0        0        0      821 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.singleton.md
--rw-rw-rw-   0        0        0     1713 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.string_builder.md
--rw-rw-rw-   0        0        0     2145 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.timestamp.md
--rw-rw-rw-   0        0        0     1220 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.trace.md
--rw-rw-rw-   0        0        0     2801 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.utils.md
--rw-rw-rw-   0        0        0     5686 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.buttons.md
--rw-rw-rw-   0        0        0     3263 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.labeledit.md
--rw-rw-rw-   0        0        0    30518 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.layouts.md
--rw-rw-rw-   0        0        0     1669 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.line_widgets.md
--rw-rw-rw-   0        0        0     2010 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.link_label.md
--rw-rw-rw-   0        0        0      596 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.md
--rw-rw-rw-   0        0        0     3450 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     8961 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     8844 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.toggle.md
--rw-rw-rw-   0        0        0     1440 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.toolbar.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:33.530889 qtstrap-0.6.0/docs/extras/
--rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.6.0/docs/extras/code_editor.md
--rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.6.0/docs/extras/command_palette.md
--rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.6.0/docs/extras/index.md
--rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.6.0/docs/extras/log_monitor.md
--rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.6.0/docs/extras/styles.md
--rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.6.0/docs/index.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:33.616425 qtstrap-0.6.0/docs/quickstart/
--rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/quickstart/baseapplication.md
--rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/quickstart/basemainwindow.md
--rw-rw-rw-   0        0        0     3157 2024-05-21 21:30:41.000000 qtstrap-0.6.0/docs/quickstart/context_layouts.md
--rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.6.0/docs/quickstart/gettingstarted.md
--rw-rw-rw-   0        0        0      857 2023-10-11 23:04:26.000000 qtstrap-0.6.0/docs/quickstart/installation.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.061848 qtstrap-0.6.0/docs/reference/
--rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/base_application.md
--rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/base_window.md
--rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/options.md
--rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/settings.md
--rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/toolbar.md
--rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.adapter.md
--rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.decorators.md
--rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.defer.md
--rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.md
--rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.signals.md
--rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.singleton.md
--rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.timestamp.md
--rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.utils.md
--rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/widgets.buttons.md
--rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/widgets.labeledit.md
--rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.layouts.md
--rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.line_widgets.md
--rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.link_label.md
--rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/widgets.md
--rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/screenshot1.png
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.120849 qtstrap-0.6.0/docs/structure/
--rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/structure/makefile.md
--rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.6.0/docs/structure/structure.md
--rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.6.0/docs/test.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.125850 qtstrap-0.6.0/docs_theme/
--rw-rw-rw-   0        0        0      533 2024-05-08 19:17:34.000000 qtstrap-0.6.0/docs_theme/main.html
--rw-rw-rw-   0        0        0     1012 2024-05-08 19:02:43.000000 qtstrap-0.6.0/mkdocs.yml
--rw-rw-rw-   0        0        0      472 2023-09-01 05:22:34.000000 qtstrap-0.6.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.165428 qtstrap-0.6.0/qtstrap/
--rw-rw-rw-   0        0        0     1032 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/__init__.py
--rw-rw-rw-   0        0        0     1824 2024-05-08 19:26:13.000000 qtstrap-0.6.0/qtstrap/__main__.py
--rw-rw-rw-   0        0        0     2043 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/base_application.py
--rw-rw-rw-   0        0        0     2074 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/base_window.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.309871 qtstrap-0.6.0/qtstrap/experimental/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.6.0/qtstrap/experimental/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.323871 qtstrap-0.6.0/qtstrap/experimental/bindings/
--rw-rw-rw-   0        0        0       72 2024-05-21 21:31:21.000000 qtstrap-0.6.0/qtstrap/experimental/bindings/bind.py
--rw-rw-rw-   0        0        0      932 2024-05-21 21:31:23.000000 qtstrap-0.6.0/qtstrap/experimental/bindings/bind_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.332577 qtstrap-0.6.0/qtstrap/extras/
--rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.6.0/qtstrap/extras/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.366577 qtstrap-0.6.0/qtstrap/extras/code_editor/
--rw-rw-rw-   0        0        0      115 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/__init__.py
--rw-rw-rw-   0        0        0    12583 2023-09-01 05:35:36.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/code_editor.py
--rw-rw-rw-   0        0        0      842 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/code_line.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.427247 qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/
--rw-rw-rw-   0        0        0       38 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/__init__.py
--rw-rw-rw-   0        0        0     6354 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/python.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.444027 qtstrap-0.6.0/qtstrap/extras/command_palette/
--rw-rw-rw-   0        0        0       53 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/command_palette/__init__.py
--rw-rw-rw-   0        0        0    11922 2023-09-01 05:34:23.000000 qtstrap-0.6.0/qtstrap/extras/command_palette/command_palette.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.520609 qtstrap-0.6.0/qtstrap/extras/log_monitor/
--rw-rw-rw-   0        0        0     1151 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/__init__.py
--rw-rw-rw-   0        0        0     2425 2024-05-11 18:23:36.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_database_handler.py
--rw-rw-rw-   0        0        0    16860 2023-09-01 05:33:03.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_filter_controls.py
--rw-rw-rw-   0        0        0     4137 2023-09-01 05:31:54.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_profile.py
--rw-rw-rw-   0        0        0     3899 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_table_view.py
--rw-rw-rw-   0        0        0     4710 2023-09-01 05:31:19.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.553969 qtstrap-0.6.0/qtstrap/extras/settings_model/
--rw-rw-rw-   0        0        0       42 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/settings_model/__init__.py
--rw-rw-rw-   0        0        0      860 2023-09-10 15:38:48.000000 qtstrap-0.6.0/qtstrap/extras/settings_model/settings_model.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.582046 qtstrap-0.6.0/qtstrap/extras/style/
--rw-rw-rw-   0        0        0      131 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/style/__init__.py
--rw-rw-rw-   0        0        0     1087 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/style/colors.py
--rw-rw-rw-   0        0        0     2041 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/style/dark_palette.py
--rw-rw-rw-   0        0        0     4105 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/style/themes.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.587697 qtstrap-0.6.0/qtstrap/optional/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.6.0/qtstrap/optional/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-09-01 05:16:34.000000 qtstrap-0.6.0/qtstrap/options.py
--rw-rw-rw-   0        0        0      695 2023-09-01 05:17:27.000000 qtstrap-0.6.0/qtstrap/qt.py
--rw-rw-rw-   0        0        0      483 2023-10-25 22:17:39.000000 qtstrap-0.6.0/qtstrap/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.600474 qtstrap-0.6.0/qtstrap/template/
--rw-rw-rw-   0        0        0      128 2023-09-01 03:55:46.000000 qtstrap-0.6.0/qtstrap/template/.gitignore
--rw-rw-rw-   0        0        0     6016 2023-09-01 07:22:26.000000 qtstrap-0.6.0/qtstrap/template/Makefile
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.603187 qtstrap-0.6.0/qtstrap/template/app/
--rw-rw-rw-   0        0        0      959 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/template/app/main.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.608843 qtstrap-0.6.0/qtstrap/template/app/resources/
--rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.6.0/qtstrap/template/app/resources/application.ico
--rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.6.0/qtstrap/template/app/resources/icon.svg
--rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.6.0/qtstrap/template/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.617378 qtstrap-0.6.0/qtstrap/template/scripts/
--rw-rw-rw-   0        0        0     1032 2023-09-01 04:31:54.000000 qtstrap-0.6.0/qtstrap/template/scripts/bundle.spec
--rw-rw-rw-   0        0        0     2531 2023-09-01 04:31:30.000000 qtstrap-0.6.0/qtstrap/template/scripts/installer.iss
--rw-rw-rw-   0        0        0      908 2023-09-01 04:31:44.000000 qtstrap-0.6.0/qtstrap/template/scripts/onefile.spec
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.660313 qtstrap-0.6.0/qtstrap/utils/
--rw-rw-rw-   0        0        0      392 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/__init__.py
--rw-rw-rw-   0        0        0     2568 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/adapter.py
--rw-rw-rw-   0        0        0      344 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/call_later.py
--rw-rw-rw-   0        0        0      660 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/defer.py
--rw-rw-rw-   0        0        0     2776 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/utils/drag_and_drop.py
--rw-rw-rw-   0        0        0      631 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/get_ip.py
--rw-rw-rw-   0        0        0      373 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/signals.py
--rw-rw-rw-   0        0        0      418 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/singleton.py
--rw-rw-rw-   0        0        0     1033 2023-09-09 06:01:01.000000 qtstrap-0.6.0/qtstrap/utils/string_builder.py
--rw-rw-rw-   0        0        0      810 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/timestamp.py
--rw-rw-rw-   0        0        0     1033 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/trace.py
--rw-rw-rw-   0        0        0     2486 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.700819 qtstrap-0.6.0/qtstrap/widgets/
--rw-rw-rw-   0        0        0      885 2023-09-01 05:18:02.000000 qtstrap-0.6.0/qtstrap/widgets/__init__.py
--rw-rw-rw-   0        0        0     2967 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/buttons.py
--rw-rw-rw-   0        0        0     1580 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/labeledit.py
--rw-rw-rw-   0        0        0    14244 2024-05-21 20:56:22.000000 qtstrap-0.6.0/qtstrap/widgets/layouts.py
--rw-rw-rw-   0        0        0      667 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/line_widgets.py
--rw-rw-rw-   0        0        0      826 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/link_label.py
--rw-rw-rw-   0        0        0     3161 2024-01-06 22:05:43.000000 qtstrap-0.6.0/qtstrap/widgets/persistent_tab_widget.py
--rw-rw-rw-   0        0        0     5415 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/widgets/persistent_widgets.py
--rw-rw-rw-   0        0        0     7286 2023-09-01 05:29:00.000000 qtstrap-0.6.0/qtstrap/widgets/toggle.py
--rw-rw-rw-   0        0        0      910 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/widgets/toolbar.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.735154 qtstrap-0.6.0/qtstrap.egg-info/
--rw-rw-rw-   0        0        0     4070 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5390 2024-05-21 21:34:31.000000 qtstrap-0.6.0/qtstrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 21:34:29.000000 qtstrap-0.6.0/qtstrap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       52 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2023-09-01 05:40:08.000000 qtstrap-0.6.0/requirements.txt
--rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.6.0/requirements_build.txt
--rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.6.0/requirements_test.txt
--rw-rw-rw-   0        0        0       55 2023-10-25 22:17:30.000000 qtstrap-0.6.0/ruff.toml
--rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.6.0/run_tox_tests.py
--rw-rw-rw-   0        0        0     1246 2024-05-21 21:34:34.755069 qtstrap-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.712234 qtstrap-0.6.0/test/
--rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.6.0/test/test_base_app.py
--rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.6.0/test/test_base_window.py
--rw-rw-rw-   0        0        0     2953 2024-05-21 20:22:47.000000 qtstrap-0.6.0/test/test_layouts.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.728752 qtstrap-0.6.0/test/utils/
--rw-rw-rw-   0        0        0      434 2024-05-08 19:00:02.000000 qtstrap-0.6.0/test/utils/test_call_later.py
--rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.6.0/test/utils/test_defer.py
--rw-rw-rw-   0        0        0      811 2024-05-08 19:00:02.000000 qtstrap-0.6.0/test/utils/test_signal_adapter.py
--rw-rw-rw-   0        0        0      161 2024-05-08 19:00:02.000000 qtstrap-0.6.0/test/utils/test_singleton.py
--rw-rw-rw-   0        0        0      688 2023-09-09 06:03:50.000000 qtstrap-0.6.0/test/utils/test_string_builder.py
--rw-rw-rw-   0        0        0     2689 2023-09-09 03:30:22.000000 qtstrap-0.6.0/test/utils/test_utils.py
--rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.6.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.291703 qtstrap-0.6.1/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:42.963816 qtstrap-0.6.1/.github/
+-rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.6.1/.github/FUNDING.yml
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:42.964815 qtstrap-0.6.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1026 2024-05-08 19:00:02.000000 qtstrap-0.6.1/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      173 2024-04-03 18:10:27.000000 qtstrap-0.6.1/.gitignore
+-rw-rw-rw-   0        0        0     1159 2023-09-14 23:58:51.000000 qtstrap-0.6.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      132 2023-09-01 03:46:41.000000 qtstrap-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3048 2024-05-21 21:28:07.000000 qtstrap-0.6.1/Makefile
+-rw-rw-rw-   0        0        0     4070 2024-05-21 21:45:43.290704 qtstrap-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2975 2024-05-08 19:00:02.000000 qtstrap-0.6.1/README.md
+-rw-rw-rw-   0        0        0      340 2024-05-08 19:00:02.000000 qtstrap-0.6.1/build_docs.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:42.969815 qtstrap-0.6.1/docs/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.035505 qtstrap-0.6.1/docs/api/
+-rw-rw-rw-   0        0        0       68 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/.pages
+-rw-rw-rw-   0        0        0      395 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/experimental.md
+-rw-rw-rw-   0        0        0     5155 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.code_editor.code_editor.md
+-rw-rw-rw-   0        0        0     1469 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.code_editor.code_line.md
+-rw-rw-rw-   0        0        0      489 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.code_editor.highlighters.md
+-rw-rw-rw-   0        0        0     3309 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.code_editor.highlighters.python.md
+-rw-rw-rw-   0        0        0      505 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.code_editor.md
+-rw-rw-rw-   0        0        0     9538 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.command_palette.command_palette.md
+-rw-rw-rw-   0        0        0      480 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.command_palette.md
+-rw-rw-rw-   0        0        0     2636 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.log_monitor.log_database_handler.md
+-rw-rw-rw-   0        0        0    15224 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.log_monitor.log_filter_controls.md
+-rw-rw-rw-   0        0        0     4096 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.log_monitor.log_profile.md
+-rw-rw-rw-   0        0        0     4743 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.log_monitor.log_table_view.md
+-rw-rw-rw-   0        0        0     5173 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.log_monitor.log_widget.md
+-rw-rw-rw-   0        0        0      969 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.log_monitor.md
+-rw-rw-rw-   0        0        0      383 2024-05-21 21:28:28.000000 qtstrap-0.6.1/docs/api/extras.md
+-rw-rw-rw-   0        0        0      925 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.style.colors.md
+-rw-rw-rw-   0        0        0      854 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.style.dark_palette.md
+-rw-rw-rw-   0        0        0      471 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.style.md
+-rw-rw-rw-   0        0        0     1423 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/extras.style.themes.md
+-rw-rw-rw-   0        0        0      387 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/optional.md
+-rw-rw-rw-   0        0        0      628 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/options.md
+-rw-rw-rw-   0        0        0    11611 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/overview.md
+-rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.6.1/docs/api/settings.md
+-rw-rw-rw-   0        0        0     1513 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.adapter.md
+-rw-rw-rw-   0        0        0      750 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.call_later.md
+-rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.6.1/docs/api/utils.decorators.md
+-rw-rw-rw-   0        0        0     1142 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.defer.md
+-rw-rw-rw-   0        0        0     1846 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.drag_and_drop.md
+-rw-rw-rw-   0        0        0      824 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.get_ip.md
+-rw-rw-rw-   0        0        0      500 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.md
+-rw-rw-rw-   0        0        0     1069 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.signals.md
+-rw-rw-rw-   0        0        0      821 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.singleton.md
+-rw-rw-rw-   0        0        0     1713 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.string_builder.md
+-rw-rw-rw-   0        0        0     2145 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.timestamp.md
+-rw-rw-rw-   0        0        0     1220 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.trace.md
+-rw-rw-rw-   0        0        0     2801 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/utils.utils.md
+-rw-rw-rw-   0        0        0     5686 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.buttons.md
+-rw-rw-rw-   0        0        0     3263 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.labeledit.md
+-rw-rw-rw-   0        0        0    30518 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.layouts.md
+-rw-rw-rw-   0        0        0     1669 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0     2010 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.link_label.md
+-rw-rw-rw-   0        0        0      596 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.md
+-rw-rw-rw-   0        0        0     3450 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     8961 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     8844 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.toggle.md
+-rw-rw-rw-   0        0        0     1440 2024-05-21 21:28:29.000000 qtstrap-0.6.1/docs/api/widgets.toolbar.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.042508 qtstrap-0.6.1/docs/extras/
+-rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.6.1/docs/extras/code_editor.md
+-rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.6.1/docs/extras/command_palette.md
+-rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.6.1/docs/extras/index.md
+-rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.6.1/docs/extras/log_monitor.md
+-rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.6.1/docs/extras/styles.md
+-rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.6.1/docs/index.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.048506 qtstrap-0.6.1/docs/quickstart/
+-rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.6.1/docs/quickstart/baseapplication.md
+-rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.6.1/docs/quickstart/basemainwindow.md
+-rw-rw-rw-   0        0        0     3157 2024-05-21 21:30:41.000000 qtstrap-0.6.1/docs/quickstart/context_layouts.md
+-rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.6.1/docs/quickstart/gettingstarted.md
+-rw-rw-rw-   0        0        0      857 2023-10-11 23:04:26.000000 qtstrap-0.6.1/docs/quickstart/installation.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.076707 qtstrap-0.6.1/docs/reference/
+-rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/base_application.md
+-rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/base_window.md
+-rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/options.md
+-rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/settings.md
+-rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/toolbar.md
+-rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.adapter.md
+-rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.decorators.md
+-rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.defer.md
+-rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.md
+-rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.signals.md
+-rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.singleton.md
+-rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.timestamp.md
+-rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/utils.utils.md
+-rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/widgets.buttons.md
+-rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/widgets.labeledit.md
+-rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.6.1/docs/reference/widgets.layouts.md
+-rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.6.1/docs/reference/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.6.1/docs/reference/widgets.link_label.md
+-rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.6.1/docs/reference/widgets.md
+-rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.6.1/docs/reference/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.6.1/docs/reference/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.6.1/docs/screenshot1.png
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.078705 qtstrap-0.6.1/docs/structure/
+-rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.6.1/docs/structure/makefile.md
+-rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.6.1/docs/structure/structure.md
+-rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.6.1/docs/test.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.080707 qtstrap-0.6.1/docs_theme/
+-rw-rw-rw-   0        0        0      533 2024-05-08 19:17:34.000000 qtstrap-0.6.1/docs_theme/main.html
+-rw-rw-rw-   0        0        0     1012 2024-05-08 19:02:43.000000 qtstrap-0.6.1/mkdocs.yml
+-rw-rw-rw-   0        0        0      472 2023-09-01 05:22:34.000000 qtstrap-0.6.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.089706 qtstrap-0.6.1/qtstrap/
+-rw-rw-rw-   0        0        0     1032 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/__init__.py
+-rw-rw-rw-   0        0        0     1824 2024-05-08 19:26:13.000000 qtstrap-0.6.1/qtstrap/__main__.py
+-rw-rw-rw-   0        0        0     2043 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/base_application.py
+-rw-rw-rw-   0        0        0     2074 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/base_window.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.124703 qtstrap-0.6.1/qtstrap/experimental/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.6.1/qtstrap/experimental/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.126705 qtstrap-0.6.1/qtstrap/experimental/bindings/
+-rw-rw-rw-   0        0        0       72 2024-05-21 21:31:21.000000 qtstrap-0.6.1/qtstrap/experimental/bindings/bind.py
+-rw-rw-rw-   0        0        0      932 2024-05-21 21:31:23.000000 qtstrap-0.6.1/qtstrap/experimental/bindings/bind_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.128706 qtstrap-0.6.1/qtstrap/extras/
+-rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.6.1/qtstrap/extras/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.131704 qtstrap-0.6.1/qtstrap/extras/code_editor/
+-rw-rw-rw-   0        0        0      115 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/code_editor/__init__.py
+-rw-rw-rw-   0        0        0    12583 2023-09-01 05:35:36.000000 qtstrap-0.6.1/qtstrap/extras/code_editor/code_editor.py
+-rw-rw-rw-   0        0        0      842 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/code_editor/code_line.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.144705 qtstrap-0.6.1/qtstrap/extras/code_editor/highlighters/
+-rw-rw-rw-   0        0        0       38 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/code_editor/highlighters/__init__.py
+-rw-rw-rw-   0        0        0     6354 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/extras/code_editor/highlighters/python.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.146704 qtstrap-0.6.1/qtstrap/extras/command_palette/
+-rw-rw-rw-   0        0        0       53 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/command_palette/__init__.py
+-rw-rw-rw-   0        0        0    11922 2023-09-01 05:34:23.000000 qtstrap-0.6.1/qtstrap/extras/command_palette/command_palette.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.154703 qtstrap-0.6.1/qtstrap/extras/log_monitor/
+-rw-rw-rw-   0        0        0     1151 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/extras/log_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2425 2024-05-11 18:23:36.000000 qtstrap-0.6.1/qtstrap/extras/log_monitor/log_database_handler.py
+-rw-rw-rw-   0        0        0    16860 2023-09-01 05:33:03.000000 qtstrap-0.6.1/qtstrap/extras/log_monitor/log_filter_controls.py
+-rw-rw-rw-   0        0        0     4137 2023-09-01 05:31:54.000000 qtstrap-0.6.1/qtstrap/extras/log_monitor/log_profile.py
+-rw-rw-rw-   0        0        0     3899 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/extras/log_monitor/log_table_view.py
+-rw-rw-rw-   0        0        0     4710 2023-09-01 05:31:19.000000 qtstrap-0.6.1/qtstrap/extras/log_monitor/log_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.158703 qtstrap-0.6.1/qtstrap/extras/settings_model/
+-rw-rw-rw-   0        0        0       42 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/settings_model/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-09-10 15:38:48.000000 qtstrap-0.6.1/qtstrap/extras/settings_model/settings_model.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.163705 qtstrap-0.6.1/qtstrap/extras/style/
+-rw-rw-rw-   0        0        0      131 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/style/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-09-01 05:20:00.000000 qtstrap-0.6.1/qtstrap/extras/style/colors.py
+-rw-rw-rw-   0        0        0     2041 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/extras/style/dark_palette.py
+-rw-rw-rw-   0        0        0     4105 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/extras/style/themes.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.165707 qtstrap-0.6.1/qtstrap/optional/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.6.1/qtstrap/optional/__init__.py
+-rw-rw-rw-   0        0        0     1174 2023-09-01 05:16:34.000000 qtstrap-0.6.1/qtstrap/options.py
+-rw-rw-rw-   0        0        0      695 2023-09-01 05:17:27.000000 qtstrap-0.6.1/qtstrap/qt.py
+-rw-rw-rw-   0        0        0      483 2023-10-25 22:17:39.000000 qtstrap-0.6.1/qtstrap/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.167705 qtstrap-0.6.1/qtstrap/template/
+-rw-rw-rw-   0        0        0      128 2023-09-01 03:55:46.000000 qtstrap-0.6.1/qtstrap/template/.gitignore
+-rw-rw-rw-   0        0        0     6016 2023-09-01 07:22:26.000000 qtstrap-0.6.1/qtstrap/template/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.169705 qtstrap-0.6.1/qtstrap/template/app/
+-rw-rw-rw-   0        0        0      959 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/template/app/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.172705 qtstrap-0.6.1/qtstrap/template/app/resources/
+-rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.6.1/qtstrap/template/app/resources/application.ico
+-rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.6.1/qtstrap/template/app/resources/icon.svg
+-rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.6.1/qtstrap/template/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.176705 qtstrap-0.6.1/qtstrap/template/scripts/
+-rw-rw-rw-   0        0        0     1032 2023-09-01 04:31:54.000000 qtstrap-0.6.1/qtstrap/template/scripts/bundle.spec
+-rw-rw-rw-   0        0        0     2531 2023-09-01 04:31:30.000000 qtstrap-0.6.1/qtstrap/template/scripts/installer.iss
+-rw-rw-rw-   0        0        0      908 2023-09-01 04:31:44.000000 qtstrap-0.6.1/qtstrap/template/scripts/onefile.spec
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.234705 qtstrap-0.6.1/qtstrap/utils/
+-rw-rw-rw-   0        0        0      392 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/utils/__init__.py
+-rw-rw-rw-   0        0        0     2568 2024-05-08 19:00:02.000000 qtstrap-0.6.1/qtstrap/utils/adapter.py
+-rw-rw-rw-   0        0        0      344 2024-05-08 19:00:02.000000 qtstrap-0.6.1/qtstrap/utils/call_later.py
+-rw-rw-rw-   0        0        0      660 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/utils/defer.py
+-rw-rw-rw-   0        0        0     2776 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/utils/drag_and_drop.py
+-rw-rw-rw-   0        0        0      631 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/utils/get_ip.py
+-rw-rw-rw-   0        0        0      373 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/utils/signals.py
+-rw-rw-rw-   0        0        0      418 2024-05-08 19:00:02.000000 qtstrap-0.6.1/qtstrap/utils/singleton.py
+-rw-rw-rw-   0        0        0     1033 2023-09-09 06:01:01.000000 qtstrap-0.6.1/qtstrap/utils/string_builder.py
+-rw-rw-rw-   0        0        0      810 2024-05-08 19:00:02.000000 qtstrap-0.6.1/qtstrap/utils/timestamp.py
+-rw-rw-rw-   0        0        0     1033 2024-05-08 19:00:02.000000 qtstrap-0.6.1/qtstrap/utils/trace.py
+-rw-rw-rw-   0        0        0     2486 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.269703 qtstrap-0.6.1/qtstrap/widgets/
+-rw-rw-rw-   0        0        0      885 2023-09-01 05:18:02.000000 qtstrap-0.6.1/qtstrap/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2967 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/widgets/buttons.py
+-rw-rw-rw-   0        0        0     1580 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/widgets/labeledit.py
+-rw-rw-rw-   0        0        0    14244 2024-05-21 21:44:57.000000 qtstrap-0.6.1/qtstrap/widgets/layouts.py
+-rw-rw-rw-   0        0        0      667 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/widgets/line_widgets.py
+-rw-rw-rw-   0        0        0      826 2023-09-01 05:20:01.000000 qtstrap-0.6.1/qtstrap/widgets/link_label.py
+-rw-rw-rw-   0        0        0     3161 2024-01-06 22:05:43.000000 qtstrap-0.6.1/qtstrap/widgets/persistent_tab_widget.py
+-rw-rw-rw-   0        0        0     5415 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/widgets/persistent_widgets.py
+-rw-rw-rw-   0        0        0     7286 2023-09-01 05:29:00.000000 qtstrap-0.6.1/qtstrap/widgets/toggle.py
+-rw-rw-rw-   0        0        0      910 2023-09-01 05:22:52.000000 qtstrap-0.6.1/qtstrap/widgets/toolbar.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.288704 qtstrap-0.6.1/qtstrap.egg-info/
+-rw-rw-rw-   0        0        0     4070 2024-05-21 21:45:42.000000 qtstrap-0.6.1/qtstrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5390 2024-05-21 21:45:42.000000 qtstrap-0.6.1/qtstrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:45:42.000000 qtstrap-0.6.1/qtstrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-21 21:45:42.000000 qtstrap-0.6.1/qtstrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 21:45:41.000000 qtstrap-0.6.1/qtstrap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       52 2024-05-21 21:45:42.000000 qtstrap-0.6.1/qtstrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 21:45:42.000000 qtstrap-0.6.1/qtstrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1101 2023-09-01 05:40:08.000000 qtstrap-0.6.1/requirements.txt
+-rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.6.1/requirements_build.txt
+-rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.6.1/requirements_test.txt
+-rw-rw-rw-   0        0        0       55 2023-10-25 22:17:30.000000 qtstrap-0.6.1/ruff.toml
+-rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.6.1/run_tox_tests.py
+-rw-rw-rw-   0        0        0     1246 2024-05-21 21:45:43.295703 qtstrap-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.274705 qtstrap-0.6.1/test/
+-rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.6.1/test/test_base_app.py
+-rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.6.1/test/test_base_window.py
+-rw-rw-rw-   0        0        0     2953 2024-05-21 20:22:47.000000 qtstrap-0.6.1/test/test_layouts.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:45:43.286701 qtstrap-0.6.1/test/utils/
+-rw-rw-rw-   0        0        0      434 2024-05-08 19:00:02.000000 qtstrap-0.6.1/test/utils/test_call_later.py
+-rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.6.1/test/utils/test_defer.py
+-rw-rw-rw-   0        0        0      811 2024-05-08 19:00:02.000000 qtstrap-0.6.1/test/utils/test_signal_adapter.py
+-rw-rw-rw-   0        0        0      161 2024-05-08 19:00:02.000000 qtstrap-0.6.1/test/utils/test_singleton.py
+-rw-rw-rw-   0        0        0      688 2023-09-09 06:03:50.000000 qtstrap-0.6.1/test/utils/test_string_builder.py
+-rw-rw-rw-   0        0        0     2689 2023-09-09 03:30:22.000000 qtstrap-0.6.1/test/utils/test_utils.py
+-rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.6.1/tox.ini
```

### Comparing `qtstrap-0.6.0/.github/FUNDING.yml` & `qtstrap-0.6.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/.github/workflows/main.yml` & `qtstrap-0.6.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/CONTRIBUTING.md` & `qtstrap-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/LICENSE` & `qtstrap-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/Makefile` & `qtstrap-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/PKG-INFO` & `qtstrap-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.6.0
+Version: 0.6.1
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Documentation, https://qtstrap.github.io/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
```

### Comparing `qtstrap-0.6.0/README.md` & `qtstrap-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.code_editor.code_editor.md` & `qtstrap-0.6.1/docs/api/extras.code_editor.code_editor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.code_editor.code_line.md` & `qtstrap-0.6.1/docs/api/extras.code_editor.code_line.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.code_editor.highlighters.python.md` & `qtstrap-0.6.1/docs/api/extras.code_editor.highlighters.python.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.command_palette.command_palette.md` & `qtstrap-0.6.1/docs/api/extras.command_palette.command_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.log_monitor.log_database_handler.md` & `qtstrap-0.6.1/docs/api/extras.log_monitor.log_database_handler.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.log_monitor.log_filter_controls.md` & `qtstrap-0.6.1/docs/api/extras.log_monitor.log_filter_controls.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.log_monitor.log_profile.md` & `qtstrap-0.6.1/docs/api/extras.log_monitor.log_profile.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.log_monitor.log_table_view.md` & `qtstrap-0.6.1/docs/api/extras.log_monitor.log_table_view.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.log_monitor.log_widget.md` & `qtstrap-0.6.1/docs/api/extras.log_monitor.log_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.log_monitor.md` & `qtstrap-0.6.1/docs/api/extras.log_monitor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.style.colors.md` & `qtstrap-0.6.1/docs/api/extras.style.colors.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.style.dark_palette.md` & `qtstrap-0.6.1/docs/api/extras.style.dark_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/extras.style.themes.md` & `qtstrap-0.6.1/docs/api/extras.style.themes.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/options.md` & `qtstrap-0.6.1/docs/api/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/overview.md` & `qtstrap-0.6.1/docs/api/overview.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/settings.md` & `qtstrap-0.6.1/docs/api/settings.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.adapter.md` & `qtstrap-0.6.1/docs/api/utils.adapter.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.call_later.md` & `qtstrap-0.6.1/docs/api/utils.call_later.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.decorators.md` & `qtstrap-0.6.1/docs/api/utils.decorators.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.defer.md` & `qtstrap-0.6.1/docs/api/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.drag_and_drop.md` & `qtstrap-0.6.1/docs/api/utils.drag_and_drop.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.get_ip.md` & `qtstrap-0.6.1/docs/api/utils.get_ip.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.signals.md` & `qtstrap-0.6.1/docs/api/utils.signals.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.singleton.md` & `qtstrap-0.6.1/docs/api/utils.singleton.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.string_builder.md` & `qtstrap-0.6.1/docs/api/utils.string_builder.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.timestamp.md` & `qtstrap-0.6.1/docs/api/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.trace.md` & `qtstrap-0.6.1/docs/api/utils.trace.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/utils.utils.md` & `qtstrap-0.6.1/docs/api/utils.utils.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.buttons.md` & `qtstrap-0.6.1/docs/api/widgets.buttons.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.labeledit.md` & `qtstrap-0.6.1/docs/api/widgets.labeledit.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.layouts.md` & `qtstrap-0.6.1/docs/api/widgets.layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.line_widgets.md` & `qtstrap-0.6.1/docs/api/widgets.line_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.link_label.md` & `qtstrap-0.6.1/docs/api/widgets.link_label.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.md` & `qtstrap-0.6.1/docs/api/widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.persistent_tab_widget.md` & `qtstrap-0.6.1/docs/api/widgets.persistent_tab_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.persistent_widgets.md` & `qtstrap-0.6.1/docs/api/widgets.persistent_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.toggle.md` & `qtstrap-0.6.1/docs/api/widgets.toggle.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/api/widgets.toolbar.md` & `qtstrap-0.6.1/docs/api/widgets.toolbar.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/extras/code_editor.md` & `qtstrap-0.6.1/docs/extras/code_editor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/extras/command_palette.md` & `qtstrap-0.6.1/docs/extras/command_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/extras/log_monitor.md` & `qtstrap-0.6.1/docs/extras/log_monitor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/index.md` & `qtstrap-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/quickstart/baseapplication.md` & `qtstrap-0.6.1/docs/quickstart/baseapplication.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/quickstart/basemainwindow.md` & `qtstrap-0.6.1/docs/quickstart/basemainwindow.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/quickstart/context_layouts.md` & `qtstrap-0.6.1/docs/quickstart/context_layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/quickstart/gettingstarted.md` & `qtstrap-0.6.1/docs/quickstart/gettingstarted.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/quickstart/installation.md` & `qtstrap-0.6.1/docs/quickstart/installation.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/base_application.md` & `qtstrap-0.6.1/docs/reference/base_application.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/base_window.md` & `qtstrap-0.6.1/docs/reference/base_window.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/options.md` & `qtstrap-0.6.1/docs/reference/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/toolbar.md` & `qtstrap-0.6.1/docs/reference/toolbar.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/utils.adapter.md` & `qtstrap-0.6.1/docs/reference/utils.adapter.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/utils.defer.md` & `qtstrap-0.6.1/docs/reference/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/utils.signals.md` & `qtstrap-0.6.1/docs/reference/utils.signals.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/utils.timestamp.md` & `qtstrap-0.6.1/docs/reference/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/utils.utils.md` & `qtstrap-0.6.1/docs/reference/utils.utils.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.buttons.md` & `qtstrap-0.6.1/docs/reference/widgets.buttons.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.labeledit.md` & `qtstrap-0.6.1/docs/reference/widgets.labeledit.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.layouts.md` & `qtstrap-0.6.1/docs/reference/widgets.layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.line_widgets.md` & `qtstrap-0.6.1/docs/reference/widgets.line_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.link_label.md` & `qtstrap-0.6.1/docs/reference/widgets.link_label.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.md` & `qtstrap-0.6.1/docs/reference/widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.persistent_tab_widget.md` & `qtstrap-0.6.1/docs/reference/widgets.persistent_tab_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/reference/widgets.persistent_widgets.md` & `qtstrap-0.6.1/docs/reference/widgets.persistent_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/screenshot1.png` & `qtstrap-0.6.1/docs/screenshot1.png`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/structure/makefile.md` & `qtstrap-0.6.1/docs/structure/makefile.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/structure/structure.md` & `qtstrap-0.6.1/docs/structure/structure.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs/test.md` & `qtstrap-0.6.1/docs/test.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/docs_theme/main.html` & `qtstrap-0.6.1/docs_theme/main.html`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/mkdocs.yml` & `qtstrap-0.6.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/__init__.py` & `qtstrap-0.6.1/qtstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/__main__.py` & `qtstrap-0.6.1/qtstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/base_application.py` & `qtstrap-0.6.1/qtstrap/base_application.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/base_window.py` & `qtstrap-0.6.1/qtstrap/base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/experimental/bindings/bind_widgets.py` & `qtstrap-0.6.1/qtstrap/experimental/bindings/bind_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/code_editor/code_editor.py` & `qtstrap-0.6.1/qtstrap/extras/code_editor/code_editor.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/code_editor/code_line.py` & `qtstrap-0.6.1/qtstrap/extras/code_editor/code_line.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/python.py` & `qtstrap-0.6.1/qtstrap/extras/code_editor/highlighters/python.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/command_palette/command_palette.py` & `qtstrap-0.6.1/qtstrap/extras/command_palette/command_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/log_monitor/__init__.py` & `qtstrap-0.6.1/qtstrap/extras/log_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_database_handler.py` & `qtstrap-0.6.1/qtstrap/extras/log_monitor/log_database_handler.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_filter_controls.py` & `qtstrap-0.6.1/qtstrap/extras/log_monitor/log_filter_controls.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_profile.py` & `qtstrap-0.6.1/qtstrap/extras/log_monitor/log_profile.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_table_view.py` & `qtstrap-0.6.1/qtstrap/extras/log_monitor/log_table_view.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_widget.py` & `qtstrap-0.6.1/qtstrap/extras/log_monitor/log_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/settings_model/settings_model.py` & `qtstrap-0.6.1/qtstrap/extras/settings_model/settings_model.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/style/colors.py` & `qtstrap-0.6.1/qtstrap/extras/style/colors.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/style/dark_palette.py` & `qtstrap-0.6.1/qtstrap/extras/style/dark_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/extras/style/themes.py` & `qtstrap-0.6.1/qtstrap/extras/style/themes.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/options.py` & `qtstrap-0.6.1/qtstrap/options.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/qt.py` & `qtstrap-0.6.1/qtstrap/qt.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/Makefile` & `qtstrap-0.6.1/qtstrap/template/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/app/main.py` & `qtstrap-0.6.1/qtstrap/template/app/main.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/app/resources/application.ico` & `qtstrap-0.6.1/qtstrap/template/app/resources/application.ico`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/app/resources/icon.svg` & `qtstrap-0.6.1/qtstrap/template/app/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/scripts/bundle.spec` & `qtstrap-0.6.1/qtstrap/template/scripts/bundle.spec`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/scripts/installer.iss` & `qtstrap-0.6.1/qtstrap/template/scripts/installer.iss`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/template/scripts/onefile.spec` & `qtstrap-0.6.1/qtstrap/template/scripts/onefile.spec`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/adapter.py` & `qtstrap-0.6.1/qtstrap/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/defer.py` & `qtstrap-0.6.1/qtstrap/utils/defer.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/drag_and_drop.py` & `qtstrap-0.6.1/qtstrap/utils/drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/get_ip.py` & `qtstrap-0.6.1/qtstrap/utils/get_ip.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/string_builder.py` & `qtstrap-0.6.1/qtstrap/utils/string_builder.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/timestamp.py` & `qtstrap-0.6.1/qtstrap/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/trace.py` & `qtstrap-0.6.1/qtstrap/utils/trace.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/utils/utils.py` & `qtstrap-0.6.1/qtstrap/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/__init__.py` & `qtstrap-0.6.1/qtstrap/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/buttons.py` & `qtstrap-0.6.1/qtstrap/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/labeledit.py` & `qtstrap-0.6.1/qtstrap/widgets/labeledit.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/layouts.py` & `qtstrap-0.6.1/qtstrap/widgets/layouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 self.setContentsMargins(*margins)
             elif isinstance(margins, int):
                 self.setContentsMargins(margins, margins, margins, margins)
 
         if align in alignments:
             self.setAlignment(alignments[align])
 
-        self._stack: Sequence[ContextLayoutBase] = []
+        self._stack: list[ContextLayoutBase] = []
         self.next_layout: ContextLayoutBase | None = None
 
     def __getattr__(self, name: str):
         return getattr(self._layout, name)
 
     @property
     def _layout(self):
@@ -308,15 +308,15 @@
 
         return b
 
 
 # --------------------------------------------------------------------------- #
 
 
-class CSplitter(QSplitter, ContextLayout):
+class CSplitter(QSplitter, ContextLayoutBase):
     def __init__(
         self,
         parent: QWidget | QLayout | ContextLayoutBase | None = None,
         margins: QMargins | tuple | int | None = None,
         orientation: OrientationType | None = None,
         **kwargs,
     ):
```

### Comparing `qtstrap-0.6.0/qtstrap/widgets/line_widgets.py` & `qtstrap-0.6.1/qtstrap/widgets/line_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/link_label.py` & `qtstrap-0.6.1/qtstrap/widgets/link_label.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/persistent_tab_widget.py` & `qtstrap-0.6.1/qtstrap/widgets/persistent_tab_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/persistent_widgets.py` & `qtstrap-0.6.1/qtstrap/widgets/persistent_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/toggle.py` & `qtstrap-0.6.1/qtstrap/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap/widgets/toolbar.py` & `qtstrap-0.6.1/qtstrap/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/qtstrap.egg-info/PKG-INFO` & `qtstrap-0.6.1/qtstrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.6.0
+Version: 0.6.1
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Documentation, https://qtstrap.github.io/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
```

### Comparing `qtstrap-0.6.0/qtstrap.egg-info/SOURCES.txt` & `qtstrap-0.6.1/qtstrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/requirements.txt` & `qtstrap-0.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/requirements_build.txt` & `qtstrap-0.6.1/requirements_build.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/requirements_test.txt` & `qtstrap-0.6.1/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/setup.cfg` & `qtstrap-0.6.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7473 7472 6170 0d0a 7665 7273   = qtstrap..vers
-00000020: 696f 6e20 3d20 302e 362e 300d 0a64 6573  ion = 0.6.0..des
+00000020: 696f 6e20 3d20 302e 362e 310d 0a64 6573  ion = 0.6.1..des
 00000030: 6372 6970 7469 6f6e 203d 204c 696b 6520  cription = Like 
 00000040: 426f 6f74 7374 7261 702c 2062 7574 2071  Bootstrap, but q
 00000050: 742d 6572 2e0d 0a6c 6f6e 675f 6465 7363  t-er...long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
```

### Comparing `qtstrap-0.6.0/test/test_base_app.py` & `qtstrap-0.6.1/test/test_base_app.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/test/test_base_window.py` & `qtstrap-0.6.1/test/test_base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/test/test_layouts.py` & `qtstrap-0.6.1/test/test_layouts.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/test/utils/test_signal_adapter.py` & `qtstrap-0.6.1/test/utils/test_signal_adapter.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/test/utils/test_string_builder.py` & `qtstrap-0.6.1/test/utils/test_string_builder.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.6.0/test/utils/test_utils.py` & `qtstrap-0.6.1/test/utils/test_utils.py`

 * *Files identical despite different names*

