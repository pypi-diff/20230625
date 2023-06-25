# Comparing `tmp/i8-terminal-0.2.90.tar.gz` & `tmp/i8-terminal-0.2.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i8-terminal-0.2.90.tar", last modified: Sun Jun 25 17:44:34 2023, max compression
+gzip compressed data, was "i8-terminal-0.2.91.tar", last modified: Sun Jun 25 17:46:51 2023, max compression
```

## Comparing `i8-terminal-0.2.90.tar` & `i8-terminal-0.2.91.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.851699 i8-terminal-0.2.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-25 17:44:34.851699 i8-terminal-0.2.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.835699 i8-terminal-0.2.90/i8_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.835699 i8-terminal-0.2.90/i8_terminal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/api/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/api/earnings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/app/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/app/plot_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/assets/i8t_chart_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/assets/i8t_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/assets/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/assets/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/commands/company/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/company/company_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/company/company_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/company/compnay_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/commands/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/earnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_recent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_upcoming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.839699 i8-terminal-0.2.90/i8_terminal/commands/financials/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/financials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/financials/financials_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/financials/financials_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/financials/financials_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/financials/financials_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/market/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/market/market_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_describe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_historical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/news/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/news/news_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/notebook/notebook_launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/price/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/price/price_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/price/price_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/price/price_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/screen/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/screen/screen_gainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/screen/screen_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/screen/screen_losers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/screen/screen_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.843699 i8-terminal-0.2.90/i8_terminal/commands/user/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/user/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/user/user_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/user/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.847699 i8-terminal-0.2.90/i8_terminal/commands/watchlist/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.847699 i8-terminal-0.2.90/i8_terminal/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/i8_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.847699 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-25 17:44:34.000000 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-25 17:44:34.000000 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:44:34.000000 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-25 17:44:34.000000 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-25 17:44:34.000000 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 17:44:34.000000 i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.847699 i8-terminal-0.2.90/i8_terminal/service_result/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/service_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/service_result/column_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/service_result/columns_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/service_result/earning_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/service_result/service_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.847699 i8-terminal-0.2.90/i8_terminal/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/services/earnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:44:34.851699 i8-terminal-0.2.90/i8_terminal/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/auto_complete_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/chart_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/fin_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/fin_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/fin_statement_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/i8_auto_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/i8_completer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/indicator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/market_indice_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/metric_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/metric_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/metric_view_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/output_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/period_type_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/price_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/screening_condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/screening_operator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/screening_value_field_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/sort_order_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/ticker_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/user_watchlist_tickers_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/types/user_watchlists_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/utils_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/i8_terminal/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:44:34.851699 i8-terminal-0.2.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-25 17:43:19.000000 i8-terminal-0.2.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/api/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/api/earnings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/app/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/app/plot_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/i8t_chart_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/i8t_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/assets/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.477773 i8-terminal-0.2.91/i8_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/company/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/company_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/company_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/company/compnay_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/earnings/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_recent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_upcoming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/financials/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/financials/financials_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/market/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/market/market_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/news/news_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/notebook/notebook_launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/price/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/price_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/price_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/price/price_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_gainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_losers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/screen/screen_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.481773 i8-terminal-0.2.91/i8_terminal/commands/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/user_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/user/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/commands/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/financials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/i8_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 17:46:51.000000 i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/service_result/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/column_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/columns_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/earning_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/service_result/service_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.485773 i8-terminal-0.2.91/i8_terminal/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/services/earnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/i8_terminal/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/auto_complete_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/chart_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/fin_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/fin_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/fin_statement_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/i8_auto_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/i8_completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/indicator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/market_indice_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/metric_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/metric_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/metric_view_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/output_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/period_type_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/price_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/screening_condition_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/screening_operator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/screening_value_field_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/sort_order_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/ticker_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/user_watchlist_tickers_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/types/user_watchlists_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/utils_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/i8_terminal/version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:46:51.489773 i8-terminal-0.2.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-25 17:45:52.000000 i8-terminal-0.2.91/setup.py
```

### Comparing `i8-terminal-0.2.90/LICENSE` & `i8-terminal-0.2.91/LICENSE`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/PKG-INFO` & `i8-terminal-0.2.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.90
+Version: 0.2.91
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.90/README.md` & `i8-terminal-0.2.91/README.md`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/app/layout.py` & `i8-terminal-0.2.91/i8_terminal/app/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/app/plot_server.py` & `i8-terminal-0.2.91/i8_terminal/app/plot_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,16 +149,15 @@
     APP.title = f"i8 Terminal: {cmd_context['plot_title']}"
     app_url = f"http://localhost:{APP_SETTINGS['app']['port']}/"
     console = Console()
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         is_port_in_use = s.connect_ex(("localhost", APP_SETTINGS["app"]["port"])) == 0
     if is_port_in_use:
         console.print(
-            f"Port number {APP_SETTINGS['app']['port']} is already in use. Please make sure that only one instance of \
-                i8-terminal runs at a time!",
+            f"Port number {APP_SETTINGS['app']['port']} is already in use. Please make sure that only one instance of i8-terminal runs at a time!",  # noqa: E501
             style="yellow",
         )
         return
     with open(os.devnull, "w") as f, contextlib.redirect_stderr(f):
         Timer(2, lambda: webbrowser.open_new(app_url)).start()
         console.print(
             f'[bold green]Your plot is serving on http://127.0.0.1:{APP_SETTINGS["app"]["port"]}/[/bold green]'
```

### Comparing `i8-terminal-0.2.90/i8_terminal/assets/favicon.ico` & `i8-terminal-0.2.91/i8_terminal/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/assets/i8t_chart_logo.png` & `i8-terminal-0.2.91/i8_terminal/assets/i8t_chart_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/assets/i8t_logo.png` & `i8-terminal-0.2.91/i8_terminal/assets/i8t_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/assets/loading.gif` & `i8-terminal-0.2.91/i8_terminal/assets/loading.gif`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/assets/styles.css` & `i8-terminal-0.2.91/i8_terminal/assets/styles.css`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/company/company_compare.py` & `i8-terminal-0.2.91/i8_terminal/commands/company/company_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/company/company_search.py` & `i8-terminal-0.2.91/i8_terminal/commands/company/company_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/company/compnay_details.py` & `i8-terminal-0.2.91/i8_terminal/commands/company/compnay_details.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_list.py` & `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_plot.py` & `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_recent.py` & `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_recent.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/earnings/earnings_upcoming.py` & `i8-terminal-0.2.91/i8_terminal/commands/earnings/earnings_upcoming.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/financials/financials_compare.py` & `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,16 +107,15 @@
     default="income",
     help="Type of financial statement.",
 )
 @click.option(
     "--period_type",
     "-m",
     type=PeriodTypeParamType(),
-    help="Period by which you want to view the report. Possible values are `FY` for yearly, \
-        `Q` for quarterly, and `TTM` for TTM reports.",
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",  # noqa: E501
 )
 @click.option("--plot", is_flag=True, default=False, help="Plot results on the browser.")
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
 def compare(
     ctx: click.Context,
     identifiers: str,
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/financials/financials_coverage.py` & `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_coverage.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/financials/financials_list.py` & `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,15 @@
     default="income",
     help="Type of financial statement.",
 )
 @click.option(
     "--period_type",
     "-m",
     type=PeriodTypeParamType(),
-    help="Period by which you want to view the report. Possible values are `FY` for yearly, \
-        `Q` for quarterly, and `TTM` for TTM reports.",
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",  # noqa: E501
 )
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
 def list(identifier: str, statement: str, period_type: Optional[str], export_path: Optional[str]) -> None:
     """
     Lists financial metrics of a given company.
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/financials/financials_plot.py` & `i8-terminal-0.2.91/i8_terminal/commands/financials/financials_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,15 @@
     help="Comma-separated list of tickers.",
 )
 @click.option(
     "--period_type",
     "-m",
     type=PeriodTypeParamType(),
     default="FY",
-    help="Period by which you want to view the report. Possible values are `FY` for yearly, \
-        `Q` for quarterly, and `TTM` for TTM reports.",
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",  # noqa: E501
 )
 @click.option("--metrics", "-m", type=MetricParamType(), default="basic_eps", help="Comma-separated list of metrics.")
 @click.option("--from_date", "-f", type=DateTime(), help="Histotical financials from date.")
 @click.option("--to_date", "-t", type=DateTime(), help="Histotical financials to date.")
 @click.option(
     "--chart_type",
     "-c",
@@ -181,23 +180,21 @@
     to_date: Optional[datetime],
 ) -> None:
     """
     Compare and plot financial metrics of given companies. TICKERS is a comma-separated list of tickers.
 
     Examples:
 
-    `i8 financials plot --period_type Q --metrics net_ppe --from_date 2020-05-01 --to_date 2022-05-01 \
-        --tickers AMD,INTC,QCOM --chart_type line`
-    """
+    `i8 financials plot --period_type Q --metrics net_ppe --from_date 2020-05-01 --to_date 2022-05-01 --tickers AMD,INTC,QCOM --chart_type line`
+    """  # noqa: E501
     metrics_list = metrics.replace(" ", "").split(",")
     matched_metrics = [find_similar_fin_metric(metric.replace("_", "")) for metric in metrics_list]
     if not matched_metrics:
         click.echo(
-            f"`{metrics}` is not valid metrics name. See the list of valid financial metrics with the \
-                following command:\n`i8 metrics`"
+            f"`{metrics}` is not valid metrics name. See the list of valid financial metrics with the following command:\n`i8 metrics`"  # noqa: E501
         )
         return
     if len(matched_metrics) > 2:
         click.echo("You can enter up to 2 metrics.")
         return
     if chart_type not in [t[0] for t in get_chart_param_types()]:
         click.echo(f"`{chart_type}` is not valid chart type.")
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/market/market_summary.py` & `i8-terminal-0.2.91/i8_terminal/commands/market/market_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_current.py` & `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_current.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,16 @@
         fy = most recent fiscal year,
         ttm = trailing 12 months,
         ytd = year to date,
         p = default period type
 
     Examples:
 
-    `i8 metrics current --metrics total_revenue.q,net_income.fy,close.d,total_revenue \
-        --tickers AMD,INTC,QCOM`
-    """
+    `i8 metrics current --metrics total_revenue.q,net_income.fy,close.d,total_revenue --tickers AMD,INTC,QCOM`
+    """  # noqa: E501
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         df = get_current_metrics_df(tickers, metrics.replace(".p", ""))
     if df is None:
         console.print("No data found for metrics with selected tickers", style="yellow")
         return
     for m in [*set(metric.split(".")[0] for metric in set(metrics.split(","))) - set(df["metric_name"])]:
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_describe.py` & `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_describe.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_historical.py` & `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,15 @@
     help="Plot can be bar or line chart.",
 )
 @click.option("--pivot", "-pv", is_flag=True, default=False, help="Output will be pivot table.")
 @click.option(
     "--period_type",
     "-t",
     type=PeriodTypeParamType(),
-    help="Period by which you want to view the report. Possible values are `D` for daily, \
-        `FY` for yearly, `Q` for quarterly, `TTM` for TTM reports, `YTD` for YTD reports.",
+    help="Period by which you want to view the report. Possible values are `D` for daily, `FY` for yearly, `Q` for quarterly, `TTM` for TTM reports, `YTD` for YTD reports.",  # noqa: E501
 )
 @click.option("--from_date", "-f", type=DateTime(), help="Histotical metrics from date.")
 @click.option("--to_date", "-t", type=DateTime(), help="Histotical metrics to date.")
 @pass_command
 def historical(
     ctx: click.Context,
     tickers: str,
@@ -290,18 +289,16 @@
 ) -> None:
     """
     Lists, compares and plots metrics of given companies. TICKERS is a comma-separated list of tickers.
 
     Examples:
 
     `i8 metrics historical --metrics net_income --tickers AMD,INTC,QCOM --output plot --plot_type bar --period_type Q`
-    `i8 metrics historical --metrics total_revenue,total_assets --tickers AMD,INTC,QCOM --output terminal \
-        --period_type FY --pivot`
-
-    """
+    `i8 metrics historical --metrics total_revenue,total_assets --tickers AMD,INTC,QCOM --output terminal --period_type FY --pivot`
+    """  # noqa: E501
     metrics_list = metrics.replace(" ", "").split(",")
     if output not in ["terminal", "plot"]:
         click.echo(click.style(f"`{output}` is not valid output type.", fg="yellow"))
         return
     if output == "plot" and len(metrics_list) > 2:
         click.echo(click.style("For the `plot` output type you can enter up to only two metrics.", fg="yellow"))
         return
@@ -342,18 +339,15 @@
 
     console = Console()
     with console.status("Fetching data...", spinner="material") as status:
         df = get_historical_metrics_df(tickers_list, metrics_list, period_type, from_date, to_date)
         df = df.sort_values(["PeriodDateTime"], ascending=False).groupby(["Ticker", "Metric", "Period"]).head(1)
         if len(df["default_period_type"].unique()) > 1:
             console.print(
-                (
-                    "The `period type` of the provided metrics are not compatible. Make sure the provided metrics have "
-                    "the same period type. Check `metrics describe` command to find more about metrics."
-                ),
+                "The `period type` of the provided metrics are not compatible. Make sure the provided metrics have the same period type. Check `metrics describe` command to find more about metrics.",  # noqa: E501
                 style="yellow",
             )
             return
         if output == "plot":
             cmd_context["plot_title"] = f"Historical {' and '.join(list(set(df['Metric'])))}"
             status.update("Generating plot...")
             fig = create_fig(df, cmd_context, tickers_list, plot_type, metrics_type_df)
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/metrics/metrics_search.py` & `i8-terminal-0.2.91/i8_terminal/commands/metrics/metrics_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/news/news_list.py` & `i8-terminal-0.2.91/i8_terminal/commands/news/news_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/notebook/notebook_launch.py` & `i8-terminal-0.2.91/i8_terminal/commands/notebook/notebook_launch.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/price/price_compare.py` & `i8-terminal-0.2.91/i8_terminal/commands/price/price_compare.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/price/price_list.py` & `i8-terminal-0.2.91/i8_terminal/commands/price/price_list.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/price/price_plot.py` & `i8-terminal-0.2.91/i8_terminal/commands/price/price_plot.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/screen/screen_gainers.py` & `i8-terminal-0.2.91/i8_terminal/commands/screen/screen_gainers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/screen/screen_losers.py` & `i8-terminal-0.2.91/i8_terminal/commands/screen/screen_losers.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/screen/screen_search.py` & `i8-terminal-0.2.91/i8_terminal/commands/screen/screen_search.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/user/user_login.py` & `i8-terminal-0.2.91/i8_terminal/commands/user/user_login.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/user/webserver.py` & `i8-terminal-0.2.91/i8_terminal/commands/user/webserver.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_add.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_add.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,13 @@
 
     """
     console = Console()
     tickers_list = tickers.replace(" ", "").upper().split(",")
     with console.status("Updating Watchlist...", spinner="material"):
         add_tickers_to_watchlist(name, tickers_list)
     console.print(
-        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}\
-            [/cyan] added to watchlist [cyan]{name}[/cyan] successfully!"
+        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}[/cyan] added to watchlist [cyan]{name}[/cyan] successfully!"  # noqa: E501
     )
     terminal_command_style = Style(**get_terminal_command_layout())
     console.print(
-        f'Try `[{terminal_command_style}]watchlist summary --name "{name}"[/{terminal_command_style}]`\
-             to see the watchlist.'
+        f'Try `[{terminal_command_style}]watchlist summary --name "{name}"[/{terminal_command_style}]`to see the watchlist.'  # noqa: E501
     )
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_create.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_create.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_export.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_export.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_financials.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_list.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 def prepare_watchlists_df(watchlists: List[WatchlistDto]) -> DataFrame:
     wls: List[Dict[str, str]] = []
     for wl in watchlists:
         wls.append(
             {
                 "name": wl.name,
-                "tickers": f"{', '.join(str(ticker) for ticker in wl.tickers[:5])} \
-                    {f'and {len(wl.tickers)-5} more' if len(wl.tickers) > 5 else ''}",
+                "tickers": f"{', '.join(str(ticker) for ticker in wl.tickers[:5])} {f'and {len(wl.tickers)-5} more' if len(wl.tickers) > 5 else ''}",  # noqa: E501
             }
         )
     watchlists_df = DataFrame(wls)
     col_names = {
         "name": "Name",
         "tickers": "Tickers",
     }
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_metrics.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_metrics.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_rm.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_rm.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,15 +49,13 @@
 
     """
     console = Console()
     tickers_list = tickers.replace(" ", "").upper().split(",")
     with console.status("Updating Watchlist...", spinner="material"):
         remove_tickers_from_watchlist(name, tickers_list)
     console.print(
-        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}[/cyan] removed from \
-            watchlist [cyan]{name}[/cyan] successfully!"
+        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}[/cyan] removed from watchlist [cyan]{name}[/cyan] successfully!"  # noqa: E501
     )
     terminal_command_style = Style(**get_terminal_command_layout())
     console.print(
-        f'Try `[{terminal_command_style}]watchlist summary --name "{name}"[/{terminal_command_style}]`\
-             to see the watchlist.'
+        f'Try `[{terminal_command_style}]watchlist summary --name "{name}"[/{terminal_command_style}]`to see the watchlist.'  # noqa: E501
     )
```

### Comparing `i8-terminal-0.2.90/i8_terminal/commands/watchlist/watchlist_summary.py` & `i8-terminal-0.2.91/i8_terminal/commands/watchlist/watchlist_summary.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/cli.py` & `i8-terminal-0.2.91/i8_terminal/common/cli.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/financials.py` & `i8-terminal-0.2.91/i8_terminal/common/financials.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/formatting.py` & `i8-terminal-0.2.91/i8_terminal/common/formatting.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/layout.py` & `i8-terminal-0.2.91/i8_terminal/common/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/metrics.py` & `i8-terminal-0.2.91/i8_terminal/common/metrics.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/price.py` & `i8-terminal-0.2.91/i8_terminal/common/price.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/screen.py` & `i8-terminal-0.2.91/i8_terminal/common/screen.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/stock_info.py` & `i8-terminal-0.2.91/i8_terminal/common/stock_info.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/common/utils.py` & `i8-terminal-0.2.91/i8_terminal/common/utils.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/config.py` & `i8-terminal-0.2.91/i8_terminal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 def init_settings() -> None:
     if not os.path.exists(SETTINGS_FOLDER):
         try:
             os.mkdir(SETTINGS_FOLDER)
         except Exception:
             logging.error(
-                f"Cannot initialize app. Application needs write access to create app directory in the following path: \
-                    '{OS_HOME_PATH}'"
+                f"Cannot initialize app. Application needs write access to create app directory in the following path: '{OS_HOME_PATH}'"  # noqa: E501
             )
 
     if not os.path.exists(USER_SETTINGS_PATH):
         try:
             user_setting = {"app_instance_id": uuid.uuid4().hex}
             with open(USER_SETTINGS_PATH, "w") as f:
                 yaml.dump(user_setting, f)
@@ -48,16 +47,15 @@
             app_settings_src_path = os.path.join(PACKAGE_PATH, "config.yml")
             if os.path.exists(app_settings_src_path):
                 shutil.copyfile(app_settings_src_path, APP_SETTINGS_PATH)
             else:
                 shutil.copyfile(f"{EXECUTABLE_APP_DIR}/config.yml", APP_SETTINGS_PATH)
         except Exception as e:
             logging.error(
-                f"Cannot initalize app settings. Make sure you have write access to the path: \
-                    '{APP_SETTINGS_PATH}'\n {e}"
+                f"Cannot initalize app settings. Make sure you have write access to the path: '{APP_SETTINGS_PATH}'\n {e}"  # noqa: E501
             )
 
 
 def load_user_settings() -> Any:
     if not os.path.exists(USER_SETTINGS_PATH):
         return {}
     with open(USER_SETTINGS_PATH, "r") as f:
@@ -131,16 +129,15 @@
         return {
             "header_style": Style(**styles["header"]),
             "row_styles": [Style(**styles["row"]), Style(**styles["alternate_row"])],
             "show_lines": styles.get("show_lines", False),
         }
     except Exception:
         raise I8Exception(
-            "Cannot parse table style settings from the configuration file! \
-                Check to see if the configuration file is formatted correctly!"
+            "Cannot parse table style settings from the configuration file! Check to see if the configuration file is formatted correctly!"  # noqa: E501
         )
 
 
 def is_user_logged_in() -> bool:
     if not USER_SETTINGS.get("i8_core_api_key") or not USER_SETTINGS.get("i8_core_token"):
         return False
     return True
```

### Comparing `i8-terminal-0.2.90/i8_terminal/config.yml` & `i8-terminal-0.2.91/i8_terminal/config.yml`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/PKG-INFO` & `i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.90
+Version: 0.2.91
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
```

### Comparing `i8-terminal-0.2.90/i8_terminal/i8_terminal.egg-info/SOURCES.txt` & `i8-terminal-0.2.91/i8_terminal/i8_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/main.py` & `i8-terminal-0.2.91/i8_terminal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
         while True:
             try:
                 repl(click.get_current_context(), prompt_kwargs=prompt_kwargs)
             except ApiException as e:
                 if "apiKey" in e.body.decode("utf-8"):
                     console.print(
-                        "You need to login before using i8 Terminal. Please login to i8 Terminal using \
-                            [magenta]user login[/magenta] command."
+                        "You need to login before using i8 Terminal. Please login to i8 Terminal using [magenta]user login[/magenta] command."  # noqa: E501
                     )
                 else:
                     console.print(f"⚠ Error: {e.body.decode('utf-8')}", style="yellow")
                 log_terminal_usage(click.get_current_context(), e.body.decode("utf-8"))
             except Exception as e:
                 display_error = f"- Type: {type(e).__name__}\n- Message: {e}"
                 log_terminal_usage(click.get_current_context(), display_error)
@@ -157,16 +156,15 @@
         init_api_configs()
 
     try:
         cli(obj={})
     except ApiException as e:
         if "apiKey" in e.body.decode("utf-8"):
             console.print(
-                "You need to login before using i8 Terminal. Please login to i8 Terminal \
-                    using [magenta]user login[/magenta] command."
+                "You need to login before using i8 Terminal. Please login to i8 Terminal using [magenta]user login[/magenta] command."  # noqa: E501
             )
         else:
             console.print(f"⚠ Error: {e.body.decode('utf-8')}", style="yellow")
     except Exception as e:
         display_error = f"- Type: {type(e).__name__}\n- Message: {e}"
         console.print(f"⚠ Error:\n{display_error}", style="yellow")
```

### Comparing `i8-terminal-0.2.90/i8_terminal/service_result/column_info.py` & `i8-terminal-0.2.91/i8_terminal/service_result/column_info.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/service_result/columns_context.py` & `i8-terminal-0.2.91/i8_terminal/service_result/columns_context.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/service_result/earning_list_result.py` & `i8-terminal-0.2.91/i8_terminal/service_result/earning_list_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/service_result/service_result.py` & `i8-terminal-0.2.91/i8_terminal/service_result/service_result.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/services/earnings.py` & `i8-terminal-0.2.91/i8_terminal/services/earnings.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/auto_complete_choice.py` & `i8-terminal-0.2.91/i8_terminal/types/auto_complete_choice.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/chart_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/chart_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/command_parser.py` & `i8-terminal-0.2.91/i8_terminal/types/command_parser.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/condition_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/fin_identifier_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/fin_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/fin_period_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/fin_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/fin_statement_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/fin_statement_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/i8_auto_suggest.py` & `i8-terminal-0.2.91/i8_terminal/types/i8_auto_suggest.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/i8_completer.py` & `i8-terminal-0.2.91/i8_terminal/types/i8_completer.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/indicator_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/indicator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/market_indice_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/market_indice_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/metric_identifier_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/metric_identifier_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/metric_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/metric_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/metric_view_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/metric_view_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/output_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/output_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/period_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/period_type_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/period_type_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/price_period_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/price_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/screening_condition_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/screening_condition_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/screening_operator_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/screening_operator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/screening_value_field_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/screening_value_field_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/sort_order_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/sort_order_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/ticker_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/ticker_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/user_watchlist_tickers_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/user_watchlist_tickers_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/types/user_watchlists_param_type.py` & `i8-terminal-0.2.91/i8_terminal/types/user_watchlists_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/i8_terminal/utils_setup.py` & `i8-terminal-0.2.91/i8_terminal/utils_setup.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.90/setup.py` & `i8-terminal-0.2.91/setup.py`

 * *Files identical despite different names*

