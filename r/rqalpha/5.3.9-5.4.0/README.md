# Comparing `tmp/rqalpha-5.3.9.tar.gz` & `tmp/rqalpha-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-rf3mmfs2/rqalpha-5.3.9.tar", last modified: Tue Apr 16 02:18:48 2024, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-y1qj44jj/rqalpha-5.4.0.tar", last modified: Tue May 21 07:39:02 2024, max compression
```

## Comparing `rqalpha-5.3.9.tar` & `rqalpha-5.4.0.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-04-16 02:18:41.000000 rqalpha-5.3.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-16 02:18:41.000000 rqalpha-5.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 02:18:41.000000 rqalpha-5.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 02:18:48.000000 rqalpha-5.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-16 02:18:41.000000 rqalpha-5.3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    35275 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    58869 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (127)    18961 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    34676 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)    22708 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (127)    34880 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)    21406 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28049 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29447 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25895 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21138 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (127)    32799 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20452 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    56217 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 02:18:41.000000 rqalpha-5.3.9/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 02:18:48.000000 rqalpha-5.3.9/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 02:18:48.000000 rqalpha-5.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-16 02:18:41.000000 rqalpha-5.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_f_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_pit_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:18:48.000000 rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-16 02:18:41.000000 rqalpha-5.3.9/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    86835 2024-04-16 02:18:41.000000 rqalpha-5.3.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-05-21 07:38:56.000000 rqalpha-5.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-21 07:38:56.000000 rqalpha-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 07:38:56.000000 rqalpha-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-21 07:39:02.000000 rqalpha-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-21 07:38:56.000000 rqalpha-5.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35275 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58869 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17409 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24370 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22708 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35064 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21406 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27907 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    23382 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30953 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25639 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)    32799 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19772 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    56502 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-21 07:38:56.000000 rqalpha-5.4.0/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 07:39:02.000000 rqalpha-5.4.0/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 07:39:02.000000 rqalpha-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-21 07:38:56.000000 rqalpha-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_f_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_f_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_pit_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/unittest/test_data/test_auto_update_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_data/test_auto_update_bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:39:02.000000 rqalpha-5.4.0/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-21 07:38:56.000000 rqalpha-5.4.0/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-21 07:38:57.000000 rqalpha-5.4.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-21 07:38:57.000000 rqalpha-5.4.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86835 2024-05-21 07:38:57.000000 rqalpha-5.4.0/versioneer.py
```

### Comparing `rqalpha-5.3.9/CHANGELOG.rst` & `rqalpha-5.4.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/LICENSE` & `rqalpha-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/PKG-INFO` & `rqalpha-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.3.9
+Version: 5.4.0
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.3.9/README.rst` & `rqalpha-5.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/__init__.py` & `rqalpha-5.4.0/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/__main__.py` & `rqalpha-5.4.0/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/api.py` & `rqalpha-5.4.0/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/apis/__init__.py` & `rqalpha-5.4.0/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/apis/api_abstract.py` & `rqalpha-5.4.0/rqalpha/apis/api_abstract.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/apis/api_base.py` & `rqalpha-5.4.0/rqalpha/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/apis/api_rqdatac.py` & `rqalpha-5.4.0/rqalpha/apis/api_rqdatac.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/apis/names.py` & `rqalpha-5.4.0/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/cmds/__init__.py` & `rqalpha-5.4.0/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/cmds/bundle.py` & `rqalpha-5.4.0/rqalpha/cmds/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/cmds/entry.py` & `rqalpha-5.4.0/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/cmds/misc.py` & `rqalpha-5.4.0/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/cmds/mod.py` & `rqalpha-5.4.0/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/cmds/run.py` & `rqalpha-5.4.0/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/config.yml` & `rqalpha-5.4.0/rqalpha/config.yml`

 * *Files 17% similar despite different names*

```diff
@@ -37,14 +37,19 @@
   round_price: false
   # 用户自定义的期货合约数据，用于设置期货手续菲费率
   future_info: {}
   # 强平
   forced_liquidation: true
   # 是否开启期货历史交易参数进行回测，默认为 False
   futures_time_series_trading_parameters: false
+  # 是否开启在回测过程中自动下载所需的 bundle 数据
+  # 当前支持数据：1. 盘前集合竞价成交量；2. 期货历史交易参数
+  auto_update_bundle: false
+  # 自动下载的 bundle 文件支持单独设置存储路径，若不设置则使用 data_bundle_path 路径
+  auto_update_bundle_path: ~
 
 
 extra:
   # 选择日期的输出等级，有 `verbose` | `info` | `warning` | `error` 等选项，您可以通过设置 `verbose` 来查看最详细的日志，
   # 或者设置 `error` 只查看错误级别的日志输出
   log_level: info
   # 通过该参数可以将预定义变量传入 `context` 内。
```

### Comparing `rqalpha-5.3.9/rqalpha/const.py` & `rqalpha-5.4.0/rqalpha/const.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/__init__.py` & `rqalpha-5.4.0/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/events.py` & `rqalpha-5.4.0/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/execution_context.py` & `rqalpha-5.4.0/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/executor.py` & `rqalpha-5.4.0/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/global_var.py` & `rqalpha-5.4.0/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/strategy.py` & `rqalpha-5.4.0/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/strategy_context.py` & `rqalpha-5.4.0/rqalpha/core/strategy_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/strategy_loader.py` & `rqalpha-5.4.0/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/core/strategy_universe.py` & `rqalpha-5.4.0/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/__init__.py` & `rqalpha-5.4.0/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/bar_dict_price_board.py` & `rqalpha-5.4.0/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/base_data_source/__init__.py` & `rqalpha-5.4.0/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/base_data_source/adjust.py` & `rqalpha-5.4.0/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/base_data_source/data_source.py` & `rqalpha-5.4.0/rqalpha/data/base_data_source/data_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from itertools import groupby
 from typing import Dict, Iterable, List, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 import six
 from rqalpha.utils.i18n import gettext as _
-from rqalpha.const import INSTRUMENT_TYPE, TRADING_CALENDAR_TYPE, DEFAULT_ACCOUNT_TYPE
+from rqalpha.const import INSTRUMENT_TYPE, TRADING_CALENDAR_TYPE
 from rqalpha.interface import AbstractDataSource
 from rqalpha.model.instrument import Instrument
 from rqalpha.utils.datetime_func import (convert_date_to_int, convert_int_to_date, convert_int_to_datetime)
-from rqalpha.utils.exception import RQInvalidArgument, RQDatacVersionTooLow
+from rqalpha.utils.exception import RQInvalidArgument
 from rqalpha.utils.functools import lru_cache
 from rqalpha.utils.typing import DateLike
 from rqalpha.environment import Environment
-from rqalpha.data.bundle import update_futures_trading_parameters
-from rqalpha.utils.logger import user_system_log
 from rqalpha.data.base_data_source.adjust import FIELDS_REQUIRE_ADJUSTMENT, adjust_bars
 from rqalpha.data.base_data_source.storage_interface import (AbstractCalendarStore, AbstractDateSet,
                                 AbstractDayBarStore, AbstractDividendStore,
                                 AbstractInstrumentStore)
 from rqalpha.data.base_data_source.storages import (DateSet, DayBarStore, DividendStore,
                        ExchangeTradingCalendarStore, FutureDayBarStore,
-                       FutureInfoStore, FuturesTradingParametersStore,InstrumentStore,
+                       FutureInfoStore,InstrumentStore,
                        ShareTransformationStore, SimpleFactorStore,
                        YieldCurveStore, FuturesTradingParameters)
 
 
 BAR_RESAMPLE_FIELD_METHODS = {
     "open": "first",
     "close": "last",
@@ -68,16 +66,15 @@
 
 class BaseDataSource(AbstractDataSource):
     DEFAULT_INS_TYPES = (
         INSTRUMENT_TYPE.CS, INSTRUMENT_TYPE.FUTURE, INSTRUMENT_TYPE.ETF, INSTRUMENT_TYPE.LOF, INSTRUMENT_TYPE.INDX,
         INSTRUMENT_TYPE.PUBLIC_FUND,
     )
 
-    def __init__(self, path, custom_future_info, futures_time_series_trading_parameters=False, end_date=None):       
-        # type: (str, dict, bool, date) -> None
+    def __init__(self, path: str, custom_future_info: dict, *args, **kwargs) -> None:
         if not os.path.exists(path):
             raise RuntimeError('bundle path {} not exist'.format(os.path.abspath(path)))
 
         def _p(name):
             return os.path.join(path, name)
 
         funds_day_bar_store = DayBarStore(_p('funds.h5'))
@@ -85,30 +82,30 @@
             INSTRUMENT_TYPE.CS: DayBarStore(_p('stocks.h5')),
             INSTRUMENT_TYPE.INDX: DayBarStore(_p('indexes.h5')),
             INSTRUMENT_TYPE.FUTURE: FutureDayBarStore(_p('futures.h5')),
             INSTRUMENT_TYPE.ETF: funds_day_bar_store,
             INSTRUMENT_TYPE.LOF: funds_day_bar_store
         }  # type: Dict[INSTRUMENT_TYPE, AbstractDayBarStore]
         
-        self._futures_trading_parameters_store = None
         self._future_info_store = FutureInfoStore(_p("future_info.json"), custom_future_info)
         
         self._instruments_stores = {}  # type: Dict[INSTRUMENT_TYPE, AbstractInstrumentStore]
         self._ins_id_or_sym_type_map = {}  # type: Dict[str, INSTRUMENT_TYPE]
         instruments = []
         
+        env = Environment.get_instance()
         with open(_p('instruments.pk'), 'rb') as f:
             for i in pickle.load(f):
                 if i["type"] == "Future" and Instrument.is_future_continuous_contract(i["order_book_id"]):
                     i["listed_date"] = datetime(1990, 1, 1)
                 instruments.append(Instrument(
                     i, 
                     lambda i: self._future_info_store.get_tick_size(i),
-                    lambda i, dt: self.get_futures_trading_parameters(i, dt).long_margin_ratio,
-                    lambda i, dt: self.get_futures_trading_parameters(i, dt).short_margin_ratio
+                    # lambda i, dt: env.data_proxy.get_futures_trading_parameters(i, dt).long_margin_ratio,
+                    # lambda i, dt: env.data_proxy.get_futures_trading_parameters(i, dt).short_margin_ratio
                     ))
         for ins_type in self.DEFAULT_INS_TYPES:
             self.register_instruments_store(InstrumentStore(instruments, ins_type))
         dividend_store = DividendStore(_p('dividends.h5'))
         self._dividends = {
             INSTRUMENT_TYPE.CS: dividend_store,
             INSTRUMENT_TYPE.ETF: dividend_store,
@@ -129,28 +126,14 @@
         }
         self._ex_cum_factor = SimpleFactorStore(_p('ex_cum_factor.h5'))
         self._share_transformation = ShareTransformationStore(_p('share_transformation.json'))
 
         self._suspend_days = [DateSet(_p('suspended_days.h5'))]  # type: List[AbstractDateSet]
         self._st_stock_days = DateSet(_p('st_stock_days.h5'))
 
-        if futures_time_series_trading_parameters:
-            try:
-                import rqdatac
-            except ImportError:
-                user_system_log.warn(_("RQDatac is not installed, \"config.base.futures_time_series_trading_parameters\" will be disabled."))
-            else:
-                try:
-                    update_futures_trading_parameters(path, end_date)
-                except (rqdatac.share.errors.PermissionDenied, RQDatacVersionTooLow):
-                    user_system_log.warn(_("RQDatac does not have permission to obtain futures histrical trading parameters, \"config.base.futures_time_series_trading_parameters\" will be disabled."))
-                else:
-                    file = os.path.join(path, "futures_trading_parameters.h5")
-                    self._futures_trading_parameters_store = FuturesTradingParametersStore(file, custom_future_info)
-
     def register_day_bar_store(self, instrument_type, store):
         #  type: (INSTRUMENT_TYPE, AbstractDayBarStore) -> None
         self._day_bars[instrument_type] = store
 
     def register_instruments_store(self, instruments_store):
         # type: (AbstractInstrumentStore) -> None
         instrument_type = instruments_store.instrument_type
@@ -378,23 +361,16 @@
             s, e = self._day_bars[INSTRUMENT_TYPE.INDX].get_date_range('000001.XSHG')
             return convert_int_to_date(s).date(), convert_int_to_date(e).date()
 
     def get_yield_curve(self, start_date, end_date, tenor=None):
         return self._yield_curve.get_yield_curve(start_date, end_date, tenor=tenor)
 
     @lru_cache(1024)
-    def get_futures_trading_parameters(self, instrument, dt):
-        # type: (Instrument, datetime.date) -> FuturesTradingParameters
-        if self._futures_trading_parameters_store:
-            trading_parameters = self._futures_trading_parameters_store.get_futures_trading_parameters(instrument, dt)
-            if trading_parameters is None:
-                return self._future_info_store.get_future_info(instrument.order_book_id, instrument.underlying_symbol)
-            return trading_parameters
-        else:
-            return self._future_info_store.get_future_info(instrument.order_book_id, instrument.underlying_symbol)
+    def get_futures_trading_parameters(self, instrument: Instrument, dt: datetime.date) -> FuturesTradingParameters:
+        return self._future_info_store.get_future_info(instrument.order_book_id, instrument.underlying_symbol)
 
     def get_merge_ticks(self, order_book_id_list, trading_date, last_dt=None):
         raise NotImplementedError
 
     def history_ticks(self, instrument, count, dt):
         raise NotImplementedError
```

### Comparing `rqalpha-5.3.9/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-5.4.0/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/base_data_source/storages.py` & `rqalpha-5.4.0/rqalpha/data/base_data_source/storages.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             self._default_data = {
                 item.get("order_book_id") or item.get("underlying_symbol"): self._process_future_info_item(
                     item
                 ) for item in json.load(json_file)
             }
         self._custom_data = custom_future_info
         if "margin_rate" not in self._default_data[next(iter(self._default_data))]:
-            raise RuntimeError(_("Your bundle data is too old, please use 'rqalpha update-bundle' or 'rqalpha download-bundle' to update it to lastest before using"))
+            raise RuntimeError(_("The bundle data you are using is too old, please update it to lastest before using"))
 
     @classmethod
     def _process_future_info_item(cls, item):
         item["commission_type"] = cls.COMMISSION_TYPE_MAP[item["commission_type"]]
         return item
 
     @lru_cache(1024)
@@ -243,80 +243,14 @@
                 return 20050104, 20050104
 
 
 class FutureDayBarStore(DayBarStore):
     DEFAULT_DTYPE = np.dtype(DayBarStore.DEFAULT_DTYPE.descr + [("open_interest", '<f8')])
 
 
-class FuturesTradingParametersStore(object):
-    COMMISSION_TYPE_MAP = {
-        0: COMMISSION_TYPE.BY_MONEY,
-        1: COMMISSION_TYPE.BY_VOLUME
-    }
-
-    # 历史期货交易参数的数据在2010年4月之后才有
-    FUTURES_TRADING_PARAMETERS_START_DATE = 20100401
-
-    def __init__(self, path, custom_future_info):
-        self._path = path
-        self._custom_data = custom_future_info
-
-    def get_futures_trading_parameters(self, instrument, dt):
-        # type: (Instrument, datetime.date) -> FuturesTradingParameters or None
-        dt = convert_date_to_date_int(dt)
-        if dt < self.FUTURES_TRADING_PARAMETERS_START_DATE:
-            return None
-        order_book_id = instrument.order_book_id
-        underlying_symbol = instrument.underlying_symbol
-        data = self.get_futures_trading_parameters_all_time(order_book_id)
-        if data is None: 
-            return None
-        else:
-            arr = data[data['datetime'] == dt]
-            if len(arr) == 0:
-                if dt >= convert_date_to_date_int(instrument.listed_date) and dt <= convert_date_to_date_int(instrument.de_listed_date):
-                    user_system_log.info("Historical futures trading parameters are abnormal, the lastst parameters will be used for calculations.\nPlease contract RiceQuant to repair: 0755-26569969")
-                return None
-            custom_info = self._custom_data.get(order_book_id) or self._custom_data.get(underlying_symbol)
-            if custom_info:
-                arr[0] = self.set_custom_info(arr[0], custom_info)        
-            futures_trading_parameters = self._to_namedtuple(arr[0])
-        return futures_trading_parameters
-    
-    @lru_cache(1024)
-    def get_futures_trading_parameters_all_time(self, order_book_id):
-        # type: (str) -> numpy.ndarray or None
-        with h5_file(self._path) as h5:
-            try:
-                data = h5[order_book_id][:]
-            except KeyError:
-                return None
-        return data
-    
-    def set_custom_info(self, arr, custom_info):
-        for field in custom_info:
-            if field == "commission_type":
-                if custom_info[field] == COMMISSION_TYPE.BY_MONEY:
-                    value = 0
-                elif custom_info[field] == COMMISSION_TYPE.BY_VOLUME:
-                    value = 1
-            else:
-                value = custom_info[field]
-            arr[field] = value
-        return arr
-            
-    def _to_namedtuple(self, arr):
-        # type: (numpy.void) -> FuturesTradingParameters
-        dic = dict(zip(arr.dtype.names, arr))
-        del dic['datetime']
-        dic["commission_type"] = self.COMMISSION_TYPE_MAP[dic['commission_type']]
-        futures_trading_parameters = FuturesTradingParameters(**dic)
-        return futures_trading_parameters
-
-
 class DividendStore(AbstractDividendStore):
     def __init__(self, path):
         self._path = path
 
     def get_dividend(self, order_book_id):
         with h5_file(self._path) as h5:
             try:
```

### Comparing `rqalpha-5.3.9/rqalpha/data/bundle.py` & `rqalpha-5.4.0/rqalpha/data/bundle.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,28 +14,23 @@
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 import datetime
 import json
 import os
 import pickle
 import re
 from itertools import chain
-from typing import Callable, Optional, List
+from typing import Callable, Optional, Union, List
+from filelock import FileLock, Timeout
 
 import h5py
 import numpy as np
-import pandas as pd
 from rqalpha.apis.api_rqdatac import rqdatac
-from rqalpha.utils.concurrent import (ProgressedProcessPoolExecutor,
-                                      ProgressedTask)
-from rqalpha.utils.datetime_func import (convert_date_to_date_int,
-                                         convert_date_to_int,)
-from rqalpha.utils.exception import RQDatacVersionTooLow
+from rqalpha.utils.concurrent import ProgressedProcessPoolExecutor, ProgressedTask
+from rqalpha.utils.datetime_func import convert_date_to_date_int, convert_date_to_int
 from rqalpha.utils.i18n import gettext as _
-from rqalpha.utils.logger import system_log
-from rqalpha.const import TRADING_CALENDAR_TYPE
 from rqalpha.utils.functools import lru_cache
 from rqalpha.environment import Environment
 from rqalpha.model.instrument import Instrument
 
 START_DATE = 20050104
 END_DATE = 29991231
 
@@ -441,213 +436,28 @@
         # windows上子进程需要执行rqdatac.init, 其他os则需要执行rqdatac.reset; rqdatac.init包含了rqdatac.reset的功能
         for func in gen_file_funcs:
             executor.submit(GenerateFileTask(func), path)
         for file, order_book_id, field in day_bar_args:
             executor.submit(_DayBarTask(order_book_id), os.path.join(path, file), field, **kwargs)
 
 
-FUTURES_TRADING_PARAMETERS_FIELDS = ["long_margin_ratio", "short_margin_ratio", "commission_type", "open_commission", "close_commission", "close_commission_today"]
-TRADING_PARAMETERS_START_DATE = 20100401
-FUTURES_TRADING_PARAMETERS_FILE = "futures_trading_parameters.h5"
-
-
-class FuturesTradingParametersTask(object):
-    def __init__(self, order_book_ids, underlying_symbols):
-        self._order_book_ids = order_book_ids
-        self._underlying_symbols = underlying_symbols
-    
-    def __call__(self, path, fields, end_date):
-        if rqdatac.__version__ < '2.11.12':
-            raise RQDatacVersionTooLow(_("RQAlpha already supports backtesting using futures historical margins and rates, please upgrade RQDatac to version 2.11.12 and above to use it"))
-            
-        if not os.path.exists(path):
-            self.generate_futures_trading_parameters(path, fields, end_date)
-        else:
-            self.update_futures_trading_parameters(path, fields, end_date)
-    
-    def generate_futures_trading_parameters(self, path, fields, end_date, recreate_futures_list=None):
-        # type: (str, list, datetime.date, list) -> None
-        if not recreate_futures_list:
-            system_log.info(_("Futures historical trading parameters data is being updated, please wait......"))
-        order_book_ids = self._order_book_ids
-        if recreate_futures_list:
-            order_book_ids = recreate_futures_list      
-        df = rqdatac.futures.get_trading_parameters(order_book_ids, TRADING_PARAMETERS_START_DATE, end_date, fields)
-        if not (df is None or df.empty):
-            df.dropna(axis=0, how="all")
-            df.reset_index(inplace=True)
-            df['datetime'] = df['trading_date'].map(convert_date_to_date_int)
-            del df["trading_date"]
-            df['commission_type'] = df['commission_type'].map(self.set_commission_type)
-            df.rename(columns={
-                'close_commission': "close_commission_ratio",
-                'close_commission_today': "close_commission_today_ratio",
-                'open_commission': 'open_commission_ratio'
-                }, inplace=True)
-            df.set_index(["order_book_id", "datetime"], inplace=True)
-            df.sort_index(inplace=True)
-            with h5py.File(path, "w") as h5:
-                for order_book_id in df.index.levels[0]:
-                    h5.create_dataset(order_book_id, data=df.loc[order_book_id].to_records())
-        # 更新期货连续合约的历史交易参数数据（当函数执行目的为补充上次未正常更新的数据时，不需要执行此段逻辑）
-        if recreate_futures_list is None:
-            with h5py.File(path, "a") as h5:
-                df = rqdatac.all_instruments("Future")
-                for underlying_symbol in self._underlying_symbols:
-                    futures_continuous_contract = df[(df['underlying_symbol'] == underlying_symbol) & (df["listed_date"] == '0000-00-00')].order_book_id.tolist()
-                    s = rqdatac.futures.get_dominant(underlying_symbol, TRADING_PARAMETERS_START_DATE, end_date)
-                    if (s is None or s.empty):
-                        continue
-                    s = s.to_frame().reset_index()
-                    s['date'] = s['date'].map(convert_date_to_date_int)
-                    s.set_index(['date'], inplace=True)
-                    trading_parameters_list = []
-                    for date in s.index:
-                        try:
-                            data = h5[s['dominant'][date]][:]
-                        except KeyError:
-                            continue
-                        trading_parameters = data[data['datetime'] == date]
-                        if len(trading_parameters) != 0:
-                            trading_parameters_list.append(trading_parameters[0])
-                    data = np.array(trading_parameters_list)
-                    for order_book_id in futures_continuous_contract:
-                        h5.create_dataset(order_book_id, data=data)
-
-    def update_futures_trading_parameters(self, path, fields, end_date):
-        # type: (str, list, datetime.date) -> None
-        try:
-            h5 = h5py.File(path, "a")
-            h5.close()
-        except OSError as e:
-            raise OSError(_("File {} update failed, if it is using, please update later, or you can delete then update again".format(path))) from e
-        last_date = self.get_h5_last_date(path)
-        recreate_futures_list = self.get_recreate_futures_list(path, last_date)
-        if recreate_futures_list:
-            self.generate_futures_trading_parameters(path, fields, last_date, recreate_futures_list=recreate_futures_list)
-        if end_date > last_date:
-            if rqdatac.get_previous_trading_date(end_date) == last_date:
-                return
-            else:
-                system_log.info(_("Futures historical trading parameters data is being updated, please wait......"))
-                start_date = rqdatac.get_next_trading_date(last_date)
-                df = rqdatac.futures.get_trading_parameters(self._order_book_ids, start_date, end_date, fields)
-                if not(df is None or df.empty):
-                    df = df.dropna(axis=0, how="all")
-                    df.reset_index(inplace=True)
-                    df['datetime'] = df['trading_date'].map(convert_date_to_date_int)
-                    del [df['trading_date']]
-                    df['commission_type'] = df['commission_type'].map(self.set_commission_type)
-                    df.rename(columns={
-                        'close_commission': "close_commission_ratio",
-                        'close_commission_today': "close_commission_today_ratio",
-                        'open_commission': 'open_commission_ratio'
-                        }, inplace=True)
-                    df.set_index(['order_book_id', 'datetime'], inplace=True)
-                    with h5py.File(path, "a") as h5:
-                        for order_book_id in df.index.levels[0]:
-                            if order_book_id in h5:
-                                data = np.array(
-                                    [tuple(i) for i in chain(h5[order_book_id][:], df.loc[order_book_id].to_records())],
-                                    dtype=h5[order_book_id].dtype
-                                )
-                                del h5[order_book_id]
-                                h5.create_dataset(order_book_id, data=data)
-                            else:
-                                h5.create_dataset(order_book_id, data=df.loc[order_book_id].to_records())
-                # 更新期货连续合约历史交易参数
-                with h5py.File(path, "a") as h5:
-                    df = rqdatac.all_instruments("Future")
-                    for underlying_symbol in self._underlying_symbols:
-                        futures_continuous_contract = df[(df['underlying_symbol'] == underlying_symbol) & (df["listed_date"] == '0000-00-00')].order_book_id.tolist()
-                        s = rqdatac.futures.get_dominant(underlying_symbol, start_date, end_date)
-                        if (s is None or s.empty):
-                            continue
-                        s = s.to_frame().reset_index()
-                        s['date'] = s['date'].map(convert_date_to_date_int)
-                        s.set_index(['date'], inplace=True)
-                        trading_parameters_list = []
-                        for date in s.index:
-                            try:
-                                data = h5[s['dominant'][date]][:]
-                            except KeyError:
-                                continue
-                            trading_parameters = data[data['datetime'] == date]
-                            if len(trading_parameters) != 0:
-                                trading_parameters_list.append(trading_parameters[0])
-                        for order_book_id in futures_continuous_contract:
-                            if order_book_id in h5:
-                                data = np.array(
-                                    [tuple(i) for i in chain(h5[order_book_id][:], trading_parameters_list)],
-                                    dtype=h5[order_book_id].dtype
-                                )
-                                del h5[order_book_id]
-                                h5.create_dataset(order_book_id, data=data)
-                            else:
-                                h5.create_dataset(order_book_id, data=np.array(trading_parameters))
-
-    def set_commission_type(self, commission_type):
-        if commission_type == "by_money":
-            commission_type = 0
-        elif commission_type == "by_volume":
-            commission_type = 1
-        return commission_type
-    
-    def get_h5_last_date(self, path):
-        last_date = TRADING_PARAMETERS_START_DATE
-        with h5py.File(path, "r") as h5:
-            for key in h5.keys():
-                if int(h5[key]['datetime'][-1]) > last_date:
-                    last_date = h5[key]['datetime'][-1]
-        last_date = datetime.datetime.strptime(str(last_date), "%Y%m%d").date()
-        return last_date
-
-    def get_recreate_futures_list(self, path, h5_last_date):
-        # type: (str, datetime.date) -> list
-        """
-        用户在运行策略的过程中可能中断进程，进而可能导致在创建 h5 文件时，部分合约没有成功 download
-        通过该函数，获取在上一次更新中因为异常而没有更新的合约
-        """
-        recreate_futures_list = []
-        df = rqdatac.all_instruments("Future")
-        last_update_futures_list = df[(df['de_listed_date'] >= str(TRADING_PARAMETERS_START_DATE)) & (df['listed_date'] <= h5_last_date.strftime("%Y%m%d"))].order_book_id.to_list()
-        with h5py.File(path, "r") as h5:
-            h5_order_book_ids = h5.keys()
-            for order_book_id in last_update_futures_list:
-                if order_book_id in h5_order_book_ids:
-                    continue
-                else:
-                    recreate_futures_list.append(order_book_id)
-        return recreate_futures_list
-
-
-def update_futures_trading_parameters(path, end_date):
-    # type: (str, datetime.date) -> None
-    df = rqdatac.all_instruments("Future")
-    order_book_ids = (df[df['de_listed_date'] >= str(TRADING_PARAMETERS_START_DATE)]).order_book_id.tolist()
-    underlying_symbols = list(set((df[df['de_listed_date'] >= str(TRADING_PARAMETERS_START_DATE)]).underlying_symbol.tolist()))
-    FuturesTradingParametersTask(order_book_ids, underlying_symbols)(
-        os.path.join(path, FUTURES_TRADING_PARAMETERS_FILE), 
-        FUTURES_TRADING_PARAMETERS_FIELDS, 
-        end_date
-    )
-
-
 class AutomaticUpdateBundle(object):
-    def __init__(self, path: str, filename: str, api: Callable, fields: List[str], end_date: datetime.date) -> None:
+    def __init__(self, path: str, filename: str, api: Callable, fields: List[str], end_date: datetime.date, start_date: Union[int, datetime.date] = START_DATE) -> None:
         if not os.path.exists(path):
             os.makedirs(path)
         self._file = os.path.join(path, filename)
         self._trading_dates = None
         self._filename = filename
         self._api = api
         self._fields = fields
+        self._start_date = start_date
         self._end_date = end_date
         self.updated = []
         self._env = Environment.get_instance()
+        self._file_lock = FileLock(self._file + ".lock")
 
     def get_data(self, instrument: Instrument, dt: datetime.date) -> Optional[np.ndarray]:
         dt = convert_date_to_date_int(dt)
         data = self._get_data_all_time(instrument)
         if data is None:
             return data
         else:
@@ -672,42 +482,48 @@
         """
         在 rqalpha 策略运行过程中自动更新所需的日线数据
 
         :param instrument: 合约对象
         :type instrument: `Instrument`
         """
         order_book_id = instrument.order_book_id
-        start_date = START_DATE
+        start_date = self._start_date
         try:
-            h5 = h5py.File(self._file, "a")
-            if order_book_id in h5:
-                if len(h5[order_book_id][:]) != 0:
-                    last_date = datetime.datetime.strptime(str(h5[order_book_id][-1]['trading_dt']), "%Y%m%d").date()
-                    if last_date >= self._end_date:
-                        return
-                    start_date = self._env.data_proxy._data_source.get_next_trading_date(last_date).date()
-                    if start_date > self._end_date:
-                        return
-            arr = self._get_array(instrument, start_date)
-            if arr is None:
-                if order_book_id not in h5:
-                    arr = np.array([])
-                    h5.create_dataset(order_book_id, data=arr)
-            else:
-                if order_book_id in h5:
-                    data = np.array(
-                        [tuple(i) for i in chain(h5[order_book_id][:], arr)],
-                        dtype=h5[order_book_id].dtype)
-                    del h5[order_book_id]
-                    h5.create_dataset(order_book_id, data=data)
+            with self._file_lock.acquire():
+                h5 = h5py.File(self._file, "a")
+                if order_book_id in h5 and h5[order_book_id].dtype.names:
+                    if 'trading_dt' in h5[order_book_id].dtype.names:
+                        # 需要兼容此前的旧版数据，对字段名进行更新
+                        if len(h5[order_book_id][:]) != 0:
+                            last_date = datetime.datetime.strptime(str(h5[order_book_id][-1]['trading_dt']), "%Y%m%d").date()
+                            if last_date >= self._end_date:
+                                return
+                            start_date = self._env.data_proxy._data_source.get_next_trading_date(last_date).date()
+                            if start_date > self._end_date:
+                                return
+                    else:
+                        del h5[order_book_id]
+                
+                arr = self._get_array(instrument, start_date)
+                if arr is None:
+                    if order_book_id not in h5:
+                        arr = np.array([])
+                        h5.create_dataset(order_book_id, data=arr)
                 else:
-                    h5.create_dataset(order_book_id, data=arr)
-        except OSError as e:
+                    if order_book_id in h5:
+                        data = np.array(
+                            [tuple(i) for i in chain(h5[order_book_id][:], arr)],
+                            dtype=h5[order_book_id].dtype)
+                        del h5[order_book_id]
+                        h5.create_dataset(order_book_id, data=data)
+                    else:
+                        h5.create_dataset(order_book_id, data=arr)
+        except (OSError, Timeout) as e:
             raise OSError(_("File {} update failed, if it is using, please update later, "
-                          "or you can delete then update again".format(self._file))) from e 
+                          "or you can delete then update again".format(self._file))) from e
         finally:
             h5.close()
     
     def _get_array(self, instrument: Instrument, start_date: datetime.date) -> Optional[np.ndarray]:
         df = self._api(instrument.order_book_id, start_date, self._end_date, self._fields)
         if not (df is None or df.empty):
             df = df[self._fields].loc[instrument.order_book_id] # rqdatac.get_open_auction_info get Futures's data will auto add 'open_interest' and 'prev_settlement'
```

### Comparing `rqalpha-5.3.9/rqalpha/data/data_proxy.py` & `rqalpha-5.4.0/rqalpha/data/data_proxy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/data/trading_dates_mixin.py` & `rqalpha-5.4.0/rqalpha/data/trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/environment.py` & `rqalpha-5.4.0/rqalpha/environment.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-5.4.0/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/IF_macd.py` & `rqalpha-5.4.0/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/buy_and_hold.py` & `rqalpha-5.4.0/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-5.4.0/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-5.4.0/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-5.4.0/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-5.4.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-5.4.0/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/golden_cross.py` & `rqalpha-5.4.0/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/macd.py` & `rqalpha-5.4.0/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/pair_trading.py` & `rqalpha-5.4.0/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/rsi.py` & `rqalpha-5.4.0/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/run_code_demo.py` & `rqalpha-5.4.0/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/run_func_demo.py` & `rqalpha-5.4.0/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/subscribe_event.py` & `rqalpha-5.4.0/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/test_pt.py` & `rqalpha-5.4.0/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/examples/turtle.py` & `rqalpha-5.4.0/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/interface.py` & `rqalpha-5.4.0/rqalpha/interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/main.py` & `rqalpha-5.4.0/rqalpha/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,17 @@
         return
 
     try:
         import rqdatac
     except ImportError:
         return
 
-    if isinstance(rqdatac.client.get_client(), rqdatac.client.DummyClient):
+    if rqdatac.initialized():
+        return True
+    else:
         init_rqdatac_env(rqdatac_uri)
         try:
             rqdatac.init()
             return True
         except Exception as e:
             system_log.warn(_('rqdatac init failed, some apis will not function properly: {}').format(str(e)))
             return
```

### Comparing `rqalpha-5.3.9/rqalpha/mod/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,46 +90,47 @@
         return env.data_proxy.get_last_price(order_book_id)
     if isinstance(style, ALGO_ORDER_STYLES):
         price, _ = env.data_proxy.get_algo_bar(order_book_id, style, env.calendar_dt)
         return price
     raise RuntimeError(f"no support {style} order style")
 
 
-def _submit_order(ins, amount, side, position_effect, style, current_quantity, auto_switch_order_value):
+def _submit_order(ins, amount, side, position_effect, style, current_quantity, auto_switch_order_value, zero_amount_as_exception=True):
     env = Environment.get_instance()
     if isinstance(style, LimitOrder) and np.isnan(style.get_limit_price()):
         raise RQInvalidArgument(_(u"Limit order price should not be nan."))
     price = env.data_proxy.get_last_price(ins.order_book_id)
     if not is_valid_price(price):
         reason = _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id)
         env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
         return
 
     if (side == SIDE.BUY and current_quantity != -amount) or (side == SIDE.SELL and current_quantity != abs(amount)):
         # 在融券回测中，需要用买单作为平空，对于此种情况下出现的碎股，亦允许一次性申报卖出
         amount = _round_order_quantity(ins, amount)
 
     if amount == 0:
-        reason = _(u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}").format(order_book_id=ins.order_book_id)
-        env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
+        if zero_amount_as_exception:
+            reason = _(u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}").format(order_book_id=ins.order_book_id)
+            env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
         return
     order = Order.__from_create__(ins.order_book_id, abs(amount), side, style, position_effect)
     if side == SIDE.BUY and auto_switch_order_value:
         account, position, ins = _get_account_position_ins(ins)
         if validate_cash(env, order, account.cash):
             user_system_log.warn(_(
                 "insufficient cash, use all remaining cash({}) to create order"
             ).format(account.cash))
             return _order_value(account, position, ins, account.cash, style)
     return env.submit_order(order)
 
 
-def _order_shares(ins, amount, style, quantity, auto_switch_order_value):
+def _order_shares(ins, amount, style, quantity, auto_switch_order_value, zero_amount_as_exception=True):
     side, position_effect = (SIDE.BUY, POSITION_EFFECT.OPEN) if amount > 0 else (SIDE.SELL, POSITION_EFFECT.CLOSE)
-    return _submit_order(ins, amount, side, position_effect, style, quantity, auto_switch_order_value)
+    return _submit_order(ins, amount, side, position_effect, style, quantity, auto_switch_order_value, zero_amount_as_exception)
 
 
 def _order_value(account, position, ins, cash_amount, style, zero_amount_as_exception=True):
     env = Environment.get_instance()
     if cash_amount > 0:
         cash_amount = min(cash_amount, account.cash)
     if isinstance(style, LimitOrder):
@@ -157,15 +158,15 @@
                 reason = _(u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}").format(order_book_id=ins.order_book_id)
                 env.order_creation_failed(order_book_id=ins.order_book_id, reason=reason)
             return
 
     if amount < 0:
         amount = max(amount, -position.closable)
 
-    return _order_shares(ins, amount, style, position.quantity, auto_switch_order_value=False)
+    return _order_shares(ins, amount, style, position.quantity, auto_switch_order_value=False, zero_amount_as_exception=zero_amount_as_exception)
 
 
 @order_shares.register(INST_TYPE_IN_STOCK_ACCOUNT)
 def stock_order_shares(id_or_ins, amount, price_or_style=None, price=None, style=None):
     auto_switch_order_value = Environment.get_instance().config.mod.sys_accounts.auto_switch_order_value
     account, position, ins = _get_account_position_ins(id_or_ins)
     return _order_shares(
```

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,23 +78,21 @@
             'portfolio_daily_returns': [float(v) for v in self._portfolio_daily_returns],
             'total_portfolios': self._total_portfolios,
             'total_benchmark_portfolios': self._total_benchmark_portfolios,
             'sub_accounts': self._sub_accounts,
             'positions': self._positions,
             'orders': self._orders,
             'trades': self._trades,
-            'daily_pnl': self._daily_pnl,
+            'daily_pnl': self._daily_pnl
         }).encode('utf-8')
 
     def set_state(self, state):
         value = jsonpickle.loads(state.decode('utf-8'))
-        self._benchmark_daily_returns = value['benchmark_daily_returns']
         self._portfolio_daily_returns = value["portfolio_daily_returns"]
         self._total_portfolios = value['total_portfolios']
-        self._total_benchmark_portfolios = value["total_benchmark_portfolios"]
         self._sub_accounts = value['sub_accounts']
         self._positions = value["positions"]
         self._orders = value['orders']
         self._trades = value["trades"]
         self._daily_pnl = value.get("daily_pnl", [])
 
     def start_up(self, env, mod_config):
@@ -176,15 +174,15 @@
                     "date {}").format(order_book_id, available_s, _s, available_e, _e)
                 )
         self._benchmark_daily_returns = self._benchmark_daily_returns / weight
         
         # generate benchmark portfolio
         unit_net_value = (self._benchmark_daily_returns + 1).cumprod()
         self._total_benchmark_portfolios = {
-            "date": trading_dates,
+            "date": list(trading_dates.date),
             "unit_net_value": unit_net_value
         }
 
     def _subscribe_events(self, event):
         self._env.event_bus.add_listener(EVENT.BEFORE_STRATEGY_RUN, self.generate_benchmark_daily_returns_and_portfolio)
         self._env.event_bus.add_listener(EVENT.TRADE, self._collect_trade)
         self._env.event_bus.add_listener(EVENT.ORDER_CREATION_PASS, self._collect_order)
```

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         data["annual_tracking_error"].append(risk.annual_tracking_error)
         data["weekly_excess_win_rate"].append(weekly_excess_win_rate)
         data["monthly_excess_win_rate"].append(monthly_excess_win_rate)
         data["excess_annual_volatility"].append(risk.excess_annual_volatility)
         data["annual_volatility"].append(risk.annual_volatility)
         data["max_drawdown"].append(risk.max_drawdown)
         data["max_drawdown_days"].append((max_dd.end_date - max_dd.start_date).days)
+        data["alpha"].append(risk.alpha)
+        data["beta"].append(risk.beta)
     return data
 
 
 def _monthly_returns(p_returns: Series):
     data = DataFrame(index=p_returns.index.year.unique(), columns=list(range(1, 13)))
     for year, p_year_returns in p_returns.groupby(p_returns.index.year):
         for month, p_month_returns in p_year_returns.groupby(p_year_returns.index.month):
```

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx`

 * *Files 11% similar despite different names*

```diff
@@ -109,1350 +109,1354 @@
 000006c0: af69 cb7a 6fc9 a523 2b90 a644 ce90 59f8  .i.zo..#+..D..Y.
 000006d0: 90d9 42ea f335 a256 a1a5 24c1 b07e cae9  ..B..5.V..$..~..
 000006e0: 88ca fb22 6303 1e27 5afd 9fe8 ef6b d152  ..."c..'Z....k.R
 000006f0: 5246 2585 9a03 9de6 f9ec 3805 b4bc a445  RF%.......8....E
 00000700: 7313 7fdc 9946 7ce7 30bc 320f a758 6e2f  s....F|.0.2..Xn/
 00000710: c9a2 f731 b13d 63ce 57cf 3712 cede b2fa  ...1.=c.W.7.....
 00000720: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00000730: 0000 0021 00fc 9a79 c6cb 0300 00fe 0900  ...!...y........
+00000730: 0000 0021 0088 e43b c8ce 0300 00fe 0900  ...!...;........
 00000740: 000f 0000 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
 00000750: 2e78 6d6c ac56 4d6f db46 10bd 17e8 7f60  .xml.VMo.F.....`
-00000760: 173e 3440 697e 88a4 54c2 5260 cb56 23a0  .>4@i~..T.R`.V#.
-00000770: 4d8c c649 2e02 8835 b932 1726 77e9 e5d2  M..I...5.2.&w...
-00000780: 9210 e492 a2b0 9bb4 3d35 a734 40da 430a  ........=5.4@.C.
-00000790: f4d2 4b1b b445 fa6f 62d5 39e5 2f74 4889  ..K..E.ob.9./tH.
-000007a0: 322d c588 9a98 12f7 83cb 79f3 66f6 cd4a  2-........y.f..J
-000007b0: 6b57 8771 a41c 1291 52ce 9ac8 58d5 9142  kW.q....R...X..B
-000007c0: 98cf 03ca f69a e8d6 4e47 6d20 2595 9805  ........NGm %...
-000007d0: 38e2 8c34 d188 a4e8 6aeb c30f d606 5cec  8..4....j.....\.
-000007e0: ef72 beaf 0000 4b9b 2894 3271 352d f543  .r....K.(.2q5-.C
-000007f0: 12e3 7495 2784 c14a 9f8b 184b 988a 3d2d  ..t.'..J...K..=-
-00000800: 4d04 c141 1a12 22e3 4833 75dd d162 4c19  M..A..".H3u..bL.
-00000810: 9a20 b862 190c deef 539f 6c72 3f8b 0993  . .b....S.lr?...
-00000820: 1310 4122 2c81 7e1a d224 2dd1 627f 19b8  ..A",.~..$-.b...
-00000830: 188b fd2c 517d 1e27 00b1 4b23 2a47 0528  ...,Q}.'..K#*G.(
-00000840: 5262 dfed ee31 2ef0 6e04 610f 0d5b 190a  Rb...1..n.a..[..
-00000850: f83a 701b 3a34 66e9 0996 165c c5d4 173c  .:p.:4f....\...<
-00000860: e57d b90a d0da 84f4 42fc 86ae 19c6 b914  .}......B.......
-00000870: 0c17 73b0 1c92 a509 7248 f33d 9cb1 12ce  ..s.....rH.=....
-00000880: 3bb2 7266 58ce 1998 a1bf 379a 01d2 2ab4  ;.rfX.....7...*.
-00000890: e242 f2de 11cd 9e71 3351 6bad 4f23 727b  .B.....q3Qk.O#r{
-000008a0: 225d 0527 c975 1ce7 3b15 2125 c2a9 dc0a  "].'.u..;.!%....
-000008b0: a824 4113 d561 ca07 e4ec 818d 1491 251b  .$A..a........%.
-000008c0: 198d 60d5 ac5b a68d b4d6 4cce db02 26b0  ..`..[....L...&.
-000008d0: f7eb 9124 8261 49da 9c49 90da 94fa fbca  ...$.aI..I......
-000008e0: aac0 6e87 1c44 ac7c 490e 322a 08d4 0e48  ..n..D.|I.2*...H
-000008f0: 08c2 8116 fb2e de4d b7b1 0c95 4c44 4db4  .......M....LDM.
-00000900: e5f6 da3c 203d 01ef 1f64 98c9 9e38 c051  ...< =...d...8.Q
-00000910: 12e2 591f f3a0 1c7b 30f6 d251 ea61 86a3  ..Y....{0..Q.a..
-00000920: 514a 444f 9084 0bd9 9324 4ea0 4448 daab  QJDO.....$N.DH..
-00000930: 6816 2f16 c8ff 502d f6f3 a469 90a8 4930  h./...P-...i..I0
-00000940: 93f1 7cd2 2026 e196 cadc 9642 8171 77f3  ..|. &.....B.qw.
-00000950: 73d8 9d9b f810 f60a 1411 4c4b b90b 9b61  s.........LK...a
-00000960: d43c e60b d7f0 ee5a ed76 c3da f8b4 a63a  .<.....Z.v.....:
-00000970: 96d3 562d 5baf ab1b 8ea9 abba 6d77 6cd3  ..V-[.......mwl.
-00000980: d01b 1bb6 790f 8211 8eeb 739c c970 2a83  ....y.....s..p*.
-00000990: 1cba 892c d8f3 85a5 2ff0 b05c 3174 37a3  ...,..../..\1t7.
-000009a0: c119 8dbb faf4 52f3 7eae 29d7 eee5 01e7  ......R.~.).....
-000009b0: 07de 6d4a 06e9 9960 f2a9 32bc 4359 c007  ..mJ...`..2.CY..
-000009c0: 4d54 6b98 0d88 6a54 ce55 b30e d341 b17a  MTk...jT.U...A.z
-000009d0: 8706 32cc 5f71 acd9 b36b 84ee 8540 d934  ..2._q...k...@.4
-000009e0: ccfc 2154 464e ad89 ce51 da9c 50ea c0a5  ..!TFN...Q..P...
-000009f0: e6cd 394a 5a85 5371 b602 b7a2 5758 510f  ..9JZ.Sq....WXQ.
-00000a00: e367 f74f 7f39 8643 3c3f 778b 2c83 fedd  .g.O.9.C<?w.,...
-00000a10: dc87 e806 461e 54f5 ed93 bf7e 3ff9 fbd9  ....F.T....~?...
-00000a20: f8db a3f1 d3a3 8a0d 1c76 331b 73de 66fc  .........v3.s.f.
-00000a30: e371 6ef3 c3f3 7f1f 3fa8 d8d4 2a36 b537  .qn.....?...*6.7
-00000a40: db9c 3eff fad5 cf4f 2696 af5f 1c9f 1c3d  ..>....O&.._...=
-00000a50: 7df9 cfa3 d72f bea9 a058 1514 6b1e e5e5  }..../...X..k...
-00000a60: 9fbf 9ede ff69 fce4 ab57 47df 556c f20a  .....i...WG.Ul..
-00000a70: 2f23 2c8a fb5c 84df 3f3c 79f0 78fc c7c3  /#,..\..?<y.x...
-00000a80: d3df 1e55 6c40 3233 1ba7 d076 99cc 80f4  ...Ul@23...v....
-00000a90: 2923 417e ba40 6a2b b369 8203 4ca3 91e7  )#A~.@j+.i..L...
-00000aa0: 0550 609e cf33 2651 ab7d e3d6 f59d f58f  .P`..3&Q.}......
-00000ab0: abf4 3e5a 5977 57d6 afa8 c69a 5681 780b  ..>ZYwW.....V.x.
-00000ac0: 5e8a 5a37 3a9d 9b5b 3bf3 502b e627 3a7c  ^.Z7:..[;.P+.':|
-00000ad0: 165c 5f59 167d 50e8 ce83 b3ef cd1e 3a97  .\_Y.}P.......:.
-00000ae0: e5c1 d62f f0f0 d965 79a8 5f14 c3b5 cbf2  .../...ey._.....
-00000af0: 10e3 e105 4174 2fcd 05c1 ec02 1fed 657d  ....At/.......e}
-00000b00: 5485 054a f571 e46f 0b25 ef8a b2b7 2c7b  T..J.q.o.%....,{
-00000b10: f253 a795 7fdd 5aff 0100 00ff ff03 0050  .S....Z........P
-00000b20: 4b03 0414 0006 0008 0000 0021 000e 1564  K..........!...d
-00000b30: c916 0100 007b 0500 001a 0008 0178 6c2f  .....{.......xl/
-00000b40: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
-00000b50: 6d6c 2e72 656c 7320 a204 0128 a000 0100  ml.rels ...(....
-00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000760: 173e 3440 6992 1225 3384 a5c0 96ac 4640  .>4@i..%3.....F@
+00000770: 9b18 8d93 5c04 106b 7265 2e4c eed2 bb4b  ....\..kre.L...K
+00000780: 4b42 904b 8ac2 6ed2 f6d4 9cd2 0069 0f29  KB.K..n......i.)
+00000790: d04b 2f6d d016 e9bf 8955 e794 bfd0 2125  .K/m.....U....!%
+000007a0: cab4 14a3 6a62 4adc 0f2e e7cd 9bd9 372b  ....jbJ.......7+
+000007b0: ad5f 1bc6 9176 4884 a49c 3590 b56a 228d  ._...vH...5..j".
+000007c0: 309f 0794 ed35 d0ed 9d8e ee20 4d2a cc02  0....5..... M*..
+000007d0: 1c71 461a 6844 24ba d6fc f083 f501 17fb  .qF.hD$.........
+000007e0: bb9c ef6b 00c0 6403 854a 25ae 6148 3f24  ...k..d..J%.aH?$
+000007f0: 3196 ab3c 210c 56fa 5cc4 58c1 54ec 1932  1..<!.V.\.X.T..2
+00000800: 1104 0732 2444 c591 5131 cdba 1163 cad0  ...2$D..Q1...c..
+00000810: 04c1 15cb 60f0 7e9f faa4 cdfd 3426 4c4d  ....`.~.....4&LM
+00000820: 4004 89b0 02fa 32a4 892c d062 7f19 b818  @.....2..,.b....
+00000830: 8bfd 34d1 7d1e 2700 b14b 23aa 4639 28d2  ..4.}.'..K#.F9(.
+00000840: 62df edee 312e f06e 0461 0fad 9a36 14f0  b...1..n.a...6..
+00000850: adc3 6d99 d054 0a4f b0b4 e02a a6be e092  ..m..T.O...*....
+00000860: f7d5 2a40 1b13 d20b f15b a661 59e7 5230  ..*@.....[.aY.R0
+00000870: 5ccc c172 48b6 21c8 21cd f670 c64a d4df  \..rH.!.!..p.J..
+00000880: 9155 7d86 553f 03b3 ccf7 46b3 405a b956  .U}.U?....F.@Z.V
+00000890: 5c48 de3b a2d5 66dc 2aa8 b9de a711 b933  \H.;..f.*......3
+000008a0: 91ae 8693 e406 8eb3 9d8a 9016 61a9 b602  ............a...
+000008b0: aa48 d040 6b30 e503 72f6 a086 3491 269b  .H.@k0..r...4.&.
+000008c0: 298d 60b5 b266 576a c868 cee4 bc2d 6002  ).`..fWj.h...-`.
+000008d0: 7bbf 1129 2218 56a4 c599 02a9 4da9 bfaf  {..)".V.....M...
+000008e0: ac72 ec56 c841 c4da 17e4 20a5 8240 ed80  .r.V.A.... ..@..
+000008f0: 8420 1c68 b1ef e25d b98d 55a8 a522 6aa0  . .h...]..U.."j.
+00000900: 2db7 d7e2 01e9 0978 ff20 c54c f5c4 018e  -......x. .L....
+00000910: 9210 cffa 9807 c5d8 83b1 2747 d2c3 0c47  ..........'G...G
+00000920: 2349 444f 9084 0bd5 5324 4ea0 4488 ec95  #IDO....S$N.D...
+00000930: 348b 170b e47f a816 fb59 d20c 48d4 2498  4........Y..H.$.
+00000940: c978 3e69 1093 700b 656e 2ba1 c1b8 dbfe  .x>i..p.en+.....
+00000950: 0c76 e716 3e84 bd02 4504 d352 eec2 6658  .v..>...E..R..fX
+00000960: 558f f9c2 b5bc 7bb6 d96e 5b95 96a3 6f6d  U.....{..n[...om
+00000970: 6e3a badd 72ae ea8e d369 eb56 c7de ec58  n:..r....i.V...X
+00000980: d5aa ed98 95fb 108c a8bb 3ec7 a90a a732  ..........>....2
+00000990: c8a0 1bc8 863d 5f58 fa1c 0f8b 15cb 7453  .....=_X......tS
+000009a0: 1a9c d1b8 674e 2f3d ebe7 9a62 ed7e 1670  ....gN/=...b.~.p
+000009b0: 76e0 dda1 6420 cf04 934d b5e1 5dca 023e  v...d ...M..]..>
+000009c0: 0007 f65a 1da2 1a15 f36a fd2a 4c07 f9ea  ...Z.....j.*L...
+000009d0: 5d1a a810 24e7 38e6 ecd9 7542 f742 a06c  ]...$.8...uB.B.l
+000009e0: d5ec 2a08 132a 23a3 d640 e728 b527 943a  ..*..*#..@.(.'.:
+000009f0: 70e9 5973 8e92 51e2 949f adc0 2def 3596  p.Ys..Q.....-.5.
+00000a00: d7c3 f8f9 83d3 9f8f e110 cfce dd3c cba0  .............<..
+00000a10: 7f37 f321 ba81 9505 557e fbe4 cfdf 4efe  .7.!....U~....N.
+00000a20: 7a3e fee6 68fc eca8 6403 87dd cca6 326f  z>..h...d.....2o
+00000a30: 33fe e138 b3f9 fec5 3f4f 1e96 6caa 259b  3..8....?O..l.%.
+00000a40: eadb 6d4e 5f7c f5fa a7a7 13cb 372f 8f4f  ..mN_|......7/.O
+00000a50: 8e9e bdfa fbf1 9b97 5f97 50ec 128a 3d8f  ........_.P...=.
+00000a60: f2ea 8f5f 4e1f fc38 7efa e5eb a36f 4b36  ..._N..8~....oK6
+00000a70: 5985 1711 e6c5 7d2e c2ef 1e9d 3c7c 32fe  Y.....}.....<|2.
+00000a80: fdd1 e9af 8f4b 3620 9999 4d3d d776 91cc  .....K6 ..M=.v..
+00000a90: 80f4 2923 4176 ba40 6a4b b369 8203 4ca3  ..)#Av.@jK.i..L.
+00000aa0: 91e7 0550 609e cf53 a650 b375 f3f6 8d9d  ...P`..S.P.u....
+00000ab0: 8d8f cbf4 3e5a d970 5736 aee8 d6ba 5182  ....>Z.pW6....Q.
+00000ac0: f80f 3c89 9a37 3b9d 5b5b 3bf3 502b 954f  ..<..7;.[[;.P+.O
+00000ad0: 4cf8 2cb8 beb2 2cfa 20d7 9d07 67df db3d  L.,...,. ...g..=
+00000ae0: 742e cb43 cdbc c0c3 a797 e561 eda2 18ae  t..C.......a....
+00000af0: 5f96 8718 0f2f 08a2 7b69 2e08 6617 f868  _..../..{i..f..h
+00000b00: 2deb a32c 2c50 aa8f 237f 5b68 5997 97bd  -..,,P..#.[hY...
+00000b10: 6dd7 263f 7546 f1d7 adf9 2f00 0000 ffff  m.&?uF..../.....
+00000b20: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00000b30: 0e15 64c9 1601 0000 7b05 0000 1a00 0801  ..d.....{.......
+00000b40: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
+00000b50: 6b2e 786d 6c2e 7265 6c73 20a2 0401 28a0  k.xml.rels ...(.
+00000b60: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c50: 0000 0000 0000 0000 0000 0000 0000 00bc  ................
-00000c60: 944d 6ac3 3010 85f7 85de 4168 5fcb 7612  .Mj.0.....Ah_.v.
-00000c70: 372d 91b3 0985 6c5b f700 c21e ff10 5b32  7-....l[......[2
-00000c80: 9a49 5bdf bec2 a58d 0341 dd18 6f04 3383  .I[......A..o.3.
-00000c90: defb 3482 b7db 7f75 2dfb 008b 8dd1 9247  ..4....u-......G
-00000ca0: 41c8 19e8 dc14 8dae 247f cf5e 1eb6 9c21  A.......$..^...!
-00000cb0: 295d a8d6 6890 7c00 e4fb f4fe 6ef7 0aad  )]..h.|.....n...
-00000cc0: 2277 09eb a647 e654 344a 5e13 f5cf 4260  "w...G.T4J^...B`
-00000cd0: 5e43 a730 303d 6837 298d ed14 b9d2 56a2  ^C.00=h7).....V.
-00000ce0: 57f9 4955 20e2 304c 849d 6af0 f44a 931d  W.IU .0L..j..J..
-00000cf0: 0bc9 edb1 70fe d9d0 3be7 ffb5 4d59 3639  ....p...;...MY69
-00000d00: 1c4c 7eee 40d3 0d0b 8134 b4ee 012c 53b6  .L~.@....4...,S.
-00000d10: 0292 fca7 0e1c 2317 b7ed 5773 da7f 1a7b  ......#...Ws...{
-00000d20: c21a 802e 047f 2d14 e364 e583 799c 1386  ......-..d..y...
-00000d30: dc1f c105 642c c578 463e 8678 e185 c43e  ....d,.xF>.x...>
-00000d40: 9868 6118 ef66 9285 6112 df66 360b c36c  .ha..f..a..f6..l
-00000d50: 7c30 eb85 61d6 3e98 a759 03a5 5616 8a37  |0..a.>..Y..V..7
-00000d60: b22e 2fa7 b932 6dff c288 abc8 4cbf 0100  ../..2m.....L...
-00000d70: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00000d80: 0021 0017 9da7 7635 0600 00e3 2600 0018  .!....v5....&...
-00000d90: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00000da0: 2f73 6865 6574 312e 786d 6c9c 935d 6f9b  /sheet1.xml..]o.
-00000db0: 3014 86ef 27f5 3f58 be0f 0642 b214 8554  0...'.?X...B...T
-00000dc0: 5dab 6abd 9bd6 7d5c 3be6 10ac d898 d926  ].j...}\;......&
-00000dd0: 1f9a f6df 770c 21a9 949b a808 6cb0 7d9e  ....w.!.....l.}.
-00000de0: f73d f661 f970 d08a ecc0 3a69 9a82 2651  .=.a.p....:i..&Q
-00000df0: 4c09 34c2 94b2 d914 f4e7 8f97 c982 12e7  L.4.............
-00000e00: 7953 7265 1a28 e811 1c7d 58dd 7d5a ee8d  ySre.(...}X.}Z..
-00000e10: ddba 1ac0 1324 34ae a0b5 f76d ce98 1335  .....$4....m...5
-00000e20: 68ee 22d3 4283 3395 b19a 7bfc b41b e65a  h.".B.3...{....Z
-00000e30: 0bbc ec83 b462 691c cf99 e6b2 a103 21b7  .....bi.......!.
-00000e40: b730 4c55 4901 cf46 741a 1a3f 402c 28ee  .0LUI..Ft..?@,(.
-00000e50: d1bf ab65 eb46 9a16 b7e0 34b7 dbae 9d08  ...e.F....4.....
-00000e60: a35b 44ac a592 fed8 4329 d122 7fdd 34c6  .[D.....C)."..4.
-00000e70: f2b5 c2bc 0f49 c605 3958 bc53 7ca6 a34c  .....I..9X.S|..L
-00000e80: 3f7e a5a4 a5b0 c699 ca47 4866 83e7 ebf4  ?~.......GHf....
-00000e90: efd9 3de3 e24c bace ff26 4c92 310b 3b19  ..=..L...&L.1.;.
-00000ea0: 0ef0 824a 3f66 2999 9d59 e905 36fd 206c  ...J?f)..Y..6. l
-00000eb0: 7e86 85ed b279 27cb 82fe 8d4f d704 fb24  ~....y'....O...$
-00000ec0: 34f1 a519 e7fe d1d5 b294 78c2 212b 62a1  4.........x.!+b.
-00000ed0: 2ae8 6392 7f99 a594 ad96 7d01 fd92 b077  *.c.......}....w
-00000ee0: efde 89e7 eb37 5020 3ca0 4842 49a8 cfb5  .....7P <.HBI...
-00000ef0: 31db b0f0 1587 6244 ba7e 4140 72e1 e50e  1.....bD.~A@r...
-00000f00: 9e40 2924 6758 e27f 0691 2c08 b0b3 c2fb  .@)$gX....,.....
-00000f10: f751 eda5 afe8 6f96 9450 f14e f927 a37e  .Q....o..P.N.'.~
-00000f20: cbd2 d705 5d44 8bcf 333a 8e7f 37fb af20  ....]D..3:..7.. 
-00000f30: 37b5 2f68 1a47 c998 5adf a33f d139 6ff4  7./h.G..Z..?.9o.
-00000f40: b802 07fa 4aca cbe3 3338 81a5 8d8e a364  ....J...38.....d
-00000f50: 16ec 08a3 501b 5ba2 65f8 47b1 34f9 61c8  ....P.[.e.G.4.a.
-00000f60: 71d0 9d86 04fc 3194 299e da00 3e59 4a4e  q.....1.)...>YJN
-00000f70: 8021 1467 fb50 ecf7 4368 368f d0f1 4dc1  .!.g.P..Ch6...M.
-00000f80: 7886 83ee 7cba 40c1 13e0 94f3 9910 b6af  x...|.@.........
-00000f90: 37fc 1f00 00ff ff00 0000 ffff b49a dd6e  7..............n
-00000fa0: d340 1046 5fa5 f203 10ef 9f1d 5749 2450  .@.F_.......WI$P
-00000fb0: 2f78 8d28 4494 0b5a 5487 026f cfee ced4  /x.(D..ZT..o....
-00000fc0: d999 d9b9 1cae 50f8 981c b939 f93c eb1e  ......P....9.<..
-00000fd0: d6e7 ebf5 f674 be9d 4f87 b7d7 3f0f 6fc7  .....t..O...?.o.
-00000fe0: c10d 0feb aff3 cb9a fff6 e887 87e7 db71  ...............q
-00000ff0: f0e3 2737 b67f 72e6 f27b bdbd fefc 7afd  ..'7..r..{....z.
-00001000: f1bd 24f2 0b7f 5d3c 5f1e bffd 7bba ae97  ..$...]<_...{...
-00001010: eb4b 7e2d ffa7 349c 0e97 32f4 7399 9a63  .K~-..4...2.s..c
-00001020: 7960 fe97 35bf fc7e 1a0f bbf7 d361 77c1  y`..5..~.....aw.
-00001030: c817 8c34 09b7 2576 196e 23cc 430c 08cb  ...4..%v.n#.C...
-00001040: d44c 189a f7f7 8c10 226d 22f4 0973 c480  .L......"m"..s..
-00001050: b04c 6584 9111 42a4 254c 7dc2 6842 58a6  .Le...B.%L}.hBX.
-00001060: 32c2 8911 42a4 259c fb84 c984 b04c 6584  2...B.%......Le.
-00001070: 7b46 0891 9670 e913 4e26 8465 2a23 745c  {F...p..N&.e*#t\
-00001080: 15c8 b488 4e71 6536 612c 5339 2397 0532  ....Nqe6a,S9#..2
-00001090: 8451 b165 6fc2 58a6 66c6 fc79 dbbe 711c  .Q.eo.X.f..y..q.
-000010a0: d705 3224 a2f8 b298 3096 a99c 910b 0319  ..2$....0.......
-000010b0: c2a8 18e3 4613 c83a 9653 7269 3094 ddb9  ....F..:.Sri0...
-000010c0: 5f6d 451b 67d4 30d8 1fed 95f2 a263 20d4  _mE.g.0......c .
-000010d0: 627a c59c d255 1645 883d 4330 b93b f5bd  bz...U.E.=C0.;..
-000010e0: 8f43 d67c bb9a 5e91 a714 9605 2696 0dc1  .C.|..^.....&...
-000010f0: e4fa d4f7 3e0e 24a3 f853 3cb4 c0c4 c621  ....>.$..S<....!
-00001100: 08dc a0fa dec7 81fc d035 856c 5a27 df08  .........5.lZ'..
-00001110: 09d1 bd50 0842 0453 53c8 a67a 5ca7 7b82  ...P.B.SS..z\.{.
-00001120: 5008 42f9 eb7d fb6c 064d 219b f671 9dfa  P.B..}.l.M!..q..
-00001130: 0942 2108 e56f f83b a6a6 904d 0139 6c20  .B!..o.;...M.9l 
-00001140: 72bf 2814 8210 c1d4 14b2 e920 8725 4430  r.(........ .%D0
-00001150: 8542 1022 988a 42de a685 ea58 76cf 11b8  .B."..B....Xv...
-00001160: 4218 229f 4d45 216f d342 752c bf49 e70a  B.".ME!o.Bu,.I..
-00001170: 6128 5fd3 edb3 19b5 5dc7 68d9 e96c 3b51  a(_.....].h..l;Q
-00001180: ac3b 106a af66 5414 f236 2d54 c7f2 abc9  .;.j.fT..6-T....
-00001190: 15c2 10c1 5414 f236 2d54 c772 4cae d047  ....T..6-T.rL..G
-000011a0: 28eb 71ff a96b 0ed9 d490 ef6c 3f51 3884  (.q..k.....l?Q8.
-000011b0: 21c2 a949 64d3 43be d343 4948 2497 a0a4  !..Id.C..CIH$...
-000011c0: 4964 d343 bed3 4349 4884 a1f6 7226 cd22  Id.C..CIH...r&."
-000011d0: 9b22 f29d 224a c222 0c11 4e4d 239b 26f2  .".."J."..NM#.&.
-000011e0: 9d26 4a42 2308 9123 0ec5 a260 d344 752c  .&JB#..#...`.Du,
-000011f0: db87 12b7 0843 edcd 5c52 240a 364d 54c7  .....C..\R$.6MT.
-00001200: 32cc 894b 84a1 1673 5224 0a36 4d54 c772  2..K...sR$.6MT.r
-00001210: 4c2e 1186 08a6 76f4 6674 f6d6 d987 2671  L.....v.ft....&q
-00001220: fa06 a176 6d9b 1485 824d 13d5 b1fc 6a72  ...vm....M....jr
-00001230: 8530 4430 3585 6c8a 2874 f6a1 4928 0421  .0D05.l.(t..I(.!
-00001240: 82a9 2964 d343 017b a8dd 2e67 a110 845a  ..)d.C.{...g...Z
-00001250: cc59 53c8 a687 0256 0cc1 140a 41a8 5568  .YS....V....A.Uh
-00001260: d614 b2a9 a1d0 3991 9b85 4210 2298 9a42  ......9...B."..B
-00001270: 362d 143a 8772 b350 0842 0453 5128 dab4  6-.:.r.P.B.SQ(..
-00001280: 501d cb4c 9fb9 4218 2298 8a42 d1a6 85ea  P..L..B."..B....
-00001290: 587e e0ce 15c2 50bb 5dee 1585 a24d 0bd5  X~....P.]....M..
-000012a0: b11c 932b 8421 82a9 2814 6d5a a88e e598  ...+.!..(.mZ....
-000012b0: 5c21 0c11 4ced 2990 4d0b 453c 956b 6fd2  \!..L.).M.E<.ko.
-000012c0: f6e2 4110 8408 a6a6 904d 0bc5 ce3a b417  ..A......M...:..
-000012d0: 0a41 8860 6a0a d9b4 50ec 6c43 8b50 489e  .A.`j...P.lC.PH.
-000012e0: ca2d 9a42 362d 143b dbd0 2214 8250 bbab  .-.B6-.;.."..P..
-000012f0: 2f9a 4236 2d14 3bcb d022 1492 a772 8ba6  /.B6-.;.."...r..
-00001300: 904d 0bc5 ce2e b408 85e4 a9dc a23d 4db5  .M...........=M.
-00001310: 69a1 54c6 b22f a445 3c50 8550 abd0 a228  i.T../.E<P.P...(
-00001320: 946c 5aa8 8e65 98f9 371a f883 5f78 38d4  .lZ..e..7..._x8.
-00001330: 72ba 5191 28d9 f450 1d9b 41db c676 23b7  r.Q.(..P..A..v#.
-00001340: e823 9579 ef4f db46 eed1 eefe bb1d ff01  .#.y.O.F........
-00001350: 0000 ffff 0000 00ff ff3c 8d41 0ac2 3010  .........<.A..0.
-00001360: 45af 12e6 00d6 2222 48d3 8dab 2e04 af10  E.....""H.......
-00001370: cd34 19d4 9930 192c dede 54d0 dd7f f0f8  .4...0.,..T.....
-00001380: 6f28 5918 8d6e 1775 b3b0 4dd1 c30e 9cbd  o(Y..n.u..M.....
-00001390: 0b7a 6039 09bf 502b 0943 370e 2524 3c07  .z`9..P+.C7.%$<.
-000013a0: 4dc4 d53d 7036 0fdb cd61 0f4e 29e5 3f98  M..=p6...a.N).?.
-000013b0: 140f 3db8 ab98 c9f3 3b33 8688 bada 4d9e  ..=.....;3....M.
-000013c0: 45ec 07ed 336a 5888 93d3 23b5 b44e b15f  E...3jX...#..N._
-000013d0: 4bdd 227a af19 d1c6 0f00 0000 ffff 0300  K."z............
-000013e0: 504b 0304 1400 0600 0800 0000 2100 cce4  PK..........!...
-000013f0: d4c2 a303 0000 460a 0000 1800 0000 786c  ......F.......xl
-00001400: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00001410: 7432 2e78 6d6c 9c93 4d6f a330 1086 ef2b  t2.xml..Mo.0...+
-00001420: ed7f b07c 0f06 92a6 290a a956 adaa cd65  ...|....)..V...e
-00001430: 55ed 57cf 8e19 8215 1bb3 b6f3 b5ab fdef  U.W.............
-00001440: 1d43 a091 7249 8b82 6d18 e679 67ec 37f3  .C..rI..m..yg.7.
-00001450: fb83 5664 07d6 4953 e734 8962 4aa0 16a6  ..Vd..IS.4.bJ...
-00001460: 90f5 3aa7 bf7e 3e8d 6694 38cf eb82 2b53  ..:..~>.f.8...+S
-00001470: 434e 8fe0 e8fd e2f3 a7f9 ded8 8dab 003c  CN.............<
-00001480: 4142 ed72 5a79 df64 8c39 5181 e62e 320d  AB.rZy.d.9Q...2.
-00001490: d418 298d d5dc e3a3 5d33 d758 e045 9ba4  ..).....]3.X.E..
-000014a0: 154b e378 ca34 9735 ed08 99bd 8661 ca52  .K.x.4.5.....a.R
-000014b0: 0a78 3462 aba1 f61d c482 e21e eb77 956c  .x4b.........w.l
-000014c0: 5c4f d3e2 1a9c e676 b36d 46c2 e806 112b  \O.....v.mF....+
-000014d0: a9a4 3fb6 504a b4c8 96eb da58 be52 d8f7  ..?.PJ.....X.R..
-000014e0: 2199 7041 0e16 7f29 dee3 5ea6 7d7f a1a4  !.pA...)..^.}...
-000014f0: a5b0 c699 d247 4866 5dcd 97ed dfb1 3bc6  .....GHf].....;.
-00001500: c540 baec ff2a 4c32 6116 7632 1ce0 1b2a  .@...*L2a.v2...*
-00001510: fd58 49c9 cdc0 4adf 60e3 0fc2 a603 2c6c  .XI...J.`.....,l
-00001520: 97cd b6b2 c8e9 bff8 748d 704e c210 8fe2  ........t.pN....
-00001530: 240c 67d7 7fba 9817 124f 3874 452c 9439  $.g......O8tE,.9
-00001540: fd92 64cf 2965 8b79 eb9f df12 f6ee 6c4d  ..d.)e.y......lM
-00001550: fe1a a37f 08ae e05b 309c 422b c768 e560  .......[0.B+.h.`
-00001560: d295 319b f0f9 12c5 63e4 3a50 2082 5d08  ..1.....c.:P .].
-00001570: c769 070f a0f0 f3e5 0dfa fc4f ab84 4b94  .i.........O..K.
-00001580: 6183 cef9 bad7 7c6a 6dfd 6c49 0125 df2a  a.....|jm.lI.%.*
-00001590: ff60 d48b 2c7c 1574 a3d9 2dc2 4e81 ef66  .`..,|.t..-.N..f
-000015a0: ff15 e4ba f218 9945 21d0 3a26 2b8e 8fe0  .......E!.:&+...
-000015b0: 045a 188b 8a92 5651 1885 781c 8996 e1bf  .Z....VQ..x.....
-000015c0: 8816 e487 76de 9fd0 6934 4d43 9dfe 182c  ....v...i4MC...,
-000015d0: 8927 24b6 ce1b dd2b 87b2 8774 8c76 e953  .'$....+...t.v.S
-000015e0: dc86 2e3f 9dbc 233f b91d 00e3 d964 60f4  ...?..#?.....d`.
-000015f0: ed0d 3584 ad6a 2b7f 0500 00ff ff00 0000  ..5..j+.........
-00001600: ffff b4d4 dd6e 8240 1005 e057 213c 4061  .....n.@...W!<@a
-00001610: 1705 3148 528b 15ff 7d05 b225 b517 d5c6  ..1HR...}..%....
-00001620: a5b6 7dfb 0e95 887b 726e eb8d 66f9 9c99  ..}....{rn..f...
-00001630: ec9c 90d9 435d 3745 d554 7976 3e7d 79e7  ....C]7E.Tyv>}y.
-00001640: 89af 7ccf 7e54 472b bfc6 2af6 bd43 33f1  ..|.~TG+..*..C3.
-00001650: 75f8 a0c2 fb8f 20f3 699b d37b 59bf bdb6  u..... .i..{Y...
-00001660: 420e bed5 a032 e397 9fa2 b6a6 3eca 99fc  B....2......>...
-00001670: 69e8 e799 69ab 3eb6 65a5 907c c913 2bc7  i...i.>.e..|..+.
-00001680: 975c 8583 2cb8 e459 603a 3465 68e4 9a27  .\..,..Y`:4eh..'
-00001690: 5a68 e8a2 82a2 d845 33da 2d75 d133 4530  Zh.....E3.-u.3E0
-000016a0: d39c a134 742b 95b4 52e2 a205 1d1c d092  ...4t+..R.......
-000016b0: 2298 6945 50a4 dd6e 6b5a 086e 6043 500c  ".iEP..nkZ.n`CP.
-000016c0: cdb6 c424 6076 ac99 824b da53 a46e 6307  ...$`v...K.S.nc.
-000016d0: 12d2 5b52 f5ff 24b5 2d2b 8196 e8f7 4955  ..[R..$.-+....IU
-000016e0: 7073 d30e 250e 8a20 aa14 41e6 0b8a 20cf  ps..%.. ..A... .
-000016f0: 3382 224c 6a67 46ce 4890 f939 ed06 f92a  3."LjgF.H..9...*
-00001700: 3b94 3a95 609d 0b5a 0966 5a32 a461 e7ab  ;.:.`..Z.fZ2.a..
-00001710: 2bd2 e17d 3bdd effc effd b126 2801 b321  +..};......&(..!
-00001720: 2686 89b6 7422 d8ee 8e22 d8ee 9ea0 a4bf  &...t"..."......
-00001730: c96b 5283 fefd fa0b 0000 ffff 0000 00ff  .kR.............
-00001740: ff34 cc4d 0ac2 3010 c5f1 ab84 3980 1544  .4.M..0.....9..D
-00001750: dc34 ddb8 7221 7885 6827 1fa8 f3c2 64a8  .4..r!x.h'....d.
-00001760: 787b 5b21 bbf7 7b8b ff58 3384 ad3c 6eea  x{[!..{..X3..<n.
-00001770: 22c4 2eb3 a703 39fb 56f6 2438 4316 d656  ".....9.V.$8C..V
-00001780: 2034 4c63 0d89 af41 5391 e65e 1ccd d37e   4Lc...AS..^...~
-00001790: 7722 a725 e5be 0df5 ff1e c9dd 6186 7757  w".%........a.wW
-000017a0: e630 b36e 5af3 11b0 8eb5 3b7c a0cf 9699  .0.nZ.....;|....
-000017b0: 6dfa 0100 00ff ff03 0050 4b03 0414 0006  m........PK.....
-000017c0: 0008 0000 0021 004d 3d34 677d 0300 00a9  .....!.M=4g}....
-000017d0: 0900 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
-000017e0: 6565 7473 2f73 6865 6574 332e 786d 6c9c  eets/sheet3.xml.
-000017f0: 934d 8f9b 3010 86ef 95fa 1f2c df83 8124  .M..0......,...$
-00001800: 348b 4256 5556 abee 6555 f5f3 ec98 2158  4.BVUV..eU....!X
-00001810: b131 b59d af56 fdef 1d43 4852 e512 2d02  .1...V...CHR..-.
-00001820: db30 f6f3 ce98 d7f3 c783 5664 07d6 49d3  .0........Vd..I.
-00001830: 1434 8962 4aa0 11a6 94cd baa0 dfbf 3d8f  .4.bJ.........=.
-00001840: 6694 38cf 9b92 2bd3 4041 8fe0 e8e3 e2fd  f.8...+.@A......
-00001850: bbf9 ded8 8dab 013c 4142 e30a 5a7b dfe6  .......<AB..Z{..
-00001860: 8c39 5183 e62e 322d 3418 a98c d5dc e3ab  .9Q...2-4.......
-00001870: 5d33 d75a e065 b748 2b96 c671 c634 970d  ]3.Z.e.H+..q.4..
-00001880: ed09 b9bd 8761 aa4a 0a78 3262 aba1 f13d  .....a.J.x2b...=
-00001890: c482 e21e f377 b56c dd40 d3e2 1e9c e676  .....w.l.@.....v
-000018a0: b36d 47c2 e816 112b a9a4 3f76 504a b4c8  .mG....+..?vPJ..
-000018b0: 5fd6 8db1 7ca5 b0ee 4332 e182 1c2c de29  _...|...C2...,.)
-000018c0: 3ee3 41a6 fb7e a3a4 a5b0 c699 ca47 4866  >.A..~.......GHf
-000018d0: 7dce b7e5 3fb0 07c6 c599 745b ff5d 9864  }...?.....t[.].d
-000018e0: c22c ec64 f881 1754 fab6 9492 e999 955e  .,.d...T.......^
-000018f0: 60e3 37c2 b233 2c6c 97cd b7b2 2ce8 9ff8  `.7..3,l....,...
-00001900: 748d b04f 4213 8f62 f442 371a 627f e962  t..OB..b.B7.b..b
-00001910: 5e4a fcc3 a12a 62a1 2ae8 c724 7f4d 295b  ^J...*b.*..$.M)[
-00001920: cc3b fffc 90b0 7757 63f2 db18 fd55 7005  .;....wWc....Up.
-00001930: afc1 700a ad1c a395 8349 57c6 6cc2 f417  ..p......IW.l...
-00001940: 148f 91eb 4081 0876 211c bb1d 2c41 e1f4  ....@..v!...,A..
-00001950: 6582 05bb 5f9d 5418 a310 3b2b 5d8f 07d5  e..._.T...;+]...
-00001960: e7ce d89f 2d29 a1e2 5be5 9746 fd94 a5af  ....-)..[..F....
-00001970: 8372 34fb 30a5 43e0 8bd9 7f02 b9ae 3d46  .r4.0.C.......=F
-00001980: f030 7586 c9cb e313 3881 0ec6 9ca2 641a  .0u.....8.....d.
-00001990: e484 51c8 c696 6819 8e22 3a90 1fba 7eff  ..Q...h..":...~.
-000019a0: 3fd7 f963 7064 8a09 8bad f346 0fba 274a  ?..cpd.....F..'J
-000019b0: bf1e a3fd fa09 6ec3 0990 4559 8a89 dd07  ......n...EY....
-000019c0: c0ac 4e84 6c3c bb82 9caa bb40 c256 75c9  ..N.l<.....@.Vu.
-000019d0: ff03 0000 ffff 0000 00ff ffb4 d4dd 6e82  ..............n.
-000019e0: 4010 05e0 5721 fb00 5d16 b055 b392 5451  @...W!..]..U..TQ
-000019f0: f18f 7720 eb46 7b51 6d5c 6adb b777 8844  ..w .F{Qm\j..w.D
-00001a00: 9cc9 b92d 3790 c9c7 243b 67c0 86a3 f74d  ...-7...$;g....M
-00001a10: 5137 756e 2fe7 9fe8 3251 4645 e1ab 3e05  Q7un/...2QFE..>.
-00001a20: 7a1a 9b4c 45c7 66a2 92f8 c5c4 cf17 21f7  z..LE.f.......!.
-00001a30: 1d9a f367 e93f 0ead a0c2 afc9 6a37 deff  ...g.?......j7..
-00001a40: 153e 387f a21a bd34 50b9 756d d7f7 b62d  .>8....4P.um...-
-00001a50: 3532 4a77 95e9 a312 910d 04af b949 32ab  52Jw.........I2.
-00001a60: afb9 d5ae 4333 8806 1c15 10bd 7234 87e8  ....C3......r4..
-00001a70: 8da3 0544 438e 9610 8d38 2a11 4a63 8e56  ...DC....8*.Jc.V
-00001a80: 1019 8ed6 1025 1c6d 204a 39da 4224 26be  .....%.m J9.B$&.
-00001a90: 8348 4cbc 82a8 9fb8 a65d 7a2c 54f2 3f0b  .HL......]z,T.?.
-00001aa0: d5b6 a585 a25b bf3e 468c 65da a1f4 19a5  .....[.>F.e.....
-00001ab0: 22f4 1944 22f4 0222 11fa 1ca1 4c84 be80  "..D".."....L...
-00001ac0: 4884 be84 489c ae84 4884 be82 4884 be86  H...H...H...H...
-00001ad0: 4884 be81 487c 665b 88c4 c477 1089 8957  H...H|f[...w...W
-00001ae0: 10f5 13bf ef98 ee7f 6037 0000 00ff ff00  ........`7......
-00001af0: 0000 ffff 34cc 4d0a c230 10c5 f1ab 8439  ....4.M..0.....9
-00001b00: 8015 44dc 34dd b872 2178 8568 271f a8f3  ..D.4..r!x.h'...
-00001b10: c264 a878 7b5b 21bb f77b 8bff 5833 84ad  .d.x{[!..{..X3..
-00001b20: 3c6e ea22 c42e b3a7 0339 fb56 f624 3843  <n.".....9.V.$8C
-00001b30: 16d6 5620 344c 630d 89af 4153 91e6 5e1c  ..V 4Lc...AS..^.
-00001b40: cdd3 7e77 22a7 25e5 be0d f5ff 1ec9 dd61  ..~w".%........a
-00001b50: 8677 57e6 30b3 6e5a f311 b08e b53b 7ca0  .wW.0.nZ.....;|.
-00001b60: cf96 996d fa01 0000 ffff 0300 504b 0304  ...m........PK..
-00001b70: 1400 0600 0800 0000 2100 c33a 3cca 6e03  ........!..:<.n.
-00001b80: 0000 9309 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00001b90: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
-00001ba0: 6d6c 9c93 4d8f db20 1086 ef95 f63f 20ee  ml..M.. .....? .
-00001bb0: 31b6 93b8 592b ce6a b5d1 aa7b a9aa 6adb  1...Y+.j...{..j.
-00001bc0: 9e09 1ec7 2860 5cc0 f950 d5ff dec1 8993  ....(`\..P......
-00001bd0: 54b9 448b 6cc0 1ef1 cc3b f032 7fda 6b45  T.D.l....;.2..kE
-00001be0: b660 9d34 4d41 9328 a604 1a61 4ad9 ac0b  .`.4MA.(...aJ...
-00001bf0: fae3 fd75 34a3 c479 de94 5c99 060a 7a00  ...u4..y..\...z.
-00001c00: 479f 160f 9fe6 3b63 37ae 06f0 0409 8d2b  G.....;c7......+
-00001c10: 68ed 7d9b 33e6 440d 9abb c8b4 d060 a432  h.}.3.D......`.2
-00001c20: 5673 8f9f 76cd 5c6b 8197 fd22 ad58 1ac7  Vs..v.\k...".X..
-00001c30: 19d3 5c36 f448 c8ed 3d0c 5355 52c0 d288  ..\6.H..=.SUR...
-00001c40: 4e43 e38f 100b 8a7b d4ef 6ad9 ba81 a6c5  NC.....{..j.....
-00001c50: 3d38 cded a66b 47c2 e816 112b a9a4 3ff4  =8...kG....+..?.
-00001c60: 504a b4c8 dfd6 8db1 7ca5 b0ee 7d32 e182  PJ......|...}2..
-00001c70: ec2d 3e29 bee3 214d ffff 2693 96c2 1a67  .->)..!M..&....g
-00001c80: 2a1f 2199 1d35 df96 ffc8 1e19 1767 d26d  *.!..5.......g.m
-00001c90: fd77 6192 09b3 b095 e100 2fa8 f463 9292  .wa......./..c..
-00001ca0: e999 955e 60e3 0fc2 b233 2c6c 97cd 3b59  ...^`....3,l..;Y
-00001cb0: 16f4 4f7c 6a23 1c93 d0c5 a378 1cba abf6  ..O|j#.....x....
-00001cc0: 972e e6a5 c413 0e55 110b 5541 9f93 fc6b  .......U..UA...k
-00001cd0: 4ad9 62de fbe7 a784 9dbb 9a93 60c7 9531  J.b.........`..1
-00001ce0: 9b10 78c3 3431 121c 2810 c118 84e3 b085  ..x.41..(.......
-00001cf0: 1750 aaa0 cb74 8296 fedd 43c3 1c91 eccc  .P...t....C.....
-00001d00: bc9e 0ffc d7de c2df 2c29 a1e2 9df2 2f46  ........,)..../F
-00001d10: fd92 a5af f1ba c4d1 ecf3 940e 81ef 66f7  ..............f.
-00001d20: 05e4 baf6 18c1 6bd3 5b23 2f0f 4b70 02bd  ......k.[#/.Kp..
-00001d30: 8a9a a264 1ad2 09a3 908d 3dd1 325c 3af4  ...d......=.2\:.
-00001d40: 1adf f7e3 ee7f aef3 87e0 bd14 cf42 74ce  .............Bt.
-00001d50: 1b3d e43d 518e eb31 7a5c 8f75 0d80 2cca  .=.=Q..1z\.u..,.
-00001d60: 5214 761f 0055 9d08 d978 7605 3955 7781  R.v..U...xv.9Uw.
-00001d70: 84ad eac5 ff03 0000 ffff 0000 00ff ffb4  ................
-00001d80: d4dd 6e82 4010 05e0 5721 fb00 5d16 b055  ..n.@...W!..]..U
-00001d90: b392 5451 f18f 7720 eb46 7b51 6d5c 6adb  ..TQ..w .F{Qm\j.
-00001da0: b777 8844 9cc9 b92d 3790 c9c7 243b 67c0  .w.D...-7...$;g.
-00001db0: 86a3 f74d 5137 756e 2fe7 9fe8 3251 4645  ...MQ7un/...2QFE
-00001dc0: e1ab 3e05 7a1a 9b4c 45c7 66a2 92f8 c5c4  ..>.z..LE.f.....
-00001dd0: cf17 21f7 1d9a f367 e93f 0ead a0c2 afc9  ..!....g.?......
-00001de0: 6a37 deff 153e 387f a21a bd34 50b9 756d  j7...>8....4P.um
-00001df0: d7f7 b62d 3532 4a77 95e9 a312 910d 04af  ...-52Jw........
-00001e00: b949 32ab afb9 d5ae 4333 8806 1c15 10bd  .I2.....C3......
-00001e10: 7234 87e8 8da3 0544 438e 9610 8d38 2a11  r4.....DC....8*.
-00001e20: 4a63 8e56 1019 8ed6 1025 1c6d 204a 39da  Jc.V.....%.m J9.
-00001e30: 4224 26be 8348 4cbc 82a8 9fb8 a65d 7a2c  B$&..HL......]z,
-00001e40: 54f2 3f0b d5b6 a585 a25b bf3e 468c 65da  T.?......[.>F.e.
-00001e50: a1f4 19a5 22f4 1944 22f4 0222 11fa 1ca1  ...."..D".."....
-00001e60: 4c84 be80 4884 be84 489c ae84 4884 be82  L...H...H...H...
-00001e70: 4884 be86 4884 be81 487c 665b 88c4 c477  H...H...H|f[...w
-00001e80: 1089 8957 10f5 13bf ef98 ee7f 6037 0000  ...W........`7..
-00001e90: 00ff ff00 0000 ffff 34cc 4d0a c230 10c5  ........4.M..0..
-00001ea0: f1ab 8439 8015 44dc 34dd b872 2178 8568  ...9..D.4..r!x.h
-00001eb0: 271f a8f3 c264 a878 7b5b 21bb f77b 8bff  '....d.x{[!..{..
-00001ec0: 5833 84ad 3c6e ea22 c42e b3a7 0339 fb56  X3..<n.".....9.V
-00001ed0: f624 3843 16d6 5620 344c 630d 89af 4153  .$8C..V 4Lc...AS
-00001ee0: 91e6 5e1c cdd3 7e77 22a7 25e5 be0d f5ff  ..^...~w".%.....
-00001ef0: 1ec9 dd61 8677 57e6 30b3 6e5a f311 b08e  ...a.wW.0.nZ....
-00001f00: b53b 7ca0 cf96 996d fa01 0000 ffff 0300  .;|....m........
-00001f10: 504b 0304 1400 0600 0800 0000 2100 f7b3  PK..........!...
-00001f20: 830c 2403 0000 d507 0000 1800 0000 786c  ..$...........xl
-00001f30: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00001f40: 7435 2e78 6d6c 9c93 cb8e db20 1486 f795  t5.xml..... ....
-00001f50: e61d 10fb 18e3 5c34 b1e2 8c46 198d 9a5d  ......\4...F...]
-00001f60: 55b5 d335 c1c7 310a 1817 c84d 55df bd07  U..5..1....MU...
-00001f70: 3b37 299b 7410 060c 3adf b9f0 337b 3918  ;7).t...:...3{9.
-00001f80: 4d76 e0bc b24d 4179 9252 028d b4a5 6ad6  Mv...MAy.R....j.
-00001f90: 05fd f9e3 7df0 4c89 0fa2 2985 b60d 14f4  ....}.L...).....
-00001fa0: 089e becc 9fbe ccf6 d66d 7c0d 1008 121a  .........m|.....
-00001fb0: 5fd0 3a84 3667 cccb 1a8c f089 6da1 c193  _.:.6g......m...
-00001fc0: ca3a 2302 feba 35f3 ad03 5176 4646 b32c  .:#...5...QvFF.,
-00001fd0: 4d27 cc08 d5d0 9e90 bb47 18b6 aa94 8437  M'.......G.....7
-00001fe0: 2bb7 069a d043 1c68 1130 7e5f abd6 9f69  +....C.h.0~_...i
-00001ff0: 463e 8233 c26d b6ed 405a d322 62a5 b40a  F>.3.m..@Z."b...
-00002000: c70e 4a89 91f9 72dd 5827 561a f33e f091  ..J...r.X'V..>..
-00002010: 90e4 e0b0 67f8 0dcf 6eba fd3b 4f46 4967  ....g...n..;OFIg
-00002020: bdad 4282 64d6 c77c 9ffe 944d 9990 17d2  ..B.d..|...M....
-00002030: 7dfe 0f61 f888 39d8 a978 8157 54f6 b990  }..a..9..x.WT...
-00002040: f8f8 c2ca aeb0 e127 6193 0b2c 96cb e55b  .......'a..,...[
-00002050: 5516 f44f 7a6a 039c 791c d241 3a8a c34d  U..Ozj..y..A:..M
-00002060: fb4b e7b3 52e1 0dc7 ac88 83aa a0af 3c5f  .K..R.........<_
-00002070: 6694 cd67 9d7e 3e14 ecfd cd9a 4439 aeac  f..g.~>.....D9..
-00002080: ddc4 8325 ba49 91e0 4183 8cc2 2002 a71d  ...%.I..A... ...
-00002090: 2c40 eb82 2ea2 a27f 774c 5c22 905d 88b7  ,@......wL\".]..
-000020a0: eb33 fdbd 13f0 3747 4aa8 c456 8785 d5bf  .3....7GJ..V....
-000020b0: 5419 ea82 4e93 6c4c cfdb dfed fe2b a875  T...N.lL.....+.u
-000020c0: 1df0 11a1 834e 1679 797c 032f 51a7 184f  .....N.yy|./Q..O
-000020d0: c2c7 d199 b41a c938 12a3 e283 439d 8943  .......8....C..C
-000020e0: 41b1 dafb 9eca 47c9 2472 7d38 46dd 6578  A.....G.$r}8F.ex
-000020f0: 22b7 3e58 73f2 ca4f 94de 1e0b dbd9 4faf  ".>Xs..O......O.
-00002100: f6e9 ffd8 737c ef1d 804f 86cf a30b a44f  ....s|...O.....O
-00002110: ed1a 42ac 5217 f93f 0000 00ff ff00 0000  ..B.R..?........
-00002120: ffff 94d3 dd0e 8220 14c0 f157 713c 408a  ....... ...Wq<@.
-00002130: 8aa5 43b6 f2fb 3198 b975 654d 9cd5 db87  ..C...1..ueM....
-00002140: 8b69 e7ec dc74 0583 df05 f01f d2dc 8661  .i...t.........a
-00002150: 2ef5 ac95 9cee 4f6f ca19 679e 79e8 d1d8  ......Oo..g.y...
-00002160: 5996 32ef c563 dd67 d777 3998 7e18 e79c  Y.2..c.g.w9.~...
-00002170: 0507 2e98 92fd 6acf 2bce 5968 07bb 63ec  ......j.+.Yh..c.
-00002180: f2a2 b808 a4bf 28e9 f70e 5d48 c421 2a48  ......(...]H.!*H
-00002190: 1442 5492 2882 a822 510c 51ed 5002 0e2e  .BT.(.."Q.Q.P...
-000021a0: 206a 4894 40d4 92e8 0851 479e e9b4 21df   jH.@....QG...!.
-000021b0: befd 1620 fc27 c08a 6d80 18dc 2345 011c  ... .'..m...#E..
-000021c0: 12bf 2841 950a 8722 8050 a592 44a8 5245  ..(A...".P..D.RE
-000021d0: 2254 a926 11aa d490 0855 6a49 842a 7524  "T.&.....UjI.*u$
-000021e0: da2b 7d03 f8fb 6ff8 0000 00ff ff00 0000  .+}...o.........
-000021f0: ffff 3c8c 4b0a c240 1005 af32 f401 8c22  ..<.K..@...2..."
-00002200: 924d 261b 572e 845c 614c 7a3e a8fd 869e  .M&.W..\aLz>....
-00002210: 46f1 f646 4177 5550 d450 3384 adcc 93ba  F..FAwUP.P3.....
-00002220: 08b1 d3e2 694f ce5e 953d 098e 9007 6b2b  ....iO.^.=....k+
-00002230: 10ea c6a1 86c4 e7a0 a948 7337 8ee6 69bb  .........Hs7..i.
-00002240: e90f e4b4 a4fc 1743 f5b4 2377 8119 ee5f  .......C..#w..._
-00002250: cc1c 16d6 4fbd c611 b09f accf ee09 bdb6  ....O...........
-00002260: cc6c e31b 0000 ffff 0300 504b 0304 1400  .l........PK....
-00002270: 0600 0800 0000 2100 0031 94de e503 0000  ......!..1......
-00002280: 3b0b 0000 1800 0000 786c 2f77 6f72 6b73  ;.......xl/works
-00002290: 6865 6574 732f 7368 6565 7436 2e78 6d6c  heets/sheet6.xml
-000022a0: 9c94 db8e da30 1086 ef2b f51d 22df 9313  .....0...+.."...
-000022b0: 2104 04ac 2814 756f aa55 8fd7 c631 6061  !...(.uo.U...1`a
-000022c0: c7d4 360b 74d5 77ef d8c1 0189 aa0a 4880  ..6.t.w.......H.
-000022d0: 079c f9fe 99f1 6f46 4f47 c183 57aa 3493  ......oFOG..W.4.
-000022e0: d518 2561 8c02 5a11 59b2 6a3d 46df bf2d  ..%a..Z.Y.j=F..-
-000022f0: 3a05 0ab4 c155 89b9 ace8 189d a846 4f93  :....U.......FO.
-00002300: f7ef 4607 a9b6 7a43 a909 8050 e931 da18  ..F...zC...P.1..
-00002310: b31b 4691 261b 2ab0 0ee5 8e56 b0b3 924a  ..F.&.*....V...J
-00002320: 6003 5fd5 3ad2 3b45 71e9 9204 8fd2 38ce  `._.:.;Eq.....8.
-00002330: 2381 5985 6ac2 50b5 61c8 d58a 113a 9764  #.Y.j.P.a....:.d
-00002340: 2f68 656a 88a2 1c1b a85f 6fd8 4e7b 9a20  /hej....._o.N{. 
-00002350: 6d70 02ab ed7e d721 52ec 00b1 649c 9993  mp...~.!R...d...
-00002360: 83a2 4090 e1f3 ba92 0a2f 39f4 7d4c 324c  ..@....../9.}L2L
-00002370: 82a3 8257 0aef ae97 71bf df28 0946 94d4  ...W....q..(.F..
-00002380: 7265 4220 4775 cdb7 ed0f a241 8449 43ba  reB Gu.....A.IC.
-00002390: edbf 1526 c922 455f 993d c00b 2a7d aca4  ...&."E_.=..*}..
-000023a0: a4d7 b0d2 0bac fb20 2c6f 6076 5c6a b867  ....... ,o`v\j.g
-000023b0: e518 bd2d 8a6c 96e4 d9b4 d39f 1759 279b  ...-.l.......Y'.
-000023c0: 76d3 4e51 6471 a7ff 713e 4db3 593c 4d3f  v.NQdq..q>M.Y<M?
-000023d0: e47f d064 5432 3861 db55 a0e8 6a8c a6c9  ...dT28a.U..j...
-000023e0: f025 45d1 64e4 fcf3 83d1 83be 8a83 df52  .%E.d..........R
-000023f0: 8aaf 0473 fad9 1a8e 8395 63b0 b235 e952  ...s......c..5.R
-00002400: caad 7dfc 19c4 63e0 6aca 29b1 7609 302c  ..}...c.j.).v.0,
-00002410: af74 4639 3cbe c8c1 e7bf 9c12 8420 1335  .tF9<........ .5
-00002420: 3ad7 b1d7 5c38 5bbf a8a0 a42b bce7 6626  :...\8[....+..f&
-00002430: f94f 569a 8dd5 0d8b 7e0f f98d 2ff2 f089  .OV.....~.../...
-00002440: b2f5 c6c0 4e11 da0d e798 6179 9a53 4dc0  ....N.....ay.SM.
-00002450: c250 5498 f4ac 2291 1cf0 f019 0866 ef22  .PT..."......f."
-00002460: 5810 1fdd 7aa8 d169 1ce6 2910 b439 594b  X...z..i..)..9YK
-00002470: c209 91bd 3652 78e5 33a4 4e87 5d97 0ecf  ....6Rx.3.N.]...
-00002480: fbf4 ec8e 7418 874b 87f5 dfe9 49ff bff2  ....t..K....I...
-00002490: b0eb f261 7d44 1efe 755c 3aac 0fc9 0ffc  ...a}D..u\:.....
-000024a0: f0ac 09ce d3bb a7fd a499 3e04 6740 9285  ..........>.g@..
-000024b0: 5d7b 80ad c69f f8f9 dbc0 03f2 da1a ed00  ]{..............
-000024c0: 7067 eaf3 87e0 0268 ad9f f974 08fc 04a0  pg.....h...t....
-000024d0: 9776 daa0 526b 5fb9 27bd a77b 6f9f 24ef  .v..Rk_.'..{o.$.
-000024e0: 1697 02fc dd68 8ab0 f7cc d9fe 2f00 0000  .....h....../...
-000024f0: ffff 0000 00ff ffb4 94d1 8e82 3010 457f  ............0.E.
-00002500: 85f4 032c 4505 3595 4445 4557 5d7f 81d4  ...,E.5.DEEW]...
-00002510: 467d 5037 9655 f7ef 7758 119c 615e 9717  F}P7.U..wX..a^..
-00002520: c8e5 f4a6 e919 d0ee 606d 9e64 7916 ebeb  ........`m.dy...
-00002530: e5ee 5d87 4209 cf7d 6567 074f 0315 0aef  ..].B..}eg.O....
-00002540: 900f 45e0 b794 ff7e 0164 be5d 7e39 a5f6  ..E....~.d.]~9..
-00002550: b82f 0808 1eaa 9399 c1ee 27b1 ced8 3364  ./........'...3d
-00002560: b0a8 2b62 6d8a d651 510b 4570 8337 0ee2  ..+bm..QQ.Ep.7..
-00002570: 5bac c29e 96b7 584b 5342 6316 ea63 68c2  [.....XKSBc..ch.
-00002580: 4191 8fa1 8485 1486 a62c 1460 6856 4270  A........,.`hVBp
-00002590: 12f5 c6a3 3686 e66c 5307 4329 d7d4 277b  ....6..lS.C)..'{
-000025a0: 5ab0 4d5d dcb4 64a1 b082 24a8 ac7c 06ff  Z.M]..d...$..|..
-000025b0: e3b3 a805 edf8 5822 e2b3 8422 7476 44fa  ......X"..."tvD.
-000025c0: 8485 88f4 8483 7a44 fa94 85ea 63f9 1bc4  ......zD....c...
-000025d0: 190b 1155 7316 22aa 5216 22aa 162c 4466  ...Us.".R."..,Df
-000025e0: 6cc9 4264 c63e 9e50 e00b 597e 2eab 46b2  l.Bd.>.P..Y~..F.
-000025f0: 6e24 9baa fab5 eab3 916c df93 e7ec c8fa  n$.......l......
-00002600: bff0 0b00 00ff ff00 0000 ffff 34cd c10a  ............4...
-00002610: c230 1004 d05f 09fb 0156 14e9 a5e9 c593  .0..._...V......
-00002620: 07a1 bf10 db6d 12d4 9db0 5914 ffde 2ae4  .....m....Y...*.
-00002630: 366f 0e33 4349 10b6 3c4f ea56 885d 164f  6o.3CI..<O.V.].O
-00002640: 0772 f629 ec49 7086 bc58 6b86 5037 0e25  .r.).Ip..Xk.P7.%
-00002650: 44be 068d 59aa 7bf0 6a9e f6bb 9e9c e698  D...Y.{.j.......
-00002660: 5a36 947f 7b22 7783 199e 4d89 c3c2 fad3  Z6..{"w...M.....
-00002670: 91b6 2758 c3b6 dbbd a1f7 9a98 6dfc 0200  ..'X........m...
-00002680: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00002690: 0021 00e9 a625 b866 0600 0053 1b00 0013  .!...%.f...S....
-000026a0: 0000 0078 6c2f 7468 656d 652f 7468 656d  ...xl/theme/them
-000026b0: 6531 2e78 6d6c ec59 cd6e 1b37 10be 17e8  e1.xml.Y.n.7....
-000026c0: 3b10 7b4f 2cd9 9262 1991 034b 96e2 3671  ;.{O,..b...K..6q
-000026d0: 62d8 4a8a 1ca9 5d6a 9711 77b9 2029 3bba  b.J...]j..w. );.
-000026e0: 15c9 b140 81a2 69d1 4b81 de7a 28da 0648  ...@..i.K..z(..H
-000026f0: 805e d2a7 719b a24d 81bc 4287 e44a 5a5a  .^..q..M..B..JZZ
-00002700: 546c 2706 fa17 1d6c 2df7 e3fc cf70 86ba  Tl'....l-....p..
-00002710: 7aed 41ca d021 1192 f2ac 1554 2f57 0244  z.A..!.....T/W.D
-00002720: b290 4734 8b5b c19d 7eef d27a 80a4 c259  ..G4.[..~..z...Y
-00002730: 8419 cf48 2b98 1019 5cdb 7cff bdab 7843  ...H+...\.|...xC
-00002740: 2524 2508 f667 7203 b782 44a9 7c63 6545  %$%..gr...D.|ceE
-00002750: 86b0 8ce5 659e 930c de0d b948 b182 4711  ....e......H..G.
-00002760: af44 021f 01dd 94ad ac56 2a8d 9514 d32c  .D.......V*....,
-00002770: 4019 4e81 eced e190 8604 f535 c960 734a  @.N........5.`sJ
-00002780: bccb e031 5352 2f84 4c1c 68d2 c4d9 61b0  ...1SR/.L.h...a.
-00002790: d1a8 aa11 7222 3b4c a043 cc5a 01f0 89f8  ....r";L.C.Z....
-000027a0: 519f 3c50 0162 582a 78d1 0a2a e613 ac6c  Q.<P.bX*x..*...l
-000027b0: 5e5d c11b c526 a696 ec2d edeb 994f b1af  ^]...&...-...O..
-000027c0: d810 8d56 0d4f 110f 664c abbd 5af3 caf6  ...V.O..fL..Z...
-000027d0: 8cbe 0130 b588 eb76 bb9d 6e75 46cf 0070  ...0...v..nuF..p
-000027e0: 1882 a656 9632 cd5a 6fbd da9e d22c 81ec  ...V.2.Zo....,..
-000027f0: d745 da9d 4abd 5273 f125 fa6b 0b32 37db  .E..J.Rs.%.k.27.
-00002800: ed76 bd59 c862 891a 90fd 5a5b c0af 571a  .v.Y.b....Z[..W.
-00002810: b5ad 5507 6f40 165f 5fc0 d7da 5b9d 4ec3  ..U.o@.__...[.N.
-00002820: c11b 90c5 3716 f0bd 2bcd 46cd c51b 50c2  ....7...+.F...P.
-00002830: 6836 5a40 6b87 f67a 05f5 1964 c8d9 8e17  h6Z@k..z...d....
-00002840: be0e f0f5 4a01 9fa3 201a 66d1 a559 0c79  ....J... .f..Y.y
-00002850: a696 c55a 8aef 73d1 0380 0632 ac68 86d4  ...Z..s....2.h..
-00002860: 2427 431c 4214 7770 3a10 146b 0678 83e0  $'C.B.wp:..k.x..
-00002870: d21b bb14 ca85 25cd 0bc9 50d0 5cb5 820f  ......%...P.\...
-00002880: 730c 1931 a7f7 eaf9 f7af 9e3f 45af 9e3f  s..1.......?E..?
-00002890: 397e f8ec f8e1 4fc7 8f1e 1d3f fcd1 d272  9~....O....?...r
-000028a0: 36ee e02c 2e6f 7cf9 ed67 7f7e fd31 fae3  6..,.o|..g.~.1..
-000028b0: e937 2f1f 7fe1 c7cb 32fe d71f 3ef9 e5e7  .7/.....2...>...
-000028c0: cffd 40c8 a0b9 442f be7c f2db b327 2fbe  ..@...D/.|...'/.
-000028d0: faf4 f7ef 1e7b e05b 020f caf0 3e4d 8944  .....{.[....>M.D
-000028e0: b7c8 11da e729 e866 0ce3 4a4e 06e2 7c3b  .....).f..JN..|;
-000028f0: fa09 a6ce 0e9c 006d 0fe9 ae4a 1ce0 ad09  .......m...J....
-00002900: 663e 5c9b b8c6 bb2b a078 f880 d7c7 f71d  f>\....+.x......
-00002910: 590f 1231 56d4 c3f9 4692 3ac0 5dce 599b  Y..1V...F.:.].Y.
-00002920: 0baf 016e 685e 250b f7c7 59ec 672e c665  ...nh^%...Y.g..e
-00002930: dc3e c687 3ede 1d9c 39ae ed8e 73a8 9ad3  .>..>...9...s...
-00002940: a074 6cdf 4988 23e6 1ec3 99c2 31c9 8842  .tl.I.#.....1..B
-00002950: fa1d 1f11 e2d1 ee1e a58e 5d77 6928 b8e4  ..........]wi(..
-00002960: 4385 ee51 d4c6 d46b 923e 1d38 8134 dfb4  C..Q...k.>.8.4..
-00002970: 4353 f0cb c4a7 33b8 dab1 cdee 5dd4 e6cc  CS....3.....]...
-00002980: a7f5 3639 7491 9010 9879 84ef 13e6 98f1  ..69t....y......
-00002990: 3a1e 2b9c fa48 f671 caca 06bf 8955 e213  :.+..H.q.....U..
-000029a0: f260 22c2 32ae 2b15 783a 268c a36e 44a4  .`".2.+.x:&..nD.
-000029b0: f4ed b92d 40df 92d3 6f60 a857 5eb7 efb2  ...-@...o`.W^...
-000029c0: 49ea 2285 a223 1fcd 9b98 f332 729b 8f3a  I."..#.....2r..:
-000029d0: 094e 73af cc34 4bca d80f e408 4214 a33d  .Ns..4K.....B..=
-000029e0: ae7c f05d ee66 887e 063f e06c a9bb ef52  .|.].f.~.?.l...R
-000029f0: e2b8 fbf4 4270 87c6 8e48 f300 d16f c6a2  ....Bp...H...o..
-00002a00: a8da 4efd 4d69 f6ba 62cc 2854 e377 c578  ..N.Mi..b.(T.w.x
-00002a10: 7a3a 6dc1 d1e4 4b89 9d13 2578 19ee 5f58  z:m...K...%x.._X
-00002a20: 78b7 f138 db23 10eb 8b07 cfbb bafb aeee  x..8.#..........
-00002a30: 06ff f9ba bb2c 97cf 5a6d e705 169a e479  .....,..Zm.....y
-00002a40: 5f6c bae4 7469 933c a48c 1da8 0923 37a5  _l..ti.<.....#7.
-00002a50: e993 251c 1651 0f16 4d03 6fa6 b8d9 d094  ..%..Q..M.o.....
-00002a60: 27f0 b528 ee0e 2e16 d8ec 4182 ab8f a84a  '..(......A....J
-00002a70: 0e12 9c43 8f5d 3523 5f2c 0bd2 b144 3997  ...C.]5#_,...D9.
-00002a80: 30db 9965 337c 9213 b4cd 3849 a1cd 3693  0..e3|....8I..6.
-00002a90: 615d cf0c b61e 48ac 7679 6497 d7ca b3e1  a]....H.vyd.....
-00002aa0: 8c8c 9914 6333 7f4e 19ad 6902 6765 b676  ....c3.N..i.ge.v
-00002ab0: e5ed 9855 ad54 4bcd e6aa 5635 a299 52e7  ...U.TK...V5..R.
-00002ac0: a836 5319 7cb8 a81a 2cce ac09 5d08 82de  .6S.|...,...]...
-00002ad0: 05ac dc80 115d cb0e b309 6624 d276 b773  .....]....f$.v.s
-00002ae0: f3d4 2d9a f585 ba48 2638 2285 8fb4 de8b  ..-....H&8".....
-00002af0: 3eaa 1a27 4d63 651a 461e 1fe9 39ef 141f  >..'Mce.F...9...
-00002b00: 95b8 3535 d9b7 e076 1627 95d9 d596 b09b  ..55...v.'......
-00002b10: 7aef 6dbc 341d 6ee7 5ed2 797b 221d 5956  z.m.4.n.^.y{".YV
-00002b20: 4e4e 96a1 a356 d0ac afd6 0314 e2bc 150c  NN...V..........
-00002b30: 61ac 85af 690e 5e97 baf1 c32c 86bb a150  a...i.^....,...P
-00002b40: 091b f6a7 26b3 09d7 b937 9bfe b0ac c24d  ....&....7.....M
-00002b50: 85b5 fb82 c24e 1dc8 8554 db58 2636 34cc  .....N...T.X&64.
-00002b60: ab22 0458 6686 7023 ff6a 1dcc 7a51 0ad8  .".Xf.p#.j..zQ..
-00002b70: 487f 0329 d6d6 2118 fe36 29c0 8eae 6bc9  H..)..!..6)...k.
-00002b80: 7048 4255 7676 69c5 dc51 1840 514a f958  pHBUvvi..Q.@QJ.X
-00002b90: 1171 9044 4768 c0c6 621f 83fb 75a8 823e  .q.DGh..b...u..>
-00002ba0: 1195 703b 612a 827e 80ab 346d 6df3 ca2d  ..p;a*.~..4mm..-
-00002bb0: ce45 d295 2fb0 0cce ae63 9627 b828 b73a  .E../....c.'.(.:
-00002bc0: 45a7 996c e126 8f67 3298 272b ad11 0f74  E..l.&.g2.'+...t
-00002bd0: f3ca 6e94 3bbf 2a26 e52f 4895 7218 ffcf  ..n.;.*&./H.r...
-00002be0: 54d1 e709 5c17 ac45 da03 21dc e40a 8c74  T...\..E..!....t
-00002bf0: beb6 022e 54c2 a10a e509 0d7b 022e b94c  ....T......{...L
-00002c00: ed80 6881 eb58 780d 4105 f7c9 e6bf 2087  ..h..Xx.A..... .
-00002c10: fabf cd39 4bc3 a435 4c7d 6a9f c648 5038  ...9K..5L}j..HP8
-00002c20: 8f54 2208 d983 b264 a2ef 1462 d5e2 ecb2  .T"....d...b....
-00002c30: 2459 41c8 4454 495c 995b b107 e490 b0be  $YA.DTI\.[......
-00002c40: ae81 0d7d b607 2881 5037 d5a4 2803 0677  ...}..(.P7..(..w
-00002c50: 32fe dce7 2283 06b1 6e72 fea9 9d8f 4de6  2..."...nr....M.
-00002c60: f3b6 07ba 3bb0 2d96 dd7f c65e a456 2afa  ....;.-....^.V*.
-00002c70: a5a3 a0e9 3dfb 4c4f 352b 07af 39d8 cf79  ....=.LO5+..9..y
-00002c80: d4da 8ab5 a0f1 6afd cc47 6d0e 973e 48ff  ......j..Gm..>H.
-00002c90: 81f3 8f8a 90d9 1f27 f481 dae7 fb50 5b11  .......'.....P[.
-00002ca0: fcd6 60db 2b04 517d c936 1e48 1748 5b1e  ..`.+.Q}.6.H.H[.
-00002cb0: 07d0 38d9 451b 4c9a 946d 588a eef6 c2db  ..8.E.L..mX.....
-00002cc0: 28b8 912e 3add 195f c8d2 37e9 74cf 69ec  (...:.._..7.t.i.
-00002cd0: 5973 e6b2 7372 f1f5 dde7 f98c 5d58 d8b1  Ys..sr......]X..
-00002ce0: 75b9 d3f5 981a 92f6 648a eaf6 683a c818  u.......d...h:..
-00002cf0: c798 5fb5 ca3f 3cf1 c17d 70f4 365c f18f  .._..?<..}p.6\..
-00002d00: 9992 f66a ff01 5cf1 c194 617f 2480 e4b7  ...j..\...a.$...
-00002d10: ce35 5b37 ff02 0000 ffff 0300 504b 0304  .5[7........PK..
-00002d20: 1400 0600 0800 0000 2100 209e 4fe6 fa05  ........!. .O...
-00002d30: 0000 ca21 0000 0d00 0000 786c 2f73 7479  ...!......xl/sty
-00002d40: 6c65 732e 786d 6cd4 5acd 6ee3 3610 be17  les.xml.Z.n.6...
-00002d50: e83b 083a 750f 8efe 65cb 6b7b bb4e 2260  .;.:u...e.k{.N"`
-00002d60: 816d 5134 2950 a05b 2c64 89b6 8948 a241  .mQ4)P.[,d...H.A
-00002d70: d159 7b17 7beb a5e8 b10f d153 7b5e 1428  .Y{.{......S{^.(
-00002d80: fa32 5d6c 1fa3 43d2 b2e8 f837 8e93 b806  .2]l..C....7....
-00002d90: 9288 1439 f3f1 9be1 703c 4ceb d924 4bb5  ...9....p<L..$K.
-00002da0: 6b44 0b4c f2b6 6e9d 98ba 86f2 9824 381f  kD.L..n......$8.
-00002db0: b4f5 ef2e c35a 43d7 0a16 e549 9492 1cb5  .....ZC....I....
-00002dc0: f529 2af4 679d cf3f 6b15 6c9a a28b 2142  .)*.g..?k.l...!B
-00002dd0: 4c03 1179 d1d6 878c 8d9a 8651 c443 9445  L..y.......Q.C.E
-00002de0: c509 19a1 1cde f409 cd22 064d 3a30 8a11  .........".M:0..
-00002df0: 4551 52f0 4959 6ad8 a6e9 1b59 8473 5d4a  EQR.IYj....Y.s]J
-00002e00: 6866 f12e 42b2 885e 8d47 b598 64a3 88e1  hf..B..^.G..d...
-00002e10: 1e4e 319b 0a59 ba96 c5cd 1783 9cd0 a897  .N1..Y..........
-00002e20: 02d4 89e5 46b1 36b1 7c6a 6b13 5a2a 11bd  ....F.6.|jk.Z*..
-00002e30: 4b7a 321c 5352 903e 3b01 b906 e9f7 718c  Kz2.SR.>;.....q.
-00002e40: 96e1 0646 6044 7125 0924 ef27 c9f2 0cd3  ...F`Dq%.$.'....
-00002e50: 5e58 fb84 ee29 c935 28ba c6dc 7c7a a795  ^X...).5(...|z..
-00002e60: 8fb3 3063 8516 9371 ceda ba37 efd2 e49b  ..0c...q...7....
-00002e70: 1709 d8b8 eeeb 9ab4 ca29 49b8 49e1 6364  .........)I.I.cd
-00002e80: 46f2 f44b dd28 452c 8caf 2f8e 374f 4cd3  F..K.(E,../.7OL.
-00002e90: 7cad ad19 0cfe a20a e783 d78e 0d6e 8c7d  |............n.}
-00002ea0: fde4 e90f dfa2 e4c7 575f 98af 9eac 96df  ........W_......
-00002eb0: 0007 5d90 2f85 1bb3 9577 5a7d 9257 0400  ..]./....wZ}.W..
-00002ec0: 7261 efe6 554e dee4 217f 0504 002b 7c54  ra..UN..!....+|T
-00002ed0: a755 bcd5 aea3 147a 2cae 2c26 29a1 1a03  .U.....z,.,&)...
-00002ee0: ef05 5244 4f1e 6548 8ef8 f8c7 2fff fcf5  ..RDO.eH..../...
-00002ef0: ab18 358c 6801 4e2f 273a 2eef 132e 3f1b  ..5.h.N/':....?.
-00002f00: 9961 7040 de69 481d 3734 d995 263a e8b5  .ap@.iH.74..&:..
-00002f10: f530 0432 e123 563b 57f7 9ce2 28e5 5dfd  .0.2.#V;W...(.].
-00002f20: 28c3 e954 2a13 5357 4a0d 1667 1f0a ec5a  (..T*.SWJ..g...Z
-00002f30: b12a 2ae7 00a4 0812 37d1 ffe9 f79f 3ffd  .**.....7.....?.
-00002f40: f9f7 4d42 d6aa 5e4d fd56 2d15 6ff7 bfc0  ..MB..^M.V-.o...
-00002f50: 1b06 df6f 8162 9d05 7809 4ed3 f9a6 af73  ...o.b..x.N....s
-00002f60: f786 8e4e 0be2 2343 340f a1a1 cd9e 2fa7  ...N..#C4...../.
-00002f70: 2370 ee1c 42b9 7451 316e cbe8 018d a696  #p..B.tQ1n......
-00002f80: eded 3ea1 2029 4e38 8ac1 a9ba a504 ffbd  ..>. )N8........
-00002f90: 591f ce13 3441 108e 7cd1 6d28 58f9 d6d9  Y...4A..|.m(X...
-00002fa0: 05d7 1a35 82d9 fb57 e3ea 1ac3 3cc8 d6cc  ...5...W....<...
-00002fb0: 13db 0d82 7add e29f 7a23 106e f980 00cc  ....z...z#.n....
-00002fc0: 937a 1004 1ee8 369d 86db 809f fb46 308b  .z....6......F0.
-00002fd0: 5ca1 f870 bfb8 cd6a 8571 c169 7b84 2690  \..p...j.q.i{.&.
-00002fe0: 7794 6755 031c 4676 755a 29ea 3390 4af1  w.gU..FvuZ).3.J.
-00002ff0: 60c8 ff32 32e2 3a08 6370 3677 5a09 8e06  `..22.:.cp6wZ...
-00003000: 248f 521e 63cb 19ea 4cc8 5720 3569 eb6c  $.R.c...L.W 5i.l
-00003010: 08a9 4519 d6a3 3123 b3a8 6e70 f10f 287d  ..E...1#..np..(}
-00003020: 2b1e 58df 2d96 5712 b355 aca0 4fb0 f7f8  +.X.-.W..U..O...
-00003030: 081e c87e 5b17 2a9d 68bb 0fed 41f2 7c89  ...~[.*.h...A.|.
-00003040: 0703 b152 d052 d6a0 baf3 8e33 b678 c6b2  ...R.R.....3.x..
-00003050: 0ac5 4377 54b1 89e8 d9ae 8518 10a3 34bd  ..CwT.........4.
-00003060: e0bb f5fb fe3c 1038 b067 277d 2501 1519  .....<.8.g'}%...
-00003070: 5fce 78ee ca1f e168 983d ca4d 2f1b c0fe  _.x....h.=.M/...
-00003080: ba49 5635 0932 df6a 123f 28a3 140f f20c  .IV5.2.j.?(.....
-00003090: e54c 1b12 8adf 4256 c8f3 c118 3a10 7c63  .L....BV....:.|c
-000030a0: 80ef 450c c76a cf1b 1a8d 2ed1 04c2 3e48  ..E..j........>H
-000030b0: 2d86 14e7 5797 24c4 a20d 1046 9430 1433  -...W.$....F.0.3
-000030c0: 48c6 b594 c457 fc7c 13c7 9131 e93f 08be  H....W.|...1.?..
-000030d0: 6d10 0c95 7049 bfc2 bccd 19b9 3df5 daa4  m...pI......=...
-000030e0: bfd5 0670 5a96 8673 541b 40a3 9cad 45a3  ...pZ..sT.@...E.
-000030f0: 513a e539 ba20 57b6 c0d8 55ab 2b4e 8caa  Q:.9. W...U.+N..
-00003100: fdbc 349e cce9 2b5b 2ed9 8d1f 159b 4ce0  ..4...+[......L.
-00003110: adf5 ab8d f00e 0760 1d3f d07f 0cfc 28f0  .......`.?....(.
-00003120: 80aa 6a0b 3d26 3c4b 890b 3be3 fb7a 9cf5  ..j.=&<K..;..z..
-00003130: 100d 454d 4271 b387 733a 4810 f917 5819  ..EMBq..s:H...X.
-00003140: cefe 47b0 5793 bdb0 9797 9ce1 68c9 3e7a  ..G.W.......h.>z
-00003150: d8a2 e2b2 e423 470e 7b1f 1739 48b8 578f  .....#G.{..9H.W.
-00003160: 6e91 daac 38b9 579e 006b 42c8 02cf 9032  n...8.W..kB....2
-00003170: 2c46 e047 f76a 8567 5ec9 9be5 43b6 1a97  ,F.G.j.g^...C...
-00003180: a171 0cc7 c63a 7890 3b1d 193c 885d d5a9  .q...:x.;..<.]..
-00003190: 767c f016 8c0b 27f0 91e5 04e0 913b b377  v|....'......;.w
-000031a0: e024 4edd c23b 6771 bb6c e13b e676 962c  .$N..;gq.l.;.v.,
-000031b0: 54cb 187e 54c0 eaa2 ea7e 8cc0 94cc e898  T..~T....~......
-000031c0: 18db 21de c290 ddb7 e4bd 7c6b 58d8 825b  ..!.......|kX..[
-000031d0: e0dc d5b5 571f f49b 113c c496 9317 5b4b  ....W....<....[K
-000031e0: 69d3 e303 5363 8192 f33f 3a30 5709 05eb  i...Sc...?:0W...
-000031f0: ceea 255f ba7d fe73 7b7f 1375 0aa8 4c28  ..%_.}.s{..u..L(
-00003200: 15a2 85fa d0bc 8ca1 f12b 3aa8 c13b 9e6d  .........+:..;.m
-00003210: 07be ef07 66dd abbb be6b 3bfc ea4f d425  ....f....k;..O.%
-00003220: f869 4e9b 630c b598 77f2 aecd 346b f0e0  .iN.c...w...4k..
-00003230: f15f e249 fe32 bbf2 ed7b 71a1 5516 a64a  ._.I.2...{q.U..J
-00003240: 055c a2ed 3bbe 6339 7e3d b01d d39f 2be0  .\..;.c9~=....+.
-00003250: c9d6 2e0a ecf3 0d0a 3e7e f8f0 ef6f 3f29  ........>~...o?)
-00003260: 61a4 37c6 295c 30cc 2b2b 55e9 0658 4926  a.7.)\0.++U..XI&
-00003270: 55bd 4c14 9818 bff2 1695 b439 4f60 b804  U.L........9O`..
-00003280: f5a3 71ca 2ee7 2fdb 7af5 fc15 4af0 3803  ..q.../.z...J.8.
-00003290: 0f98 8dfa 065f 1326 44b4 f5ea f925 afc1  ....._.&D....%..
-000032a0: 5b3e e704 ca5e 2f0b 289c c35f 6d4c 31d0  [>...^/.(.._mL1.
-000032b0: 79de ad07 67e7 a15d 6b98 dd46 cd75 9057  y...g..]k..F.u.W
-000032c0: 0bbc ee59 cd73 4fbb 6767 6160 dae6 e97b  ...Y.sO.gga`...{
-000032d0: e5e2 fd0e d7ee e2ff 04a0 3a65 b9cd 2285  ..........:e..".
-000032e0: cb79 3a5b ec0c fc45 d5d7 d695 8684 2fae  .y:[...E....../.
-000032f0: ae00 b68a 3db0 7df3 b967 99b5 d031 ad9a  ....=.}..g...1..
-00003300: eb47 8d5a c377 bc5a e859 f699 ef76 cfbd  .G.Z.w.Z.Y...v..
-00003310: d053 b07b 7b5e cf9b 8665 c98b 7e0e de6b  .S.{{^...e..~..k
-00003320: 329c a114 e7a5 ad4a 0ba9 bd60 2468 6e58  2......J...`$hnX
-00003330: 8451 5ac2 a8fe 09a3 f31f 0000 00ff ff03  .QZ.............
-00003340: 0050 4b03 0414 0006 0008 0000 0021 0088  .PK..........!..
-00003350: b934 c7ff 0500 0035 1c00 0014 0000 0078  .4.....5.......x
-00003360: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
-00003370: 786d 6cac 594b 531b 4710 bea7 2aff 4125  xml.YKS.G...*.A%
-00003380: 558e b140 0e7e a400 1f5c 95aa dc72 48ce  U..@.~...\...rH.
-00003390: 5b63 ed80 b6bc 3bab ec8e 00e5 24ca 7104  [c....;.....$.q.
-000033a0: 36f8 9180 b103 0a0f e307 4e19 3965 0218  6.........N.9e..
-000033b0: 41f9 cfec ec4a 27ff 858c 342b bc52 cfac  A....J'...4+.R..
-000033c0: 94b5 8fea 9dfe a6bb a7e7 eb9e d6f8 b539  ...............9
-000033d0: cb4c cd60 c735 6c32 911e bd30 924e 6192  .L.`.5l2...0.Na.
-000033e0: b775 834c 4fa4 7ffa f1bb afaf a453 2e45  .u.LO........S.E
-000033f0: 4447 a64d f044 ba8c ddf4 b5c9 2fbf 1877  DG.M.D....../..w
-00003400: 5d9a e2ba c49d 4817 282d 7e9b cdba f902  ].....H.(-~.....
-00003410: b690 7bc1 2e62 c2bf 4cd9 8e85 28ff e94c  ..{..b..L...(..L
-00003420: 67dd a283 91ee 1630 a696 99cd 8d8c 5cca  g......0......\.
-00003430: 5ac8 20e9 54de 2e11 3a91 cee5 f836 2562  Z. .T...:....6%b
-00003440: fc5c c2d7 8564 f46a 2e3d 39ee 1a93 e374  .\...d.j.=9....t
-00003450: 3278 fd28 587d c61e 2c07 2fde 8c67 e9e4  2x.(X}..,./..g..
-00003460: 78b6 2d17 df32 2e75 10c5 d365 8d20 0b67  x.-..2.u...e. .g
-00003470: fa3f b3d3 0a7b 71d7 5f7b e66f 6c4a 5491  .?...{q._{.olJT.
-00003480: 4335 9dab 03bd a0f1 875f db54 e861 a2cb  C5......._.T.a..
-00003490: b5bc c6d3 606b de7f 54f5 1a87 6a43 a70c  ....`k..T...jC..
-000034a0: 5362 e842 8d1b dafc f7d7 56f5 a1dc 507e  Sb.B......V...P~
-000034b0: 225a 1eb9 0560 ab77 fc67 d0d8 639b 27ac  "Z...`.w.g..c.'.
-000034c0: fa1b 50bd c14f b360 21e7 260c 4d47 4111  ..P..O.`!.&.MGA.
-000034d0: d573 35cd 2d5b 376c 1368 fb95 865f bb15  .s5.-[7l.h..._..
-000034e0: acdf 013b 529b 2253 9b41 6649 e2e5 e29e  ...;R."S.AfI....
-000034f0: 77f6 44e1 a5d4 397f e590 6f12 dcab 2af6  w.D...9...o...*.
-00003500: 7130 2d39 c485 debd 3b60 4b8f d4da 8890  q0-9....;`K.....
-00003510: 1232 8d5f b0ae 2921 9657 bdb3 6556 adb0  .2._..)!.W..eV..
-00003520: ca29 d89d 272b d508 a60a 47bd c659 6ba7  .)..'+....G..Yk.
-00003530: 26d5 82b6 facb 3bfe e25d a98f dc37 9bdf  &.....;..]...7..
-00003540: 4e18 feb5 67ac 5655 2ba2 9969 9ea2 8659  N...g.VU+..i...Y
-00003550: d6da e191 43bc dd61 775e ca76 9db1 4d44  ....C..aw^.v..MD
-00003560: 0dd3 a065 18d6 ddfb fe93 7dbf be22 d373  ...e......}..".s
-00003570: 0bc8 29c2 43f7 8eef 36b7 975a 4fef b59e  ..).C...6..ZO...
-00003580: ec81 88e8 f62c 710d 1d6b 8ee1 c21c 0d0e  .....,q..k......
-00003590: 76fc fb0f 9af5 13d5 8eb6 430d 62c3 f06c  v.........C.b..l
-000035a0: 54d8 ee0b b6fe 97ff fb2e d8d2 4273 9aee  T...........Bs..
-000035b0: a0d9 f6d6 4053 98e9 358e 6487 3e83 e049  ....@S..5.d.>..I
-000035c0: 346f 6dc8 6231 6b10 ad4d 4c90 59d6 17bc  4om.b1k..ML.Y...
-000035d0: 93fb dc1f 6057 d1b1 a778 5299 b6eb ca55  ....`W...xR....U
-000035e0: fd8d 4a6b f5bd f02a 96d8 a21e 6a7a 89db  ..Jk...*....jz..
-000035f0: c1d9 5de3 34ae a2bb 2872 2cf5 c991 9584  ..].4...(r,.....
-00003600: 18c5 f597 e683 c66b b6bb e7af 4216 97e3  .......k....B...
-00003610: eaa8 0c6f 4bf3 f036 bf5a e266 0f1d 113c  ...oK..6.Z.f...<
-00003620: 97c7 3cac ff3b 30aa cde2 eb43 dc66 ca58  ..<..;0....C.f.X
-00003630: a9b6 8a8d 5bac 5f03 c3f7 e174 8155 b7bc  ....[._....t.U..
-00003640: b3d5 0fa7 8b20 1d43 6815 3b46 cde5 38c1  ..... .Ch.;F..8.
-00003650: fe9a bf51 8fc1 c997 2c35 d376 c8ba 0f71  ...Q....,5.v...q
-00003660: a065 82c2 95a0 adc7 efd9 9b15 ffed 2af0  .e............*.
-00003670: 0c99 c502 0217 b379 5063 dbf0 56de c014  .......yPc..V...
-00003680: aef5 de6f fbf3 7505 2919 44b4 3eed 3bd7  ...o..u.).D.>.;.
-00003690: b97a 70ab 480a b30e a3ca 2824 3c00 05ab  .zp.H.....($<...
-000036a0: 46a3 c5b5 99a8 774a 4e0f c162 a8bd 2fff  F.....wJN..b../.
-000036b0: cef9 7398 2489 a5d4 5ee0 0576 f25c c199  ..s.$...^..v.\..
-000036c0: 964d 6881 97ac d056 2585 368f 369b c7af  .Mh....V%.6.6...
-000036d0: 9af5 3a3b da87 6d81 83f2 37db bd12 761c  ..:;..m...7...v.
-000036e0: 1bd2 357b f892 1ba0 ce8d 598c 6f72 13e4  ..5{......Y.or..
-000036f0: 2922 9415 8912 6a4a f345 28aa 8f3a d455  )"....jJ.E(..:.U
-00003700: 1cb5 d03e af85 c0e5 aeb6 a218 0af5 d894  ...>............
-00003710: 0d11 0667 6e18 81b8 0308 b178 5b3e f81c  ...gn......x[>..
-00003720: 387f abeb 7408 149b 5bdd d0d4 9bfb dba2  8...t...[.......
-00003730: 30fa 47ff f003 56c5 a864 e6b1 a319 44c7  0.G...V..d....D.
-00003740: 73b0 b7e9 a446 70f0 116b e081 09b8 2276  s....Fp..k...."v
-00003750: 3a37 9ee4 712c b4b8 08d1 0de2 8d0d efc1  :7..q,..........
-00003760: 609b 21f0 40cb 7bb0 8776 40d1 eb88 3ba3  `.!.@.{..v@...;.
-00003770: bcaf 9c9b 783f dc7f 24e2 c1a2 ecd0 fbf8  ....x?..$.......
-00003780: 2d8e 85a2 4b07 f060 d0a8 b1fa 3bb1 e980  -...K..`....;...
-00003790: a502 5504 52ce f43d fb3e 7c29 67b5 3ef6  ..U.R..=.>|)g.>.
-000037a0: 5350 5f19 4b5a cb8c aaf6 663e 3ecf 944b  SP_.KZ....f>>..K
-000037b0: a6b1 6d61 ea18 f92e 9d8a 9520 eb33 bd3d  ..ma....... .3.=
-000037c0: 91ac e3ca 002c 65fb ac5e ca9f 2392 662e  .....,e..^..#.f.
-000037d0: 13e6 6158 cb63 ca53 6688 2582 3f15 45b7  ..aX.c.Sf.%.?.E.
-000037e0: 0b30 8098 3221 ed0c 2a42 de71 c5df 58e8  .0..2!..*B.q..X.
-000037f0: 4f6a ef64 4926 3d5e 9448 d9fa ba14 6145  Oj.dI&=^.H....aE
-00003800: b6f6 f66b 29ee 2de9 dabf 656b dfd5 646b  ...k).-...ek..dk
-00003810: 97e7 e552 b97b 6c79 5eee 61fb 2e9d 3c67  ...R.{ly^.a...<g
-00003820: 77b6 f85c 0070 ef28 4cba 1c14 5d84 a26f  w..\.p.(L...]..o
-00003830: a068 0c8a 2e41 d165 28ba 0245 57a1 6874  .h...A.e(..EW.ht
-00003840: 4422 93d8 3f2a 7180 77b8 4059 3e41 e22d  D"..?*q.w.@Y>A.-
-00003850: bdc7 074c 9586 77fc 4af2 1ab2 3022 fd41  ...L..w.J...0".A
-00003860: 74a9 de2f b20c b02a 37f6 55ff aab1 1120  t../...*7.U.... 
-00003870: ba0c 5771 1280 4f73 d9f3 35d3 99d8 4958  ..Wq..Os..5...IX
-00003880: 84db 0ca5 dc6a c952 43b2 9297 a03c 2654  .....j.RC....<&T
-00003890: cb49 0eb8 fb6d 4c72 38dd 6f97 257a dc29  .I...mLr8.o.%z.)
-000038a0: 58e4 3b53 445e 4dfc ad6a 6be7 71f7 c152  X.;SD^M..jk.q..R
-000038b0: 2cf0 e926 35f2 3f38 a929 de85 7eaf f399  ,..&5.?8.)..~...
-000038c0: 643a 45cb 453e f224 f675 9b84 23d2 74b6  d:E.E>.$.u..#.t.
-000038d0: 67fa 085e e109 71c0 7332 214e 6f35 4dea  g..^..q.s2!No5M.
-000038e0: 9464 7496 106a 5011 4f1c ae8f 551c b490  .dt..jP.O...U...
-000038f0: 49bd ee9f 6c7d 92cb a06d 4888 96a1 06ed  I...l}...mH.....
-00003900: 4e8b 9342 f4cf 7d92 e2f4 4e2e 92a2 f434  N..B..}...N....4
-00003910: 2c49 41e0 9b20 7170 2233 cbc4 8111 f39e  ,IA.. qp"3......
-00003920: e8eb 2d29 546c d7f6 d940 7bdb b7a4 b03d  ..-)Tl...@{....=
-00003930: f317 41b4 9f46 1391 c7a0 187a f96b 87ad  ..A..F.....z.k..
-00003940: b583 4e61 9220 5f1c 82a0 a3ec f0d9 303b  ..Na. _.......0;
-00003950: 7f49 0cc3 3bc3 5818 5264 c477 f0d4 49e8  .I..;.X.Rd.w..I.
-00003960: 7b32 e4f8 b297 e57f fb4d fe07 0000 ffff  {2.......M......
-00003970: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00003980: fd81 bcbe 2302 0000 cc04 0000 1800 0000  ....#...........
-00003990: 786c 2f64 7261 7769 6e67 732f 6472 6177  xl/drawings/draw
-000039a0: 696e 6731 2e78 6d6c 9c54 4b6e db30 10dd  ing1.xml.TKn.0..
-000039b0: 17e8 1d08 ee65 7dfd 132c 0575 6c15 018a  .....e}..,.ul...
-000039c0: 348b e600 0445 5902 44d2 2019 db41 9093  4....EY.D. ..A..
-000039d0: 74d5 5d4f d1db 04e8 31ca 9f6c 2371 8136  t.]O....1..l#q.6
-000039e0: 5a50 c319 bd19 f2bd 192d ae0e b407 3b22  ZP.......-....;"
-000039f0: 64c7 5901 e351 0401 6198 d71d db14 f0fe  d.Y..Q..a.......
-00003a00: 5b15 cc20 900a b11a f59c 9102 3e12 09af  [.. ........>...
-00003a10: ca8f 1f16 875a e47b b912 4027 6032 d7db  .....Z.{..@'`2..
-00003a20: 02b6 4a6d f330 94b8 2514 c911 df12 a6a3  ..Jm.0..%.......
-00003a30: 0d17 1429 bd15 9bb0 1668 af53 d33e 4ca2  ...).....h.S.>L.
-00003a40: 6812 caad 20a8 962d 216a e522 d0e7 43ef  h... ..-!j."..C.
-00003a50: c846 51c7 6069 4fa6 f6fc 9af4 fd27 865b  .FQ.`iO......'.[
-00003a60: 2e9c ab11 9c3a 0bf3 be4c 17a1 b981 312d  .....:...L....1-
-00003a70: 401b 5f9b a68c 8e6e b3b3 11c1 f765 ecdc  @._....n.....e..
-00003a80: c61c 7c26 1e27 d3c8 2374 c822 6cd6 5329  ..|&.'..#t."l.S)
-00003a90: c54f 25e3 e9e5 9ae3 743c cffe 5238 492e  .O%.....t<..R8I.
-00003aa0: 574e e274 3e1f 1f63 a7d2 43c1 8d40 dbb6  WN.t>..c..C..@..
-00003ab0: c395 4094 008a b0e0 05f4 dcb0 dde7 b3e0  ..@.............
-00003ac0: 9da7 07df eeee 04e8 ea02 a610 308d 2ae0  ............0.*.
-00003ad0: cbf7 5fbf 7ffc 0489 c6a1 9c1c d417 a9bc  .._.............
-00003ae0: 051e 4457 c0a7 aa4a 96e3 7595 0595 b682  ..DW...J..u.....
-00003af0: 2c5a 66c1 729d cd83 2a49 67eb 645a 5d27  ,Zf.r...*Ig.dZ]'
-00003b00: e9e4 d9a0 e349 8eb5 d24a 37d9 4d3d 281c  .....I...J7.M=(.
-00003b10: 4fde 684c 3b7d 50c9 1b35 c29c 86bc 693a  O.hL;}P..5....i:
-00003b20: 4c86 9ed1 1d13 67a1 d5d8 1ef3 29f2 4fa0  L.....g.....).O.
-00003b30: df33 b344 a725 4a5d f019 86e5 22b4 a71f  .3.D.%J]...."...
-00003b40: def6 164e 7c73 65af cfed 2b52 0ccc 34c8  ...N|se...+R..4.
-00003b50: 65b2 0e8d d0bd 8472 7d42 7028 a01e 9a47  e......r}Bp(...G
-00003b60: b36a 902d 05b0 73e2 c16b 530d 202f 8df9  .j.-..s..kS. /..
-00003b70: d69b 2ba4 90a3 f4bf 2708 b748 284d 31ce  ..+.....'..H(M1.
-00003b80: ade5 b9c5 ef98 1e97 c927 f8a7 6176 faac  .........'..av..
-00003b90: 387e a084 2937 d182 f456 66d9 765b 0981  8~..)7...Vf.v[..
-00003ba0: c84d 4789 9b3a f642 9cdd d80a 7224 c352  .MG..:.B....r$.R
-00003bb0: 74de b55e 98be d3b9 0d41 8322 af46 dbe2  t..^.....A.".F..
-00003bc0: cc8f a8fc 0300 00ff ff03 0050 4b03 0414  ...........PK...
-00003bd0: 0006 0008 0000 0021 00a1 a6aa e6ce 0700  .......!........
-00003be0: 0099 2200 0014 0000 0078 6c2f 6368 6172  .."......xl/char
-00003bf0: 7473 2f63 6861 7274 312e 786d 6cec 5acd  ts/chart1.xml.Z.
-00003c00: 721b b911 bea7 2aef 303b bb39 a548 ce0c  r.....*.0;.9.H..
-00003c10: 3924 67ca d496 3432 375b 91d7 2e4b de43  9$g...427[...K.C
-00003c20: 5229 1788 0149 4418 600c 6024 d25b 7b49  R)...ID.`.`$.[{I
-00003c30: 0e39 e511 72c8 354f 9007 4aa5 92b7 48e3  .9..r.5O..J...H.
-00003c40: 6728 9292 bc94 edcd 561c f940 0ffe 1a8d  g(......V..@....
-00003c50: 467f fd07 3df9 7255 b1e0 8a48 4505 9f84  F...=.rU...HE...
-00003c60: 7137 0a03 c2b1 2829 5f4c c257 17d3 ce38  q7....()_L.W...8
-00003c70: 0c94 46bc 444c 7032 09d7 4485 5f1e fdfc  ..F.DLp2..D._...
-00003c80: 674f 708e 9748 eaf3 1a61 1200 11ae 723c  gOp..H...a....r<
-00003c90: 0997 5ad7 79af a7f0 9254 4875 454d 388c  ..Z.y....THuEM8.
-00003ca0: cd85 ac90 86a6 5cf4 4a89 ae81 78c5 7a49  ......\.J...x.zI
-00003cb0: 140d 7b96 48e8 09a0 f720 5021 cadb f5f2  ..{.H.... P!....
-00003cc0: 90f5 623e a798 9c0a dc54 846b c785 240c  ..b>.....T.k..$.
-00003cd0: 6990 805a d25a b5d4 703c 94c9 2d8a 15c5  i..Z.Z..p<..-...
-00003ce0: 5228 31d7 5d2c aa9e 23d6 1e0a 88c5 696f  R(1.],..#.....io
-00003cf0: 73aa 2310 5289 3489 b368 105c 2136 09a3  s.#.R.4..h.\!6..
-00003d00: b067 3a19 e20b d7f1 76d9 29be 719d 5234  .g:.....v.).q.R4
-00003d10: bc24 6521 2487 ebd8 9a5f e1fc 9869 2239  .$e!$...._...i"9
-00003d20: 902a 04d7 c0b5 9757 7590 c42b 242f 9bba  .*.....Wu..+$/..
-00003d30: 03ec d670 c819 6554 afed b1c3 a327 40bb  ...p..eT.....'@.
-00003d40: 580a 9047 f092 bc69 a824 6a12 e278 7023  X..G...i.$j..xp#
-00003d50: 82c1 4305 108d 7ae3 5ee2 ef15 0e1b 0f72  ..C...z.^......r
-00003d60: a5d7 8cb8 03c5 5162 4edb dbec 6b59 9822  ......QbN...kY."
-00003d70: c666 085f 1ad9 6c4d de4c bd19 370b f785  .f._..lM.L..7...
-00003d80: 6156 5935 321f 9a6a 46ec c7ca fc4a 8a97  aVY52..jF....J..
-00003d90: 474f 503e 13e5 fa85 0ca4 d0e6 1202 55e3  GOP>..........U.
-00003da0: 2995 4a9f 21a5 5f20 097a 079d 8002 fd1c  ).J.!._ .z......
-00003db0: 7ee6 4c5c 4f42 c218 e802 056d 30fd 2005  ~.L\OB.....m0. .
-00003dc0: 21df 86c1 b544 f524 546f 1a24 4918 208e  !....D.$To.$I. .
-00003dd0: a11b 24a6 65db 2834 b463 7346 9433 a5cf  ..$.e.(4.csF.3..
-00003de0: cdd1 6da3 363d 35f0 5092 f905 9a9d bf9d  ..m.6=5.P.......
-00003df0: 8459 3c18 4411 dc02 caa1 f325 8c19 c598  .Y<.D......%....
-00003e00: 844e 2902 0553 6233 2198 59fe a8fd 6d26  .N)..Sb3!.Y...m&
-00003e10: 2107 241a 544a 7a09 88e4 e2dc 7e85 c125  !.$.TJz.....~..%
-00003e20: e808 2c01 5cd9 13da e933 a408 a306 b96e  ..,.\....3.....n
-00003e30: 2325 182d a794 31b3 ab85 2929 9874 97a3  #%.-..1...)).t..
-00003e40: 57b1 6586 35d5 3351 babe 611a 0139 779c  W.e.5.3Q..a..9w.
-00003e50: a67a 3e9f bbee 7edb dddb a202 f70a aded  .z>...~.........
-00003e60: 0d0c aa78 a0d7 3599 8399 9884 bfac 7887  ...x..5.......x.
-00003e70: 6947 8ea0 bd01 82dc 0056 7b03 5859 9d69  iG.......V{.XY.i
-00003e80: a564 b701 499a 13b8 9f7d c921 0637 6b24  .d..I....}.!.7k$
-00003e90: 4978 e7d5 b9a3 aa8f fef1 f7bf fdeb 0f7f  Ix..............
-00003ea0: fde7 5ffe f8ef 3ffd d970 aa2d 21a0 00df  .._...?..p.-!...
-00003eb0: 703b bd56 5be0 435b e511 70f3 0cad 77a0  p;.V[.C[..p...w.
-00003ec0: abfc c65c 1821 3ab9 70c3 c9a6 03a8 31db  ...\.!:.p.....1.
-00003ed0: 43e6 7382 f599 d246 e141 b1ed 4a43 dbb1  C.s....F.A..JC..
-00003ee0: fea8 929f a64a 125e 1a93 b20f 67a3 04ad  .....J.^....g...
-00003ef0: 9e39 1530 7ad6 5a2b d468 7161 1aa7 8411  .9.0z.Z+.hqa....
-00003f00: 4d3c f8bc bba8 99d0 c792 20e7 3ad6 a231  M<........ .:..1
-00003f10: 1a05 5e04 605d 181f 6c1a 0b70 1f35 f855  ..^.`]..l..p.5.U
-00003f20: a7ac ce63 cbd2 7996 2b24 d785 6062 c7ab  ...c..y.+$..`b..
-00003f30: 8042 12d0 7d9c d372 b5a3 e142 96c4 1b04  .B..}..r...B....
-00003f40: bfbf 4303 d89b 9764 6e56 cc77 a0f4 d917  ..C....dnV.w....
-00003f50: c517 b151 703b 06b3 0a04 dedf ccab 7501  ...Qp;........u.
-00003f60: 3e4d 7bcb ef78 a975 001b 3a6b 84f3 aba3  >M{..x.u..:k....
-00003f70: 8a20 6e16 5f59 8cd4 0693 c607 b444 5cc3  . n._Y.......D\.
-00003f80: eebb 8165 0b41 c603 b0d3 c938 1da5 6180  ...e.A.....8..a.
-00003f90: 8d5d 96bc b406 ec5d 460e 610c 0ed4 5ae8  .].....]F.a...Z.
-00003fa0: 7d6b 653d b0bb a777 22d8 3854 273b b5ae  }ke=...w".8T';..
-00003fb0: 6602 e227 e3db ad55 7650 bf99 8091 bd9d  f..'...UvP......
-00003fc0: 6dd9 fd36 fadd 6725 a26c fdfa b509 0ed4  m..6..g%.l......
-00003fd0: 7b8b ee73 b3fc f383 85e7 5901 5ecd ddf0  {..s......Y.^...
-00003fe0: a6da dce6 1647 d784 2e96 fa75 7b2b f64a  .....G.....u{+.J
-00003ff0: 61ea e64a 5d24 5788 921c 45dd 28fa 8565  a..J]$W...E.(..e
-00004000: de46 77b6 efc0 4b8f 6e31 7db3 075c 73cb  .Fw...K.n1}..\s.
-00004010: 9b51 0bc7 adaa 84d0 cb1d 3525 2b63 5acd  .Q........5%+cZ.
-00004020: 51e0 2b68 2478 c7ef 8a7e 7f1c 15c5 a093  Q.+h$x...~......
-00004030: 9e0e 9f76 0651 5674 4e9e f693 ced3 5172  ...v.QVtN.....Qr
-00004040: 9a64 a37e da2f 8aef b7c2 bb07 0777 83ad  .d.~./.......w..
-00004050: b866 9837 9cbe 69c8 d71e acdf 81a3 b4ff  .f.7..i.........
-00004060: 3ac3 3839 ee0c a627 a3ce 493a 9d76 d2a4  :.89...'..I:.v..
-00004070: 3fca 06c0 d8f4 24fd de7a 32cb b3d5 f4f6  ?.....$..z2.....
-00004080: 1446 cfbd 4aed a1d2 6a2a ceb7 50e9 7b7e  .F..J...j*..P.{~
-00004090: 0895 bffa 0054 8e52 7bb3 ff65 50ba 786f  .....T.R{..eP.xo
-000040a0: 2f84 7804 e56b 0fca 51ba 3115 8f90 b449  /.x..k..Q.1....I
-000040b0: a4c9 b70e 8164 fc71 2169 f574 0792 bee7  .....d.q!i.t....
-000040c0: 8720 f9f5 8738 4ab4 fa09 fc64 df47 de3b  . ...8J....d.G.;
-000040d0: 1ef5 1192 2d24 2b77 298f 6e12 93ed 1ac8  ....-$+w).n.....
-000040e0: 2198 4c3e 0c93 e5d9 8c29 5b2f 588a eb33  !.L>.....)[/X..3
-000040f0: b280 a8fb d764 2f55 8391 6f91 8fce 7c28  .....d/U..o...|(
-00004100: aba0 af40 fa1b 54f9 82c4 56ff 3991 77f6  ...@..T...V.9.w.
-00004110: bf20 d284 8cbb 6920 d039 6966 3346 cee9  . ....i .9if3F..
-00004120: db6d 52e0 c86f 58bb 1db5 a055 1b2e c451  .mR..oX....U...Q
-00004130: 1c27 f063 1186 f3ad 812c 1d0c b361 32f6  .'.c.....,...a2.
-00004140: a1c2 4e98 6f42 be63 9b9c de4b 4961 044b  ..N.oB.c...KIa.K
-00004150: 1646 3642 5260 dc56 b61c f715 e5cf d0ca  .F6BR`.V........
-00004160: 13de 9a58 daac 63e7 8468 f542 f82a d4cc  ...X..c..h.B.*..
-00004170: 85ee e074 a695 0e6e 42c0 49f8 1581 5a15  ...t...nB.I...Z.
-00004180: 6250 6e10 0d08 e98c f24b 526e ca5c 15fa  bPn......KRn.\..
-00004190: bd90 1714 5f3e 8380 7937 48c6 39b0 72ff  ...._>..y7H.9.r.
-000041a0: a086 4570 c11b 0ea0 22e3 78b8 33fd 3669  ..Ep....".x.3.6i
-000041b0: 4096 266d 1630 87aa 0324 0455 0d9c 28be  @.&m.0...$.U..(.
-000041c0: 80ca 0c5b 405d c414 696c d1e3 8115 90f8  ...[@]..il......
-000041d0: ee0a c8f8 b00a c8a1 b6f2 6354 050e 2d4e  ..........cT..-N
-000041e0: 992b c4e4 f8d8 5fd4 3d85 aa77 95a5 b2f7  .+...._.=..w....
-000041f0: ac4a 7de2 d5a8 8353 7f28 5842 1159 1dfb  .J}....S.(XB.Y..
-00004200: cc3b de86 bc1f 231e 7ca6 32f0 1b22 85d3  .;....#.|.2.."..
-00004210: 7fd3 da81 299b 3128 ca29 d266 d9ae 5887  ....).1(.).f..X.
-00004220: 7323 e90b 5a91 579c faa1 12ad 5d1d cd15  s#..Z.W.....]...
-00004230: a59d 1581 fcea 9639 d965 e6e3 9b13 e68e  .......9.e......
-00004240: 62ad c357 9296 c6c0 3953 ee6b 6b2e b1ff  b..W....9S.kk...
-00004250: df46 34f8 81db 07bc c382 da2c 7adf 7efa  .F4........,z.~.
-00004260: 0cef e3d9 4f0e 79e6 8557 a11f a782 d919  ....O.y..W......
-00004270: faec f727 2dae 3fda 2c5b 917e 4805 fdbd  ...'-.?.,[.~H...
-00004280: 6dd6 6efc 62ed d9dd 36cb 0e9d 107d 4d08  m.n.b...6....}M.
-00004290: 77b6 6be6 1a3e 0ed9 d8a0 0fd5 4cc0 dc4e  w.k..>......L..N
-000042a0: a9d4 4685 b652 6abf f6e3 1928 ed43 29d5  ..F..Rj....(.C).
-000042b0: 8c57 8837 889d 6dda 2b78 fef0 411d 2917  .W.7..m.+x..A.).
-000042c0: c4d9 abf5 5d9d 6de9 b49b 0cb2 f128 8992  ....].m......(..
-000042d0: 2c49 a341 3a8a 3c84 db88 b49b 25c3 241b  ,I.A:.<.....%.$.
-000042e0: 66e9 789c a651 6663 3b9c 5f7b 53de 4dfb  f.x..Qfc;._{S.M.
-000042f0: 093c b48c 9364 38cc e268 e01e c970 ee2b  .<...d8..h...p.+
-00004300: 5e69 37eb 67f1 6804 d162 361c 8db2 6cfc  ^i7.g.h..b6...l.
-00004310: b4e3 6a25 fbac 8304 6e4e f5ff f27c f108  ..j%....nN...|..
-00004320: fa1f 0ff4 46a1 3630 32e0 fa96 aae7 9c79  ....F.602......y
-00004330: b5f6 4a5e 5255 9fc0 d3e5 a53a f641 cb02  ..J^RU.....:.A..
-00004340: d53e 5e87 3ce9 d4a4 6ae6 6115 528f add8  .>^.<...j.a.R...
-00004350: 0548 6f5e 6d5b e4bf ab70 3f5b dc59 b4ff  .Ho^m[...p?[.Y..
-00004360: 1482 85fd 47c1 fb5f 8fef d175 ffb8 e41e  ....G.._...u....
-00004370: 161f 60d1 6b49 b93e 271a 5e69 1736 045b  ..`.kI.>'.^i.6.[
-00004380: 1204 af3f 53a8 b613 691f 996a b420 90be  ...?S...i..j. ..
-00004390: 2d28 57f6 19ba 6b1e 5bcc 5f32 7447 6100  -(W...k.[._2tGa.
-000043a0: 4fdd f67f f3a8 6e07 dc72 d3ea 8790 6518  O.....n..r....e.
-000043b0: 2aae b1a1 059b 35b5 7b25 d9db bcd5 07fb  *.....5.{%......
-000043c0: 1725 47ff 0100 00ff ff03 0050 4b03 0414  .%G........PK...
-000043d0: 0006 0008 0000 0021 00a2 0807 919f 0400  .......!........
-000043e0: 0087 2600 0014 0000 0078 6c2f 6368 6172  ..&......xl/char
-000043f0: 7473 2f73 7479 6c65 312e 786d 6cec 5a6d  ts/style1.xml.Zm
-00004400: 6fe2 3810 fe2b 917f 4003 f468 292a 957a  o.8..+..@..h)*.z
-00004410: ad56 3a89 de56 7b2b dd67 9338 e05b c7ce  .V:..V{+.g.8.[..
-00004420: d966 29fd f537 765e 88f3 c24b 0bb4 70fb  .f)..7v^...K..p.
-00004430: 0d4f 82e3 7966 fccc 78c6 b781 1a06 332c  .O..yf..x.....3,
-00004440: f55f 7ac9 88f7 1233 0e02 3542 33ad 93a1  ._z....3..5B3...
-00004450: efab 6046 62ac 2e62 1a48 a144 a42f 0211  ..`Fb..b.H.D./..
-00004460: fb22 8a68 40fc 50e2 05e5 53bf d7e9 f6fc  .".h@.P...S.....
-00004470: d52c 289b 06d7 6611 09e1 f089 48c8 186b  .,(...f.....H..k
-00004480: 7521 e434 9f23 6630 4be7 ca8f 31e5 c8a3  u!.4.#f0K...1...
-00004490: e108 f57a d7e8 ee16 9687 5fa8 fa4e 3523  ...z......_..N5#
-000044a0: 76c4 f837 12c1 0b2f 23d4 41be 1545 94b1  v..7.../#.A..E..
-000044b0: 9a90 4411 0974 fd5d c157 c298 7221 e123  ..D..t.].W..r!.#
-000044c0: 7868 d524 0f4c 7a3f 311b 21fd d2b5 6236  xh.$.Lz?1.!...b6
-000044d0: 8f9f 4498 caae fa9d 8efd 221e 82f8 6b14  ..D......."...k.
-000044e0: a5e2 cb5c ec97 66b9 bbf5 61e1 51fa 2dbb  ...\..f...a.Q.-.
-000044f0: c690 44df 9ea5 a75e 47a8 6be6 f17e 10c9  ..D....^G.k..~..
-00004500: e137 286d b430 afbb 7a06 5893 a990 cb7b  .7(m.0..z.X....{
-00004510: d0fe 9415 57c9 b334 0833 ee2d 46e8 a6df  ....W..4.3.-F...
-00004520: eb23 2fc0 c908 450c 6bf8 1927 606b c5a7  .#/...E.k..'`k..
-00004530: c8c3 6c0a 8804 3ab3 8860 34fc 0296 ddd2  ..l...:..`4.....
-00004540: 3cdd 66f3 0c5a cc03 c62a 7f40 8a39 0f8d  <.f..Z...*.@.9..
-00004550: 1dcc 4253 73a4 0b07 bb94 4c77 d36c b99a  ..BSs.....Lw.l..
-00004560: adec 5eb8 9704 7bb1 0861 3361 c6c4 e24f  ..^...{..a3a...O
-00004570: 61d4 f9fa 9348 4943 02ea 5ad9 9872 92cb  a....HIC..Z..r..
-00004580: 527f 3f9a 8767 7e57 76d3 dc5a 0e38 95cd  R.?..g~Wv..Z.8..
-00004590: 3199 76ad cb56 203c 0b03 b7ed cdc2 a0e9  1.v..V <........
-000045a0: 66c6 1a8f f184 806f 827f 7c18 235d 37bb  f......o..|.#]7.
-000045b0: 7c6f 6746 6a71 ebd0 51b3 183d 18cf 9deb  |ogFjq..Q..=....
-000045c0: e3e9 1efe d837 1b6f e3e6 4cb7 b8b9 25a4  .....7.o..L...%.
-000045d0: 35ec d4b4 dcc2 266e f028 2c58 091e ced6  5.....&n.(,X....
-000045e0: da9d 93c0 2927 225c 42bc 9142 9b38 e9a9  ....)'"\B..B.8..
-000045f0: 24f8 42a5 d263 acf4 3396 1099 bbc8 0326  $.B..c..3......&
-00004600: d286 7a22 2022 205e 4613 e4cd 847c adca  ..z" " ^F....|..
-00004610: cc7b 10ca e109 f216 d270 b7fa 778e 2541  .{.......p..w.%A
-00004620: 1efb 8303 bb5d 5ef5 afaf 90a7 eda0 3be8  .....]^.......;.
-00004630: 0d06 c893 e527 93f2 13cc 0398 2a25 7a2f  .....'......*%z/
-00004640: 1d3c 6818 a736 56c9 fd5c 0351 ea8c 9c52  .<h..6V..\.Q...R
-00004650: 3d52 466e f440 237c 1694 6fe7 8fe6 2380  =RFn.@#|..o...#.
-00004660: 8e32 c94e 11ed 317c 310f c259 2e61 df7a  .2.N..1|1..Y.a.z
-00004670: 770a f146 824d 66b0 b43a c59a 1c21 755c  w..F.Mf..:...!u\
-00004680: f3cb d5bb 185d 3e6e b52f cf10 874c f302  .....]>n./...L..
-00004690: 0913 58eb 586c 30bf e5f2 7a52 6999 0040  ..X.Xl0...zRi..@
-000046a0: 3fa4 47a4 f1b3 37e8 5fe7 1992 e461 9a9c  ?.G...7._....a..
-000046b0: ae21 9b16 5fc1 c3d6 8cc6 719e 02a4 02b6  .!.._.....q.....
-000046c0: 272c 2135 dd1f 70a7 bbdf 9c9c 7513 e9b7  ',!5..p.....u...
-000046d0: edd9 6a3e e9a0 5fc2 ba82 ff18 2f21 c47a  ..j>.._...../!.z
-000046e0: 6a19 4f04 9c47 022a 0306 7cab e82b 19a1  j.O..G.*..|..+..
-000046f0: 7e76 ee29 fef3 3795 2492 383e 417f 2f1d  ~v.)..7.$.8>A./.
-00004700: 088e e0ee 2e50 06bf ef78 72da 07cb 3c95  .....P...xr...<.
-00004710: e1f6 7401 11e7 bc8f 5aae cd42 b1e0 bfe3  ..t.....Z..B....
-00004720: 06b6 3a54 61c0 e476 6f8c ea7b c862 db4f  ..:Ta..vo..{.b.O
-00004730: 5c9b e869 0f05 8df5 39a9 e5b5 9235 4229  \..i....9....5B)
-00004740: 92e6 087c c89a cd1a d31c fa78 5ad4 81dc  ...|.......xZ...
-00004750: 0cbf a81a adcb f037 45eb 3296 503d 10f2  .......7E.2.P=..
-00004760: a83e 6f7c e703 81dd b1ee b66d 61c7 38ac  .>o|.......ma.8.
-00004770: 8325 9c82 c411 9964 03aa 0e9d 9bdd 5d08  .%.....d......].
-00004780: 6ac7 415b 6a2c 163f 85e2 1283 d4f7 09ff  j.A[j,.?........
-00004790: f389 d439 d1e2 9081 b60e 6821 31e5 e3e3  ...9......h!1...
-000047a0: 9680 3e70 1f36 179b 6ede 595f 7510 2ef0  ..>p.6..n.Y_u...
-000047b0: 9cd1 b1f8 5f45 8f1d 4b79 bb90 9c8b 25c1  ...._E..Ky....%.
-000047c0: 2191 bf02 f308 ed23 30b3 0a9a 644a 7878  !......#0...dJxx
-000047d0: 265d aa96 9a30 5be9 9830 a14f aec7 61f8  &]...0[..0.O..a.
-000047e0: 265f b8b5 543e b87c 3ca9 5e4d 598f acf2  &_..T>.|<.^MY...
-000047f0: a588 a444 9d7a bf70 73b7 ada2 673a fc45  ...D.z.ps...g:.E
-00004800: 69fb a1b4 0a9a fa9c faee bf99 eeed c4f6  i...............
-00004810: 434a dd77 d31b b1b2 0956 c464 ced9 c502  CJ.w.....V.d....
-00004820: b3c3 56ea 6b09 d46e 9eee ab32 9a5f 5e38  ..V.k..n...2._^8
-00004830: 7c49 b97b d3e9 83e2 b6e9 feae 1a5b 020d  |I.{.........[..
-00004840: a447 ac66 e9c5 07b5 548f 4267 6d0a b769  .G.f....T.Bgm..i
-00004850: 6ea1 7300 2be0 fb04 6dd3 bd5d e468 0991  n.s.+...m..].h..
-00004860: 0dba ce93 53a9 52b5 763d 8bdb 1b6f 2935  ....S.R.v=...o)5
-00004870: bde7 7246 e379 7705 28dc d799 93f3 0f7a  ..rF.yw.(......z
-00004880: ae9a 0b68 c17f 9a83 e78e a58a 74ed 8622  ...h........t.."
-00004890: 5637 c6ee fe03 0000 ffff 0300 504b 0304  V7..........PK..
-000048a0: 1400 0600 0800 0000 2100 1c14 a7a8 fd00  ........!.......
-000048b0: 0000 6e03 0000 1500 0000 786c 2f63 6861  ..n.......xl/cha
-000048c0: 7274 732f 636f 6c6f 7273 312e 786d 6ca4  rts/colors1.xml.
-000048d0: 9341 6ec2 3010 45af 12f9 0071 1220 ad22  .An.0.E....q. ."
-000048e0: c2a6 eb8a 0527 184d 6c62 c9f6 20db a570  .....'.Mlb.. ..p
-000048f0: 7b9c 5068 4321 12c1 3bfb ebbf f97f 242f  {.PhC!..;.....$/
-00004900: d157 489a dc26 1cb5 480e 46db f8e0 6bd6  .WH..&..H.F...k.
-00004910: 86b0 ab38 f7d8 0a03 3e35 0a1d 7992 2145  ...8....>5..y.!E
-00004920: 329c a454 2878 e3e0 5bd9 2d2f b2bc e0d8  2..T(x..[.-/....
-00004930: 820b 3d85 fd60 e01f 8576 c2c6 1192 9c81  ..=..`...v......
-00004940: e053 72db 0bc3 e848 c94a 6e40 5996 1811  .Sr....H.Jn@Y...
-00004950: da9a e111 b560 896a 6a96 676c b584 aa4f  .....`.jj.gl...O
-00004960: 233e b44b f6a0 6b06 88c2 869c f187 5a31  #>.K..k.......Z1
-00004970: a2cd 46b4 f988 b618 d1ca 4e8b 2bdd 8353  ..F.......N.+..S
-00004980: 1014 d99b 6b17 547f 994f 6ace 0dca 2c9e  ....k.T..Oj...,.
-00004990: cec3 ff9a 8688 5bcf fbc5 d3a3 d652 9e51  ......[......R.Q
-000049a0: 717d d351 4f8c bf46 1e8e 9f4f 18bf 98e0  q}.QO..F...O....
-000049b0: 79bb df7e f60a ea89 f6d7 c8c3 f68f 9a74  y..~...........t
-000049c0: e4df efb5 3a01 0000 ffff 0300 504b 0304  ....:.......PK..
-000049d0: 1400 0600 0800 0000 2100 15af aa3c bd00  ........!....<..
-000049e0: 0000 2b01 0000 2300 0000 786c 2f77 6f72  ..+...#...xl/wor
-000049f0: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
-00004a00: 6565 7431 2e78 6d6c 2e72 656c 7384 8fcd  eet1.xml.rels...
-00004a10: 0ac2 3010 84ef 82ef 10f6 6ed2 7a10 91a6  ..0.......n.z...
-00004a20: 5e44 f02a f501 9664 fb83 6d12 b2f1 a76f  ^D.*...d..m....o
-00004a30: 6f2e 8282 e06d 6797 fd66 a6da 3fa7 51dc  o....mg..f..?.Q.
-00004a40: 29f2 e09d 8652 1620 c819 6f07 d769 b834  )....R. ..o..i.4
-00004a50: c7d5 1604 2774 1647 ef48 c34c 0cfb 7ab9  ....'t.G.H.L..z.
-00004a60: a8ce 3462 ca4f dc0f 8145 a638 d6d0 a714  ..4b.O...E.8....
-00004a70: 764a b1e9 6942 963e 90cb 97d6 c709 5396  vJ..iB.>......S.
-00004a80: b153 01cd 153b 52eb a2d8 a8f8 c980 fa8b  .S...;R.........
-00004a90: 294e 5643 3cd9 1244 3387 ecfc 9fed db76  )NVC<..D3......v
-00004aa0: 3074 f0e6 3691 4b3f 2c94 8df8 c8cd 3212  0t..6.K?,.....2.
-00004ab0: 6347 4983 94ef 1dbf 8752 e6c8 a0ea 4a7d  cGI......R....J}
-00004ac0: 55ac 5f00 0000 ffff 0300 504b 0304 1400  U._.......PK....
-00004ad0: 0600 0800 0000 2100 0e44 f4df bc00 0000  ......!..D......
-00004ae0: 2501 0000 2300 0000 786c 2f64 7261 7769  %...#...xl/drawi
-00004af0: 6e67 732f 5f72 656c 732f 6472 6177 696e  ngs/_rels/drawin
-00004b00: 6731 2e78 6d6c 2e72 656c 7384 8fcd 0ac2  g1.xml.rels.....
-00004b10: 3010 84ef 82ef 10f6 6ed2 7a10 91a6 bd88  0.......n.z.....
-00004b20: d0ab d407 58d2 ed0f b649 c846 b16f 6fa0  ....X....I.F.oo.
-00004b30: 1705 c1d3 b03b ec37 3b45 f59a 27f1 a4c0  .....;.7;E..'...
-00004b40: a3b3 1a72 9981 206b 5c3b da5e c3ad b9ec  ...r.. k\;.^....
-00004b50: 8e20 38a2 6d71 7296 342c c450 95db 4d71  . 8.mqr.4,.P..Mq
-00004b60: a509 633a e261 f42c 12c5 b286 2146 7f52  ..c:.a.,....!F.R
-00004b70: 8acd 4033 b274 9e6c 723a 1766 8c69 0cbd  ..@3.t.lr:.f.i..
-00004b80: f268 eed8 93da 67d9 4185 4f06 945f 4c51  .h....g.A.O.._LQ
-00004b90: b71a 42dd e620 9ac5 a7e4 ff6c d775 a3a1  ..B.. .....l.u..
-00004ba0: b333 8f99 6cfc 11a1 cc80 2126 2086 9ea2  .3..l.....!& ...
-00004bb0: 0629 d70d af92 cbf4 2ca8 b250 5fe5 ca37  .)......,..P_..7
-00004bc0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00004bd0: 0000 0021 0080 1bdc 81d2 0000 008f 0100  ...!............
-00004be0: 001f 0000 0078 6c2f 6368 6172 7473 2f5f  .....xl/charts/_
-00004bf0: 7265 6c73 2f63 6861 7274 312e 786d 6c2e  rels/chart1.xml.
-00004c00: 7265 6c73 ac90 c14a c430 1086 ef82 ef10  rels...J.0......
-00004c10: e66e d3ec 4144 36dd 8320 ec55 d707 08e9  .n..AD6.. .U....
-00004c20: b40d 9b64 c24c 10fb f6a6 17b1 8b47 8f33  ...d.L.......G.3
-00004c30: c3ff 7d3f 733c 7da5 a83e 9125 50b6 60ba  ..}?s<}..>.%P.`.
-00004c40: 1e14 664f 63c8 b385 8fcb ebc3 1328 a92e  ..fOc........(..
-00004c50: 8f2e 5246 0b2b 0a9c 86fb bbe3 1b46 575b  ..RF.+.......FW[
-00004c60: 4896 5044 354a 160b 4bad e559 6bf1 0b26  H.PD5J..K..Yk..&
-00004c70: 271d 15cc ed32 1127 57db c8b3 2ece 5fdd  '....2.'W....._.
-00004c80: 8cfa d0f7 8f9a 7f33 60d8 31d5 79b4 c0e7  .......3`.1.y...
-00004c90: f100 eab2 9666 be61 a7e0 9984 a6da 794a  .....f.a......yJ
-00004ca0: 9aa6 29f8 8d6a cc9e aafd e2b8 be50 247e  ..)..j.......P$~
-00004cb0: af6b c446 733c 63b5 e0b7 9d98 ae15 04fd  .k.Fs<c.........
-00004cc0: b7db fc87 fb46 2b5b 8b1f abde bd71 f806  .....F+[.....q..
-00004cd0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00004ce0: 0000 2100 c063 9302 5001 0000 6502 0000  ..!..c..P...e...
-00004cf0: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
-00004d00: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
-00004d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c60: 0000 bc94 4d6a c330 1085 f785 de41 685f  ....Mj.0.....Ah_
+00000c70: cb76 1237 2d91 b309 856c 5bf7 00c2 1eff  .v.7-....l[.....
+00000c80: 105b 329a 495b dfbe c2a5 8d03 41dd 186f  .[2.I[......A..o
+00000c90: 0433 83de fb34 82b7 db7f 752d fb00 8b8d  .3...4....u-....
+00000ca0: d192 4741 c819 e8dc 148d ae24 7fcf 5e1e  ..GA.......$..^.
+00000cb0: b69c 2129 5da8 d668 907c 00e4 fbf4 fe6e  ..!)]..h.|.....n
+00000cc0: f70a ad22 7709 eba6 47e6 5434 4a5e 13f5  ..."w...G.T4J^..
+00000cd0: cf42 605e 43a7 3030 3d68 3729 8ded 14b9  .B`^C.00=h7)....
+00000ce0: d256 a257 f949 5520 e230 4c84 9d6a f0f4  .V.W.IU .0L..j..
+00000cf0: 4a93 1d0b c9ed b170 fed9 d03b e7ff b54d  J......p...;...M
+00000d00: 5936 391c 4c7e ee40 d30d 0b81 34b4 ee01  Y69.L~.@....4...
+00000d10: 2c53 b602 92fc a70e 1c23 17b7 ed57 73da  ,S.......#...Ws.
+00000d20: 7f1a 7bc2 1a80 2e04 7f2d 14e3 64e5 8379  ..{......-..d..y
+00000d30: 9c13 86dc 1fc1 0564 2cc5 7846 3e86 78e1  .......d,.xF>.x.
+00000d40: 85c4 3e98 6861 18ef 6692 8561 12df 6636  ..>.ha..f..a..f6
+00000d50: 0bc3 6c7c 30eb 8561 d63e 98a7 5903 a556  ..l|0..a.>..Y..V
+00000d60: 168a 37b2 2e2f a7b9 326d ffc2 88ab c84c  ..7../..2m.....L
+00000d70: bf01 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00000d80: 0800 0000 2100 179d a776 3506 0000 e326  ....!....v5....&
+00000d90: 0000 1800 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00000da0: 6574 732f 7368 6565 7431 2e78 6d6c 9c93  ets/sheet1.xml..
+00000db0: 5d6f 9b30 1486 ef27 f53f 58be 0f06 42b2  ]o.0...'.?X...B.
+00000dc0: 1485 545d ab6a bd9b d67d 5c3b e610 acd8  ..T].j...}\;....
+00000dd0: 98d9 261f 9af6 df77 0c21 a994 9ba8 086c  ..&....w.!.....l
+00000de0: b07d 9ef7 3df6 61f9 70d0 8aec c03a 699a  .}..=.a.p....:i.
+00000df0: 8226 514c 0934 c294 b2d9 14f4 e78f 97c9  .&QL.4..........
+00000e00: 8212 e779 5372 651a 28e8 111c 7d58 dd7d  ...ySre.(...}X.}
+00000e10: 5aee 8ddd ba1a c013 2434 aea0 b5f7 6dce  Z.......$4....m.
+00000e20: 9813 3568 ee22 d342 8333 95b1 9a7b fcb4  ..5h.".B.3...{..
+00000e30: 1be6 5a0b bcec 83b4 6269 1ccf 99e6 b2a1  ..Z.....bi......
+00000e40: 0321 b7b7 304c 5549 01cf 4674 1a1a 3f40  .!..0LUI..Ft..?@
+00000e50: 2c28 eed1 bfab 65eb 469a 16b7 e034 b7db  ,(....e.F....4..
+00000e60: ae9d 08a3 5b44 aca5 92fe d843 29d1 227f  ....[D.....C).".
+00000e70: dd34 c6f2 b5c2 bc0f 49c6 0539 58bc 537c  .4......I..9X.S|
+00000e80: a6a3 4c3f 7ea5 a4a5 b0c6 99ca 4748 6683  ..L?~.......GHf.
+00000e90: e7eb f4ef d93d e3e2 4cba ceff 264c 9231  .....=..L...&L.1
+00000ea0: 0b3b 190e f082 4a3f 6629 999d 59e9 0536  .;....J?f)..Y..6
+00000eb0: fd20 6c7e 8685 edb2 7927 cb82 fe8d 4fd7  . l~....y'....O.
+00000ec0: 04fb 2434 f1a5 19e7 fed1 d5b2 9478 c221  ..$4.........x.!
+00000ed0: 2b62 a12a e863 927f 99a5 94ad 967d 01fd  +b.*.c.......}..
+00000ee0: 92b0 77ef de89 e7eb 3750 203c a048 4249  ..w.....7P <.HBI
+00000ef0: a8cf b531 dbb0 f015 8762 44ba 7e41 4072  ...1.....bD.~A@r
+00000f00: e1e5 0e9e 4029 2467 58e2 7f06 912c 08b0  ....@)$gX....,..
+00000f10: b3c2 fbf7 51ed a5af e86f 9694 50f1 4ef9  ....Q....o..P.N.
+00000f20: 27a3 7ecb d2d7 055d 448b cf33 3a8e 7f37  '.~....]D..3:..7
+00000f30: fbaf 2037 b52f 681a 47c9 985a dfa3 3fd1  .. 7./h.G..Z..?.
+00000f40: 396f f4b8 0207 fa4a cacb e333 3881 a58d  9o.....J...38...
+00000f50: 8ea3 6416 ec08 a350 1b5b a265 f847 b134  ..d....P.[.e.G.4
+00000f60: f961 c871 d09d 8604 fc31 9429 9eda 003e  .a.q.....1.)...>
+00000f70: 594a 4e80 2114 67fb 50ec f743 6836 8fd0  YJN.!.g.P..Ch6..
+00000f80: f14d c178 8683 ee7c ba40 c113 e094 f399  .M.x...|.@......
+00000f90: 10b6 af37 fc1f 0000 ffff 0000 00ff ffb4  ...7............
+00000fa0: 9add 6ed3 4010 465f a5f2 0310 ef9f 1d57  ..n.@.F_.......W
+00000fb0: 4924 502f 788d 2844 940b 5a54 8702 6fcf  I$P/x.(D..ZT..o.
+00000fc0: eece d4d9 99d9 b91c ae50 f898 1cb9 39f9  .........P....9.
+00000fd0: 3ceb 1ed6 e7eb f5f6 74be 9d4f 87b7 d73f  <.......t..O...?
+00000fe0: 0f6f c7c1 0d0f ebaf f3cb 9aff f6e8 8787  .o..............
+00000ff0: e7db 71f0 e327 37b6 7f72 e6f2 7bbd bdfe  ..q..'7..r..{...
+00001000: fc7a fdf1 bd24 f20b 7f5d 3c5f 1ebf fd7b  .z...$...]<_...{
+00001010: baae 97eb 4b7e 2dff a734 9c0e 9732 f473  ....K~-..4...2.s
+00001020: 999a 6379 60fe 9735 bffc 7e1a 0fbb f7d3  ..cy`..5..~.....
+00001030: 6177 c1c8 178c 3409 b725 7619 6e23 cc43  aw....4..%v.n#.C
+00001040: 0c08 cbd4 4c18 9af7 f78c 1022 6d22 f409  ....L......"m"..
+00001050: 73c4 80b0 4c65 8491 1142 a425 4c7d c268  s...Le...B.%L}.h
+00001060: 4258 a632 c289 1142 a425 9cfb 84c9 84b0  BX.2...B.%......
+00001070: 4c65 847b 4608 9196 70e9 134e 2684 652a  Le.{F...p..N&.e*
+00001080: 2374 5c15 c8b4 884e 7165 3661 2c53 3923  #t\....Nqe6a,S9#
+00001090: 9705 3284 51b1 656f c258 a666 c6fc 79db  ..2.Q.eo.X.f..y.
+000010a0: be71 1cd7 0532 24a2 f8b2 9830 96a9 9c91  .q...2$....0....
+000010b0: 0b03 19c2 a818 e346 13c8 3a96 5372 6930  .......F..:.Sri0
+000010c0: 94dd b95f 6d45 1b67 d430 d81f ed95 f2a2  ..._mE.g.0......
+000010d0: 6320 d462 7ac5 9cd2 5516 4588 3d43 30b9  c .bz...U.E.=C0.
+000010e0: 3bf5 bd8f 43d6 7cbb 9a5e 91a7 1496 0526  ;...C.|..^.....&
+000010f0: 960d c1e4 fad4 f73e 0e24 a3f8 533c b4c0  .......>.$..S<..
+00001100: c4c6 2108 dca0 fade c781 fcd0 3585 6c5a  ..!.........5.lZ
+00001110: 27df 0809 d1bd 5008 4204 5353 c8a6 7a5c  '.....P.B.SS..z\
+00001120: a77b 8250 0842 f9eb 7dfb 6c06 4d21 9bf6  .{.P.B..}.l.M!..
+00001130: 719d fa09 4221 08e5 6ff8 3ba6 a690 4d01  q...B!..o.;...M.
+00001140: 396c 2072 bf28 1482 10c1 d414 b2e9 2087  9l r.(........ .
+00001150: 2544 3085 4210 2298 8a42 dea6 85ea 5876  %D0.B."..B....Xv
+00001160: cf11 b842 1822 9f4d 4521 6fd3 4275 2cbf  ...B.".ME!o.Bu,.
+00001170: 49e7 0a61 285f d3ed b319 b55d c768 d9e9  I..a(_.....].h..
+00001180: 6c3b 51ac 3b10 6aaf 6654 14f2 362d 54c7  l;Q.;.j.fT..6-T.
+00001190: f2ab c915 c210 c154 14f2 362d 54c7 724c  .......T..6-T.rL
+000011a0: aed0 4728 eb71 ffa9 6b0e d9d4 90ef 6c3f  ..G(.q..k.....l?
+000011b0: 5138 8421 c2a9 4964 d343 bed3 4349 4824  Q8.!..Id.C..CIH$
+000011c0: 97a0 a449 64d3 43be d343 4948 84a1 f672  ...Id.C..CIH...r
+000011d0: 26cd 229b 22f2 9d22 4ac2 220c 114e 4d23  &.".".."J."..NM#
+000011e0: 9b26 f29d 264a 4223 0891 230e c5a2 60d3  .&..&JB#..#...`.
+000011f0: 4475 2cdb 8712 b708 43ed cd5c 5224 0a36  Du,.....C..\R$.6
+00001200: 4d54 c732 cc89 4b84 a116 7352 240a 364d  MT.2..K...sR$.6M
+00001210: 54c7 724c 2e11 8608 a676 f466 74f6 d6d9  T.rL.....v.ft...
+00001220: 8726 71fa 06a1 766d 9b14 8582 4d13 d5b1  .&q...vm....M...
+00001230: fc6a 7285 3044 3035 856c 8a28 74f6 a149  .jr.0D05.l.(t..I
+00001240: 2804 2182 a929 64d3 4301 7ba8 dd2e 67a1  (.!..)d.C.{...g.
+00001250: 1084 5acc 5953 c8a6 8702 560c c114 0a41  ..Z.YS....V....A
+00001260: a855 68d6 14b2 a9a1 d039 919b 8542 1022  .Uh......9...B."
+00001270: 989a 4236 2d14 3a87 72b3 5008 4204 5351  ..B6-.:.r.P.B.SQ
+00001280: 28da b450 1dcb 4c9f b942 1822 988a 42d1  (..P..L..B."..B.
+00001290: a685 ea58 7ee0 ce15 c250 bb5d ee15 85a2  ...X~....P.]....
+000012a0: 4d0b d5b1 1c93 2b84 2182 a928 146d 5aa8  M.....+.!..(.mZ.
+000012b0: 8ee5 985c 210c 114c ed29 904d 0b45 3c95  ...\!..L.).M.E<.
+000012c0: 6b6f d2f6 e241 1084 08a6 a690 4d0b c5ce  ko...A......M...
+000012d0: 3ab4 170a 4188 606a 0ad9 b450 ec6c 438b  :...A.`j...P.lC.
+000012e0: 5048 9eca 2d9a 4236 2d14 3bdb d022 1482  PH..-.B6-.;.."..
+000012f0: 50bb ab2f 9a42 362d 143b cbd0 2214 92a7  P../.B6-.;.."...
+00001300: 728b a690 4d0b c5ce 2eb4 0885 e4a9 dca2  r...M...........
+00001310: 3d4d b569 a154 c6b2 2fa4 453c 5085 50ab  =M.i.T../.E<P.P.
+00001320: d0a2 2894 6c5a a88e 6598 f937 1af8 835f  ..(.lZ..e..7..._
+00001330: 7838 d472 ba51 9128 d9f4 501d 9b41 dbc6  x8.r.Q.(..P..A..
+00001340: 7623 b7e8 2395 79ef 4fdb 46ee d1ee febb  v#..#.y.O.F.....
+00001350: 1dff 0100 00ff ff00 0000 ffff 3c8d 410a  ............<.A.
+00001360: c230 1045 af12 e600 d622 2248 d38d ab2e  .0.E.....""H....
+00001370: 04af 10cd 3419 d499 3019 2cde de54 d0dd  ....4...0.,..T..
+00001380: 7ff0 f86f 2859 188d 6e17 75b3 b04d d1c3  ...o(Y..n.u..M..
+00001390: 0e9c bd0b 7a60 3909 bf50 2b09 4337 0e25  ....z`9..P+.C7.%
+000013a0: 243c 074d c4d5 3d70 360f dbcd 610f 4e29  $<.M..=p6...a.N)
+000013b0: e53f 9814 0f3d b8ab 98c9 f33b 3386 88ba  .?...=.....;3...
+000013c0: da4d 9e45 ec07 ed33 6a58 8893 d323 b5b4  .M.E...3jX...#..
+000013d0: 4eb1 5f4b dd22 7aaf 19d1 c60f 0000 00ff  N._K."z.........
+000013e0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+000013f0: 0086 3fa2 e2c0 0300 00eb 0a00 0018 0000  ..?.............
+00001400: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00001410: 6865 6574 322e 786d 6c9c 93db 8e9b 3010  heet2.xml.....0.
+00001420: 86ef 2bf5 1d2c df87 530e 9ba0 9055 b5ab  ..+..,..S....U..
+00001430: 55b7 aaaa 2a3d 5d3b 6608 566c 4c6d 9343  U...*=];f.VlLm.C
+00001440: 577d f78e 21b0 9172 932e 02db 7834 df3f  W}..!..r....x4.?
+00001450: 837f 96f7 4725 c91e 8c15 baca 681c 4494  ....G%......h.D.
+00001460: 40c5 752e aa6d 467f 7c7f 1acd 29b1 8e55  @.u..mF.|...)..U
+00001470: 3993 ba82 8c9e c0d2 fbd5 fb77 cb83 363b  9..........w..6;
+00001480: 5b02 3882 84ca 66b4 74ae 4ec3 d0f2 1214  [.8...f.t.N.....
+00001490: b381 aea1 c248 a18d 620e 5fcd 36b4 b501  .....H..b._.6...
+000014a0: 96b7 494a 8649 14cd 42c5 4445 3b42 6a6e  ..IJ.I..B.DE;Bjn
+000014b0: 61e8 a210 1c1e 356f 1454 ae83 1890 cc61  a.....5o.T.....a
+000014c0: fdb6 14b5 ed69 8adf 8253 ccec 9a7a c4b5  .....i...S...z..
+000014d0: aa11 b111 52b8 530b a544 f1f4 795b 69c3  ....R.S..D..y[i.
+000014e0: 3612 fb3e c613 c6c9 d1e0 9de0 33ee 65da  6..>........3.e.
+000014f0: fd2b 2525 b8d1 5617 2e40 72d8 d57c ddfe  .+%%..V..@r..|..
+00001500: 225c 848c 0fa4 ebfe 6fc2 c493 d0c0 5ef8  "\......o.....^.
+00001510: 037c 4525 6f2b 299e 0eac e415 367e 236c  .|E%o+).....6~#l
+00001520: 36c0 fce7 3269 23f2 8cbe 44e7 6b84 73ec  6...2i#...D.k.s.
+00001530: 8768 14c5 7eb8 b8fe d2d5 3217 78c2 be2b  .h..~.....2.x..+
+00001540: 62a0 c8e8 8738 5d27 345c 2d5b fffc 1470  b....8]'4\-[...p
+00001550: b017 6be2 74fd 190a f700 5266 f453 4cc9  ..k.t.....Rf.SL.
+00001560: 1fad d537 ce24 7cf1 0ec4 4dd4 a0c4 bb76  ...7.$|...M....v
+00001570: a3f5 cee7 3f63 3511 0a59 90c0 bd7f 08c3  ....?c5..Y......
+00001580: 690f 1d63 7d87 c6ff dd4a e312 75c3 41f8  i..c}....J..u.A.
+00001590: 72dd 17f1 d4fa fcab 2139 14ac 91ee 41cb  r.......!9....A.
+000015a0: 5f22 77a5 d70d e677 53da 07d6 faf0 11c4  _"w....wS.......
+000015b0: b674 1899 073e d05a 28cd 4f8f 6039 7a1a  .t...>.Z(.O.`9z.
+000015c0: 8b0a e2a9 57e4 5a22 1e47 a284 ff39 d193  ....W.Z".G...9..
+000015d0: ecd8 ce87 333a 0966 0912 ac3b 798f e291  ....3:.f...;y...
+000015e0: f1c6 3aad 7ae5 33a4 4bc7 6897 8e7f f439  ..:.z.3.K.h....9
+000015f0: 3f99 fc47 7ebc e801 b3f1 7c32 30fa f686  ?..G~.....|20...
+00001600: 1afc a76a 2bff 0700 00ff ff00 0000 ffff  ...j+...........
+00001610: b494 dd4e 8340 1484 5f85 f000 c22e 2d94  ...N.@.._.....-.
+00001620: 8692 58a9 a5ff 3f6f 4090 582f 6c4d 17ab  ..X...?o@.X/lM..
+00001630: bebd 8794 083b 995b b981 2c1f 3387 b373  .....;.[..,.3..s
+00001640: 3631 a7aa aab3 a22e d2e4 7af9 72ae 1357  61........z.r..W
+00001650: b98e f928 ce46 9ec6 6ae4 3aa7 7ae2 6aff  ...(.F..j.:.z.j.
+00001660: 41f9 fd4b a0f2 d3d4 97f7 bc7a 7b6d 0859  A..K.......z{m.Y
+00001670: f856 83a2 1cbf fc64 9529 abb3 acc9 4743  .V.....d.)....GC
+00001680: 374d ca46 f5b1 9115 21b9 c91b 23cb b754  7M.F....!...#..T
+00001690: f983 c4bb a589 57b6 d094 4123 9b79 a242  ......W...A#.y.B
+000016a0: 431b ca28 14da d08c bac5 36f4 4c21 a869  C..(......6.L!.i
+000016b0: cea0 d8b7 9572 aa14 d9d0 8216 0ed0 9242  .....r.........B
+000016c0: 50d3 8a40 81b6 ddd6 5408 3ab0 2150 0866  P..@....T.:.!P.f
+000016d0: 5bc2 44c0 ec98 9982 26ed 29a4 ecb2 0fb4  [.D.....&.).....
+000016e0: dd90 a523 85ba 9c78 12f7 bfcc ebff c97c  ...#...x.......|
+000016f0: 232b a311 f633 af60 0fa6 2d14 5950 00a1  #+...3.`..-.YP..
+00001700: a710 fc71 4621 988c 1981 02cc 7ccb c8f0  ...qF!......|...
+00001710: 77b3 aa60 7ae6 d40d 929a b750 6c29 4130  w..`z......Pl)A0
+00001720: 1654 096a 5a32 4843 7a56 7748 fb7d 3b0d  .T.jZ2HCzVwH.};.
+00001730: e959 1328 0266 4398 102a dad2 8a60 7777  .Y.(.fC..*...`ww
+00001740: 1482 dddd 1328 824e 1e98 500c 6e47 0a75  .....(.N..P.nG.u
+00001750: 6ef7 cc7b dd99 ff0b 0000 ffff 0000 00ff  n..{............
+00001760: ff34 cc4d 0ac2 3010 c5f1 ab84 3980 1544  .4.M..0.....9..D
+00001770: dc34 ddb8 7221 7885 6827 1fa8 f3c2 64a8  .4..r!x.h'....d.
+00001780: 787b 5b21 bbf7 7b8b ff58 3384 ad3c 6eea  x{[!..{..X3..<n.
+00001790: 22c4 2eb3 a703 39fb 56f6 2438 4316 d656  ".....9.V.$8C..V
+000017a0: 2034 4c63 0d89 af41 5391 e65e 1ccd d37e   4Lc...AS..^...~
+000017b0: 7722 a725 e5be 0df5 ff1e c9dd 6186 7757  w".%........a.wW
+000017c0: e630 b36e 5af3 11b0 8eb5 3b7c a0cf 9699  .0.nZ.....;|....
+000017d0: 6dfa 0100 00ff ff03 0050 4b03 0414 0006  m........PK.....
+000017e0: 0008 0000 0021 004d 3d34 677d 0300 00a9  .....!.M=4g}....
+000017f0: 0900 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
+00001800: 6565 7473 2f73 6865 6574 332e 786d 6c9c  eets/sheet3.xml.
+00001810: 934d 8f9b 3010 86ef 95fa 1f2c df83 8124  .M..0......,...$
+00001820: 348b 4256 5556 abee 6555 f5f3 ec98 2158  4.BVUV..eU....!X
+00001830: b131 b59d af56 fdef 1d43 4852 e512 2d02  .1...V...CHR..-.
+00001840: db30 f6f3 ce98 d7f3 c783 5664 07d6 49d3  .0........Vd..I.
+00001850: 1434 8962 4aa0 11a6 94cd baa0 dfbf 3d8f  .4.bJ.........=.
+00001860: 6694 38cf 9b92 2bd3 4041 8fe0 e8e3 e2fd  f.8...+.@A......
+00001870: bbf9 ded8 8dab 013c 4142 e30a 5a7b dfe6  .......<AB..Z{..
+00001880: 8c39 5183 e62e 322d 3418 a98c d5dc e3ab  .9Q...2-4.......
+00001890: 5d33 d75a e065 b748 2b96 c671 c634 970d  ]3.Z.e.H+..q.4..
+000018a0: ed09 b9bd 8761 aa4a 0a78 3262 aba1 f13d  .....a.J.x2b...=
+000018b0: c482 e21e f377 b56c dd40 d3e2 1e9c e676  .....w.l.@.....v
+000018c0: b36d 47c2 e816 112b a9a4 3f76 504a b4c8  .mG....+..?vPJ..
+000018d0: 5fd6 8db1 7ca5 b0ee 4332 e182 1c2c de29  _...|...C2...,.)
+000018e0: 3ee3 41a6 fb7e a3a4 a5b0 c699 ca47 4866  >.A..~.......GHf
+000018f0: 7dce b7e5 3fb0 07c6 c599 745b ff5d 9864  }...?.....t[.].d
+00001900: c22c ec64 f881 1754 fab6 9492 e999 955e  .,.d...T.......^
+00001910: 60e3 37c2 b233 2c6c 97cd b7b2 2ce8 9ff8  `.7..3,l....,...
+00001920: 748d b04f 4213 8f62 f442 371a 627f e962  t..OB..b.B7.b..b
+00001930: 5e4a fcc3 a12a 62a1 2ae8 c724 7f4d 295b  ^J...*b.*..$.M)[
+00001940: cc3b fffc 90b0 7757 63f2 db18 fd55 7005  .;....wWc....Up.
+00001950: afc1 700a ad1c a395 8349 57c6 6cc2 f417  ..p......IW.l...
+00001960: 148f 91eb 4081 0876 211c bb1d 2c41 e1f4  ....@..v!...,A..
+00001970: 6582 05bb 5f9d 5418 a310 3b2b 5d8f 07d5  e..._.T...;+]...
+00001980: e7ce d89f 2d29 a1e2 5be5 9746 fd94 a5af  ....-)..[..F....
+00001990: 8372 34fb 30a5 43e0 8bd9 7f02 b9ae 3d46  .r4.0.C.......=F
+000019a0: f030 7586 c9cb e313 3881 0ec6 9ca2 641a  .0u.....8.....d.
+000019b0: e484 51c8 c696 6819 8e22 3a90 1fba 7eff  ..Q...h..":...~.
+000019c0: 3fd7 f963 7064 8a09 8bad f346 0fba 274a  ?..cpd.....F..'J
+000019d0: bf1e a3fd fa09 6ec3 0990 4559 8a89 dd07  ......n...EY....
+000019e0: c0ac 4e84 6c3c bb82 9caa bb40 c256 75c9  ..N.l<.....@.Vu.
+000019f0: ff03 0000 ffff 0000 00ff ffb4 d4dd 6e82  ..............n.
+00001a00: 4010 05e0 5721 fb00 5d16 b055 b392 5451  @...W!..]..U..TQ
+00001a10: f18f 7720 eb46 7b51 6d5c 6adb b777 8844  ..w .F{Qm\j..w.D
+00001a20: 9cc9 b92d 3790 c9c7 243b 67c0 86a3 f74d  ...-7...$;g....M
+00001a30: 5137 756e 2fe7 9fe8 3251 4645 e1ab 3e05  Q7un/...2QFE..>.
+00001a40: 7a1a 9b4c 45c7 66a2 92f8 c5c4 cf17 21f7  z..LE.f.......!.
+00001a50: 1d9a f367 e93f 0ead a0c2 afc9 6a37 deff  ...g.?......j7..
+00001a60: 153e 387f a21a bd34 50b9 756d d7f7 b62d  .>8....4P.um...-
+00001a70: 3532 4a77 95e9 a312 910d 04af b949 32ab  52Jw.........I2.
+00001a80: afb9 d5ae 4333 8806 1c15 10bd 7234 87e8  ....C3......r4..
+00001a90: 8da3 0544 438e 9610 8d38 2a11 4a63 8e56  ...DC....8*.Jc.V
+00001aa0: 1019 8ed6 1025 1c6d 204a 39da 4224 26be  .....%.m J9.B$&.
+00001ab0: 8348 4cbc 82a8 9fb8 a65d 7a2c 54f2 3f0b  .HL......]z,T.?.
+00001ac0: d5b6 a585 a25b bf3e 468c 65da a1f4 19a5  .....[.>F.e.....
+00001ad0: 22f4 1944 22f4 0222 11fa 1ca1 4c84 be80  "..D".."....L...
+00001ae0: 4884 be84 489c ae84 4884 be82 4884 be86  H...H...H...H...
+00001af0: 4884 be81 487c 665b 88c4 c477 1089 8957  H...H|f[...w...W
+00001b00: 10f5 13bf ef98 ee7f 6037 0000 00ff ff00  ........`7......
+00001b10: 0000 ffff 34cc 4d0a c230 10c5 f1ab 8439  ....4.M..0.....9
+00001b20: 8015 44dc 34dd b872 2178 8568 271f a8f3  ..D.4..r!x.h'...
+00001b30: c264 a878 7b5b 21bb f77b 8bff 5833 84ad  .d.x{[!..{..X3..
+00001b40: 3c6e ea22 c42e b3a7 0339 fb56 f624 3843  <n.".....9.V.$8C
+00001b50: 16d6 5620 344c 630d 89af 4153 91e6 5e1c  ..V 4Lc...AS..^.
+00001b60: cdd3 7e77 22a7 25e5 be0d f5ff 1ec9 dd61  ..~w".%........a
+00001b70: 8677 57e6 30b3 6e5a f311 b08e b53b 7ca0  .wW.0.nZ.....;|.
+00001b80: cf96 996d fa01 0000 ffff 0300 504b 0304  ...m........PK..
+00001b90: 1400 0600 0800 0000 2100 c33a 3cca 6e03  ........!..:<.n.
+00001ba0: 0000 9309 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
+00001bb0: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
+00001bc0: 6d6c 9c93 4d8f db20 1086 ef95 f63f 20ee  ml..M.. .....? .
+00001bd0: 31b6 93b8 592b ce6a b5d1 aa7b a9aa 6adb  1...Y+.j...{..j.
+00001be0: 9e09 1ec7 2860 5cc0 f950 d5ff dec1 8993  ....(`\..P......
+00001bf0: 54b9 448b 6cc0 1ef1 cc3b f032 7fda 6b45  T.D.l....;.2..kE
+00001c00: b660 9d34 4d41 9328 a604 1a61 4ad9 ac0b  .`.4MA.(...aJ...
+00001c10: fae3 fd75 34a3 c479 de94 5c99 060a 7a00  ...u4..y..\...z.
+00001c20: 479f 160f 9fe6 3b63 37ae 06f0 0409 8d2b  G.....;c7......+
+00001c30: 68ed 7d9b 33e6 440d 9abb c8b4 d060 a432  h.}.3.D......`.2
+00001c40: 5673 8f9f 76cd 5c6b 8197 fd22 ad58 1ac7  Vs..v.\k...".X..
+00001c50: 19d3 5c36 f448 c8ed 3d0c 5355 52c0 d288  ..\6.H..=.SUR...
+00001c60: 4e43 e38f 100b 8a7b d4ef 6ad9 ba81 a6c5  NC.....{..j.....
+00001c70: 3d38 cded a66b 47c2 e816 112b a9a4 3ff4  =8...kG....+..?.
+00001c80: 504a b4c8 dfd6 8db1 7ca5 b0ee 7d32 e182  PJ......|...}2..
+00001c90: ec2d 3e29 bee3 214d ffff 2693 96c2 1a67  .->)..!M..&....g
+00001ca0: 2a1f 2199 1d35 df96 ffc8 1e19 1767 d26d  *.!..5.......g.m
+00001cb0: fd77 6192 09b3 b095 e100 2fa8 f463 9292  .wa......./..c..
+00001cc0: e999 955e 60e3 0fc2 b233 2c6c 97cd 3b59  ...^`....3,l..;Y
+00001cd0: 16f4 4f7c 6a23 1c93 d0c5 a378 1cba abf6  ..O|j#.....x....
+00001ce0: 972e e6a5 c413 0e55 110b 5541 9f93 fc6b  .......U..UA...k
+00001cf0: 4ad9 62de fbe7 a784 9dbb 9a93 60c7 9531  J.b.........`..1
+00001d00: 9b10 78c3 3431 121c 2810 c118 84e3 b085  ..x.41..(.......
+00001d10: 1750 aaa0 cb74 8296 fedd 43c3 1c91 eccc  .P...t....C.....
+00001d20: bc9e 0ffc d7de c2df 2c29 a1e2 9df2 2f46  ........,)..../F
+00001d30: fd92 a5af f1ba c4d1 ecf3 940e 81ef 66f7  ..............f.
+00001d40: 05e4 baf6 18c1 6bd3 5b23 2f0f 4b70 02bd  ......k.[#/.Kp..
+00001d50: 8a9a a264 1ad2 09a3 908d 3dd1 325c 3af4  ...d......=.2\:.
+00001d60: 1adf f7e3 ee7f aef3 87e0 bd14 cf42 74ce  .............Bt.
+00001d70: 1b3d e43d 518e eb31 7a5c 8f75 0d80 2cca  .=.=Q..1z\.u..,.
+00001d80: 5214 761f 0055 9d08 d978 7605 3955 7781  R.v..U...xv.9Uw.
+00001d90: 84ad eac5 ff03 0000 ffff 0000 00ff ffb4  ................
+00001da0: d4dd 6e82 4010 05e0 5721 fb00 5d16 b055  ..n.@...W!..]..U
+00001db0: b392 5451 f18f 7720 eb46 7b51 6d5c 6adb  ..TQ..w .F{Qm\j.
+00001dc0: b777 8844 9cc9 b92d 3790 c9c7 243b 67c0  .w.D...-7...$;g.
+00001dd0: 86a3 f74d 5137 756e 2fe7 9fe8 3251 4645  ...MQ7un/...2QFE
+00001de0: e1ab 3e05 7a1a 9b4c 45c7 66a2 92f8 c5c4  ..>.z..LE.f.....
+00001df0: cf17 21f7 1d9a f367 e93f 0ead a0c2 afc9  ..!....g.?......
+00001e00: 6a37 deff 153e 387f a21a bd34 50b9 756d  j7...>8....4P.um
+00001e10: d7f7 b62d 3532 4a77 95e9 a312 910d 04af  ...-52Jw........
+00001e20: b949 32ab afb9 d5ae 4333 8806 1c15 10bd  .I2.....C3......
+00001e30: 7234 87e8 8da3 0544 438e 9610 8d38 2a11  r4.....DC....8*.
+00001e40: 4a63 8e56 1019 8ed6 1025 1c6d 204a 39da  Jc.V.....%.m J9.
+00001e50: 4224 26be 8348 4cbc 82a8 9fb8 a65d 7a2c  B$&..HL......]z,
+00001e60: 54f2 3f0b d5b6 a585 a25b bf3e 468c 65da  T.?......[.>F.e.
+00001e70: a1f4 19a5 22f4 1944 22f4 0222 11fa 1ca1  ...."..D".."....
+00001e80: 4c84 be80 4884 be84 489c ae84 4884 be82  L...H...H...H...
+00001e90: 4884 be86 4884 be81 487c 665b 88c4 c477  H...H...H|f[...w
+00001ea0: 1089 8957 10f5 13bf ef98 ee7f 6037 0000  ...W........`7..
+00001eb0: 00ff ff00 0000 ffff 34cc 4d0a c230 10c5  ........4.M..0..
+00001ec0: f1ab 8439 8015 44dc 34dd b872 2178 8568  ...9..D.4..r!x.h
+00001ed0: 271f a8f3 c264 a878 7b5b 21bb f77b 8bff  '....d.x{[!..{..
+00001ee0: 5833 84ad 3c6e ea22 c42e b3a7 0339 fb56  X3..<n.".....9.V
+00001ef0: f624 3843 16d6 5620 344c 630d 89af 4153  .$8C..V 4Lc...AS
+00001f00: 91e6 5e1c cdd3 7e77 22a7 25e5 be0d f5ff  ..^...~w".%.....
+00001f10: 1ec9 dd61 8677 57e6 30b3 6e5a f311 b08e  ...a.wW.0.nZ....
+00001f20: b53b 7ca0 cf96 996d fa01 0000 ffff 0300  .;|....m........
+00001f30: 504b 0304 1400 0600 0800 0000 2100 f7b3  PK..........!...
+00001f40: 830c 2403 0000 d507 0000 1800 0000 786c  ..$...........xl
+00001f50: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00001f60: 7435 2e78 6d6c 9c93 cb8e db20 1486 f795  t5.xml..... ....
+00001f70: e61d 10fb 18e3 5c34 b1e2 8c46 198d 9a5d  ......\4...F...]
+00001f80: 55b5 d335 c1c7 310a 1817 c84d 55df bd07  U..5..1....MU...
+00001f90: 3b37 299b 7410 060c 3adf b9f0 337b 3918  ;7).t...:...3{9.
+00001fa0: 4d76 e0bc b24d 4179 9252 028d b4a5 6ad6  Mv...MAy.R....j.
+00001fb0: 05fd f9e3 7df0 4c89 0fa2 2985 b60d 14f4  ....}.L...).....
+00001fc0: 089e becc 9fbe ccf6 d66d 7c0d 1008 121a  .........m|.....
+00001fd0: 5fd0 3a84 3667 cccb 1a8c f089 6da1 c193  _.:.6g......m...
+00001fe0: ca3a 2302 feba 35f3 ad03 5176 4646 b32c  .:#...5...QvFF.,
+00001ff0: 4d27 cc08 d5d0 9e90 bb47 18b6 aa94 8437  M'.......G.....7
+00002000: 2bb7 069a d043 1c68 1130 7e5f abd6 9f69  +....C.h.0~_...i
+00002010: 463e 8233 c26d b6ed 405a d322 62a5 b40a  F>.3.m..@Z."b...
+00002020: c70e 4a89 91f9 72dd 5827 561a f33e f091  ..J...r.X'V..>..
+00002030: 90e4 e0b0 67f8 0dcf 6eba fd3b 4f46 4967  ....g...n..;OFIg
+00002040: bdad 4282 64d6 c77c 9ffe 944d 9990 17d2  ..B.d..|...M....
+00002050: 7dfe 0f61 f888 39d8 a978 8157 54f6 b990  }..a..9..x.WT...
+00002060: f8f8 c2ca aeb0 e127 6193 0b2c 96cb e55b  .......'a..,...[
+00002070: 5516 f44f 7a6a 039c 791c d241 3a8a c34d  U..Ozj..y..A:..M
+00002080: fb4b e7b3 52e1 0dc7 ac88 83aa a0af 3c5f  .K..R.........<_
+00002090: 6694 cd67 9d7e 3e14 ecfd cd9a 4439 aeac  f..g.~>.....D9..
+000020a0: ddc4 8325 ba49 91e0 4183 8cc2 2002 a71d  ...%.I..A... ...
+000020b0: 2c40 eb82 2ea2 a27f 774c 5c22 905d 88b7  ,@......wL\".]..
+000020c0: eb33 fdbd 13f0 3747 4aa8 c456 8785 d5bf  .3....7GJ..V....
+000020d0: 5419 ea82 4e93 6c4c cfdb dfed fe2b a875  T...N.lL.....+.u
+000020e0: 1df0 11a1 834e 1679 797c 032f 51a7 184f  .....N.yy|./Q..O
+000020f0: c2c7 d199 b41a c938 12a3 e283 439d 8943  .......8....C..C
+00002100: 41b1 dafb 9eca 47c9 2472 7d38 46dd 6578  A.....G.$r}8F.ex
+00002110: 22b7 3e58 73f2 ca4f 94de 1e0b dbd9 4faf  ".>Xs..O......O.
+00002120: f6e9 ffd8 737c ef1d 804f 86cf a30b a44f  ....s|...O.....O
+00002130: ed1a 42ac 5217 f93f 0000 00ff ff00 0000  ..B.R..?........
+00002140: ffff 94d3 dd0e 8220 14c0 f157 713c 408a  ....... ...Wq<@.
+00002150: 8aa5 43b6 f2fb 3198 b975 654d 9cd5 db87  ..C...1..ueM....
+00002160: 8b69 e7ec dc74 0583 df05 f01f d2dc 8661  .i...t.........a
+00002170: 2ef5 ac95 9cee 4f6f ca19 679e 79e8 d1d8  ......Oo..g.y...
+00002180: 5996 32ef c563 dd67 d777 3998 7e18 e79c  Y.2..c.g.w9.~...
+00002190: 0507 2e98 92fd 6acf 2bce 5968 07bb 63ec  ......j.+.Yh..c.
+000021a0: f2a2 b808 a4bf 28e9 f70e 5d48 c421 2a48  ......(...]H.!*H
+000021b0: 1442 5492 2882 a822 510c 51ed 5002 0e2e  .BT.(.."Q.Q.P...
+000021c0: 206a 4894 40d4 92e8 0851 479e e9b4 21df   jH.@....QG...!.
+000021d0: befd 1620 fc27 c08a 6d80 18dc 2345 011c  ... .'..m...#E..
+000021e0: 12bf 2841 950a 8722 8050 a592 44a8 5245  ..(A...".P..D.RE
+000021f0: 2254 a926 11aa d490 0855 6a49 842a 7524  "T.&.....UjI.*u$
+00002200: da2b 7d03 f8fb 6ff8 0000 00ff ff00 0000  .+}...o.........
+00002210: ffff 3c8c 4b0a c240 1005 af32 f401 8c22  ..<.K..@...2..."
+00002220: 924d 261b 572e 845c 614c 7a3e a8fd 869e  .M&.W..\aLz>....
+00002230: 46f1 f646 4177 5550 d450 3384 adcc 93ba  F..FAwUP.P3.....
+00002240: 08b1 d3e2 694f ce5e 953d 098e 9007 6b2b  ....iO.^.=....k+
+00002250: 10ea c6a1 86c4 e7a0 a948 7337 8ee6 69bb  .........Hs7..i.
+00002260: e90f e4b4 a4fc 1743 f5b4 2377 8119 ee5f  .......C..#w..._
+00002270: cc1c 16d6 4fbd c611 b09f accf ee09 bdb6  ....O...........
+00002280: cc6c e31b 0000 ffff 0300 504b 0304 1400  .l........PK....
+00002290: 0600 0800 0000 2100 0031 94de e503 0000  ......!..1......
+000022a0: 3b0b 0000 1800 0000 786c 2f77 6f72 6b73  ;.......xl/works
+000022b0: 6865 6574 732f 7368 6565 7436 2e78 6d6c  heets/sheet6.xml
+000022c0: 9c94 db8e da30 1086 ef2b f51d 22df 9313  .....0...+.."...
+000022d0: 2104 04ac 2814 756f aa55 8fd7 c631 6061  !...(.uo.U...1`a
+000022e0: c7d4 360b 74d5 77ef d8c1 0189 aa0a 4880  ..6.t.w.......H.
+000022f0: 079c f9fe 99f1 6f46 4f47 c183 57aa 3493  ......oFOG..W.4.
+00002300: d518 2561 8c02 5a11 59b2 6a3d 46df bf2d  ..%a..Z.Y.j=F..-
+00002310: 3a05 0ab4 c155 89b9 ace8 189d a846 4f93  :....U.......FO.
+00002320: f7ef 4607 a9b6 7a43 a909 8050 e931 da18  ..F...zC...P.1..
+00002330: b31b 4691 261b 2ab0 0ee5 8e56 b0b3 924a  ..F.&.*....V...J
+00002340: 6003 5fd5 3ad2 3b45 71e9 9204 8fd2 38ce  `._.:.;Eq.....8.
+00002350: 2381 5985 6ac2 50b5 61c8 d58a 113a 9764  #.Y.j.P.a....:.d
+00002360: 2f68 656a 88a2 1c1b a85f 6fd8 4e7b 9a20  /hej....._o.N{. 
+00002370: 6d70 02ab ed7e d721 52ec 00b1 649c 9993  mp...~.!R...d...
+00002380: 83a2 4090 e1f3 ba92 0a2f 39f4 7d4c 324c  ..@....../9.}L2L
+00002390: 82a3 8257 0aef ae97 71bf df28 0946 94d4  ...W....q..(.F..
+000023a0: 7265 4220 4775 cdb7 ed0f a241 8449 43ba  reB Gu.....A.IC.
+000023b0: edbf 1526 c922 455f 993d c00b 2a7d aca4  ...&."E_.=..*}..
+000023c0: a4d7 b0d2 0bac fb20 2c6f 6076 5c6a b867  ....... ,o`v\j.g
+000023d0: e518 bd2d 8a6c 96e4 d9b4 d39f 1759 279b  ...-.l.......Y'.
+000023e0: 76d3 4e51 6471 a7ff 713e 4db3 593c 4d3f  v.NQdq..q>M.Y<M?
+000023f0: e47f d064 5432 3861 db55 a0e8 6a8c a6c9  ...dT28a.U..j...
+00002400: f025 45d1 64e4 fcf3 83d1 83be 8a83 df52  .%E.d..........R
+00002410: 8aaf 0473 fad9 1a8e 8395 63b0 b235 e952  ...s......c..5.R
+00002420: caad 7dfc 19c4 63e0 6aca 29b1 7609 302c  ..}...c.j.).v.0,
+00002430: af74 4639 3cbe c8c1 e7bf 9c12 8420 1335  .tF9<........ .5
+00002440: 3ad7 b1d7 5c38 5bbf a8a0 a42b bce7 6626  :...\8[....+..f&
+00002450: f94f 569a 8dd5 0d8b 7e0f f98d 2ff2 f089  .OV.....~.../...
+00002460: b2f5 c6c0 4e11 da0d e798 6179 9a53 4dc0  ....N.....ay.SM.
+00002470: c250 5498 f4ac 2291 1cf0 f019 0866 ef22  .PT..."......f."
+00002480: 5810 1fdd 7aa8 d169 1ce6 2910 b439 594b  X...z..i..)..9YK
+00002490: c209 91bd 3652 78e5 33a4 4e87 5d97 0ecf  ....6Rx.3.N.]...
+000024a0: fbf4 ec8e 7418 874b 87f5 dfe9 49ff bff2  ....t..K....I...
+000024b0: b0eb f261 7d44 1efe 755c 3aac 0fc9 0ffc  ...a}D..u\:.....
+000024c0: f0ac 09ce d3bb a7fd a499 3e04 6740 9285  ..........>.g@..
+000024d0: 5d7b 80ad c69f f8f9 dbc0 03f2 da1a ed00  ]{..............
+000024e0: 7067 eaf3 87e0 0268 ad9f f974 08fc 04a0  pg.....h...t....
+000024f0: 9776 daa0 526b 5fb9 27bd a77b 6f9f 24ef  .v..Rk_.'..{o.$.
+00002500: 1697 02fc dd68 8ab0 f7cc d9fe 2f00 0000  .....h....../...
+00002510: ffff 0000 00ff ffb4 94d1 8e82 3010 457f  ............0.E.
+00002520: 85f4 032c 4505 3595 4445 4557 5d7f 81d4  ...,E.5.DEEW]...
+00002530: 467d 5037 9655 f7ef 7758 119c 615e 9717  F}P7.U..wX..a^..
+00002540: c8e5 f4a6 e919 d0ee 606d 9e64 7916 ebeb  ........`m.dy...
+00002550: e5ee 5d87 4209 cf7d 6567 074f 0315 0aef  ..].B..}eg.O....
+00002560: 900f 45e0 b794 ff7e 0164 be5d 7e39 a5f6  ..E....~.d.]~9..
+00002570: b82f 0808 1eaa 9399 c1ee 27b1 ced8 3364  ./........'...3d
+00002580: b0a8 2b62 6d8a d651 510b 4570 8337 0ee2  ..+bm..QQ.Ep.7..
+00002590: 5bac c29e 96b7 584b 5342 6316 ea63 68c2  [.....XKSBc..ch.
+000025a0: 4191 8fa1 8485 1486 a62c 1460 6856 4270  A........,.`hVBp
+000025b0: 12f5 c6a3 3686 e66c 5307 4329 d7d4 277b  ....6..lS.C)..'{
+000025c0: 5ab0 4d5d dcb4 64a1 b082 24a8 ac7c 06ff  Z.M]..d...$..|..
+000025d0: e3b3 a805 edf8 5822 e2b3 8422 7476 44fa  ......X"..."tvD.
+000025e0: 8485 88f4 8483 7a44 fa94 85ea 63f9 1bc4  ......zD....c...
+000025f0: 190b 1155 7316 22aa 5216 22aa 162c 4466  ...Us.".R."..,Df
+00002600: 6cc9 4264 c63e 9e50 e00b 597e 2eab 46b2  l.Bd.>.P..Y~..F.
+00002610: 6e24 9baa fab5 eab3 916c df93 e7ec c8fa  n$.......l......
+00002620: bff0 0b00 00ff ff00 0000 ffff 34cd c10a  ............4...
+00002630: c230 1004 d05f 09fb 0156 14e9 a5e9 c593  .0..._...V......
+00002640: 07a1 bf10 db6d 12d4 9db0 5914 ffde 2ae4  .....m....Y...*.
+00002650: 366f 0e33 4349 10b6 3c4f ea56 885d 164f  6o.3CI..<O.V.].O
+00002660: 0772 f629 ec49 7086 bc58 6b86 5037 0e25  .r.).Ip..Xk.P7.%
+00002670: 44be 068d 59aa 7bf0 6a9e f6bb 9e9c e698  D...Y.{.j.......
+00002680: 5a36 947f 7b22 7783 199e 4d89 c3c2 fad3  Z6..{"w...M.....
+00002690: 91b6 2758 c3b6 dbbd a1f7 9a98 6dfc 0200  ..'X........m...
+000026a0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000026b0: 0021 00e9 a625 b866 0600 0053 1b00 0013  .!...%.f...S....
+000026c0: 0000 0078 6c2f 7468 656d 652f 7468 656d  ...xl/theme/them
+000026d0: 6531 2e78 6d6c ec59 cd6e 1b37 10be 17e8  e1.xml.Y.n.7....
+000026e0: 3b10 7b4f 2cd9 9262 1991 034b 96e2 3671  ;.{O,..b...K..6q
+000026f0: 62d8 4a8a 1ca9 5d6a 9711 77b9 2029 3bba  b.J...]j..w. );.
+00002700: 15c9 b140 81a2 69d1 4b81 de7a 28da 0648  ...@..i.K..z(..H
+00002710: 805e d2a7 719b a24d 81bc 4287 e44a 5a5a  .^..q..M..B..JZZ
+00002720: 546c 2706 fa17 1d6c 2df7 e3fc cf70 86ba  Tl'....l-....p..
+00002730: 7aed 41ca d021 1192 f2ac 1554 2f57 0244  z.A..!.....T/W.D
+00002740: b290 4734 8b5b c19d 7eef d27a 80a4 c259  ..G4.[..~..z...Y
+00002750: 8419 cf48 2b98 1019 5cdb 7cff bdab 7843  ...H+...\.|...xC
+00002760: 2524 2508 f667 7203 b782 44a9 7c63 6545  %$%..gr...D.|ceE
+00002770: 86b0 8ce5 659e 930c de0d b948 b182 4711  ....e......H..G.
+00002780: af44 021f 01dd 94ad ac56 2a8d 9514 d32c  .D.......V*....,
+00002790: 4019 4e81 eced e190 8604 f535 c960 734a  @.N........5.`sJ
+000027a0: bccb e031 5352 2f84 4c1c 68d2 c4d9 61b0  ...1SR/.L.h...a.
+000027b0: d1a8 aa11 7222 3b4c a043 cc5a 01f0 89f8  ....r";L.C.Z....
+000027c0: 519f 3c50 0162 582a 78d1 0a2a e613 ac6c  Q.<P.bX*x..*...l
+000027d0: 5e5d c11b c526 a696 ec2d edeb 994f b1af  ^]...&...-...O..
+000027e0: d810 8d56 0d4f 110f 664c abbd 5af3 caf6  ...V.O..fL..Z...
+000027f0: 8cbe 0130 b588 eb76 bb9d 6e75 46cf 0070  ...0...v..nuF..p
+00002800: 1882 a656 9632 cd5a 6fbd da9e d22c 81ec  ...V.2.Zo....,..
+00002810: d745 da9d 4abd 5273 f125 fa6b 0b32 37db  .E..J.Rs.%.k.27.
+00002820: ed76 bd59 c862 891a 90fd 5a5b c0af 571a  .v.Y.b....Z[..W.
+00002830: b5ad 5507 6f40 165f 5fc0 d7da 5b9d 4ec3  ..U.o@.__...[.N.
+00002840: c11b 90c5 3716 f0bd 2bcd 46cd c51b 50c2  ....7...+.F...P.
+00002850: 6836 5a40 6b87 f67a 05f5 1964 c8d9 8e17  h6Z@k..z...d....
+00002860: be0e f0f5 4a01 9fa3 201a 66d1 a559 0c79  ....J... .f..Y.y
+00002870: a696 c55a 8aef 73d1 0380 0632 ac68 86d4  ...Z..s....2.h..
+00002880: 2427 431c 4214 7770 3a10 146b 0678 83e0  $'C.B.wp:..k.x..
+00002890: d21b bb14 ca85 25cd 0bc9 50d0 5cb5 820f  ......%...P.\...
+000028a0: 730c 1931 a7f7 eaf9 f7af 9e3f 45af 9e3f  s..1.......?E..?
+000028b0: 397e f8ec f8e1 4fc7 8f1e 1d3f fcd1 d272  9~....O....?...r
+000028c0: 36ee e02c 2e6f 7cf9 ed67 7f7e fd31 fae3  6..,.o|..g.~.1..
+000028d0: e937 2f1f 7fe1 c7cb 32fe d71f 3ef9 e5e7  .7/.....2...>...
+000028e0: cffd 40c8 a0b9 442f be7c f2db b327 2fbe  ..@...D/.|...'/.
+000028f0: faf4 f7ef 1e7b e05b 020f caf0 3e4d 8944  .....{.[....>M.D
+00002900: b7c8 11da e729 e866 0ce3 4a4e 06e2 7c3b  .....).f..JN..|;
+00002910: fa09 a6ce 0e9c 006d 0fe9 ae4a 1ce0 ad09  .......m...J....
+00002920: 663e 5c9b b8c6 bb2b a078 f880 d7c7 f71d  f>\....+.x......
+00002930: 590f 1231 56d4 c3f9 4692 3ac0 5dce 599b  Y..1V...F.:.].Y.
+00002940: 0baf 016e 685e 250b f7c7 59ec 672e c665  ...nh^%...Y.g..e
+00002950: dc3e c687 3ede 1d9c 39ae ed8e 73a8 9ad3  .>..>...9...s...
+00002960: a074 6cdf 4988 23e6 1ec3 99c2 31c9 8842  .tl.I.#.....1..B
+00002970: fa1d 1f11 e2d1 ee1e a58e 5d77 6928 b8e4  ..........]wi(..
+00002980: 4385 ee51 d4c6 d46b 923e 1d38 8134 dfb4  C..Q...k.>.8.4..
+00002990: 4353 f0cb c4a7 33b8 dab1 cdee 5dd4 e6cc  CS....3.....]...
+000029a0: a7f5 3639 7491 9010 9879 84ef 13e6 98f1  ..69t....y......
+000029b0: 3a1e 2b9c fa48 f671 caca 06bf 8955 e213  :.+..H.q.....U..
+000029c0: f260 22c2 32ae 2b15 783a 268c a36e 44a4  .`".2.+.x:&..nD.
+000029d0: f4ed b92d 40df 92d3 6f60 a857 5eb7 efb2  ...-@...o`.W^...
+000029e0: 49ea 2285 a223 1fcd 9b98 f332 729b 8f3a  I."..#.....2r..:
+000029f0: 094e 73af cc34 4bca d80f e408 4214 a33d  .Ns..4K.....B..=
+00002a00: ae7c f05d ee66 887e 063f e06c a9bb ef52  .|.].f.~.?.l...R
+00002a10: e2b8 fbf4 4270 87c6 8e48 f300 d16f c6a2  ....Bp...H...o..
+00002a20: a8da 4efd 4d69 f6ba 62cc 2854 e377 c578  ..N.Mi..b.(T.w.x
+00002a30: 7a3a 6dc1 d1e4 4b89 9d13 2578 19ee 5f58  z:m...K...%x.._X
+00002a40: 78b7 f138 db23 10eb 8b07 cfbb bafb aeee  x..8.#..........
+00002a50: 06ff f9ba bb2c 97cf 5a6d e705 169a e479  .....,..Zm.....y
+00002a60: 5f6c bae4 7469 933c a48c 1da8 0923 37a5  _l..ti.<.....#7.
+00002a70: e993 251c 1651 0f16 4d03 6fa6 b8d9 d094  ..%..Q..M.o.....
+00002a80: 27f0 b528 ee0e 2e16 d8ec 4182 ab8f a84a  '..(......A....J
+00002a90: 0e12 9c43 8f5d 3523 5f2c 0bd2 b144 3997  ...C.]5#_,...D9.
+00002aa0: 30db 9965 337c 9213 b4cd 3849 a1cd 3693  0..e3|....8I..6.
+00002ab0: 615d cf0c b61e 48ac 7679 6497 d7ca b3e1  a]....H.vyd.....
+00002ac0: 8c8c 9914 6333 7f4e 19ad 6902 6765 b676  ....c3.N..i.ge.v
+00002ad0: e5ed 9855 ad54 4bcd e6aa 5635 a299 52e7  ...U.TK...V5..R.
+00002ae0: a836 5319 7cb8 a81a 2cce ac09 5d08 82de  .6S.|...,...]...
+00002af0: 05ac dc80 115d cb0e b309 6624 d276 b773  .....]....f$.v.s
+00002b00: f3d4 2d9a f585 ba48 2638 2285 8fb4 de8b  ..-....H&8".....
+00002b10: 3eaa 1a27 4d63 651a 461e 1fe9 39ef 141f  >..'Mce.F...9...
+00002b20: 95b8 3535 d9b7 e076 1627 95d9 d596 b09b  ..55...v.'......
+00002b30: 7aef 6dbc 341d 6ee7 5ed2 797b 221d 5956  z.m.4.n.^.y{".YV
+00002b40: 4e4e 96a1 a356 d0ac afd6 0314 e2bc 150c  NN...V..........
+00002b50: 61ac 85af 690e 5e97 baf1 c32c 86bb a150  a...i.^....,...P
+00002b60: 091b f6a7 26b3 09d7 b937 9bfe b0ac c24d  ....&....7.....M
+00002b70: 85b5 fb82 c24e 1dc8 8554 db58 2636 34cc  .....N...T.X&64.
+00002b80: ab22 0458 6686 7023 ff6a 1dcc 7a51 0ad8  .".Xf.p#.j..zQ..
+00002b90: 487f 0329 d6d6 2118 fe36 29c0 8eae 6bc9  H..)..!..6)...k.
+00002ba0: 7048 4255 7676 69c5 dc51 1840 514a f958  pHBUvvi..Q.@QJ.X
+00002bb0: 1171 9044 4768 c0c6 621f 83fb 75a8 823e  .q.DGh..b...u..>
+00002bc0: 1195 703b 612a 827e 80ab 346d 6df3 ca2d  ..p;a*.~..4mm..-
+00002bd0: ce45 d295 2fb0 0cce ae63 9627 b828 b73a  .E../....c.'.(.:
+00002be0: 45a7 996c e126 8f67 3298 272b ad11 0f74  E..l.&.g2.'+...t
+00002bf0: f3ca 6e94 3bbf 2a26 e52f 4895 7218 ffcf  ..n.;.*&./H.r...
+00002c00: 54d1 e709 5c17 ac45 da03 21dc e40a 8c74  T...\..E..!....t
+00002c10: beb6 022e 54c2 a10a e509 0d7b 022e b94c  ....T......{...L
+00002c20: ed80 6881 eb58 780d 4105 f7c9 e6bf 2087  ..h..Xx.A..... .
+00002c30: fabf cd39 4bc3 a435 4c7d 6a9f c648 5038  ...9K..5L}j..HP8
+00002c40: 8f54 2208 d983 b264 a2ef 1462 d5e2 ecb2  .T"....d...b....
+00002c50: 2459 41c8 4454 495c 995b b107 e490 b0be  $YA.DTI\.[......
+00002c60: ae81 0d7d b607 2881 5037 d5a4 2803 0677  ...}..(.P7..(..w
+00002c70: 32fe dce7 2283 06b1 6e72 fea9 9d8f 4de6  2..."...nr....M.
+00002c80: f3b6 07ba 3bb0 2d96 dd7f c65e a456 2afa  ....;.-....^.V*.
+00002c90: a5a3 a0e9 3dfb 4c4f 352b 07af 39d8 cf79  ....=.LO5+..9..y
+00002ca0: d4da 8ab5 a0f1 6afd cc47 6d0e 973e 48ff  ......j..Gm..>H.
+00002cb0: 81f3 8f8a 90d9 1f27 f481 dae7 fb50 5b11  .......'.....P[.
+00002cc0: fcd6 60db 2b04 517d c936 1e48 1748 5b1e  ..`.+.Q}.6.H.H[.
+00002cd0: 07d0 38d9 451b 4c9a 946d 588a eef6 c2db  ..8.E.L..mX.....
+00002ce0: 28b8 912e 3add 195f c8d2 37e9 74cf 69ec  (...:.._..7.t.i.
+00002cf0: 5973 e6b2 7372 f1f5 dde7 f98c 5d58 d8b1  Ys..sr......]X..
+00002d00: 75b9 d3f5 981a 92f6 648a eaf6 683a c818  u.......d...h:..
+00002d10: c798 5fb5 ca3f 3cf1 c17d 70f4 365c f18f  .._..?<..}p.6\..
+00002d20: 9992 f66a ff01 5cf1 c194 617f 2480 e4b7  ...j..\...a.$...
+00002d30: ce35 5b37 ff02 0000 ffff 0300 504b 0304  .5[7........PK..
+00002d40: 1400 0600 0800 0000 2100 209e 4fe6 fa05  ........!. .O...
+00002d50: 0000 ca21 0000 0d00 0000 786c 2f73 7479  ...!......xl/sty
+00002d60: 6c65 732e 786d 6cd4 5acd 6ee3 3610 be17  les.xml.Z.n.6...
+00002d70: e83b 083a 750f 8efe 65cb 6b7b bb4e 2260  .;.:u...e.k{.N"`
+00002d80: 816d 5134 2950 a05b 2c64 89b6 8948 a241  .mQ4)P.[,d...H.A
+00002d90: d159 7b17 7beb a5e8 b10f d153 7b5e 1428  .Y{.{......S{^.(
+00002da0: fa32 5d6c 1fa3 43d2 b2e8 f837 8e93 b806  .2]l..C....7....
+00002db0: 9288 1439 f3f1 9be1 703c 4ceb d924 4bb5  ...9....p<L..$K.
+00002dc0: 6b44 0b4c f2b6 6e9d 98ba 86f2 9824 381f  kD.L..n......$8.
+00002dd0: b4f5 ef2e c35a 43d7 0a16 e549 9492 1cb5  .....ZC....I....
+00002de0: f529 2af4 679d cf3f 6b15 6c9a a28b 2142  .)*.g..?k.l...!B
+00002df0: 4c03 1179 d1d6 878c 8d9a 8651 c443 9445  L..y.......Q.C.E
+00002e00: c509 19a1 1cde f409 cd22 064d 3a30 8a11  .........".M:0..
+00002e10: 4551 52f0 4959 6ad8 a6e9 1b59 8473 5d4a  EQR.IYj....Y.s]J
+00002e20: 6866 f12e 42b2 885e 8d47 b598 64a3 88e1  hf..B..^.G..d...
+00002e30: 1e4e 319b 0a59 ba96 c5cd 1783 9cd0 a897  .N1..Y..........
+00002e40: 02d4 89e5 46b1 36b1 7c6a 6b13 5a2a 11bd  ....F.6.|jk.Z*..
+00002e50: 4b7a 321c 5352 903e 3b01 b906 e9f7 718c  Kz2.SR.>;.....q.
+00002e60: 96e1 0646 6044 7125 0924 ef27 c9f2 0cd3  ...F`Dq%.$.'....
+00002e70: 5e58 fb84 ee29 c935 28ba c6dc 7c7a a795  ^X...).5(...|z..
+00002e80: 8fb3 3063 8516 9371 ceda ba37 efd2 e49b  ..0c...q...7....
+00002e90: 1709 d8b8 eeeb 9ab4 ca29 49b8 49e1 6364  .........)I.I.cd
+00002ea0: 46f2 f44b dd28 452c 8caf 2f8e 374f 4cd3  F..K.(E,../.7OL.
+00002eb0: 7cad ad19 0cfe a20a e783 d78e 0d6e 8c7d  |............n.}
+00002ec0: fde4 e90f dfa2 e4c7 575f 98af 9eac 96df  ........W_......
+00002ed0: 0007 5d90 2f85 1bb3 9577 5a7d 9257 0400  ..]./....wZ}.W..
+00002ee0: 7261 efe6 554e dee4 217f 0504 002b 7c54  ra..UN..!....+|T
+00002ef0: a755 bcd5 aea3 147a 2cae 2c26 29a1 1a03  .U.....z,.,&)...
+00002f00: ef05 5244 4f1e 6548 8ef8 f8c7 2fff fcf5  ..RDO.eH..../...
+00002f10: ab18 358c 6801 4e2f 273a 2eef 132e 3f1b  ..5.h.N/':....?.
+00002f20: 9961 7040 de69 481d 3734 d995 263a e8b5  .ap@.iH.74..&:..
+00002f30: f530 0432 e123 563b 57f7 9ce2 28e5 5dfd  .0.2.#V;W...(.].
+00002f40: 28c3 e954 2a13 5357 4a0d 1667 1f0a ec5a  (..T*.SWJ..g...Z
+00002f50: b12a 2ae7 00a4 0812 37d1 ffe9 f79f 3ffd  .**.....7.....?.
+00002f60: f9f7 4d42 d6aa 5e4d fd56 2d15 6ff7 bfc0  ..MB..^M.V-.o...
+00002f70: 1b06 df6f 8162 9d05 7809 4ed3 f9a6 af73  ...o.b..x.N....s
+00002f80: f786 8e4e 0be2 2343 340f a1a1 cd9e 2fa7  ...N..#C4...../.
+00002f90: 2370 ee1c 42b9 7451 316e cbe8 018d a696  #p..B.tQ1n......
+00002fa0: eded 3ea1 2029 4e38 8ac1 a9ba a504 ffbd  ..>. )N8........
+00002fb0: 591f ce13 3441 108e 7cd1 6d28 58f9 d6d9  Y...4A..|.m(X...
+00002fc0: 05d7 1a35 82d9 fb57 e3ea 1ac3 3cc8 d6cc  ...5...W....<...
+00002fd0: 13db 0d82 7add e29f 7a23 106e f980 00cc  ....z...z#.n....
+00002fe0: 937a 1004 1ee8 369d 86db 809f fb46 308b  .z....6......F0.
+00002ff0: 5ca1 f870 bfb8 cd6a 8571 c169 7b84 2690  \..p...j.q.i{.&.
+00003000: 7794 6755 031c 4676 755a 29ea 3390 4af1  w.gU..FvuZ).3.J.
+00003010: 60c8 ff32 32e2 3a08 6370 3677 5a09 8e06  `..22.:.cp6wZ...
+00003020: 248f 521e 63cb 19ea 4cc8 5720 3569 eb6c  $.R.c...L.W 5i.l
+00003030: 08a9 4519 d6a3 3123 b3a8 6e70 f10f 287d  ..E...1#..np..(}
+00003040: 2b1e 58df 2d96 5712 b355 aca0 4fb0 f7f8  +.X.-.W..U..O...
+00003050: 081e c87e 5b17 2a9d 68bb 0fed 41f2 7c89  ...~[.*.h...A.|.
+00003060: 0703 b152 d052 d6a0 baf3 8e33 b678 c6b2  ...R.R.....3.x..
+00003070: 0ac5 4377 54b1 89e8 d9ae 8518 10a3 34bd  ..CwT.........4.
+00003080: e0bb f5fb fe3c 1038 b067 277d 2501 1519  .....<.8.g'}%...
+00003090: 5fce 78ee ca1f e168 983d ca4d 2f1b c0fe  _.x....h.=.M/...
+000030a0: ba49 5635 0932 df6a 123f 28a3 140f f20c  .IV5.2.j.?(.....
+000030b0: e54c 1b12 8adf 4256 c8f3 c118 3a10 7c63  .L....BV....:.|c
+000030c0: 80ef 450c c76a cf1b 1a8d 2ed1 04c2 3e48  ..E..j........>H
+000030d0: 2d86 14e7 5797 24c4 a20d 1046 9430 1433  -...W.$....F.0.3
+000030e0: 48c6 b594 c457 fc7c 13c7 9131 e93f 08be  H....W.|...1.?..
+000030f0: 6d10 0c95 7049 bfc2 bccd 19b9 3df5 daa4  m...pI......=...
+00003100: bfd5 0670 5a96 8673 541b 40a3 9cad 45a3  ...pZ..sT.@...E.
+00003110: 513a e539 ba20 57b6 c0d8 55ab 2b4e 8caa  Q:.9. W...U.+N..
+00003120: fdbc 349e cce9 2b5b 2ed9 8d1f 159b 4ce0  ..4...+[......L.
+00003130: adf5 ab8d f00e 0760 1d3f d07f 0cfc 28f0  .......`.?....(.
+00003140: 80aa 6a0b 3d26 3c4b 890b 3be3 fb7a 9cf5  ..j.=&<K..;..z..
+00003150: 100d 454d 4271 b387 733a 4810 f917 5819  ..EMBq..s:H...X.
+00003160: cefe 47b0 5793 bdb0 9797 9ce1 68c9 3e7a  ..G.W.......h.>z
+00003170: d8a2 e2b2 e423 470e 7b1f 1739 48b8 578f  .....#G.{..9H.W.
+00003180: 6e91 daac 38b9 579e 006b 42c8 02cf 9032  n...8.W..kB....2
+00003190: 2c46 e047 f76a 8567 5ec9 9be5 43b6 1a97  ,F.G.j.g^...C...
+000031a0: a171 0cc7 c63a 7890 3b1d 193c 885d d5a9  .q...:x.;..<.]..
+000031b0: 767c f016 8c0b 27f0 91e5 04e0 913b b377  v|....'......;.w
+000031c0: e024 4edd c23b 6771 bb6c e13b e676 962c  .$N..;gq.l.;.v.,
+000031d0: 54cb 187e 54c0 eaa2 ea7e 8cc0 94cc e898  T..~T....~......
+000031e0: 18db 21de c290 ddb7 e4bd 7c6b 58d8 825b  ..!.......|kX..[
+000031f0: e0dc d5b5 571f f49b 113c c496 9317 5b4b  ....W....<....[K
+00003200: 69d3 e303 5363 8192 f33f 3a30 5709 05eb  i...Sc...?:0W...
+00003210: ceea 255f ba7d fe73 7b7f 1375 0aa8 4c28  ..%_.}.s{..u..L(
+00003220: 15a2 85fa d0bc 8ca1 f12b 3aa8 c13b 9e6d  .........+:..;.m
+00003230: 07be ef07 66dd abbb be6b 3bfc ea4f d425  ....f....k;..O.%
+00003240: f869 4e9b 630c b598 77f2 aecd 346b f0e0  .iN.c...w...4k..
+00003250: f15f e249 fe32 bbf2 ed7b 71a1 5516 a64a  ._.I.2...{q.U..J
+00003260: 055c a2ed 3bbe 6339 7e3d b01d d39f 2be0  .\..;.c9~=....+.
+00003270: c9d6 2e0a ecf3 0d0a 3e7e f8f0 ef6f 3f29  ........>~...o?)
+00003280: 61a4 37c6 295c 30cc 2b2b 55e9 0658 4926  a.7.)\0.++U..XI&
+00003290: 55bd 4c14 9818 bff2 1695 b439 4f60 b804  U.L........9O`..
+000032a0: f5a3 71ca 2ee7 2fdb 7af5 fc15 4af0 3803  ..q.../.z...J.8.
+000032b0: 0f98 8dfa 065f 1326 44b4 f5ea f925 afc1  ....._.&D....%..
+000032c0: 5b3e e704 ca5e 2f0b 289c c35f 6d4c 31d0  [>...^/.(.._mL1.
+000032d0: 79de ad07 67e7 a15d 6b98 dd46 cd75 9057  y...g..]k..F.u.W
+000032e0: 0bbc ee59 cd73 4fbb 6767 6160 dae6 e97b  ...Y.sO.gga`...{
+000032f0: e5e2 fd0e d7ee e2ff 04a0 3a65 b9cd 2285  ..........:e..".
+00003300: cb79 3a5b ec0c fc45 d5d7 d695 8684 2fae  .y:[...E....../.
+00003310: ae00 b68a 3db0 7df3 b967 99b5 d031 ad9a  ....=.}..g...1..
+00003320: eb47 8d5a c377 bc5a e859 f699 ef76 cfbd  .G.Z.w.Z.Y...v..
+00003330: d053 b07b 7b5e cf9b 8665 c98b 7e0e de6b  .S.{{^...e..~..k
+00003340: 329c a114 e7a5 ad4a 0ba9 bd60 2468 6e58  2......J...`$hnX
+00003350: 8451 5ac2 a8fe 09a3 f31f 0000 00ff ff03  .QZ.............
+00003360: 0050 4b03 0414 0006 0008 0000 0021 0073  .PK..........!.s
+00003370: 7a97 f518 0600 0041 1d00 0014 0000 0078  z......A.......x
+00003380: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
+00003390: 786d 6cac 594b 531b 4710 bea7 2aff 41b5  xml.YKS.G...*.A.
+000033a0: aa1c 6301 0e7e a400 1f5c 95aa dc72 48ce  ..c..~...\...rH.
+000033b0: 5b63 ed80 b6bc 3bab ec8e 00e5 248a 38e2  [c....;.....$.8.
+000033c0: e957 c0d8 0185 87f1 03a7 8c9c 3201 8ca0  .W..........2...
+000033d0: f833 3bbb d2c9 7f21 23ed 0a56 ea99 95bc  .3;....!#..V....
+000033e0: f651 bdd3 df74 f7f4 7cdd d31a b935 6d1a  .Q...t..|....5m.
+000033f0: a949 6c3b ba45 4695 c12b 034a 0a93 aca5  .Il;.EF..+.J....
+00003400: e964 6254 f9e5 e71f bebd a1a4 1c8a 8886  .dbT............
+00003410: 0c8b e051 a588 1de5 d6d8 d75f 8d38 0e4d  ...Q......._.8.M
+00003420: 715d e28c 2a39 4af3 df67 324e 3687 4de4  q]..*9J..g2N6.M.
+00003430: 5cb1 f298 f02f e396 6d22 ca7f da13 1927  \..../..m".....'
+00003440: 6f63 a439 398c a969 6486 0606 ae65 4ca4  oc.99..id....eL.
+00003450: 1325 95b5 0a84 8e2a 4357 8794 5481 e8bf  .%.....*CW..T...
+00003460: 16f0 ed40 3278 f39a 3236 e2e8 6323 74cc  ...@2x..26..c#t.
+00003470: 7ffb c45f 7dc1 1e2e fbaf de8d 64e8 d848  ..._}.......d..H
+00003480: a629 0fbe a51d 6a23 8a27 8a2a 4126 4e77  .)....j#.'.*A&Nw
+00003490: 7f66 a725 f66a d15b 7be1 6d6c 0a54 914d  .f.%.j.[{.ml.T.M
+000034a0: 558d ab03 3dbf f6a7 57d9 94e8 61a2 89b5  U...=...W...a...
+000034b0: dcda 737f 6bc6 7b52 766b 8772 43c7 7543  ..s.k.{Rvk.rC.uC
+000034c0: 60e8 5c85 1b5a ffef f746 f991 d850 7e22  `.\..Z...F...P~"
+000034d0: 6a16 3939 60ab 7bfc 975f db63 9b27 acfc  j.99`.{.._.c.'..
+000034e0: 0750 bdc3 4f33 6722 fb2e 0c4d 4b41 12d5  .P..O3g"...MKA..
+000034f0: 0b35 d529 9a77 2c03 687b a59a 5799 f5d7  .5.).w,.h{..W...
+00003500: 17c0 8ed4 a2c8 5027 9151 1078 39bf e79e  ......P'.Q.x9...
+00003510: 3d93 7829 74ce 5b39 e49b f8f7 cb92 7d6c  =.x)t.[9......}l
+00003520: 4c0b 3671 a077 1f0e d8d2 13b9 3622 a480  L.6q.w......6"..
+00003530: 0cfd 37ac a952 88e5 55f7 6c99 954b ac74  ..7..R..U.l..K.t
+00003540: 0a76 e7c9 4a55 82a9 c451 b776 d6d8 a908  .v..JU...Q.v....
+00003550: b5a0 adde f28e 37bf 28f4 91fb 66f1 db09  ......7.(...f...
+00003560: c3bf f682 55ca 7245 3439 c153 5437 8a6a  ....U.rE49.ST7.j
+00003570: 333c 6288 f73b 6ce1 b568 d749 cb40 5437  3<b..;l..h.I.@T7
+00003580: 745a 8461 dd7d e03d dbf7 aa2b 223d 2787  tZ.a.}.=...+"='.
+00003590: ec3c 3c74 f778 b1be bdd4 787e bff1 6c0f  .<<t.x....x~..l.
+000035a0: 4444 b3a6 88a3 6b58 b575 07e6 a87f b0e3  DD....kX.u......
+000035b0: 3d78 58af 9ec8 76b4 6caa 130b 8667 a3c4  =xX...v.l....g..
+000035c0: 765f b1f5 bfbd c7bb 604b 134d ab9a 8da6  v_......`K.M....
+000035d0: 9a5b 03cd c04c b776 243a f449 044f a23e  .[...L.v$:.I.O.>
+000035e0: bb21 8ac5 944e d426 3141 6659 9f73 4f1e  .!...N.&1AfY.sO.
+000035f0: 707f 805d 79db 1ae7 4965 588e 2356 f536  p..]y...IeX.#V.6
+00003600: 4a8d d5f3 c0ab 5862 8b7a a86a 056e 0767  J.....Xb.z.j.n.g
+00003610: 7795 d3b8 8cee a2c8 b1d4 2746 9612 6214  w.........'F..b.
+00003620: d75b 9af1 6b6f d9ee 9eb7 0a59 5c8c aba1  .[..ko.....Y\...
+00003630: 22bc 2df5 c37b fc6a 0537 bbef 88e0 e92c  ".-..{.j.7.....,
+00003640: e661 fde4 c0c8 368b af0f 719b 4963 25db  .a....6...q.Ic%.
+00003650: 2a36 6eb1 7ef5 0cdf c7d3 3956 de72 cf56  *6n.~.....9V.r.V
+00003660: 3f9e ce83 740c a165 ec18 3597 e3f8 fb6b  ?...t..e..5....k
+00003670: de46 3506 275b 30e5 4cdb 22eb 2ec4 9e96  .F5.'[0.L.".....
+00003680: 0514 2e05 6d3c 3d67 ef56 bcf7 abc0 3364  ....m<=g.V....3d
+00003690: e473 085c ccfa 4185 6dc3 5b79 0753 b8d6  .s.\..A.m.[y.S..
+000036a0: 3ddf f666 aa12 52d2 49d0 fa34 ef5c ebea  =..f..R.I..4.\..
+000036b0: c1ad 2229 cc5a 8c2a a290 f000 24ac 1a8d  ..").Z.*....$...
+000036c0: 16d7 6641 bd93 727a 0816 43ed 5df9 77c1  ..fA..rz..C.].w.
+000036d0: 9ffd 2449 2ca5 7602 cfb1 9397 12ce 342d  ..$I,.v.......4-
+000036e0: 4273 bc64 85b6 4a29 b47e b459 3f7e 53af  Bs.d..J).~.Y?~S.
+000036f0: 56d9 d13e 6c0b 6c94 bddb ec95 b06d 5b90  V..>l.l......m[.
+00003700: aed9 a3d7 dc00 796e 4c61 7c97 9b20 4e91  ......ynLa|.. N.
+00003710: 4059 9228 a1a6 305f 0245 f951 87ba 92a3  @Y.(..0_.E.Q....
+00003720: 0eb4 2f6a 2170 b9ad 2d29 8681 7a6c ca86  ../j!p..-)..zl..
+00003730: 08bd 3337 8c40 dc01 8458 bc2d ef7d 0e9c  ..37.@...X.-.}..
+00003740: bfe5 753a 048a cdad 7668 aaf5 fded a030  ..u:....vh.....0
+00003750: 7a47 fff2 0396 c5a8 6064 b1ad ea44 c3d3  zG......`d...D..
+00003760: b0b7 69a5 867f 7089 d5f3 c002 b83c b65b  ..i...p......<.[
+00003770: 379e 6471 2c74 7011 a21b c41b 1bde 83de  7.dq,tp.........
+00003780: 3643 e09e 9677 60f7 ed80 a4d7 09ee 8cf4  6C...w`.........
+00003790: be72 6ee2 fd70 f791 040f 1669 87de c56f  .rn..p.....i...o
+000037a0: 712c 145d da83 07fd 5a85 553f 049b f658  q,.]....Z.U?...X
+000037b0: 1aa0 0681 1433 7dc7 be8f 5e8b 59ad 8bfd  .....3}...^.Y...
+000037c0: 24d4 57c4 82d6 322d abbd e9cb e799 74c9  $.W...2-......t.
+000037d0: 04b6 4c4c 6d3d dba6 d360 25c8 fa74 674f  ..LLm=...`%..tgO
+000037e0: 24ea b8d2 004b da3e cb97 f2e7 88a0 994b  $....K.>.......K
+000037f0: 8779 18d6 f298 f294 ee63 49c0 9f92 a2db  .y.......cI.....
+00003800: 06e8 414c e990 767a 1521 f7b8 e46d cc75  ..AL..vz.!...m.u
+00003810: 27b5 7bb2 2492 1ecf 0ba4 6c7d 5d88 b022  '.{.$.....l}].."
+00003820: 5a7b efad 1077 56b8 f61f d1da 0f15 d1da  Z{...wV.........
+00003830: e519 b154 ec1e 5b9e 117b d8bc 4b27 2fd9  ...T..[..{..K'/.
+00003840: c216 9f0b 00ee 1d84 4937 0445 57a1 e83b  ........I7.EW..;
+00003850: 281a 86a2 6b50 741d 8a6e 40d1 4d28 1a1c  (...kPt..n@.M(..
+00003860: 10c8 04f6 0f0a 1ce0 1d2e 5016 4f90 784b  ..........P.O.xK
+00003870: eff2 0153 a9e6 1ebf 11bc 864c 8c48 7710  ...S.......L.Hw.
+00003880: 1daa 758b 4c1d ac1a 1afe a67b d5f0 0010  ..u.L......{....
+00003890: 5d87 ab38 09c0 a7b9 e8f9 9a6e 4dec 042c  ]..8.......nM..,
+000038a0: c26d 8652 6eb5 60a9 2e58 c94b 5016 13aa  .m.Rn.`..X.KP...
+000038b0: 0e09 0eb8 fd6d 5870 38ed 6fd7 057a dc29  .....mXp8.o..z.)
+000038c0: 58e4 5b53 445e 4dbc ad72 63e7 69fb c192  X.[SD^M..rc.i...
+000038d0: cff1 e926 d5b3 3fd9 a971 de85 fea8 f199  ...&..?..q......
+000038e0: a492 a2c5 3c1f 7912 ebb6 45c2 11a9 92e9  ....<.y...E.....
+000038f0: 983e 8257 7842 1cf0 9c4c 88d3 594d 933a  .>.WxB...L..YM.:
+00003900: 2518 9d25 84ea 55c4 1387 ebb2 8a83 1632  %..%..U........2
+00003910: a9d7 dd93 adcf 7219 b40d 09d1 d254 a7ed  ......r......T..
+00003920: 6971 5288 eeb9 4f52 9cce c945 5294 8e86  iqR...OR...ER...
+00003930: 2529 087c 1324 0e4e 6466 9938 30c1 bc27  %).|.$.Ndf.80..'
+00003940: fa7a 4b0a 15db b57d 31d0 cef6 2d29 6cc7  .zK....}1...-)l.
+00003950: fc25 20da cfa3 89c8 6330 187a 796b 878d  .% .....c0.zyk..
+00003960: b583 5661 1220 5fed 83a0 a3ec f0c5 305b  ..Va. _.......0[
+00003970: 7f49 f4c3 3bfd 5818 5264 c477 f0d4 49e8  .I..;.X.Rd.w..I.
+00003980: 7b32 e47e ca5e 3a32 1e49 681c 7fc2 b4e7  {2.~.^:2.Ih.....
+00003990: 6a09 113a 6738 4963 7439 f4fb 6484 0cff  j..:g8Ict9..d...
+000039a0: 0b74 ec7f 0000 00ff ff03 0050 4b03 0414  .t.........PK...
+000039b0: 0006 0008 0000 0021 00fd 81bc be23 0200  .......!.....#..
+000039c0: 00cc 0400 0018 0000 0078 6c2f 6472 6177  .........xl/draw
+000039d0: 696e 6773 2f64 7261 7769 6e67 312e 786d  ings/drawing1.xm
+000039e0: 6c9c 544b 6edb 3010 dd17 e81d 08ee 657d  l.TKn.0.......e}
+000039f0: fd13 2c05 756c 1501 8a34 8be6 0004 4559  ..,.ul...4....EY
+00003a00: 0244 d220 19db 4190 9374 d55d 4fd1 db04  .D. ..A..t.]O...
+00003a10: e831 ca9f 6c23 7181 365a 50c3 19bd 19f2  .1..l#q.6ZP.....
+00003a20: bd19 2dae 0eb4 073b 2264 c759 01e3 5104  ..-....;"d.Y..Q.
+00003a30: 0161 98d7 1ddb 14f0 fe5b 15cc 2090 0ab1  .a.......[.. ...
+00003a40: 1af5 9c91 023e 1209 afca 8f1f 1687 5ae4  .....>........Z.
+00003a50: 7bb9 1240 2760 32d7 db02 b64a 6df3 3094  {..@'`2....Jm.0.
+00003a60: b825 14c9 11df 12a6 a30d 1714 29bd 159b  .%..........)...
+00003a70: b016 68af 53d3 3e4c a268 12ca ad20 a896  ..h.S.>L.h... ..
+00003a80: 2d21 6ae5 22d0 e743 efc8 4651 c760 694f  -!j."..C..FQ.`iO
+00003a90: a6f6 fc9a f4fd 2786 5b2e 9cab 119c 3a0b  ......'.[.....:.
+00003aa0: f3be 4c17 a1b9 8131 2d40 1b5f 9ba6 8c8e  ..L....1-@._....
+00003ab0: 6eb3 b311 c1f7 65ec dcc6 1c7c 261e 27d3  n.....e....|&.'.
+00003ac0: c823 74c8 226c d653 29c5 4f25 e3e9 e59a  .#t."l.S).O%....
+00003ad0: e374 3ccf fe52 3849 2e57 4ee2 743e 1f1f  .t<..R8I.WN.t>..
+00003ae0: 63a7 d243 c18d 40db b6c3 9540 9400 8ab0  c..C..@....@....
+00003af0: e005 f4dc b0dd e7b3 e09d a707 dfee ee04  ................
+00003b00: e8ea 02a6 1030 8d2a e0cb f75f bf7f fc04  .....0.*..._....
+00003b10: 89c6 a19c 1cd4 17a9 bc05 1e44 57c0 a7aa  ...........DW...
+00003b20: 4a96 e375 9505 95b6 822c 5a66 c172 9dcd  J..u.....,Zf.r..
+00003b30: 832a 4967 eb64 5a5d 27e9 e4d9 a0e3 498e  .*Ig.dZ]'.....I.
+00003b40: b5d2 4a37 d94d 3d28 1c4f de68 4c3b 7d50  ..J7.M=(.O.hL;}P
+00003b50: c91b 35c2 9c86 bc69 3a4c 869e d11d 1367  ..5....i:L.....g
+00003b60: a1d5 d81e f329 f24f a0df 33b3 44a7 254a  .....).O..3.D.%J
+00003b70: 5df0 1986 e522 b4a7 1fde f616 4e7c 7365  ]...."......N|se
+00003b80: afcf ed2b 520c cc34 c865 b20e 8dd0 bd84  ...+R..4.e......
+00003b90: 727d 4270 28a0 1e9a 47b3 6a90 2d05 b073  r}Bp(...G.j.-..s
+00003ba0: e2c1 6b53 0d20 2f8d f9d6 9b2b a490 a3f4  ..kS. /....+....
+00003bb0: bf27 08b7 4828 4d31 cead e5b9 c5ef 981e  .'..H(M1........
+00003bc0: 97c9 27f8 a761 76fa ac38 7ea0 8429 37d1  ..'..av..8~..)7.
+00003bd0: 82f4 5666 d976 5b09 81c8 4d47 899b 3af6  ..Vf.v[...MG..:.
+00003be0: 429c ddd8 0a72 24c3 5274 deb5 5e98 bed3  B....r$.Rt..^...
+00003bf0: b90d 4183 22af 46db e2cc 8fa8 fc03 0000  ..A.".F.........
+00003c00: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00003c10: 2100 a1a6 aae6 ce07 0000 9922 0000 1400  !.........."....
+00003c20: 0000 786c 2f63 6861 7274 732f 6368 6172  ..xl/charts/char
+00003c30: 7431 2e78 6d6c ec5a cd72 1bb9 11be a72a  t1.xml.Z.r.....*
+00003c40: ef30 3bbb 39a5 48ce 0c39 2467 cad4 9634  .0;.9.H..9$g...4
+00003c50: 3237 5b91 d72e 4bde 4352 2917 8801 4944  27[...K.CR)...ID
+00003c60: 1860 0c60 24d2 5b7b 490e 39e5 1172 c835  .`.`$.[{I.9..r.5
+00003c70: 4f90 074a a592 b748 e367 2892 92bc 94ed  O..J...H.g(.....
+00003c80: cd56 1cf9 400f fe1a 8d46 7ffd 073d f972  .V..@....F...=.r
+00003c90: 55b1 e08a 4845 059f 8471 370a 03c2 b128  U...HE...q7....(
+00003ca0: 295f 4cc2 5717 d3ce 380c 9446 bc44 4c70  )_L.W...8..F.DLp
+00003cb0: 3209 d744 855f 1efd fc67 4f70 8e97 48ea  2..D._...gOp..H.
+00003cc0: f31a 6112 0011 ae72 3c09 975a d779 afa7  ..a....r<..Z.y..
+00003cd0: f092 5448 7545 4d38 8ccd 85ac 9086 a65c  ..THuEM8.......\
+00003ce0: f44a 89ae 8178 c57a 4914 0d7b 9648 e809  .J...x.zI..{.H..
+00003cf0: a0f7 2050 21ca dbf5 f290 f562 3ea7 989c  .. P!......b>...
+00003d00: 0adc 5484 6bc7 8524 0c69 9080 5ad2 5ab5  ..T.k..$.i..Z.Z.
+00003d10: d470 3c94 c92d 8a15 c552 2831 d75d 2caa  .p<..-...R(1.],.
+00003d20: 9e23 d61e 0a88 c569 6f73 aa23 1052 8934  .#.....ios.#.R.4
+00003d30: 89b3 6810 5c21 3609 a3b0 673a 19e2 0bd7  ..h.\!6...g:....
+00003d40: f176 d929 be71 9d52 34bc 2465 2124 87eb  .v.).q.R4.$e!$..
+00003d50: d89a 5fe1 fc98 6922 3990 2a04 d7c0 b597  .._...i"9.*.....
+00003d60: 5775 90c4 2b24 2f9b ba03 ecd6 70c8 1965  Wu..+$/.....p..e
+00003d70: 54af edb1 c3a3 2740 bb58 0a90 47f0 92bc  T.....'@.X..G...
+00003d80: 69a8 246a 12e2 7870 2382 c143 0510 8d7a  i.$j..xp#..C...z
+00003d90: e35e e2ef 150e 1b0f 72a5 d78c b803 c551  .^......r......Q
+00003da0: 624e dbdb ec6b 5998 22c6 6608 5f1a d96c  bN...kY.".f._..l
+00003db0: 4dde 4cbd 1937 0bf7 8561 5659 3532 1f9a  M.L..7...aVY52..
+00003dc0: 6a46 ecc7 cafc 4a8a 9747 4f50 3e13 e5fa  jF....J..GOP>...
+00003dd0: 850c a4d0 e612 0255 e329 954a 9f21 a55f  .......U.).J.!._
+00003de0: 2009 7a07 9d80 02fd 1c7e e64c 5c4f 42c2   .z......~.L\OB.
+00003df0: 18e8 0205 6d30 fd20 0521 df86 c1b5 44f5  ....m0. .!....D.
+00003e00: 2454 6f1a 2449 1820 8ea1 1b24 a665 db28  $To.$I. ...$.e.(
+00003e10: 34b4 6373 4694 33a5 cfcd d16d a336 3d35  4.csF.3....m.6=5
+00003e20: f050 92f9 059a 9dbf 9d84 593c 1844 11dc  .P........Y<.D..
+00003e30: 02ca a1f3 258c 19c5 9884 4e29 0205 5362  ....%.....N)..Sb
+00003e40: 3321 9859 fea8 fd6d 2621 0724 1a54 4a7a  3!.Y...m&!.$.TJz
+00003e50: 0988 e4e2 dc7e 85c1 25e8 082c 015c d913  .....~..%..,.\..
+00003e60: dae9 33a4 08a3 06b9 6e23 2518 2da7 9431  ..3.....n#%.-..1
+00003e70: b3ab 8529 2998 7497 a357 b165 8635 d533  ...)).t..W.e.5.3
+00003e80: 51ba be61 1a01 3977 9ca6 7a3e 9fbb ee7e  Q..a..9w..z>...~
+00003e90: dbdd dba2 02f7 0aad ed0d 0caa 78a0 d735  ............x..5
+00003ea0: 9983 9998 84bf ac78 8769 478e a0bd 0182  .......x.iG.....
+00003eb0: dc00 567b 0358 599d 69a5 64b7 0149 9a13  ..V{.XY.i.d..I..
+00003ec0: b89f 7dc9 2106 376b 2449 78e7 d5b9 a3aa  ..}.!.7k$Ix.....
+00003ed0: 8ffe f1f7 bffd eb0f 7ffd e75f fef8 ef3f  ..........._...?
+00003ee0: fdd9 70aa 2d21 a000 df70 3bbd 565b e043  ..p.-!...p;.V[.C
+00003ef0: 5be5 1170 f30c ad77 a0ab fcc6 5c18 213a  [..p...w....\.!:
+00003f00: b970 c3c9 a603 a831 db43 e673 82f5 99d2  .p.....1.C.s....
+00003f10: 46e1 41b1 ed4a 43db b1fe a892 9fa6 4a12  F.A..JC.......J.
+00003f20: 5e1a 93b2 0f67 a304 ad9e 3915 307a d65a  ^....g....9.0z.Z
+00003f30: 2bd4 6871 611a a784 114d 3cf8 bcbb a899  +.hqa....M<.....
+00003f40: d0c7 9220 e73a d6a2 311a 055e 0460 5d18  ... .:..1..^.`].
+00003f50: 1f6c 1a0b 701f 35f8 55a7 acce 63cb d279  .l..p.5.U...c..y
+00003f60: 962b 24d7 8560 62c7 ab80 4212 d07d 9cd3  .+$..`b...B..}..
+00003f70: 72b5 a3e1 4296 c41b 04bf bf43 03d8 9b97  r...B......C....
+00003f80: 646e 56cc 77a0 f4d9 17c5 17b1 5170 3b06  dnV.w.......Qp;.
+00003f90: b30a 04de dfcc ab75 013e 4d7b cbef 78a9  .......u.>M{..x.
+00003fa0: 7500 1b3a 6b84 f3ab a38a 206e 165f 598c  u..:k..... n._Y.
+00003fb0: d406 93c6 07b4 445c c3ee bb81 650b 41c6  ......D\....e.A.
+00003fc0: 03b0 d3c9 381d a561 808d 5d96 bcb4 06ec  ....8..a..].....
+00003fd0: 5d46 0e61 0c0e d45a e87d 6b65 3db0 bba7  ]F.a...Z.}ke=...
+00003fe0: 7722 d838 5427 3bb5 ae66 02e2 27e3 dbad  w".8T';..f..'...
+00003ff0: 5576 50bf 9980 91bd 9d6d d9fd 36fa dd67  UvP......m..6..g
+00004000: 25a2 6cfd fab5 090e d47b 8bee 73b3 fcf3  %.l......{..s...
+00004010: 8385 e759 015e cddd f0a6 dadc e616 47d7  ...Y.^........G.
+00004020: 842e 96fa 757b 2bf6 4a61 eae6 4a5d 2457  ....u{+.Ja..J]$W
+00004030: 8892 1c45 dd28 fa85 65de 4677 b6ef c04b  ...E.(..e.Fw...K
+00004040: 8f6e 317d b307 5c73 cb9b 510b c7ad aa84  .n1}..\s..Q.....
+00004050: d0cb 1d35 252b 635a cd51 e02b 6824 78c7  ...5%+cZ.Q.+h$x.
+00004060: ef8a 7e7f 1c15 c5a0 939e 0e9f 7606 5156  ..~.........v.QV
+00004070: 744e 9ef6 93ce d351 729a 64a3 7eda 2f8a  tN.....Qr.d.~./.
+00004080: efb7 c2bb 0707 7783 adb8 6698 379c be69  ......w...f.7..i
+00004090: c8d7 1eac df81 a3b4 ff3a c338 39ee 0ca6  .........:.89...
+000040a0: 27a3 ce49 3a9d 76d2 a43f ca06 c0d8 f424  '..I:.v..?.....$
+000040b0: fdde 7a32 cbb3 d5f4 f614 46cf bd4a eda1  ..z2......F..J..
+000040c0: d26a 2ace b750 e97b 7e08 95bf fa00 548e  .j*..P.{~.....T.
+000040d0: 527b b3ff 6550 ba78 6f2f 8478 04e5 6b0f  R{..eP.xo/.x..k.
+000040e0: ca51 ba31 158f 90b4 49a4 c9b7 0e81 64fc  .Q.1....I.....d.
+000040f0: 7121 69f5 7407 92be e787 20f9 f587 384a  q!i.t..... ...8J
+00004100: b4fa 09fc 64df 47de 3b1e f511 922d 242b  ....d.G.;....-$+
+00004110: 7729 8f6e 1293 ed1a c821 984c 3e0c 93e5  w).n.....!.L>...
+00004120: d98c 295b 2f58 8aeb 33b2 80a8 fbd7 642f  ..)[/X..3.....d/
+00004130: 5583 916f 918f ce7c 28ab a0af 40fa 1b54  U..o...|(...@..T
+00004140: f982 c456 ff39 9177 f6bf 20d2 848c bb69  ...V.9.w.. ....i
+00004150: 20d0 3969 6633 46ce e9db 6d52 e0c8 6f58   .9if3F...mR..oX
+00004160: bb1d b5a0 551b 2ec4 511c 27f0 6311 86f3  ....U...Q.'.c...
+00004170: ad81 2c1d 0cb3 6132 f6a1 c24e 986f 42be  ..,...a2...N.oB.
+00004180: 639b 9cde 4b49 6104 4b16 4636 4252 60dc  c...KIa.K.F6BR`.
+00004190: 56b6 1cf7 15e5 cfd0 ca13 de9a 58da ac63  V...........X..c
+000041a0: e784 68f5 42f8 2ad4 cc85 eee0 74a6 950e  ..h.B.*.....t...
+000041b0: 6e42 c049 f815 815a 1562 506e 100d 08e9  nB.I...Z.bPn....
+000041c0: 8cf2 4b52 6eca 5c15 fabd 9017 145f 3e83  ..KRn.\......_>.
+000041d0: 8079 3748 c639 b072 ffa0 8645 70c1 1b0e  .y7H.9.r...Ep...
+000041e0: a022 e378 b833 fd36 6940 9626 6d16 3087  .".x.3.6i@.&m.0.
+000041f0: aa03 2404 550d 9c28 be80 ca0c 5b40 5dc4  ..$.U..(....[@].
+00004200: 1469 6cd1 e381 1590 f8ee 0ac8 f8b0 0ac8  .il.............
+00004210: a1b6 f263 5405 0e2d 4e99 2bc4 e4f8 d85f  ...cT..-N.+...._
+00004220: d43d 85aa 7795 a5b2 f7ac 4a7d e2d5 a883  .=..w.....J}....
+00004230: 537f 2858 4211 591d fbcc 3bde 86bc 1f23  S.(XB.Y...;....#
+00004240: 1e7c a632 f01b 2285 d37f d3da 8129 9b31  .|.2.."......).1
+00004250: 28ca 29d2 66d9 ae58 8773 23e9 0b5a 9157  (.).f..X.s#..Z.W
+00004260: 9cfa a112 ad5d 1dcd 15a5 9d15 81fc ea96  .....]..........
+00004270: 39d9 65e6 e39b 13e6 8e62 adc3 5792 96c6  9.e......b..W...
+00004280: c039 53ee 6b6b 2eb1 ffdf 4634 f881 db07  .9S.kk....F4....
+00004290: bcc3 82da 2c7a df7e fa0c efe3 d94f 0e79  ....,z.~.....O.y
+000042a0: e685 57a1 1fa7 82d9 19fa ecf7 272d ae3f  ..W.........'-.?
+000042b0: da2c 5b91 7e48 05fd bd6d d66e fc62 edd9  .,[.~H...m.n.b..
+000042c0: dd36 cb0e 9d10 7d4d 0877 b66b e61a 3e0e  .6....}M.w.k..>.
+000042d0: d9d8 a00f d54c c0dc 4ea9 d446 85b6 526a  .....L..N..F..Rj
+000042e0: bff6 e319 28ed 4329 d58c 5788 3788 9d6d  ....(.C)..W.7..m
+000042f0: da2b 78fe f041 1d29 17c4 d9ab f55d 9d6d  .+x..A.).....].m
+00004300: e9b4 9b0c b2f1 2889 922c 49a3 413a 8a3c  ......(..,I.A:.<
+00004310: 84db 88b4 9b25 c324 1b66 e978 9ca6 5166  .....%.$.f.x..Qf
+00004320: 633b 9c5f 7b53 de4d fb09 3cb4 8c93 6438  c;._{S.M..<...d8
+00004330: cce2 68e0 1ec9 70ee 2b5e 6937 eb67 f168  ..h...p.+^i7.g.h
+00004340: 04d1 6236 1c8d b26c fcb4 e36a 25fb ac83  ..b6...l...j%...
+00004350: 046e 4ef5 fff2 7cf1 08fa 1f0f f446 a136  .nN...|......F.6
+00004360: 3032 e0fa 96aa e79c 79b5 f64a 5e52 559f  02......y..J^RU.
+00004370: c0d3 e5a5 3af6 41cb 02d5 3e5e 873c e9d4  ....:.A...>^.<..
+00004380: a46a e661 1552 8fad d805 486f 5e6d 5be4  .j.a.R....Ho^m[.
+00004390: bfab 703f 5bdc 59b4 ff14 8285 fd47 c1fb  ..p?[.Y......G..
+000043a0: 5f8f efd1 75ff b8e4 1e16 1f60 d16b 49b9  _...u......`.kI.
+000043b0: 3e27 1a5e 6917 3604 5b12 04af 3f53 a8b6  >'.^i.6.[...?S..
+000043c0: 1369 1f99 6ab4 2090 be2d 2857 f619 ba6b  .i..j. ..-(W...k
+000043d0: 1e5b cc5f 3274 4761 004f ddf6 7ff3 a86e  .[._2tGa.O.....n
+000043e0: 07dc 72d3 ea87 9065 182a aeb1 a105 9b35  ..r....e.*.....5
+000043f0: b57b 25d9 dbbc d507 fb17 2547 ff01 0000  .{%.......%G....
+00004400: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00004410: 2100 a208 0791 9f04 0000 8726 0000 1400  !..........&....
+00004420: 0000 786c 2f63 6861 7274 732f 7374 796c  ..xl/charts/styl
+00004430: 6531 2e78 6d6c ec5a 6d6f e238 10fe 2b91  e1.xml.Zmo.8..+.
+00004440: 7f40 03f4 6829 2a95 7aad 563a 89de 567b  .@..h)*.z.V:..V{
+00004450: 2bdd 6793 38e0 5bc7 ced9 6629 fdf5 3776  +.g.8.[...f)..7v
+00004460: 5e88 f3c2 4b0b b470 fb0d 4f82 e379 66fc  ^...K..p..O..yf.
+00004470: cc78 c6b7 811a 0633 2cf5 5f7a c988 f712  .x.....3,._z....
+00004480: 330e 0235 4233 ad93 a1ef ab60 4662 ac2e  3..5B3.....`Fb..
+00004490: 621a 48a1 44a4 2f02 11fb 228a 6840 fc50  b.H.D./...".h@.P
+000044a0: e205 e553 bfd7 e9f6 fcd5 2c28 9b06 d766  ...S......,(...f
+000044b0: 1109 e1f0 8948 c818 6b75 21e4 349f 2366  .....H..ku!.4.#f
+000044c0: 304b e7ca 8f31 e5c8 a3e1 08f5 7ad7 e8ee  0K...1......z...
+000044d0: 1696 875f a8fa 4e35 2376 c4f8 3712 c10b  ..._..N5#v..7...
+000044e0: 2f23 d441 be15 4594 b19a 9044 1109 74fd  /#.A..E....D..t.
+000044f0: 5dc1 57c2 9872 21e1 2378 68d5 240f 4c7a  ].W..r!.#xh.$.Lz
+00004500: 3f31 1b21 fdd2 b562 368f 9f44 98ca aefa  ?1.!...b6..D....
+00004510: 9d8e fd22 1e82 f86b 14a5 e2cb 5cec 9766  ..."...k....\..f
+00004520: b9bb f561 e151 fa2d bbc6 9044 df9e a5a7  ...a.Q.-...D....
+00004530: 5e47 a86b e6f1 7e10 c9e1 3728 6db4 30af  ^G.k..~...7(m.0.
+00004540: bb7a 0658 93a9 90cb 7bd0 fe94 1557 c9b3  .z.X....{....W..
+00004550: 3408 33ee 2d46 e8a6 dfeb 232f c0c9 0845  4.3.-F....#/...E
+00004560: 0c6b f819 2760 6bc5 a7c8 c36c 0a88 043a  .k..'`k....l...:
+00004570: b388 6034 fc02 96dd d23c dd66 f30c 5acc  ..`4.....<.f..Z.
+00004580: 03c6 2a7f 408a 390f 8d1d cc42 5373 a40b  ..*.@.9....BSs..
+00004590: 07bb 944c 77d3 6cb9 9aad ec5e b897 047b  ...Lw.l....^...{
+000045a0: b108 6133 61c6 c4e2 4f61 d4f9 fa93 4849  ..a3a...Oa....HI
+000045b0: 4302 ea5a d998 7292 cb52 7f3f 9a87 677e  C..Z..r..R.?..g~
+000045c0: 5776 d3dc 5a0e 3895 cd31 9976 adcb 5620  Wv..Z.8..1.v..V 
+000045d0: 3c0b 03b7 edcd c2a0 e966 c61a 8ff1 8480  <........f......
+000045e0: 6f82 7f7c 1823 5d37 bb7c 6f67 466a 71eb  o..|.#]7.|ogFjq.
+000045f0: d051 b318 3d18 cf9d ebe3 e91e fed8 371b  .Q..=.........7.
+00004600: 6fe3 e64c b7b8 b925 a435 ecd4 b4dc c226  o..L...%.5.....&
+00004610: 6ef0 282c 5809 1ece d6da 9d93 c029 2722  n.(,X........)'"
+00004620: 5c42 bc91 429b 38e9 a924 f842 a5d2 63ac  \B..B.8..$.B..c.
+00004630: f433 9610 99bb c803 26d2 867a 2220 2220  .3......&..z" " 
+00004640: 5e46 13e4 cd84 7cad cacc 7b10 cae1 09f2  ^F....|...{.....
+00004650: 16d2 70b7 fa77 8e25 411e fb83 03bb 5d5e  ..p..w.%A.....]^
+00004660: f5af af90 a7ed a03b e80d 06c8 93e5 2793  .......;......'.
+00004670: f213 cc03 982a 257a 2f1d 3c68 18a7 3656  .....*%z/.<h..6V
+00004680: c9fd 5c03 51ea 8c9c 523d 5246 6ef4 4023  ..\.Q...R=RFn.@#
+00004690: 7c16 946f e78f e623 808e 32c9 4e11 ed31  |..o...#..2.N..1
+000046a0: 7c31 0fc2 592e 61df 7a77 0af1 4682 4d66  |1..Y.a.zw..F.Mf
+000046b0: b0b4 3ac5 9a1c 2175 5cf3 cbd5 bb18 5d3e  ..:...!u\.....]>
+000046c0: 6eb5 2fcf 1087 4cf3 0209 1358 eb58 6c30  n./...L....X.Xl0
+000046d0: bfe5 f27a 5269 9900 403f a447 a4f1 b337  ...zRi..@?.G...7
+000046e0: e85f e719 92e4 619a 9cae 219b 165f c1c3  ._....a...!.._..
+000046f0: d68c c671 9e02 a402 b627 2c21 35dd 1f70  ...q.....',!5..p
+00004700: a7bb df9c 9c75 13e9 b7ed d96a 3ee9 a05f  .....u.....j>.._
+00004710: c2ba 82ff 182f 21c4 7a6a 194f 049c 4702  ...../!.zj.O..G.
+00004720: 2a03 067c abe8 2b19 a17e 76ee 29fe f337  *..|..+..~v.)..7
+00004730: 9524 9238 3e41 7f2f 1d08 8ee0 ee2e 5006  .$.8>A./......P.
+00004740: bfef 7872 da07 cb3c 95e1 f674 0111 e7bc  ..xr...<...t....
+00004750: 8f5a aecd 42b1 e0bf e306 b63a 5461 c0e4  .Z..B......:Ta..
+00004760: 766f 8cea 7bc8 62db 4f5c 9be8 690f 058d  vo..{.b.O\..i...
+00004770: f539 a9e5 b592 3542 2992 e608 7cc8 9acd  .9....5B)...|...
+00004780: 1ad3 1cfa 785a d481 dc0c bfa8 1aad cbf0  ....xZ..........
+00004790: 3745 eb32 9650 3d10 f2a8 3e6f 7ce7 0381  7E.2.P=...>o|...
+000047a0: ddb1 eeb6 6d61 c738 ac83 259c 82c4 1199  ....ma.8..%.....
+000047b0: 6403 aa0e 9d9b dd5d 086a c741 5b6a 2c16  d......].j.A[j,.
+000047c0: 3f85 e212 83d4 f709 fff3 89d4 39d1 e290  ?...........9...
+000047d0: 81b6 0e68 2131 e5e3 e396 803e 701f 3617  ...h!1.....>p.6.
+000047e0: 9b6e de59 5f75 102e f09c d1b1 f85f 458f  .n.Y_u......._E.
+000047f0: 1d4b 79bb 909c 8b25 c121 91bf 02f3 08ed  .Ky....%.!......
+00004800: 2330 b30a 9a64 4a78 7826 5daa 969a 305b  #0...dJxx&]...0[
+00004810: e998 30a1 4fae c761 f826 5fb8 b554 3eb8  ..0.O..a.&_..T>.
+00004820: 7c3c a95e 4d59 8fac f2a5 88a4 449d 7abf  |<.^MY......D.z.
+00004830: 7073 b7ad a267 3afc 4569 fba1 b40a 9afa  ps...g:.Ei......
+00004840: 9cfa eebf 99ee edc4 f643 4add 77d3 1bb1  .........CJ.w...
+00004850: b209 56c4 64ce d9c5 02b3 c356 ea6b 09d4  ..V.d......V.k..
+00004860: 6e9e eeab 329a 5f5e 387c 49b9 7bd3 e983  n...2._^8|I.{...
+00004870: e2b6 e9fe ae1a 5b02 0da4 47ac 66e9 c507  ......[...G.f...
+00004880: b554 8f42 676d 0ab7 696e a173 002b e0fb  .T.Bgm..in.s.+..
+00004890: 046d d3bd 5de4 6809 910d bace 9353 a952  .m..].h......S.R
+000048a0: b576 3d8b db1b 6f29 35bd e772 46e3 7977  .v=...o)5..rF.yw
+000048b0: 0528 dcd7 9993 f30f 7aae 9a0b 68c1 7f9a  .(......z...h...
+000048c0: 83e7 8ea5 8a74 ed86 2256 37c6 eefe 0300  .....t.."V7.....
+000048d0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000048e0: 0021 001c 14a7 a8fd 0000 006e 0300 0015  .!.........n....
+000048f0: 0000 0078 6c2f 6368 6172 7473 2f63 6f6c  ...xl/charts/col
+00004900: 6f72 7331 2e78 6d6c a493 416e c230 1045  ors1.xml..An.0.E
+00004910: af12 f900 7112 20ad 22c2 a6eb 8a05 2718  ....q. .".....'.
+00004920: 4d6c 62c9 f620 dba5 707b 9c50 6843 2112  Mlb.. ..p{.PhC!.
+00004930: c13b fbeb bff9 7f24 2fd1 5748 9adc 261c  .;.....$/.WH..&.
+00004940: b548 0e46 dbf8 e06b d686 b0ab 38f7 d80a  .H.F...k....8...
+00004950: 033e 350a 1d79 9221 4532 9ca4 5428 78e3  .>5..y.!E2..T(x.
+00004960: e05b d92d 2fb2 bce0 d882 0b3d 85fd 60e0  .[.-/......=..`.
+00004970: 1f85 76c2 c611 929c 81e0 5372 db0b c3e8  ..v.......Sr....
+00004980: 48c9 4a6e 4059 9618 11da 9ae1 11b5 6089  H.Jn@Y........`.
+00004990: 6a6a 9667 6cb5 84aa 4f23 3eb4 4bf6 a06b  jj.gl...O#>.K..k
+000049a0: 0688 c286 9cf1 875a 31a2 cd46 b4f9 88b6  .......Z1..F....
+000049b0: 18d1 ca4e 8b2b dd83 5310 14d9 9b6b 1754  ...N.+..S....k.T
+000049c0: 7f99 4f6a ce0d ca2c 9ece c3ff 9a86 885b  ..Oj...,.......[
+000049d0: cffb c5d3 a3d6 529e 5171 7dd3 514f 8cbf  ......R.Qq}.QO..
+000049e0: 461e 8e9f 4f18 bf98 e079 bbdf 7ef6 0aea  F...O....y..~...
+000049f0: 89f6 d7c8 c3f6 8f9a 74e4 dfef b53a 0100  ........t....:..
+00004a00: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00004a10: 0021 0015 afaa 3cbd 0000 002b 0100 0023  .!....<....+...#
+00004a20: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00004a30: 2f5f 7265 6c73 2f73 6865 6574 312e 786d  /_rels/sheet1.xm
+00004a40: 6c2e 7265 6c73 848f cd0a c230 1084 ef82  l.rels.....0....
+00004a50: ef10 f66e d27a 1091 a65e 44f0 2af5 0196  ...n.z...^D.*...
+00004a60: 64fb 836d 12b2 f1a7 6f6f 2e82 82e0 6d67  d..m....oo....mg
+00004a70: 97fd 66a6 da3f a751 dc29 f2e0 9d86 5216  ..f..?.Q.)....R.
+00004a80: 20c8 196f 07d7 69b8 34c7 d516 0427 7416   ..o..i.4....'t.
+00004a90: 47ef 48c3 4c0c fb7a b9a8 ce34 62ca 4fdc  G.H.L..z...4b.O.
+00004aa0: 0f81 45a6 38d6 d0a7 1476 4ab1 e969 4296  ..E.8....vJ..iB.
+00004ab0: 3e90 cb97 d6c7 0953 96b1 5301 cd15 3b52  >......S..S...;R
+00004ac0: eba2 d8a8 f8c9 80fa 8b29 4e56 433c d912  .........)NVC<..
+00004ad0: 4433 87ec fc9f eddb 7630 74f0 e636 914b  D3......v0t..6.K
+00004ae0: 3f2c 948d f8c8 cd32 1263 4749 8394 ef1d  ?,.....2.cGI....
+00004af0: bf87 52e6 c8a0 ea4a 7d55 ac5f 0000 00ff  ..R....J}U._....
+00004b00: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00004b10: 000e 44f4 dfbc 0000 0025 0100 0023 0000  ..D......%...#..
+00004b20: 0078 6c2f 6472 6177 696e 6773 2f5f 7265  .xl/drawings/_re
+00004b30: 6c73 2f64 7261 7769 6e67 312e 786d 6c2e  ls/drawing1.xml.
+00004b40: 7265 6c73 848f cd0a c230 1084 ef82 ef10  rels.....0......
+00004b50: f66e d27a 1091 a6bd 88d0 abd4 0758 d2ed  .n.z.........X..
+00004b60: 0fb6 49c8 46b1 6f6f a017 05c1 d3b0 3bec  ..I.F.oo......;.
+00004b70: 373b 45f5 9a27 f1a4 c0a3 b31a 7299 8120  7;E..'......r.. 
+00004b80: 6b5c 3bda 5ec3 adb9 ec8e 2038 a26d 7172  k\;.^..... 8.mqr
+00004b90: 9634 2cc4 5095 db4d 71a5 0963 3ae2 61f4  .4,.P..Mq..c:.a.
+00004ba0: 2c12 c5b2 8621 467f 528a cd40 33b2 749e  ,....!F.R..@3.t.
+00004bb0: 6c72 3a17 668c 690c bdf2 68ee d893 da67  lr:.f.i...h....g
+00004bc0: d941 854f 0694 5f4c 51b7 1a42 dde6 209a  .A.O.._LQ..B.. .
+00004bd0: c5a7 e4ff 6cd7 75a3 a1b3 338f 996c fc11  ....l.u...3..l..
+00004be0: a1cc 8021 2620 869e a206 29d7 0daf 92cb  ...!& ....).....
+00004bf0: f42c a8b2 505f e5ca 3700 0000 ffff 0300  .,..P_..7.......
+00004c00: 504b 0304 1400 0600 0800 0000 2100 801b  PK..........!...
+00004c10: dc81 d200 0000 8f01 0000 1f00 0000 786c  ..............xl
+00004c20: 2f63 6861 7274 732f 5f72 656c 732f 6368  /charts/_rels/ch
+00004c30: 6172 7431 2e78 6d6c 2e72 656c 73ac 90c1  art1.xml.rels...
+00004c40: 4ac4 3010 86ef 82ef 10e6 6ed3 ec41 4436  J.0.......n..AD6
+00004c50: dd83 20ec 55d7 0708 e9b4 0d9b 64c2 4c10  .. .U.......d.L.
+00004c60: fbf6 a617 b18b 478f 33c3 ff7d 3f73 3c7d  ......G.3..}?s<}
+00004c70: a5a8 3e91 2550 b660 ba1e 1466 4f63 c8b3  ..>.%P.`...fOc..
+00004c80: 858f cbeb c313 28a9 2e8f 2e52 460b 2b0a  ......(....RF.+.
+00004c90: 9c86 fbbb e31b 4657 5b48 9650 4435 4a16  ......FW[H.PD5J.
+00004ca0: 0b4b ade5 596b f10b 2627 1d15 cced 3211  .K..Yk..&'....2.
+00004cb0: 2757 dbc8 b32e ce5f dd8c fad0 f78f 9a7f  'W....._........
+00004cc0: 3360 d831 d579 b4c0 e7f1 00ea b296 66be  3`.1.y........f.
+00004cd0: 61a7 e099 84a6 da79 4a9a a629 f88d 6acc  a......yJ..)..j.
+00004ce0: 9eaa fde2 b8be 5024 7eaf 6bc4 4673 3c63  ......P$~.k.Fs<c
+00004cf0: b5e0 b79d 98ae 1504 fdb7 dbfc 87fb 462b  ..............F+
+00004d00: 5b8b 1fab debd 71f8 0600 00ff ff03 0050  [.....q........P
+00004d10: 4b03 0414 0006 0008 0000 0021 00eb 7571  K..........!..uq
+00004d20: 7c52 0100 0065 0200 0011 0008 0164 6f63  |R...e.......doc
+00004d30: 5072 6f70 732f 636f 7265 2e78 6d6c 20a2  Props/core.xml .
+00004d40: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
 00004d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004e00: 0000 0000 0000 0000 0000 0000 007c 925d  .............|.]
-00004e10: 4bc3 3018 85ef 05ff 43c9 7d9b b413 99a1  K.0.....C.}.....
-00004e20: ed40 6557 0e04 2b8a 7721 79d7 159b 0f92  .@eW..+.w!y.....
-00004e30: 6857 7fbd 69b7 d50e 45c8 4d72 4e9e 9cf3  hW..i...E.MrN...
-00004e40: 927c b597 6df4 09d6 355a 1528 4d08 8a40  .|..m...5Z.(M..@
-00004e50: 712d 1a55 17e8 b95a c74b 1439 cf94 60ad  q-.U...Z.K.9..`.
-00004e60: 5650 a01e 1c5a 9597 1739 3794 6b0b 8f56  VP...Z...97.k..V
-00004e70: 1bb0 be01 1705 9272 949b 02ed bc37 1463  .......r.....7.c
-00004e80: c777 2099 4b82 4305 71ab ad64 3e6c 6d8d  .w .K.C.q..d>lm.
-00004e90: 0de3 efac 069c 1172 8d25 7826 9867 7800  .......r.%x&.gx.
-00004ea0: c666 22a2 2352 f009 693e 6c3b 0204 c7d0  .f".#R..i>l;....
-00004eb0: 8204 e51d 4e93 14ff 783d 58e9 febc 302a  ....N...x=X...0*
-00004ec0: 33a7 6c7c 6f42 a763 dc39 5bf0 8338 b9f7  3.l|oB.c.9[..8..
-00004ed0: ae99 8c5d d725 dd62 8c11 f2a7 f875 f3f0  ...].%.b.....u..
-00004ee0: 3456 8d1b 35cc 8a03 2a73 c129 b7c0 bcb6  4V..5...*s.)....
-00004ef0: e5d0 dff4 fb36 c7b3 c361 802d 737e 1366  .....6...a.-s~.f
-00004f00: bd6d 40dc f665 dba8 4868 557f ed98 cef1  .m@..e..HhU.....
-00004f10: 6f3d 30c7 0a07 3088 2884 a287 0a27 e565  o=0...0.(....'.e
-00004f20: 7177 5fad 5199 912c 8bc9 22ce 6e2a 4228  qw_.Q..,..".n*B(
-00004f30: 5952 42de 86e7 cfee 0f21 0f07 f218 e27f  YRB......!......
-00004f40: e255 4cc2 baa9 5242 b38c 9274 463c 01ca  .UL...RB...tF<..
-00004f50: 31f7 f9c7 28bf 0100 00ff ff03 0050 4b03  1...(........PK.
-00004f60: 0414 0006 0008 0000 0021 00d0 51b3 73f5  .........!..Q.s.
-00004f70: 0100 00b4 0300 0010 0008 0164 6f63 5072  ...........docPr
-00004f80: 6f70 732f 6170 702e 786d 6c20 a204 0128  ops/app.xml ...(
-00004f90: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00004fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e40: 0000 0000 0000 7c92 514b c330 1485 df05  ......|.QK.0....
+00004e50: ff43 c97b 9bb4 1b6e 0b6d 072a 7b72 2038  .C.{...n.m.*{r 8
+00004e60: 517c 0bc9 5d57 6c93 9044 bbfa eb4d dbad  Q|..]Wl..D...M..
+00004e70: 7628 3ee6 9e93 2fe7 5c92 ae8f 7515 7c82  v(>.../.\...u.|.
+00004e80: b1a5 9219 8a23 8202 905c 8952 1619 7ade  .....#...\.R..z.
+00004e90: 6dc2 250a ac63 52b0 4a49 c850 0b16 adf3  m.%..cR.JI.P....
+00004ea0: ebab 946b ca95 8147 a334 1857 820d 3c49  ...k...G.4.W..<I
+00004eb0: 5aca 7586 0ece 698a b1e5 07a8 998d bc43  Z.u...i........C
+00004ec0: 7a71 af4c cd9c 3f9a 026b c6df 5901 3821  zq.L..?..k..Y.8!
+00004ed0: e406 d7e0 9860 8ee1 0e18 ea91 884e 48c1  .....`.......NH.
+00004ee0: 47a4 fe30 550f 101c 4305 3548 6771 1cc5  G..0U...C.5Hgq..
+00004ef0: f8c7 ebc0 d4f6 cf0b bd32 71d6 a56b b5ef  .........2q..k..
+00004f00: 748a 3b65 0b3e 88a3 fb68 cbd1 d834 4dd4  t.;e.>...h...4M.
+00004f10: ccfa 183e 7f8c 5fb7 0f4f 7dd5 b094 ddae  ...>.._..O}.....
+00004f20: 38a0 3c15 9c72 03cc 2993 77fd 757b ac52  8.<..r..).w.u{.R
+00004f30: 3c19 760b ac98 755b bfeb 7d09 e2b6 cdab  <.v...u[..}.....
+00004f40: 5206 42c9 e2eb c054 8a7f eb9e d957 18c0  R.B....T.....W..
+00004f50: 2002 1f8a 0e15 ceca cbec ee7e b741 7942   ..........~.AyB
+00004f60: 9224 24b3 3059 ed08 a164 4909 79eb 9ebf  .$$.0Y...dI.y...
+00004f70: b8df 851c 06f5 29c4 ffc4 7948 e661 bcd8  ......)...yH.a..
+00004f80: 9115 8d17 74be 9810 cf80 bccf 7df9 31f2  ....t.......}.1.
+00004f90: 6f00 0000 ffff 0300 504b 0304 1400 0600  o.......PK......
+00004fa0: 0800 0000 2100 d051 b373 f501 0000 b403  ....!..Q.s......
+00004fb0: 0000 1000 0801 646f 6350 726f 7073 2f61  ......docProps/a
+00004fc0: 7070 2e78 6d6c 20a2 0401 28a0 0001 0000  pp.xml ...(.....
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005090: 0000 009c 93cb 6ed3 4014 86f7 48bc 8335  ......n.@...H..5
-000050a0: fb66 dc82 2214 8d5d a116 d405 8848 49bb  .f.."..].....HI.
-000050b0: 1fc6 c7c9 0867 c69a 9946 09cb 2294 d002  .....g...F.."...
-000050c0: 2bba 6a2b b548 6d11 1b36 502e 6adf 2636  +.j+.Hm..6P.j.&6
-000050d0: eeaa afc0 d856 5387 462c d89d cbef 5f9f  .....VS.F,...._.
-000050e0: cf39 4396 07bd c8e9 83d2 5c0a 0f2d d65c  .9C.......\..-.\
-000050f0: e480 6032 e0a2 e3a1 f5f6 e385 07c8 d186  ..`2............
-00005100: 8a80 4652 8087 86a0 d1b2 7ff7 0e69 2a19  ..FR.........i*.
-00005110: 8332 1cb4 632d 84f6 50d7 98b8 81b1 665d  .2..c-..P.....f]
-00005120: e851 5db3 6d61 3ba1 543d 6a6c aa3a 5886  .Q].ma;.T=jl.:X.
-00005130: 2167 b02a d966 0f84 c14b ae5b c730 3020  !g.*.f...K.[.00 
-00005140: 0208 16e2 a921 2a1d 1b7d f3bf a681 6439  .....!*..}....d9
-00005150: 9fde 680f 630b ec93 8771 1c71 468d fd4b  ..h.c....q.qF..K
-00005160: ff29 674a 6a19 1ae7 d180 4144 70b5 492c  .)gJj.....ADp.I,
-00005170: 5d0b d8a6 e266 e8bb 0457 53d2 6234 8215  ]....f...WS.b4..
-00005180: 6bec 8734 d240 f04d 81ac 01cd 87d6 a45c  k..4.@.M.......\
-00005190: 699f f44d a30f cc48 e568 fed2 8e6d 0939  i..M...H.h...m.9
-000051a0: cfa9 861c c743 7daa 3815 c662 e5b2 3229  .....C}.8..b..2)
-000051b0: e228 d646 f9c9 f7e3 c9c5 7e76 f489 60db  .(.F......~v..`.
-000051c0: 2f6b 4558 9556 637e dfaf 1702 1bcc 0a73  /kEX.Vc~.......s
-000051d0: 8392 c336 6609 dbdc 44a0 9f85 4daa cc1c  ...6f...D...M...
-000051e0: e07a 15b8 6028 714b 9cf4 642b 3b1d 57f9  .z..`(qK..d+;.W.
-000051f0: a6a4 c9cf afc9 af93 f4ed 283d 1ccd 15a4  ..........(=....
-00005200: fbe3 5cf0 e1ec f7de f63f 04d9 d9eb cb8f  ..\......?......
-00005210: 07a5 ecea 7c9c 8c0e 2717 bb57 e76f e67e  ....|...'..W.o.~
-00005220: 32f9 f139 db3a 4a0f 5e5d 8ede cda7 7abf  2..9.:J.^]....z.
-00005230: 936c efa5 df76 b22f bbb7 c65a 2cca 0ee8  .l...v./...Z,...
-00005240: af91 3ce1 e285 5e8f db72 951a b8de f86c  ..<...^..r.....l
-00005250: 91b4 ba54 4160 8f64 7a11 d302 59b3 cb56  ...TA`.dz...Y..V
-00005260: 516e b2d2 a5a2 03c1 b5e6 7623 bfcf 8df2  Qn........v#....
-00005270: 11fa 8bf5 9a7b cfb5 a757 a911 7cf3 dcfc  .....{...W..|...
-00005280: 3f00 0000 ffff 0300 504b 0304 1400 0600  ?.......PK......
-00005290: 0800 0000 2100 b537 2dde 2901 0000 0c02  ....!..7-.).....
-000052a0: 0000 1300 0801 646f 6350 726f 7073 2f63  ......docProps/c
-000052b0: 7573 746f 6d2e 786d 6c20 a204 0128 a000  ustom.xml ...(..
-000052c0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-000052d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000052e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000052f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000050a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000050b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000050c0: 0000 0000 0000 0000 0000 0000 0000 9c93  ................
+000050d0: cb6e d340 1486 f748 bc83 35fb 66dc 8222  .n.@...H..5.f.."
+000050e0: 148d 5da1 16d4 0588 4849 bb1f c6c7 c908  ..].....HI......
+000050f0: 67c6 9a99 4609 cb22 94d0 022b ba6a 2bb5  g...F.."...+.j+.
+00005100: 486d 111b 3650 2e6a df26 36ee aaaf c0d8  Hm..6P.j.&6.....
+00005110: 5653 8746 2cd8 9dcb ef5f 9fcf 3943 9607  VS.F,...._..9C..
+00005120: bdc8 e983 d25c 0a0f 2dd6 5ce4 8060 32e0  .....\..-.\..`2.
+00005130: a2e3 a1f5 f6e3 8507 c8d1 868a 8046 5280  .............FR.
+00005140: 8786 a0d1 b27f f70e 692a 1983 321c b463  ........i*..2..c
+00005150: 2d84 f650 d798 b881 b166 5de8 515d b36d  -..P.....f].Q].m
+00005160: 613b a154 3d6a 6caa 3a58 8621 67b0 2ad9  a;.T=jl.:X.!g.*.
+00005170: 660f 84c1 4bae 5bc7 3030 2002 0816 e2a9  f...K.[.00 .....
+00005180: 212a 1d1b 7df3 bfa6 8164 399f de68 0f63  !*..}....d9..h.c
+00005190: 0bec 9387 711c 7146 8dfd 4bff 2967 4a6a  ....q.qF..K.)gJj
+000051a0: 191a e7d1 8041 4470 b549 2c5d 0bd8 a6e2  .....ADp.I,]....
+000051b0: 66e8 bb04 5753 d262 3482 156b ec87 34d2  f...WS.b4..k..4.
+000051c0: 40f0 4d81 ac01 cd87 d6a4 5c69 9ff4 4da3  @.M.......\i..M.
+000051d0: 0fcc 48e5 68fe d28e 6d09 39cf a986 1cc7  ..H.h...m.9.....
+000051e0: 437d aa38 15c6 62e5 b232 29e2 28d6 46f9  C}.8..b..2).(.F.
+000051f0: c9f7 e3c9 c57e 76f4 8960 db2f 6b45 5895  .....~v..`./kEX.
+00005200: 5663 7edf af17 021b cc0a 7383 92c3 3666  Vc~.......s...6f
+00005210: 09db dc44 a09f 854d aacc 1ce0 7a15 b860  ...D...M....z..`
+00005220: 2871 4b9c f464 2b3b 1d57 f9a6 a4c9 cfaf  (qK..d+;.W......
+00005230: c9af 93f4 ed28 3d1c cd15 a4fb e35c f0e1  .....(=......\..
+00005240: ecf7 def6 3f04 d9d9 ebcb 8f07 a5ec ea7c  ....?..........|
+00005250: 9c8c 0e27 17bb 57e7 6fe6 7e32 f9f1 39db  ...'..W.o.~2..9.
+00005260: 3a4a 0f5e 5d8e decd a77a bf93 6cef a5df  :J.^]....z..l...
+00005270: 76b2 2fbb b7c6 5a2c ca0e e8af 913c e1e2  v./...Z,.....<..
+00005280: 855e 8fdb 7295 1ab8 def8 6c91 b4ba 5441  .^..r.....l...TA
+00005290: 608f 647a 11d3 0259 b3cb 5651 6eb2 d2a5  `.dz...Y..VQn...
+000052a0: a203 c1b5 e676 23bf cf8d f211 fa8b f59a  .....v#.........
+000052b0: 7bcf b5a7 57a9 117c f3dc fc3f 0000 00ff  {...W..|...?....
+000052c0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+000052d0: 00b5 372d de29 0100 000c 0200 0013 0008  ..7-.)..........
+000052e0: 0164 6f63 5072 6f70 732f 6375 7374 6f6d  .docProps/custom
+000052f0: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
 00005300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000053c0: 00a4 9141 4bc3 3014 c7ef 82df 21e4 9e26  ...AK.0.....!..&
-000053d0: 4dd7 751d 6dc7 9a76 201e 149c bb97 34dd  M.u.m..v .....4.
-000053e0: 0a4d 5292 743a c4ef 6e86 cee1 c18b 1edf  .MR.t:..n.......
-000053f0: fb3f 7eef f778 d9ea 550e e028 8ced b5ca  .?~..x..U..(....
-00005400: 6118 1008 84e2 baed d53e 87cf db0d 5a40  a........>....Z@
-00005410: 605d a3da 66d0 4ae4 f024 2c5c 15b7 37d9  `]..f.J..$,\..7.
-00005420: a3d1 a330 ae17 1678 84b2 393c 3837 2e31  ...0...x..9<87.1
-00005430: b6fc 2064 6303 1f2b 9f74 dac8 c6f9 d2ec  .. dc..+.t......
-00005440: b1ee ba9e 8b4a f349 0ae5 3025 648e f964  .....J.I..0%d..d
-00005450: 9d96 68fc c6c1 4fde f2e8 fe8a 6c35 3fdb  ..h...O.....l5?.
-00005460: d9dd f634 7add 22fb 829f 4027 5ddf e6f0  ...4z."...@']...
-00005470: ad8a 5955 c524 46b4 4e19 0a49 58a2 344a  ..YU.$F.N..IX.4J
-00005480: 1344 1684 d092 b24d baae df21 18cf c314  .D.....M...!....
-00005490: 02d5 487f fafd d383 c7b6 1377 e5d4 0fed  ..H........w....
-000054a0: 4e18 8f3e bae5 30be 5867 0a4a 628a e280  N..>..0.Xg.Jb...
-000054b0: 0661 9024 e922 c3d7 28c3 1783 7fba 4417  .a.$."..(.....D.
-000054c0: 973b b6fb b17c 16cf c2a4 8ed6 e566 c62a  .;...|.......f.*
-000054d0: 5652 12b1 b0ac e794 b26a 5efb c66f 36f8  VR.......j^..o6.
-000054e0: fac6 e203 0000 ffff 0300 504b 0102 2d00  ..........PK..-.
-000054f0: 1400 0600 0800 0000 2100 bb97 352e bb01  ........!...5...
-00005500: 0000 7509 0000 1300 0000 0000 0000 0000  ..u.............
-00005510: 0000 0000 0000 0000 5b43 6f6e 7465 6e74  ........[Content
-00005520: 5f54 7970 6573 5d2e 786d 6c50 4b01 022d  _Types].xmlPK..-
-00005530: 0014 0006 0008 0000 0021 0013 5ebe 6502  .........!..^.e.
-00005540: 0100 00df 0200 000b 0000 0000 0000 0000  ................
-00005550: 0000 0000 00f4 0300 005f 7265 6c73 2f2e  ........._rels/.
-00005560: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00005570: 0000 2100 fc9a 79c6 cb03 0000 fe09 0000  ..!...y.........
-00005580: 0f00 0000 0000 0000 0000 0000 0000 2707  ..............'.
-00005590: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
-000055a0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000055b0: 000e 1564 c916 0100 007b 0500 001a 0000  ...d.....{......
-000055c0: 0000 0000 0000 0000 0000 001f 0b00 0078  ...............x
-000055d0: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
-000055e0: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
-000055f0: 0006 0008 0000 0021 0017 9da7 7635 0600  .......!....v5..
-00005600: 00e3 2600 0018 0000 0000 0000 0000 0000  ..&.............
-00005610: 0000 0075 0d00 0078 6c2f 776f 726b 7368  ...u...xl/worksh
-00005620: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
-00005630: 4b01 022d 0014 0006 0008 0000 0021 00cc  K..-.........!..
-00005640: e4d4 c2a3 0300 0046 0a00 0018 0000 0000  .......F........
-00005650: 0000 0000 0000 0000 00e0 1300 0078 6c2f  .............xl/
-00005660: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00005670: 322e 786d 6c50 4b01 022d 0014 0006 0008  2.xmlPK..-......
-00005680: 0000 0021 004d 3d34 677d 0300 00a9 0900  ...!.M=4g}......
-00005690: 0018 0000 0000 0000 0000 0000 0000 00b9  ................
-000056a0: 1700 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-000056b0: 2f73 6865 6574 332e 786d 6c50 4b01 022d  /sheet3.xmlPK..-
-000056c0: 0014 0006 0008 0000 0021 00c3 3a3c ca6e  .........!..:<.n
-000056d0: 0300 0093 0900 0018 0000 0000 0000 0000  ................
-000056e0: 0000 0000 006c 1b00 0078 6c2f 776f 726b  .....l...xl/work
-000056f0: 7368 6565 7473 2f73 6865 6574 342e 786d  sheets/sheet4.xm
-00005700: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00005710: 00f7 b383 0c24 0300 00d5 0700 0018 0000  .....$..........
-00005720: 0000 0000 0000 0000 0000 0010 1f00 0078  ...............x
-00005730: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00005740: 6574 352e 786d 6c50 4b01 022d 0014 0006  et5.xmlPK..-....
-00005750: 0008 0000 0021 0000 3194 dee5 0300 003b  .....!..1......;
-00005760: 0b00 0018 0000 0000 0000 0000 0000 0000  ................
-00005770: 006a 2200 0078 6c2f 776f 726b 7368 6565  .j"..xl/workshee
-00005780: 7473 2f73 6865 6574 362e 786d 6c50 4b01  ts/sheet6.xmlPK.
-00005790: 022d 0014 0006 0008 0000 0021 00e9 a625  .-.........!...%
-000057a0: b866 0600 0053 1b00 0013 0000 0000 0000  .f...S..........
-000057b0: 0000 0000 0000 0085 2600 0078 6c2f 7468  ........&..xl/th
-000057c0: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
-000057d0: 0102 2d00 1400 0600 0800 0000 2100 209e  ..-.........!. .
-000057e0: 4fe6 fa05 0000 ca21 0000 0d00 0000 0000  O......!........
-000057f0: 0000 0000 0000 0000 1c2d 0000 786c 2f73  .........-..xl/s
-00005800: 7479 6c65 732e 786d 6c50 4b01 022d 0014  tyles.xmlPK..-..
-00005810: 0006 0008 0000 0021 0088 b934 c7ff 0500  .......!...4....
-00005820: 0035 1c00 0014 0000 0000 0000 0000 0000  .5..............
-00005830: 0000 0041 3300 0078 6c2f 7368 6172 6564  ...A3..xl/shared
-00005840: 5374 7269 6e67 732e 786d 6c50 4b01 022d  Strings.xmlPK..-
-00005850: 0014 0006 0008 0000 0021 00fd 81bc be23  .........!.....#
-00005860: 0200 00cc 0400 0018 0000 0000 0000 0000  ................
-00005870: 0000 0000 0072 3900 0078 6c2f 6472 6177  .....r9..xl/draw
-00005880: 696e 6773 2f64 7261 7769 6e67 312e 786d  ings/drawing1.xm
-00005890: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000058a0: 00a1 a6aa e6ce 0700 0099 2200 0014 0000  ..........".....
-000058b0: 0000 0000 0000 0000 0000 00cb 3b00 0078  ............;..x
-000058c0: 6c2f 6368 6172 7473 2f63 6861 7274 312e  l/charts/chart1.
-000058d0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-000058e0: 0021 00a2 0807 919f 0400 0087 2600 0014  .!..........&...
-000058f0: 0000 0000 0000 0000 0000 0000 00cb 4300  ..............C.
-00005900: 0078 6c2f 6368 6172 7473 2f73 7479 6c65  .xl/charts/style
-00005910: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
-00005920: 0000 0021 001c 14a7 a8fd 0000 006e 0300  ...!.........n..
-00005930: 0015 0000 0000 0000 0000 0000 0000 009c  ................
-00005940: 4800 0078 6c2f 6368 6172 7473 2f63 6f6c  H..xl/charts/col
-00005950: 6f72 7331 2e78 6d6c 504b 0102 2d00 1400  ors1.xmlPK..-...
-00005960: 0600 0800 0000 2100 15af aa3c bd00 0000  ......!....<....
-00005970: 2b01 0000 2300 0000 0000 0000 0000 0000  +...#...........
-00005980: 0000 cc49 0000 786c 2f77 6f72 6b73 6865  ...I..xl/workshe
-00005990: 6574 732f 5f72 656c 732f 7368 6565 7431  ets/_rels/sheet1
-000059a0: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
-000059b0: 0006 0008 0000 0021 000e 44f4 dfbc 0000  .......!..D.....
-000059c0: 0025 0100 0023 0000 0000 0000 0000 0000  .%...#..........
-000059d0: 0000 00ca 4a00 0078 6c2f 6472 6177 696e  ....J..xl/drawin
-000059e0: 6773 2f5f 7265 6c73 2f64 7261 7769 6e67  gs/_rels/drawing
-000059f0: 312e 786d 6c2e 7265 6c73 504b 0102 2d00  1.xml.relsPK..-.
-00005a00: 1400 0600 0800 0000 2100 801b dc81 d200  ........!.......
-00005a10: 0000 8f01 0000 1f00 0000 0000 0000 0000  ................
-00005a20: 0000 0000 c74b 0000 786c 2f63 6861 7274  .....K..xl/chart
-00005a30: 732f 5f72 656c 732f 6368 6172 7431 2e78  s/_rels/chart1.x
-00005a40: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
-00005a50: 0008 0000 0021 00c0 6393 0250 0100 0065  .....!..c..P...e
-00005a60: 0200 0011 0000 0000 0000 0000 0000 0000  ................
-00005a70: 00d6 4c00 0064 6f63 5072 6f70 732f 636f  ..L..docProps/co
-00005a80: 7265 2e78 6d6c 504b 0102 2d00 1400 0600  re.xmlPK..-.....
-00005a90: 0800 0000 2100 d051 b373 f501 0000 b403  ....!..Q.s......
-00005aa0: 0000 1000 0000 0000 0000 0000 0000 0000  ................
-00005ab0: 5d4f 0000 646f 6350 726f 7073 2f61 7070  ]O..docProps/app
-00005ac0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00005ad0: 0000 2100 b537 2dde 2901 0000 0c02 0000  ..!..7-.).......
-00005ae0: 1300 0000 0000 0000 0000 0000 0000 8852  ...............R
-00005af0: 0000 646f 6350 726f 7073 2f63 7573 746f  ..docProps/custo
-00005b00: 6d2e 786d 6c50 4b05 0600 0000 0017 0017  m.xmlPK.........
-00005b10: 001b 0600 00ea 5400 0000 00              ......T....
+000053c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000053d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000053e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000053f0: 0000 0000 0000 0000 0000 0000 a491 414b  ..............AK
+00005400: c330 14c7 ef82 df21 e49e 264d d775 1d6d  .0.....!..&M.u.m
+00005410: c79a 7620 1e14 9cbb 9734 dd0a 4d52 9274  ..v .....4..MR.t
+00005420: 3ac4 ef6e 86ce e1c1 8b1e dffb 3f7e eff7  :..n........?~..
+00005430: 78d9 ea55 0ee0 288c edb5 ca61 1810 0884  x..U..(....a....
+00005440: e2ba edd5 3e87 cfdb 0d5a 4060 5da3 da66  ....>....Z@`]..f
+00005450: d04a e4f0 242c 5c15 b737 d9a3 d1a3 30ae  .J..$,\..7....0.
+00005460: 1716 7884 b239 3c38 372e 31b6 fc20 6463  ..x..9<87.1.. dc
+00005470: 031f 2b9f 74da c8c6 f9d2 ecb1 eeba 9e8b  ..+.t...........
+00005480: 4af3 490a e530 2564 8ef9 649d 9668 fcc6  J.I..0%d..d..h..
+00005490: c14f def2 e8fe 8a6c 353f dbd9 ddf6 347a  .O.....l5?....4z
+000054a0: dd22 fb82 9f40 275d dfe6 f0ad 8a59 55c5  ."...@'].....YU.
+000054b0: 2446 b44e 190a 4958 a234 4a13 4416 84d0  $F.N..IX.4J.D...
+000054c0: 92b2 4dba aedf 2118 cfc3 1402 d548 7ffa  ..M...!......H..
+000054d0: fdd3 83c7 b613 77e5 d40f ed4e 188f 3eba  ......w....N..>.
+000054e0: e530 be58 670a 4a62 8ae2 8006 6190 24e9  .0.Xg.Jb....a.$.
+000054f0: 22c3 d728 c317 837f ba44 1797 3bb6 fbb1  "..(.....D..;...
+00005500: 7c16 cfc2 a48e d6e5 66c6 2a56 5212 b1b0  |.......f.*VR...
+00005510: ace7 94b2 6a5e fbc6 6f36 f8fa c6e2 0300  ....j^..o6......
+00005520: 00ff ff03 0050 4b01 022d 0014 0006 0008  .....PK..-......
+00005530: 0000 0021 00bb 9735 2ebb 0100 0075 0900  ...!...5.....u..
+00005540: 0013 0000 0000 0000 0000 0000 0000 0000  ................
+00005550: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
+00005560: 735d 2e78 6d6c 504b 0102 2d00 1400 0600  s].xmlPK..-.....
+00005570: 0800 0000 2100 135e be65 0201 0000 df02  ....!..^.e......
+00005580: 0000 0b00 0000 0000 0000 0000 0000 0000  ................
+00005590: f403 0000 5f72 656c 732f 2e72 656c 7350  ...._rels/.relsP
+000055a0: 4b01 022d 0014 0006 0008 0000 0021 0088  K..-.........!..
+000055b0: e43b c8ce 0300 00fe 0900 000f 0000 0000  .;..............
+000055c0: 0000 0000 0000 0000 0027 0700 0078 6c2f  .........'...xl/
+000055d0: 776f 726b 626f 6f6b 2e78 6d6c 504b 0102  workbook.xmlPK..
+000055e0: 2d00 1400 0600 0800 0000 2100 0e15 64c9  -.........!...d.
+000055f0: 1601 0000 7b05 0000 1a00 0000 0000 0000  ....{...........
+00005600: 0000 0000 0000 220b 0000 786c 2f5f 7265  ......"...xl/_re
+00005610: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
+00005620: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
+00005630: 0000 2100 179d a776 3506 0000 e326 0000  ..!....v5....&..
+00005640: 1800 0000 0000 0000 0000 0000 0000 780d  ..............x.
+00005650: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00005660: 7368 6565 7431 2e78 6d6c 504b 0102 2d00  sheet1.xmlPK..-.
+00005670: 1400 0600 0800 0000 2100 863f a2e2 c003  ........!..?....
+00005680: 0000 eb0a 0000 1800 0000 0000 0000 0000  ................
+00005690: 0000 0000 e313 0000 786c 2f77 6f72 6b73  ........xl/works
+000056a0: 6865 6574 732f 7368 6565 7432 2e78 6d6c  heets/sheet2.xml
+000056b0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+000056c0: 4d3d 3467 7d03 0000 a909 0000 1800 0000  M=4g}...........
+000056d0: 0000 0000 0000 0000 0000 d917 0000 786c  ..............xl
+000056e0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+000056f0: 7433 2e78 6d6c 504b 0102 2d00 1400 0600  t3.xmlPK..-.....
+00005700: 0800 0000 2100 c33a 3cca 6e03 0000 9309  ....!..:<.n.....
+00005710: 0000 1800 0000 0000 0000 0000 0000 0000  ................
+00005720: 8c1b 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00005730: 732f 7368 6565 7434 2e78 6d6c 504b 0102  s/sheet4.xmlPK..
+00005740: 2d00 1400 0600 0800 0000 2100 f7b3 830c  -.........!.....
+00005750: 2403 0000 d507 0000 1800 0000 0000 0000  $...............
+00005760: 0000 0000 0000 301f 0000 786c 2f77 6f72  ......0...xl/wor
+00005770: 6b73 6865 6574 732f 7368 6565 7435 2e78  ksheets/sheet5.x
+00005780: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00005790: 2100 0031 94de e503 0000 3b0b 0000 1800  !..1......;.....
+000057a0: 0000 0000 0000 0000 0000 0000 8a22 0000  ............."..
+000057b0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000057c0: 6565 7436 2e78 6d6c 504b 0102 2d00 1400  eet6.xmlPK..-...
+000057d0: 0600 0800 0000 2100 e9a6 25b8 6606 0000  ......!...%.f...
+000057e0: 531b 0000 1300 0000 0000 0000 0000 0000  S...............
+000057f0: 0000 a526 0000 786c 2f74 6865 6d65 2f74  ...&..xl/theme/t
+00005800: 6865 6d65 312e 786d 6c50 4b01 022d 0014  heme1.xmlPK..-..
+00005810: 0006 0008 0000 0021 0020 9e4f e6fa 0500  .......!. .O....
+00005820: 00ca 2100 000d 0000 0000 0000 0000 0000  ..!.............
+00005830: 0000 003c 2d00 0078 6c2f 7374 796c 6573  ...<-..xl/styles
+00005840: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00005850: 0000 2100 737a 97f5 1806 0000 411d 0000  ..!.sz......A...
+00005860: 1400 0000 0000 0000 0000 0000 0000 6133  ..............a3
+00005870: 0000 786c 2f73 6861 7265 6453 7472 696e  ..xl/sharedStrin
+00005880: 6773 2e78 6d6c 504b 0102 2d00 1400 0600  gs.xmlPK..-.....
+00005890: 0800 0000 2100 fd81 bcbe 2302 0000 cc04  ....!.....#.....
+000058a0: 0000 1800 0000 0000 0000 0000 0000 0000  ................
+000058b0: ab39 0000 786c 2f64 7261 7769 6e67 732f  .9..xl/drawings/
+000058c0: 6472 6177 696e 6731 2e78 6d6c 504b 0102  drawing1.xmlPK..
+000058d0: 2d00 1400 0600 0800 0000 2100 a1a6 aae6  -.........!.....
+000058e0: ce07 0000 9922 0000 1400 0000 0000 0000  ....."..........
+000058f0: 0000 0000 0000 043c 0000 786c 2f63 6861  .......<..xl/cha
+00005900: 7274 732f 6368 6172 7431 2e78 6d6c 504b  rts/chart1.xmlPK
+00005910: 0102 2d00 1400 0600 0800 0000 2100 a208  ..-.........!...
+00005920: 0791 9f04 0000 8726 0000 1400 0000 0000  .......&........
+00005930: 0000 0000 0000 0000 0444 0000 786c 2f63  .........D..xl/c
+00005940: 6861 7274 732f 7374 796c 6531 2e78 6d6c  harts/style1.xml
+00005950: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00005960: 1c14 a7a8 fd00 0000 6e03 0000 1500 0000  ........n.......
+00005970: 0000 0000 0000 0000 0000 d548 0000 786c  ...........H..xl
+00005980: 2f63 6861 7274 732f 636f 6c6f 7273 312e  /charts/colors1.
+00005990: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+000059a0: 0021 0015 afaa 3cbd 0000 002b 0100 0023  .!....<....+...#
+000059b0: 0000 0000 0000 0000 0000 0000 0005 4a00  ..............J.
+000059c0: 0078 6c2f 776f 726b 7368 6565 7473 2f5f  .xl/worksheets/_
+000059d0: 7265 6c73 2f73 6865 6574 312e 786d 6c2e  rels/sheet1.xml.
+000059e0: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
+000059f0: 0000 2100 0e44 f4df bc00 0000 2501 0000  ..!..D......%...
+00005a00: 2300 0000 0000 0000 0000 0000 0000 034b  #..............K
+00005a10: 0000 786c 2f64 7261 7769 6e67 732f 5f72  ..xl/drawings/_r
+00005a20: 656c 732f 6472 6177 696e 6731 2e78 6d6c  els/drawing1.xml
+00005a30: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00005a40: 0000 0021 0080 1bdc 81d2 0000 008f 0100  ...!............
+00005a50: 001f 0000 0000 0000 0000 0000 0000 0000  ................
+00005a60: 4c00 0078 6c2f 6368 6172 7473 2f5f 7265  L..xl/charts/_re
+00005a70: 6c73 2f63 6861 7274 312e 786d 6c2e 7265  ls/chart1.xml.re
+00005a80: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00005a90: 2100 eb75 717c 5201 0000 6502 0000 1100  !..uq|R...e.....
+00005aa0: 0000 0000 0000 0000 0000 0000 0f4d 0000  .............M..
+00005ab0: 646f 6350 726f 7073 2f63 6f72 652e 786d  docProps/core.xm
+00005ac0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00005ad0: 00d0 51b3 73f5 0100 00b4 0300 0010 0000  ..Q.s...........
+00005ae0: 0000 0000 0000 0000 0000 0098 4f00 0064  ............O..d
+00005af0: 6f63 5072 6f70 732f 6170 702e 786d 6c50  ocProps/app.xmlP
+00005b00: 4b01 022d 0014 0006 0008 0000 0021 00b5  K..-.........!..
+00005b10: 372d de29 0100 000c 0200 0013 0000 0000  7-.)............
+00005b20: 0000 0000 0000 0000 00c3 5200 0064 6f63  ..........R..doc
+00005b30: 5072 6f70 732f 6375 7374 6f6d 2e78 6d6c  Props/custom.xml
+00005b40: 504b 0506 0000 0000 1700 1700 1b06 0000  PK..............
+00005b50: 2555 0000 0000                           %U....
```

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 import datetime
 from collections import defaultdict
+from copy import copy
 from rqalpha.const import MATCHING_TYPE, ORDER_TYPE, POSITION_EFFECT, SIDE
 from rqalpha.environment import Environment
 from rqalpha.core.events import EVENT, Event
 from rqalpha.model.order import Order, ALGO_ORDER_STYLES
 from rqalpha.model.trade import Trade
 from rqalpha.model.tick import TickObject
 from rqalpha.portfolio.account import Account
@@ -127,15 +128,15 @@
                 # 撮合的时候无行情数据也不需要撤单，等到有行情再撮合
                 reason = None
                 # reason = _(u"Order Cancelled: current bar [{order_book_id}] miss market data.").format(
                 #     order_book_id=order.order_book_id)
             if reason:
                 order.mark_rejected(reason)
             return
-
+        
         price_board = self._env.price_board
         if order.type == ORDER_TYPE.LIMIT:
             if order.side == SIDE.BUY and order.price < deal_price:
                 return
             if order.side == SIDE.SELL and order.price > deal_price:
                 return
             # 是否限制涨跌停不成交
@@ -204,14 +205,26 @@
             position_effect=order.position_effect,
             order_book_id=order.order_book_id,
             frozen_price=order.frozen_price,
             close_today_amount=ct_amount
         )
         trade._commission = self._env.get_trade_commission(trade)
         trade._tax = self._env.get_trade_tax(trade)
+
+        if order.side == SIDE.BUY and self._slippage_decider.decider.rate != 0:
+            # 标的价格经过滑点处理后，账户资金可能不够买入，需要进行验证
+            cost_money = instrument.calc_cash_occupation(price, order.quantity, order.position_direction, order.trading_datetime.date())
+            cost_money += trade.transaction_cost
+            if cost_money > account.cash + order.init_frozen_cash:
+                reason = _(u"Order Cancelled: not enough money to buy {order_book_id}, needs {cost_money:.2f}, cash {cash:.2f}").format(
+                        order_book_id=order_book_id, cost_money=cost_money, cash = account.cash + order.init_frozen_cash
+                        )
+                order.mark_rejected(reason)
+                return
+
         order.fill(trade)
         self._turnover[order.order_book_id] += fill
 
         self._env.event_bus.publish_event(Event(EVENT.TRADE, account=account, trade=trade, order=order))
 
         if order.type == ORDER_TYPE.MARKET and order.unfilled_quantity != 0:
             reason = _(
@@ -340,14 +353,20 @@
                 )
             else:
                 # TODO：这里报错信息比较模糊，可以根据撮合类型给出更明确的提示，比如是否是熔断了，是否是涨跌停了
                 reason = _(u"Order Cancelled: current tick [{order_book_id}] miss market data.").format(
                     order_book_id=order.order_book_id)
             order.mark_rejected(reason)
             return
+        
+        # 对价格进行滑点处理
+        if instrument.during_call_auction(self._env.calendar_dt):
+            price = deal_price
+        else:
+            price = self._slippage_decider.get_trade_price(order, deal_price)
 
         price_board = self._env.price_board
         if order.type == ORDER_TYPE.LIMIT:
             if order.side == SIDE.BUY and order.price < deal_price:
                 return
             if order.side == SIDE.SELL and order.price > deal_price:
                 return
@@ -430,33 +449,38 @@
         else:
             # 下单数量就是成交数量
             fill = order.unfilled_quantity
 
         # 平今的数量
         ct_amount = account.calc_close_today_amount(order_book_id, fill, order.position_direction, order.position_effect)
 
-        # 对价格进行滑点处理
-        if instrument.during_call_auction(self._env.calendar_dt):
-            price = deal_price
-        else:
-            price = self._slippage_decider.get_trade_price(order, deal_price)
-
         # 成交记录
         trade = Trade.__from_create__(
             order_id=order.order_id,
             price=price,
             amount=fill,
             side=order.side,
             position_effect=order.position_effect,
             order_book_id=order.order_book_id,
             frozen_price=order.frozen_price,
             close_today_amount=ct_amount
         )
         trade._commission = self._env.get_trade_commission(trade)
         trade._tax = self._env.get_trade_tax(trade)
+
+        if order.side == SIDE.BUY and self._slippage_decider.decider.rate != 0:
+            cost_money = instrument.calc_cash_occupation(price, order.quantity, order.position_direction, order.trading_datetime.date())
+            cost_money += trade.transaction_cost
+            if cost_money > account.cash + order.init_frozen_cash:
+                reason = _(u"Order Cancelled: not enough money to buy {order_book_id}, needs {cost_money:.2f}, cash {cash:.2f}").format(
+                        order_book_id=order_book_id, cost_money=cost_money, cash=account.cash + order.init_frozen_cash
+                    )
+                order.mark_rejected(reason)
+                return
+
         order.fill(trade)
         self._turnover[order.order_book_id] += fill
 
         self._env.event_bus.publish_event(Event(EVENT.TRADE, account=account, trade=trade, order=order))
 
         if order.type == ORDER_TYPE.MARKET and order.unfilled_quantity != 0:
             reason = _(
```

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-5.4.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/mod/utils.py` & `rqalpha-5.4.0/rqalpha/mod/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/model/__init__.py` & `rqalpha-5.4.0/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/model/bar.py` & `rqalpha-5.4.0/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/model/instrument.py` & `rqalpha-5.4.0/rqalpha/model/instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,17 @@
             year, month, day = ds.split('-')
             return datetime.datetime(int(year), int(month), int(day))
         except:
             return parse(ds)
 
     __repr__ = property_repr
 
-    def __init__(self, dic, futures_tick_size_getter=None, futures_long_margin_ratio_getter=None, futures_short_margin_ratio_getter=None):
-        # type: (Dict, Optional[Callable[[Instrument], float]], Optional[Callable[[Instrument], float]], Optional[Callable[[Instrument], float]]) -> None
+    def __init__(self, dic: Dict, futures_tick_size_getter: Optional[Callable] = None, *args, **kwrags) -> None:
         self.__dict__ = copy.copy(dic)
         self._futures_tick_size_getter = futures_tick_size_getter
-        self._futures_long_margin_ratio_getter = futures_long_margin_ratio_getter
-        self._futures_short_margin_ratio_getter = futures_short_margin_ratio_getter
 
         if "listed_date" in dic:
             self.__dict__["listed_date"] = self._fix_date(dic["listed_date"])
         if "de_listed_date" in dic:
             self.__dict__["de_listed_date"] = self._fix_date(dic["de_listed_date"], self.DEFAULT_DE_LISTED_DATE)
         if "maturity_date" in self.__dict__:
             self.__dict__["maturity_date"] = self._fix_date(dic["maturity_date"], self.DEFAULT_DE_LISTED_DATE)
@@ -442,28 +439,26 @@
             return 0.001
         elif self.type == INSTRUMENT_TYPE.FUTURE:
             return self._futures_tick_size_getter(self)
         else:
             raise NotImplementedError
 
     @lru_cache(8)
-    def get_long_margin_ratio(self, dt):
-        # type: (datetime.date) -> float
+    def get_long_margin_ratio(self, dt: datetime.date) -> float:
         """
         获取多头保证金率（期货专用）
         """
-        return self._futures_long_margin_ratio_getter(self, dt)
+        return Environment.get_instance().data_proxy.get_futures_trading_parameters(self.order_book_id, dt).long_margin_ratio
 
     @lru_cache(8)
-    def get_short_margin_ratio(self, dt):
-        # type: (datetime.date) -> float
+    def get_short_margin_ratio(self, dt: datetime.date) -> float:
         """
         获取空头保证金率（期货专用）
         """
-        return self._futures_short_margin_ratio_getter(self, dt)
+        return Environment.get_instance().data_proxy.get_futures_trading_parameters(self.order_book_id, dt).short_margin_ratio
 
     def calc_cash_occupation(self, price, quantity, direction, dt):
         # type: (float, int, POSITION_DIRECTION, datetime.date) -> float
         if self.type in INST_TYPE_IN_STOCK_ACCOUNT:
             return price * quantity
         elif self.type == INSTRUMENT_TYPE.FUTURE:
             margin_multiplier = Environment.get_instance().config.base.margin_multiplier
```

### Comparing `rqalpha-5.3.9/rqalpha/model/order.py` & `rqalpha-5.4.0/rqalpha/model/order.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/model/tick.py` & `rqalpha-5.4.0/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/model/trade.py` & `rqalpha-5.4.0/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/portfolio/__init__.py` & `rqalpha-5.4.0/rqalpha/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/portfolio/account.py` & `rqalpha-5.4.0/rqalpha/portfolio/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,18 @@
 
         self._backward_trade_set.clear()
 
         fee = self._management_fee()
         self._management_fees += fee
         self._total_cash -= fee
 
+        # 如果期货结算结束时 cash 为负数，抛出提醒给到用户
+        if self._type == "FUTURE" and self.cash < 0:
+            user_system_log.warn(_("Futures account's cash turns negative after settlement"))
+
         # 如果 total_value <= 0 则认为已爆仓，清空仓位，资金归0
         forced_liquidation = self._env.config.base.forced_liquidation
         if self.total_value <= 0 and forced_liquidation:
             if self._positions:
                 user_system_log.warn(_("Trigger Forced Liquidation, current total_value is 0"))
             self._positions.clear()
             self._total_cash = 0
```

### Comparing `rqalpha-5.3.9/rqalpha/portfolio/position.py` & `rqalpha-5.4.0/rqalpha/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/resource/ricequant-logo.png` & `rqalpha-5.4.0/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/user_module.py` & `rqalpha-5.4.0/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/__init__.py` & `rqalpha-5.4.0/rqalpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/arg_checker.py` & `rqalpha-5.4.0/rqalpha/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/class_helper.py` & `rqalpha-5.4.0/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/click_helper.py` & `rqalpha-5.4.0/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/concurrent.py` & `rqalpha-5.4.0/rqalpha/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/config.py` & `rqalpha-5.4.0/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/datetime_func.py` & `rqalpha-5.4.0/rqalpha/utils/datetime_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/dict_func.py` & `rqalpha-5.4.0/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/exception.py` & `rqalpha-5.4.0/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/functools.py` & `rqalpha-5.4.0/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/i18n.py` & `rqalpha-5.4.0/rqalpha/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/log_capture.py` & `rqalpha-5.4.0/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/logger.py` & `rqalpha-5.4.0/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/package_helper.py` & `rqalpha-5.4.0/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/persisit_helper.py` & `rqalpha-5.4.0/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/repr.py` & `rqalpha-5.4.0/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/risk_free_helper.py` & `rqalpha-5.4.0/rqalpha/utils/risk_free_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/rq_json.py` & `rqalpha-5.4.0/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/strategy_loader_help.py` & `rqalpha-5.4.0/rqalpha/utils/strategy_loader_help.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/testing/__init__.py` & `rqalpha-5.4.0/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/testing/fixtures.py` & `rqalpha-5.4.0/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/testing/mocking.py` & `rqalpha-5.4.0/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/translations/__init__.py` & `rqalpha-5.4.0/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-12 15:23+0800\n"
+"POT-Creation-Date: 2024-05-15 14:39+0800\n"
 "PO-Revision-Date: 2016-10-24 21:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -128,18 +128,16 @@
 msgstr ""
 "{} 文件更新失败，如果其正在使用中，请稍后再进行更新，或者您可以将其删除后再重"
 "新更新"
 
 msgid "Frequency {} is not support."
 msgstr "不支持回测频率: {}"
 
-msgid ""
-"Futures historical trading parameters data is being updated, please "
-"wait......"
-msgstr "正在更新期货历史交易参数，请稍后......"
+msgid "Futures account's cash turns negative after settlement"
+msgstr "期货账户的现金在结算后变为负数"
 
 msgid "Generate default config file"
 msgstr "生成默认的配置文件"
 
 msgid "Generate example strategies to target folder"
 msgstr "在目标文件夹生成样例策略"
 
@@ -240,14 +238,21 @@
 "Order Cancelled: market order {order_book_id} volume {order_volume} is "
 "larger than {volume_percent_limit} percent of current bar volume, fill "
 "{filled_volume} actually"
 msgstr ""
 "{order_book_id} 下单量 {order_volume} 超过当前 Bar 成交量的 "
 "{volume_percent_limit}%，实际成交 {filled_volume}"
 
+msgid ""
+"Order Cancelled: not enough money to buy {order_book_id}, needs "
+"{cost_money:.2f}, cash {cash:.2f}"
+msgstr ""
+"订单创建失败: 可用资金不足。当前资金: {cash:.2f}，{order_book_id} 下单所需资"
+"金: {cost_money:.2f}"
+
 msgid "Order Cancelled: {order_book_id} bar no volume"
 msgstr "订单被撤销：{order_book_id} 当前无成交量"
 
 msgid "Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
 msgstr "{order_book_id} 的订单创建失败：下单数量为 0"
 
 msgid "Order Creation Failed: [{order_book_id}] No market data"
@@ -300,49 +305,32 @@
 
 msgid "Output Version Info"
 msgstr "输出版本号信息"
 
 msgid "ProfitLossRate"
 msgstr "盈亏比"
 
-msgid ""
-"RQAlpha already supports backtesting using futures historical margins and "
-"rates, please upgrade RQDatac to version 2.11.12 and above to use it"
-msgstr ""
-"RQAlpha 已支持使用期货历史保证金和费率进行回测，请将 RQDatac 升级至 2.11.12 "
-"及以上版本进行使用"
-
-msgid ""
-"RQDatac does not have permission to obtain futures histrical trading "
-"parameters, \"config.base.futures_time_series_trading_parameters\" will be "
-"disabled."
-msgstr ""
-"RQDatac 缺少获取期货历史交易参数的权限，将关闭配置 \"config.base."
-"futures_time_series_trading_parameters\""
-
-msgid ""
-"RQDatac is not installed, \"config.base."
-"futures_time_series_trading_parameters\" will be disabled."
-msgstr ""
-"未安装 RQDatac，将关闭配置 \"config.base."
-"futures_time_series_trading_parameters\""
-
 msgid "Run a strategy"
 msgstr "运行策略"
 
 msgid "Sharpe"
 msgstr "夏普率"
 
 msgid "Sortino"
 msgstr "索提诺比率"
 
 msgid "Strategy"
 msgstr "策略收益"
 
 msgid ""
+"The bundle data you are using is too old, please update it to lastest before "
+"using"
+msgstr "您所使用的 Bundle 数据过旧，请将其更新至最新后再进行使用"
+
+msgid ""
 "There is no data between {start_date} and {end_date}. Please check your data "
 "bundle or select other backtest period."
 msgstr ""
 "未在 {start_date} 和 {end_date} 区间内查询到数据，请检查并升级您的 data "
 "bundle 或者选择其他回测区间。"
 
 msgid "TotalReturns"
@@ -401,21 +389,14 @@
 
 msgid "WinRate"
 msgstr "胜率"
 
 msgid "You cannot call %s when executing %s"
 msgstr "%s 不能在 %s 中调用。"
 
-msgid ""
-"Your bundle data is too old, please use 'rqalpha update-bundle' or 'rqalpha "
-"download-bundle' to update it to lastest before using"
-msgstr ""
-"您的 Bundle 数据过旧，请使用 'rqalpha update-bundle' 或 'rqalpha download-"
-"bundle' 将其更新至最新后再进行使用"
-
 msgid "[sys_analyser] Generate report from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件生成报告"
 
 msgid "[sys_analyser] Plot from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件绘制收益图"
 
 msgid ""
```

### Comparing `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-12 15:23+0800\n"
+"POT-Creation-Date: 2024-05-15 14:39+0800\n"
 "PO-Revision-Date: 2016-10-24 21:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -72,16 +72,16 @@
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:62
 msgid "Index Future contracts[99] are not supported in paper trading."
 msgstr "期货指数连续合约[99] 在实盘模拟中暂不支持。"
 
 #: rqalpha/apis/api_base.py:173
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:66
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:103
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:140
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:343
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:141
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:344
 msgid "Order Creation Failed: [{order_book_id}] No market data"
 msgstr "订单创建失败: 当前合约[{order_book_id}]没有市场数据。"
 
 #: rqalpha/apis/api_rqdatac.py:50
 msgid "rqdatac is not available, extension apis will not function properly"
 msgstr ""
 "rqdatac 不存在，扩展 API 无法使用，您可以访问 https://www.ricequant.com/welcome/rqdata 获取"
@@ -259,54 +259,26 @@
 msgid "not run {}({}, {}) because strategy is hold"
 msgstr "策略暂停中，取消执行 {}({}, {})"
 
 #: rqalpha/core/strategy.py:53
 msgid "deprecated parameter[bar_dict] in before_trading function."
 msgstr "[Deprecated]在before_trading函数中，第二个参数bar_dict已经不再使用了。"
 
-#: rqalpha/data/bundle.py:460
-msgid ""
-"RQAlpha already supports backtesting using futures historical margins and"
-" rates, please upgrade RQDatac to version 2.11.12 and above to use it"
-msgstr "RQAlpha 已支持使用期货历史保证金和费率进行回测，请将 RQDatac 升级至 2.11.12 及以上版本进行使用"
-
-#: rqalpha/data/bundle.py:470 rqalpha/data/bundle.py:531
-msgid ""
-"Futures historical trading parameters data is being updated, please "
-"wait......"
-msgstr "正在更新期货历史交易参数，请稍后......"
-
-#: rqalpha/data/bundle.py:522 rqalpha/data/bundle.py:706
+#: rqalpha/data/bundle.py:522
 msgid ""
 "File {} update failed, if it is using, please update later, or you can "
 "delete then update again"
 msgstr "{} 文件更新失败，如果其正在使用中，请稍后再进行更新，或者您可以将其删除后再重新更新"
 
-#: rqalpha/data/base_data_source/data_source.py:140
-msgid ""
-"RQDatac is not installed, "
-"\"config.base.futures_time_series_trading_parameters\" will be disabled."
-msgstr "未安装 RQDatac，将关闭配置 \"config.base.futures_time_series_trading_parameters\""
-
-#: rqalpha/data/base_data_source/data_source.py:145
-msgid ""
-"RQDatac does not have permission to obtain futures histrical trading "
-"parameters, \"config.base.futures_time_series_trading_parameters\" will "
-"be disabled."
-msgstr ""
-"RQDatac 缺少获取期货历史交易参数的权限，将关闭配置 "
-"\"config.base.futures_time_series_trading_parameters\""
-
 #: rqalpha/data/base_data_source/storages.py:81
 msgid ""
-"Your bundle data is too old, please use 'rqalpha update-bundle' or "
-"'rqalpha download-bundle' to update it to lastest before using"
+"The bundle data you are using is too old, please update it to lastest "
+"before using"
 msgstr ""
-"您的 Bundle 数据过旧，请使用 'rqalpha update-bundle' 或 'rqalpha download-bundle' "
-"将其更新至最新后再进行使用"
+"您所使用的 Bundle 数据过旧，请将其更新至最新后再进行使用"
 
 #: rqalpha/data/base_data_source/storages.py:97
 #: rqalpha/data/base_data_source/storages.py:124
 msgid "unsupported future instrument {}"
 msgstr "不支持的期货标的{}"
 
 #: rqalpha/data/base_data_source/storages.py:195
@@ -353,16 +325,16 @@
 msgid ""
 "Order Creation Failed: not enough position {order_book_id} to close or "
 "exercise, target sell quantity is {quantity}, closable quantity is "
 "{closable}"
 msgstr "订单创建失败：{order_book_id} 的仓位不足，目标平仓/行权量为 {quantity}，可平仓/行权量为 {closable}"
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:50
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:112
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:157
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:113
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:158
 msgid "Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
 msgstr "{order_book_id} 的订单创建失败：下单数量为 0"
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py:56
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:100
 msgid "Limit order price should not be nan."
 msgstr "限价单价格不能为 nan。"
@@ -387,50 +359,50 @@
 
 #: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:66
 msgid ""
 "order_book_id: {order_book_id} needs stock account, please set and try "
 "again!"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:119
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:120
 msgid "insufficient cash, use all remaining cash({}) to create order"
 msgstr "现金不足，使用当前剩余资金({})创建订单"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:332
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:333
 #, fuzzy
 msgid ""
 "function order_target_portfolio: invalid keys of target_portfolio, "
 "expected order_book_ids or Instrument objects, got {} (type: {})"
 msgstr ""
 "函数 order_target_portfolio：不合法的参数。target_portfolio 的键应为合约代码或 Instrument "
 "对象，实际传入了 {}（类型：{}）。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:337
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:338
 msgid ""
 "function order_target_portfolio: invalid instrument type, excepted "
 "CS/ETF/LOF/INDX, got {}"
 msgstr "函数 order_target_portfolio：不合法的资产类型。应传入股票、ETF、LOF 或指数，实际传入了 {}。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:351
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:352
 msgid ""
 "function order_target_portfolio: invalid values of target_portfolio, "
 "excepted float between 0 and 1, got {} (key: {})"
 msgstr "函数 order_target_portfolio：不合法的目标权重，应传入 0 和 1 之间的浮点数，实际传入了 {}（类型：{}）。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:360
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:361
 msgid "total percent should be lower than 1, current: {}"
 msgstr "目标持仓占比总和应小于 1，当前值：{}。"
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:380
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:381
 msgid ""
 "Adjust position of {id_or_ins} Failed: Invalid close/open price "
 "{close_price}/{open_price}"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:693
+#: rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py:694
 msgid "in get_dividend, start_date {} is later than the previous test day {}"
 msgstr "在 get_dividend 函数中，start_date {} 晚于当前回测时间的上一个交易日 {}。"
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py:66
 msgid "[sys_analyser] save report"
 msgstr ""
 
@@ -474,39 +446,39 @@
 msgid "show weekly indicators and return curve on plot"
 msgstr ""
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py:115
 msgid "[sys_analyser] Generate report from strategy output file"
 msgstr "【sys_analyser】使用策略输出的文件生成报告"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:113
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:111
 msgid ""
 "config 'base.benchmark' is deprecated, use 'mod.sys_analyser.benchmark' "
 "instead"
 msgstr "配置'base.benchmark'已被弃用，使用'mod.sys_analyser.benchmark'代替"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:151
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:149
 msgid "benchmark {} not exists, please entry correct order_book_id"
 msgstr "基准标的 {} 信息不存在，请输入正确的标的代码"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:163
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:161
 msgid "benchmark {} missing data between backtest start date {} and end date {}"
 msgstr "基准标的 {} 在回测起始日期 {} 结束日期 {} 间缺失数据"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:175
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:173
 msgid ""
-"benchmark {} available data start date {} >= backtest start date {} or end"
-" date {} <= backtest end date {}"
+"benchmark {} available data start date {} >= backtest start date {} or "
+"end date {} <= backtest end date {}"
 msgstr "基准标的 {} 的可用行情数据开始日期 {} >= 回测起始日期 {} 或结束日期 {} <= 回测结束日期 {}"
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:243
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:241
 msgid "invalid init benchmark {}, should be in format 'order_book_id:weight'"
 msgstr ""
 
-#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:248
+#: rqalpha/mod/rqalpha_mod_sys_analyser/mod.py:246
 msgid "invalid weight for instrument {order_book_id}: {weight}"
 msgstr ""
 
 #: rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py:60
 msgid "Strategy"
 msgstr "策略收益"
 
@@ -740,85 +712,92 @@
 
 #: rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py:34
 msgid ""
 "Create order failed, there are active orders leading to the risk of self-"
 "trade: [{}...]"
 msgstr "订单创建失败，当前存在可能导致自成交的挂单：[{}...]"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:118
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:335
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:119
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:348
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:69
 msgid ""
 "Order Cancelled: current security [{order_book_id}] can not be traded in "
 "listed date [{listed_date}]"
 msgstr "订单被撤销: [{order_book_id}] 上市首日无法交易"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:125
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:165
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:126
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:166
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:86
 msgid "Order Cancelled: {order_book_id} bar no volume"
 msgstr "订单被撤销：{order_book_id} 当前无成交量"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:150
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:151
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:95
 msgid "Order Cancelled: current bar [{order_book_id}] reach the limit_up price."
 msgstr "订单被拒单: [{order_book_id}] 已涨停。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:156
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:157
 #: rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py:104
 msgid "Order Cancelled: current bar [{order_book_id}] reach the limit_down price."
 msgstr "订单被拒单: [{order_book_id}] 已跌停。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:178
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:417
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:567
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:179
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:436
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:591
 msgid ""
 "Order Cancelled: market order {order_book_id} volume {order_volume} due "
 "to volume limit"
 msgstr "订单被撤销: 订单 [{order_book_id}] 的下单量 {order_volume} 超过了成交量限制。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:217
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:218
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:474
+msgid ""
+"Order Cancelled: not enough money to buy {order_book_id}, needs "
+"{cost_money:.2f}, cash {cash:.2f}"
+msgstr "订单创建失败: 可用资金不足。当前资金: {cash:.2f}，{order_book_id} 下单所需资金: {cost_money:.2f}"
+
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:230
 msgid ""
 "Order Cancelled: market order {order_book_id} volume {order_volume} is "
 "larger than {volume_percent_limit} percent of current bar volume, fill "
 "{filled_volume} actually"
 msgstr ""
 "{order_book_id} 下单量 {order_volume} 超过当前 Bar 成交量的 "
 "{volume_percent_limit}%，实际成交 {filled_volume}"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:343
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:356
 msgid "Order Cancelled: current tick [{order_book_id}] miss market data."
 msgstr "订单被拒单: [{order_book_id}] 当前缺失市场数据。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:368
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:387
 msgid "Order Cancelled: current tick [{order_book_id}] reach the limit_up price."
 msgstr "订单被拒单: [{order_book_id}] 已涨停。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:374
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:393
 msgid ""
 "Order Cancelled: current tick [{order_book_id}] reach the limit_down "
 "price."
 msgstr "订单被拒单: [{order_book_id}] 已跌停。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:381
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:387
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:400
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:406
 msgid "Order Cancelled: [{order_book_id}] has no liquidity."
 msgstr "合约 [{order_book_id}] 流动性不足，拒单。"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:462
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:486
 #, fuzzy
 msgid ""
 "Order Cancelled: market order {order_book_id} volume {order_volume} is "
 "larger than {volume_percent_limit} percent of current tick volume, fill "
 "{filled_volume} actually"
 msgstr ""
 "{order_book_id} 下单量 {order_volume} 超过当前 Tick 成交量的 "
 "{volume_percent_limit}%，实际成交 {filled_volume}"
 
-#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:611
+#: rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py:635
 msgid ""
 "Order Cancelled: market order {order_book_id} fill {filled_volume} "
 "actually"
 msgstr "订单取消：标的 {order_book_id} 实际成交 {filled_volume}"
 
 #: rqalpha/mod/rqalpha_mod_sys_simulation/mod.py:42
 msgid "invalid margin multiplier value: value range is (0, +∞]"
@@ -912,19 +891,23 @@
 msgid "invalid account type {}, choose in {}"
 msgstr "不合法的账户类型 {}， 请在以下账户类型中选择 {}"
 
 #: rqalpha/portfolio/__init__.py:282
 msgid "Cash add {}. units {} become to {}"
 msgstr "入金{}元，份额由{}变动为{}"
 
-#: rqalpha/portfolio/account.py:352
+#: rqalpha/portfolio/account.py:350
+msgid "Futures account's cash turns negative after settlement"
+msgstr "期货账户的现金在结算后变为负数"
+
+#: rqalpha/portfolio/account.py:356
 msgid "Trigger Forced Liquidation, current total_value is 0"
 msgstr "触发强制清算，当前总权益为 0"
 
-#: rqalpha/portfolio/account.py:502 rqalpha/portfolio/account.py:521
+#: rqalpha/portfolio/account.py:506 rqalpha/portfolio/account.py:525
 msgid "insufficient cash, current {}, target withdrawal {}"
 msgstr "现金不足，当前现金 {}，目标出金 {}"
 
 #: rqalpha/utils/arg_checker.py:51
 msgid ""
 "function {}: invalid {} argument, expect a value of type {}, got {} "
 "(type: {})"
@@ -1568,7 +1551,36 @@
 #~ "margin and rates, and fixed data "
 #~ "will be used for calculations\n"
 #~ "You can contact RiceQuant to activate permission: 0755-26569969"
 #~ msgstr ""
 #~ "您的 RQData 账号没有权限使用期货历史保证金和费率，将使用固定的数据进行回测和计算\n"
 #~ "您可联系米筐科技开通相关权限：0755-26569969"
 
+#~ msgid ""
+#~ "RQAlpha already supports backtesting using "
+#~ "futures historical margins and rates, "
+#~ "please upgrade RQDatac to version "
+#~ "2.11.12 and above to use it"
+#~ msgstr "RQAlpha 已支持使用期货历史保证金和费率进行回测，请将 RQDatac 升级至 2.11.12 及以上版本进行使用"
+
+#~ msgid ""
+#~ "Futures historical trading parameters data "
+#~ "is being updated, please wait......"
+#~ msgstr "正在更新期货历史交易参数，请稍后......"
+
+#~ msgid ""
+#~ "RQDatac is not installed, "
+#~ "\"config.base.futures_time_series_trading_parameters\" will "
+#~ "be disabled."
+#~ msgstr ""
+#~ "未安装 RQDatac，将关闭配置 "
+#~ "\"config.base.futures_time_series_trading_parameters\""
+
+#~ msgid ""
+#~ "RQDatac does not have permission to "
+#~ "obtain futures histrical trading parameters,"
+#~ " \"config.base.futures_time_series_trading_parameters\" will"
+#~ " be disabled."
+#~ msgstr ""
+#~ "RQDatac 缺少获取期货历史交易参数的权限，将关闭配置 "
+#~ "\"config.base.futures_time_series_trading_parameters\""
+
```

### Comparing `rqalpha-5.3.9/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-5.4.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha/utils/typing.py` & `rqalpha-5.4.0/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/rqalpha.egg-info/PKG-INFO` & `rqalpha-5.4.0/rqalpha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.3.9
+Version: 5.4.0
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.3.9/rqalpha.egg-info/SOURCES.txt` & `rqalpha-5.4.0/rqalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/setup.py` & `rqalpha-5.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     'simplejson',
     'PyYAML',
     'tabulate',
     'rqrisk >=1.0.6',
     'h5py',
     'matplotlib >=3.1.0',
     "openpyxl",
-    "methodtools"
+    "methodtools",
+    "filelock"
 ]
 
 if sys.version_info < (3, 5):
     requirements.append('typing')
 
 if sys.version_info.major == 2 and sys.version_info.minor == 7:
     requirements.extend([
```

### Comparing `rqalpha-5.3.9/tests/__init__.py` & `rqalpha-5.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/__init__.py` & `rqalpha-5.4.0/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/__init__.py` & `rqalpha-5.4.0/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_margin_stocks.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_accounts/test_position_models.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_match.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_match.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py` & `rqalpha-5.4.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/test_api_base.py` & `rqalpha-5.4.0/tests/api_tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/test_api_future.py` & `rqalpha-5.4.0/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/test_api_stock.py` & `rqalpha-5.4.0/tests/api_tests/test_api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/api_tests/test_config.py` & `rqalpha-5.4.0/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_f_buy_and_hold.py` & `rqalpha-5.4.0/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_f_delivery.py` & `rqalpha-5.4.0/tests/test_f_delivery.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_f_macd.py` & `rqalpha-5.4.0/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_f_macd_signal.py` & `rqalpha-5.4.0/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_f_mean_reverting.py` & `rqalpha-5.4.0/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_f_tick_size.py` & `rqalpha-5.4.0/tests/test_f_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_buy_and_hold.py` & `rqalpha-5.4.0/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_dual_thrust.py` & `rqalpha-5.4.0/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_pit_tax.py` & `rqalpha-5.4.0/tests/test_s_pit_tax.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_scheduler.py` & `rqalpha-5.4.0/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_tick_size.py` & `rqalpha-5.4.0/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_turtle.py` & `rqalpha-5.4.0/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_s_turtle_signal.py` & `rqalpha-5.4.0/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/test_sf_buy_and_hold.py` & `rqalpha-5.4.0/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/__init__.py` & `rqalpha-5.4.0/tests/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py` & `rqalpha-5.4.0/tests/unittest/test_data/test_auto_update_bundle/test_auto_update_bundle_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-5.4.0/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/test_data/test_trading_dates_mixin.py` & `rqalpha-5.4.0/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/test_mod/__init__.py` & `rqalpha-5.4.0/tests/unittest/test_mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/__init__.py` & `rqalpha-5.4.0/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-5.4.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/tests/utils.py` & `rqalpha-5.4.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.3.9/versioneer.py` & `rqalpha-5.4.0/versioneer.py`

 * *Files identical despite different names*

