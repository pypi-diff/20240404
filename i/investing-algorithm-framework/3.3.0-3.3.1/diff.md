# Comparing `tmp/investing_algorithm_framework-3.3.0.tar.gz` & `tmp/investing_algorithm_framework-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-3.3.0.tar", max compression
+gzip compressed data, was "investing_algorithm_framework-3.3.1.tar", max compression
```

## Comparing `investing_algorithm_framework-3.3.0.tar` & `investing_algorithm_framework-3.3.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
--rw-r--r--   0        0        0    11343 2024-04-02 21:01:41.822444 investing_algorithm_framework-3.3.0/LICENSE
--rw-r--r--   0        0        0    19512 2024-04-02 21:01:41.822444 investing_algorithm_framework-3.3.0/README.md
--rw-r--r--   0        0        0     2084 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/__init__.py
--rw-r--r--   0        0        0      501 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0        0        0    35307 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0        0        0    30887 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/app.py
--rw-r--r--   0        0        0     1092 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/__init__.py
--rw-r--r--   0        0        0     2362 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0        0        0      154 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0        0        0      451 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0        0        0     1062 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0        0        0     1085 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0        0        0     3750 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0        0        0      963 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/task.py
--rw-r--r--   0        0        0      134 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/__init__.py
--rw-r--r--   0        0        0      587 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0        0        0      693 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0        0        0      727 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0        0        0      617 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0        0        0      506 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0        0        0     2020 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0        0        0      585 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0        0        0      158 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/run_strategies.py
--rw-r--r--   0        0        0      361 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0        0        0      442 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0        0        0      743 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0        0        0      437 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0        0        0       80 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0        0        0      603 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/create_app.py
--rw-r--r--   0        0        0     6206 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/dependency_container.py
--rw-r--r--   0        0        0     3866 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0        0        0     3686 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/config.py
--rw-r--r--   0        0        0     2293 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0        0        0      962 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/data_structures.py
--rw-r--r--   0        0        0      823 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/decimal_parsing.py
--rw-r--r--   0        0        0     1628 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/exceptions.py
--rw-r--r--   0        0        0     1121 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0        0        0      812 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/app_mode.py
--rw-r--r--   0        0        0      253 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
--rw-r--r--   0        0        0    13604 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
--rw-r--r--   0        0        0      674 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
--rw-r--r--   0        0        0      659 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/base_model.py
--rw-r--r--   0        0        0       87 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/market/__init__.py
--rw-r--r--   0        0        0      779 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/market/market_credential.py
--rw-r--r--   0        0        0      237 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0        0        0    10301 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0        0        0     1110 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0        0        0      814 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0        0        0      937 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0        0        0      751 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_type.py
--rw-r--r--   0        0        0      230 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0        0        0     2495 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1752 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
--rw-r--r--   0        0        0     3141 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      123 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0        0        0     1131 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
--rw-r--r--   0        0        0     4598 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/strategy_profile.py
--rw-r--r--   0        0        0     2659 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0        0        0     2798 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0        0        0     2011 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0        0        0       99 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/__init__.py
--rw-r--r--   0        0        0     6819 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade.py
--rw-r--r--   0        0        0      807 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade_status.py
--rw-r--r--   0        0        0     1119 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0        0        0     6791 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0        0        0      564 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_credential_service.py
--rw-r--r--   0        0        0     9759 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_data_sources.py
--rw-r--r--   0        0        0     3520 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_service.py
--rw-r--r--   0        0        0      115 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
--rw-r--r--   0        0        0      320 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0      258 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0        0        0      156 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0        0        0     1805 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/strategy.py
--rw-r--r--   0        0        0      700 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0        0        0    10969 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/backtesting.py
--rw-r--r--   0        0        0     2746 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0        0        0      275 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0        0        0      417 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0        0        0      608 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0        0        0      253 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/synchronized.py
--rw-r--r--   0        0        0     1361 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/__init__.py
--rw-r--r--   0        0        0      176 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
--rw-r--r--   0        0        0      732 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      327 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
--rw-r--r--   0        0        0      437 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
--rw-r--r--   0        0        0    16664 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
--rw-r--r--   0        0        0     5472 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
--rw-r--r--   0        0        0      142 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/model_extension.py
--rw-r--r--   0        0        0      102 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0        0        0      847 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py
--rw-r--r--   0        0        0      141 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0        0        0     3226 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1238 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      135 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0        0        0     1898 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0        0        0      842 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
--rw-r--r--   0        0        0      567 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      487 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0        0        0     3352 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0        0        0     1073 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0        0        0     1967 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
--rw-r--r--   0        0        0     1994 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0        0        0      680 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
--rw-r--r--   0        0        0     7661 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0      163 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0        0        0       91 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
--rw-r--r--   0        0        0    14984 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
--rw-r--r--   0        0        0      195 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
--rw-r--r--   0        0        0       43 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
--rw-r--r--   0        0        0    11932 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
--rw-r--r--   0        0        0     1318 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0        0        0      191 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/__init__.py
--rw-r--r--   0        0        0     1025 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
--rw-r--r--   0        0        0    14835 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_service.py
--rw-r--r--   0        0        0      624 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/configuration_service.py
--rw-r--r--   0        0        0      820 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_credential_service.py
--rw-r--r--   0        0        0      235 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
--rw-r--r--   0        0        0     5212 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
--rw-r--r--   0        0        0     6267 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
--rw-r--r--   0        0        0      159 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/__init__.py
--rw-r--r--   0        0        0     7774 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
--rw-r--r--   0        0        0    27733 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_service.py
--rw-r--r--   0        0        0      510 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/__init__.py
--rw-r--r--   0        0        0      825 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
--rw-r--r--   0        0        0     2055 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
--rw-r--r--   0        0        0     4493 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
--rw-r--r--   0        0        0     1984 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
--rw-r--r--   0        0        0    16126 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0     1052 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0        0        0      525 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_snapshot_service.py
--rw-r--r--   0        0        0      995 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0        0        0     8075 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0        0        0       68 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/trade_service/__init__.py
--rw-r--r--   0        0        0    14625 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/trade_service/trade_service.py
--rw-r--r--   0        0        0      742 2024-04-02 21:01:53.826645 investing_algorithm_framework-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/LICENSE
+-rw-r--r--   0        0        0    19512 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/README.md
+-rw-r--r--   0        0        0     2084 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0        0        0    35307 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0        0        0    31166 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/app.py
+-rw-r--r--   0        0        0     1092 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/__init__.py
+-rw-r--r--   0        0        0     2362 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0        0        0      451 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0        0        0     1062 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0        0        0     1085 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0        0        0     3750 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0        0        0      963 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/task.py
+-rw-r--r--   0        0        0      134 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0        0        0      693 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0        0        0      727 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0        0        0      617 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0        0        0      506 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0        0        0     2020 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0        0        0      585 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0        0        0      158 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/run_strategies.py
+-rw-r--r--   0        0        0      361 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0        0        0      743 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0        0        0      437 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0        0        0       80 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0        0        0      603 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/create_app.py
+-rw-r--r--   0        0        0     6312 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/dependency_container.py
+-rw-r--r--   0        0        0     3866 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0        0        0     2293 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0        0        0      962 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/data_structures.py
+-rw-r--r--   0        0        0      823 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/decimal_parsing.py
+-rw-r--r--   0        0        0     1628 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/exceptions.py
+-rw-r--r--   0        0        0     1121 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/app_mode.py
+-rw-r--r--   0        0        0      253 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
+-rw-r--r--   0        0        0    13604 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
+-rw-r--r--   0        0        0      674 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
+-rw-r--r--   0        0        0      659 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/base_model.py
+-rw-r--r--   0        0        0       87 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/market/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/market/market_credential.py
+-rw-r--r--   0        0        0      237 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0        0        0    10194 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0        0        0     1110 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0        0        0      814 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0        0        0      937 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0        0        0      751 2024-04-04 09:20:58.321474 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_type.py
+-rw-r--r--   0        0        0      230 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1752 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+-rw-r--r--   0        0        0     3141 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      123 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0        0        0     1131 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/position/position_snapshot.py
+-rw-r--r--   0        0        0     4598 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/strategy_profile.py
+-rw-r--r--   0        0        0     2659 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0        0        0     2798 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0        0        0     2011 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0        0        0       99 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trade/__init__.py
+-rw-r--r--   0        0        0     6819 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trade/trade.py
+-rw-r--r--   0        0        0      807 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trade/trade_status.py
+-rw-r--r--   0        0        0     1119 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0        0        0     6791 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0        0        0      564 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/market_credential_service.py
+-rw-r--r--   0        0        0     9941 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/market_data_sources.py
+-rw-r--r--   0        0        0     3520 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/market_service.py
+-rw-r--r--   0        0        0      115 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0      258 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0        0        0      156 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0        0        0     1805 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/strategy.py
+-rw-r--r--   0        0        0      700 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0        0        0    10969 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/backtesting.py
+-rw-r--r--   0        0        0     2746 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0        0        0      275 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0        0        0      417 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0        0        0      608 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0        0        0      253 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/synchronized.py
+-rw-r--r--   0        0        0     1361 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+-rw-r--r--   0        0        0      732 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/decimal_parser.py
+-rw-r--r--   0        0        0      437 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
+-rw-r--r--   0        0        0    17466 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
+-rw-r--r--   0        0        0     5472 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
+-rw-r--r--   0        0        0      142 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/model_extension.py
+-rw-r--r--   0        0        0      102 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0        0        0      847 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+-rw-r--r--   0        0        0      141 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     3226 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1238 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      135 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0        0        0      842 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
+-rw-r--r--   0        0        0      567 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      487 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0        0        0     3352 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0        0        0     1073 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0        0        0     1967 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
+-rw-r--r--   0        0        0     1994 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0        0        0      680 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
+-rw-r--r--   0        0        0     7661 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0      163 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
+-rw-r--r--   0        0        0    15303 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
+-rw-r--r--   0        0        0      195 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
+-rw-r--r--   0        0        0    11932 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
+-rw-r--r--   0        0        0     1318 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/backtesting/__init__.py
+-rw-r--r--   0        0        0     1025 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
+-rw-r--r--   0        0        0    15007 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/backtesting/backtest_service.py
+-rw-r--r--   0        0        0      624 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/configuration_service.py
+-rw-r--r--   0        0        0      820 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_credential_service.py
+-rw-r--r--   0        0        0      235 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_data_source_service/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
+-rw-r--r--   0        0        0     6267 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
+-rw-r--r--   0        0        0      159 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/order_service/__init__.py
+-rw-r--r--   0        0        0     7644 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/order_service/order_backtest_service.py
+-rw-r--r--   0        0        0    27823 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/order_service/order_service.py
+-rw-r--r--   0        0        0      510 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
+-rw-r--r--   0        0        0     2055 2024-04-04 09:20:58.325475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
+-rw-r--r--   0        0        0     4493 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_service.py
+-rw-r--r--   0        0        0     1984 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
+-rw-r--r--   0        0        0    16126 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0     1052 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0        0        0      525 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/position_snapshot_service.py
+-rw-r--r--   0        0        0      995 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0        0        0     8075 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0        0        0       68 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/trade_service/__init__.py
+-rw-r--r--   0        0        0    14625 2024-04-04 09:20:58.329475 investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/trade_service/trade_service.py
+-rw-r--r--   0        0        0      742 2024-04-04 09:21:06.681426 investing_algorithm_framework-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.3.1/PKG-INFO
```

### Comparing `investing_algorithm_framework-3.3.0/LICENSE` & `investing_algorithm_framework-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/README.md` & `investing_algorithm_framework-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/algorithm.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,15 +274,21 @@
         market_data_sources = market_data_source_service \
             .get_market_data_sources()
 
         if market_data_sources is not None:
             backtest_market_data_sources = [
                 market_data_source.to_backtest_market_data_source()
                 for market_data_source in market_data_sources
+                if market_data_source is not None
             ]
+
+            for market_data_source in backtest_market_data_sources:
+                if market_data_source is not None:
+                    market_data_source.config = self.config
+
             self.container.market_data_source_service.override(
                 BacktestMarketDataSourceService(
                     market_data_sources=backtest_market_data_sources,
                     market_service=self.container.market_service(),
                     market_credential_service=self.container
                     .market_credential_service(),
                     configuration_service=self.container
@@ -783,14 +789,15 @@
                 report=report, output_directory=output_directory
             )
             reports.append(report)
 
         return reports
 
     def add_market_data_source(self, market_data_source):
+        market_data_source.config = self.config
         self._market_data_source_service.add(market_data_source)
 
     def add_market_credential(self, market_credential: MarketCredential):
         market_credential.market = market_credential.market.upper()
         self._market_credential_service.add(market_credential)
 
     def on_initialize(self, app_hook: AppHook):
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/create_app.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/dependency_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     portfolio_configuration_service = providers.ThreadSafeSingleton(
         PortfolioConfigurationService,
         portfolio_repository=portfolio_repository,
         position_repository=position_repository,
     )
     order_service = providers.Factory(
         OrderService,
+        configuration_service=configuration_service,
         order_repository=order_repository,
         order_fee_repository=order_fee_repository,
         portfolio_repository=portfolio_repository,
         position_repository=position_repository,
         market_service=market_service,
         market_credential_service=market_credential_service,
         portfolio_configuration_service=portfolio_configuration_service,
@@ -121,14 +122,15 @@
         PerformanceService,
         order_repository=order_repository,
         position_repository=position_repository,
         portfolio_repository=portfolio_repository
     )
     backtest_service = providers.Factory(
         BacktestService,
+        configuration_service=configuration_service,
         order_service=order_service,
         portfolio_repository=portfolio_repository,
         performance_service=performance_service,
         position_repository=position_repository,
         market_data_source_service=market_data_source_service,
     )
     backtest_report_writer_service = providers.Factory(
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     RESOURCE_DIRECTORY = os.getenv(RESOURCE_DIRECTORY)
     SCHEDULER_API_ENABLED = True
     CHECK_PENDING_ORDERS = True
     SQLITE_ENABLED = True
     SQLITE_INITIALIZED = False
     BACKTEST_DATA_DIRECTORY_NAME = "backtest_data"
     SYMBOLS = None
+    DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
     def __init__(self, resource_directory=None):
         super().__init__()
 
         if resource_directory is not None:
             self.RESOURCE_DIRECTORY = resource_directory
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/data_structures.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/data_structures.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/decimal_parsing.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/decimal_parsing.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/app_mode.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/app_mode.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/backtest_position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/backtest_report.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/market/market_credential.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/market/market_credential.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
 from dateutil.parser import parse
-from dateutil.tz import gettz
 
 from investing_algorithm_framework.domain.exceptions import \
     OperationalException
 from investing_algorithm_framework.domain.models.base_model import BaseModel
 from investing_algorithm_framework.domain.models.order import OrderStatus, \
     OrderType, OrderSide
 from investing_algorithm_framework.domain.models.order.order_fee import \
@@ -304,18 +303,15 @@
             status=status,
             order_type=ccxt_order.get("type", None),
             order_side=ccxt_order.get("side", None),
             filled=ccxt_order.get("filled", None),
             remaining=ccxt_order.get("remaining", None),
             cost=ccxt_order.get("cost", None),
             fee=OrderFee.from_ccxt_fee(ccxt_order.get("fee", None)),
-            created_at=parse(
-                ccxt_order.get("datetime", None),
-                tzinfos={"UTC": gettz("UTC")}
-            )
+            created_at=parse(ccxt_order.get("datetime", None))
         )
 
     def __repr__(self):
 
         if not hasattr(self, "id"):
             id_value = "ccxt external order"
         else:
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position_snapshot.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/strategy_profile.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/strategy_profile.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trade/trade.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade_status.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trade/trade_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_credential_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_data_sources.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/market_data_sources.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,22 @@
         self._market = market
         self._symbol = symbol
         self._start_date = start_date
         self._end_date = end_date
         self._backtest_data_start_date = backtest_data_start_date
         self._backtest_data_index_date = backtest_data_index_date
 
+    @property
+    def config(self):
+        return self._config
+
+    @config.setter
+    def config(self, value):
+        self._config = value
+
     def _data_source_exists(self, file_path):
         """
         Function to check if the data source exists.
         This function will check if the file exists and if the column names
         are correct.
 
         This function will return True if the file exists and the column names
@@ -56,17 +64,15 @@
                         f"Wrong column names on {file_path}, required "
                         f"column names are {self.column_names}"
                     )
             else:
                 return False
 
             return True
-        except Exception as e:
-            logger.error(f"Error reading {file_path}")
-            logger.error(e)
+        except Exception:
             return False
 
     def write_data_to_file_path(self, data_file, data):
         """
         Function to write data to a csv file.
         This function will write the column names and all the data to the
         file.
@@ -147,31 +153,39 @@
     def backtest_data_index_date(self, value):
         self._backtest_data_index_date = value
 
 
 class MarketDataSource(ABC):
 
     def __init__(
-            self,
-            identifier,
-            market,
-            symbol,
+        self,
+        identifier,
+        market,
+        symbol,
     ):
         self._identifier = identifier
         self._market = market
         self._symbol = symbol
         self._market_credential_service = None
 
     def initialize(self, config):
         pass
 
     @property
     def identifier(self):
         return self._identifier
 
+    @property
+    def config(self):
+        return self._config
+
+    @config.setter
+    def config(self, value):
+        self._config = value
+
     def get_identifier(self):
         return self.identifier
 
     @property
     def market(self):
         return self._market
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/backtesting.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/backtesting.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import os
 from datetime import timedelta
 
 import polars
+from dateutil import parser
 
 from investing_algorithm_framework.domain import RESOURCE_DIRECTORY, \
     BACKTEST_DATA_DIRECTORY_NAME, DATETIME_FORMAT_BACKTESTING, \
     OperationalException, DATETIME_FORMAT, OHLCVMarketDataSource, \
     BacktestMarketDataSource, OrderBookMarketDataSource, \
     TickerMarketDataSource, TimeFrame
 from investing_algorithm_framework.infrastructure.services import \
@@ -55,15 +56,15 @@
             market=market,
             symbol=symbol,
             timeframe=timeframe,
             start_date=start_date,
             start_date_func=start_date_func,
             end_date=end_date,
             end_date_func=end_date_func,
-            window_size=window_size
+            window_size=window_size,
         )
 
     def prepare_data(
         self,
         config,
         backtest_start_date,
         backtest_end_date,
@@ -76,15 +77,14 @@
         This implementation will check if the data source already exists before
         pulling all the data. This optimization will prevent downloading
         of unnecessary resources.
 
         When downloading the data it will use the ccxt library.
         """
         # Calculating the backtest data start date
-
         difference = self.end_date - self.start_date
         total_minutes = 0
 
         if difference.days > 0:
             total_minutes += difference.days * 24 * 60
 
         if difference.seconds > 0:
@@ -123,15 +123,18 @@
                 except Exception as e:
                     logger.error(e)
                     raise OperationalException(
                         f"Could not create backtest data file {file_path}"
                     )
 
             # Get the OHLCV data from the ccxt market service
-            market_service = CCXTMarketService(self.market_credential_service)
+            market_service = CCXTMarketService(
+                market_credential_service=self.market_credential_service,
+            )
+            market_service.config = config
             ohlcv = market_service.get_ohlcv(
                 symbol=self.symbol,
                 time_frame=self.timeframe,
                 from_timestamp=backtest_data_start_date,
                 to_timestamp=backtest_end_date,
                 market=self.market
             )
@@ -167,14 +170,15 @@
         data.
         """
         file_path = self._create_file_path()
         to_timestamp = backtest_index_date
         from_timestamp = backtest_index_date - timedelta(
             minutes=self.total_minutes_timeframe
         )
+        datetime_format = self._config["DATETIME_FORMAT"]
         self.backtest_data_index_date = backtest_index_date\
             .replace(microsecond=0)
         from_timestamp = from_timestamp.replace(microsecond=0)
 
         if from_timestamp < self.backtest_data_start_date:
             raise OperationalException(
                 f"Cannot get data from {from_timestamp} as the "
@@ -189,30 +193,33 @@
 
         # Load the csv file and filter out the dates that are not in the
         # backtest index date range
         df = polars.read_csv(
             file_path, columns=self.column_names, separator=","
         )
         df = df.filter(
-            (df['Datetime'] >= from_timestamp.strftime(DATETIME_FORMAT))
-            & (df['Datetime'] <= to_timestamp.strftime(DATETIME_FORMAT))
+            (df['Datetime'] >= from_timestamp.strftime(datetime_format))
+            & (df['Datetime'] <= to_timestamp.strftime(datetime_format))
         )
         return df
 
     def to_backtest_market_data_source(self) -> BacktestMarketDataSource:
         # Ignore this method for now
         pass
 
     def empty(self):
         return False
 
     @property
     def file_name(self):
         return self._create_file_path().split("/")[-1]
 
+    def write_data_to_file_path(self, data_file, data: polars.DataFrame):
+        data.write_csv(data_file)
+
 
 class CCXTTickerBacktestMarketDataSource(
     TickerMarketDataSource, BacktestMarketDataSource
 ):
     """
     CCXTTickerBacktestMarketDataSource implementation using ccxt to download
     all data sources.
@@ -300,15 +307,18 @@
                 except Exception as e:
                     logger.error(e)
                     raise OperationalException(
                         f"Could not create backtest data file {file_path}"
                     )
 
             # Get the OHLCV data from the ccxt market service
-            market_service = CCXTMarketService(self.market_credential_service)
+            market_service = CCXTMarketService(
+                market_credential_service=self.market_credential_service
+            )
+            market_service.config = config
             ohlcv = market_service.get_ohlcv(
                 symbol=self.symbol,
                 time_frame=self.timeframe,
                 from_timestamp=self.backtest_data_start_date,
                 to_timestamp=backtest_end_date,
                 market=self.market
             )
@@ -359,21 +369,20 @@
             .amount_of_minutes
         backtest_index_date = kwargs["backtest_index_date"]
         end_date = backtest_index_date + timedelta(minutes=timeframe_minutes)
 
         # Filter the data based on the backtest index date and the end date
         df = polars.read_csv(file_path)
         df = df.filter(
-            (df['Datetime'] >= backtest_index_date
-             .strftime(DATETIME_FORMAT))
+            (df['Datetime'] >= backtest_index_date.strftime(DATETIME_FORMAT))
         )
-
         first_row = df.head(1)[0]
+        first_row_datetime = parser.parse(first_row["Datetime"][0])
 
-        if first_row["Datetime"][0] > end_date.strftime(DATETIME_FORMAT):
+        if first_row_datetime > end_date:
             logger.warning(
                 f"No ticker data available for the given backtest "
                 f"index date {backtest_index_date} and symbol {self.symbol} "
                 f"and market {self.market}"
             )
 
         # Calculate the bid and ask price based on the high and low price
@@ -382,20 +391,25 @@
             "bid": float((first_row["Low"][0])
                          + float(first_row["High"][0]))/2,
             "ask": float((first_row["Low"][0])
                          + float(first_row["High"][0]))/2,
             "datetime": first_row["Datetime"][0],
         }
 
+    def write_data_to_file_path(self, data_file, data: polars.DataFrame):
+        data.write_csv(data_file)
+
 
 class CCXTOHLCVMarketDataSource(OHLCVMarketDataSource):
 
     def get_data(self, **kwargs):
-        market_service = CCXTMarketService(self.market_credential_service)
-
+        market_service = CCXTMarketService(
+            market_credential_service=self.market_credential_service,
+        )
+        market_service.config = self.config
         if self.start_date is None:
             raise OperationalException(
                 "Either start_date or start_date_func should be set "
                 "for OHLCVMarketDataSource"
             )
 
         return market_service.get_ohlcv(
@@ -418,15 +432,18 @@
             timeframe=self.timeframe,
         )
 
 
 class CCXTOrderBookMarketDataSource(OrderBookMarketDataSource):
 
     def get_data(self, **kwargs):
-        market_service = CCXTMarketService(self.market_credential_service)
+        market_service = CCXTMarketService(
+            market_credential_service=self.market_credential_service
+        )
+        market_service.config = self.config
         return market_service.get_order_book(
             symbol=self.symbol, market=self.market
         )
 
     def to_backtest_market_data_source(self) -> BacktestMarketDataSource:
         pass
 
@@ -434,25 +451,29 @@
 class CCXTTickerMarketDataSource(TickerMarketDataSource):
 
     def __init__(
         self,
         identifier,
         market,
         symbol=None,
-        backtest_timeframe=None
+        backtest_timeframe=None,
+
     ):
         super().__init__(
             identifier=identifier,
             market=market,
             symbol=symbol,
         )
         self._backtest_timeframe = backtest_timeframe
 
     def get_data(self, **kwargs):
-        market_service = CCXTMarketService(self.market_credential_service)
+        market_service = CCXTMarketService(
+            market_credential_service=self.market_credential_service
+        )
+        market_service.config = self.config
 
         if self.market is None:
 
             if "market" not in kwargs:
                 raise OperationalException(
                     "Either market or market should be "
                     "passed as a parameter"
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import logging
-from typing import Dict
 from datetime import datetime
 from time import sleep
-import polars as pl
+from typing import Dict
+
 import ccxt
+import polars as pl
 from dateutil import parser
-from dateutil.tz import gettz
 
 from investing_algorithm_framework.domain import OperationalException, Order, \
-    CCXT_DATETIME_FORMAT, MarketService
+    MarketService
 
 logger = logging.getLogger(__name__)
 
 
 class CCXTMarketService(MarketService):
     """
     Market service implementation using the CCXT library
     """
     msec = 1000
     minute = 60 * msec
 
+    def __init__(self, market_credential_service):
+        super(CCXTMarketService, self).__init__(
+            market_credential_service=market_credential_service,
+        )
+
+    @property
+    def config(self):
+        return self._config
+
+    @config.setter
+    def config(self, config):
+        self._config = config
+
     def initialize_exchange(self, market, market_credential):
         market = market.lower()
         if not hasattr(ccxt, market):
             raise OperationalException(
                 f"No market service found for market id {market}"
             )
 
@@ -145,23 +158,24 @@
         except Exception as e:
             logger.exception(e)
             raise OperationalException("Could not retrieve order")
 
     def get_orders(self, symbol, market, since: datetime = None):
         market_credential = self.get_market_credential(market)
         exchange = self.initialize_exchange(market, market_credential)
+        datetime_format = self.config["DATETIME_FORMAT"]
 
         if not exchange.has['fetchOrders']:
             raise OperationalException(
                 f"Market service {market} does not support "
                 f"functionality get_orders"
             )
 
         if since is not None:
-            since = exchange.parse8601(since.strftime(":%Y-%m-%d %H:%M:%S"))
+            since = exchange.parse8601(datetime_format)
 
             try:
                 ccxt_orders = exchange.fetchOrders(symbol, since=since)
                 return [Order.from_ccxt_order(order) for order in ccxt_orders]
             except Exception as e:
                 logger.exception(e)
                 raise OperationalException("Could not retrieve orders")
@@ -339,56 +353,56 @@
         except Exception as e:
             logger.exception(e)
             raise OperationalException("Could not retrieve closed orders")
 
     def get_ohlcv(
         self, symbol, time_frame, from_timestamp, market, to_timestamp=None
     ) -> pl.DataFrame:
+        datetime_format = self.config["DATETIME_FORMAT"]
         market_credential = self.get_market_credential(market)
         exchange = self.initialize_exchange(market, market_credential)
 
         if not exchange.has['fetchOHLCV']:
             raise OperationalException(
                 f"Market service {market} does not support "
                 f"functionality get_ohclvs"
             )
 
         from_time_stamp = exchange.parse8601(
-            from_timestamp.strftime(CCXT_DATETIME_FORMAT)
+            from_timestamp.strftime(datetime_format)
         )
 
         if to_timestamp is None:
             to_timestamp = exchange.milliseconds()
         else:
             to_timestamp = exchange.parse8601(
-                to_timestamp.strftime(CCXT_DATETIME_FORMAT)
+                to_timestamp.strftime(datetime_format)
             )
         data = []
 
         while from_time_stamp < to_timestamp:
             ohlcv = exchange.fetch_ohlcv(symbol, time_frame, from_time_stamp)
 
             if len(ohlcv) > 0:
                 from_time_stamp = \
                     ohlcv[-1][0] + exchange.parse_timeframe(time_frame) * 1000
             else:
                 from_time_stamp = to_timestamp
 
             for candle in ohlcv:
-                datetime_stamp = parser.parse(
-                    exchange.iso8601(candle[0]),
-                    tzinfos={"UTC": gettz("UTC")}
+                datetime_stamp = parser.parse(exchange.iso8601(candle[0]))
 
-                )
                 to_timestamp_datetime = parser.parse(
                     exchange.iso8601(to_timestamp),
-                    tzinfos={"UTC": gettz("UTC")}
                 )
 
                 if datetime_stamp <= to_timestamp_datetime:
+                    datetime_stamp = datetime_stamp\
+                        .strftime(datetime_format)
+
                     data.append([datetime_stamp] + candle[1:])
 
             sleep(exchange.rateLimit / 1000)
 
         # Predefined column names
         col_names = ["Datetime", "Open", "High", "Low", "Close", "Volume"]
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/backtesting/backtest_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timedelta
-
+from dateutil import parser
 import pandas as pd
 from tqdm import tqdm
 
 from investing_algorithm_framework.domain import BacktestReport, \
     BACKTESTING_INDEX_DATETIME, TimeUnit, BacktestPosition, \
     TradingDataType, OrderStatus, OperationalException, MarketDataSource, \
     OrderSide
@@ -18,27 +18,29 @@
     def __init__(
         self,
         market_data_source_service: MarketDataSourceService,
         order_service,
         portfolio_repository,
         position_repository,
         performance_service,
+        configuration_service
     ):
         self._resource_directory = None
         self._order_service = order_service
         self._portfolio_repository = portfolio_repository
         self._data_index = {
             TradingDataType.OHLCV: {},
             TradingDataType.TICKER: {}
         }
         self._performance_service = performance_service
         self._position_repository = position_repository
         self._market_data_source_service: MarketDataSourceService \
             = market_data_source_service
         self._backtest_market_data_sources = []
+        self._configuration_service = configuration_service
 
     @property
     def resource_directory(self):
         return self._resource_directory
 
     @resource_directory.setter
     def resource_directory(self, resource_directory):
@@ -92,18 +94,19 @@
             total=len(schedule),
             desc=f"Running backtests {algorithm.name}",
             colour="GREEN"
         ):
             strategy_profile = self.get_strategy_from_strategy_profiles(
                 strategy_profiles, row['id']
             )
+            index_date = parser.parse(str(index))
             self.run_backtest_for_profile(
                 algorithm=algorithm,
                 strategy=algorithm.get_strategy(strategy_profile.strategy_id),
-                index_date=index,
+                index_date=index_date,
             )
         return self.create_backtest_report(
             algorithm, len(schedule), start_date, end_date, initial_unallocated
         )
 
     def run_backtests(self, algorithms, start_date, end_date=None):
         """
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/configuration_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_credential_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             desc="Preparing backtest market data",
             colour="GREEN"
         ):
 
             if backtest_market_data_source is not None:
                 backtest_market_data_source.market_credentials_service = \
                     self._market_credential_service
+
                 backtest_market_data_source.prepare_data(
                     config=configuration_service.get_config(),
                     backtest_start_date=configuration_service
                     .get_config()[BACKTESTING_START_DATE],
                     backtest_end_date=configuration_service
                     .get_config()[BACKTESTING_END_DATE],
                     market_credential_service=self._market_credential_service
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_backtest_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/order_service/order_backtest_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,14 @@
         """
 
         # Extract attributes from the order object
         created_at = order.get_created_at()
         order_side = order.get_order_side()
         order_price = order.get_price()
 
-        # Convert 'created_at' to pandas Timestamp for easier comparison
-        created_at = pd.Timestamp(created_at, tz='UTC')
-
         # Filter OHLCV data after the order creation time
         ohlcv_data_after_order = ohlcv_data_frame.loc[created_at:]
 
         # Check if the order execution conditions are met
         if OrderSide.BUY.equals(order_side):
             # Check if the low price drops below or equals the order price
             if (ohlcv_data_after_order['Low'] <= order_price).any():
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/order_service/order_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 logger = logging.getLogger("investing_algorithm_framework")
 
 
 class OrderService(RepositoryService):
 
     def __init__(
         self,
+        configuration_service,
         order_repository,
         order_fee_repository,
         market_service: MarketService,
         position_repository,
         portfolio_repository,
         portfolio_configuration_service,
         portfolio_snapshot_service,
         market_credential_service
     ):
         super(OrderService, self).__init__(order_repository)
+        self.configuration_service = configuration_service
         self.order_repository = order_repository
         self.order_fee_repository = order_fee_repository
         self.market_service: MarketService = market_service
         self.position_repository = position_repository
         self.portfolio_repository = portfolio_repository
         self.portfolio_configuration_service = portfolio_configuration_service
         self.portfolio_snapshot_service = portfolio_snapshot_service
```

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_snapshot_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/position_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/trade_service/trade_service.py` & `investing_algorithm_framework-3.3.1/investing_algorithm_framework/services/trade_service/trade_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.3.0/pyproject.toml` & `investing_algorithm_framework-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investing-algorithm-framework"
-version = "v3.3.0"
+version = "v3.3.1"
 description = "A framework for creating trading bots"
 authors = ["MDUYN"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 wrapt = "^1.16.0"
```

### Comparing `investing_algorithm_framework-3.3.0/PKG-INFO` & `investing_algorithm_framework-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 3.3.0
+Version: 3.3.1
 Summary: A framework for creating trading bots
 Author: MDUYN
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.3.0
+Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.3.1
 Summary: A framework for creating trading bots Author: MDUYN Requires-Python:
 >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.9,<4.0.0) Requires-Dist: Flask-Migrate
 (>=2.6.0,<3.0.0) Requires-Dist: MarkupSafe (>=2.1.2,<3.0.0) Requires-Dist:
```

