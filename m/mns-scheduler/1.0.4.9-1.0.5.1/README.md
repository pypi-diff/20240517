# Comparing `tmp/mns-scheduler-1.0.4.9.tar.gz` & `tmp/mns-scheduler-1.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.4.9.tar", last modified: Wed May 15 16:05:57 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.5.1.tar", last modified: Fri May 17 13:06:51 2024, max compression
```

## Comparing `mns-scheduler-1.0.4.9.tar` & `mns-scheduler-1.0.5.1.tar`

### file list

```diff
@@ -1,116 +1,122 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.085101 mns-scheduler-1.0.4.9/
--rw-rw-rw-   0        0        0       62 2024-05-15 16:05:57.084104 mns-scheduler-1.0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.051192 mns-scheduler-1.0.4.9/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-05-15 00:08:32.000000 mns-scheduler-1.0.4.9/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.053187 mns-scheduler-1.0.4.9/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.053187 mns-scheduler-1.0.4.9/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.055181 mns-scheduler-1.0.4.9/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.056179 mns-scheduler-1.0.4.9/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.057176 mns-scheduler-1.0.4.9/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.059171 mns-scheduler-1.0.4.9/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15735 2024-05-13 09:25:17.000000 mns-scheduler-1.0.4.9/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20342 2024-05-13 09:29:51.000000 mns-scheduler-1.0.4.9/mns_scheduler/company_info/company_info_sync_api.py
--rw-rw-rw-   0        0        0     1709 2024-05-15 14:54:05.000000 mns-scheduler-1.0.4.9/mns_scheduler/company_info/de_list_stock_service.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.059171 mns-scheduler-1.0.4.9/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.060168 mns-scheduler-1.0.4.9/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/clean/kpl_concept_clean_api.py
--rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.061165 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.062162 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.063160 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.064157 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.066152 mns-scheduler-1.0.4.9/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.4.9/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.066152 mns-scheduler-1.0.4.9/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.069144 mns-scheduler-1.0.4.9/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.4.9/mns_scheduler/finance/__init__.py
--rw-rw-rw-   0        0        0    17231 2024-05-15 08:23:18.000000 mns-scheduler-1.0.4.9/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
--rw-rw-rw-   0        0        0    13989 2024-05-15 14:22:01.000000 mns-scheduler-1.0.4.9/mns_scheduler/finance/em_financial_profit_sync_service_api.py
--rw-rw-rw-   0        0        0     1075 2024-05-15 09:52:38.000000 mns-scheduler-1.0.4.9/mns_scheduler/finance/finance_common_api.py
--rw-rw-rw-   0        0        0     8782 2024-05-15 14:21:03.000000 mns-scheduler-1.0.4.9/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
--rw-rw-rw-   0        0        0     6331 2024-05-15 14:55:34.000000 mns-scheduler-1.0.4.9/mns_scheduler/finance/sync_financial_report_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.069144 mns-scheduler-1.0.4.9/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.071138 mns-scheduler-1.0.4.9/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.071138 mns-scheduler-1.0.4.9/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.4.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.072136 mns-scheduler-1.0.4.9/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.072136 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.073134 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.074131 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.075128 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.076125 mns-scheduler-1.0.4.9/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.9/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.077123 mns-scheduler-1.0.4.9/mns_scheduler/risk/
--rw-rw-rw-   0        0        0      163 2024-05-14 14:32:33.000000 mns-scheduler-1.0.4.9/mns_scheduler/risk/__init__.py
--rw-rw-rw-   0        0        0     4949 2024-05-15 12:17:25.000000 mns-scheduler-1.0.4.9/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.079117 mns-scheduler-1.0.4.9/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.9/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.9/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.9/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.080115 mns-scheduler-1.0.4.9/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.082109 mns-scheduler-1.0.4.9/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17272 2024-05-11 03:32:32.000000 mns-scheduler-1.0.4.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.4.9/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.083106 mns-scheduler-1.0.4.9/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    16256 2024-05-15 15:07:01.000000 mns-scheduler-1.0.4.9/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:05:57.084104 mns-scheduler-1.0.4.9/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-15 16:05:56.000000 mns-scheduler-1.0.4.9/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3784 2024-05-15 16:05:57.000000 mns-scheduler-1.0.4.9/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:05:56.000000 mns-scheduler-1.0.4.9/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 16:05:56.000000 mns-scheduler-1.0.4.9/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 16:05:57.085101 mns-scheduler-1.0.4.9/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-15 16:01:39.000000 mns-scheduler-1.0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.676024 mns-scheduler-1.0.5.1/
+-rw-rw-rw-   0        0        0       62 2024-05-17 13:06:51.675027 mns-scheduler-1.0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.631160 mns-scheduler-1.0.5.1/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-05-15 00:08:32.000000 mns-scheduler-1.0.5.1/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.634136 mns-scheduler-1.0.5.1/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.635133 mns-scheduler-1.0.5.1/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.637128 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.638125 mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.638125 mns-scheduler-1.0.5.1/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.640120 mns-scheduler-1.0.5.1/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    14306 2024-05-17 08:56:50.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20539 2024-05-17 11:33:24.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_info_sync_api.py
+-rw-rw-rw-   0        0        0     1993 2024-05-17 07:32:00.000000 mns-scheduler-1.0.5.1/mns_scheduler/company_info/de_list_stock_service.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.641118 mns-scheduler-1.0.5.1/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.642116 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.643114 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.644110 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.646106 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.648099 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.650094 mns-scheduler-1.0.5.1/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-05-10 13:05:35.000000 mns-scheduler-1.0.5.1/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.651091 mns-scheduler-1.0.5.1/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.654083 mns-scheduler-1.0.5.1/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-15 14:37:41.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/__init__.py
+-rw-rw-rw-   0        0        0    19437 2024-05-16 00:08:00.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
+-rw-rw-rw-   0        0        0    14145 2024-05-16 00:05:34.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_profit_sync_service_api.py
+-rw-rw-rw-   0        0        0     2471 2024-05-16 08:53:00.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/finance_common_api.py
+-rw-rw-rw-   0        0        0    10561 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
+-rw-rw-rw-   0        0        0     5042 2024-05-16 09:27:25.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/sync_financial_report_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.655081 mns-scheduler-1.0.5.1/mns_scheduler/finance/test/
+-rw-rw-rw-   0        0        0      163 2024-05-16 01:05:27.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/test/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-05-16 06:04:02.000000 mns-scheduler-1.0.5.1/mns_scheduler/finance/test/fix_blask_list.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.656078 mns-scheduler-1.0.5.1/mns_scheduler/hk/
+-rw-rw-rw-   0        0        0      163 2024-05-16 07:31:10.000000 mns-scheduler-1.0.5.1/mns_scheduler/hk/__init__.py
+-rw-rw-rw-   0        0        0     3661 2024-05-17 08:14:15.000000 mns-scheduler-1.0.5.1/mns_scheduler/hk/hk_company_info_sync_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.657075 mns-scheduler-1.0.5.1/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.658073 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.659069 mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5652 2024-05-11 03:27:17.000000 mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.660067 mns-scheduler-1.0.5.1/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.660067 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.662061 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.663059 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.664056 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.665053 mns-scheduler-1.0.5.1/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.666051 mns-scheduler-1.0.5.1/mns_scheduler/risk/
+-rw-rw-rw-   0        0        0      163 2024-05-14 14:32:33.000000 mns-scheduler-1.0.5.1/mns_scheduler/risk/__init__.py
+-rw-rw-rw-   0        0        0     5086 2024-05-17 13:05:26.000000 mns-scheduler-1.0.5.1/mns_scheduler/risk/register_and_investigate_stock_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.668045 mns-scheduler-1.0.5.1/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.5.1/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.669042 mns-scheduler-1.0.5.1/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.672035 mns-scheduler-1.0.5.1/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17272 2024-05-17 08:19:07.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-05-17 08:14:54.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7604 2024-05-09 15:06:22.000000 mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.674030 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    16262 2024-05-17 11:18:38.000000 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.5.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:06:51.675027 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3950 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 13:06:51.000000 mns-scheduler-1.0.5.1/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 13:06:51.676024 mns-scheduler-1.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-17 13:06:42.000000 mns-scheduler-1.0.5.1/setup.py
```

### Comparing `mns-scheduler-1.0.4.9/README.md` & `mns-scheduler-1.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.5.1/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.5.1/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_constant_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,116 +7,14 @@
 sys.path.append(project_path)
 import pandas as pd
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.utils.data_frame_util as data_frame_util
 
 mongodb_util = MongodbUtil('27017')
 
-# 退市股票
-de_listed_stock_list = [
-    "002018",
-    "600240",
-    "000033",
-    "000405",
-    "000406",
-    "000418",
-    "000508",
-    "000535",
-    "000542",
-    "000549",
-    "000569",
-    "000583",
-    "000594",
-    "000618",
-    "000621",
-    "000660",
-    "000675",
-    "000689",
-    "000699",
-    "000730",
-    "000748",
-    "000763",
-    "000765",
-    "000769",
-    "000787",
-    "000805",
-    "000817",
-    "000827",
-    "000866",
-    "000916",
-    "000939",
-    "000956",
-    "002477",
-    "300028",
-    "300090",
-    "300104",
-    "300156",
-    "300431",
-    "600001",
-    "600002",
-    "600003",
-    "600005",
-    "600065",
-    "600069",
-    "600087",
-    "600092",
-    "600102",
-    "600181",
-    "600205",
-    "600263",
-    "600270",
-    "600286",
-    "600296",
-    "600317",
-    "600357",
-    "600401",
-    "600472",
-    "600553",
-    "600591",
-    "600625",
-    "600627",
-    "600631",
-    "600632",
-    "600646",
-    "600670",
-    "600672",
-    "600680",
-    "600752",
-    "600772",
-    "600786",
-    "600788",
-    "600799",
-    "600813",
-    "600832",
-    "600849",
-    "600852",
-    "600899",
-    "600991",
-    "601558"
-]
-
-# 需要修改行业的股票
-fix_symbol_list = [
-    '688507',
-    '301387',
-    '688480',
-    '301112',
-    '603260',
-    '300559',
-    '300836',
-    '300293',
-    '688630',
-    '001309',
-    '600338',
-    '000032',
-    '300042',
-    '300295',
-    '300483'
-]
-
 
 def get_fix_symbol_industry():
     return pd.DataFrame([['688480', '赛恩斯', '760103', '环境治理'],
                          ['000032', '深桑达Ａ', '730200', '通信网络设备及器件'],
                          ['688480', '赛恩斯', '640704', '自动化设备'],
                          ['603260', '合盛硅业', '220316', '有机硅'],
                          ['300559', '佳发教育', '461102', '培训教育'],
@@ -127,14 +25,15 @@
                          ['600338', '西藏珠峰', '240603', '锂'],
                          ['300042', '朗科科技', '270108', '半导体设备'],
                          ['688507', '索辰科技', '710402', '横向通用软件'],
                          ['301387', '光大同创', '270504', '消费电子零部件及组装'],
                          ['300295', '三六五网', '430300', '物业管理'],
                          ['300947', '德必集团', '430300', '物业管理'],
                          ['300483', '首华燃气', '410301', '燃气Ⅲ'],
+                         ['300215', '电科院', '410110', '电能综合服务'],
                          ],
                         columns=['symbol', 'name', 'new_industry_code', 'new_industry'])
 
 
 def get_industry_final_fix_df():
     return pd.DataFrame([
         # 汽车
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,37 +182,39 @@
     company_info['sync_date'] = str_now_date
 
     try:
         # 次新股
         sub_stock = ths_stock_api.ths_stock_concept('885598')
         sub_stock_symbol_list = list(sub_stock['symbol'])
     except BaseException as e:
+        logger.error("出现异常:{},{}", symbol, e)
         query = {'concept_code': 885598}
         ths_stock_concept_detail = mongodb_util.find_query_data('ths_stock_concept_detail', query)
         sub_stock_symbol_list = list(ths_stock_concept_detail['symbol'])
     company_info.loc[:, 'sub_stock'] = False
     company_info.loc[company_info['symbol'].isin(sub_stock_symbol_list), 'sub_stock'] = True
 
     try:
         company_info.dropna(subset=['symbol'], axis=0, inplace=True)
         company_info.dropna(subset=['_id'], axis=0, inplace=True)
         mongodb_util.save_mongo(company_info, 'company_info')
     except BaseException as e:
-        logger.error("出现异常:{}", symbol)
+        logger.error("出现异常:{},{}", symbol, e)
 
     return company_info
 
 
 def sync_company_base_info(symbol_list):
     global result
     result = []
     create_index()
     east_money_stock_info = get_east_money_stock_info()
+    de_listed_stock_list = company_common_service_api.get_de_list_company()
     east_money_stock_info = east_money_stock_info.loc[~(
-        east_money_stock_info['symbol'].isin(company_constant_data_api.de_listed_stock_list))]
+        east_money_stock_info['symbol'].isin(de_listed_stock_list))]
     east_money_stock_info = common_service_fun_api.exclude_ts_symbol(east_money_stock_info)
     east_money_stock_info = east_money_stock_info.loc[~((east_money_stock_info['industry'] == '-')
                                                         & (east_money_stock_info['now_price'] == 0))]
 
     east_money_stock_info = common_service_fun_api.total_mv_classification(east_money_stock_info)
     east_money_stock_info = common_service_fun_api.classify_symbol(east_money_stock_info)
 
@@ -292,16 +294,16 @@
             company_info_type['classification'] = company_one.classification
             company_info_type['mv_circulation_ratio'] = calculate_circu_ratio(company_one.symbol)
             # 获取同花顺最新概念
             company_info_type = ths_concept_common_service_api.set_ths_concept(company_one.symbol, company_info_type)
             now_date = datetime.now()
             str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
             company_info_type['sync_date'] = str_now_date
-
-            if company_one.symbol in company_constant_data_api.fix_symbol_list:
+            fix_symbol_industry_df = company_constant_data_api.get_fix_symbol_industry()
+            if company_one.symbol in list(fix_symbol_industry_df['symbol']):
                 # fix sw_industry
                 company_info_type = company_constant_data_api.fix_symbol_industry(company_info_type, company_one.symbol)
 
             # todo fix industry
             company_info_type['industry'] = company_info_type['second_sw_industry']
             company_info_type['amount'] = company_one.amount
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/company_info/de_list_stock_service.py` & `mns-scheduler-1.0.5.1/mns_scheduler/company_info/de_list_stock_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,11 +29,19 @@
                                                   "终止上市日期": "de_list_date"
                                                   })
     all_de_list_df = pd.concat([sz_de_list_df, sh_de_list_df])
     all_de_list_df['_id'] = all_de_list_df['symbol']
     all_de_list_df['list_date'] = all_de_list_df['list_date'].astype(str)
     all_de_list_df['de_list_date'] = all_de_list_df['de_list_date'].astype(str)
     mongodb_util.save_mongo(all_de_list_df, db_name_constant.DE_LIST_STOCK)
+    remove_black_list(all_de_list_df)
+
+
+# 移除黑名单
+def remove_black_list(all_de_list_df):
+    symbol_list = list(all_de_list_df['symbol'])
+    remove_query = {'symbol': {"$in": symbol_list}}
+    mongodb_util.remove_data(remove_query, db_name_constant.SELF_BLACK_STOCK)
 
 
 if __name__ == '__main__':
     sync_de_list_stock()
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/clean/kpl_concept_clean_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/kpl_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.5.1/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.5.1/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 end = file_path.index('mns') + 16
 project_path = file_path[0:end]
 sys.path.append(project_path)
 import akshare as ak
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_scheduler.finance.finance_common_api as finance_common_api
 import mns_common.constant.db_name_constant as db_name_constant
+
 mongodb_util = MongodbUtil('27017')
 from loguru import logger
 import mns_common.utils.data_frame_util as data_frame_util
 
 
 #
 # {
@@ -341,18 +342,19 @@
 # 资产负债表
 # https://emweb.securities.eastmoney.com/PC_HSF10/NewFinanceAnalysis/Index?type=web&code=sh600519#zcfzb-0
 def get_em_asset_liability_api(symbol):
     sec_code = finance_common_api.get_sec_code(symbol)
     try:
         stock_balance_sheet_by_report_em_df = ak.stock_balance_sheet_by_report_em(sec_code)
     except Exception as e:
-        logger.error("同步利润表异常:{},{}", symbol, e)
+        logger.error("同步资产表异常:{},{}", symbol, e)
         return None
     if data_frame_util.is_empty(stock_balance_sheet_by_report_em_df):
         return None
+    stock_balance_sheet_by_report_em_df = check_columns(stock_balance_sheet_by_report_em_df)
     stock_balance_sheet_by_report_em_df = stock_balance_sheet_by_report_em_df[[
         'SECUCODE',
         'SECURITY_CODE',
         'SECURITY_NAME_ABBR',
         'ORG_CODE',
         'ORG_TYPE',
         'REPORT_DATE',
@@ -422,15 +424,68 @@
         new_asset_df = stock_balance_sheet_by_report_em_df.loc[
             ~(stock_balance_sheet_by_report_em_df['SECURITY_CODE'].isin(list(exist_asset_em_df['SECURITY_CODE'])))]
     else:
         new_asset_df = stock_balance_sheet_by_report_em_df
     if data_frame_util.is_empty(new_asset_df):
         return None
     new_asset_df.fillna(0, inplace=True)
-    mongodb_util.insert_mongo(new_asset_df, db_name_constant.EM_STOCK_ASSET_LIABILITY)
+    return new_asset_df
+
+
+def check_columns(new_asset_df):
+    if 'CONTRACT_LIAB' not in new_asset_df.columns:
+        new_asset_df['CONTRACT_LIAB'] = 0
+
+    if 'DEVELOP_EXPENSE' not in new_asset_df.columns:
+        new_asset_df['DEVELOP_EXPENSE'] = 0
+
+    if 'INVENTORY' not in new_asset_df.columns:
+        new_asset_df['INVENTORY'] = 0
+
+    if 'NONCURRENT_LIAB_1YEAR' not in new_asset_df.columns:
+        new_asset_df['NONCURRENT_LIAB_1YEAR'] = 0
+
+    if 'NOTE_ACCOUNTS_PAYABLE' not in new_asset_df.columns:
+        new_asset_df['NOTE_ACCOUNTS_PAYABLE'] = 0
+
+    if 'NOTE_ACCOUNTS_RECE' not in new_asset_df.columns:
+        new_asset_df['NOTE_ACCOUNTS_RECE'] = 0
+
+    if 'OTHER_CURRENT_ASSET' not in new_asset_df.columns:
+        new_asset_df['OTHER_CURRENT_ASSET'] = 0
+
+    if 'OTHER_CURRENT_LIAB' not in new_asset_df.columns:
+        new_asset_df['OTHER_CURRENT_LIAB'] = 0
+
+    if 'OTHER_NONCURRENT_ASSET' not in new_asset_df.columns:
+        new_asset_df['OTHER_NONCURRENT_ASSET'] = 0
+    if 'OTHER_NONCURRENT_FINASSET' not in new_asset_df.columns:
+        new_asset_df['OTHER_NONCURRENT_FINASSET'] = 0
+    if 'PREPAYMENT' not in new_asset_df.columns:
+        new_asset_df['PREPAYMENT'] = 0
+    if 'TOTAL_CURRENT_ASSETS' not in new_asset_df.columns:
+        new_asset_df['TOTAL_CURRENT_ASSETS'] = 0
+    if 'TOTAL_CURRENT_LIAB' not in new_asset_df.columns:
+        new_asset_df['TOTAL_CURRENT_LIAB'] = 0
+    if 'TOTAL_NONCURRENT_ASSETS' not in new_asset_df.columns:
+        new_asset_df['TOTAL_NONCURRENT_ASSETS'] = 0
+    if 'TOTAL_NONCURRENT_LIAB' not in new_asset_df.columns:
+        new_asset_df['TOTAL_NONCURRENT_LIAB'] = 0
+    if 'TOTAL_OTHER_PAYABLE' not in new_asset_df.columns:
+        new_asset_df['TOTAL_OTHER_PAYABLE'] = 0
+    if 'TOTAL_OTHER_RECE' not in new_asset_df.columns:
+        new_asset_df['TOTAL_OTHER_RECE'] = 0
+    if 'ACCOUNTS_RECE' not in new_asset_df.columns:
+        new_asset_df['ACCOUNTS_RECE'] = 0
+
+    if 'LOAN_ADVANCE' not in new_asset_df.columns:
+        new_asset_df['LOAN_ADVANCE'] = 0
+    if 'MONETARYFUNDS' not in new_asset_df.columns:
+        new_asset_df['MONETARYFUNDS'] = 0
+    return new_asset_df
 
 
 if __name__ == '__main__':
     get_em_asset_liability_api('832876')
 
     stock_cash_flow_sheet_by_report_em_df = ak.stock_cash_flow_sheet_by_report_em(symbol="SH600519")
     print(stock_cash_flow_sheet_by_report_em_df)
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/finance/em_financial_profit_sync_service_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/finance/em_financial_profit_sync_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,16 +322,21 @@
         profit_df['FINANCE_EXPENSE'] = 0
     if 'FE_INTEREST_EXPENSE' not in profit_df.columns:
         profit_df['FE_INTEREST_EXPENSE'] = 0
     if 'FE_INTEREST_INCOME' not in profit_df.columns:
         profit_df['FE_INTEREST_INCOME'] = 0
     if 'CREDIT_IMPAIRMENT_INCOME' not in profit_df.columns:
         profit_df['CREDIT_IMPAIRMENT_INCOME'] = 0
-    if 'FAIRVALUE_CHANGE_INCOME' not in profit_df.columns:
-            profit_df['FAIRVALUE_CHANGE_INCOME'] = 0
+    if 'ACCOUNTS_RECE' not in profit_df.columns:
+        profit_df['ACCOUNTS_RECE'] = 0
+
+    if 'LOAN_ADVANCE' not in profit_df.columns:
+        profit_df['LOAN_ADVANCE'] = 0
+    if 'MONETARYFUNDS' not in profit_df.columns:
+        profit_df['MONETARYFUNDS'] = 0
     return profit_df
 
 
 import mns_common.api.em.east_money_stock_api as east_money_stock_api
 
 if __name__ == '__main__':
     em_df = east_money_stock_api.get_real_time_quotes_all_stocks()
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import mns_scheduler.finance.finance_common_api as finance_common_api
 from loguru import logger
 import mns_common.constant.db_name_constant as db_name_constant
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.component.trade_date.trade_date_common_service_api as trade_date_common_service_api
 import mns_common.component.common_service_fun_api as common_service_fun_api
 import pandas as pd
+
 # 1.无保留意见/标准报告：报告没问题。（没有发现造假，但也不能保证为真）
 #
 # 2.带强调事项段的无保留意见：报告没问题，但是有亏损获对其可持续经营有重大疑虑（可能造假，至少是在粉饰报表）
 #
 # 3.保留意见报告：有问题，财务造假
 #
 # 4.否定意见报告：有很大问题
@@ -31,14 +32,19 @@
 
 # 利润为负的时候最小营业收入 主板 3.2亿
 MIN_INCOME_MAIN = 320000000
 # 利润为负的时候最小营业收入 科创 创业 1.2亿
 MIN_INCOME_SUB = 120000000
 # 最大负债比
 MAX_LIABILITY_RATIO = 90
+# 负载超过90%时候最小净资产
+MIN_NET_ASSET = 1000000000
+# 排除校验负债比的行业
+EXCLUDE_INDUSTRY = ['保险', '银行', '证券']
+
 # 最迟出报告的天数
 LATE_REPORT_DAYS = 3
 
 
 #### 退市新规 ####
 # 1 股价类:连续20个交易日估价低于1元
 # 2 市值类: 主板小于5亿、创业板3亿
@@ -60,26 +66,27 @@
     # 审核意见
     opinion_type = list(new_report_one_df['OPINION_TYPE'])[0]
     symbol = list(new_report_one_df['SECURITY_CODE'])[0]
     name = list(new_report_one_df['SECURITY_NAME_ABBR'])[0]
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
-    id_key = symbol + "_" + period_time
+
     # 年报有问题
     if opinion_type != OPINION_TYPE:
+        id_key = symbol + "_" + period_time + "_" + black_list_service_api.FINANCIAL_PROBLEM_ANNUAL_REPORT
         black_list_service_api.save_black_stock(id_key,
                                                 symbol,
                                                 name,
                                                 str_day,
                                                 str_now_date,
-                                                '年报审计有问题:'+"["+opinion_type+"]",
+                                                '年报审计有问题:' + "[" + str(opinion_type) + "]",
                                                 '年报审计有问题',
                                                 '',
-                                                black_list_service_api.FINANCIAL_PROBLEM)
+                                                black_list_service_api.FINANCIAL_PROBLEM_ANNUAL_REPORT)
 
     if report_type == db_name_constant.EM_STOCK_PROFIT:
         # 利润总额  净利润 扣除非经常性损益后的净利润  三者最小为负
         # 利润总额
         total_profit = list(new_report_one_df['TOTAL_PROFIT'])[0]
         #  净利润
         net_profit = list(new_report_one_df['NETPROFIT'])[0]
@@ -89,60 +96,77 @@
         continued_profit = list(new_report_one_df['CONTINUED_NETPROFIT'])[0]
         # 归属于母公司股东的净利润
         parent_profit = list(new_report_one_df['PARENT_NETPROFIT'])[0]
         # 扣除非经常性损益后的净利润
         deduct_parent_profit = list(new_report_one_df['DEDUCT_PARENT_NETPROFIT'])[0]
         # 营业总收入
         total_operate_income = list(new_report_one_df['TOTAL_OPERATE_INCOME'])[0]
+        if total_operate_income == 0:
+            #  营业收入
+            total_operate_income = list(new_report_one_df['OPERATE_INCOME'])[0]
 
-        # 最小利润收入
+            # 最小利润收入
         min_profit = min(total_profit, net_profit, operate_profit,
                          continued_profit, parent_profit, deduct_parent_profit)
         if min_profit < 0:
 
             classification = common_service_fun_api.classify_symbol_one(symbol)
             if ((classification in ['S', 'H'] and total_operate_income < MIN_INCOME_MAIN)
                     | (classification in ['K', 'C'] and total_operate_income < MIN_INCOME_SUB)):
-                id_key = symbol + "_" + period_time
+                id_key = symbol + "_" + period_time + "_" + black_list_service_api.FINANCIAL_PROBLEM_PROFIT
+                min_profit = round(min_profit / common_service_fun_api.TEN_THOUSAND, 1)
+                total_operate_income = round(total_operate_income / common_service_fun_api.HUNDRED_MILLION, 1)
+
                 black_list_service_api.save_black_stock(id_key,
                                                         symbol,
                                                         name,
                                                         str_day,
                                                         str_now_date,
-                                                        '年报&利润收入触发退市',
-                                                        '年报&利润收入触发退市',
+                                                        '年报:利润:' + '[' + str(min_profit) + '万]' + '收入:' + str(
+                                                            total_operate_income) + '[' + '亿元]--' + '触发退市风险',
+                                                        '年报:利润:' + '[' + str(min_profit) + '万]' + '收入:' + str(
+                                                            total_operate_income) + '[' + '亿元]--' + '触发退市风险',
                                                         '',
-                                                        black_list_service_api.FINANCIAL_PROBLEM)
+                                                        black_list_service_api.FINANCIAL_PROBLEM_PROFIT)
 
 
 # 负债比校验
 def liability_ratio_check(report_type, new_report_df, period_time):
     if report_type == db_name_constant.EM_STOCK_ASSET_LIABILITY:
         new_report_df = new_report_df.sort_values(by=['REPORT_DATE'], ascending=False)
         new_report_one_df = new_report_df.iloc[0:1]
         # 负债比
         liability_ratio = list(new_report_one_df['liability_ratio'])[0]
+        # 净资产
+        net_asset = round(list(new_report_one_df['TOTAL_ASSETS'])[0] - list(new_report_one_df['TOTAL_LIABILITIES'])[0],
+                          2)
 
         symbol = list(new_report_one_df['SECURITY_CODE'])[0]
         name = list(new_report_one_df['SECURITY_NAME_ABBR'])[0]
         now_date = datetime.now()
         str_day = now_date.strftime('%Y-%m-%d')
         str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
-        id_key = symbol + "_" + period_time
+        id_key = symbol + "_" + period_time + "_" + black_list_service_api.FINANCIAL_PROBLEM_DEBT
+
+        query_company = {'_id': symbol, 'industry': {'$in': EXCLUDE_INDUSTRY}}
+        if mongodb_util.exist_data_query(db_name_constant.COMPANY_INFO, query_company):
+            return None
 
         if liability_ratio >= MAX_LIABILITY_RATIO:
             black_list_service_api.save_black_stock(id_key,
                                                     symbol,
                                                     name,
                                                     str_day,
                                                     str_now_date,
-                                                    '负债过高',
-                                                    '负债过高',
+                                                    '负债过高:' + "[" + str(
+                                                        liability_ratio) + "]" + "," + "净资产:" + str(round(
+                                                        net_asset / common_service_fun_api.HUNDRED_MILLION, 0)) + "亿",
+                                                    '负债过高:' + "[" + str(liability_ratio) + "]",
                                                     '',
-                                                    black_list_service_api.FINANCIAL_PROBLEM)
+                                                    black_list_service_api.FINANCIAL_PROBLEM_DEBT)
 
 
 # 未出财报
 def un_report_check(sync_time, now_year, period, period_time):
     un_report_asset_df = finance_common_api.find_un_report_symbol(period_time,
                                                                   db_name_constant.EM_STOCK_ASSET_LIABILITY)
     un_report_profit_df = finance_common_api.find_un_report_symbol(period_time,
@@ -151,28 +175,28 @@
     if period == 4 or period == 1:
         last_report_day = str(now_year) + "-05-01"
     elif period == 2:
         last_report_day = str(now_year) + "-07-01"
     elif period == 3:
         last_report_day = str(now_year) + "-10-01"
     max_report_day = trade_date_common_service_api.get_before_trade_date(last_report_day, LATE_REPORT_DAYS)
-    if max_report_day > sync_time:
+    if max_report_day >= sync_time:
 
         for un_asset_one in un_report_df.itertuples():
             symbol = un_asset_one.symbol
-            id_key = symbol + "_" + period_time
+            id_key = symbol + "_" + period_time + "_" + black_list_service_api.FINANCIAL_PROBLEM_NOT_REPORT
             name = un_asset_one.name
             now_date = datetime.now()
             str_day = now_date.strftime('%Y-%m-%d')
             try:
 
                 black_list_service_api.save_black_stock(id_key,
                                                         symbol,
                                                         name,
                                                         str_day,
                                                         sync_time,
                                                         '未出财报',
                                                         '未出财报',
                                                         '',
-                                                        black_list_service_api.FINANCIAL_PROBLEM)
+                                                        black_list_service_api.FINANCIAL_PROBLEM_NOT_REPORT)
             except Exception as e:
-                logger.error("同步利润表异常:{},{},{}", symbol, period_time, e)
+                logger.error("更新未出报告异常:{},{},{}", symbol, period_time, e)
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/finance/sync_financial_report_service_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/finance/sync_financial_report_service_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import os
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 16
 project_path = file_path[0:end]
 sys.path.append(project_path)
 from datetime import datetime
-import mns_common.api.em.east_money_stock_api as east_money_stock_api
-import mns_scheduler.finance.finance_common_api as finance_common_api
+
 import mns_common.constant.db_name_constant as db_name_constant
 import mns_scheduler.finance.em_financial_profit_sync_service_api as em_financial_profit_sync_service_api
 from mns_common.db.MongodbUtil import MongodbUtil
 from loguru import logger
 import \
     mns_scheduler.finance.em_financial_asset_liability_sync_service_api as em_financial_asset_liability_sync_service_api
 import mns_scheduler.finance.financial_high_risk_stock_clean_service_api as financial_high_risk_stock_clean_service_api
 import mns_common.utils.data_frame_util as data_frame_util
+import mns_scheduler.finance.finance_common_api as finance_common_api
 
 mongodb_util = MongodbUtil('27017')
 
 
 # 上市公司年报披露时间:每年1月1日一- 4月30日。
 # 2、上市公司中年报披露时间:每年7月1日--8月30日。
 # 3、上市公司季报披露时间:
@@ -32,43 +32,44 @@
     now_year = now_date.year
     now_month = now_date.month
     sync_time = now_date.strftime('%Y-%m-%d %H:%M:%S')
     # 年报
     if 1 <= now_month <= 5:
         period = 4
         period_time = str(now_year - 1) + "-12-31 00:00:00"
-        sync_profit_report(period_time, sync_time, period, now_year)
-        sync_asset_liability_report(period_time, sync_time, period, now_year)
+        sync_profit_report(period_time, sync_time, period)
+        sync_asset_liability_report(period_time, sync_time, period)
 
     # 一季报
     elif now_month == 5:
         period = 1
         period_time = str(now_year) + "-03-31 00:00:00"
-        sync_profit_report(period_time, sync_time, period, now_year)
-        sync_asset_liability_report(period_time, sync_time, period, now_year)
+        sync_profit_report(period_time, sync_time, period)
+        sync_asset_liability_report(period_time, sync_time, period)
 
     # 二季报
     elif 7 <= now_month <= 8:
         period = 2
         period_time = str(now_year) + "-06-30 00:00:00"
-        sync_profit_report(period_time, sync_time, period, now_year)
-        sync_asset_liability_report(period_time, sync_time, period, now_year)
+        sync_profit_report(period_time, sync_time, period)
+        sync_asset_liability_report(period_time, sync_time, period)
     # 三季报
     elif now_month == 10:
         period = 3
         period_time = str(now_year) + "-09-30 00:00:00"
-        sync_profit_report(period_time, sync_time, period, now_year)
-        sync_asset_liability_report(period_time, sync_time, period, now_year)
+        sync_profit_report(period_time, sync_time, period)
+        sync_asset_liability_report(period_time, sync_time, period)
     # 未出报告check
     financial_high_risk_stock_clean_service_api.un_report_check(sync_time, now_year, period, period_time)
 
 
 # 同步资产表
-def sync_asset_liability_report(period_time, sync_time, period, now_year):
-    un_report_asset_df = find_un_report_symbol(period_time, db_name_constant.EM_STOCK_ASSET_LIABILITY)
+def sync_asset_liability_report(period_time, sync_time, period):
+    un_report_asset_df = finance_common_api.find_un_report_symbol(period_time,
+                                                                  db_name_constant.EM_STOCK_ASSET_LIABILITY)
     for un_report_asset_one in un_report_asset_df.itertuples():
         try:
             symbol = un_report_asset_one.symbol
             new_asset_df = em_financial_asset_liability_sync_service_api.get_em_asset_liability_api(symbol)
             # 负债比
             new_asset_df['liability_ratio'] = round(
                 new_asset_df['TOTAL_LIABILITIES'] * 100 / new_asset_df['TOTAL_ASSETS'],
@@ -80,54 +81,33 @@
             mongodb_util.insert_mongo(new_asset_df, db_name_constant.EM_STOCK_ASSET_LIABILITY)
 
             # 年报审核
             financial_high_risk_stock_clean_service_api.financial_report_check(new_asset_df, period_time, period,
                                                                                db_name_constant.EM_STOCK_ASSET_LIABILITY)
 
         except Exception as e:
-            logger.error("同步利润表异常:{},{},{}", symbol, period_time, e)
+            logger.error("同步资产表异常:{},{},{}", symbol, period_time, e)
 
 
 # 同步利润表
-def sync_profit_report(period_time, sync_time, period, now_year):
-    un_report_profit_df = find_un_report_symbol(period_time, db_name_constant.EM_STOCK_PROFIT)
+def sync_profit_report(period_time, sync_time, period):
+    un_report_profit_df = finance_common_api.find_un_report_symbol(period_time, db_name_constant.EM_STOCK_PROFIT)
     for un_report_profit_one in un_report_profit_df.itertuples():
         try:
             symbol = un_report_profit_one.symbol
             new_profit_df = em_financial_profit_sync_service_api.get_em_profit_api(symbol)
-            new_profit_df['sync_time'] = sync_time
             if data_frame_util.is_empty(new_profit_df):
                 continue
+            new_profit_df['sync_time'] = sync_time
+
             new_profit_df['symbol'] = symbol
             mongodb_util.insert_mongo(new_profit_df, db_name_constant.EM_STOCK_PROFIT)
 
             # 年报审核
             financial_high_risk_stock_clean_service_api.financial_report_check(new_profit_df, period_time,
                                                                                period, db_name_constant.EM_STOCK_PROFIT)
         except Exception as e:
             logger.error("同步利润表异常:{},{},{}", symbol, period_time, e)
 
 
-# 查出未报告的股票
-def find_un_report_symbol(period_time, report_name):
-    real_time_quotes_df = east_money_stock_api.get_real_time_quotes_all_stocks()
-    real_time_quotes_df = real_time_quotes_df.loc[~(real_time_quotes_df['name'].str.contains('退'))]
-
-    de_list_stock_df = mongodb_util.find_all_data(db_name_constant.DE_LIST_STOCK)
-    real_time_quotes_df = real_time_quotes_df.loc[
-        ~(real_time_quotes_df['symbol'].isin(list(de_list_stock_df['symbol'])))]
-
-    if report_name == db_name_constant.EM_STOCK_ASSET_LIABILITY:
-        had_asset_df = finance_common_api.find_asset_liability_report(period_time)
-        if data_frame_util.is_not_empty(had_asset_df):
-            real_time_quotes_df = real_time_quotes_df.loc[
-                ~(real_time_quotes_df['symbol'].isin(list(had_asset_df['SECURITY_CODE'])))]
-    if report_name == db_name_constant.EM_STOCK_PROFIT:
-        had_profit_df = finance_common_api.find_profit_report(period_time)
-        if data_frame_util.is_not_empty(had_profit_df):
-            real_time_quotes_df = real_time_quotes_df.loc[
-                ~(real_time_quotes_df['symbol'].isin(list(had_profit_df['SECURITY_CODE'])))]
-    return real_time_quotes_df
-
-
 if __name__ == '__main__':
     sync_financial_report()
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.5.1/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/risk/register_and_investigate_stock_sync_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/risk/register_and_investigate_stock_sync_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,18 @@
     const_num = 30
     init_date = datetime.now()
     str_day = init_date.strftime('%Y-%m-%d')
     # 过去30天新增风险股票
     begin_date = date_handle_util.add_date_day(date_handle_util.no_slash_date(str_day), -before_days)
     begin_day = begin_date.strftime('%Y-%m-%d')
     search_key = '立案'
-    new_high_risk_stocks_df = sync_all_investigate_stocks(const_num, search_key, begin_day, str_day)
+
+    end_date = date_handle_util.add_date_day(date_handle_util.no_slash_date(str_day), 1)
+    end_day = end_date.strftime('%Y-%m-%d')
+    new_high_risk_stocks_df = sync_all_investigate_stocks(const_num, search_key, begin_day, end_day)
     if data_frame_util.is_empty(new_high_risk_stocks_df):
         return None
     new_high_risk_stocks_df = new_high_risk_stocks_df.sort_values(by=['announcementTime'], ascending=False)
     for high_risk_stocks_one in new_high_risk_stocks_df.itertuples():
         try:
             symbol = high_risk_stocks_one.secCode
             announcement_id = high_risk_stocks_one.announcementId
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             miss_symbol_list = list(stock_high_chg_pool_df['symbol'])
             sync_all_kc_zt_data(str_day, miss_symbol_list)
         except BaseException as e:
             logger.error("发生异常:{},{}", str_day, e)
 
 
 if __name__ == '__main__':
-    sync_all_kc_zt_data('2024-05-10', None)
+    sync_all_kc_zt_data('2024-05-17', None)
     # sync_all_kc_zt_data('2023-08-16')
     # sync_all_kc_zt_data('2023-07-07')
     # realtime_quotes_now_zt_new_kc_open_sync()
     # hui_ce_all('2023-06-16')
     # fix_diff_day()
     # sync_all_kc_zt_data('2023-06-30')
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
             logger.info("更新高涨幅数据成功{},{}", stock_one.symbol, str_day)
         except Exception as e:
             logger.error("更新高涨幅数据异常:{},{},{}", stock_one.symbol, str_day, e)
             continue
 
 
 if __name__ == '__main__':
-    sync_one_day_zt_info('2022-06-28')
+    sync_one_day_zt_info('2024-05-17')
 
     # sync_date = date_handle_util.add_date_day('20221022', 0)
     # now_date = datetime.now()
     # str_now_day = sync_date.strftime('%Y-%m-%d')
     # while now_date > sync_date:
     #     try:
     #         save_one_symbol_day('000948', str_now_day)
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,14 +391,14 @@
 # 更新开盘啦指数关系
 blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='18,22', minute='25')
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(sync_position, 'cron', hour='0,08', minute='10')
 
 # 同步被立案调查的股票
-blockingScheduler.add_job(sync_new_high_risk_stocks, 'cron', hour='0,09', minute='20')
+blockingScheduler.add_job(sync_new_high_risk_stocks, 'cron', hour='0,09,12,16', minute='20')
 
 print('定时任务启动成功')
 blockingScheduler.start()
 #
 # if __name__ == '__main__':
 #     sync_kpl_best_his_quotes()
```

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.5.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.9/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.5.1/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 mns_scheduler/dt/stock_dt_pool_sync.py
 mns_scheduler/finance/__init__.py
 mns_scheduler/finance/em_financial_asset_liability_sync_service_api.py
 mns_scheduler/finance/em_financial_profit_sync_service_api.py
 mns_scheduler/finance/finance_common_api.py
 mns_scheduler/finance/financial_high_risk_stock_clean_service_api.py
 mns_scheduler/finance/sync_financial_report_service_api.py
+mns_scheduler/finance/test/__init__.py
+mns_scheduler/finance/test/fix_blask_list.py
+mns_scheduler/hk/__init__.py
+mns_scheduler/hk/hk_company_info_sync_service_api.py
 mns_scheduler/k_line/__init__.py
 mns_scheduler/k_line/clean/__init__.py
 mns_scheduler/k_line/clean/k_line_info_clean_impl.py
 mns_scheduler/k_line/clean/k_line_info_clean_service.py
 mns_scheduler/k_line/sync/__init__.py
 mns_scheduler/k_line/sync/daily_week_month_line_sync.py
 mns_scheduler/kpl/__init__.py
```

