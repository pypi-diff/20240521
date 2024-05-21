# Comparing `tmp/qtstrap-0.5.3.tar.gz` & `tmp/qtstrap-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtstrap-0.5.3.tar", last modified: Sat Sep  9 06:13:51 2023, max compression
+gzip compressed data, was "qtstrap-0.6.0.tar", last modified: Tue May 21 21:34:34 2024, max compression
```

## Comparing `qtstrap-0.5.3.tar` & `qtstrap-0.6.0.tar`

### file list

```diff
@@ -1,200 +1,212 @@
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.456005 qtstrap-0.5.3/
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.187508 qtstrap-0.5.3/.github/
--rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.5.3/.github/FUNDING.yml
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.189508 qtstrap-0.5.3/.github/workflows/
--rw-rw-rw-   0        0        0      978 2022-07-30 04:06:00.000000 qtstrap-0.5.3/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      161 2022-11-24 04:51:10.000000 qtstrap-0.5.3/.gitignore
--rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.5.3/LICENSE
--rw-rw-rw-   0        0        0      132 2023-09-01 03:46:41.000000 qtstrap-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3574 2023-09-01 03:44:43.000000 qtstrap-0.5.3/Makefile
--rw-rw-rw-   0        0        0     3544 2023-09-09 06:13:51.456005 qtstrap-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2441 2023-03-27 09:49:48.000000 qtstrap-0.5.3/README.md
--rw-rw-rw-   0        0        0      272 2022-07-30 03:58:00.000000 qtstrap-0.5.3/build_docs.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.195505 qtstrap-0.5.3/docs/
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.264006 qtstrap-0.5.3/docs/api/
--rw-rw-rw-   0        0        0       68 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/.pages
--rw-rw-rw-   0        0        0     4540 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.code_editor.code_editor.md
--rw-rw-rw-   0        0        0     1305 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.code_editor.code_line.md
--rw-rw-rw-   0        0        0      448 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.code_editor.highlighters.md
--rw-rw-rw-   0        0        0     3021 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.code_editor.highlighters.python.md
--rw-rw-rw-   0        0        0      464 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.code_editor.md
--rw-rw-rw-   0        0        0     8390 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.command_palette.command_palette.md
--rw-rw-rw-   0        0        0      439 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.command_palette.md
--rw-rw-rw-   0        0        0     2349 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.log_monitor.log_database_handler.md
--rw-rw-rw-   0        0        0    13379 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.log_monitor.log_filter_controls.md
--rw-rw-rw-   0        0        0     3604 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.log_monitor.log_profile.md
--rw-rw-rw-   0        0        0     4181 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.log_monitor.log_table_view.md
--rw-rw-rw-   0        0        0     4558 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.log_monitor.log_widget.md
--rw-rw-rw-   0        0        0      887 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.log_monitor.md
--rw-rw-rw-   0        0        0      342 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.md
--rw-rw-rw-   0        0        0      802 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.style.colors.md
--rw-rw-rw-   0        0        0      772 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.style.dark_palette.md
--rw-rw-rw-   0        0        0      430 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.style.md
--rw-rw-rw-   0        0        0     1259 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/extras.style.themes.md
--rw-rw-rw-   0        0        0      546 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/options.md
--rw-rw-rw-   0        0        0    11165 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/overview.md
--rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.5.3/docs/api/settings.md
--rw-rw-rw-   0        0        0     1958 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.adapter.md
--rw-rw-rw-   0        0        0      784 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.call_later.md
--rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.5.3/docs/api/utils.decorators.md
--rw-rw-rw-   0        0        0     1019 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.defer.md
--rw-rw-rw-   0        0        0     1641 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.drag_and_drop.md
--rw-rw-rw-   0        0        0      742 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.get_ip.md
--rw-rw-rw-   0        0        0      459 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.md
--rw-rw-rw-   0        0        0      946 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.signals.md
--rw-rw-rw-   0        0        0      607 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.singleton.md
--rw-rw-rw-   0        0        0     1414 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.string_builder.md
--rw-rw-rw-   0        0        0     1597 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.timestamp.md
--rw-rw-rw-   0        0        0      641 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.trace.md
--rw-rw-rw-   0        0        0     2555 2023-03-27 09:43:36.000000 qtstrap-0.5.3/docs/api/utils.utils.md
--rw-rw-rw-   0        0        0     4948 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.buttons.md
--rw-rw-rw-   0        0        0     2853 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.labeledit.md
--rw-rw-rw-   0        0        0    16745 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.layouts.md
--rw-rw-rw-   0        0        0     1464 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.line_widgets.md
--rw-rw-rw-   0        0        0     1764 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.link_label.md
--rw-rw-rw-   0        0        0      555 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.md
--rw-rw-rw-   0        0        0     3040 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     7854 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     7763 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.toggle.md
--rw-rw-rw-   0        0        0     1276 2023-03-27 09:43:37.000000 qtstrap-0.5.3/docs/api/widgets.toolbar.md
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.272506 qtstrap-0.5.3/docs/extras/
--rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.5.3/docs/extras/code_editor.md
--rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.5.3/docs/extras/command_palette.md
--rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.5.3/docs/extras/index.md
--rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.5.3/docs/extras/log_monitor.md
--rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.5.3/docs/extras/styles.md
--rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.5.3/docs/index.md
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.280004 qtstrap-0.5.3/docs/quickstart/
--rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.5.3/docs/quickstart/baseapplication.md
--rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.5.3/docs/quickstart/basemainwindow.md
--rw-rw-rw-   0        0        0     1700 2021-04-01 21:16:04.000000 qtstrap-0.5.3/docs/quickstart/context_layouts.md
--rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.5.3/docs/quickstart/gettingstarted.md
--rw-rw-rw-   0        0        0      857 2021-04-01 21:16:04.000000 qtstrap-0.5.3/docs/quickstart/installation.md
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.310505 qtstrap-0.5.3/docs/reference/
--rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/base_application.md
--rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/base_window.md
--rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/options.md
--rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/settings.md
--rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/toolbar.md
--rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.adapter.md
--rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.decorators.md
--rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.defer.md
--rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.md
--rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.signals.md
--rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.singleton.md
--rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.timestamp.md
--rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/utils.utils.md
--rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/widgets.buttons.md
--rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/widgets.labeledit.md
--rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.5.3/docs/reference/widgets.layouts.md
--rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.5.3/docs/reference/widgets.line_widgets.md
--rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.5.3/docs/reference/widgets.link_label.md
--rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.5.3/docs/reference/widgets.md
--rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.5.3/docs/reference/widgets.persistent_tab_widget.md
--rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.5.3/docs/reference/widgets.persistent_widgets.md
--rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.5.3/docs/screenshot1.png
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.314007 qtstrap-0.5.3/docs/structure/
--rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.5.3/docs/structure/makefile.md
--rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.5.3/docs/structure/structure.md
--rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.5.3/docs/test.md
--rw-rw-rw-   0        0        0      987 2023-03-27 08:50:48.000000 qtstrap-0.5.3/mkdocs.yml
--rw-rw-rw-   0        0        0      472 2023-09-01 05:22:34.000000 qtstrap-0.5.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.324506 qtstrap-0.5.3/qtstrap/
--rw-rw-rw-   0        0        0     1032 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-09-01 05:12:32.000000 qtstrap-0.5.3/qtstrap/__main__.py
--rw-rw-rw-   0        0        0     2043 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/base_application.py
--rw-rw-rw-   0        0        0     2074 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/base_window.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.364006 qtstrap-0.5.3/qtstrap/experimental/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.5.3/qtstrap/experimental/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.365005 qtstrap-0.5.3/qtstrap/extras/
--rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.5.3/qtstrap/extras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.368506 qtstrap-0.5.3/qtstrap/extras/code_editor/
--rw-rw-rw-   0        0        0      115 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/code_editor/__init__.py
--rw-rw-rw-   0        0        0    12583 2023-09-01 05:35:36.000000 qtstrap-0.5.3/qtstrap/extras/code_editor/code_editor.py
--rw-rw-rw-   0        0        0      842 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/code_editor/code_line.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.371505 qtstrap-0.5.3/qtstrap/extras/code_editor/highlighters/
--rw-rw-rw-   0        0        0       38 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/code_editor/highlighters/__init__.py
--rw-rw-rw-   0        0        0     6354 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/extras/code_editor/highlighters/python.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.374005 qtstrap-0.5.3/qtstrap/extras/command_palette/
--rw-rw-rw-   0        0        0       53 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/command_palette/__init__.py
--rw-rw-rw-   0        0        0    11922 2023-09-01 05:34:23.000000 qtstrap-0.5.3/qtstrap/extras/command_palette/command_palette.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.384007 qtstrap-0.5.3/qtstrap/extras/log_monitor/
--rw-rw-rw-   0        0        0     1151 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/extras/log_monitor/__init__.py
--rw-rw-rw-   0        0        0     2425 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/extras/log_monitor/log_database_handler.py
--rw-rw-rw-   0        0        0    16860 2023-09-01 05:33:03.000000 qtstrap-0.5.3/qtstrap/extras/log_monitor/log_filter_controls.py
--rw-rw-rw-   0        0        0     4137 2023-09-01 05:31:54.000000 qtstrap-0.5.3/qtstrap/extras/log_monitor/log_profile.py
--rw-rw-rw-   0        0        0     3899 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/extras/log_monitor/log_table_view.py
--rw-rw-rw-   0        0        0     4710 2023-09-01 05:31:19.000000 qtstrap-0.5.3/qtstrap/extras/log_monitor/log_widget.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.387005 qtstrap-0.5.3/qtstrap/extras/settings_model/
--rw-rw-rw-   0        0        0       42 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/settings_model/__init__.py
--rw-rw-rw-   0        0        0      860 2023-05-25 14:16:23.000000 qtstrap-0.5.3/qtstrap/extras/settings_model/settings_model.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.394506 qtstrap-0.5.3/qtstrap/extras/style/
--rw-rw-rw-   0        0        0      131 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/style/__init__.py
--rw-rw-rw-   0        0        0     1087 2023-09-01 05:20:00.000000 qtstrap-0.5.3/qtstrap/extras/style/colors.py
--rw-rw-rw-   0        0        0     2041 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/extras/style/dark_palette.py
--rw-rw-rw-   0        0        0     4105 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/extras/style/themes.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.397006 qtstrap-0.5.3/qtstrap/optional/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.5.3/qtstrap/optional/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-09-01 05:16:34.000000 qtstrap-0.5.3/qtstrap/options.py
--rw-rw-rw-   0        0        0      695 2023-09-01 05:17:27.000000 qtstrap-0.5.3/qtstrap/qt.py
--rw-rw-rw-   0        0        0      483 2023-09-09 06:07:50.000000 qtstrap-0.5.3/qtstrap/settings.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.401004 qtstrap-0.5.3/qtstrap/template/
--rw-rw-rw-   0        0        0      128 2023-09-01 03:55:46.000000 qtstrap-0.5.3/qtstrap/template/.gitignore
--rw-rw-rw-   0        0        0     6016 2023-09-01 07:22:26.000000 qtstrap-0.5.3/qtstrap/template/Makefile
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.402005 qtstrap-0.5.3/qtstrap/template/app/
--rw-rw-rw-   0        0        0      959 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/template/app/main.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.406506 qtstrap-0.5.3/qtstrap/template/app/resources/
--rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.5.3/qtstrap/template/app/resources/application.ico
--rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.5.3/qtstrap/template/app/resources/icon.svg
--rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.5.3/qtstrap/template/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.411506 qtstrap-0.5.3/qtstrap/template/scripts/
--rw-rw-rw-   0        0        0     1032 2023-09-01 04:31:54.000000 qtstrap-0.5.3/qtstrap/template/scripts/bundle.spec
--rw-rw-rw-   0        0        0     2531 2023-09-01 04:31:30.000000 qtstrap-0.5.3/qtstrap/template/scripts/installer.iss
--rw-rw-rw-   0        0        0      908 2023-09-01 04:31:44.000000 qtstrap-0.5.3/qtstrap/template/scripts/onefile.spec
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.429005 qtstrap-0.5.3/qtstrap/utils/
--rw-rw-rw-   0        0        0      392 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/__init__.py
--rw-rw-rw-   0        0        0     2467 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/adapter.py
--rw-rw-rw-   0        0        0      272 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/call_later.py
--rw-rw-rw-   0        0        0      660 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/defer.py
--rw-rw-rw-   0        0        0     2776 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/utils/drag_and_drop.py
--rw-rw-rw-   0        0        0      631 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/get_ip.py
--rw-rw-rw-   0        0        0      373 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/signals.py
--rw-rw-rw-   0        0        0      252 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/singleton.py
--rw-rw-rw-   0        0        0     1033 2023-09-09 06:01:01.000000 qtstrap-0.5.3/qtstrap/utils/string_builder.py
--rw-rw-rw-   0        0        0      519 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/timestamp.py
--rw-rw-rw-   0        0        0      293 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/trace.py
--rw-rw-rw-   0        0        0     2486 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.444005 qtstrap-0.5.3/qtstrap/widgets/
--rw-rw-rw-   0        0        0      885 2023-09-01 05:18:02.000000 qtstrap-0.5.3/qtstrap/widgets/__init__.py
--rw-rw-rw-   0        0        0     2967 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/widgets/buttons.py
--rw-rw-rw-   0        0        0     1580 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/widgets/labeledit.py
--rw-rw-rw-   0        0        0    12901 2023-09-09 05:36:25.000000 qtstrap-0.5.3/qtstrap/widgets/layouts.py
--rw-rw-rw-   0        0        0      667 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/widgets/line_widgets.py
--rw-rw-rw-   0        0        0      826 2023-09-01 05:20:01.000000 qtstrap-0.5.3/qtstrap/widgets/link_label.py
--rw-rw-rw-   0        0        0     3153 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/widgets/persistent_tab_widget.py
--rw-rw-rw-   0        0        0     5415 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/widgets/persistent_widgets.py
--rw-rw-rw-   0        0        0     7286 2023-09-01 05:29:00.000000 qtstrap-0.5.3/qtstrap/widgets/toggle.py
--rw-rw-rw-   0        0        0      910 2023-09-01 05:22:52.000000 qtstrap-0.5.3/qtstrap/widgets/toolbar.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.362007 qtstrap-0.5.3/qtstrap.egg-info/
--rw-rw-rw-   0        0        0     3544 2023-09-09 06:13:50.000000 qtstrap-0.5.3/qtstrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5120 2023-09-09 06:13:51.000000 qtstrap-0.5.3/qtstrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-09 06:13:50.000000 qtstrap-0.5.3/qtstrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-09-09 06:13:50.000000 qtstrap-0.5.3/qtstrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-09-09 06:13:50.000000 qtstrap-0.5.3/qtstrap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       52 2023-09-09 06:13:50.000000 qtstrap-0.5.3/qtstrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-09-09 06:13:50.000000 qtstrap-0.5.3/qtstrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2023-09-01 05:40:08.000000 qtstrap-0.5.3/requirements.txt
--rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.5.3/requirements_build.txt
--rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.5.3/requirements_test.txt
--rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.5.3/run_tox_tests.py
--rw-rw-rw-   0        0        0     1254 2023-09-09 06:13:51.458505 qtstrap-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.449005 qtstrap-0.5.3/test/
--rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.5.3/test/test_base_app.py
--rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.5.3/test/test_base_window.py
--rw-rw-rw-   0        0        0     2352 2023-09-09 05:45:52.000000 qtstrap-0.5.3/test/test_layouts.py
-drwxrwxrwx   0        0        0        0 2023-09-09 06:13:51.454007 qtstrap-0.5.3/test/utils/
--rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.5.3/test/utils/test_defer.py
--rw-rw-rw-   0        0        0      688 2023-09-09 06:03:50.000000 qtstrap-0.5.3/test/utils/test_string_builder.py
--rw-rw-rw-   0        0        0     2689 2023-09-09 03:30:22.000000 qtstrap-0.5.3/test/utils/test_utils.py
--rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.5.3/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.738673 qtstrap-0.6.0/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:31.563301 qtstrap-0.6.0/.github/
+-rw-rw-rw-   0        0        0      784 2023-03-26 02:17:30.000000 qtstrap-0.6.0/.github/FUNDING.yml
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:31.603155 qtstrap-0.6.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1026 2024-05-08 19:00:02.000000 qtstrap-0.6.0/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      173 2024-04-03 18:10:27.000000 qtstrap-0.6.0/.gitignore
+-rw-rw-rw-   0        0        0     1159 2023-09-14 23:58:51.000000 qtstrap-0.6.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1090 2021-04-01 21:16:04.000000 qtstrap-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      132 2023-09-01 03:46:41.000000 qtstrap-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3048 2024-05-21 21:28:07.000000 qtstrap-0.6.0/Makefile
+-rw-rw-rw-   0        0        0     4070 2024-05-21 21:34:34.736673 qtstrap-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2975 2024-05-08 19:00:02.000000 qtstrap-0.6.0/README.md
+-rw-rw-rw-   0        0        0      340 2024-05-08 19:00:02.000000 qtstrap-0.6.0/build_docs.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:31.721212 qtstrap-0.6.0/docs/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:33.441359 qtstrap-0.6.0/docs/api/
+-rw-rw-rw-   0        0        0       68 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/.pages
+-rw-rw-rw-   0        0        0      395 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/experimental.md
+-rw-rw-rw-   0        0        0     5155 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.code_editor.md
+-rw-rw-rw-   0        0        0     1469 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.code_line.md
+-rw-rw-rw-   0        0        0      489 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.highlighters.md
+-rw-rw-rw-   0        0        0     3309 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.highlighters.python.md
+-rw-rw-rw-   0        0        0      505 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.code_editor.md
+-rw-rw-rw-   0        0        0     9538 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.command_palette.command_palette.md
+-rw-rw-rw-   0        0        0      480 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.command_palette.md
+-rw-rw-rw-   0        0        0     2636 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_database_handler.md
+-rw-rw-rw-   0        0        0    15224 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_filter_controls.md
+-rw-rw-rw-   0        0        0     4096 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_profile.md
+-rw-rw-rw-   0        0        0     4743 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_table_view.md
+-rw-rw-rw-   0        0        0     5173 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.log_widget.md
+-rw-rw-rw-   0        0        0      969 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.log_monitor.md
+-rw-rw-rw-   0        0        0      383 2024-05-21 21:28:28.000000 qtstrap-0.6.0/docs/api/extras.md
+-rw-rw-rw-   0        0        0      925 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.colors.md
+-rw-rw-rw-   0        0        0      854 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.dark_palette.md
+-rw-rw-rw-   0        0        0      471 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.md
+-rw-rw-rw-   0        0        0     1423 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/extras.style.themes.md
+-rw-rw-rw-   0        0        0      387 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/optional.md
+-rw-rw-rw-   0        0        0      628 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/options.md
+-rw-rw-rw-   0        0        0    11611 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/overview.md
+-rw-rw-rw-   0        0        0      754 2022-07-30 03:58:01.000000 qtstrap-0.6.0/docs/api/settings.md
+-rw-rw-rw-   0        0        0     1513 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.adapter.md
+-rw-rw-rw-   0        0        0      750 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.call_later.md
+-rw-rw-rw-   0        0        0      599 2022-07-30 03:58:01.000000 qtstrap-0.6.0/docs/api/utils.decorators.md
+-rw-rw-rw-   0        0        0     1142 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.defer.md
+-rw-rw-rw-   0        0        0     1846 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.drag_and_drop.md
+-rw-rw-rw-   0        0        0      824 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.get_ip.md
+-rw-rw-rw-   0        0        0      500 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.md
+-rw-rw-rw-   0        0        0     1069 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.signals.md
+-rw-rw-rw-   0        0        0      821 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.singleton.md
+-rw-rw-rw-   0        0        0     1713 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.string_builder.md
+-rw-rw-rw-   0        0        0     2145 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.timestamp.md
+-rw-rw-rw-   0        0        0     1220 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.trace.md
+-rw-rw-rw-   0        0        0     2801 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/utils.utils.md
+-rw-rw-rw-   0        0        0     5686 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.buttons.md
+-rw-rw-rw-   0        0        0     3263 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.labeledit.md
+-rw-rw-rw-   0        0        0    30518 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.layouts.md
+-rw-rw-rw-   0        0        0     1669 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0     2010 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.link_label.md
+-rw-rw-rw-   0        0        0      596 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.md
+-rw-rw-rw-   0        0        0     3450 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     8961 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     8844 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.toggle.md
+-rw-rw-rw-   0        0        0     1440 2024-05-21 21:28:29.000000 qtstrap-0.6.0/docs/api/widgets.toolbar.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:33.530889 qtstrap-0.6.0/docs/extras/
+-rw-rw-rw-   0        0        0      684 2023-03-27 09:12:02.000000 qtstrap-0.6.0/docs/extras/code_editor.md
+-rw-rw-rw-   0        0        0     1183 2023-03-27 09:27:16.000000 qtstrap-0.6.0/docs/extras/command_palette.md
+-rw-rw-rw-   0        0        0      105 2023-03-27 09:29:20.000000 qtstrap-0.6.0/docs/extras/index.md
+-rw-rw-rw-   0        0        0     1594 2023-03-27 09:42:00.000000 qtstrap-0.6.0/docs/extras/log_monitor.md
+-rw-rw-rw-   0        0        0       48 2023-03-27 09:41:38.000000 qtstrap-0.6.0/docs/extras/styles.md
+-rw-rw-rw-   0        0        0     1611 2023-03-26 02:25:27.000000 qtstrap-0.6.0/docs/index.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:33.616425 qtstrap-0.6.0/docs/quickstart/
+-rw-rw-rw-   0        0        0     2618 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/quickstart/baseapplication.md
+-rw-rw-rw-   0        0        0      920 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/quickstart/basemainwindow.md
+-rw-rw-rw-   0        0        0     3157 2024-05-21 21:30:41.000000 qtstrap-0.6.0/docs/quickstart/context_layouts.md
+-rw-rw-rw-   0        0        0     1264 2021-04-02 17:24:51.000000 qtstrap-0.6.0/docs/quickstart/gettingstarted.md
+-rw-rw-rw-   0        0        0      857 2023-10-11 23:04:26.000000 qtstrap-0.6.0/docs/quickstart/installation.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.061848 qtstrap-0.6.0/docs/reference/
+-rw-rw-rw-   0        0        0      759 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/base_application.md
+-rw-rw-rw-   0        0        0      682 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/base_window.md
+-rw-rw-rw-   0        0        0      653 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/options.md
+-rw-rw-rw-   0        0        0      287 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/settings.md
+-rw-rw-rw-   0        0        0      962 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/toolbar.md
+-rw-rw-rw-   0        0        0     1484 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.adapter.md
+-rw-rw-rw-   0        0        0       88 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.decorators.md
+-rw-rw-rw-   0        0        0      618 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.defer.md
+-rw-rw-rw-   0        0        0      353 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.md
+-rw-rw-rw-   0        0        0      576 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.signals.md
+-rw-rw-rw-   0        0        0      105 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.singleton.md
+-rw-rw-rw-   0        0        0      690 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.timestamp.md
+-rw-rw-rw-   0        0        0     1349 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/utils.utils.md
+-rw-rw-rw-   0        0        0     2361 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/widgets.buttons.md
+-rw-rw-rw-   0        0        0     1196 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/widgets.labeledit.md
+-rw-rw-rw-   0        0        0     4766 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.layouts.md
+-rw-rw-rw-   0        0        0      516 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.line_widgets.md
+-rw-rw-rw-   0        0        0      638 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.link_label.md
+-rw-rw-rw-   0        0        0     1408 2022-07-30 03:40:50.000000 qtstrap-0.6.0/docs/reference/widgets.md
+-rw-rw-rw-   0        0        0     1324 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.persistent_tab_widget.md
+-rw-rw-rw-   0        0        0     3704 2022-07-30 03:40:51.000000 qtstrap-0.6.0/docs/reference/widgets.persistent_widgets.md
+-rw-rw-rw-   0        0        0     2949 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/screenshot1.png
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.120849 qtstrap-0.6.0/docs/structure/
+-rw-rw-rw-   0        0        0     1193 2021-04-01 21:16:04.000000 qtstrap-0.6.0/docs/structure/makefile.md
+-rw-rw-rw-   0        0        0     3013 2022-07-30 00:37:45.000000 qtstrap-0.6.0/docs/structure/structure.md
+-rw-rw-rw-   0        0        0     7886 2022-07-30 03:01:48.000000 qtstrap-0.6.0/docs/test.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.125850 qtstrap-0.6.0/docs_theme/
+-rw-rw-rw-   0        0        0      533 2024-05-08 19:17:34.000000 qtstrap-0.6.0/docs_theme/main.html
+-rw-rw-rw-   0        0        0     1012 2024-05-08 19:02:43.000000 qtstrap-0.6.0/mkdocs.yml
+-rw-rw-rw-   0        0        0      472 2023-09-01 05:22:34.000000 qtstrap-0.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.165428 qtstrap-0.6.0/qtstrap/
+-rw-rw-rw-   0        0        0     1032 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/__init__.py
+-rw-rw-rw-   0        0        0     1824 2024-05-08 19:26:13.000000 qtstrap-0.6.0/qtstrap/__main__.py
+-rw-rw-rw-   0        0        0     2043 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/base_application.py
+-rw-rw-rw-   0        0        0     2074 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/base_window.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.309871 qtstrap-0.6.0/qtstrap/experimental/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:28.000000 qtstrap-0.6.0/qtstrap/experimental/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.323871 qtstrap-0.6.0/qtstrap/experimental/bindings/
+-rw-rw-rw-   0        0        0       72 2024-05-21 21:31:21.000000 qtstrap-0.6.0/qtstrap/experimental/bindings/bind.py
+-rw-rw-rw-   0        0        0      932 2024-05-21 21:31:23.000000 qtstrap-0.6.0/qtstrap/experimental/bindings/bind_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.332577 qtstrap-0.6.0/qtstrap/extras/
+-rw-rw-rw-   0        0        0        0 2021-04-08 13:05:51.000000 qtstrap-0.6.0/qtstrap/extras/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.366577 qtstrap-0.6.0/qtstrap/extras/code_editor/
+-rw-rw-rw-   0        0        0      115 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/__init__.py
+-rw-rw-rw-   0        0        0    12583 2023-09-01 05:35:36.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/code_editor.py
+-rw-rw-rw-   0        0        0      842 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/code_line.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.427247 qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/
+-rw-rw-rw-   0        0        0       38 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/__init__.py
+-rw-rw-rw-   0        0        0     6354 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/python.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.444027 qtstrap-0.6.0/qtstrap/extras/command_palette/
+-rw-rw-rw-   0        0        0       53 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/command_palette/__init__.py
+-rw-rw-rw-   0        0        0    11922 2023-09-01 05:34:23.000000 qtstrap-0.6.0/qtstrap/extras/command_palette/command_palette.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.520609 qtstrap-0.6.0/qtstrap/extras/log_monitor/
+-rw-rw-rw-   0        0        0     1151 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2425 2024-05-11 18:23:36.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_database_handler.py
+-rw-rw-rw-   0        0        0    16860 2023-09-01 05:33:03.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_filter_controls.py
+-rw-rw-rw-   0        0        0     4137 2023-09-01 05:31:54.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_profile.py
+-rw-rw-rw-   0        0        0     3899 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_table_view.py
+-rw-rw-rw-   0        0        0     4710 2023-09-01 05:31:19.000000 qtstrap-0.6.0/qtstrap/extras/log_monitor/log_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.553969 qtstrap-0.6.0/qtstrap/extras/settings_model/
+-rw-rw-rw-   0        0        0       42 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/settings_model/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-09-10 15:38:48.000000 qtstrap-0.6.0/qtstrap/extras/settings_model/settings_model.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.582046 qtstrap-0.6.0/qtstrap/extras/style/
+-rw-rw-rw-   0        0        0      131 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/style/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-09-01 05:20:00.000000 qtstrap-0.6.0/qtstrap/extras/style/colors.py
+-rw-rw-rw-   0        0        0     2041 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/style/dark_palette.py
+-rw-rw-rw-   0        0        0     4105 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/extras/style/themes.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.587697 qtstrap-0.6.0/qtstrap/optional/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:57:38.000000 qtstrap-0.6.0/qtstrap/optional/__init__.py
+-rw-rw-rw-   0        0        0     1174 2023-09-01 05:16:34.000000 qtstrap-0.6.0/qtstrap/options.py
+-rw-rw-rw-   0        0        0      695 2023-09-01 05:17:27.000000 qtstrap-0.6.0/qtstrap/qt.py
+-rw-rw-rw-   0        0        0      483 2023-10-25 22:17:39.000000 qtstrap-0.6.0/qtstrap/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.600474 qtstrap-0.6.0/qtstrap/template/
+-rw-rw-rw-   0        0        0      128 2023-09-01 03:55:46.000000 qtstrap-0.6.0/qtstrap/template/.gitignore
+-rw-rw-rw-   0        0        0     6016 2023-09-01 07:22:26.000000 qtstrap-0.6.0/qtstrap/template/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.603187 qtstrap-0.6.0/qtstrap/template/app/
+-rw-rw-rw-   0        0        0      959 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/template/app/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.608843 qtstrap-0.6.0/qtstrap/template/app/resources/
+-rw-rw-rw-   0        0        0    59285 2021-04-01 21:16:04.000000 qtstrap-0.6.0/qtstrap/template/app/resources/application.ico
+-rw-rw-rw-   0        0        0     5523 2021-04-01 21:16:04.000000 qtstrap-0.6.0/qtstrap/template/app/resources/icon.svg
+-rw-rw-rw-   0        0        0        0 2021-04-01 21:16:04.000000 qtstrap-0.6.0/qtstrap/template/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.617378 qtstrap-0.6.0/qtstrap/template/scripts/
+-rw-rw-rw-   0        0        0     1032 2023-09-01 04:31:54.000000 qtstrap-0.6.0/qtstrap/template/scripts/bundle.spec
+-rw-rw-rw-   0        0        0     2531 2023-09-01 04:31:30.000000 qtstrap-0.6.0/qtstrap/template/scripts/installer.iss
+-rw-rw-rw-   0        0        0      908 2023-09-01 04:31:44.000000 qtstrap-0.6.0/qtstrap/template/scripts/onefile.spec
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.660313 qtstrap-0.6.0/qtstrap/utils/
+-rw-rw-rw-   0        0        0      392 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/__init__.py
+-rw-rw-rw-   0        0        0     2568 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/adapter.py
+-rw-rw-rw-   0        0        0      344 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/call_later.py
+-rw-rw-rw-   0        0        0      660 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/defer.py
+-rw-rw-rw-   0        0        0     2776 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/utils/drag_and_drop.py
+-rw-rw-rw-   0        0        0      631 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/get_ip.py
+-rw-rw-rw-   0        0        0      373 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/signals.py
+-rw-rw-rw-   0        0        0      418 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/singleton.py
+-rw-rw-rw-   0        0        0     1033 2023-09-09 06:01:01.000000 qtstrap-0.6.0/qtstrap/utils/string_builder.py
+-rw-rw-rw-   0        0        0      810 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/timestamp.py
+-rw-rw-rw-   0        0        0     1033 2024-05-08 19:00:02.000000 qtstrap-0.6.0/qtstrap/utils/trace.py
+-rw-rw-rw-   0        0        0     2486 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.700819 qtstrap-0.6.0/qtstrap/widgets/
+-rw-rw-rw-   0        0        0      885 2023-09-01 05:18:02.000000 qtstrap-0.6.0/qtstrap/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2967 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/buttons.py
+-rw-rw-rw-   0        0        0     1580 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/labeledit.py
+-rw-rw-rw-   0        0        0    14244 2024-05-21 20:56:22.000000 qtstrap-0.6.0/qtstrap/widgets/layouts.py
+-rw-rw-rw-   0        0        0      667 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/line_widgets.py
+-rw-rw-rw-   0        0        0      826 2023-09-01 05:20:01.000000 qtstrap-0.6.0/qtstrap/widgets/link_label.py
+-rw-rw-rw-   0        0        0     3161 2024-01-06 22:05:43.000000 qtstrap-0.6.0/qtstrap/widgets/persistent_tab_widget.py
+-rw-rw-rw-   0        0        0     5415 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/widgets/persistent_widgets.py
+-rw-rw-rw-   0        0        0     7286 2023-09-01 05:29:00.000000 qtstrap-0.6.0/qtstrap/widgets/toggle.py
+-rw-rw-rw-   0        0        0      910 2023-09-01 05:22:52.000000 qtstrap-0.6.0/qtstrap/widgets/toolbar.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.735154 qtstrap-0.6.0/qtstrap.egg-info/
+-rw-rw-rw-   0        0        0     4070 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5390 2024-05-21 21:34:31.000000 qtstrap-0.6.0/qtstrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-21 21:34:29.000000 qtstrap-0.6.0/qtstrap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       52 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 21:34:30.000000 qtstrap-0.6.0/qtstrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1101 2023-09-01 05:40:08.000000 qtstrap-0.6.0/requirements.txt
+-rw-rw-rw-   0        0        0      529 2022-10-26 06:20:37.000000 qtstrap-0.6.0/requirements_build.txt
+-rw-rw-rw-   0        0        0      520 2022-10-26 06:55:20.000000 qtstrap-0.6.0/requirements_test.txt
+-rw-rw-rw-   0        0        0       55 2023-10-25 22:17:30.000000 qtstrap-0.6.0/ruff.toml
+-rw-rw-rw-   0        0        0      158 2022-11-24 06:15:10.000000 qtstrap-0.6.0/run_tox_tests.py
+-rw-rw-rw-   0        0        0     1246 2024-05-21 21:34:34.755069 qtstrap-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-07-30 01:23:30.000000 qtstrap-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.712234 qtstrap-0.6.0/test/
+-rw-rw-rw-   0        0        0      876 2021-04-01 21:16:04.000000 qtstrap-0.6.0/test/test_base_app.py
+-rw-rw-rw-   0        0        0     1073 2021-04-01 21:16:04.000000 qtstrap-0.6.0/test/test_base_window.py
+-rw-rw-rw-   0        0        0     2953 2024-05-21 20:22:47.000000 qtstrap-0.6.0/test/test_layouts.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:34:34.728752 qtstrap-0.6.0/test/utils/
+-rw-rw-rw-   0        0        0      434 2024-05-08 19:00:02.000000 qtstrap-0.6.0/test/utils/test_call_later.py
+-rw-rw-rw-   0        0        0      230 2022-11-24 04:25:54.000000 qtstrap-0.6.0/test/utils/test_defer.py
+-rw-rw-rw-   0        0        0      811 2024-05-08 19:00:02.000000 qtstrap-0.6.0/test/utils/test_signal_adapter.py
+-rw-rw-rw-   0        0        0      161 2024-05-08 19:00:02.000000 qtstrap-0.6.0/test/utils/test_singleton.py
+-rw-rw-rw-   0        0        0      688 2023-09-09 06:03:50.000000 qtstrap-0.6.0/test/utils/test_string_builder.py
+-rw-rw-rw-   0        0        0     2689 2023-09-09 03:30:22.000000 qtstrap-0.6.0/test/utils/test_utils.py
+-rw-rw-rw-   0        0        0      348 2022-11-30 16:27:29.000000 qtstrap-0.6.0/tox.ini
```

### Comparing `qtstrap-0.5.3/.github/FUNDING.yml` & `qtstrap-0.6.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/.github/workflows/main.yml` & `qtstrap-0.6.0/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,31 @@
   push:
     branches:
       - master
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
-          submodules: "recursive" 
           fetch-depth: 0       # Fetch all history for .GitInfo and .Lastmod
       - name: Setup Python
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v5
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           architecture: 'x64'
       - name: Install dependencies
         run: |
           python3 -m pip install --upgrade pip     # install pip
           python3 -m pip install mkdocs            # install mkdocs 
           python3 -m pip install mkdocs-mermaid2-plugin
           python3 -m pip install mkdocs-literate-nav
       - name: Build site
-        run: mkdocs build
+        run: |
+          # python3 buiid_docs.py
+          mkdocs build
       - name: Deploy
-        uses: peaceiris/actions-gh-pages@v3
+        uses: peaceiris/actions-gh-pages@v4
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: ./site
+          cname: docs.qtstrap.dev
```

### Comparing `qtstrap-0.5.3/LICENSE` & `qtstrap-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/Makefile` & `qtstrap-0.6.0/Makefile`

 * *Files 26% similar despite different names*

```diff
@@ -35,19 +35,23 @@
 
 #
 tox: venv
 	$(VENV_PYTHON) -m tox
 
 #
 tests: venv
-	$(VENV_PYTHON) -m pytest
+	$(VENV_PYTHON) -m pytest -s
 
 coverage: venv
 	$(VENV_PYTHON) -m pytest --cov
 
+docs: venv
+	$(VENV_PYTHON) build_docs.py
+.PHONY: docs
+
 # remove build artifacts
 clean:
 	-$(RM) build
 	-$(RM) dist
 	-$(RM) qtstrap.egg-info
 
 ## **************************************************************************** #
@@ -72,24 +76,24 @@
 VENV_PYTHON := $(VENV)/$(PYTHON)
 VENV_PYINSTALLER := $(VENV)/pyinstaller
 RM := rm -rf 
 CP := cp
 
 # Add this as a requirement to any make target that relies on the venv
 .PHONY: venv
-venv: $(VENV_DIR) $(VENV_CANARY_FILE)
+# venv: $(VENV_DIR) $(VENV_CANARY_FILE)
+venv: $(VENV_DIR)
 
 # Create the venv if it doesn't exist
 $(VENV_DIR):
 	$(PYTHON) -m venv $(VENV_DIR)
 
 # Update the venv if the canary is out of date
 $(VENV_CANARY_FILE): $(REQUIREMENTS)
-	$(VENV_PYTHON) -m pip install --upgrade pip
-	$(VENV_PYTHON) -m pip install -r $(REQUIREMENTS)
+	uv pip install -r $(REQUIREMENTS)
 	-$(RM) $(VENV_CANARY_DIR)
 	-mkdir $(VENV_CANARY_DIR)
 	-$(CP) $(REQUIREMENTS) $(VENV_CANARY_FILE)
 
 # forcibly update the canary file
 canary: $(VENV_CANARY_DIR)
 	-$(RM) $(VENV_CANARY_DIR)
@@ -98,38 +102,22 @@
 
 # update requirements.txt to match the state of the venv
 freeze_reqs: venv
 	$(VENV_PYTHON) -m pip freeze > $(REQUIREMENTS)
 
 # try to update the venv - expirimental feature, don't rely on it
 update_venv: venv
-	$(VENV_PYTHON) -m pip install --upgrade pip
-	$(VENV_PYTHON) -m pip install --upgrade -r $(REQUIREMENTS)
+	uv pip install -r $(REQUIREMENTS)
 	-$(RM) $(VENV_CANARY_DIR)
 	-mkdir $(VENV_CANARY_DIR)
 	-$(CP) $(REQUIREMENTS) $(VENV_CANARY_FILE)
 
 # remove all packages from the venv
 clean_venv:
 	$(RM) $(VENV_CANARY_DIR)
 	mkdir $(VENV_TMP_DIR)
 	$(VENV_PYTHON) -m pip freeze > $(VENV_TMP_FREEZE)
 	$(VENV_PYTHON) -m pip uninstall -y -r $(VENV_TMP_FREEZE)
 	$(RM) $(VENV_TMP_DIR)
 
 # clean the venv and rebuild it
 reset_venv: clean_venv update_venv
-
-# **************************************************************************** #
-# expirimental, probably not reliable
-
-# If the first argument is "pip"...
-ifeq (pip,$(firstword $(MAKECMDGOALS)))
-  # use the rest as arguments for "pip"
-  RUN_ARGS := $(wordlist 2,$(words $(MAKECMDGOALS)),$(MAKECMDGOALS))
-  # ...and turn them into do-nothing targets
-  $(eval $(RUN_ARGS):;@:)
-endif
-
-# forward pip commands to the venv
-pip: venv
-	$(VENV_PYTHON) -m pip $(RUN_ARGS)
```

### Comparing `qtstrap-0.5.3/PKG-INFO` & `qtstrap-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.5.3
+Version: 0.6.0
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
-Project-URL: Documentation, https://qtstrap.github.io/qtstrap/
+Project-URL: Documentation, https://qtstrap.github.io/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
 Project-URL: Tracker, https://github.com/qtstrap/qtstrap/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Widget Sets
@@ -38,23 +38,43 @@
 
 Qt is excellent, but it's also enormous. There's a lot of topics, and many of them have hidden gotchas. PySide2 and PyQt are also excellent, letting us leverage the powerful Qt libraries from up in the clouds in PythonLand, but this arrangement has its own gotchas. 
 
 The goal of qtstrap is get your applications up and running quickly, so you can focus on your problem instead of on Qt's idiosyncracies.
 
 # Features
 
-More complete docs are available [here](https://qtstrap.github.io/qtstrap/).
+More complete docs are available [here](https://qtstrap.github.io/).
 
 * `qtstrap` command line tool to bootstrap new projects
 * crossplatform makefile with useful development commands
 * preconfigured build system using PyInstaller and InnoSetup
 * custom Qt widgets with useful behaviors
 * Pythonic layout system using ContextLayouts
 * Some other stuff I haven't remembered yet
 
+# Quick start
+
+```sh
+$ mkdir test && cd test
+$ python3 -m venv .venv
+$ source .venv/bin/activate
+$ python3 -m pip install qtstrap PySide6
+$ qtstrap init
+```
+
+The init script will prompt you to enter the name of your application and the name of its publisher(which is probably you), and then it will generate an application skeleton.
+
+You can test that everything installed properly by executing:
+```sh
+$ python3 app/main.py
+```
+If you see a window like this, then you're good to go:
+
+![screenshot](docs/screenshot1.png) 
+
 ## Custom Widgets
 
 - `LabelEdit`
 - `HLine` and `VLine`
 - `LinkLabel`
 - Buttons:
   - `StateButton`
```

### Comparing `qtstrap-0.5.3/README.md` & `qtstrap-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,43 @@
 
 Qt is excellent, but it's also enormous. There's a lot of topics, and many of them have hidden gotchas. PySide2 and PyQt are also excellent, letting us leverage the powerful Qt libraries from up in the clouds in PythonLand, but this arrangement has its own gotchas. 
 
 The goal of qtstrap is get your applications up and running quickly, so you can focus on your problem instead of on Qt's idiosyncracies.
 
 # Features
 
-More complete docs are available [here](https://qtstrap.github.io/qtstrap/).
+More complete docs are available [here](https://qtstrap.github.io/).
 
 * `qtstrap` command line tool to bootstrap new projects
 * crossplatform makefile with useful development commands
 * preconfigured build system using PyInstaller and InnoSetup
 * custom Qt widgets with useful behaviors
 * Pythonic layout system using ContextLayouts
 * Some other stuff I haven't remembered yet
 
+# Quick start
+
+```sh
+$ mkdir test && cd test
+$ python3 -m venv .venv
+$ source .venv/bin/activate
+$ python3 -m pip install qtstrap PySide6
+$ qtstrap init
+```
+
+The init script will prompt you to enter the name of your application and the name of its publisher(which is probably you), and then it will generate an application skeleton.
+
+You can test that everything installed properly by executing:
+```sh
+$ python3 app/main.py
+```
+If you see a window like this, then you're good to go:
+
+![screenshot](docs/screenshot1.png) 
+
 ## Custom Widgets
 
 - `LabelEdit`
 - `HLine` and `VLine`
 - `LinkLabel`
 - Buttons:
   - `StateButton`
```

### Comparing `qtstrap-0.5.3/docs/api/extras.code_editor.code_editor.md` & `qtstrap-0.6.0/docs/api/extras.log_monitor.log_profile.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,211 +1,179 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `extras.code_editor.code_editor`
+# <kbd>module</kbd> `extras.log_monitor.log_profile`
 
 
 
 
 **Global Variables**
 ---------------
-- **TYPE_CHECKING**
-- **PYQT6**
-- **PYQT5**
-- **PYSIDE2**
-- **PYSIDE6**
+- **session_start_time**
+- **default_columns**
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `CodeEditor`
+## <kbd>class</kbd> `Column`
 
 
 
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.__init__`
+### <kbd>method</kbd> `Column.__init__`
 
 ```python
-__init__(*args, changed=None, model=None, highlighter=None, **kwargs)
+__init__(title=None, query=None, visible=True, width=0)
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L211"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.duplicate_selection`
+### <kbd>method</kbd> `Column.get_data`
 
 ```python
-duplicate_selection(direction)
+get_data()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L19"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.eventFilter`
+### <kbd>method</kbd> `Column.set_data`
 
 ```python
-eventFilter(obj, event)
+set_data(data)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L161"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.expand_selection`
+### <kbd>method</kbd> `Column.set_visibility`
 
 ```python
-expand_selection(cursor)
+set_visibility(visible)
 ```
 
 
 
 
 
----
-
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L307"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-### <kbd>method</kbd> `CodeEditor.indent_selection`
-
-```python
-indent_selection(direction)
-```
-
-
-
-
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.insert_completion`
+## <kbd>class</kbd> `LogProfile`
 
-```python
-insert_completion(completion)
-```
 
 
 
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L55"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-
----
-
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L73"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-### <kbd>method</kbd> `CodeEditor.keyPressEvent`
+### <kbd>method</kbd> `LogProfile.__init__`
 
 ```python
-keyPressEvent(event: PySide2.QtGui.QKeyEvent)
+__init__()
 ```
 
 
 
 
 
----
-
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L251"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.move_selection`
+---
 
-```python
-move_selection(direction)
-```
+#### <kbd>property</kbd> LogProfile.column_data
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L373"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+#### <kbd>property</kbd> LogProfile.visible_columns
 
-### <kbd>method</kbd> `CodeEditor.text`
 
-```python
-text()
-```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L68"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L88"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.text_under_cursor`
+### <kbd>method</kbd> `LogProfile.build_query`
 
 ```python
-text_under_cursor()
+build_query(row_count)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L164"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.toggle_comments`
+### <kbd>method</kbd> `LogProfile.get_log_level_column`
 
 ```python
-toggle_comments()
+get_log_level_column()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.update_tab_width`
+### <kbd>method</kbd> `LogProfile.set_columns`
 
 ```python
-update_tab_width()
+set_columns(column_data)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_editor.py#L356"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_profile.py#L77"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `CodeEditor.wrap_selection`
+### <kbd>method</kbd> `LogProfile.set_filter`
 
 ```python
-wrap_selection(key)
+set_filter(filt)
 ```
```

#### html2text {}

```diff
@@ -1,32 +1,25 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`extras.code_editor.code_editor` **Global Variables** --------------- -
-**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
-`CodeEditor` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
-method `CodeEditor.__init__` ```python __init__(*args, changed=None,
-model=None, highlighter=None, **kwargs) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.duplicate_selection`
-```python duplicate_selection(direction) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.eventFilter` ```python
-eventFilter(obj, event) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.expand_selection` ```python
-expand_selection(cursor) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.indent_selection` ```python
-indent_selection(direction) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.insert_completion` ```python
-insert_completion(completion) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.keyPressEvent` ```python
-keyPressEvent(event: PySide2.QtGui.QKeyEvent) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.move_selection`
-```python move_selection(direction) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `CodeEditor.text` ```python text()
-``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
-method `CodeEditor.text_under_cursor` ```python text_under_cursor() ``` ---
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`CodeEditor.toggle_comments` ```python toggle_comments() ``` --- _[_h_t_t_p_s_:_/_/
+`extras.log_monitor.log_profile` **Global Variables** --------------- -
+**session_start_time** - **default_columns** --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `Column` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Column.__init__` ```python
+__init__(title=None, query=None, visible=True, width=0) ``` --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`Column.get_data` ```python get_data() ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
+_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Column.set_data` ```python set_data
+(data) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `Column.set_visibility` ```python set_visibility(visible) ```
+--- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
+`LogProfile` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
+method `LogProfile.__init__` ```python __init__() ``` --- #### property
+LogProfile.column_data --- #### property LogProfile.visible_columns --- _[_h_t_t_p_s_:
+_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`LogProfile.build_query` ```python build_query(row_count) ``` --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`CodeEditor.update_tab_width` ```python update_tab_width() ``` --- _[_h_t_t_p_s_:_/_/
+`LogProfile.get_log_level_column` ```python get_log_level_column() ``` ---
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`LogProfile.set_columns` ```python set_columns(column_data) ``` --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`CodeEditor.wrap_selection` ```python wrap_selection(key) ``` --- _This file
-was automatically generated via [lazydocs](https://github.com/ml-tooling/
+`LogProfile.set_filter` ```python set_filter(filt) ``` --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/extras.code_editor.code_line.md` & `qtstrap-0.6.0/docs/api/extras.code_editor.code_line.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\code_editor\code_line.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\code_line.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.code_editor.code_line`
 
 
 
 
 **Global Variables**
@@ -14,22 +14,22 @@
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_line.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\code_line.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CodeLine`
 
 
 
 
-<a href="..\..\qtstrap\extras\code_editor\code_line.py#L6"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\code_line.py#L6"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeLine.__init__`
 
 ```python
 __init__(*args, **kwargs)
 ```
 
@@ -38,20 +38,20 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\code_line.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\code_line.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CodeLine.keyPressEvent`
 
 ```python
-keyPressEvent(event: PySide2.QtGui.QKeyEvent)
+keyPressEvent(event: PySide6.QtGui.QKeyEvent)
 ```
```

#### html2text {}

```diff
@@ -2,9 +2,9 @@
 `extras.code_editor.code_line` **Global Variables** --------------- -
 **TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
 `CodeLine` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
 method `CodeLine.__init__` ```python __init__(*args, **kwargs) ``` --- _[_h_t_t_p_s_:_/
 _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `CodeLine.keyPressEvent` ```python keyPressEvent(event:
-PySide2.QtGui.QKeyEvent) ``` --- _This file was automatically generated via
+PySide6.QtGui.QKeyEvent) ``` --- _This file was automatically generated via
 [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/extras.code_editor.highlighters.python.md` & `qtstrap-0.6.0/docs/api/extras.code_editor.highlighters.python.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.code_editor.highlighters.python`
 
 
 
 
 **Global Variables**
@@ -14,48 +14,50 @@
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 - **STYLES**
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `format`
 
 ```python
 format(color, style='')
 ```
 
 Return a QTextCharFormat with the given attributes. 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `get_style`
 
 ```python
 get_style(kind)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PythonHighlighter`
-Syntax highlighter for the Python language. 
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+
+
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L98"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PythonHighlighter.__init__`
 
 ```python
 __init__(document)
 ```
 
@@ -64,41 +66,41 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PythonHighlighter.build_rules`
 
 ```python
 build_rules()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L137"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L137"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PythonHighlighter.highlightBlock`
 
 ```python
 highlightBlock(text)
 ```
 
 Apply syntax highlighting to the given block of text. 
 
 ---
 
-<a href="..\..\qtstrap\extras\code_editor\highlighters\python.py#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\code_editor\highlighters\python.py#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PythonHighlighter.match_multiline`
 
 ```python
 match_multiline(text, delimiter, in_state, style)
 ```
```

#### html2text {}

```diff
@@ -2,23 +2,22 @@
 `extras.code_editor.highlighters.python` **Global Variables** --------------- -
 **TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** -
 **STYLES** --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]## function `format` ```python format(color, style='') ``` Return a
 QTextCharFormat with the given attributes. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
 _s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `get_style` ```python get_style
 (kind) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## class `PythonHighlighter` Syntax highlighter for the Python language.
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`PythonHighlighter.__init__` ```python __init__(document) ``` --- _[_h_t_t_p_s_:_/_/
+_s_q_u_a_r_e_]## class `PythonHighlighter` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `PythonHighlighter.__init__` ```python
+__init__(document) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `PythonHighlighter.build_rules` ```python
+build_rules() ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `PythonHighlighter.highlightBlock` ```python highlightBlock
+(text) ``` Apply syntax highlighting to the given block of text. --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`PythonHighlighter.build_rules` ```python build_rules() ``` --- _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`PythonHighlighter.highlightBlock` ```python highlightBlock(text) ``` Apply
-syntax highlighting to the given block of text. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `PythonHighlighter.match_multiline` ```python match_multiline(text, delimiter,
 in_state, style) ``` Do highlighting of multi-line strings. ``delimiter``
 should be a ``QRegularExpression`` for triple-single-quotes or triple-double-
 quotes, and ``in_state`` should be a unique integer to represent the
 corresponding state changes when inside those strings. Returns True if we're
 still inside a multi-line string when this function is finished. --- _This file
 was automatically generated via [lazydocs](https://github.com/ml-tooling/
```

### Comparing `qtstrap-0.5.3/docs/api/extras.command_palette.command_palette.md` & `qtstrap-0.6.0/docs/api/extras.command_palette.command_palette.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.command_palette.command_palette`
 
 
 
 
 **Global Variables**
@@ -15,37 +15,37 @@
 - **PYSIDE2**
 - **PYSIDE6**
 - **COMMAND_PALETTE_COLORS**
 - **registry**
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L26"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L26"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `get_color`
 
 ```python
 get_color(key)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L30"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L30"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CommandRegistry`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandRegistry.__init__`
 
 ```python
 __init__() → None
 ```
 
@@ -54,51 +54,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandRegistry.execute`
 
 ```python
 execute(command_name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandRegistry.register_command`
 
 ```python
 register_command(command)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `Command`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L48"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L48"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Command.__init__`
 
 ```python
 __init__(*args, **kwargs)
 ```
 
@@ -107,37 +107,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L56"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L56"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Command.used`
 
 ```python
 used()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PopupDelegate`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.__init__`
 
 ```python
 __init__(parent=None)
 ```
 
@@ -146,138 +146,138 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L65"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L65"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.get_colors`
 
 ```python
 get_colors()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.paint`
 
 ```python
 paint(
-    painter: PySide2.QtGui.QPainter,
-    option: PySide2.QtWidgets.QStyleOptionViewItem,
-    index: PySide2.QtCore.QModelIndex
+    painter: PySide6.QtGui.QPainter,
+    option: PySide6.QtWidgets.QStyleOptionViewItem,
+    index: PySide6.QtCore.QModelIndex
 )
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L72"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L72"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PopupDelegate.set_prefix`
 
 ```python
 set_prefix(prefix)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L143"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L149"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CommandModel`
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L155"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L161"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.data`
 
 ```python
-data(index: PySide2.QtCore.QModelIndex, role: int) → Any
+data(index: PySide6.QtCore.QModelIndex, role: int) → Any
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L165"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L171"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.index`
 
 ```python
-index(row: int, column: int, parent: PySide2.QtCore.QModelIndex) → QModelIndex
+index(row: int, column: int, parent: PySide6.QtCore.QModelIndex) → QModelIndex
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L152"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L158"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.rowCount`
 
 ```python
-rowCount(parent: PySide2.QtCore.QModelIndex) → int
+rowCount(parent: PySide6.QtCore.QModelIndex) → int
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L146"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L152"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandModel.sort_commands`
 
 ```python
 sort_commands(prefix)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L169"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L175"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `CommandCompleter`
 
 
 
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L170"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L176"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.__init__`
 
 ```python
 __init__(parent=None)
 ```
 
@@ -286,99 +286,99 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L200"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L206"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.close`
 
 ```python
 close()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L231"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L237"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.get_selection`
 
 ```python
 get_selection()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L224"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L230"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.move_selection_down`
 
 ```python
 move_selection_down()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L217"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L223"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.move_selection_up`
 
 ```python
 move_selection_up()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L195"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L201"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.open`
 
 ```python
 open()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L192"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L198"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.reset`
 
 ```python
 reset()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\command_palette\command_palette.py#L205"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\command_palette\command_palette.py#L211"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `CommandCompleter.update_prefix`
 
 ```python
 update_prefix(prefix)
 ```
```

#### html2text {}

```diff
@@ -17,26 +17,26 @@
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Command.used` ```python used() ``` ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
 `PopupDelegate` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### method `PopupDelegate.__init__` ```python __init__(parent=None) ```
 --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `PopupDelegate.get_colors` ```python get_colors() ``` --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`PopupDelegate.paint` ```python paint( painter: PySide2.QtGui.QPainter, option:
-PySide2.QtWidgets.QStyleOptionViewItem, index: PySide2.QtCore.QModelIndex ) ```
+`PopupDelegate.paint` ```python paint( painter: PySide6.QtGui.QPainter, option:
+PySide6.QtWidgets.QStyleOptionViewItem, index: PySide6.QtCore.QModelIndex ) ```
 --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `PopupDelegate.set_prefix` ```python set_prefix(prefix) ``` --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `CommandModel` -
 -- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`CommandModel.data` ```python data(index: PySide2.QtCore.QModelIndex, role:
+`CommandModel.data` ```python data(index: PySide6.QtCore.QModelIndex, role:
 int) â Any ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### method `CommandModel.index` ```python index(row: int, column: int,
-parent: PySide2.QtCore.QModelIndex) â QModelIndex ``` --- _[_h_t_t_p_s_:_/_/
+parent: PySide6.QtCore.QModelIndex) â QModelIndex ``` --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`CommandModel.rowCount` ```python rowCount(parent: PySide2.QtCore.QModelIndex)
+`CommandModel.rowCount` ```python rowCount(parent: PySide6.QtCore.QModelIndex)
 â int ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### method `CommandModel.sort_commands` ```python sort_commands(prefix)
 ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
 `CommandCompleter` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### method `CommandCompleter.__init__` ```python __init__(parent=None)
 ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
 method `CommandCompleter.close` ```python close() ``` --- _[_h_t_t_p_s_:_/_/
```

### Comparing `qtstrap-0.5.3/docs/api/extras.log_monitor.log_database_handler.md` & `qtstrap-0.6.0/docs/api/extras.log_monitor.log_database_handler.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.log_monitor.log_database_handler`
 
 
 
 
 **Global Variables**
@@ -17,22 +17,22 @@
 - **db_conn_name**
 - **initial_sql**
 - **insertion_sql**
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L62"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L62"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `DatabaseHandler`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L66"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L67"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `DatabaseHandler.__init__`
 
 ```python
 __init__(database_name)
 ```
 
@@ -49,57 +49,57 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L78"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L79"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `DatabaseHandler.emit`
 
 ```python
 emit(record)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L76"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `DatabaseHandler.format_time`
 
 ```python
 format_time(record)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L103"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L104"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>classmethod</kbd> `DatabaseHandler.register_callback`
 
 ```python
 register_callback(cb)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_database_handler.py#L107"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_database_handler.py#L108"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `DatabaseHandler.write`
 
 ```python
 write(m)
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/extras.log_monitor.log_filter_controls.md` & `qtstrap-0.6.0/docs/api/extras.log_monitor.log_filter_controls.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.log_monitor.log_filter_controls`
 
 
 
 
 **Global Variables**
@@ -14,64 +14,64 @@
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 - **LOG_FILTER_COLORS**
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `get_color`
 
 ```python
 get_color(key)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LoggerDelegate`
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L36"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L36"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerDelegate.paint`
 
 ```python
 paint(painter, option, index)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L62"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L62"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LoggerTreeWidgetItem`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L63"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L63"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.__init__`
 
 ```python
 __init__(parent, name, full_name)
 ```
 
@@ -80,107 +80,107 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L81"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L81"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.clicked`
 
 ```python
 clicked(column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.double_clicked`
 
 ```python
 double_clicked(column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.get_levels`
 
 ```python
 get_levels()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L126"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L126"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.set_all_levels`
 
 ```python
 set_all_levels(state: bool)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.set_levels`
 
 ```python
 set_levels(level_filter=[])
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L110"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L110"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidgetItem.update_data`
 
 ```python
 update_data()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L132"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L132"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LoggerTreeWidget`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L135"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L135"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.__init__`
 
 ```python
 __init__()
 ```
 
@@ -189,233 +189,233 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L168"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L168"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.click`
 
 ```python
 click(item, column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L204"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L204"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.contextMenuEvent`
 
 ```python
 contextMenuEvent(event)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L259"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L259"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.deselect_all`
 
 ```python
 deselect_all()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L234"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L234"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.disable_all_levels`
 
 ```python
 disable_all_levels(pos)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L226"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L226"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.disable_everything`
 
 ```python
 disable_everything()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L172"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L172"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.double_click`
 
 ```python
 double_click(item, column)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L230"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L230"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.enable_all_levels`
 
 ```python
 enable_all_levels(pos)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L222"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L222"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.enable_everything`
 
 ```python
 enable_everything()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L180"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L180"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.register_logger`
 
 ```python
 register_logger(full_name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L200"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L200"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.register_loggers`
 
 ```python
 register_loggers(loggers)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L251"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L251"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.select_all`
 
 ```python
 select_all()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L263"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L263"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.select_only`
 
 ```python
 select_only(pos)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L176"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L176"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.selection_changed`
 
 ```python
 selection_changed()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L216"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L216"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.set_levels_of_children`
 
 ```python
 set_levels_of_children(item, state)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L238"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L238"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LoggerTreeWidget.set_visible_loggers`
 
 ```python
 set_visible_loggers(visible_loggers)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L269"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L269"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `ProfileSelector`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L274"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L274"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.__init__`
 
 ```python
 __init__()
 ```
 
@@ -424,107 +424,107 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L297"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L297"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.eventFilter`
 
 ```python
 eventFilter(source, event)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L319"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L319"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_accept`
 
 ```python
 on_accept()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L314"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L314"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_add`
 
 ```python
 on_add()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L328"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L328"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_cancel`
 
 ```python
 on_cancel()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L310"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L310"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_change`
 
 ```python
 on_change()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L333"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L333"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `ProfileSelector.on_remove`
 
 ```python
 on_remove()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L338"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L338"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `FilterControls`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L359"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L363"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.__init__`
 
 ```python
 __init__(table)
 ```
 
@@ -533,85 +533,85 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L446"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L452"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.add_profile`
 
 ```python
 add_profile(name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L459"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L465"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.change_profile`
 
 ```python
 change_profile(profile_name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L467"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L473"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.columns_changed`
 
 ```python
 columns_changed()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L452"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L458"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.remove_profile`
 
 ```python
 remove_profile(name)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L442"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L448"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.save_settings`
 
 ```python
 save_settings()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_filter_controls.py#L471"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_filter_controls.py#L478"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `FilterControls.update_filter`
 
 ```python
 update_filter()
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/extras.log_monitor.log_widget.md` & `qtstrap-0.6.0/docs/api/extras.log_monitor.log_widget.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.log_monitor.log_widget`
 
 
 
 
 **Global Variables**
@@ -16,22 +16,22 @@
 - **PYSIDE6**
 - **db_conn_name**
 - **command_palette_available**
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogMonitorWidget`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L17"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L17"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorWidget.__init__`
 
 ```python
 __init__(parent=None)
 ```
 
@@ -40,51 +40,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorWidget.open_profile_prompt`
 
 ```python
 open_profile_prompt()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L50"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L50"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorWidget.query_existing_loggers`
 
 ```python
 query_existing_loggers()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L59"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L59"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogMonitorDockWidget`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L60"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDockWidget.__init__`
 
 ```python
 __init__(parent=None, shortcut='Ctrl+L')
 ```
 
@@ -93,51 +93,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDockWidget.adjust_size`
 
 ```python
 adjust_size()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L88"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L88"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDockWidget.toggleViewAction`
 
 ```python
 toggleViewAction()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L94"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LogMonitorDropdown`
 
 
 
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.__init__`
 
 ```python
 __init__(parent=None, shortcut='`')
 ```
 
@@ -146,57 +146,57 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L136"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L136"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.center_on_parent`
 
 ```python
 center_on_parent()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L114"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.eventFilter`
 
 ```python
-eventFilter(source: PySide2.QtCore.QObject, event: PySide2.QtCore.QEvent) → bool
+eventFilter(source: PySide6.QtCore.QObject, event: PySide6.QtCore.QEvent) → bool
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L123"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.toggleViewAction`
 
 ```python
 toggleViewAction()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\log_widget.py#L129"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\log_widget.py#L129"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LogMonitorDropdown.toggle_view`
 
 ```python
 toggle_view()
 ```
```

#### html2text {}

```diff
@@ -20,14 +20,14 @@
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `LogMonitorDropdown` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `LogMonitorDropdown.__init__`
 ```python __init__(parent=None, shortcut='`') ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `LogMonitorDropdown.center_on_parent` ```python center_on_parent() ``` ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `LogMonitorDropdown.eventFilter` ```python eventFilter(source:
-PySide2.QtCore.QObject, event: PySide2.QtCore.QEvent) â bool ``` --- _[_h_t_t_p_s_:_/
+PySide6.QtCore.QObject, event: PySide6.QtCore.QEvent) â bool ``` --- _[_h_t_t_p_s_:_/
 _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `LogMonitorDropdown.toggleViewAction` ```python toggleViewAction() ``` ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `LogMonitorDropdown.toggle_view` ```python toggle_view() ``` --- _This file was
 automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/extras.log_monitor.md` & `qtstrap-0.6.0/docs/api/extras.log_monitor.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\log_monitor\__init__.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\__init__.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.log_monitor`
 
 
 
 
 **Global Variables**
@@ -15,15 +15,15 @@
 - **log_table_view**
 - **log_widget**
 - **db_path**
 - **exception_logger_name**
 
 ---
 
-<a href="..\..\qtstrap\extras\log_monitor\__init__.py#L12"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\log_monitor\__init__.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `install`
 
 ```python
 install(database_name='P:/qtstrap/qtstrap/log.db', install_excepthook=True)
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/extras.style.colors.md` & `qtstrap-0.6.0/docs/api/options.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,23 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\style\colors.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\options.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `extras.style.colors`
+# <kbd>module</kbd> `options`
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\style\colors.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\options.py#L6"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `colors`
-
-
-
-
-
-
-
-
----
-
-<a href="..\..\qtstrap\extras\style\colors.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-## <kbd>class</kbd> `qcolors`
+## <kbd>class</kbd> `OPTIONS`
```

#### html2text {}

```diff
@@ -1,6 +1,4 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`extras.style.colors` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `colors` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `qcolors` --- _This file was
-automatically generated via [lazydocs](https://github.com/ml-tooling/
-lazydocs)._
+`options` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
+class `OPTIONS` --- _This file was automatically generated via [lazydocs]
+(https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/extras.style.themes.md` & `qtstrap-0.6.0/docs/api/extras.style.themes.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\extras\style\themes.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\style\themes.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `extras.style.themes`
 
 
 
 
 **Global Variables**
@@ -13,45 +13,45 @@
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 ---
 
-<a href="..\..\qtstrap\extras\style\themes.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\style\themes.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `dark`
 
 ```python
 dark() → QPalette
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\style\themes.py#L41"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\style\themes.py#L41"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `light`
 
 ```python
 light() → QPalette
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\extras\style\themes.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\style\themes.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `apply_theme`
 
 ```python
 apply_theme(theme, widget)
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/options.md` & `qtstrap-0.6.0/docs/api/utils.decorators.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\options.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-# <kbd>module</kbd> `options`
+<a href="..\..\qtstrap\utils\decorators.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+# <kbd>module</kbd> `utils.decorators`
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\options.py#L6"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-## <kbd>class</kbd> `OPTIONS`
+<a href="..\..\qtstrap\utils\decorators.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+## <kbd>function</kbd> `trace`
 
+```python
+trace(func)
+```
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`options` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
-class `OPTIONS` --- _This file was automatically generated via [lazydocs]
-(https://github.com/ml-tooling/lazydocs)._
+`utils.decorators` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]## function `trace` ```python trace(func) ``` --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/overview.md` & `qtstrap-0.6.0/docs/api/overview.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <!-- markdownlint-disable -->
 
 # API Overview
 
 ## Modules
 
+- [`experimental`](./experimental.md#module-experimental)
 - [`extras`](./extras.md#module-extras)
 - [`extras.code_editor`](./extras.code_editor.md#module-extrascode_editor)
 - [`extras.code_editor.code_editor`](./extras.code_editor.code_editor.md#module-extrascode_editorcode_editor)
 - [`extras.code_editor.code_line`](./extras.code_editor.code_line.md#module-extrascode_editorcode_line)
 - [`extras.code_editor.highlighters`](./extras.code_editor.highlighters.md#module-extrascode_editorhighlighters)
 - [`extras.code_editor.highlighters.python`](./extras.code_editor.highlighters.python.md#module-extrascode_editorhighlighterspython)
 - [`extras.command_palette`](./extras.command_palette.md#module-extrascommand_palette)
@@ -18,14 +19,15 @@
 - [`extras.log_monitor.log_profile`](./extras.log_monitor.log_profile.md#module-extraslog_monitorlog_profile)
 - [`extras.log_monitor.log_table_view`](./extras.log_monitor.log_table_view.md#module-extraslog_monitorlog_table_view)
 - [`extras.log_monitor.log_widget`](./extras.log_monitor.log_widget.md#module-extraslog_monitorlog_widget)
 - [`extras.style`](./extras.style.md#module-extrasstyle)
 - [`extras.style.colors`](./extras.style.colors.md#module-extrasstylecolors)
 - [`extras.style.dark_palette`](./extras.style.dark_palette.md#module-extrasstyledark_palette)
 - [`extras.style.themes`](./extras.style.themes.md#module-extrasstylethemes)
+- [`optional`](./optional.md#module-optional)
 - [`options`](./options.md#module-options)
 - [`utils`](./utils.md#module-utils)
 - [`utils.adapter`](./utils.adapter.md#module-utilsadapter)
 - [`utils.call_later`](./utils.call_later.md#module-utilscall_later)
 - [`utils.defer`](./utils.defer.md#module-utilsdefer)
 - [`utils.drag_and_drop`](./utils.drag_and_drop.md#module-utilsdrag_and_drop)
 - [`utils.get_ip`](./utils.get_ip.md#module-utilsget_ip)
@@ -46,15 +48,15 @@
 - [`widgets.toggle`](./widgets.toggle.md#module-widgetstoggle)
 - [`widgets.toolbar`](./widgets.toolbar.md#module-widgetstoolbar)
 
 ## Classes
 
 - [`code_editor.CodeEditor`](./extras.code_editor.code_editor.md#class-codeeditor)
 - [`code_line.CodeLine`](./extras.code_editor.code_line.md#class-codeline)
-- [`python.PythonHighlighter`](./extras.code_editor.highlighters.python.md#class-pythonhighlighter): Syntax highlighter for the Python language.
+- [`python.PythonHighlighter`](./extras.code_editor.highlighters.python.md#class-pythonhighlighter)
 - [`command_palette.Command`](./extras.command_palette.command_palette.md#class-command)
 - [`command_palette.CommandCompleter`](./extras.command_palette.command_palette.md#class-commandcompleter)
 - [`command_palette.CommandModel`](./extras.command_palette.command_palette.md#class-commandmodel)
 - [`command_palette.CommandRegistry`](./extras.command_palette.command_palette.md#class-commandregistry)
 - [`command_palette.PopupDelegate`](./extras.command_palette.command_palette.md#class-popupdelegate)
 - [`log_database_handler.DatabaseHandler`](./extras.log_monitor.log_database_handler.md#class-databasehandler)
 - [`log_filter_controls.FilterControls`](./extras.log_monitor.log_filter_controls.md#class-filtercontrols)
@@ -68,32 +70,33 @@
 - [`log_table_view.LogTableView`](./extras.log_monitor.log_table_view.md#class-logtableview)
 - [`log_widget.LogMonitorDockWidget`](./extras.log_monitor.log_widget.md#class-logmonitordockwidget)
 - [`log_widget.LogMonitorDropdown`](./extras.log_monitor.log_widget.md#class-logmonitordropdown)
 - [`log_widget.LogMonitorWidget`](./extras.log_monitor.log_widget.md#class-logmonitorwidget)
 - [`colors.colors`](./extras.style.colors.md#class-colors)
 - [`colors.qcolors`](./extras.style.colors.md#class-qcolors)
 - [`options.OPTIONS`](./options.md#class-options)
-- [`adapter.Adapter`](./utils.adapter.md#class-adapter): A signal adapter that helps create disposable connections between objects. 
+- [`adapter.Adapter`](./utils.adapter.md#class-adapter)
 - [`defer.Defer`](./utils.defer.md#class-defer): A context manager that emulates the defer keyword from other languages.
 - [`drag_and_drop.PreviewDrag`](./utils.drag_and_drop.md#class-previewdrag)
 - [`signals.SignalBlocker`](./utils.signals.md#class-signalblocker): A context manager that blocks the signals of the provided widget.
 - [`string_builder.Builder`](./utils.string_builder.md#class-builder): Utility class for incrementally building strings.
-- [`timestamp.TimeStamp`](./utils.timestamp.md#class-timestamp)
+- [`timestamp.TimeStamp`](./utils.timestamp.md#class-timestamp): A TimeStamp object that can be used to track the time since it was created.
 - [`buttons.ConfirmToggleButton`](./widgets.buttons.md#class-confirmtogglebutton)
 - [`buttons.IconToggleButton`](./widgets.buttons.md#class-icontogglebutton)
 - [`buttons.MenuButton`](./widgets.buttons.md#class-menubutton)
 - [`buttons.StateButton`](./widgets.buttons.md#class-statebutton)
 - [`labeledit.LabelEdit`](./widgets.labeledit.md#class-labeledit)
 - [`layouts.CFormLayout`](./widgets.layouts.md#class-cformlayout)
 - [`layouts.CGridLayout`](./widgets.layouts.md#class-cgridlayout)
 - [`layouts.CHBoxLayout`](./widgets.layouts.md#class-chboxlayout)
 - [`layouts.CScrollArea`](./widgets.layouts.md#class-cscrollarea)
 - [`layouts.CSplitter`](./widgets.layouts.md#class-csplitter)
 - [`layouts.CVBoxLayout`](./widgets.layouts.md#class-cvboxlayout)
 - [`layouts.ContextLayout`](./widgets.layouts.md#class-contextlayout)
+- [`layouts.ContextLayoutBase`](./widgets.layouts.md#class-contextlayoutbase)
 - [`layouts.PersistentCScrollArea`](./widgets.layouts.md#class-persistentcscrollarea)
 - [`layouts.PersistentCSplitter`](./widgets.layouts.md#class-persistentcsplitter)
 - [`line_widgets.HLine`](./widgets.line_widgets.md#class-hline)
 - [`line_widgets.VLine`](./widgets.line_widgets.md#class-vline)
 - [`link_label.LinkLabel`](./widgets.link_label.md#class-linklabel)
 - [`persistent_tab_widget.PersistentTabWidget`](./widgets.persistent_tab_widget.md#class-persistenttabwidget)
 - [`persistent_widgets.PersistentCheckBox`](./widgets.persistent_widgets.md#class-persistentcheckbox)
@@ -121,17 +124,18 @@
 - [`themes.apply_theme`](./extras.style.themes.md#function-apply_theme)
 - [`themes.dark`](./extras.style.themes.md#function-dark)
 - [`themes.light`](./extras.style.themes.md#function-light)
 - [`call_later.call_later`](./utils.call_later.md#function-call_later): call the given function after a specified delay
 - [`drag_and_drop.accepts_file_drops`](./utils.drag_and_drop.md#function-accepts_file_drops): Decorator that enables drag-and-drop on a QWidget.
 - [`drag_and_drop.draggable`](./utils.drag_and_drop.md#function-draggable)
 - [`get_ip.get_ip`](./utils.get_ip.md#function-get_ip): Get the current machine's IPv4 address.
-- [`singleton.singleton`](./utils.singleton.md#function-singleton):     
-- [`timestamp.time_since`](./utils.timestamp.md#function-time_since)
-- [`trace.trace`](./utils.trace.md#function-trace)
+- [`singleton.singleton`](./utils.singleton.md#function-singleton): Class decorator that only allows one instance to be created.
+- [`timestamp.time_since`](./utils.timestamp.md#function-time_since): Calculate the elapsed time since the given TimeStamp or time value.
+- [`trace.out`](./utils.trace.md#function-out): The print function used by the trace decorator.
+- [`trace.trace`](./utils.trace.md#function-trace): A decorator that logs registration, execution, and completion times of a function.
 - [`utils.disable_children`](./utils.utils.md#function-disable_children): Recursively walk the provided thing and disable all of its widget children.
 - [`utils.enable_children`](./utils.utils.md#function-enable_children): Recursively walk the provided thing and enable all of its widget children.
 - [`utils.get_children`](./utils.utils.md#function-get_children): Recursively visit all the children of the specified object and collect them in a list.
 - [`utils.print_children`](./utils.utils.md#function-print_children): Recursively visit all the children of the specified object and print them.
 - [`utils.set_font_options`](./utils.utils.md#function-set_font_options): Set the QFont options of the specified object.
```

### Comparing `qtstrap-0.5.3/docs/api/settings.md` & `qtstrap-0.6.0/docs/api/settings.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/api/utils.decorators.md` & `qtstrap-0.6.0/docs/api/utils.defer.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\decorators.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\defer.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+# <kbd>module</kbd> `utils.defer`
 
-# <kbd>module</kbd> `utils.decorators`
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\decorators.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\defer.py#L1"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `Defer`
+A context manager that emulates the defer keyword from other languages. 
+
+The deferred thing can be any callable, and arbitrary args and kwargs will be preserved and passed to the thing during __exit__(). 
+
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\defer.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>function</kbd> `trace`
+### <kbd>method</kbd> `Defer.__init__`
 
 ```python
-trace(func)
+__init__(thing, *args, **kwargs)
 ```
 
 
 
 
 
 
 
+
+
+
 
 ---
 
 _This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

#### html2text {}

```diff
@@ -1,5 +1,9 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`utils.decorators` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## function `trace` ```python trace(func) ``` --- _This file was
-automatically generated via [lazydocs](https://github.com/ml-tooling/
+`utils.defer` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]## class `Defer` A context manager that emulates the defer keyword from
+other languages. The deferred thing can be any callable, and arbitrary args and
+kwargs will be preserved and passed to the thing during __exit__(). _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`Defer.__init__` ```python __init__(thing, *args, **kwargs) ``` --- _This file
+was automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/utils.defer.md` & `qtstrap-0.6.0/docs/api/utils.signals.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\defer.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\signals.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `utils.defer`
+# <kbd>module</kbd> `utils.signals`
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\defer.py#L1"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\signals.py#L1"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `Defer`
-A context manager that emulates the defer keyword from other languages. 
+## <kbd>class</kbd> `SignalBlocker`
+A context manager that blocks the signals of the provided widget. 
 
-The deferred thing can be any callable, and arbitrary args and kwargs will be preserved and passed to the thing during __exit__(). 
+The signals are unblocked at the end of the with block. 
 
-<a href="..\..\qtstrap\utils\defer.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\signals.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `Defer.__init__`
+### <kbd>method</kbd> `SignalBlocker.__init__`
 
 ```python
-__init__(thing, *args, **kwargs)
+__init__(widget)
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`utils.defer` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## class `Defer` A context manager that emulates the defer keyword from
-other languages. The deferred thing can be any callable, and arbitrary args and
-kwargs will be preserved and passed to the thing during __exit__(). _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`Defer.__init__` ```python __init__(thing, *args, **kwargs) ``` --- _This file
-was automatically generated via [lazydocs](https://github.com/ml-tooling/
+`utils.signals` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]## class `SignalBlocker` A context manager that blocks the signals of
+the provided widget. The signals are unblocked at the end of the with block.
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`SignalBlocker.__init__` ```python __init__(widget) ``` --- _This file was
+automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/utils.drag_and_drop.md` & `qtstrap-0.6.0/docs/api/utils.drag_and_drop.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\drag_and_drop.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\drag_and_drop.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `utils.drag_and_drop`
 
 
 
 
 **Global Variables**
@@ -13,50 +13,50 @@
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 ---
 
-<a href="..\..\qtstrap\utils\drag_and_drop.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\drag_and_drop.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `accepts_file_drops`
 
 ```python
 accepts_file_drops(extensions: 'str | [str]')
 ```
 
 Decorator that enables drag-and-drop on a QWidget. Accepts a str or a list of strings of the valid file extensions. 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\drag_and_drop.py#L48"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\drag_and_drop.py#L48"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `draggable`
 
 ```python
 draggable(target)
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\drag_and_drop.py#L91"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\drag_and_drop.py#L91"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PreviewDrag`
 
 
 
 
-<a href="..\..\qtstrap\utils\drag_and_drop.py#L92"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\drag_and_drop.py#L92"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PreviewDrag.__init__`
 
 ```python
 __init__(source, mimedata=None)
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/utils.get_ip.md` & `qtstrap-0.6.0/docs/api/utils.call_later.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\get_ip.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\call_later.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `utils.get_ip`
+# <kbd>module</kbd> `utils.call_later`
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\get_ip.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\call_later.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>function</kbd> `get_ip`
+## <kbd>function</kbd> `call_later`
 
 ```python
-get_ip()
+call_later(what, msec: int = 1)
 ```
 
-Get the current machine's IPv4 address. 
-
-This process is more complicated than it appears because of the possiblity of multiple arbitrary network interfaces. 
+call the given function after a specified delay 
 
 
 
 
 ---
 
 _This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

#### html2text {}

```diff
@@ -1,7 +1,6 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`utils.get_ip` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## function `get_ip` ```python get_ip() ``` Get the current machine's
-IPv4 address. This process is more complicated than it appears because of the
-possiblity of multiple arbitrary network interfaces. --- _This file was
+`utils.call_later` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]## function `call_later` ```python call_later(what, msec: int = 1) ```
+call the given function after a specified delay --- _This file was
 automatically generated via [lazydocs](https://github.com/ml-tooling/
 lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/utils.string_builder.md` & `qtstrap-0.6.0/docs/api/utils.string_builder.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\string_builder.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\string_builder.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `utils.string_builder`
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\string_builder.py#L3"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\string_builder.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `Builder`
 Utility class for incrementally building strings. 
 
-<a href="..\..\qtstrap\utils\string_builder.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\string_builder.py#L9"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Builder.__init__`
 
 ```python
-__init__(out=None, indent=4)
+__init__(
+    out: Optional[Callable[[str], NoneType]] = None,
+    indent: int = 4,
+    endl: str = '\n'
+)
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\string_builder.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\string_builder.py#L37"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Builder.join`
 
 ```python
-join(base: str)
+join(base: str = '')
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\string_builder.py#L19"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\string_builder.py#L31"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `Builder.line`
 
 ```python
-line(string='')
+line(string: str = '')
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
 `utils.string_builder` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `Builder` Utility class for incrementally
 building strings. _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `Builder.__init__` ```python __init__(out=None, indent=4) ```
---- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`Builder.join` ```python join(base: str) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Builder.line` ```python line
-(string='') ``` --- _This file was automatically generated via [lazydocs]
-(https://github.com/ml-tooling/lazydocs)._
+_s_q_u_a_r_e_]### method `Builder.__init__` ```python __init__( out: Optional[Callable
+[[str], NoneType]] = None, indent: int = 4, endl: str = '\n' ) ``` --- _[_h_t_t_p_s_:_/
+_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`Builder.join` ```python join(base: str = '') ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Builder.line` ```python line
+(string: str = '') ``` --- _This file was automatically generated via
+[lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/utils.timestamp.md` & `qtstrap-0.6.0/docs/api/widgets.link_label.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,85 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\timestamp.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\link_label.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `utils.timestamp`
+# <kbd>module</kbd> `widgets.link_label`
 
 
 
 
+**Global Variables**
+---------------
+- **TYPE_CHECKING**
+- **PYQT6**
+- **PYQT5**
+- **PYSIDE2**
+- **PYSIDE6**
 
----
 
-<a href="..\..\qtstrap\utils\timestamp.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+---
 
-## <kbd>function</kbd> `time_since`
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\link_label.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-```python
-time_since(timestamp)
-```
+## <kbd>class</kbd> `LinkLabel`
 
 
 
 
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\link_label.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `LinkLabel.__init__`
 
----
+```python
+__init__(text='', link='', both=None, parent=None)
+```
 
-<a href="..\..\qtstrap\utils\timestamp.py#L8"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `TimeStamp`
 
 
 
 
-<a href="..\..\qtstrap\utils\timestamp.py#L9"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `TimeStamp.__init__`
 
-```python
-__init__()
-```
+---
 
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\link_label.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `LinkLabel.setBoth`
 
+```python
+setBoth(value)
+```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\timestamp.py#L12"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\link_label.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `TimeStamp.time_since`
+### <kbd>method</kbd> `LinkLabel.setLink`
 
 ```python
-time_since(timestamp=None)
+setLink(link)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\timestamp.py#L21"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\link_label.py#L20"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `TimeStamp.update`
+### <kbd>method</kbd> `LinkLabel.setText`
 
 ```python
-update()
+setText(text)
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`utils.timestamp` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## function `time_since` ```python time_since(timestamp) ``` --- _[_h_t_t_p_s_:
-_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `TimeStamp`
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`TimeStamp.__init__` ```python __init__() ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `TimeStamp.time_since`
-```python time_since(timestamp=None) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `TimeStamp.update` ```python update
-() ``` --- _This file was automatically generated via [lazydocs](https://
-github.com/ml-tooling/lazydocs)._
+`widgets.link_label` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `LinkLabel` _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`LinkLabel.__init__` ```python __init__(text='', link='', both=None,
+parent=None) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `LinkLabel.setBoth` ```python setBoth(value) ``` --- _[_h_t_t_p_s_:_/
+_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`LinkLabel.setLink` ```python setLink(link) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `LinkLabel.setText` ```python
+setText(text) ``` --- _This file was automatically generated via [lazydocs]
+(https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/utils.trace.md` & `qtstrap-0.6.0/docs/api/extras.style.dark_palette.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\trace.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\style\dark_palette.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `utils.trace`
+# <kbd>module</kbd> `extras.style.dark_palette`
 
 
 
 
 **Global Variables**
 ---------------
-- **start_time**
+- **TYPE_CHECKING**
+- **PYQT6**
+- **PYQT5**
+- **PYSIDE2**
+- **PYSIDE6**
 
 ---
 
-<a href="..\..\qtstrap\utils\trace.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\extras\style\dark_palette.py#L47"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>function</kbd> `trace`
+## <kbd>function</kbd> `install_dark_palette`
 
 ```python
-trace(func)
+install_dark_palette(app)
 ```
```

#### html2text {}

```diff
@@ -1,5 +1,7 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`utils.trace` **Global Variables** --------------- - **start_time** --- _[_h_t_t_p_s_:
-_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `trace`
-```python trace(func) ``` --- _This file was automatically generated via
-[lazydocs](https://github.com/ml-tooling/lazydocs)._
+`extras.style.dark_palette` **Global Variables** --------------- -
+**TYPE_CHECKING** - **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** ---
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function
+`install_dark_palette` ```python install_dark_palette(app) ``` --- _This file
+was automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/utils.utils.md` & `qtstrap-0.6.0/docs/api/utils.utils.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\utils\utils.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\utils.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `utils.utils`
 
 
 
 
 **Global Variables**
@@ -13,72 +13,72 @@
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 ---
 
-<a href="..\..\qtstrap\utils\utils.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\utils.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `enable_children`
 
 ```python
-enable_children(thing: PySide2.QtCore.QObject) → None
+enable_children(thing: PySide6.QtCore.QObject) → None
 ```
 
 Recursively walk the provided thing and enable all of its widget children. 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\utils.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\utils.py#L23"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `disable_children`
 
 ```python
-disable_children(thing: PySide2.QtCore.QObject) → None
+disable_children(thing: PySide6.QtCore.QObject) → None
 ```
 
 Recursively walk the provided thing and disable all of its widget children. 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\utils.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\utils.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `get_children`
 
 ```python
-get_children(obj: PySide2.QtCore.QObject) → list
+get_children(obj: PySide6.QtCore.QObject) → list
 ```
 
 Recursively visit all the children of the specified object and collect them in a list. 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\utils.py#L58"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\utils.py#L58"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `print_children`
 
 ```python
-print_children(obj: PySide2.QtCore.QObject, prefix='') → None
+print_children(obj: PySide6.QtCore.QObject, prefix='') → None
 ```
 
 Recursively visit all the children of the specified object and print them. 
 
 
 ---
 
-<a href="..\..\qtstrap\utils\utils.py#L67"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\utils.py#L67"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>function</kbd> `set_font_options`
 
 ```python
-set_font_options(obj: PySide2.QtCore.QObject, options={})
+set_font_options(obj: PySide6.QtCore.QObject, options={})
 ```
 
 Set the QFont options of the specified object. Font options are specified by providing the name of the QFont setter method. 
 
 
 
 **Example:**
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
 `utils.utils` **Global Variables** --------------- - **TYPE_CHECKING** -
 **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `enable_children` ```python
-enable_children(thing: PySide2.QtCore.QObject) â None ``` Recursively walk
+enable_children(thing: PySide6.QtCore.QObject) â None ``` Recursively walk
 the provided thing and enable all of its widget children. --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function
-`disable_children` ```python disable_children(thing: PySide2.QtCore.QObject)
+`disable_children` ```python disable_children(thing: PySide6.QtCore.QObject)
 â None ``` Recursively walk the provided thing and disable all of its widget
 children. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]##
-function `get_children` ```python get_children(obj: PySide2.QtCore.QObject) â
+function `get_children` ```python get_children(obj: PySide6.QtCore.QObject) â
 list ``` Recursively visit all the children of the specified object and collect
 them in a list. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]## function `print_children` ```python print_children(obj:
-PySide2.QtCore.QObject, prefix='') â None ``` Recursively visit all the
+PySide6.QtCore.QObject, prefix='') â None ``` Recursively visit all the
 children of the specified object and print them. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## function `set_font_options` ```python
-set_font_options(obj: PySide2.QtCore.QObject, options={}) ``` Set the QFont
+set_font_options(obj: PySide6.QtCore.QObject, options={}) ``` Set the QFont
 options of the specified object. Font options are specified by providing the
 name of the QFont setter method. **Example:** set_font_options(widget,
 {'setPointSize': 12, 'setBold': True}) is equivalent to writing: font =
 widget.font() font.setPointSize(12) font.setBold(True) widget.setFont(font) --
 - _This file was automatically generated via [lazydocs](https://github.com/ml-
 tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.labeledit.md` & `qtstrap-0.6.0/docs/api/widgets.labeledit.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `widgets.labeledit`
 
 
 
 
 **Global Variables**
@@ -14,22 +14,22 @@
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `LabelEdit`
 
 
 
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L7"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.__init__`
 
 ```python
 __init__(text, *args, changed=None, **kwargs)
 ```
 
@@ -38,99 +38,99 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.accept`
 
 ```python
 accept()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.dismiss`
 
 ```python
 dismiss()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L45"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L45"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.eventFilter`
 
 ```python
 eventFilter(source, event)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L34"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L34"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.mouseDoubleClickEvent`
 
 ```python
-mouseDoubleClickEvent(event: PySide2.QtGui.QMouseEvent) → None
+mouseDoubleClickEvent(event: PySide6.QtGui.QMouseEvent) → None
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.setText`
 
 ```python
 setText(text)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L29"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L29"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.start_editing`
 
 ```python
 start_editing()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\labeledit.py#L22"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\labeledit.py#L22"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `LabelEdit.text`
 
 ```python
 text()
 ```
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
 method `LabelEdit.accept` ```python accept() ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `LabelEdit.dismiss` ```python
 dismiss() ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### method `LabelEdit.eventFilter` ```python eventFilter(source, event)
 ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
 method `LabelEdit.mouseDoubleClickEvent` ```python mouseDoubleClickEvent(event:
-PySide2.QtGui.QMouseEvent) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
+PySide6.QtGui.QMouseEvent) â None ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
 _s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `LabelEdit.setText` ```python
 setText(text) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### method `LabelEdit.start_editing` ```python start_editing() ``` ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `LabelEdit.text` ```python text() ``` --- _This file was automatically
 generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.line_widgets.md` & `qtstrap-0.6.0/docs/api/utils.adapter.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\adapter.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `widgets.line_widgets`
+# <kbd>module</kbd> `utils.adapter`
 
 
 
 
-**Global Variables**
----------------
-- **TYPE_CHECKING**
-- **PYQT6**
-- **PYQT5**
-- **PYSIDE2**
-- **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\adapter.py#L10"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `VLine`
+## <kbd>class</kbd> `Adapter`
 
 
 
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\adapter.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `VLine.__init__`
+### <kbd>method</kbd> `Adapter.__init__`
 
 ```python
-__init__(parent=None, line_width=1)
+__init__(other=None)
 ```
 
 
 
 
 
 
 
 
-
 ---
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\adapter.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `HLine`
+### <kbd>method</kbd> `Adapter.adapter`
 
+```python
+adapter()
+```
 
 
 
-<a href="..\..\qtstrap\widgets\line_widgets.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `HLine.__init__`
 
-```python
-__init__(parent=None, line_width=1)
-```
+---
 
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\utils\adapter.py#L57"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `Adapter.kill`
 
+```python
+kill()
+```
```

#### html2text {}

```diff
@@ -1,11 +1,9 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`widgets.line_widgets` **Global Variables** --------------- - **TYPE_CHECKING**
-- **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `VLine` _[_h_t_t_p_s_:_/
-_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`VLine.__init__` ```python __init__(parent=None, line_width=1) ``` --- _[_h_t_t_p_s_:_/
-_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `HLine` _[_h_t_t_p_s_:
-_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`HLine.__init__` ```python __init__(parent=None, line_width=1) ``` --- _This
-file was automatically generated via [lazydocs](https://github.com/ml-tooling/
-lazydocs)._
+`utils.adapter` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]## class `Adapter` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Adapter.__init__` ```python __init__
+(other=None) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `Adapter.adapter` ```python adapter() ``` --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `Adapter.kill`
+```python kill() ``` --- _This file was automatically generated via [lazydocs]
+(https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.link_label.md` & `qtstrap-0.6.0/docs/api/widgets.toolbar.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,58 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\link_label.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\toolbar.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `widgets.link_label`
+# <kbd>module</kbd> `widgets.toolbar`
 
 
 
 
 **Global Variables**
 ---------------
 - **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
+- **location_map**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\link_label.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\toolbar.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `LinkLabel`
+## <kbd>class</kbd> `BaseToolbar`
 
 
 
 
-<a href="..\..\qtstrap\widgets\link_label.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\toolbar.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `LinkLabel.__init__`
+### <kbd>method</kbd> `BaseToolbar.__init__`
 
 ```python
-__init__(text='', link='', both=None, parent=None)
+__init__(parent=None, name=None, location=None, size=40, **kwargs)
 ```
 
 
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\link_label.py#L28"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\toolbar.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `LinkLabel.setBoth`
+### <kbd>method</kbd> `BaseToolbar.add_spacer`
 
 ```python
-setBoth(value)
-```
-
-
-
-
-
----
-
-<a href="..\..\qtstrap\widgets\link_label.py#L24"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-### <kbd>method</kbd> `LinkLabel.setLink`
-
-```python
-setLink(link)
-```
-
-
-
-
-
----
-
-<a href="..\..\qtstrap\widgets\link_label.py#L20"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-### <kbd>method</kbd> `LinkLabel.setText`
-
-```python
-setText(text)
+add_spacer()
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,10 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`widgets.link_label` **Global Variables** --------------- - **TYPE_CHECKING** -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `LinkLabel` _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`LinkLabel.__init__` ```python __init__(text='', link='', both=None,
-parent=None) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `LinkLabel.setBoth` ```python setBoth(value) ``` --- _[_h_t_t_p_s_:_/
-_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`LinkLabel.setLink` ```python setLink(link) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `LinkLabel.setText` ```python
-setText(text) ``` --- _This file was automatically generated via [lazydocs]
-(https://github.com/ml-tooling/lazydocs)._
+`widgets.toolbar` **Global Variables** --------------- - **TYPE_CHECKING** -
+**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **location_map** ---
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
+`BaseToolbar` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `BaseToolbar.__init__` ```python __init__(parent=None,
+name=None, location=None, size=40, **kwargs) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `BaseToolbar.add_spacer`
+```python add_spacer() ``` --- _This file was automatically generated via
+[lazydocs](https://github.com/ml-tooling/lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.md` & `qtstrap-0.6.0/docs/api/widgets.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\__init__.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\__init__.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `widgets`
 
 
 
 
 **Global Variables**
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.persistent_tab_widget.md` & `qtstrap-0.6.0/docs/api/widgets.persistent_tab_widget.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `widgets.persistent_tab_widget`
 
 
 
 
 **Global Variables**
@@ -14,22 +14,22 @@
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentTabWidget`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.__init__`
 
 ```python
 __init__(name, tabs=None, *args, **kwargs)
 ```
 
@@ -38,99 +38,99 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L87"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L89"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.close_tab`
 
 ```python
 close_tab(index)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L30"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L30"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.menu`
 
 ```python
 menu(pos) → None
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L84"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L86"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.move_tab`
 
 ```python
 move_tab(old, new)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.restore_state`
 
 ```python
 restore_state(tabs=None)
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L72"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.tab_order`
 
 ```python
 tab_order()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L35"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.unhide_all`
 
 ```python
 unhide_all()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_tab_widget.py#L78"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_tab_widget.py#L80"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTabWidget.visible_tabs`
 
 ```python
 visible_tabs()
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.persistent_widgets.md` & `qtstrap-0.6.0/docs/api/widgets.persistent_widgets.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 # <kbd>module</kbd> `widgets.persistent_widgets`
 
 
 
 
 **Global Variables**
@@ -14,22 +14,22 @@
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentCheckBox`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCheckBox.__init__`
 
 ```python
 __init__(name, changed=None, *args, **kwargs)
 ```
 
@@ -38,37 +38,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L15"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L15"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCheckBox.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L26"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L26"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentLineEdit`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentLineEdit.__init__`
 
 ```python
 __init__(name, *args, default='', changed=None, **kwargs)
 ```
 
@@ -77,37 +77,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L38"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentLineEdit.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L42"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentTextEdit`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTextEdit.__init__`
 
 ```python
 __init__(name, *args, default='', changed=None, **kwargs)
 ```
 
@@ -116,37 +116,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTextEdit.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L58"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L58"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentPlainTextEdit`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L59"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L59"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentPlainTextEdit.__init__`
 
 ```python
 __init__(name, *args, default='', changed=None, **kwargs)
 ```
 
@@ -155,37 +155,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L70"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L70"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentPlainTextEdit.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentListWidget`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentListWidget.__init__`
 
 ```python
 __init__(name, items=[], default=[], changed=None, *args, **kwargs)
 ```
 
@@ -194,51 +194,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L92"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L92"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentListWidget.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L89"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L89"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentListWidget.selected_items`
 
 ```python
 selected_items()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L100"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentTreeWidget`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L101"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L101"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTreeWidget.__init__`
 
 ```python
 __init__(
     name,
     items=[],
@@ -255,51 +255,51 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L119"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L119"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTreeWidget.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentTreeWidget.selected_items`
 
 ```python
 selected_items()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L127"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L127"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentComboBox`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L128"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L128"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentComboBox.__init__`
 
 ```python
 __init__(name, items=[], changed=None, *args, **kwargs)
 ```
 
@@ -308,37 +308,37 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L141"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L141"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentComboBox.restore_state`
 
 ```python
 restore_state()
 ```
 
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L147"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L147"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `PersistentCheckableAction`
 
 
 
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L148"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L148"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCheckableAction.__init__`
 
 ```python
 __init__(name, *args, **kwargs)
 ```
 
@@ -347,15 +347,15 @@
 
 
 
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\persistent_widgets.py#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\persistent_widgets.py#L156"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `PersistentCheckableAction.restore_state`
 
 ```python
 restore_state()
 ```
```

### Comparing `qtstrap-0.5.3/docs/api/widgets.toolbar.md` & `qtstrap-0.6.0/docs/api/widgets.line_widgets.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 <!-- markdownlint-disable -->
 
-<a href="..\..\qtstrap\widgets\toolbar.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\line_widgets.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `widgets.toolbar`
+# <kbd>module</kbd> `widgets.line_widgets`
 
 
 
 
 **Global Variables**
 ---------------
 - **TYPE_CHECKING**
 - **PYQT6**
 - **PYQT5**
 - **PYSIDE2**
 - **PYSIDE6**
-- **location_map**
 
 
 ---
 
-<a href="..\..\qtstrap\widgets\toolbar.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\line_widgets.py#L4"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `BaseToolbar`
+## <kbd>class</kbd> `VLine`
 
 
 
 
-<a href="..\..\qtstrap\widgets\toolbar.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\line_widgets.py#L5"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `BaseToolbar.__init__`
+### <kbd>method</kbd> `VLine.__init__`
 
 ```python
-__init__(parent=None, name=None, location=None, size=40, **kwargs)
+__init__(parent=None, line_width=1)
 ```
 
 
 
 
 
 
 
 
+
 ---
 
-<a href="..\..\qtstrap\widgets\toolbar.py#L27"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\line_widgets.py#L13"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `HLine`
+
+
+
 
-### <kbd>method</kbd> `BaseToolbar.add_spacer`
+<a href="https://github.com/qtstrap/qtstrap/blob/master\qtstrap\widgets\line_widgets.py#L14"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `HLine.__init__`
 
 ```python
-add_spacer()
+__init__(parent=None, line_width=1)
 ```
 
 
 
 
 
 
 
+
+
+
 
 ---
 
 _This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`widgets.toolbar` **Global Variables** --------------- - **TYPE_CHECKING** -
-**PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** - **location_map** ---
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
-`BaseToolbar` _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `BaseToolbar.__init__` ```python __init__(parent=None,
-name=None, location=None, size=40, **kwargs) ``` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `BaseToolbar.add_spacer`
-```python add_spacer() ``` --- _This file was automatically generated via
-[lazydocs](https://github.com/ml-tooling/lazydocs)._
+`widgets.line_widgets` **Global Variables** --------------- - **TYPE_CHECKING**
+- **PYQT6** - **PYQT5** - **PYSIDE2** - **PYSIDE6** --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `VLine` _[_h_t_t_p_s_:_/
+_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`VLine.__init__` ```python __init__(parent=None, line_width=1) ``` --- _[_h_t_t_p_s_:_/
+_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `HLine` _[_h_t_t_p_s_:
+_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`HLine.__init__` ```python __init__(parent=None, line_width=1) ``` --- _This
+file was automatically generated via [lazydocs](https://github.com/ml-tooling/
+lazydocs)._
```

### Comparing `qtstrap-0.5.3/docs/extras/code_editor.md` & `qtstrap-0.6.0/docs/extras/code_editor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/extras/command_palette.md` & `qtstrap-0.6.0/docs/extras/command_palette.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/extras/log_monitor.md` & `qtstrap-0.6.0/docs/extras/log_monitor.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/index.md` & `qtstrap-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/quickstart/baseapplication.md` & `qtstrap-0.6.0/docs/quickstart/baseapplication.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/quickstart/basemainwindow.md` & `qtstrap-0.6.0/docs/quickstart/basemainwindow.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/quickstart/context_layouts.md` & `qtstrap-0.6.0/docs/quickstart/context_layouts.md`

 * *Files 21% similar despite different names*

```diff
@@ -43,8 +43,60 @@
     with layout.hbox():
         layout.add(button3)
         layout.add(button4)
 ```
 
 All of the backtracking and repetition is gone. The pointless effort of naming each layout is gone. The indentation helps show the structure of the layout.
 
-The top level `CVBoxLayout` adds itself to its parent correctly and automatically. The `.add()` method can handle a layout or a widget or even a mixed list of both.
+The top level `CVBoxLayout` adds itself to its parent correctly and automatically. The `.add()` method can handle a layout or a widget or even a mixed list of both.
+
+The `.add()` method also returns the item you give it, which allows us to remove even more duplication in some situations:
+
+```py
+# note that a with block does not create a new scope
+with CHBoxLayout(QWidget()) as layout:
+    button1 = layout.add(QPushButton("One"))
+    button2 = layout.add(QPushButton("Two"))
+
+# so these references are available after the with block closes
+print(button1) 
+```
+
+Context layouts also support more advanced usages:
+
+```py
+with CVBoxLayout(QWidget()) as layout:
+    # supports '+='
+    layout += QLabel('Title') 
+    # supports '+', which returns the added widget
+    button1 = layout + QPushButton("One")
+    # All add() methods also support lists and tuples of widgets
+    button2, button3 = layout.add((QPushButton("Two"), QPushButton("Three")))
+    button4, button5 = layout + [QPushButton("Four"), QPushButton("Five")]
+```
+
+# Advanced Layouts
+
+Other Qt layout types are supported:
+
+- Forms:
+    ```py
+    with CFormLayout(QWidget()) as layout:
+        layout.add('label', QPushButton(''))
+        layout += ['label', QPushButton('')]
+        layout += {
+            'label': QPushButton(''),
+            'label': QPushButton(''),
+        }
+    ```
+- Splitters:
+    ```py
+    with CSplitter(QWidget()) as split:
+        # coming soon
+        pass
+    ```
+- Scroll Areas:
+    ```py
+    with CScrollArea(QWidget()) as layout:
+        # coming soon
+        pass
+    ```
```

### Comparing `qtstrap-0.5.3/docs/quickstart/gettingstarted.md` & `qtstrap-0.6.0/docs/quickstart/gettingstarted.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/quickstart/installation.md` & `qtstrap-0.6.0/docs/quickstart/installation.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # New Projects: 
 This is the recommended way to create a new project using qtstrap:
 ```sh
 $ mkdir test && cd test
 $ python3 -m venv .venv
 $ source .venv/bin/activate
-$ python3 -m pip install qtstrap PySide2
+$ python3 -m pip install qtstrap PySide6
 $ qtstrap init
 ```
 
 The init script will prompt you to enter the name of your application and the name of its publisher(which is probably you), and then it will generate an application skeleton. At this point you can deactivate the virtual environment and forget it exists(until you need to add a package or something).
 
 You can test that everything installed properly by executing:
 ```sh
```

### Comparing `qtstrap-0.5.3/docs/reference/base_application.md` & `qtstrap-0.6.0/docs/reference/base_application.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/base_window.md` & `qtstrap-0.6.0/docs/reference/base_window.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/options.md` & `qtstrap-0.6.0/docs/reference/options.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/toolbar.md` & `qtstrap-0.6.0/docs/reference/toolbar.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/utils.adapter.md` & `qtstrap-0.6.0/docs/reference/utils.adapter.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/utils.defer.md` & `qtstrap-0.6.0/docs/reference/utils.defer.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/utils.signals.md` & `qtstrap-0.6.0/docs/reference/utils.signals.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/utils.timestamp.md` & `qtstrap-0.6.0/docs/reference/utils.timestamp.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/utils.utils.md` & `qtstrap-0.6.0/docs/reference/utils.utils.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.buttons.md` & `qtstrap-0.6.0/docs/reference/widgets.buttons.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.labeledit.md` & `qtstrap-0.6.0/docs/reference/widgets.labeledit.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.layouts.md` & `qtstrap-0.6.0/docs/reference/widgets.layouts.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.line_widgets.md` & `qtstrap-0.6.0/docs/reference/widgets.line_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.link_label.md` & `qtstrap-0.6.0/docs/reference/widgets.link_label.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.md` & `qtstrap-0.6.0/docs/reference/widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.persistent_tab_widget.md` & `qtstrap-0.6.0/docs/reference/widgets.persistent_tab_widget.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/reference/widgets.persistent_widgets.md` & `qtstrap-0.6.0/docs/reference/widgets.persistent_widgets.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/screenshot1.png` & `qtstrap-0.6.0/docs/screenshot1.png`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/structure/makefile.md` & `qtstrap-0.6.0/docs/structure/makefile.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/structure/structure.md` & `qtstrap-0.6.0/docs/structure/structure.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/docs/test.md` & `qtstrap-0.6.0/docs/test.md`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/mkdocs.yml` & `qtstrap-0.6.0/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 site_name: qtstrap
 site_description: 'Like Bootstrap, but Qt-er!'
 site_author: 'David Kincaid'
 docs_dir: docs/
 repo_name: 'qtstrap/qtstrap'
 repo_url: 'https://github.com/qtstrap/qtstrap'
 theme:
-    name: readthedocs
+  name: readthedocs
+  custom_dir: docs_theme/
 plugins:
   - search
   - mermaid2
   - literate-nav
 
 nav:
   - Overview:
```

### Comparing `qtstrap-0.5.3/qtstrap/__init__.py` & `qtstrap-0.6.0/qtstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/__main__.py` & `qtstrap-0.6.0/qtstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/base_application.py` & `qtstrap-0.6.0/qtstrap/base_application.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/base_window.py` & `qtstrap-0.6.0/qtstrap/base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/code_editor/code_editor.py` & `qtstrap-0.6.0/qtstrap/extras/code_editor/code_editor.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/code_editor/code_line.py` & `qtstrap-0.6.0/qtstrap/extras/code_editor/code_line.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/code_editor/highlighters/python.py` & `qtstrap-0.6.0/qtstrap/extras/code_editor/highlighters/python.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/command_palette/command_palette.py` & `qtstrap-0.6.0/qtstrap/extras/command_palette/command_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/log_monitor/__init__.py` & `qtstrap-0.6.0/qtstrap/extras/log_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/log_monitor/log_database_handler.py` & `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_database_handler.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/log_monitor/log_filter_controls.py` & `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_filter_controls.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/log_monitor/log_profile.py` & `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_profile.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/log_monitor/log_table_view.py` & `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_table_view.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/log_monitor/log_widget.py` & `qtstrap-0.6.0/qtstrap/extras/log_monitor/log_widget.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/settings_model/settings_model.py` & `qtstrap-0.6.0/qtstrap/extras/settings_model/settings_model.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/style/colors.py` & `qtstrap-0.6.0/qtstrap/extras/style/colors.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/style/dark_palette.py` & `qtstrap-0.6.0/qtstrap/extras/style/dark_palette.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/extras/style/themes.py` & `qtstrap-0.6.0/qtstrap/extras/style/themes.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/options.py` & `qtstrap-0.6.0/qtstrap/options.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/qt.py` & `qtstrap-0.6.0/qtstrap/qt.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/Makefile` & `qtstrap-0.6.0/qtstrap/template/Makefile`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/app/main.py` & `qtstrap-0.6.0/qtstrap/template/app/main.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/app/resources/application.ico` & `qtstrap-0.6.0/qtstrap/template/app/resources/application.ico`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/app/resources/icon.svg` & `qtstrap-0.6.0/qtstrap/template/app/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/scripts/bundle.spec` & `qtstrap-0.6.0/qtstrap/template/scripts/bundle.spec`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/scripts/installer.iss` & `qtstrap-0.6.0/qtstrap/template/scripts/installer.iss`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/template/scripts/onefile.spec` & `qtstrap-0.6.0/qtstrap/template/scripts/onefile.spec`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/utils/adapter.py` & `qtstrap-0.6.0/qtstrap/utils/adapter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qtstrap import QObject
-
+from qtpy.QtCore import SIGNAL
 
 try:
     from qtstrap import SignalInstance
 except:
     from qtstrap import pyqtBoundSignal as SignalInstance
 
 
@@ -53,28 +53,32 @@
 
     def adapter(self):
         return self.__class__(self)
 
     def kill(self):
         if self._other:
             for name in self._get_signals(self._other):
-                # TODO: this might not be safe
-                getattr(self._other, name).disconnect(getattr(self, name).emit)
+                self.disconnect(self._other, SIGNAL(name), getattr(self, name).emit)
+            #     # TODO: this might not be safe
+            #     getattr(self._other, name).disconnect(getattr(self, name).emit)
 
 
 if __name__ == '__main__':
     from qtstrap import Signal
 
-    class Example(QObject):
-        class SignalInterface(Adapter):
-            signal1 = Signal()
-            signal2 = Signal(str)
-
-        def __init__(self):
-            super().__init__()
-            self.interface = self.SignalInterface()
+    class SignalInterface(Adapter):
+        sig = Signal()
+
+    original = SignalInterface()
+    original.sig.connect(lambda: print('original'))
+
+    copy = original.adapter()
+    copy.sig.connect(lambda: print('copy'))
+
+    original.sig.emit()
+
+    copy.kill()
 
-    ex = Example()
-    adapter = ex.interface.adapter()
+    original.sig.emit()
 
-    print(ex.interface)
-    print(adapter)
+    print(original)
+    print(copy)
```

### Comparing `qtstrap-0.5.3/qtstrap/utils/defer.py` & `qtstrap-0.6.0/qtstrap/utils/defer.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/utils/drag_and_drop.py` & `qtstrap-0.6.0/qtstrap/utils/drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/utils/get_ip.py` & `qtstrap-0.6.0/qtstrap/utils/get_ip.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/utils/string_builder.py` & `qtstrap-0.6.0/qtstrap/utils/string_builder.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/utils/timestamp.py` & `qtstrap-0.6.0/qtstrap/utils/timestamp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from time import time
 
 
-def time_since(timestamp):
-    return time() - timestamp
-
-
 class TimeStamp:
-    def __init__(self):
-        self._time = time()
+    """A TimeStamp object that can be used to track the time since it was created."""
 
-    def time_since(self, timestamp=None):
-        if timestamp is None:
-            return time() - self._time
+    def __init__(self) -> None:
+        self._time = time()
 
-        if type(timestamp) == TimeStamp():
-            return time() - timestamp._time
+    def time_since(self) -> float:
+        """Calculate the elapsed time since this TimeStamp was created or updated."""
+        return time() - self._time
 
-        return time() - timestamp
-
-    def update(self):
+    def update(self) -> None:
+        """Update the TimeStamp to the current time."""
         self._time = time()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self._time)
+
+
+def time_since(timestamp: TimeStamp | float) -> float:
+    """Calculate the elapsed time since the given TimeStamp or time value."""
+    if isinstance(timestamp, TimeStamp):
+        return time() - timestamp._time
+    else:
+        return time() - timestamp
```

### Comparing `qtstrap-0.5.3/qtstrap/utils/utils.py` & `qtstrap-0.6.0/qtstrap/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/__init__.py` & `qtstrap-0.6.0/qtstrap/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/buttons.py` & `qtstrap-0.6.0/qtstrap/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/labeledit.py` & `qtstrap-0.6.0/qtstrap/widgets/labeledit.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/layouts.py` & `qtstrap-0.6.0/qtstrap/widgets/layouts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeAlias, Literal
+from typing import TypeAlias, Literal, Sequence
 from qtpy.QtCore import (
     Qt,
     QSettings,
     QMargins,
 )
 from qtpy.QtWidgets import (
     QMainWindow,
@@ -75,16 +75,16 @@
 )
 
 MarginsType: TypeAlias = QMargins | tuple | int | None
 
 
 class ContextLayoutBase:
     def add(
-        self, item: QWidget | QLayout | list[QWidget | QLayout], *args, **kwargs
-    ) -> QWidget | QLayout | list[QWidget | QLayout]:
+        self, item: QWidget | QLayout | Sequence[QWidget | QLayout], *args, **kwargs
+    ) -> QWidget | QLayout | Sequence[QWidget | QLayout]:
         return item
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
@@ -125,15 +125,15 @@
                 self.setContentsMargins(*margins)
             elif isinstance(margins, int):
                 self.setContentsMargins(margins, margins, margins, margins)
 
         if align in alignments:
             self.setAlignment(alignments[align])
 
-        self._stack: list[ContextLayoutBase] = []
+        self._stack: Sequence[ContextLayoutBase] = []
         self.next_layout: ContextLayoutBase | None = None
 
     def __getattr__(self, name: str):
         return getattr(self._layout, name)
 
     @property
     def _layout(self):
@@ -141,32 +141,39 @@
         if len(self._stack) > 0:
             layout = self._stack[len(self._stack) - 1]
         return layout
 
     def __call__(self):
         return self._layout
 
+    def __add__(
+        self,
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
+    ) -> QWidget | QLayout | Sequence[QWidget | QLayout]:
+        self.add(item)
+        return item
+
     def __iadd__(
         self,
-        item: QWidget | QLayout | list[QWidget | QLayout],
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
     ):
         self.add(item)
         return self
 
     def add(
         self,
-        item: QWidget | QLayout | list[QWidget | QLayout],
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
         *args,
         **kwargs,
-    ) -> QWidget | QLayout | list[QWidget | QLayout]:
+    ) -> QWidget | QLayout | Sequence[QWidget | QLayout]:
         if isinstance(item, QWidget):
             self._layout.addWidget(item, *args, **kwargs)
         elif isinstance(item, QLayout):
             self._layout.addLayout(item, *args, **kwargs)
-        elif isinstance(item, list):
+        elif isinstance(item, Sequence):
             for i in item:
                 self._layout.add(i, *args, **kwargs)
 
         return item
 
     def vbox(self, *args, **kwargs):
         self.next_layout = CVBoxLayout(self._layout, *args, **kwargs)
@@ -210,20 +217,18 @@
             item = self._stack.pop()
             item.__exit__()
 
 
 # *************************************************************************** #
 
 
-class CVBoxLayout(ContextLayout, QVBoxLayout):
-    ...
+class CVBoxLayout(ContextLayout, QVBoxLayout): ...
 
 
-class CHBoxLayout(ContextLayout, QHBoxLayout):
-    ...
+class CHBoxLayout(ContextLayout, QHBoxLayout): ...
 
 
 class CGridLayout(ContextLayout, QGridLayout):
     ...
 
     def addWidget(
         self,
@@ -257,21 +262,61 @@
         """Change the function signature to allow using the spans as named params"""
         rspan = rowSpan if rowSpan != 1 else row_span
         cspan = columnSpan if columnSpan != 1 else column_span
         super().addLayout(item, row, column, rspan, cspan, **kwargs)
 
 
 class CFormLayout(ContextLayout, QFormLayout):
-    ...
+    def __add__(
+        self,
+        item: tuple[str, QWidget | QLayout],
+    ) -> QWidget | QLayout:
+        self.add(item)
+        return item[1]
+
+    def __iadd__(
+        self,
+        item: tuple[str, QWidget | QLayout],
+    ):
+        self.add(item)
+        return self
+
+    def add(
+        self,
+        a: str
+        | QWidget
+        | QLayout
+        | tuple[str, QWidget | QLayout]
+        | Sequence[tuple[str, QWidget | QLayout]]
+        | dict[str, QWidget | QLayout],
+        b: QWidget = None,
+    ):
+        if b is not None:
+            self._layout.addRow(a, b)
+            return b
+
+        if isinstance(a, Sequence):
+            if isinstance(a[0], (str, QWidget, QLayout)):
+                self._layout.addRow(*a)
+                return a[1]
+            if isinstance(a[0], Sequence):
+                for item in a:
+                    self._layout.addRow(*item)
+                return a
+        if isinstance(a, dict):
+            for name, obj in a.items():
+                self._layout.addRow(name, obj)
+
+        return b
 
 
 # --------------------------------------------------------------------------- #
 
 
-class CSplitter(QSplitter, ContextLayoutBase):
+class CSplitter(QSplitter, ContextLayout):
     def __init__(
         self,
         parent: QWidget | QLayout | ContextLayoutBase | None = None,
         margins: QMargins | tuple | int | None = None,
         orientation: OrientationType | None = None,
         **kwargs,
     ):
@@ -295,33 +340,33 @@
                 self.setContentsMargins(margins, margins, margins, margins)
 
         if orientation:
             self.setOrientation(orientation)
 
     def __iadd__(
         self,
-        item: QWidget | QLayout | list[QWidget | QLayout],
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
     ):
         self.add(item)
         return self
 
     def add(
         self,
-        item: QWidget | QLayout | list[QWidget | QLayout],
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
         stretch: int | None = None,
-    ) -> QWidget | QLayout | list[QWidget | QLayout]:
+    ) -> QWidget | QLayout | Sequence[QWidget | QLayout]:
         if isinstance(item, QWidget):
             self.addWidget(item)
             if stretch:
                 self.setStretchFactor(self.count() - 1, stretch)
         elif isinstance(item, QLayout):
             self.addWidget(QWidget(self, layout=item))
             if stretch:
                 self.setStretchFactor(self.count() - 1, stretch)
-        elif isinstance(item, list):
+        elif isinstance(item, Sequence):
             for i in item:
                 self.add(i)
         return item
 
     def __enter__(self):
         return self
 
@@ -381,33 +426,33 @@
         if orientation:
             if orientation in orientations:
                 orientation = orientations[orientation]
             self.setOrientation(orientation)
 
     def __iadd__(
         self,
-        item: QWidget | QLayout | list[QWidget | QLayout],
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
     ):
         self.add(item)
         return self
 
     def add(
         self,
-        item: QWidget | QLayout | list[QWidget | QLayout],
+        item: QWidget | QLayout | Sequence[QWidget | QLayout],
         stretch: int = None,
-    ) -> QWidget | QLayout | list[QWidget | QLayout]:
+    ) -> QWidget | QLayout | Sequence[QWidget | QLayout]:
         if isinstance(item, QWidget):
             self.widget().layout().addWidget(item)
             if stretch:
                 self.widget().layout().setStretchFactor(self.count() - 1, stretch)
         elif isinstance(item, QLayout):
             self.addWidget(QWidget(self, layout=item))
             if stretch:
                 self.setStretchFactor(self.count() - 1, stretch)
-        elif isinstance(item, list):
+        elif isinstance(item, Sequence):
             for i in item:
                 self.add(i)
         return item
 
     def addWidget(self, *args, **kwargs):
         self.widget().layout().addWidget(*args, **kwargs)
```

### Comparing `qtstrap-0.5.3/qtstrap/widgets/line_widgets.py` & `qtstrap-0.6.0/qtstrap/widgets/line_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/link_label.py` & `qtstrap-0.6.0/qtstrap/widgets/link_label.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/persistent_tab_widget.py` & `qtstrap-0.6.0/qtstrap/widgets/persistent_tab_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,18 @@
                     for name, tab in tabs.items():
                         add_tab(tab, name)
             else:
                 for name, tab in tabs.items():
                     add_tab(tab, name)
 
         prev_index = QSettings().value(self.name + '/current', 0)
-        if isinstance(prev_index, int):
+        try:
             self.setCurrentIndex(min(int(prev_index), self.count()))
+        except:
+            pass
 
         self.currentChanged.connect(lambda i: QSettings().setValue(self.name + '/current', i))
 
     def tab_order(self):
         order = []
         for i in range(self.count()):
             order.append(self.tabText(i))
```

### Comparing `qtstrap-0.5.3/qtstrap/widgets/persistent_widgets.py` & `qtstrap-0.6.0/qtstrap/widgets/persistent_widgets.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/toggle.py` & `qtstrap-0.6.0/qtstrap/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap/widgets/toolbar.py` & `qtstrap-0.6.0/qtstrap/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/qtstrap.egg-info/PKG-INFO` & `qtstrap-0.6.0/qtstrap.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qtstrap
-Version: 0.5.3
+Version: 0.6.0
 Summary: Like Bootstrap, but qt-er.
 Home-page: https://github.com/qtstrap/qtstrap
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
-Project-URL: Documentation, https://qtstrap.github.io/qtstrap/
+Project-URL: Documentation, https://qtstrap.github.io/
 Project-URL: Source, https://github.com/qtstrap/qtstrap
 Project-URL: Tracker, https://github.com/qtstrap/qtstrap/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Widget Sets
@@ -38,23 +38,43 @@
 
 Qt is excellent, but it's also enormous. There's a lot of topics, and many of them have hidden gotchas. PySide2 and PyQt are also excellent, letting us leverage the powerful Qt libraries from up in the clouds in PythonLand, but this arrangement has its own gotchas. 
 
 The goal of qtstrap is get your applications up and running quickly, so you can focus on your problem instead of on Qt's idiosyncracies.
 
 # Features
 
-More complete docs are available [here](https://qtstrap.github.io/qtstrap/).
+More complete docs are available [here](https://qtstrap.github.io/).
 
 * `qtstrap` command line tool to bootstrap new projects
 * crossplatform makefile with useful development commands
 * preconfigured build system using PyInstaller and InnoSetup
 * custom Qt widgets with useful behaviors
 * Pythonic layout system using ContextLayouts
 * Some other stuff I haven't remembered yet
 
+# Quick start
+
+```sh
+$ mkdir test && cd test
+$ python3 -m venv .venv
+$ source .venv/bin/activate
+$ python3 -m pip install qtstrap PySide6
+$ qtstrap init
+```
+
+The init script will prompt you to enter the name of your application and the name of its publisher(which is probably you), and then it will generate an application skeleton.
+
+You can test that everything installed properly by executing:
+```sh
+$ python3 app/main.py
+```
+If you see a window like this, then you're good to go:
+
+![screenshot](docs/screenshot1.png) 
+
 ## Custom Widgets
 
 - `LabelEdit`
 - `HLine` and `VLine`
 - `LinkLabel`
 - Buttons:
   - `StateButton`
```

### Comparing `qtstrap-0.5.3/qtstrap.egg-info/SOURCES.txt` & `qtstrap-0.6.0/qtstrap.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 .gitignore
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 build_docs.py
 mkdocs.yml
 pyproject.toml
 requirements.txt
 requirements_build.txt
 requirements_test.txt
+ruff.toml
 run_tox_tests.py
 setup.cfg
 setup.py
 tox.ini
 .github/FUNDING.yml
 .github/workflows/main.yml
 docs/index.md
 docs/screenshot1.png
 docs/test.md
 docs/api/.pages
+docs/api/experimental.md
 docs/api/extras.code_editor.code_editor.md
 docs/api/extras.code_editor.code_line.md
 docs/api/extras.code_editor.highlighters.md
 docs/api/extras.code_editor.highlighters.python.md
 docs/api/extras.code_editor.md
 docs/api/extras.command_palette.command_palette.md
 docs/api/extras.command_palette.md
@@ -33,14 +36,15 @@
 docs/api/extras.log_monitor.log_widget.md
 docs/api/extras.log_monitor.md
 docs/api/extras.md
 docs/api/extras.style.colors.md
 docs/api/extras.style.dark_palette.md
 docs/api/extras.style.md
 docs/api/extras.style.themes.md
+docs/api/optional.md
 docs/api/options.md
 docs/api/overview.md
 docs/api/settings.md
 docs/api/utils.adapter.md
 docs/api/utils.call_later.md
 docs/api/utils.decorators.md
 docs/api/utils.defer.md
@@ -92,14 +96,15 @@
 docs/reference/widgets.line_widgets.md
 docs/reference/widgets.link_label.md
 docs/reference/widgets.md
 docs/reference/widgets.persistent_tab_widget.md
 docs/reference/widgets.persistent_widgets.md
 docs/structure/makefile.md
 docs/structure/structure.md
+docs_theme/main.html
 qtstrap/__init__.py
 qtstrap/__main__.py
 qtstrap/base_application.py
 qtstrap/base_window.py
 qtstrap/options.py
 qtstrap/qt.py
 qtstrap/settings.py
@@ -107,14 +112,16 @@
 qtstrap.egg-info/SOURCES.txt
 qtstrap.egg-info/dependency_links.txt
 qtstrap.egg-info/entry_points.txt
 qtstrap.egg-info/not-zip-safe
 qtstrap.egg-info/requires.txt
 qtstrap.egg-info/top_level.txt
 qtstrap/experimental/__init__.py
+qtstrap/experimental/bindings/bind.py
+qtstrap/experimental/bindings/bind_widgets.py
 qtstrap/extras/__init__.py
 qtstrap/extras/code_editor/__init__.py
 qtstrap/extras/code_editor/code_editor.py
 qtstrap/extras/code_editor/code_line.py
 qtstrap/extras/code_editor/highlighters/__init__.py
 qtstrap/extras/code_editor/highlighters/python.py
 qtstrap/extras/command_palette/__init__.py
@@ -162,10 +169,13 @@
 qtstrap/widgets/persistent_tab_widget.py
 qtstrap/widgets/persistent_widgets.py
 qtstrap/widgets/toggle.py
 qtstrap/widgets/toolbar.py
 test/test_base_app.py
 test/test_base_window.py
 test/test_layouts.py
+test/utils/test_call_later.py
 test/utils/test_defer.py
+test/utils/test_signal_adapter.py
+test/utils/test_singleton.py
 test/utils/test_string_builder.py
 test/utils/test_utils.py
```

### Comparing `qtstrap-0.5.3/requirements.txt` & `qtstrap-0.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/requirements_build.txt` & `qtstrap-0.6.0/requirements_build.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/requirements_test.txt` & `qtstrap-0.6.0/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/setup.cfg` & `qtstrap-0.6.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7473 7472 6170 0d0a 7665 7273   = qtstrap..vers
-00000020: 696f 6e20 3d20 302e 352e 330d 0a64 6573  ion = 0.5.3..des
+00000020: 696f 6e20 3d20 302e 362e 300d 0a64 6573  ion = 0.6.0..des
 00000030: 6372 6970 7469 6f6e 203d 204c 696b 6520  cription = Like 
 00000040: 426f 6f74 7374 7261 702c 2062 7574 2071  Bootstrap, but q
 00000050: 742d 6572 2e0d 0a6c 6f6e 675f 6465 7363  t-er...long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
@@ -41,39 +41,38 @@
 00000280: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
 00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 000002b0: 3a3a 2033 2e31 310d 0a70 726f 6a65 6374  :: 3.11..project
 000002c0: 5f75 726c 7320 3d20 0d0a 0944 6f63 756d  _urls = ...Docum
 000002d0: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
 000002e0: 3a2f 2f71 7473 7472 6170 2e67 6974 6875  ://qtstrap.githu
-000002f0: 622e 696f 2f71 7473 7472 6170 2f0d 0a09  b.io/qtstrap/...
-00000300: 536f 7572 6365 203d 2068 7474 7073 3a2f  Source = https:/
-00000310: 2f67 6974 6875 622e 636f 6d2f 7174 7374  /github.com/qtst
-00000320: 7261 702f 7174 7374 7261 700d 0a09 5472  rap/qtstrap...Tr
-00000330: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
-00000340: 6769 7468 7562 2e63 6f6d 2f71 7473 7472  github.com/qtstr
-00000350: 6170 2f71 7473 7472 6170 2f69 7373 7565  ap/qtstrap/issue
-00000360: 730d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  s....[options]..
-00000370: 7a69 705f 7361 6665 203d 2046 616c 7365  zip_safe = False
-00000380: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000390: 643a 0d0a 706c 6174 666f 726d 7320 3d20  d:..platforms = 
-000003a0: 616e 790d 0a69 6e63 6c75 6465 5f70 6163  any..include_pac
-000003b0: 6b61 6765 5f64 6174 6120 3d20 7472 7565  kage_data = true
-000003c0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000003d0: 6573 203d 200d 0a09 5174 5079 0d0a 0963  es = ...QtPy...c
-000003e0: 6c69 636b 0d0a 0969 6e71 7569 7265 7270  lick...inquirerp
-000003f0: 790d 0a09 6170 7064 6972 730d 0a09 7174  y...appdirs...qt
-00000400: 6177 6573 6f6d 650d 0a09 7079 696e 7374  awesome...pyinst
-00000410: 616c 6c65 720d 0a70 7974 686f 6e5f 7265  aller..python_re
-00000420: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000430: 0d0a 5b62 6469 7374 5f77 6865 656c 5d0d  ..[bdist_wheel].
-00000440: 0a75 6e69 7665 7273 616c 203d 2031 0d0a  .universal = 1..
-00000450: 0d0a 5b61 6c69 6173 6573 5d0d 0a74 6573  ..[aliases]..tes
-00000460: 7420 3d20 7079 7465 7374 0d0a 0d0a 5b6f  t = pytest....[o
-00000470: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-00000480: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-00000490: 7269 7074 7320 3d20 0d0a 0971 7473 7472  ripts = ...qtstr
-000004a0: 6170 3d71 7473 7472 6170 2e5f 5f6d 6169  ap=qtstrap.__mai
-000004b0: 6e5f 5f3a 6d61 696e 0d0a 0d0a 5b65 6767  n__:main....[egg
-000004c0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000004d0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004e0: 2030 0d0a 0d0a                            0....
+000002f0: 622e 696f 2f0d 0a09 536f 7572 6365 203d  b.io/...Source =
+00000300: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000310: 636f 6d2f 7174 7374 7261 702f 7174 7374  com/qtstrap/qtst
+00000320: 7261 700d 0a09 5472 6163 6b65 7220 3d20  rap...Tracker = 
+00000330: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000340: 6f6d 2f71 7473 7472 6170 2f71 7473 7472  om/qtstrap/qtstr
+00000350: 6170 2f69 7373 7565 730d 0a0d 0a5b 6f70  ap/issues....[op
+00000360: 7469 6f6e 735d 0d0a 7a69 705f 7361 6665  tions]..zip_safe
+00000370: 203d 2046 616c 7365 0d0a 7061 636b 6167   = False..packag
+00000380: 6573 203d 2066 696e 643a 0d0a 706c 6174  es = find:..plat
+00000390: 666f 726d 7320 3d20 616e 790d 0a69 6e63  forms = any..inc
+000003a0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+000003b0: 6120 3d20 7472 7565 0d0a 696e 7374 616c  a = true..instal
+000003c0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
+000003d0: 5174 5079 0d0a 0963 6c69 636b 0d0a 0969  QtPy...click...i
+000003e0: 6e71 7569 7265 7270 790d 0a09 6170 7064  nquirerpy...appd
+000003f0: 6972 730d 0a09 7174 6177 6573 6f6d 650d  irs...qtawesome.
+00000400: 0a09 7079 696e 7374 616c 6c65 720d 0a70  ..pyinstaller..p
+00000410: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000420: 203e 3d33 2e38 0d0a 0d0a 5b62 6469 7374   >=3.8....[bdist
+00000430: 5f77 6865 656c 5d0d 0a75 6e69 7665 7273  _wheel]..univers
+00000440: 616c 203d 2031 0d0a 0d0a 5b61 6c69 6173  al = 1....[alias
+00000450: 6573 5d0d 0a74 6573 7420 3d20 7079 7465  es]..test = pyte
+00000460: 7374 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  st....[options.e
+00000470: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
+00000480: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
+00000490: 0d0a 0971 7473 7472 6170 3d71 7473 7472  ...qtstrap=qtstr
+000004a0: 6170 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e  ap.__main__:main
+000004b0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000004c0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000004d0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `qtstrap-0.5.3/test/test_base_app.py` & `qtstrap-0.6.0/test/test_base_app.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/test/test_base_window.py` & `qtstrap-0.6.0/test/test_base_window.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/test/test_layouts.py` & `qtstrap-0.6.0/test/test_layouts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from qtstrap import (
     CHBoxLayout,
     CVBoxLayout,
     CGridLayout,
+    CFormLayout,
     get_children,
 )
 from qtpy.QtCore import (
     QMargins,
 )
 from qtpy.QtWidgets import (
     QLabel,
     QWidget,
+    QPushButton,
 )
 
 
 def test_context_layout():
     def get_hbox():
         with CHBoxLayout() as hbox:
             hbox.add(QLabel('H1'))
             hbox.add(QLabel('H2'))
         return hbox
 
     widget = QWidget()
 
     with CVBoxLayout(widget) as layout:
-        layout.add(QLabel('test'))
+        layout.add(QLabel('test1'))
         layout += QLabel('test2')
         layout.add([QLabel('test3'), QLabel('test4')])
         layout += [QLabel('test5'), QLabel('test6')]
         layout.add(get_hbox())
         layout += get_hbox()
+        test7 = layout + QLabel('test7')
+        test8, test9 = layout + (QLabel('test8'), QLabel('test9'))
 
-    assert len(get_children(widget)) == 13
+    assert len(get_children(widget)) == 16
+    assert test7.text() == 'test7'
 
 
 def test_nested_context_layout():
     widget = QWidget()
 
     with CVBoxLayout(widget) as layout:
         with layout.hbox() as layout:
@@ -43,16 +48,28 @@
         with layout.hbox() as layout:
             layout.add(QLabel('lower left'))
             layout.add(QLabel('lower right'))
 
     assert len(get_children(widget)) == 7
 
 
-def test_formlayout():
-    pass
+def test_form_layout():
+    widget = QWidget()
+
+    with CFormLayout(widget) as layout:
+        # add() with two args
+        layout.add('', QPushButton(''))
+        # += tuple
+        layout += ('', QPushButton(''))
+        # += sequence of tuples
+        layout += [('', QPushButton('')), ('', QPushButton(''))]
+        # += dict
+        layout += {'1': QPushButton(''), '2': QPushButton('')}
+
+    assert len(get_children(widget)) == 9
 
 
 def test_splitter():
     pass
 
 
 def test_scrollarea():
```

### Comparing `qtstrap-0.5.3/test/utils/test_string_builder.py` & `qtstrap-0.6.0/test/utils/test_string_builder.py`

 * *Files identical despite different names*

### Comparing `qtstrap-0.5.3/test/utils/test_utils.py` & `qtstrap-0.6.0/test/utils/test_utils.py`

 * *Files identical despite different names*

