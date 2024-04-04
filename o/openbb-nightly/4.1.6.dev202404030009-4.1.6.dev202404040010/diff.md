# Comparing `tmp/openbb_nightly-4.1.6.dev202404030009.tar.gz` & `tmp/openbb_nightly-4.1.6.dev202404040010.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.6.dev202404030009.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.6.dev202404040010.tar", max compression
```

## Comparing `openbb_nightly-4.1.6.dev202404030009.tar` & `openbb_nightly-4.1.6.dev202404040010.tar`

### file list

```diff
@@ -1,763 +1,764 @@
--rw-r--r--   0        0        0     6818 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/README.md
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      418 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1945 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4159 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7196 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    17435 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2525 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5312 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2474 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2691 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8333 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2137 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      859 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2047 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      239 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       52 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      428 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      177 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      321 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0      906 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-04-03 00:09:51.747663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      346 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3864 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      808 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/custom_parameter.py
--rw-r--r--   0        0        0      435 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1912 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/fast_api_settings.py
--rw-r--r--   0        0        0     1940 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/hub/features_keys.py
--rw-r--r--   0        0        0      561 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      472 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     4694 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9593 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1418 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      450 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0       92 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     3855 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    17912 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    23314 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2632 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10218 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3443 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3025 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7759 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     1769 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1542 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1948 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    61347 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3067 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     1639 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5959 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1677 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2316 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0     3494 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8660 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     9401 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0      630 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1288 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     1591 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-04-03 00:09:51.755663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1750 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      888 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      768 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2715 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6153 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1700 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-04-03 00:09:51.759663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3083 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3474 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     4909 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9293 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.763663 openbb_nightly-4.1.6.dev202404030009/core/openbb_core/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1010 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3794 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      332 2024-04-03 00:09:51.767663 openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28108 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4036 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0     9705 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1742 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1109 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5811 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3452 2024-04-03 00:09:51.771663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     2652 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3769 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6010 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1541 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4053 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3170 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.775663 openbb_nightly-4.1.6.dev202404030009/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8610 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10087 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14280 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1313 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10975 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1885 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      370 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4204 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16751 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    57417 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0     7652 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-04-03 00:09:51.779663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    16542 2024-04-03 00:09:51.783663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.783663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-04-03 00:09:51.783663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17390 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     7156 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2422 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58414 2024-04-03 00:09:51.799663 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228603 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7101 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12351 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8398 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    18829 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3240 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5661 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6817 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3510 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    22181 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1379 2024-04-03 00:09:51.819664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   857302 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2252 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0     3666 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0     3204 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0    23603 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0      600 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0     1440 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/openbb/__init__.py
--rw-r--r--   0        0        0      674 2024-04-03 00:09:51.827664 openbb_nightly-4.1.6.dev202404030009/openbb/assets/extension_map.json
--rw-r--r--   0        0        0  1053853 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/assets/reference.json
--rw-r--r--   0        0        0     2794 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/crypto.py
--rw-r--r--   0        0        0     6589 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    11777 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/currency.py
--rw-r--r--   0        0        0     6481 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12160 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    53423 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/economy.py
--rw-r--r--   0        0        0    12674 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27673 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity.py
--rw-r--r--   0        0        0    18754 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2869 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    26106 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    27199 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   169108 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30667 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26819 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3567 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    74985 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/etf.py
--rw-r--r--   0        0        0     4649 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    20027 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7155 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26900 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    11204 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11919 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/index.py
--rw-r--r--   0        0        0    15535 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/regulators.py
--rw-r--r--   0        0        0    16562 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12446 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2516 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    14906 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9745 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.831664 openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3829 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2154 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6469 2024-04-03 00:09:51.839664 openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-03 00:09:51.847664 openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      716 2024-04-03 00:09:51.891664 openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-03 00:09:51.891664 openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-03 00:09:51.891664 openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-04-03 00:09:51.891664 openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-04-03 00:09:51.899664 openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-03 00:09:51.899664 openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-04-03 00:09:51.899664 openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-04-03 00:09:51.899664 openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5360 2024-04-03 00:09:51.899664 openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9574 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8111 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-03 00:09:51.955665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6022 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5202 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6763 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2774 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     3771 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2064 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3903 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     5922 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3131 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     2900 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4243 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.963665 openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6312 2024-04-03 00:09:51.979665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-04-03 00:09:51.983665 openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5221 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     4877 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2377 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7025 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-03 00:09:51.987665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     3716 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     4829 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3328 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8829 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     5359 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2550 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-03 00:09:51.991665 openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3954 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6262 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     5969 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2173 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5090 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-03 00:09:51.999665 openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8668 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2100 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.007665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6130 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6054 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7020 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     5973 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3618 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3690 2024-04-03 00:09:52.015665 openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8277 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2617 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13834 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7410 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.027665 openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-03 00:09:52.119666 openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5170 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4373 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8830 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5446 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12441 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4439 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3055 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10268 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6055 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5688 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38297 2024-04-03 00:09:52.131666 openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6568 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9162 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10222 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-03 00:09:52.231667 openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-04-03 00:09:52.235667 openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4529 2024-04-03 00:09:52.235667 openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4567 2024-04-03 00:09:52.235667 openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3636 2024-04-03 00:09:52.235667 openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4232 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     1935 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5722 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10040 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     3922 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6639 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-03 00:09:52.239667 openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     6884 2024-04-03 00:10:06.571782 openbb_nightly-4.1.6.dev202404030009/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404030009/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      418 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1945 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4159 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7196 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    17435 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2525 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5312 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2474 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2691 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8333 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2137 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      859 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2047 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       52 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      428 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      177 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      321 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0      906 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      346 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3864 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      808 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/custom_parameter.py
+-rw-r--r--   0        0        0      435 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1912 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/fast_api_settings.py
+-rw-r--r--   0        0        0     1940 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/hub/features_keys.py
+-rw-r--r--   0        0        0      561 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      472 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     4694 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9866 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1418 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      450 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     3855 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    17912 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23314 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2632 2024-04-04 00:10:06.037711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10218 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3443 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3025 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7759 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     1769 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1542 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1948 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    61347 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3067 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     1639 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5959 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1677 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2316 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2581 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     9401 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0      630 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1288 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     1591 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      423 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1750 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      888 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      768 2024-04-04 00:10:06.041711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2715 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6153 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1700 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3083 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3474 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     4909 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9293 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.045711 openbb_nightly-4.1.6.dev202404040010/core/openbb_core/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1010 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3794 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      332 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-04-04 00:10:06.053711 openbb_nightly-4.1.6.dev202404040010/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28108 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4036 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0     9705 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1742 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2326 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1109 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5811 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3452 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3769 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-04 00:10:06.057711 openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6010 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1541 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4053 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3170 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8610 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10087 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14280 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1313 2024-04-04 00:10:06.061711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10975 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1885 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      370 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4204 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16751 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    57417 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0     7652 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    16542 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.065711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-04-04 00:10:06.069711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17390 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     7156 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2422 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58414 2024-04-04 00:10:06.085711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228603 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7101 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12351 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8398 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    18829 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3240 2024-04-04 00:10:06.105711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5661 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6817 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3510 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    22181 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1379 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   857302 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2252 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0     3666 2024-04-04 00:10:06.109711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0     3204 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0    23603 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0     1440 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/openbb/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-04 00:10:06.113711 openbb_nightly-4.1.6.dev202404040010/openbb/assets/extension_map.json
+-rw-r--r--   0        0        0  1053853 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2794 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0       50 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6589 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    11777 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/currency.py
+-rw-r--r--   0        0        0     6481 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12160 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    53423 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/economy.py
+-rw-r--r--   0        0        0    12674 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27673 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity.py
+-rw-r--r--   0        0        0    18754 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2869 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    26106 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    27199 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   169108 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30667 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26819 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3567 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    74985 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/etf.py
+-rw-r--r--   0        0        0     4649 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    20027 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7155 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26900 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    11204 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11919 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/index.py
+-rw-r--r--   0        0        0    15535 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/regulators.py
+-rw-r--r--   0        0        0    16562 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/package/regulators_sec.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-04-04 00:10:06.117711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12446 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2516 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    14906 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9745 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3829 2024-04-04 00:10:06.121711 openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2154 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6469 2024-04-04 00:10:06.125711 openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-04-04 00:10:06.129711 openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      716 2024-04-04 00:10:06.177711 openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-04-04 00:10:06.177711 openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-04-04 00:10:06.177711 openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-04-04 00:10:06.181712 openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-04-04 00:10:06.185711 openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-04 00:10:06.185711 openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-04-04 00:10:06.185711 openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-04-04 00:10:06.185711 openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5360 2024-04-04 00:10:06.185711 openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9574 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.241712 openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8111 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6022 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5202 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-04-04 00:10:06.245712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6763 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2774 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     3771 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2064 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3903 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     5922 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3131 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     2900 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4243 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.249712 openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6656 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-04-04 00:10:06.269712 openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-04-04 00:10:06.273712 openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-04 00:10:06.273712 openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-04 00:10:06.273712 openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5221 2024-04-04 00:10:06.273712 openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.273712 openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     4877 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2377 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7025 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     3716 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     4829 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3328 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8829 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     5359 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2550 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-04 00:10:06.277712 openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3954 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6262 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     5969 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2173 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5090 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-04 00:10:06.289712 openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8668 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2100 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     6961 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6130 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6054 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6125 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     7020 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     5973 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3618 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3690 2024-04-04 00:10:06.297712 openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0     8277 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     2617 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2720 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    32406 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2754 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2079 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2790 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3009 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1714 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    13834 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7410 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.313712 openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-04 00:10:06.405712 openbb_nightly-4.1.6.dev202404040010/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-04 00:10:06.409713 openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-04-04 00:10:06.417713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.417713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-04 00:10:06.417713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-04-04 00:10:06.417713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5170 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4373 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8830 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5446 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12441 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4439 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3055 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10268 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6055 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5688 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38297 2024-04-04 00:10:06.421713 openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6568 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9162 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10222 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-04 00:10:06.517713 openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-04-04 00:10:06.521713 openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     4529 2024-04-04 00:10:06.521713 openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4567 2024-04-04 00:10:06.521713 openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3636 2024-04-04 00:10:06.521713 openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4232 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     1935 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5722 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10040 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     3922 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6639 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-04 00:10:06.525713 openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     6884 2024-04-04 00:10:17.537772 openbb_nightly-4.1.6.dev202404040010/pyproject.toml
+-rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.6.dev202404040010/PKG-INFO
```

### Comparing `openbb_nightly-4.1.6.dev202404030009/README.md` & `openbb_nightly-4.1.6.dev202404040010/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/command_runner.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/custom_parameter.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/custom_parameter.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/fast_api_settings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/fast_api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/hub/features_keys.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/hub/features_keys.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/obbject.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from pydantic import BaseModel, Field, PrivateAttr
 
 from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.app.model.abstract.tagged import Tagged
 from openbb_core.app.model.abstract.warning import Warning_
 from openbb_core.app.model.charts.chart import Chart
 from openbb_core.app.utils import basemodel_to_df
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.data import Data
 
 if TYPE_CHECKING:
     from openbb_core.app.query import Query
 
     try:
         from polars import DataFrame as PolarsDataFrame  # type: ignore
@@ -295,8 +296,13 @@
             Initialized query object.
 
         Returns
         -------
         OBBject[ResultsType]
             OBBject with results.
         """
-        return cls(results=await query.execute())
+        results = await query.execute()
+        if isinstance(results, AnnotatedResult):
+            return cls(
+                results=results.result, extra={"results_metadata": results.metadata}
+            )
+        return cls(results=results)
```

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/query.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/router.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/package_builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/app/version.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/env.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/fetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 from typing import (
     Any,
     Dict,
     Generic,
     Optional,
     TypeVar,
+    Union,
     get_args,
     get_origin,
 )
 
 from pandas import DataFrame
 
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.helpers import maybe_coroutine, run_async
 
 Q = TypeVar("Q", bound=QueryParams)
 D = TypeVar("D", bound=Data)
 R = TypeVar("R")  # Return, usually List[D], but can be just D for example
@@ -52,15 +54,15 @@
         """Asynchronously extract the data from the provider."""
 
     @staticmethod
     def extract_data(query: Q, credentials: Optional[Dict[str, str]]) -> Any:
         """Extract the data from the provider."""
 
     @staticmethod
-    def transform_data(query: Q, data: Any, **kwargs) -> R:
+    def transform_data(query: Q, data: Any, **kwargs) -> Union[R, AnnotatedResult[R]]:
         """Transform the provider-specific data."""
         raise NotImplementedError
 
     def __init_subclass__(cls, *args, **kwargs):
         """Initialize the subclass."""
         super().__init_subclass__(*args, **kwargs)
 
@@ -75,15 +77,15 @@
 
     @classmethod
     async def fetch_data(
         cls,
         params: Dict[str, Any],
         credentials: Optional[Dict[str, str]] = None,
         **kwargs,
-    ) -> R:
+    ) -> Union[R, AnnotatedResult[R]]:
         """Fetch data from a provider."""
         query = cls.transform_query(params=params)
         data = await maybe_coroutine(
             cls.extract_data, query=query, credentials=credentials, **kwargs
         )
         return cls.transform_data(query=query, data=data, **kwargs)
 
@@ -135,15 +137,15 @@
         AssertionError
             If any of the tests fail.
         """
         query = cls.transform_query(params=params)
         data = run_async(
             cls.extract_data, query=query, credentials=credentials, **kwargs
         )
-        transformed_data = cls.transform_data(query=query, data=data, **kwargs)
+        result = cls.transform_data(query=query, data=data, **kwargs)
 
         # Class Assertions
         assert isinstance(
             cls.require_credentials, bool
         ), "require_credentials must be a boolean."
 
         # Query Assertions
@@ -180,18 +182,21 @@
             assert (
                 issubclass(type(data), cls.data_type) is False
             ), f"Data must not be transformed yet. Expected: {cls.data_type} Got: {type(data)}"
 
         assert len(data) > 0, "Data must not be empty."
 
         # Transformed Data Assertions
+        transformed_data = (
+            result.result if isinstance(result, AnnotatedResult) else result
+        )
+
         assert transformed_data, "Transformed data must not be None."
 
-        is_list = isinstance(transformed_data, list)
-        if is_list:
+        if isinstance(transformed_data, list):
             return_type_args = cls.return_type.__args__[0]
             return_type_is_dict = (
                 hasattr(return_type_args, "__origin__")
                 and return_type_args.__origin__ is dict
             )
             if return_type_is_dict:
                 return_type_fields = return_type_args.__args__[1].__args__[0].__fields__
```

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/core/openbb_core/provider/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/economy/openbb_economy/economy_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/technical/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.6.dev202404040010/extensions/technical/openbb_technical/technical_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/assets/extension_map.json` & `openbb_nightly-4.1.6.dev202404040010/openbb/assets/extension_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/assets/reference.json` & `openbb_nightly-4.1.6.dev202404040010/openbb/assets/reference.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/__extensions__.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/crypto.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/crypto_price.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/currency.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/currency.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/currency_price.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/currency_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/derivatives.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/economy.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/economy.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_compare.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_fundamental.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_price.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/etf.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/etf.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_corporate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/index.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/index.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/news.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/openbb/package/regulators_sec.py` & `openbb_nightly-4.1.6.dev202404040010/openbb/package/regulators_sec.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.6.dev202404040010/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404040010/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/series.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """FRED Series Model."""
 
-import json
-import warnings
 from typing import Any, Dict, List, Literal, Optional
 
 import pandas as pd
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.fred_series import (
     SeriesData,
     SeriesQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
     get_querystring,
 )
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FredSeriesQueryParams(SeriesQueryParams):
     """FRED Series Query Params."""
 
     __alias_dict__ = {
         "symbol": "series_id",
         "start_date": "observation_start",
@@ -141,17 +138,26 @@
             observations_response = await response.json()
             series_id = response.url.query.get("series_id")
 
             metadata_response = await session.get_json(
                 f"{metadata_url}?series_id={series_id}&file_type=json&api_key={api_key}",
                 timeout=5,
             )
-            _metadata = metadata_response.get("seriess", [{}])[0]
 
-            observations = observations_response.get("observations")
+            # seriess is not a typo, it's the actual key in the response
+            _metadata = (
+                metadata_response.get("seriess", [{}])[0]
+                if isinstance(metadata_response, dict)
+                else {}
+            ) or {}
+            observations = (
+                observations_response.get("observations")
+                if isinstance(observations_response, dict)
+                else []
+            ) or []
             try:
                 for d in observations:
                     d.pop("realtime_start")
                     d.pop("realtime_end")
 
                 data = (
                     pd.DataFrame(observations)
@@ -173,33 +179,28 @@
                     "notes": _metadata.get("notes"),
                     "data": data,
                 }
             }
 
         results = await amake_requests(urls, callback, timeout=5, **kwargs)
 
-        metadata, data = {}, {}
-        for item in results:
-            for series_id, result in item.items():
-                data[series_id] = result.pop("data")
-                metadata[series_id] = result
-
-        _warn(json.dumps(metadata))
-
-        return data
+        return results
 
     # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
-        query: FredSeriesQueryParams, data: Dict, **kwargs: Any
-    ) -> List[FredSeriesData]:
+        query: FredSeriesQueryParams, data: List[Dict[str, Any]], **kwargs: Any
+    ) -> AnnotatedResult[List[FredSeriesData]]:
         """Transform data."""
-        results = (
-            pd.DataFrame(data)
+        series = {_id: s.pop("data", {}) for d in data for _id, s in d.items()}
+        metadata = {_id: m for d in data for _id, m in d.items()}
+        records = (
+            pd.DataFrame(series)
             .filter(items=query.symbol.split(","), axis=1)
             .reset_index()
             .rename(columns={"index": "date"})
             .fillna("N/A")
             .replace("N/A", None)
             .to_dict("records")
         )
-        return [FredSeriesData.model_validate(d) for d in results]
+        validated = [FredSeriesData.model_validate(r) for r in records]
+        return AnnotatedResult(result=validated, metadata=metadata)
```

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.6.dev202404040010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.6.dev202404040010/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.6.dev202404040010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.6.dev202404040010/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.6.dev202404040010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.6.dev202404040010/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.6.dev202404040010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.6.dev202404040010/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.6.dev202404030009/pyproject.toml` & `openbb_nightly-4.1.6.dev202404040010/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,179 +1,179 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.6.dev202404030009"
+version = "4.1.6.dev202404040010"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
 include = "openbb_core"
 from = "./core"
 
 [[tool.poetry.packages]]
-include = "openbb_tradingeconomics"
-from = "./providers/tradingeconomics"
-
-[[tool.poetry.packages]]
-include = "openbb_biztoc"
-from = "./providers/biztoc"
+include = "openbb_oecd"
+from = "./providers/oecd"
 
 [[tool.poetry.packages]]
-include = "openbb_federal_reserve"
-from = "./providers/federal_reserve"
+include = "openbb_benzinga"
+from = "./providers/benzinga"
 
 [[tool.poetry.packages]]
-include = "openbb_oecd"
-from = "./providers/oecd"
+include = "openbb_finra"
+from = "./providers/finra"
 
 [[tool.poetry.packages]]
-include = "openbb_fred"
-from = "./providers/fred"
+include = "openbb_stockgrid"
+from = "./providers/stockgrid"
 
 [[tool.poetry.packages]]
-include = "openbb_tmx"
-from = "./providers/tmx"
+include = "openbb_biztoc"
+from = "./providers/biztoc"
 
 [[tool.poetry.packages]]
-include = "openbb_seeking_alpha"
-from = "./providers/seeking_alpha"
+include = "openbb_wsj"
+from = "./providers/wsj"
 
 [[tool.poetry.packages]]
-include = "openbb_ecb"
-from = "./providers/ecb"
+include = "openbb_nasdaq"
+from = "./providers/nasdaq"
 
 [[tool.poetry.packages]]
-include = "openbb_intrinio"
-from = "./providers/intrinio"
+include = "openbb_finviz"
+from = "./providers/finviz"
 
 [[tool.poetry.packages]]
 include = "openbb_polygon"
 from = "./providers/polygon"
 
 [[tool.poetry.packages]]
-include = "openbb_nasdaq"
-from = "./providers/nasdaq"
+include = "openbb_intrinio"
+from = "./providers/intrinio"
 
 [[tool.poetry.packages]]
 include = "openbb_cboe"
 from = "./providers/cboe"
 
 [[tool.poetry.packages]]
-include = "openbb_yfinance"
-from = "./providers/yfinance"
+include = "openbb_fmp"
+from = "./providers/fmp"
 
 [[tool.poetry.packages]]
-include = "openbb_finviz"
-from = "./providers/finviz"
+include = "openbb_seeking_alpha"
+from = "./providers/seeking_alpha"
 
 [[tool.poetry.packages]]
-include = "openbb_finra"
-from = "./providers/finra"
+include = "openbb_tiingo"
+from = "./providers/tiingo"
 
 [[tool.poetry.packages]]
-include = "openbb_stockgrid"
-from = "./providers/stockgrid"
+include = "openbb_alpha_vantage"
+from = "./providers/alpha_vantage"
 
 [[tool.poetry.packages]]
-include = "openbb_tiingo"
-from = "./providers/tiingo"
+include = "openbb_tradier"
+from = "./providers/tradier"
 
 [[tool.poetry.packages]]
-include = "openbb_benzinga"
-from = "./providers/benzinga"
+include = "openbb_sec"
+from = "./providers/sec"
 
 [[tool.poetry.packages]]
-include = "openbb_wsj"
-from = "./providers/wsj"
+include = "openbb_tradingeconomics"
+from = "./providers/tradingeconomics"
 
 [[tool.poetry.packages]]
-include = "openbb_tradier"
-from = "./providers/tradier"
+include = "openbb_yfinance"
+from = "./providers/yfinance"
+
+[[tool.poetry.packages]]
+include = "openbb_ecb"
+from = "./providers/ecb"
 
 [[tool.poetry.packages]]
 include = "openbb_government_us"
 from = "./providers/government_us"
 
 [[tool.poetry.packages]]
-include = "openbb_sec"
-from = "./providers/sec"
+include = "openbb_federal_reserve"
+from = "./providers/federal_reserve"
 
 [[tool.poetry.packages]]
-include = "openbb_fmp"
-from = "./providers/fmp"
+include = "openbb_fred"
+from = "./providers/fred"
 
 [[tool.poetry.packages]]
-include = "openbb_alpha_vantage"
-from = "./providers/alpha_vantage"
+include = "openbb_tmx"
+from = "./providers/tmx"
 
 [[tool.poetry.packages]]
-include = "openbb_currency"
-from = "./extensions/currency"
+include = "openbb_econometrics"
+from = "./extensions/econometrics"
 
 [[tool.poetry.packages]]
 include = "openbb_commodity"
 from = "./extensions/commodity"
 
 [[tool.poetry.packages]]
-include = "openbb_index"
-from = "./extensions/index"
-
-[[tool.poetry.packages]]
-include = "openbb_technical"
-from = "./extensions/technical"
-
-[[tool.poetry.packages]]
-include = "openbb_economy"
-from = "./extensions/economy"
+include = "openbb_derivatives"
+from = "./extensions/derivatives"
 
 [[tool.poetry.packages]]
 include = "openbb_news"
 from = "./extensions/news"
 
 [[tool.poetry.packages]]
-include = "openbb_econometrics"
-from = "./extensions/econometrics"
-
-[[tool.poetry.packages]]
-include = "openbb_equity"
-from = "./extensions/equity"
+include = "openbb_index"
+from = "./extensions/index"
 
 [[tool.poetry.packages]]
-include = "openbb_regulators"
-from = "./extensions/regulators"
+include = "openbb_devtools"
+from = "./extensions/devtools"
 
 [[tool.poetry.packages]]
-include = "openbb_etf"
-from = "./extensions/etf"
+include = "openbb_crypto"
+from = "./extensions/crypto"
 
 [[tool.poetry.packages]]
 include = "openbb_fixedincome"
 from = "./extensions/fixedincome"
 
 [[tool.poetry.packages]]
+include = "openbb_equity"
+from = "./extensions/equity"
+
+[[tool.poetry.packages]]
+include = "openbb_economy"
+from = "./extensions/economy"
+
+[[tool.poetry.packages]]
 include = "openbb_quantitative"
 from = "./extensions/quantitative"
 
 [[tool.poetry.packages]]
-include = "openbb_devtools"
-from = "./extensions/devtools"
+include = "openbb_technical"
+from = "./extensions/technical"
 
 [[tool.poetry.packages]]
-include = "openbb_crypto"
-from = "./extensions/crypto"
+include = "openbb_regulators"
+from = "./extensions/regulators"
 
 [[tool.poetry.packages]]
-include = "openbb_derivatives"
-from = "./extensions/derivatives"
+include = "openbb_currency"
+from = "./extensions/currency"
+
+[[tool.poetry.packages]]
+include = "openbb_etf"
+from = "./extensions/etf"
 
 [[tool.poetry.packages]]
 include = "openbb_charting"
 from = "./obbject_extensions/charting"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -188,30 +188,28 @@
 python-multipart = "^0.0.6"
 pydantic = "^2.5.1"
 requests = "^2.31.0"
 importlib-metadata = "^6.8.0"
 python-dotenv = "^1.0.0"
 aiohttp = "^3.9.0"
 ruff = "^0.1.5"
-requests-cache = "^1.1.0"
 urllib3 = ">1.26.16"
 defusedxml = "^0.8.0rc2"
+pytest-freezegun = "^0.4.2"
+requests-cache = "^1.1.0"
+random-user-agent = "^1.0.1"
+nasdaq-data-link = "^1.0.4"
+finvizfinance = "0.14.7"
 aiohttp-client-cache = "^0.10.0"
 aiosqlite = "^0.19.0"
-random-user-agent = "^1.0.1"
-exchange-calendars = "^4.2.8"
 xmltodict = "^0.13.0"
-nasdaq-data-link = "^1.0.4"
 yfinance = "^0.2.27"
-finvizfinance = "0.14.7"
-pytest-freezegun = "^0.4.2"
+exchange-calendars = "^4.2.8"
 scipy = "^1.10.0"
 statsmodels = "^0.14.0"
-scikit-learn = "^1.3.1"
-pandas-ta = "^0.3.14b"
 arch = "^5.5.0"
 linearmodels = "<=4.25"
 pylint = "^3.0.2"
 mypy = "^1.6.1"
 pydocstyle = "^6.3.0"
 black = "^24.1.0"
 bandit = "^1.7.5"
@@ -220,57 +218,59 @@
 tox = "^4.11.3"
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 ipykernel = "^6.26.0"
 types-python-dateutil = "^2.8.19.14"
 types-toml = "^0.10.8.7"
 poetry = "^1.7.0"
+pandas-ta = "^0.3.14b"
+scikit-learn = "^1.3.1"
 plotly = "^5.17.0"
 reportlab = "^4.0.4"
 pywry = "^0.6.1"
 svglib = "^1.5.1"
 nbformat = "^5.9.2"
 
 [tool.poetry.plugins.openbb_core_extension]
-currency = "openbb_currency.currency_router:router"
+econometrics = "openbb_econometrics.econometrics_router:router"
 commodity = "openbb_commodity.commodity_router:router"
-index = "openbb_index.index_router:router"
-technical = "openbb_technical.technical_router:router"
-economy = "openbb_economy.economy_router:router"
+derivatives = "openbb_derivatives.derivatives_router:router"
 news = "openbb_news.news_router:router"
-econometrics = "openbb_econometrics.econometrics_router:router"
+index = "openbb_index.index_router:router"
+crypto = "openbb_crypto.crypto_router:router"
+fixedincome = "openbb_fixedincome.fixedincome_router:router"
 equity = "openbb_equity.equity_router:router"
+economy = "openbb_economy.economy_router:router"
+quantitative = "openbb_quantitative.quantitative_router:router"
+technical = "openbb_technical.technical_router:router"
 regulators = "openbb_regulators.regulators_router:router"
+currency = "openbb_currency.currency_router:router"
 etf = "openbb_etf.etf_router:router"
-fixedincome = "openbb_fixedincome.fixedincome_router:router"
-quantitative = "openbb_quantitative.quantitative_router:router"
-crypto = "openbb_crypto.crypto_router:router"
-derivatives = "openbb_derivatives.derivatives_router:router"
 
 [tool.poetry.plugins.openbb_provider_extension]
-tradingeconomics = "openbb_tradingeconomics:tradingeconomics_provider"
-biztoc = "openbb_biztoc:biztoc_provider"
-federal_reserve = "openbb_federal_reserve:federal_reserve_provider"
 oecd = "openbb_oecd:oecd_provider"
-fred = "openbb_fred:fred_provider"
-tmx = "openbb_tmx:tmx_provider"
-seeking_alpha = "openbb_seeking_alpha:seeking_alpha_provider"
-ecb = "openbb_ecb:ecb_provider"
-intrinio = "openbb_intrinio:intrinio_provider"
-polygon = "openbb_polygon:polygon_provider"
-nasdaq = "openbb_nasdaq:nasdaq_provider"
-cboe = "openbb_cboe:cboe_provider"
-yfinance = "openbb_yfinance:yfinance_provider"
-finviz = "openbb_finviz:finviz_provider"
+benzinga = "openbb_benzinga:benzinga_provider"
 finra = "openbb_finra:finra_provider"
 stockgrid = "openbb_stockgrid:stockgrid_provider"
-tiingo = "openbb_tiingo:tiingo_provider"
-benzinga = "openbb_benzinga:benzinga_provider"
+biztoc = "openbb_biztoc:biztoc_provider"
 wsj = "openbb_wsj:wsj_provider"
-tradier = "openbb_tradier:tradier_provider"
-government_us = "openbb_government_us:government_us_provider"
-sec = "openbb_sec:sec_provider"
+nasdaq = "openbb_nasdaq:nasdaq_provider"
+finviz = "openbb_finviz:finviz_provider"
+polygon = "openbb_polygon:polygon_provider"
+intrinio = "openbb_intrinio:intrinio_provider"
+cboe = "openbb_cboe:cboe_provider"
 fmp = "openbb_fmp:fmp_provider"
+seeking_alpha = "openbb_seeking_alpha:seeking_alpha_provider"
+tiingo = "openbb_tiingo:tiingo_provider"
 alpha_vantage = "openbb_alpha_vantage:alpha_vantage_provider"
+tradier = "openbb_tradier:tradier_provider"
+sec = "openbb_sec:sec_provider"
+tradingeconomics = "openbb_tradingeconomics:tradingeconomics_provider"
+yfinance = "openbb_yfinance:yfinance_provider"
+ecb = "openbb_ecb:ecb_provider"
+government_us = "openbb_government_us:government_us_provider"
+federal_reserve = "openbb_federal_reserve:federal_reserve_provider"
+fred = "openbb_fred:fred_provider"
+tmx = "openbb_tmx:tmx_provider"
 
 [tool.poetry.plugins.openbb_obbject_extension]
 openbb_charting = "openbb_charting:ext"
```

### Comparing `openbb_nightly-4.1.6.dev202404030009/PKG-INFO` & `openbb_nightly-4.1.6.dev202404040010/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.6.dev202404030009
+Version: 4.1.6.dev202404040010
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

