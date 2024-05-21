# Comparing `tmp/pinjected-0.2.69.tar.gz` & `tmp/pinjected-0.2.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.69.tar", max compression
+gzip compressed data, was "pinjected-0.2.70.tar", max compression
```

## Comparing `pinjected-0.2.69.tar` & `pinjected-0.2.70.tar`

### file list

```diff
@@ -1,93 +1,97 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.69/LICENSE
--rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.69/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.69/pinjected/__main__.py
--rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.69/pinjected/compatibility/__init__.py
--rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.69/pinjected/compatibility/task_group.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.69/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.69/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.69/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.69/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.69/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.69/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7958 2024-05-16 04:59:01.249430 pinjected-0.2.69/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.69/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.69/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.69/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14572 2024-05-14 13:17:02.297068 pinjected-0.2.69/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.69/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.69/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.69/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.69/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.69/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    56168 2024-05-15 06:42:25.667673 pinjected-0.2.69/pinjected/di/injected.py
--rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.69/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.69/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.69/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.69/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.69/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.69/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.69/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.69/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.69/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.69/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.69/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.69/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.69/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.69/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.69/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.69/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.69/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.69/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.69/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.69/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.69/pinjected/di/util.py
--rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.69/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.69/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.69/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.69/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.69/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.69/pinjected/global_configs.py
--rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.69/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.69/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.69/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.69/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.69/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.69/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.69/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.69/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.69/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.69/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.69/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.69/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.69/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.69/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.69/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.69/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.69/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.69/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.69/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.69/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.69/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.69/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.69/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.69/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.69/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9732 2024-05-15 05:20:27.364514 pinjected-0.2.69/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.69/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.69/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.69/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.69/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.69/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.69/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.69/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.69/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.69/pinjected/v2/di.py
--rw-r--r--   0        0        0      616 2024-05-15 04:08:13.929515 pinjected-0.2.69/pinjected/v2/keys.py
--rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.69/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0    24800 2024-05-15 05:09:47.881318 pinjected-0.2.69/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.69/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.69/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.69/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.69/pinjected/with_context.py
--rw-r--r--   0        0        0      627 2024-05-16 04:59:03.694016 pinjected-0.2.69/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.69/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.70/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.70/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.70/pinjected/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:05:50.568481 pinjected-0.2.70/pinjected/common/__init__.py
+-rw-r--r--   0        0        0        3 2024-05-21 04:18:58.523298 pinjected-0.2.70/pinjected/common/callbacks.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.70/pinjected/compatibility/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.70/pinjected/compatibility/task_group.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.70/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.70/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.70/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.70/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.70/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.70/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7958 2024-05-16 04:59:01.249430 pinjected-0.2.70/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.70/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.70/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.70/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14744 2024-05-21 04:18:58.519390 pinjected-0.2.70/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.70/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.70/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.70/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.70/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.70/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    56168 2024-05-15 06:42:25.667673 pinjected-0.2.70/pinjected/di/injected.py
+-rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.70/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.70/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.70/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.70/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.70/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.70/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.70/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.70/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.70/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.70/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.70/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.70/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.70/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.70/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0     1051 2024-05-21 04:20:44.424963 pinjected-0.2.70/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1632 2024-05-21 04:31:46.228251 pinjected-0.2.70/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.70/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.70/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.70/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.70/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.70/pinjected/di/util.py
+-rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.70/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.70/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.70/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.70/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.70/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.70/pinjected/global_configs.py
+-rw-r--r--   0        0        0     3126 2024-05-20 09:02:27.376887 pinjected-0.2.70/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.70/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.70/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.70/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.70/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.70/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.70/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.70/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.70/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.70/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.70/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.70/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.70/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.70/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.70/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.70/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.70/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.70/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.70/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.70/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.70/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.70/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.70/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.70/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.70/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9439 2024-05-21 04:18:58.493434 pinjected-0.2.70/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.70/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.70/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.70/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.70/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.70/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.70/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.70/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.70/pinjected/v2/binds.py
+-rw-r--r--   0        0        0      132 2024-05-21 04:19:54.467096 pinjected-0.2.70/pinjected/v2/callback.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.70/pinjected/v2/di.py
+-rw-r--r--   0        0        0      796 2024-05-21 04:19:54.473975 pinjected-0.2.70/pinjected/v2/events.py
+-rw-r--r--   0        0        0      616 2024-05-15 04:08:13.929515 pinjected-0.2.70/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.70/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    25050 2024-05-21 04:33:02.098641 pinjected-0.2.70/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.70/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.70/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.70/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.70/pinjected/with_context.py
+-rw-r--r--   0        0        0      627 2024-05-21 04:34:18.066941 pinjected-0.2.70/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.70/PKG-INFO
```

### Comparing `pinjected-0.2.69/LICENSE` & `pinjected-0.2.70/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/compatibility/task_group.py` & `pinjected-0.2.70/pinjected/compatibility/task_group.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/decoration.py` & `pinjected-0.2.70/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/demo.py` & `pinjected-0.2.70/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/app_designed.py` & `pinjected-0.2.70/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/app_injected.py` & `pinjected-0.2.70/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/applicative.py` & `pinjected-0.2.70/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/ast.py` & `pinjected-0.2.70/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/decorators.py` & `pinjected-0.2.70/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/design.py` & `pinjected-0.2.70/pinjected/di/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass, field, replace
 from functools import wraps
 from typing import TypeVar, List, Dict, Union, Callable, Type
 
 from cytoolz import merge
 from makefun import create_function
 
+from pinjected.v2.callback import IResolverCallback
 from pinjected.di.app_injected import EvaledInjected
 from pinjected.di.graph import DependencyResolver
 from pinjected.di.implicit_globals import IMPLICIT_BINDINGS
 from pinjected.di.injected import Injected
 from pinjected.di.injected import extract_dependency_including_self, InjectedPure, InjectedFunction
 # from pinjected.di.util import get_class_aware_args, get_dict_diff, check_picklable
 from pinjected.di.proxiable import DelegatedVar
@@ -209,18 +210,20 @@
             key = StrBindKey(k)
             bind: IBind = self.bindings[key]
             res += Design(
                 bindings={key: bind.update_metadata(meta)}
             )
         return res
 
-    def to_resolver(self):
+    def to_resolver(self,callback:IResolverCallback=None):
         from pinjected.v2.resolver import AsyncResolver,BaseResolverCallback
         bindings = {**IMPLICIT_BINDINGS, **self.bindings}
-        callback = BaseResolverCallback()
+        if callback is None:
+            callback = BaseResolverCallback()
+        assert isinstance(callback, IResolverCallback)
         return AsyncResolver(
             Design(bindings=bindings, modules=self.modules),
             callbacks=[
                 callback
             ]
         )
```

### Comparing `pinjected-0.2.69/pinjected/di/designed.py` & `pinjected-0.2.70/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.70/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/graph.py` & `pinjected-0.2.70/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/injected.py` & `pinjected-0.2.70/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/injected_analysis.py` & `pinjected-0.2.70/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/modular_injected.py` & `pinjected-0.2.70/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/overload_experimental.py` & `pinjected-0.2.70/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/proxiable.py` & `pinjected-0.2.70/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/session.py` & `pinjected-0.2.70/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/sessioned.py` & `pinjected-0.2.70/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/static_proxy.py` & `pinjected-0.2.70/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.70/pinjected/di/test_dynamic_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,29 +17,30 @@
         "A_Proxy"
     )
     x = ctx.pure("hello world")
     print(x)
     print(x.split())
     print([i for i in x.split()])
 
-
-def test_session_value_iterator():
-    d = Design().bind_instance(x=0)
-    g = d.to_resolver().to_blocking()
-    session = g.child_session(EmptyDesign)
-    ctx = DynamicProxyContextImpl(
-        lambda a: a.value,
-        lambda x: SessionValue(
-            g,
-            Designed.bind(Injected.pure(x)),
-            session,
-        ),
-        "SessionValueProxy"
-    )
-    x = ctx.pure("hello world")
-    print(x)
-    print(x.split())
-    for item in x.split():
-        print(item.eval())
-
-    print(g.sessioned("x"))
-
+# deprecated
+#
+# def test_session_value_iterator():
+#     d = Design().bind_instance(x=0)
+#     g = d.to_resolver().to_blocking()
+#     session = g.child_session(EmptyDesign)
+#     ctx = DynamicProxyContextImpl(
+#         lambda a: a.value,
+#         lambda x: SessionValue(
+#             g,
+#             Designed.bind(Injected.pure(x)),
+#             session,
+#         ),
+#         "SessionValueProxy"
+#     )
+#     x = ctx.pure("hello world")
+#     print(x)
+#     print(x.split())
+#     for item in x.split():
+#         print(item.eval())
+#
+#     print(g.sessioned("x"))
+#
```

### Comparing `pinjected-0.2.69/pinjected/di/test_graph.py` & `pinjected-0.2.70/pinjected/di/test_graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from returns.result import safe, Failure
 
-from pinjected import Design
+from pinjected import Design, instances
 
 
 def test_provide_session():
     d = Design().bind_instance(
         a=0
     )
     g = d.to_graph()
@@ -14,24 +14,27 @@
 def test_child_session():
     d = Design().bind_instance(
         a=0
     ).bind_provider(
         x=lambda a: a
     )
     g = d.to_graph()
-    child_g = g.child_session(Design().bind_instance(a=1))
-    grandchild_g = child_g.child_session(Design().bind_instance(a=2))
+    child_g = g.child_session(instances(a=1))
+    grandchild_g = child_g.child_session(instances(a=2))
     assert g["a"] == 0
     assert child_g['a'] == 1  # ah, this is actually an expected behavior.
     assert grandchild_g['a'] == 2
     assert child_g['a'] == 1  # oh why is this 0??
     assert g["a"] == 0
     assert g["x"] == 0
     assert child_g['x'] == 0  # x is already in parent, and is not overriden explicitly.
     # for this to work we need to track all the dependenciy tree of a binding.
+    from loguru import logger
+    logger.info(grandchild_g)
+    logger.info(grandchild_g.resolver._design_from_ancestors().bindings)
     assert grandchild_g['x'] == 0
     assert child_g['x'] == 0  # oh why is this 0??
     assert g["x"] == 0
     # so in order to make session work,
     # you must specify all the components,
     # implicit components in child session will be forgotten.
```

### Comparing `pinjected-0.2.69/pinjected/di/test_injected.py` & `pinjected-0.2.70/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/tools/add_overload.py` & `pinjected-0.2.70/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/di/util.py` & `pinjected-0.2.70/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/exceptions.py` & `pinjected-0.2.70/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.70/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.70/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/graph_inspection.py` & `pinjected-0.2.70/pinjected/graph_inspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from dataclasses import dataclass
 from pprint import pformat
 
 from loguru import logger
 from pinjected import Injected
 from pinjected.v2.binds import IBind, BindInjected, ExprBind
-from pinjected.v2.keys import IBindKey, StrBindKey
+from pinjected.v2.keys import IBindKey, StrBindKey, DestructorKey
 
 
 def default_get_arg_names_from_class_name(class_name):
     """Converts normal class names into normal arg names.
 
     from github's pinject
 
@@ -75,14 +75,16 @@
         mappings = dict()
         for k, v in bindings.items():
             match k, v:
                 case (StrBindKey(name), BindInjected(Injected() as injected)):
                     mappings[name] = injected
                 case (StrBindKey(name), ExprBind(src,meta)):
                     mappings[name] = src
+                case (DestructorKey(name), _):
+                    pass
                 case _:
                     raise ValueError(f"unsupported key type {k} and value type {v}")
         return mappings
 
     def total_bindings(self) -> dict[IBindKey, IBind]:
         from pinjected.di.implicit_globals import IMPLICIT_BINDINGS
         global_implicit_mappings = IMPLICIT_BINDINGS
```

### Comparing `pinjected-0.2.69/pinjected/helper_structure.py` & `pinjected-0.2.70/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/helpers.py` & `pinjected-0.2.70/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.70/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.70/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/ide_supports/default_design.py` & `pinjected-0.2.70/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.70/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.70/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/main_impl.py` & `pinjected-0.2.70/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/maybe_patch.py` & `pinjected-0.2.70/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/module_helper.py` & `pinjected-0.2.70/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/module_inspector.py` & `pinjected-0.2.70/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/module_var_path.py` & `pinjected-0.2.70/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/notification.py` & `pinjected-0.2.70/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/nx_graph_util.py` & `pinjected-0.2.70/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/run_config_utils.py` & `pinjected-0.2.70/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/run_config_utils_v2.py` & `pinjected-0.2.70/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/run_helpers/config.py` & `pinjected-0.2.70/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.70/pinjected/run_helpers/run_injected.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,77 +94,70 @@
                 design += var.design
                 var = var.internal_injected
         """
         I need to get the design overrides from with context and add it to the overrides
         """
 
         meta_design = instances(overrides=instances()) + meta_cxt.accumulated
-        meta_overrides = meta_design.provide("overrides") + meta_overrides
+        meta_resolver = meta_design.to_resolver().to_blocking()
+        meta_overrides = meta_resolver.provide("overrides") + meta_overrides
 
         # add overrides from with block
         meta_overrides += DESIGN_OVERRIDES_STORE.get_overrides(ModuleVarPath(var_path))
 
+        # obtain internal hooks from the meta_design
+        if 'provision_callback' in meta_design:
+            provision_callback = meta_resolver.provide('provision_callback')
+        else:
+            provision_callback = None
+
     design += (meta_overrides + overrides)
     logger.info(f"running target:{var} with {design_path} + {overrides}")
     logger.debug(design.keys())
     # logger.info(f"running target:{var} with cmd {cmd}, args {args}, kwargs {kwargs}")
     # logger.info(f"metadata obtained from pinjected: {meta}")
 
     # here we load the defaults and overrides from the user's environment
     design = load_user_default_design() + design + load_user_overrides_design()
 
     res = None
 
-    def run_target(d,tgt):
+    def run_target(d, tgt):
+        # here, I want to specify what to use for the provision callback.
         async def task():
             async with TaskGroup() as tg:
                 dd = d + instances(
                     __task_group__=tg
                 )
-                resolver = dd.to_resolver()
+                resolver = dd.to_resolver(
+                    callback=provision_callback
+                )
                 _res = await resolver.provide(tgt)
 
                 if isinstance(_res, Awaitable):
                     # logger.info(f"awaiting awaitable")
                     _res = await _res
                 if not return_result:
                     logger.info(f"run_injected result:\n{_res}")
             await resolver.destruct()
             return _res
-        return asyncio.run(task())
-
 
+        return asyncio.run(task())
 
     try:
         if cmd == 'call':
             args = call_args or []
             kwargs = call_kwargs or {}
             var = Injected.ensure_injected(var).proxy
             logger.info(f"run_injected call with args:{args}, kwargs:{kwargs}")
-            res = run_target(design,var(*args, **kwargs))
+            res = run_target(design, var(*args, **kwargs))
         elif cmd == 'get':
-            res = run_target(design,var)
+            res = run_target(design, var)
         elif cmd == 'fire':
             raise RuntimeError('fire is deprecated. use get.')
-            return_result = True
-            resolver = design.to_resolver()
-            res = design.provide(var)
-            if isinstance(res, Coroutine):
-                res = asyncio.run(res)
-            logger.info(f"run_injected fire result:\n{res}")
-            if inspect.iscoroutinefunction(res) or (hasattr(res, '__is_async__') and res.__is_async__):
-                logger.info(f'{res} is a coroutine function, wrapping it with asyncio.run')
-                src = res
-                # @wraps(res)
-                def synced(*args, **kwargs):
-                    return asyncio.run(src(*args, **kwargs))
-
-                res = synced
-            else:
-                logger.info(f"{res} is not a coroutine function.")
         elif cmd == 'visualize':
             from loguru import logger
             logger.info(f"visualizing {var_path} with design {design_path}")
             logger.info(f"deps:{var.dependencies()}")
             design.to_vis_graph().show_injected_html(var)
         elif cmd == 'to_script':
             from loguru import logger
```

### Comparing `pinjected-0.2.69/pinjected/runnables.py` & `pinjected-0.2.70/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/test_package/__init__.py` & `pinjected-0.2.70/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/test_package/child/module1.py` & `pinjected-0.2.70/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/v2/ainjected.py` & `pinjected-0.2.70/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/v2/binds.py` & `pinjected-0.2.70/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/v2/di.py` & `pinjected-0.2.70/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/v2/keys.py` & `pinjected-0.2.70/pinjected/v2/keys.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/v2/provide_context.py` & `pinjected-0.2.70/pinjected/v2/provide_context.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pinjected/v2/resolver.py` & `pinjected-0.2.70/pinjected/v2/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 from loguru import logger
+
+from pinjected.v2.callback import IResolverCallback
+from pinjected.v2.events import ResolverEvent, RequestEvent, ProvideEvent, DepsReadyEvent, EvalRequestEvent, \
+    CallInEvalStart, CallInEvalEnd, EvalResultEvent
+
 try:
     import nest_asyncio
     import uvloop
     logger.error(f"nest_asyncio is disabled since uvloop is also installed! nest_asyncio.apply do not work with uvloop!")
     nest_asyncio.apply = lambda:None
 except ImportError:
     pass
@@ -89,63 +94,14 @@
     '-': operator.neg,
     '~': operator.invert,
     'not': operator.not_
 }
 
 
 @dataclass
-class ResolverEvent:
-    cxt: ProvideContext
-
-
-@dataclass
-class RequestEvent(ResolverEvent):
-    key: IBindKey
-
-
-@dataclass
-class ProvideEvent(ResolverEvent):
-    key: IBindKey
-    data: Any
-
-
-@dataclass
-class DepsReadyEvent(ResolverEvent):
-    key: IBindKey
-    deps: Dict[IBindKey, Any]
-
-
-@dataclass
-class EvalRequestEvent(ResolverEvent):
-    expr: Expr
-
-
-@dataclass
-class CallInEvalStart(ResolverEvent):
-    expr: Call
-
-
-@dataclass
-class CallInEvalEnd(ResolverEvent):
-    expr: Call
-    result: Any
-
-
-@dataclass
-class EvalResultEvent(ResolverEvent):
-    expr: Expr
-    result: Any
-
-
-class IResolverCallback:
-    def __call__(self, event: ResolverEvent):
-        pass
-
-
-@dataclass
 class AsyncResolver:
     design: "Design"
     parent: Optional["AsyncResolver"] = None
     objects: Dict[IBindKey, Any] = field(default_factory=dict)
     locks: AsyncLockMap = field(default_factory=AsyncLockMap)
     callbacks: list[IResolverCallback] = field(default_factory=list)
 
@@ -159,14 +115,21 @@
     def __post_init__(self):
         from pinjected import providers
         async def dummy():
             raise RuntimeError('This should never be instantiated')
 
         dummy = Injected.bind(dummy)
 
+        # maybe,,, we can obtain __pinjected_provision_callback__ from design.
+        # but provision involves instantiating this resolver, resulting in recursion.
+        # The solution is to introduce a 'phase' for provision
+        # 1. preparation phase, instantiate all stuff like __pinjected_....__.
+        # 2. user provision phase, where user can provide stuff. we use __pinjected_...__ to provide stuff.
+        # I think we should stick to constructor injection for simplicity.
+
         self.design = self.design + providers(
             __resolver__=dummy,
             __design__=dummy
         )
         self.objects = {
             StrBindKey("__resolver__"): self,
             StrBindKey("__design__"): self.design
@@ -337,19 +300,26 @@
                 if inspect.iscoroutinefunction(tgt):
                     return await data
                 else:
                     return data
             case _:
                 raise TypeError(f"tgt must be str, IBindKey, Callable or IBind, got {tgt}")
 
+    def _design_from_ancestors(self):
+        from pinjected import Design
+        if self.parent is None:
+            p_design = Design()
+        else:
+            p_design = self.parent._design_from_ancestors()
+        return p_design + self.design
+
     async def validate_provision(self, tgt: Providable):
         logger.debug(f"validating provision...")
-        from pinjected import Design
         from pinjected import providers
-        d: Design = self.design
+        d = self._design_from_ancestors()
         errors = []
         match tgt:
             case Injected():
                 tmp_design = d + providers(__root__=tgt)
                 digraph: DIGraph = tmp_design.to_vis_graph()
                 errors = list(digraph.di_dfs_validation("__root__"))
             case str():
```

### Comparing `pinjected-0.2.69/pinjected/visualize_di.py` & `pinjected-0.2.70/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.69/pyproject.toml` & `pinjected-0.2.70/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.69"
+version = "0.2.70"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.69/PKG-INFO` & `pinjected-0.2.70/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.69
+Version: 0.2.70
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

