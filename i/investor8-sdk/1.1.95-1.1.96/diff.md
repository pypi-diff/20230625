# Comparing `tmp/investor8-sdk-1.1.95.tar.gz` & `tmp/investor8-sdk-1.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investor8-sdk-1.1.95.tar", last modified: Sat Jun 24 09:14:01 2023, max compression
+gzip compressed data, was "investor8-sdk-1.1.96.tar", last modified: Sat Jun 24 21:57:19 2023, max compression
```

## Comparing `investor8-sdk-1.1.95.tar` & `investor8-sdk-1.1.96.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:14:01.365389 investor8-sdk-1.1.95/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    27394 2023-06-24 09:14:01.365389 investor8-sdk-1.1.95/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    26761 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/README.md
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:14:01.037372 investor8-sdk-1.1.95/investor8_sdk/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8381 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/__init__.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:14:01.045372 investor8-sdk-1.1.95/investor8_sdk/api/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      663 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21896 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/earnings_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2022-01-02 07:37:24.000000 investor8-sdk-1.1.95/investor8_sdk/api/email_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    37163 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/financials_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)   105383 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/metrics_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    55709 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/news_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21615 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/price_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25818 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/screener_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4737 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/search_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10888 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/settings_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    60662 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/stock_info_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11021 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/tags_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    62859 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api/user_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25090 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/api_client.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8523 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/configuration.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:14:01.129377 investor8-sdk-1.1.95/investor8_sdk/models/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7655 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/models/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3705 2023-06-24 09:13:55.000000 investor8-sdk-1.1.95/investor8_sdk/models/active_company_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3882 2023-06-24 09:13:55.000000 investor8-sdk-1.1.95/investor8_sdk/models/add_to_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6948 2023-06-24 09:13:55.000000 investor8-sdk-1.1.95/investor8_sdk/models/authentication_request.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2564 2023-06-24 09:13:55.000000 investor8-sdk-1.1.95/investor8_sdk/models/authentication_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3992 2022-01-02 07:37:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/authorize_account_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3398 2022-01-02 07:37:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/authorize_account_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4982 2022-01-02 07:37:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/change_password_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8307 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/company_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3776 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_auth_req_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9701 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4679 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_screen_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2022-01-02 07:37:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_update_news.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12576 2022-01-02 07:37:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11840 2022-01-02 07:37:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_user_res_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4682 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/create_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3967 2022-05-17 22:57:20.000000 investor8-sdk-1.1.95/investor8_sdk/models/current_metadat_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15390 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17728 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/current_momentum_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6663 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/daily_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11983 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/detailed_latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2622 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/discovery_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22123 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/earning_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2022-01-02 07:37:22.000000 investor8-sdk-1.1.95/investor8_sdk/models/email_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14737 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/financial_metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6287 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/financial_report_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13652 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/financial_tag.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4336 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/financials_growth.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5399 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_list_metric_views_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5489 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_list_metrics_description_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15038 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_list_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5068 2023-05-27 12:46:09.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_list_metrics_screening_conditions_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7316 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_metric_view_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17044 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3856 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_screens_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3961 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/get_watchlists_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8020 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_daily_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5353 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3996 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_indicator_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4102 2022-05-17 22:57:21.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_metadata_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4699 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_metric_value_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10253 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_return.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5663 2023-06-24 09:13:56.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_returns_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6659 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/historical_value_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2551 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/history_length.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5161 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/i8_terminal_check_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4174 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/i8_terminal_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4210 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/i8_terminal_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4991 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/latest_financial_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4996 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/latest_financials_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4691 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/latest_financials_with_growth_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9535 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3881 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/list_exchange_sector_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7221 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/log_terminal_usage.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3888 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/login_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3963 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/login_with_code_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2022-01-02 07:37:22.000000 investor8-sdk-1.1.95/investor8_sdk/models/market_highlight.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10246 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/market_highlight_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2594 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/market_highlight_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6192 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/metadata_properties_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3868 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/metric_group_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11975 2022-04-10 12:05:22.000000 investor8-sdk-1.1.95/investor8_sdk/models/metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3772 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/metric_name_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5539 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7972 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/metrics_by_period_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14094 2023-03-19 11:02:32.000000 investor8-sdk-1.1.95/investor8_sdk/models/metrics_metadata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6618 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/metrics_metadata_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6294 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/momentum_metric_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4536 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/monthly_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3826 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/monthly_returns.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4191 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/news_categories_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2537 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/news_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3743 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/period_metric_value.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/period_return.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11050 2022-01-02 07:37:22.000000 investor8-sdk-1.1.95/investor8_sdk/models/plot_detail_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10058 2022-01-02 07:37:22.000000 investor8-sdk-1.1.95/investor8_sdk/models/plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3633 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/plot_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3977 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/previous_close_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2541 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/profile_name.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16061 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/recent_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3903 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/remove_from_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3792 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/rename_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2525 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/req_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4019 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/reset_password_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4476 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/result_field.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7256 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/return_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20474 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/sa_attributes_prices.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5293 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/sa_sector_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6333 2023-06-24 09:13:57.000000 investor8-sdk-1.1.95/investor8_sdk/models/screen.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5793 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/screen_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4230 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/screening_category_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4529 2023-05-27 12:46:10.000000 investor8-sdk-1.1.95/investor8_sdk/models/screening_condition.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4577 2023-05-27 12:46:10.000000 investor8-sdk-1.1.95/investor8_sdk/models/screening_condition_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3770 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/sector_returns_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5585 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/send_email_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11239 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/standardized_financial.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19718 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12763 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_financial.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5181 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7661 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15908 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_info_master_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16468 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_ipo.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17068 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_news.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19810 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_news_details.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2583 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_news_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10969 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_popularity_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4356 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_popularity_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7177 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_price.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11136 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11193 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_rating_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19887 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/stock_summary_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/string_message_result.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3988 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/symbols_current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4111 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/symbols_historical_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8621 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/tag_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5876 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/tag_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7157 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/terminal_log_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4015 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/terminal_log_os_versions_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6951 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/trading_calendar_details_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17515 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/upcoming_earning_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5651 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/update_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11673 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/user.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19274 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4052 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/validate_watchlist_name_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2022-01-02 07:37:23.000000 investor8-sdk-1.1.95/investor8_sdk/models/validate_watchlist_name_response_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5043 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/value_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3156 2022-01-02 07:37:24.000000 investor8-sdk-1.1.95/investor8_sdk/models/view_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5532 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/watchlist.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4968 2023-06-24 09:13:58.000000 investor8-sdk-1.1.95/investor8_sdk/models/watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13045 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/investor8_sdk/rest.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:14:01.041372 investor8-sdk-1.1.95/investor8_sdk.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    27394 2023-06-24 09:14:00.000000 investor8-sdk-1.1.95/investor8_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11127 2023-06-24 09:14:00.000000 investor8-sdk-1.1.95/investor8_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2023-06-24 09:14:00.000000 investor8-sdk-1.1.95/investor8_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       64 2023-06-24 09:14:00.000000 investor8-sdk-1.1.95/investor8_sdk.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       19 2023-06-24 09:14:00.000000 investor8-sdk-1.1.95/investor8_sdk.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2023-06-24 09:14:01.365389 investor8-sdk-1.1.95/setup.cfg
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1585 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/setup.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:14:01.361389 investor8-sdk-1.1.95/test/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 09:13:59.000000 investor8-sdk-1.1.95/test/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-02-07 12:25:08.000000 investor8-sdk-1.1.95/test/test_active_company_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      959 2021-11-22 21:48:03.000000 investor8-sdk-1.1.95/test/test_add_to_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:00.000000 investor8-sdk-1.1.95/test/test_authentication_request.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-12-22 22:21:41.000000 investor8-sdk-1.1.95/test/test_authentication_source.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2021-12-14 09:16:29.000000 investor8-sdk-1.1.95/test/test_authorize_account_request_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2021-12-14 09:16:29.000000 investor8-sdk-1.1.95/test/test_authorize_account_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:00.000000 investor8-sdk-1.1.95/test/test_change_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_company_info_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-12 18:39:44.000000 investor8-sdk-1.1.95/test/test_create_auth_req_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:03.000000 investor8-sdk-1.1.95/test/test_create_plot_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      962 2023-01-09 08:00:15.000000 investor8-sdk-1.1.95/test/test_create_screen_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_create_update_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_create_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-24 20:49:06.000000 investor8-sdk-1.1.95/test/test_create_user_res_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:40.000000 investor8-sdk-1.1.95/test/test_create_watchlist_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-11 07:51:15.000000 investor8-sdk-1.1.95/test/test_current_metadat_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-02-21 08:35:39.000000 investor8-sdk-1.1.95/test/test_current_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_current_momentum_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_detailed_latest_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-07-24 00:19:52.000000 investor8-sdk-1.1.95/test/test_discovery_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_earning_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1386 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_earnings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_email_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_email_type.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-04-11 12:06:05.000000 investor8-sdk-1.1.95/test/test_financial_metric_metadata_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_financial_report_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_financial_tag.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1900 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_financials_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_financials_growth.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1014 2023-06-13 21:07:21.000000 investor8-sdk-1.1.95/test/test_get_list_metric_views_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1070 2023-06-14 06:22:27.000000 investor8-sdk-1.1.95/test/test_get_list_metrics_description_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1046 2023-04-06 07:43:55.000000 investor8-sdk-1.1.95/test/test_get_list_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1136 2023-05-20 08:09:03.000000 investor8-sdk-1.1.95/test/test_get_list_metrics_screening_conditions_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      972 2023-06-13 21:07:21.000000 investor8-sdk-1.1.95/test/test_get_metric_view_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1012 2023-04-06 07:43:55.000000 investor8-sdk-1.1.95/test/test_get_metrics_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      998 2023-01-09 08:00:16.000000 investor8-sdk-1.1.95/test/test_get_screens_by_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      943 2021-10-29 23:03:04.000000 investor8-sdk-1.1.95/test/test_get_user_plots_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1001 2021-10-20 06:52:41.000000 investor8-sdk-1.1.95/test/test_get_watchlists_by_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-28 01:16:15.000000 investor8-sdk-1.1.95/test/test_historical_daily_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1027 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_historical_financial_metrics.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2022-01-04 11:42:54.000000 investor8-sdk-1.1.95/test/test_historical_indicator_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1047 2022-05-11 07:51:16.000000 investor8-sdk-1.1.95/test/test_historical_metadata_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-11 07:51:16.000000 investor8-sdk-1.1.95/test/test_historical_metric_value_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_historical_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_historical_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_historical_value_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_history_length.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1025 2022-03-12 13:22:27.000000 investor8-sdk-1.1.95/test/test_i8_terminal_check_version_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-03-09 08:58:36.000000 investor8-sdk-1.1.95/test/test_i8_terminal_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      983 2022-03-09 08:58:36.000000 investor8-sdk-1.1.95/test/test_i8_terminal_version_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_latest_financial_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:01.000000 investor8-sdk-1.1.95/test/test_latest_financials_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1055 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_latest_financials_with_growth_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_latest_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_list_exchange_sector_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-04-10 12:05:22.000000 investor8-sdk-1.1.95/test/test_log_terminal_usage.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_login_user_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-13 18:18:13.000000 investor8-sdk-1.1.95/test/test_login_with_code_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      937 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_market_highlight.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_market_highlight_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_market_highlight_status.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2022-04-11 12:06:05.000000 investor8-sdk-1.1.95/test/test_metadata_properties_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      954 2023-06-13 21:07:22.000000 investor8-sdk-1.1.95/test/test_metric_group_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2021-12-05 23:31:58.000000 investor8-sdk-1.1.95/test/test_metric_metadata_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      946 2023-06-13 21:07:22.000000 investor8-sdk-1.1.95/test/test_metric_name_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      871 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2455 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_metrics_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      988 2023-05-07 19:23:44.000000 investor8-sdk-1.1.95/test/test_metrics_by_period_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-04-11 12:06:06.000000 investor8-sdk-1.1.95/test/test_metrics_metadata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-05-11 07:51:16.000000 investor8-sdk-1.1.95/test/test_metrics_metadata_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_momentum_metric_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_monthly_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_monthly_returns.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2988 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_news_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_news_categories_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_news_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_period_metric_value.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_period_return.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      849 2021-10-29 23:03:05.000000 investor8-sdk-1.1.95/test/test_plot.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-11-10 20:39:48.000000 investor8-sdk-1.1.95/test/test_plot_detail_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      875 2021-10-29 23:03:05.000000 investor8-sdk-1.1.95/test/test_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      941 2021-11-01 09:44:52.000000 investor8-sdk-1.1.95/test/test_plot_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_previous_close_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1267 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_price_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_profile_name.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_recent_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      999 2021-11-24 17:08:48.000000 investor8-sdk-1.1.95/test/test_remove_from_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-11-24 17:08:48.000000 investor8-sdk-1.1.95/test/test_rename_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_req_type.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_reset_password_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_result_field.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_return_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_sa_attributes_prices.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_sa_sector_price_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      886 2023-01-09 08:00:17.000000 investor8-sdk-1.1.95/test/test_screen.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      912 2023-01-09 08:00:17.000000 investor8-sdk-1.1.95/test/test_screen_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1374 2021-10-01 15:22:04.000000 investor8-sdk-1.1.95/test/test_screener_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1002 2023-06-18 14:47:27.000000 investor8-sdk-1.1.95/test/test_screening_category_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1002 2022-10-17 20:31:24.000000 investor8-sdk-1.1.95/test/test_screening_condition.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1010 2023-05-20 08:09:05.000000 investor8-sdk-1.1.95/test/test_screening_condition_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      790 2021-10-01 15:22:04.000000 investor8-sdk-1.1.95/test/test_search_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_sector_returns_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_send_email_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      910 2022-03-09 08:58:38.000000 investor8-sdk-1.1.95/test/test_settings_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_standardized_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_stock_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_stock_financial.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_stock_financial_metrics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2416 2021-10-01 15:22:04.000000 investor8-sdk-1.1.95/test/test_stock_info_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_stock_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_stock_info_master_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:02.000000 investor8-sdk-1.1.95/test/test_stock_ipo.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_news.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_news_details.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_news_status.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_popularity_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_popularity_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_price.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-13 20:41:56.000000 investor8-sdk-1.1.95/test/test_stock_price_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_rating_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_stock_summary_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_string_message_result.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-28 11:55:23.000000 investor8-sdk-1.1.95/test/test_symbols_current_metrics_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2022-05-28 11:55:23.000000 investor8-sdk-1.1.95/test/test_symbols_historical_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_tag_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      899 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_tag_info_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1004 2021-10-01 15:22:04.000000 investor8-sdk-1.1.95/test/test_tags_api.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      933 2022-04-23 22:58:49.000000 investor8-sdk-1.1.95/test/test_terminal_log_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1017 2022-04-26 22:55:39.000000 investor8-sdk-1.1.95/test/test_terminal_log_os_versions_dto.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-01 22:19:51.000000 investor8-sdk-1.1.95/test/test_trading_calendar_details_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_upcoming_earning_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:06.000000 investor8-sdk-1.1.95/test/test_update_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:42.000000 investor8-sdk-1.1.95/test/test_update_watchlist_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      847 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_user.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2280 2021-10-01 15:22:04.000000 investor8-sdk-1.1.95/test/test_user_api.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_user_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1073 2021-10-31 21:17:37.000000 investor8-sdk-1.1.95/test/test_validate_watchlist_name_request_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1081 2021-10-31 21:17:37.000000 investor8-sdk-1.1.95/test/test_validate_watchlist_name_response_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.95/test/test_value_metrics_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      909 2021-10-29 23:03:06.000000 investor8-sdk-1.1.95/test/test_view_plot_dto.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-20 06:52:42.000000 investor8-sdk-1.1.95/test/test_watchlist.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-20 06:52:42.000000 investor8-sdk-1.1.95/test/test_watchlist_dto.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:19.330856 investor8-sdk-1.1.96/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    27394 2023-06-24 21:57:19.330856 investor8-sdk-1.1.96/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    26761 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/README.md
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:19.026840 investor8-sdk-1.1.96/investor8_sdk/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8381 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:19.034841 investor8-sdk-1.1.96/investor8_sdk/api/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      663 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21896 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/api/earnings_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7158 2022-01-02 07:37:24.000000 investor8-sdk-1.1.96/investor8_sdk/api/email_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    37163 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/api/financials_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)   105383 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/api/metrics_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    55709 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/news_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    21615 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/price_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25818 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/screener_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4737 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/search_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10888 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/settings_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    60662 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/stock_info_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11021 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/tags_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    62859 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api/user_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    25090 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/api_client.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8523 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/configuration.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:19.106844 investor8-sdk-1.1.96/investor8_sdk/models/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7655 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/models/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4336 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/active_company_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3882 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/add_to_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6948 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/authentication_request.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2564 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/authentication_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3992 2022-01-02 07:37:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/authorize_account_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3398 2022-01-02 07:37:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/authorize_account_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4982 2022-01-02 07:37:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/change_password_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8307 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/company_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3776 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_auth_req_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9701 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4679 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_screen_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19633 2022-01-02 07:37:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_update_news.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12576 2022-01-02 07:37:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11840 2022-01-02 07:37:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_user_res_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4682 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/create_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3967 2022-05-17 22:57:20.000000 investor8-sdk-1.1.96/investor8_sdk/models/current_metadat_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15390 2023-06-24 21:57:12.000000 investor8-sdk-1.1.96/investor8_sdk/models/current_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17728 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/current_momentum_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6663 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/daily_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11983 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/detailed_latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2622 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/discovery_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    22123 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/earning_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2512 2022-01-02 07:37:22.000000 investor8-sdk-1.1.96/investor8_sdk/models/email_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14737 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/financial_metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6287 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/financial_report_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13652 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/financial_tag.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4336 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/financials_growth.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5399 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_list_metric_views_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5489 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_list_metrics_description_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15038 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_list_metrics_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5068 2023-05-27 12:46:09.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_list_metrics_screening_conditions_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7316 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_metric_view_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17044 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_metrics_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3856 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_screens_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3961 2023-06-24 21:57:13.000000 investor8-sdk-1.1.96/investor8_sdk/models/get_watchlists_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8020 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_daily_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5353 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3996 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_indicator_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4102 2022-05-17 22:57:21.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_metadata_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4699 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_metric_value_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10253 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_return.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5663 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_returns_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6659 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/historical_value_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2551 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/history_length.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5161 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/i8_terminal_check_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4174 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/i8_terminal_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4210 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/i8_terminal_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4991 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/latest_financial_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4996 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/latest_financials_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4691 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/latest_financials_with_growth_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9535 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3881 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/list_exchange_sector_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7221 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/log_terminal_usage.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3888 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/login_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3963 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/login_with_code_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9111 2022-01-02 07:37:22.000000 investor8-sdk-1.1.96/investor8_sdk/models/market_highlight.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10246 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/market_highlight_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2594 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/market_highlight_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6192 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/metadata_properties_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3868 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/metric_group_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11975 2022-04-10 12:05:22.000000 investor8-sdk-1.1.96/investor8_sdk/models/metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3772 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/metric_name_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5539 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7972 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/metrics_by_period_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14094 2023-03-19 11:02:32.000000 investor8-sdk-1.1.96/investor8_sdk/models/metrics_metadata.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6618 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/metrics_metadata_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6294 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/momentum_metric_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4536 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/monthly_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3826 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/monthly_returns.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4191 2023-06-24 21:57:14.000000 investor8-sdk-1.1.96/investor8_sdk/models/news_categories_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2537 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/news_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3743 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/period_metric_value.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3722 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/period_return.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11050 2022-01-02 07:37:22.000000 investor8-sdk-1.1.96/investor8_sdk/models/plot_detail_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10058 2022-01-02 07:37:22.000000 investor8-sdk-1.1.96/investor8_sdk/models/plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3633 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/plot_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3977 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/previous_close_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2541 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/profile_name.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16061 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/recent_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3903 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/remove_from_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3792 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/rename_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2525 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/req_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4019 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/reset_password_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4476 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/result_field.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7256 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/return_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20474 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/sa_attributes_prices.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5293 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/sa_sector_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6333 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/screen.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5793 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/screen_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4230 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/screening_category_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4529 2023-05-27 12:46:10.000000 investor8-sdk-1.1.96/investor8_sdk/models/screening_condition.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4577 2023-05-27 12:46:10.000000 investor8-sdk-1.1.96/investor8_sdk/models/screening_condition_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3770 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/sector_returns_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5585 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/send_email_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11239 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/standardized_financial.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19718 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    12763 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_financial.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5181 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8276 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15908 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_info_master_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    16468 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_ipo.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17068 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_news.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19810 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_news_details.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2583 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_news_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10969 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_popularity_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4356 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_popularity_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7177 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_price.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11136 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11193 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_rating_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19887 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/stock_summary_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3135 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/string_message_result.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3988 2023-06-24 21:57:15.000000 investor8-sdk-1.1.96/investor8_sdk/models/symbols_current_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4111 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/symbols_historical_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8621 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/tag_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5876 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/tag_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7157 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/terminal_log_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4015 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/terminal_log_os_versions_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6951 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/trading_calendar_details_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    17515 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/upcoming_earning_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5651 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/update_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11673 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/user.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    19274 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4052 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/validate_watchlist_name_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3261 2022-01-02 07:37:23.000000 investor8-sdk-1.1.96/investor8_sdk/models/validate_watchlist_name_response_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5043 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/value_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3156 2022-01-02 07:37:24.000000 investor8-sdk-1.1.96/investor8_sdk/models/view_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5532 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/watchlist.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4968 2023-06-24 21:57:16.000000 investor8-sdk-1.1.96/investor8_sdk/models/watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    13045 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/investor8_sdk/rest.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:19.026840 investor8-sdk-1.1.96/investor8_sdk.egg-info/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    27394 2023-06-24 21:57:18.000000 investor8-sdk-1.1.96/investor8_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)    11127 2023-06-24 21:57:18.000000 investor8-sdk-1.1.96/investor8_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2023-06-24 21:57:18.000000 investor8-sdk-1.1.96/investor8_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       64 2023-06-24 21:57:18.000000 investor8-sdk-1.1.96/investor8_sdk.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       19 2023-06-24 21:57:18.000000 investor8-sdk-1.1.96/investor8_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2023-06-24 21:57:19.330856 investor8-sdk-1.1.96/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1585 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/setup.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:19.326856 investor8-sdk-1.1.96/test/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-06-24 21:57:17.000000 investor8-sdk-1.1.96/test/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-02-07 12:25:08.000000 investor8-sdk-1.1.96/test/test_active_company_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      959 2021-11-22 21:48:03.000000 investor8-sdk-1.1.96/test/test_add_to_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:00.000000 investor8-sdk-1.1.96/test/test_authentication_request.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-12-22 22:21:41.000000 investor8-sdk-1.1.96/test/test_authentication_source.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2021-12-14 09:16:29.000000 investor8-sdk-1.1.96/test/test_authorize_account_request_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2021-12-14 09:16:29.000000 investor8-sdk-1.1.96/test/test_authorize_account_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:00.000000 investor8-sdk-1.1.96/test/test_change_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_company_info_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-12 18:39:44.000000 investor8-sdk-1.1.96/test/test_create_auth_req_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:03.000000 investor8-sdk-1.1.96/test/test_create_plot_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      962 2023-01-09 08:00:15.000000 investor8-sdk-1.1.96/test/test_create_screen_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_create_update_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_create_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-24 20:49:06.000000 investor8-sdk-1.1.96/test/test_create_user_res_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:40.000000 investor8-sdk-1.1.96/test/test_create_watchlist_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-11 07:51:15.000000 investor8-sdk-1.1.96/test/test_current_metadat_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-02-21 08:35:39.000000 investor8-sdk-1.1.96/test/test_current_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_current_momentum_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_detailed_latest_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-07-24 00:19:52.000000 investor8-sdk-1.1.96/test/test_discovery_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_earning_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1386 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_earnings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_email_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_email_type.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-04-11 12:06:05.000000 investor8-sdk-1.1.96/test/test_financial_metric_metadata_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_financial_report_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_financial_tag.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1900 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_financials_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_financials_growth.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1014 2023-06-13 21:07:21.000000 investor8-sdk-1.1.96/test/test_get_list_metric_views_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1070 2023-06-14 06:22:27.000000 investor8-sdk-1.1.96/test/test_get_list_metrics_description_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1046 2023-04-06 07:43:55.000000 investor8-sdk-1.1.96/test/test_get_list_metrics_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1136 2023-05-20 08:09:03.000000 investor8-sdk-1.1.96/test/test_get_list_metrics_screening_conditions_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      972 2023-06-13 21:07:21.000000 investor8-sdk-1.1.96/test/test_get_metric_view_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1012 2023-04-06 07:43:55.000000 investor8-sdk-1.1.96/test/test_get_metrics_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      998 2023-01-09 08:00:16.000000 investor8-sdk-1.1.96/test/test_get_screens_by_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      943 2021-10-29 23:03:04.000000 investor8-sdk-1.1.96/test/test_get_user_plots_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1001 2021-10-20 06:52:41.000000 investor8-sdk-1.1.96/test/test_get_watchlists_by_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-28 01:16:15.000000 investor8-sdk-1.1.96/test/test_historical_daily_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1027 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_historical_financial_metrics.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      997 2022-01-04 11:42:54.000000 investor8-sdk-1.1.96/test/test_historical_indicator_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1047 2022-05-11 07:51:16.000000 investor8-sdk-1.1.96/test/test_historical_metadata_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-11 07:51:16.000000 investor8-sdk-1.1.96/test/test_historical_metric_value_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      945 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_historical_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      979 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_historical_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      995 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_historical_value_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_history_length.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1025 2022-03-12 13:22:27.000000 investor8-sdk-1.1.96/test/test_i8_terminal_check_version_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2022-03-09 08:58:36.000000 investor8-sdk-1.1.96/test/test_i8_terminal_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      983 2022-03-09 08:58:36.000000 investor8-sdk-1.1.96/test/test_i8_terminal_version_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_latest_financial_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:01.000000 investor8-sdk-1.1.96/test/test_latest_financials_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1055 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_latest_financials_with_growth_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_latest_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_list_exchange_sector_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2022-04-10 12:05:22.000000 investor8-sdk-1.1.96/test/test_log_terminal_usage.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_login_user_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      951 2021-12-13 18:18:13.000000 investor8-sdk-1.1.96/test/test_login_with_code_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      937 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_market_highlight.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_market_highlight_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_market_highlight_status.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      989 2022-04-11 12:06:05.000000 investor8-sdk-1.1.96/test/test_metadata_properties_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      954 2023-06-13 21:07:22.000000 investor8-sdk-1.1.96/test/test_metric_group_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      957 2021-12-05 23:31:58.000000 investor8-sdk-1.1.96/test/test_metric_metadata_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      946 2023-06-13 21:07:22.000000 investor8-sdk-1.1.96/test/test_metric_name_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      871 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2455 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_metrics_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      988 2023-05-07 19:23:44.000000 investor8-sdk-1.1.96/test/test_metrics_by_period_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2022-04-11 12:06:06.000000 investor8-sdk-1.1.96/test/test_metrics_metadata.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1031 2022-05-11 07:51:16.000000 investor8-sdk-1.1.96/test/test_metrics_metadata_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_momentum_metric_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_monthly_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_monthly_returns.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2988 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_news_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_news_categories_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_news_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      955 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_period_metric_value.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      913 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_period_return.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      849 2021-10-29 23:03:05.000000 investor8-sdk-1.1.96/test/test_plot.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-11-10 20:39:48.000000 investor8-sdk-1.1.96/test/test_plot_detail_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      875 2021-10-29 23:03:05.000000 investor8-sdk-1.1.96/test/test_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      941 2021-11-01 09:44:52.000000 investor8-sdk-1.1.96/test/test_plot_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_previous_close_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1267 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_price_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_profile_name.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_recent_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      999 2021-11-24 17:08:48.000000 investor8-sdk-1.1.96/test/test_remove_from_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-11-24 17:08:48.000000 investor8-sdk-1.1.96/test/test_rename_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_req_type.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_reset_password_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      905 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_result_field.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      921 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_return_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_sa_attributes_prices.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      949 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_sa_sector_price_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      886 2023-01-09 08:00:17.000000 investor8-sdk-1.1.96/test/test_screen.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      912 2023-01-09 08:00:17.000000 investor8-sdk-1.1.96/test/test_screen_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1374 2021-10-01 15:22:04.000000 investor8-sdk-1.1.96/test/test_screener_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1002 2023-06-18 14:47:27.000000 investor8-sdk-1.1.96/test/test_screening_category_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1002 2022-10-17 20:31:24.000000 investor8-sdk-1.1.96/test/test_screening_condition.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1010 2023-05-20 08:09:05.000000 investor8-sdk-1.1.96/test/test_screening_condition_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      790 2021-10-01 15:22:04.000000 investor8-sdk-1.1.96/test/test_search_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_sector_returns_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_send_email_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      910 2022-03-09 08:58:38.000000 investor8-sdk-1.1.96/test/test_settings_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      985 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_standardized_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_stock_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      929 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_stock_financial.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      987 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_stock_financial_metrics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2416 2021-10-01 15:22:04.000000 investor8-sdk-1.1.96/test/test_stock_info_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_stock_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_stock_info_master_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      881 2021-10-01 15:22:02.000000 investor8-sdk-1.1.96/test/test_stock_ipo.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_news.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      947 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_news_details.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_news_status.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1021 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_popularity_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_popularity_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      897 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_price.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-13 20:41:56.000000 investor8-sdk-1.1.96/test/test_stock_price_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      931 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_rating_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_stock_summary_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      971 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_string_message_result.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1015 2022-05-28 11:55:23.000000 investor8-sdk-1.1.96/test/test_symbols_current_metrics_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1039 2022-05-28 11:55:23.000000 investor8-sdk-1.1.96/test/test_symbols_historical_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      923 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_tag_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      899 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_tag_info_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1004 2021-10-01 15:22:04.000000 investor8-sdk-1.1.96/test/test_tags_api.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      933 2022-04-23 22:58:49.000000 investor8-sdk-1.1.96/test/test_terminal_log_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1017 2022-04-26 22:55:39.000000 investor8-sdk-1.1.96/test/test_terminal_log_os_versions_dto.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1023 2022-02-01 22:19:51.000000 investor8-sdk-1.1.96/test/test_trading_calendar_details_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      963 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_upcoming_earning_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      925 2021-10-29 23:03:06.000000 investor8-sdk-1.1.96/test/test_update_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      965 2021-10-20 06:52:42.000000 investor8-sdk-1.1.96/test/test_update_watchlist_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      847 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_user.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     2280 2021-10-01 15:22:04.000000 investor8-sdk-1.1.96/test/test_user_api.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      873 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_user_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1073 2021-10-31 21:17:37.000000 investor8-sdk-1.1.96/test/test_validate_watchlist_name_request_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)     1081 2021-10-31 21:17:37.000000 investor8-sdk-1.1.96/test/test_validate_watchlist_name_response_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      939 2021-10-01 15:22:03.000000 investor8-sdk-1.1.96/test/test_value_metrics_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      909 2021-10-29 23:03:06.000000 investor8-sdk-1.1.96/test/test_view_plot_dto.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      889 2021-10-20 06:52:42.000000 investor8-sdk-1.1.96/test/test_watchlist.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (998)      915 2021-10-20 06:52:42.000000 investor8-sdk-1.1.96/test/test_watchlist_dto.py
```

### Comparing `investor8-sdk-1.1.95/PKG-INFO` & `investor8-sdk-1.1.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investor8-sdk
-Version: 1.1.95
+Version: 1.1.96
 Summary: Investoreight Core API
 Home-page: UNKNOWN
 Author-email: info@investoreight.com
 License: UNKNOWN
 Project-URL: Homepage, https://www.investoreight.com/
 Project-URL: Documentation, https://github.com/investoreight/investor8-sdk#readme
 Project-URL: Download, https://github.com/investoreight/investor8-sdk/releases
@@ -16,15 +16,15 @@
 
 # investor8-sdk
 Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
-- Package version: 1.1.95
+- Package version: 1.1.96
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://www.investoreight.com](https://www.investoreight.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `investor8-sdk-1.1.95/README.md` & `investor8-sdk-1.1.96/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # investor8-sdk
 Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
-- Package version: 1.1.95
+- Package version: 1.1.96
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://www.investoreight.com](https://www.investoreight.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk/__init__.py` & `investor8-sdk-1.1.96/investor8_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/__init__.py` & `investor8-sdk-1.1.96/investor8_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/earnings_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/email_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/financials_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/metrics_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/news_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/price_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/screener_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/search_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/settings_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/stock_info_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/tags_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api/user_api.py` & `investor8-sdk-1.1.96/investor8_sdk/api/user_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/api_client.py` & `investor8-sdk-1.1.96/investor8_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.1.95/python'
+        self.user_agent = 'Swagger-Codegen/1.1.96/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk/configuration.py` & `investor8-sdk-1.1.96/investor8_sdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,9 +250,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.1\n"\
-               "SDK Package Version: 1.1.95".\
+               "SDK Package Version: 1.1.96".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/__init__.py` & `investor8-sdk-1.1.96/investor8_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/active_company_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/add_to_watchlist_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ActiveCompanyDto(object):
+class AddToWatchlistDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'ticker': 'str',
-        'name': 'str'
+        'id': 'str',
+        'tickers': 'list[str]'
     }
 
     attribute_map = {
-        'ticker': 'Ticker',
-        'name': 'Name'
+        'id': 'Id',
+        'tickers': 'Tickers'
     }
 
-    def __init__(self, ticker=None, name=None):  # noqa: E501
-        """ActiveCompanyDto - a model defined in Swagger"""  # noqa: E501
-        self._ticker = None
-        self._name = None
+    def __init__(self, id=None, tickers=None):  # noqa: E501
+        """AddToWatchlistDto - a model defined in Swagger"""  # noqa: E501
+        self._id = None
+        self._tickers = None
         self.discriminator = None
-        if ticker is not None:
-            self.ticker = ticker
-        if name is not None:
-            self.name = name
+        self.id = id
+        self.tickers = tickers
 
     @property
-    def ticker(self):
-        """Gets the ticker of this ActiveCompanyDto.  # noqa: E501
+    def id(self):
+        """Gets the id of this AddToWatchlistDto.  # noqa: E501
 
 
-        :return: The ticker of this ActiveCompanyDto.  # noqa: E501
+        :return: The id of this AddToWatchlistDto.  # noqa: E501
         :rtype: str
         """
-        return self._ticker
+        return self._id
 
-    @ticker.setter
-    def ticker(self, ticker):
-        """Sets the ticker of this ActiveCompanyDto.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this AddToWatchlistDto.
 
 
-        :param ticker: The ticker of this ActiveCompanyDto.  # noqa: E501
+        :param id: The id of this AddToWatchlistDto.  # noqa: E501
         :type: str
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._ticker = ticker
+        self._id = id
 
     @property
-    def name(self):
-        """Gets the name of this ActiveCompanyDto.  # noqa: E501
+    def tickers(self):
+        """Gets the tickers of this AddToWatchlistDto.  # noqa: E501
 
 
-        :return: The name of this ActiveCompanyDto.  # noqa: E501
-        :rtype: str
+        :return: The tickers of this AddToWatchlistDto.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._name
+        return self._tickers
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ActiveCompanyDto.
+    @tickers.setter
+    def tickers(self, tickers):
+        """Sets the tickers of this AddToWatchlistDto.
 
 
-        :param name: The name of this ActiveCompanyDto.  # noqa: E501
-        :type: str
+        :param tickers: The tickers of this AddToWatchlistDto.  # noqa: E501
+        :type: list[str]
         """
+        if tickers is None:
+            raise ValueError("Invalid value for `tickers`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._tickers = tickers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ActiveCompanyDto, dict):
+        if issubclass(AddToWatchlistDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ActiveCompanyDto):
+        if not isinstance(other, AddToWatchlistDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/add_to_watchlist_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/active_company_dto.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,89 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class AddToWatchlistDto(object):
+class ActiveCompanyDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'tickers': 'list[str]'
+        'ticker': 'str',
+        'name': 'str',
+        'peers': 'list[str]'
     }
 
     attribute_map = {
-        'id': 'Id',
-        'tickers': 'Tickers'
+        'ticker': 'Ticker',
+        'name': 'Name',
+        'peers': 'Peers'
     }
 
-    def __init__(self, id=None, tickers=None):  # noqa: E501
-        """AddToWatchlistDto - a model defined in Swagger"""  # noqa: E501
-        self._id = None
-        self._tickers = None
+    def __init__(self, ticker=None, name=None, peers=None):  # noqa: E501
+        """ActiveCompanyDto - a model defined in Swagger"""  # noqa: E501
+        self._ticker = None
+        self._name = None
+        self._peers = None
         self.discriminator = None
-        self.id = id
-        self.tickers = tickers
+        if ticker is not None:
+            self.ticker = ticker
+        if name is not None:
+            self.name = name
+        if peers is not None:
+            self.peers = peers
 
     @property
-    def id(self):
-        """Gets the id of this AddToWatchlistDto.  # noqa: E501
+    def ticker(self):
+        """Gets the ticker of this ActiveCompanyDto.  # noqa: E501
 
 
-        :return: The id of this AddToWatchlistDto.  # noqa: E501
+        :return: The ticker of this ActiveCompanyDto.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._ticker
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this AddToWatchlistDto.
+    @ticker.setter
+    def ticker(self, ticker):
+        """Sets the ticker of this ActiveCompanyDto.
 
 
-        :param id: The id of this AddToWatchlistDto.  # noqa: E501
+        :param ticker: The ticker of this ActiveCompanyDto.  # noqa: E501
         :type: str
         """
-        if id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._id = id
+        self._ticker = ticker
 
     @property
-    def tickers(self):
-        """Gets the tickers of this AddToWatchlistDto.  # noqa: E501
+    def name(self):
+        """Gets the name of this ActiveCompanyDto.  # noqa: E501
 
 
-        :return: The tickers of this AddToWatchlistDto.  # noqa: E501
+        :return: The name of this ActiveCompanyDto.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ActiveCompanyDto.
+
+
+        :param name: The name of this ActiveCompanyDto.  # noqa: E501
+        :type: str
+        """
+
+        self._name = name
+
+    @property
+    def peers(self):
+        """Gets the peers of this ActiveCompanyDto.  # noqa: E501
+
+
+        :return: The peers of this ActiveCompanyDto.  # noqa: E501
         :rtype: list[str]
         """
-        return self._tickers
+        return self._peers
 
-    @tickers.setter
-    def tickers(self, tickers):
-        """Sets the tickers of this AddToWatchlistDto.
+    @peers.setter
+    def peers(self, peers):
+        """Sets the peers of this ActiveCompanyDto.
 
 
-        :param tickers: The tickers of this AddToWatchlistDto.  # noqa: E501
+        :param peers: The peers of this ActiveCompanyDto.  # noqa: E501
         :type: list[str]
         """
-        if tickers is None:
-            raise ValueError("Invalid value for `tickers`, must not be `None`")  # noqa: E501
 
-        self._tickers = tickers
+        self._peers = peers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(AddToWatchlistDto, dict):
+        if issubclass(ActiveCompanyDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AddToWatchlistDto):
+        if not isinstance(other, ActiveCompanyDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/authentication_request.py` & `investor8-sdk-1.1.96/investor8_sdk/models/authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/authentication_source.py` & `investor8-sdk-1.1.96/investor8_sdk/models/authentication_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/authorize_account_request_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/authorize_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/authorize_account_response_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/authorize_account_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/change_password_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/company_info_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_auth_req_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_auth_req_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_plot_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_screen_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_screen_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_update_news.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_user_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_user_res_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_user_res_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/create_watchlist_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/current_metadat_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/current_metadat_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/current_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/current_momentum_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/daily_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/detailed_latest_price_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/discovery_source.py` & `investor8-sdk-1.1.96/investor8_sdk/models/discovery_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/earning_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/email_type.py` & `investor8-sdk-1.1.96/investor8_sdk/models/email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/financial_metric_metadata_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/financial_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/financial_report_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/financial_tag.py` & `investor8-sdk-1.1.96/investor8_sdk/models/financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/financials_growth.py` & `investor8-sdk-1.1.96/investor8_sdk/models/financials_growth.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_list_metric_views_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_list_metric_views_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_list_metrics_description_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_list_metrics_description_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_list_metrics_metadata_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_list_metrics_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_list_metrics_screening_conditions_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_list_metrics_screening_conditions_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_metric_view_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_metric_view_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_metrics_metadata_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_metrics_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_screens_by_user_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_screens_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_daily_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_financial_metrics.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_indicator_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_indicator_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_metadata_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_metadata_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_metric_value_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_metric_value_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_return.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_returns_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/historical_value_metrics.py` & `investor8-sdk-1.1.96/investor8_sdk/models/historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/history_length.py` & `investor8-sdk-1.1.96/investor8_sdk/models/history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/i8_terminal_check_version_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/i8_terminal_check_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/i8_terminal_version.py` & `investor8-sdk-1.1.96/investor8_sdk/models/i8_terminal_version.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/i8_terminal_version_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/i8_terminal_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/latest_financial_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/latest_financial_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/latest_financials_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/latest_price_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/list_exchange_sector_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/log_terminal_usage.py` & `investor8-sdk-1.1.96/investor8_sdk/models/log_terminal_usage.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/login_user_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/login_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/login_with_code_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/login_with_code_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/market_highlight.py` & `investor8-sdk-1.1.96/investor8_sdk/models/market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/market_highlight_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/market_highlight_status.py` & `investor8-sdk-1.1.96/investor8_sdk/models/market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metadata_properties_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metadata_properties_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metric_group_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metric_group_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metric_metadata_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metric_name_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metric_name_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metrics.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metrics_by_period_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metrics_by_period_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metrics_metadata.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metrics_metadata.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/metrics_metadata_response_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/metrics_metadata_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/momentum_metric_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/monthly_metrics.py` & `investor8-sdk-1.1.96/investor8_sdk/models/monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/monthly_returns.py` & `investor8-sdk-1.1.96/investor8_sdk/models/monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/news_categories_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/news_source.py` & `investor8-sdk-1.1.96/investor8_sdk/models/news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/period_metric_value.py` & `investor8-sdk-1.1.96/investor8_sdk/models/period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/period_return.py` & `investor8-sdk-1.1.96/investor8_sdk/models/period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/plot_detail_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/plot_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/plot_response_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/previous_close_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/profile_name.py` & `investor8-sdk-1.1.96/investor8_sdk/models/profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/recent_earning_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/recent_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/remove_from_watchlist_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/remove_from_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/rename_watchlist_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/rename_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/req_type.py` & `investor8-sdk-1.1.96/investor8_sdk/models/req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/reset_password_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/result_field.py` & `investor8-sdk-1.1.96/investor8_sdk/models/result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/return_metrics.py` & `investor8-sdk-1.1.96/investor8_sdk/models/return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/sa_attributes_prices.py` & `investor8-sdk-1.1.96/investor8_sdk/models/sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/sa_sector_price_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/screen.py` & `investor8-sdk-1.1.96/investor8_sdk/models/screen.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/screen_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/screen_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/screening_category_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/screening_category_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/screening_condition.py` & `investor8-sdk-1.1.96/investor8_sdk/models/screening_condition.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/screening_condition_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/screening_condition_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/sector_returns_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/send_email_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/standardized_financial.py` & `investor8-sdk-1.1.96/investor8_sdk/models/standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_earning_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_financial.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_financial_metrics.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_info_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_info_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,38 +31,41 @@
         'security_id': 'str',
         'ticker': 'str',
         'exchange': 'str',
         'name': 'str',
         'sector': 'str',
         'is_spx': 'bool',
         'is_active': 'bool',
-        'ticker_slug': 'str'
+        'ticker_slug': 'str',
+        'peers': 'list[str]'
     }
 
     attribute_map = {
         'security_id': 'SecurityId',
         'ticker': 'Ticker',
         'exchange': 'Exchange',
         'name': 'Name',
         'sector': 'Sector',
         'is_spx': 'IsSpx',
         'is_active': 'IsActive',
-        'ticker_slug': 'TickerSlug'
+        'ticker_slug': 'TickerSlug',
+        'peers': 'Peers'
     }
 
-    def __init__(self, security_id=None, ticker=None, exchange=None, name=None, sector=None, is_spx=None, is_active=None, ticker_slug=None):  # noqa: E501
+    def __init__(self, security_id=None, ticker=None, exchange=None, name=None, sector=None, is_spx=None, is_active=None, ticker_slug=None, peers=None):  # noqa: E501
         """StockInfoDto - a model defined in Swagger"""  # noqa: E501
         self._security_id = None
         self._ticker = None
         self._exchange = None
         self._name = None
         self._sector = None
         self._is_spx = None
         self._is_active = None
         self._ticker_slug = None
+        self._peers = None
         self.discriminator = None
         if security_id is not None:
             self.security_id = security_id
         if ticker is not None:
             self.ticker = ticker
         if exchange is not None:
             self.exchange = exchange
@@ -72,14 +75,16 @@
             self.sector = sector
         if is_spx is not None:
             self.is_spx = is_spx
         if is_active is not None:
             self.is_active = is_active
         if ticker_slug is not None:
             self.ticker_slug = ticker_slug
+        if peers is not None:
+            self.peers = peers
 
     @property
     def security_id(self):
         """Gets the security_id of this StockInfoDto.  # noqa: E501
 
 
         :return: The security_id of this StockInfoDto.  # noqa: E501
@@ -241,14 +246,35 @@
 
         :param ticker_slug: The ticker_slug of this StockInfoDto.  # noqa: E501
         :type: str
         """
 
         self._ticker_slug = ticker_slug
 
+    @property
+    def peers(self):
+        """Gets the peers of this StockInfoDto.  # noqa: E501
+
+
+        :return: The peers of this StockInfoDto.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._peers
+
+    @peers.setter
+    def peers(self, peers):
+        """Sets the peers of this StockInfoDto.
+
+
+        :param peers: The peers of this StockInfoDto.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._peers = peers
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_info_master_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_ipo.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_ipo.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_news.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_news_details.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_news_details.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_news_status.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_news_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_popularity_details_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_popularity_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_popularity_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_price.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_price.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_price_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_rating_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/stock_summary_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/stock_summary_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/string_message_result.py` & `investor8-sdk-1.1.96/investor8_sdk/models/string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/symbols_current_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/symbols_current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/symbols_historical_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/symbols_historical_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/tag_details_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/tag_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/tag_info_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/tag_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/terminal_log_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/terminal_log_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/terminal_log_os_versions_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/terminal_log_os_versions_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/trading_calendar_details_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/trading_calendar_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/upcoming_earning_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/upcoming_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/update_plot_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/user.py` & `investor8-sdk-1.1.96/investor8_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/user_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/value_metrics_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/value_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/view_plot_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/watchlist.py` & `investor8-sdk-1.1.96/investor8_sdk/models/watchlist.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/models/watchlist_dto.py` & `investor8-sdk-1.1.96/investor8_sdk/models/watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk/rest.py` & `investor8-sdk-1.1.96/investor8_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/investor8_sdk.egg-info/PKG-INFO` & `investor8-sdk-1.1.96/investor8_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investor8-sdk
-Version: 1.1.95
+Version: 1.1.96
 Summary: Investoreight Core API
 Home-page: UNKNOWN
 Author-email: info@investoreight.com
 License: UNKNOWN
 Project-URL: Homepage, https://www.investoreight.com/
 Project-URL: Documentation, https://github.com/investoreight/investor8-sdk#readme
 Project-URL: Download, https://github.com/investoreight/investor8-sdk/releases
@@ -16,15 +16,15 @@
 
 # investor8-sdk
 Investoreight API Documentation:  https://api.investoreight.com/api-docs/index.html
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.1
-- Package version: 1.1.95
+- Package version: 1.1.96
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://www.investoreight.com](https://www.investoreight.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `investor8-sdk-1.1.95/investor8_sdk.egg-info/SOURCES.txt` & `investor8-sdk-1.1.96/investor8_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/setup.py` & `investor8-sdk-1.1.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: info@investoreight.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "investor8-sdk"
-VERSION = "1.1.95"
+VERSION = "1.1.96"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `investor8-sdk-1.1.95/test/test_active_company_dto.py` & `investor8-sdk-1.1.96/test/test_active_company_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_add_to_watchlist_dto.py` & `investor8-sdk-1.1.96/test/test_add_to_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_authentication_request.py` & `investor8-sdk-1.1.96/test/test_authentication_request.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_authentication_source.py` & `investor8-sdk-1.1.96/test/test_authentication_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_authorize_account_request_dto.py` & `investor8-sdk-1.1.96/test/test_authorize_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_authorize_account_response_dto.py` & `investor8-sdk-1.1.96/test/test_authorize_account_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_change_password_dto.py` & `investor8-sdk-1.1.96/test/test_change_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_company_info_dto.py` & `investor8-sdk-1.1.96/test/test_company_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_auth_req_dto.py` & `investor8-sdk-1.1.96/test/test_create_auth_req_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_plot_dto.py` & `investor8-sdk-1.1.96/test/test_create_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_screen_dto.py` & `investor8-sdk-1.1.96/test/test_create_screen_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_update_news.py` & `investor8-sdk-1.1.96/test/test_create_update_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_user_dto.py` & `investor8-sdk-1.1.96/test/test_create_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_user_res_dto.py` & `investor8-sdk-1.1.96/test/test_create_user_res_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_create_watchlist_dto.py` & `investor8-sdk-1.1.96/test/test_create_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_current_metadat_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_current_metadat_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_current_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_current_momentum_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_current_momentum_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_daily_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_detailed_latest_price_dto.py` & `investor8-sdk-1.1.96/test/test_detailed_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_discovery_source.py` & `investor8-sdk-1.1.96/test/test_discovery_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_earning_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_earning_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_earnings_api.py` & `investor8-sdk-1.1.96/test/test_earnings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_email_api.py` & `investor8-sdk-1.1.96/test/test_email_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_email_type.py` & `investor8-sdk-1.1.96/test/test_email_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_financial_metric_metadata_dto.py` & `investor8-sdk-1.1.96/test/test_financial_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_financial_report_dto.py` & `investor8-sdk-1.1.96/test/test_financial_report_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_financial_tag.py` & `investor8-sdk-1.1.96/test/test_financial_tag.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_financials_api.py` & `investor8-sdk-1.1.96/test/test_financials_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_financials_growth.py` & `investor8-sdk-1.1.96/test/test_financials_growth.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_list_metric_views_dto.py` & `investor8-sdk-1.1.96/test/test_get_list_metric_views_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_list_metrics_description_dto.py` & `investor8-sdk-1.1.96/test/test_get_list_metrics_description_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_list_metrics_metadata_dto.py` & `investor8-sdk-1.1.96/test/test_get_list_metrics_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_list_metrics_screening_conditions_dto.py` & `investor8-sdk-1.1.96/test/test_get_list_metrics_screening_conditions_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_metric_view_dto.py` & `investor8-sdk-1.1.96/test/test_get_metric_view_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_metrics_metadata_dto.py` & `investor8-sdk-1.1.96/test/test_get_metrics_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_screens_by_user_dto.py` & `investor8-sdk-1.1.96/test/test_get_screens_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_user_plots_dto.py` & `investor8-sdk-1.1.96/test/test_get_user_plots_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_get_watchlists_by_user_dto.py` & `investor8-sdk-1.1.96/test/test_get_watchlists_by_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_daily_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_historical_daily_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_financial_metrics.py` & `investor8-sdk-1.1.96/test/test_historical_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_indicator_dto.py` & `investor8-sdk-1.1.96/test/test_historical_indicator_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_metadata_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_historical_metadata_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_metric_value_dto.py` & `investor8-sdk-1.1.96/test/test_historical_metric_value_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_return.py` & `investor8-sdk-1.1.96/test/test_historical_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_returns_dto.py` & `investor8-sdk-1.1.96/test/test_historical_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_historical_value_metrics.py` & `investor8-sdk-1.1.96/test/test_historical_value_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_history_length.py` & `investor8-sdk-1.1.96/test/test_history_length.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_i8_terminal_check_version_dto.py` & `investor8-sdk-1.1.96/test/test_i8_terminal_check_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_i8_terminal_version.py` & `investor8-sdk-1.1.96/test/test_i8_terminal_version.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_i8_terminal_version_dto.py` & `investor8-sdk-1.1.96/test/test_i8_terminal_version_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_latest_financial_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_latest_financial_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_latest_financials_dto.py` & `investor8-sdk-1.1.96/test/test_latest_financials_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_latest_financials_with_growth_dto.py` & `investor8-sdk-1.1.96/test/test_latest_financials_with_growth_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_latest_price_dto.py` & `investor8-sdk-1.1.96/test/test_latest_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_list_exchange_sector_dto.py` & `investor8-sdk-1.1.96/test/test_list_exchange_sector_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_log_terminal_usage.py` & `investor8-sdk-1.1.96/test/test_log_terminal_usage.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_login_user_dto.py` & `investor8-sdk-1.1.96/test/test_login_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_login_with_code_dto.py` & `investor8-sdk-1.1.96/test/test_login_with_code_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_market_highlight.py` & `investor8-sdk-1.1.96/test/test_market_highlight.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_market_highlight_dto.py` & `investor8-sdk-1.1.96/test/test_market_highlight_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_market_highlight_status.py` & `investor8-sdk-1.1.96/test/test_market_highlight_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metadata_properties_dto.py` & `investor8-sdk-1.1.96/test/test_metadata_properties_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metric_group_dto.py` & `investor8-sdk-1.1.96/test/test_metric_group_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metric_metadata_dto.py` & `investor8-sdk-1.1.96/test/test_metric_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metric_name_dto.py` & `investor8-sdk-1.1.96/test/test_metric_name_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metrics.py` & `investor8-sdk-1.1.96/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metrics_api.py` & `investor8-sdk-1.1.96/test/test_metrics_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metrics_by_period_dto.py` & `investor8-sdk-1.1.96/test/test_metrics_by_period_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metrics_metadata.py` & `investor8-sdk-1.1.96/test/test_metrics_metadata.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_metrics_metadata_response_dto.py` & `investor8-sdk-1.1.96/test/test_metrics_metadata_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_momentum_metric_dto.py` & `investor8-sdk-1.1.96/test/test_momentum_metric_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_monthly_metrics.py` & `investor8-sdk-1.1.96/test/test_monthly_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_monthly_returns.py` & `investor8-sdk-1.1.96/test/test_monthly_returns.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_news_api.py` & `investor8-sdk-1.1.96/test/test_news_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_news_categories_dto.py` & `investor8-sdk-1.1.96/test/test_news_categories_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_news_source.py` & `investor8-sdk-1.1.96/test/test_news_source.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_period_metric_value.py` & `investor8-sdk-1.1.96/test/test_period_metric_value.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_period_return.py` & `investor8-sdk-1.1.96/test/test_period_return.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_plot.py` & `investor8-sdk-1.1.96/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_plot_detail_dto.py` & `investor8-sdk-1.1.96/test/test_plot_detail_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_plot_dto.py` & `investor8-sdk-1.1.96/test/test_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_plot_response_dto.py` & `investor8-sdk-1.1.96/test/test_plot_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_previous_close_dto.py` & `investor8-sdk-1.1.96/test/test_previous_close_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_price_api.py` & `investor8-sdk-1.1.96/test/test_price_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_profile_name.py` & `investor8-sdk-1.1.96/test/test_profile_name.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_recent_earning_dto.py` & `investor8-sdk-1.1.96/test/test_recent_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_remove_from_watchlist_dto.py` & `investor8-sdk-1.1.96/test/test_remove_from_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_rename_watchlist_dto.py` & `investor8-sdk-1.1.96/test/test_rename_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_req_type.py` & `investor8-sdk-1.1.96/test/test_req_type.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_reset_password_dto.py` & `investor8-sdk-1.1.96/test/test_reset_password_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_result_field.py` & `investor8-sdk-1.1.96/test/test_result_field.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_return_metrics.py` & `investor8-sdk-1.1.96/test/test_return_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_sa_attributes_prices.py` & `investor8-sdk-1.1.96/test/test_sa_attributes_prices.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_sa_sector_price_dto.py` & `investor8-sdk-1.1.96/test/test_sa_sector_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_screen.py` & `investor8-sdk-1.1.96/test/test_screen.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_screen_dto.py` & `investor8-sdk-1.1.96/test/test_screen_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_screener_api.py` & `investor8-sdk-1.1.96/test/test_screener_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_screening_category_dto.py` & `investor8-sdk-1.1.96/test/test_screening_category_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_screening_condition.py` & `investor8-sdk-1.1.96/test/test_screening_condition.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_screening_condition_dto.py` & `investor8-sdk-1.1.96/test/test_screening_condition_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_search_api.py` & `investor8-sdk-1.1.96/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_sector_returns_dto.py` & `investor8-sdk-1.1.96/test/test_sector_returns_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_send_email_dto.py` & `investor8-sdk-1.1.96/test/test_send_email_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_settings_api.py` & `investor8-sdk-1.1.96/test/test_settings_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_standardized_financial.py` & `investor8-sdk-1.1.96/test/test_standardized_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_earning_dto.py` & `investor8-sdk-1.1.96/test/test_stock_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_financial.py` & `investor8-sdk-1.1.96/test/test_stock_financial.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_financial_metrics.py` & `investor8-sdk-1.1.96/test/test_stock_financial_metrics.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_info_api.py` & `investor8-sdk-1.1.96/test/test_stock_info_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_info_dto.py` & `investor8-sdk-1.1.96/test/test_stock_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_info_master_dto.py` & `investor8-sdk-1.1.96/test/test_stock_info_master_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_ipo.py` & `investor8-sdk-1.1.96/test/test_stock_ipo.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_news.py` & `investor8-sdk-1.1.96/test/test_stock_news.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_news_details.py` & `investor8-sdk-1.1.96/test/test_stock_news_details.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_news_status.py` & `investor8-sdk-1.1.96/test/test_stock_news_status.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_popularity_details_dto.py` & `investor8-sdk-1.1.96/test/test_stock_popularity_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_popularity_dto.py` & `investor8-sdk-1.1.96/test/test_stock_popularity_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_price.py` & `investor8-sdk-1.1.96/test/test_stock_price.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_price_dto.py` & `investor8-sdk-1.1.96/test/test_stock_price_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_rating_dto.py` & `investor8-sdk-1.1.96/test/test_stock_rating_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_stock_summary_dto.py` & `investor8-sdk-1.1.96/test/test_stock_summary_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_string_message_result.py` & `investor8-sdk-1.1.96/test/test_string_message_result.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_symbols_current_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_symbols_current_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_symbols_historical_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_symbols_historical_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_tag_details_dto.py` & `investor8-sdk-1.1.96/test/test_tag_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_tag_info_dto.py` & `investor8-sdk-1.1.96/test/test_tag_info_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_tags_api.py` & `investor8-sdk-1.1.96/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_terminal_log_dto.py` & `investor8-sdk-1.1.96/test/test_terminal_log_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_terminal_log_os_versions_dto.py` & `investor8-sdk-1.1.96/test/test_terminal_log_os_versions_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_trading_calendar_details_dto.py` & `investor8-sdk-1.1.96/test/test_trading_calendar_details_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_upcoming_earning_dto.py` & `investor8-sdk-1.1.96/test/test_upcoming_earning_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_update_plot_dto.py` & `investor8-sdk-1.1.96/test/test_update_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_update_watchlist_dto.py` & `investor8-sdk-1.1.96/test/test_update_watchlist_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_user.py` & `investor8-sdk-1.1.96/test/test_user.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_user_api.py` & `investor8-sdk-1.1.96/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_user_dto.py` & `investor8-sdk-1.1.96/test/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_validate_watchlist_name_request_dto.py` & `investor8-sdk-1.1.96/test/test_validate_watchlist_name_request_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_validate_watchlist_name_response_dto.py` & `investor8-sdk-1.1.96/test/test_validate_watchlist_name_response_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_value_metrics_dto.py` & `investor8-sdk-1.1.96/test/test_value_metrics_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_view_plot_dto.py` & `investor8-sdk-1.1.96/test/test_view_plot_dto.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_watchlist.py` & `investor8-sdk-1.1.96/test/test_watchlist.py`

 * *Files identical despite different names*

### Comparing `investor8-sdk-1.1.95/test/test_watchlist_dto.py` & `investor8-sdk-1.1.96/test/test_watchlist_dto.py`

 * *Files identical despite different names*

