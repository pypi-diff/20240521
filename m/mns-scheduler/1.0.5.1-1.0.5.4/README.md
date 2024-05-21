# Comparing `tmp/mns-scheduler-1.0.5.1.tar.gz` & `tmp/mns-scheduler-1.0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.5.1.tar", last modified: Fri May 17 13:06:51 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.5.4.tar", last modified: Tue May 21 16:15:33 2024, max compression
```

## Comparing `mns-scheduler-1.0.5.1.tar` & `mns-scheduler-1.0.5.4.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.676024 mns-scheduler-1.0.5.1/
--rw-rw-rw-   0        0        0       62 2024-05-17 13:06:51.675027 mns-scheduler-1.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.631160 mns-scheduler-1.0.5.1/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-05-15 00:08:32.000000 mns-scheduler-1.0.5.1/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.634136 mns-scheduler-1.0.5.1/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.635133 mns-scheduler-1.0.5.1/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.637128 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.638125 mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.638125 mns-scheduler-1.0.5.1/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.640120 mns-scheduler-1.0.5.1/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20539 2024-05-17 11:33:24.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_info_sync_api.py
--rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/de_list_stock_service.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.641118 mns-scheduler-1.0.5.1/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.642116 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.643114 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.644110 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.646106 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.648099 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.650094 mns-scheduler-1.0.5.1/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.1/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.651091 mns-scheduler-1.0.5.1/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.654083 mns-scheduler-1.0.5.1/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
--rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_profit_sync_service_api.py
--rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/finance_common_api.py
--rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
--rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/sync_financial_report_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.655081 mns-scheduler-1.0.5.1/mns_scheduler/finance/test/
--rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/test/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/test/fix_blask_list.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.656078 mns-scheduler-1.0.5.1/mns_scheduler/hk/
--rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.1/mns_scheduler/hk/__init__.py
--rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.1/mns_scheduler/hk/hk_company_info_sync_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.657075 mns-scheduler-1.0.5.1/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.658073 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.659069 mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.660067 mns-scheduler-1.0.5.1/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.660067 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.662061 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.663059 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.664056 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.665053 mns-scheduler-1.0.5.1/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.666051 mns-scheduler-1.0.5.1/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-14 14:32:33.000000 mns-scheduler-1.0.5.1/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.1/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.668045 mns-scheduler-1.0.5.1/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.669042 mns-scheduler-1.0.5.1/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.672035 mns-scheduler-1.0.5.1/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17272 2024-05-17 08:19:07.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.674030 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16262 2024-05-17 11:18:38.000000 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.675027 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3950 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 13:06:51.676024 mns-scheduler-1.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-17 13:06:42.000000 mns-scheduler-1.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.022274 mns-scheduler-1.0.5.4/
+-rw-rw-rw-   0        0        0       62 2024-05-21 16:15:33.022274 mns-scheduler-1.0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.978026 mns-scheduler-1.0.5.4/mns_scheduler/
+-rw-rw-rw-   0        0        0      165 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.4/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.980022 mns-scheduler-1.0.5.4/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.980022 mns-scheduler-1.0.5.4/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.983014 mns-scheduler-1.0.5.4/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.983014 mns-scheduler-1.0.5.4/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.984011 mns-scheduler-1.0.5.4/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.986862 mns-scheduler-1.0.5.4/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.4/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    21598 2024-05-20 14:38:40.000000 mns-scheduler-1.0.5.4/mns_scheduler/company_info/company_info_sync_api.py
+-rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.4/mns_scheduler/company_info/de_list_stock_service.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.987372 mns-scheduler-1.0.5.4/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.988364 mns-scheduler-1.0.5.4/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.989362 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.990359 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.992354 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.993351 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.995346 mns-scheduler-1.0.5.4/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.4/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.996343 mns-scheduler-1.0.5.4/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:32.999335 mns-scheduler-1.0.5.4/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.000332 mns-scheduler-1.0.5.4/mns_scheduler/finance/test/
+-rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/test/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.4/mns_scheduler/finance/test/fix_blask_list.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.001329 mns-scheduler-1.0.5.4/mns_scheduler/hk/
+-rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.4/mns_scheduler/hk/__init__.py
+-rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.4/mns_scheduler/hk/hk_company_info_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.002326 mns-scheduler-1.0.5.4/mns_scheduler/irm/
+-rw-rw-rw-   0        0        0      163 2024-05-20 12:48:16.000000 mns-scheduler-1.0.5.4/mns_scheduler/irm/__init__.py
+-rw-rw-rw-   0        0        0     2086 2024-05-21 05:28:39.000000 mns-scheduler-1.0.5.4/mns_scheduler/irm/stock_irm_cninfo_service.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.002326 mns-scheduler-1.0.5.4/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.004321 mns-scheduler-1.0.5.4/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    22057 2024-05-20 14:34:17.000000 mns-scheduler-1.0.5.4/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.005318 mns-scheduler-1.0.5.4/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.4/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.005318 mns-scheduler-1.0.5.4/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.006316 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.007313 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.008310 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.009308 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.011302 mns-scheduler-1.0.5.4/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.4/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.013297 mns-scheduler-1.0.5.4/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-18 01:43:20.000000 mns-scheduler-1.0.5.4/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.4/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+-rw-rw-rw-   0        0        0      871 2024-05-18 01:43:32.000000 mns-scheduler-1.0.5.4/mns_scheduler/risk/stock_equity_mortgage_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.015320 mns-scheduler-1.0.5.4/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.4/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.4/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.4/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.016290 mns-scheduler-1.0.5.4/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.019282 mns-scheduler-1.0.5.4/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0     1641 2024-05-21 16:15:11.000000 mns-scheduler-1.0.5.4/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17525 2024-05-21 15:36:02.000000 mns-scheduler-1.0.5.4/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.4/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.4/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.021276 mns-scheduler-1.0.5.4/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16262 2024-05-18 00:16:23.000000 mns-scheduler-1.0.5.4/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.4/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-21 16:15:33.021276 mns-scheduler-1.0.5.4/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-21 16:15:32.000000 mns-scheduler-1.0.5.4/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4079 2024-05-21 16:15:32.000000 mns-scheduler-1.0.5.4/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 16:15:32.000000 mns-scheduler-1.0.5.4/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 16:15:32.000000 mns-scheduler-1.0.5.4/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 16:15:33.022274 mns-scheduler-1.0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-21 16:15:11.000000 mns-scheduler-1.0.5.4/setup.py
```

### Comparing `mns-scheduler-1.0.5.1/README.md` & `mns-scheduler-1.0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.5.4/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.5.4/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.5.4/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import mns_common.component.common_service_fun_api as common_service_fun_api
 import mns_common.component.concept.ths_concept_common_service_api as ths_concept_common_service_api
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.api.kpl.symbol.kpl_real_time_quotes_api as kpl_real_time_quotes_api
 import mns_common.utils.data_frame_util as data_frame_util
 import mns_common.api.kpl.constant.kpl_constant as kpl_constant
 import mns_common.component.company.company_common_service_api as company_common_service_api
+import mns_common.constant.db_name_constant as db_name_constant
+import mns_common.component.k_line.common.k_line_common_service_api as k_line_common_service_api
 
 mongodb_util = MongodbUtil('27017')
 # 分页大小
 MAX_PAGE_NUMBER = 6000
 import threading
 
 # 定义一个全局锁，用于保护 result 变量的访问
@@ -85,14 +87,15 @@
         "total_mv",
         "flow_mv",
         "flow_mv_level",
         "holder_controller_name",
         "holder_controller_rate",
         "area",
         "list_date",
+        "deal_days",
         "pe_ttm",
         "pb",
         "ROE",
         "classification",
         "base_business",
         "address",
         "market_id",
@@ -192,21 +195,36 @@
         sub_stock_symbol_list = list(ths_stock_concept_detail['symbol'])
     company_info.loc[:, 'sub_stock'] = False
     company_info.loc[company_info['symbol'].isin(sub_stock_symbol_list), 'sub_stock'] = True
 
     try:
         company_info.dropna(subset=['symbol'], axis=0, inplace=True)
         company_info.dropna(subset=['_id'], axis=0, inplace=True)
-        mongodb_util.save_mongo(company_info, 'company_info')
+        mongodb_util.save_mongo(company_info, db_name_constant.COMPANY_INFO)
+        # 保存历史数据
+        save_company_info_his(company_info)
     except BaseException as e:
         logger.error("出现异常:{},{}", symbol, e)
 
     return company_info
 
 
+def save_company_info_his(company_info_df):
+    now_date = datetime.now()
+    str_day = now_date.strftime('%Y-%m-%d')
+    company_info_df['symbol'] = company_info_df['_id']
+    company_info_df['str_day'] = str_day
+    company_info_df['_id'] = company_info_df['_id'] + "_" + str_day
+    remove_query = {'str_day': str_day}
+    tag = mongodb_util.remove_data(remove_query, db_name_constant.COMPANY_INFO_HIS)
+    success = tag.acknowledged
+    if success:
+        mongodb_util.insert_mongo(company_info_df, db_name_constant.COMPANY_INFO_HIS)
+
+
 def sync_company_base_info(symbol_list):
     global result
     result = []
     create_index()
     east_money_stock_info = get_east_money_stock_info()
     de_listed_stock_list = company_common_service_api.get_de_list_company()
     east_money_stock_info = east_money_stock_info.loc[~(
@@ -306,15 +324,18 @@
             # todo fix industry
             company_info_type['industry'] = company_info_type['second_sw_industry']
             company_info_type['amount'] = company_one.amount
 
             company_info_type['kpl_plate_list_info'] = '-'
             company_info_type['kpl_plate_name'] = '-'
             company_info_type['kpl_most_relative_name'] = '-'
-
+            now_date = datetime.now()
+            str_day = now_date.strftime('%Y-%m-%d')
+            deal_days = k_line_common_service_api.get_deal_days(str_day, company_one.symbol)
+            company_info_type['deal_days'] = deal_days
             try:
                 if data_frame_util.is_not_empty(kpl_real_time_quotes):
                     kpl_real_time_quotes_one = kpl_real_time_quotes.loc[
                         kpl_real_time_quotes['symbol'] == company_one.symbol]
 
                     if data_frame_util.is_not_empty(kpl_real_time_quotes_one):
                         company_info_type['kpl_plate_name'] = list(kpl_real_time_quotes_one['plate_name_list'])[0]
@@ -468,10 +489,10 @@
     # sync_company_base_info()
     # fix_company_industry()
     # calculate_circu_ratio("601069")
     # sync_company_base_info()
     # 300293
     # sync_company_base_info(None)
     # new_company_info_update()
-    sync_company_base_info(['300483'])
-    fix_company_industry('300483')
+    sync_company_base_info(None)
+    fix_company_industry(None)
     # group_by_industry()
```

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/company_info/de_list_stock_service.py` & `mns-scheduler-1.0.5.4/mns_scheduler/company_info/de_list_stock_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.5.4/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.5.4/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_profit_sync_service_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/finance/em_financial_profit_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/finance/finance_common_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/finance/finance_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/finance/sync_financial_report_service_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/finance/sync_financial_report_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/finance/test/fix_blask_list.py` & `mns-scheduler-1.0.5.4/mns_scheduler/finance/test/fix_blask_list.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/hk/hk_company_info_sync_service_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/hk/hk_company_info_sync_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.5.4/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import mns_common.utils.data_frame_util as data_frame_util
 import pandas as pd
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.utils.date_handle_util as date_handle_util
 import mns_common.component.k_line.patterns.k_line_patterns_service_api as k_line_patterns_service
 import mns_common.component.k_line.clean.sh_small_normal_zt_k_line_check_api as sh_small_normal_zt_k_line_check_api
 import mns_common.component.classify.symbol_classify_api as symbol_classify_api
+import mns_common.component.k_line.common.k_line_common_service_api as k_line_common_service_api
 
 mongodb_util = MongodbUtil('27017')
 # 排除最近10天有三个连板的股票
 EXCLUDE_DAYS = 10
 
 MAX_CONTINUE_BOARDS = 3
 
@@ -115,19 +116,19 @@
     k_line_info['week_last_day'] = list(stock_hfq_weekly_last['date'])[0]
 
     return k_line_info
 
 
 # 处理日线
 def handle_day_line(k_line_info, str_day, symbol):
-    # 当天没有k线数据时 进行同步
-    query = {"symbol": symbol, 'date': {"$lt": date_handle_util.no_slash_date(str_day)}}
-    deal_days = mongodb_util.count(query, 'stock_qfq_daily')
+    deal_days = k_line_common_service_api.get_deal_days(str_day, symbol)
 
     # 取五天刚好包含一周 todo 选择60天的历史记录
+    # 当天没有k线数据时 进行同步
+    query = {"symbol": symbol, 'date': {"$lt": date_handle_util.no_slash_date(str_day)}}
     stock_qfq_daily = mongodb_util.descend_query(query, 'stock_qfq_daily', 'date', 60)
     if stock_qfq_daily.shape[0] == 0:
         return k_line_info
     k_line_info = init_day_line_data(k_line_info, stock_qfq_daily)
     k_line_info = calculate_30_day_max_chg(stock_qfq_daily, k_line_info)
 
     stock_qfq_daily = calculate_exchange_avg_param(stock_qfq_daily)
@@ -402,23 +403,26 @@
     std_amount_sixty = 0
     mean_amount_sixty = 0
 
     if daily_num >= 10:
         stock_qfq_daily_ten = stock_qfq_daily.iloc[0:10]
         # 计算 amount 的标准差
         std_amount_ten = round(stock_qfq_daily_ten['amount_level'].std(), 2)
+        # 计算 amount 的平均值
         mean_amount_ten = round(stock_qfq_daily_ten['amount_level'].mean(), 2)
 
     if daily_num >= 30:
         stock_qfq_daily_thirty = stock_qfq_daily.iloc[0:30]
         # 计算 amount 的标准差
         std_amount_thirty = round(stock_qfq_daily_thirty['amount_level'].std(), 2)
+        # 计算 amount 的平均值
         mean_amount_thirty = round(stock_qfq_daily_thirty['amount_level'].mean(), 2)
     if daily_num >= 60:
         std_amount_sixty = round(stock_qfq_daily['amount_level'].std(), 2)
+        # 计算 amount 的平均值
         mean_amount_sixty = round(stock_qfq_daily['amount_level'].mean(), 2)
 
     # text = list(stock_qfq_daily_one['history_data'])[0]
     # history_data_df = pd.read_csv(StringIO(text), delim_whitespace=True)
 
     stock_qfq_daily_one.loc[:, 'std_amount_ten'] = std_amount_ten
     stock_qfq_daily_one.loc[:, 'mean_amount_ten'] = mean_amount_ten
```

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.5.4/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.5.4/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import mns_common.component.company.company_common_service_api as company_common_service_api
 import mns_common.component.common_service_fun_api as common_service_fun_api
 import mns_common.component.data.data_init_api as data_init_api
 import pandas as pd
 from datetime import time
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.utils.data_frame_util as data_frame_util
+import mns_common.component.k_line.common.k_line_common_service_api as k_line_common_service_api
 
 mongodb_util = MongodbUtil('27017')
 mongodb_util_21019 = MongodbUtil('27019')
 
 realtime_quotes_now_zt_new_kc_open_field = ['_id',
                                             'symbol',
                                             'name',
@@ -219,14 +220,18 @@
     # 计算日期差值 距离现在上市时间
     realtime_quotes_now_zt_new_kc_open_copy['diff_days'] = realtime_quotes_now_zt_new_kc_open_copy.apply(
         lambda row: (row['str_day_01'] - row['list_date_01']).days, axis=1)
 
     del realtime_quotes_now_zt_new_kc_open_copy['str_day_01']
     del realtime_quotes_now_zt_new_kc_open_copy['list_date_01']
 
+    deal_days = k_line_common_service_api.get_deal_days(str_day, kc_one.symbol)
+
+    realtime_quotes_now_zt_new_kc_open_copy['deal_days'] = deal_days
+
     mongodb_util.save_mongo(realtime_quotes_now_zt_new_kc_open_copy, 'realtime_quotes_now_zt_new_kc_open')
 
 
 # 同步当前day整天数据
 def one_symbol_day_data(str_day, kc_one, realtime_quotes_now_kc):
     realtime_quotes_now_kc.loc[
         realtime_quotes_now_kc['symbol'] == kc_one.symbol, 'industry'] = kc_one.industry
```

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.5.4/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.5.1/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.5.4/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 mns_scheduler/finance/finance_common_api.py
 mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
 mns_scheduler/finance/sync_financial_report_service_api.py
 mns_scheduler/finance/test/__init__.py
 mns_scheduler/finance/test/fix_blask_list.py
 mns_scheduler/hk/__init__.py
 mns_scheduler/hk/hk_company_info_sync_service_api.py
+mns_scheduler/irm/__init__.py
+mns_scheduler/irm/stock_irm_cninfo_service.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
 mns_scheduler/k_line/clean/k_line_info_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
 mns_scheduler/kpl/__init__.py
@@ -65,14 +67,15 @@
 mns_scheduler/kpl/selection/total/__init__.py
 mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
 mns_scheduler/real_time/__init__.py
 mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
 mns_scheduler/real_time/realtime_quotes_now_sync.py
 mns_scheduler/risk/__init__.py
 mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+mns_scheduler/risk/stock_equity_mortgage_sync_api.py
 mns_scheduler/trade/__init__.py
 mns_scheduler/trade/auto_ipo_buy_api.py
 mns_scheduler/trade/auto_sell_service_api.py
 mns_scheduler/trade/sync_position_api.py
 mns_scheduler/zb/__init__.py
 mns_scheduler/zb/stock_zb_pool_sync.py
 mns_scheduler/zt/__init__.py
```

