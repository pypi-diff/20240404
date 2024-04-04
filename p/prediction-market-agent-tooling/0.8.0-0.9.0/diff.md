# Comparing `tmp/prediction_market_agent_tooling-0.8.0.tar.gz` & `tmp/prediction_market_agent_tooling-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prediction_market_agent_tooling-0.8.0.tar", max compression
+gzip compressed data, was "prediction_market_agent_tooling-0.9.0.tar", max compression
```

## Comparing `prediction_market_agent_tooling-0.8.0.tar` & `prediction_market_agent_tooling-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0     7650 2024-04-02 13:18:35.221075 prediction_market_agent_tooling-0.8.0/LICENSE
--rw-r--r--   0        0        0     2985 2024-04-02 13:18:35.221075 prediction_market_agent_tooling-0.8.0/README.md
--rw-r--r--   0        0        0     9578 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
--rw-r--r--   0        0        0    11406 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
--rw-r--r--   0        0        0     9841 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
--rw-r--r--   0        0        0     4777 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
--rw-r--r--   0        0        0     7315 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json
--rw-r--r--   0        0        0     1775 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json
--rw-r--r--   0        0        0    15953 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json
--rw-r--r--   0        0        0     6055 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/wxdai.abi.json
--rw-r--r--   0        0        0        0 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/__init__.py
--rw-r--r--   0        0        0     3737 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/agents.py
--rw-r--r--   0        0        0    21237 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/benchmark.py
--rw-r--r--   0        0        0     2748 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/utils.py
--rw-r--r--   0        0        0     2596 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/config.py
--rw-r--r--   0        0        0     7627 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/agent.py
--rw-r--r--   0        0        0      607 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/agent_example.py
--rw-r--r--   0        0        0       82 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/constants.py
--rw-r--r--   0        0        0     3739 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/gcp/deploy.py
--rw-r--r--   0        0        0     5255 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/gcp/utils.py
--rw-r--r--   0        0        0     2526 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/gtypes.py
--rw-r--r--   0        0        0     4488 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/agent_market.py
--rw-r--r--   0        0        0     1026 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/categorize.py
--rw-r--r--   0        0        0      763 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/data_models.py
--rw-r--r--   0        0        0        0 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/__init__.py
--rw-r--r--   0        0        0     6882 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/api.py
--rw-r--r--   0        0        0     5357 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/data_models.py
--rw-r--r--   0        0        0     3402 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/manifold.py
--rw-r--r--   0        0        0      513 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/utils.py
--rw-r--r--   0        0        0     1550 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/markets.py
--rw-r--r--   0        0        0        0 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/__init__.py
--rw-r--r--   0        0        0    10343 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/data_models.py
--rw-r--r--   0        0        0    23821 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen.py
--rw-r--r--   0        0        0    18800 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py
--rw-r--r--   0        0        0     5508 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py
--rw-r--r--   0        0        0    11382 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
--rw-r--r--   0        0        0    13738 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
--rw-r--r--   0        0        0     4188 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/api.py
--rw-r--r--   0        0        0     4199 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/data_models.py
--rw-r--r--   0        0        0    10863 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
--rw-r--r--   0        0        0     2652 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py
--rw-r--r--   0        0        0     1960 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/utils.py
--rw-r--r--   0        0        0     2503 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/markets/manifold.py
--rw-r--r--   0        0        0     2419 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/markets/omen.py
--rw-r--r--   0        0        0     2413 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/markets/polymarket.py
--rw-r--r--   0        0        0    11465 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/monitor.py
--rw-r--r--   0        0        0     4045 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/monitor_app.py
--rw-r--r--   0        0        0        0 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/py.typed
--rw-r--r--   0        0        0      625 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/balances.py
--rw-r--r--   0        0        0     3520 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
--rw-r--r--   0        0        0     4367 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
--rw-r--r--   0        0        0      422 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
--rw-r--r--   0        0        0      429 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
--rw-r--r--   0        0        0      499 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/cache.py
--rw-r--r--   0        0        0     5879 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/contract.py
--rw-r--r--   0        0        0      660 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/gnosis_rpc.py
--rw-r--r--   0        0        0     1761 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/google.py
--rw-r--r--   0        0        0     2037 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/hexbytes_custom.py
--rw-r--r--   0        0        0     2613 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/is_predictable.py
--rw-r--r--   0        0        0      733 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/parallelism.py
--rw-r--r--   0        0        0     4674 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/utils.py
--rw-r--r--   0        0        0     5314 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/web3_utils.py
--rw-r--r--   0        0        0     1355 2024-04-02 13:18:35.229075 prediction_market_agent_tooling-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4653 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7650 2024-04-04 11:57:12.147864 prediction_market_agent_tooling-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2992 2024-04-04 11:57:12.147864 prediction_market_agent_tooling-0.9.0/README.md
+-rw-r--r--   0        0        0     9578 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
+-rw-r--r--   0        0        0    11406 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
+-rw-r--r--   0        0        0     9841 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
+-rw-r--r--   0        0        0     4777 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
+-rw-r--r--   0        0        0     7315 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json
+-rw-r--r--   0        0        0     1775 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json
+-rw-r--r--   0        0        0    15953 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json
+-rw-r--r--   0        0        0     6055 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/wxdai.abi.json
+-rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/__init__.py
+-rw-r--r--   0        0        0     3737 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/agents.py
+-rw-r--r--   0        0        0    21237 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2748 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/utils.py
+-rw-r--r--   0        0        0     2596 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/config.py
+-rw-r--r--   0        0        0     7621 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent.py
+-rw-r--r--   0        0        0      621 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent_example.py
+-rw-r--r--   0        0        0       82 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/constants.py
+-rw-r--r--   0        0        0     3739 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/deploy.py
+-rw-r--r--   0        0        0     5255 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/utils.py
+-rw-r--r--   0        0        0     2526 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/gtypes.py
+-rw-r--r--   0        0        0     4488 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/agent_market.py
+-rw-r--r--   0        0        0     1026 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/categorize.py
+-rw-r--r--   0        0        0      763 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/data_models.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/__init__.py
+-rw-r--r--   0        0        0     6882 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/api.py
+-rw-r--r--   0        0        0     5357 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/data_models.py
+-rw-r--r--   0        0        0     3402 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/manifold.py
+-rw-r--r--   0        0        0      513 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/utils.py
+-rw-r--r--   0        0        0     1550 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/markets.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/__init__.py
+-rw-r--r--   0        0        0    10800 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/data_models.py
+-rw-r--r--   0        0        0    27589 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen.py
+-rw-r--r--   0        0        0    19354 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py
+-rw-r--r--   0        0        0     7399 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_replicate.py
+-rw-r--r--   0        0        0    11382 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
+-rw-r--r--   0        0        0    15423 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
+-rw-r--r--   0        0        0     4188 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/api.py
+-rw-r--r--   0        0        0     4199 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models.py
+-rw-r--r--   0        0        0    10863 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
+-rw-r--r--   0        0        0     2652 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py
+-rw-r--r--   0        0        0     1960 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/utils.py
+-rw-r--r--   0        0        0     2503 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/manifold.py
+-rw-r--r--   0        0        0     2419 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/omen.py
+-rw-r--r--   0        0        0     2413 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/polymarket.py
+-rw-r--r--   0        0        0    11465 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor.py
+-rw-r--r--   0        0        0     4045 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor_app.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/py.typed
+-rw-r--r--   0        0        0      625 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/balances.py
+-rw-r--r--   0        0        0     3520 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
+-rw-r--r--   0        0        0     4367 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
+-rw-r--r--   0        0        0      422 2024-04-04 11:57:12.151864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
+-rw-r--r--   0        0        0      429 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
+-rw-r--r--   0        0        0      499 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/cache.py
+-rw-r--r--   0        0        0     5879 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/contract.py
+-rw-r--r--   0        0        0      660 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/gnosis_rpc.py
+-rw-r--r--   0        0        0     1761 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/google.py
+-rw-r--r--   0        0        0     2037 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/hexbytes_custom.py
+-rw-r--r--   0        0        0     2613 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/is_predictable.py
+-rw-r--r--   0        0        0      733 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/parallelism.py
+-rw-r--r--   0        0        0      729 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/singleton.py
+-rw-r--r--   0        0        0     4674 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/utils.py
+-rw-r--r--   0        0        0     5314 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/web3_utils.py
+-rw-r--r--   0        0        0     1355 2024-04-04 11:57:12.155864 prediction_market_agent_tooling-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.9.0/PKG-INFO
```

### Comparing `prediction_market_agent_tooling-0.8.0/LICENSE` & `prediction_market_agent_tooling-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/README.md` & `prediction_market_agent_tooling-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ```python
 import random
 from prediction_market_agent_tooling.deploy.agent import DeployableAgent
 from prediction_market_agent_tooling.markets.agent_market import AgentMarket
 
 class DeployableCoinFlipAgent(DeployableAgent):
-    def answer_binary_market(self, market: AgentMarket) -> bool:
+    def answer_binary_market(self, market: AgentMarket) -> bool | None:
         return random.choice([True, False])
 
 DeployableCoinFlipAgent().deploy_gcp(...)
 ```
 
 ## Monitoring
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_dxdao.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_kleros.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_oracle.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/omen_realitio.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/abis/wxdai.abi.json` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/abis/wxdai.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/agents.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/agents.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/benchmark.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/benchmark/utils.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/config.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/config.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/agent.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     AgentMarket,
     FilterBy,
     SortBy,
 )
 from prediction_market_agent_tooling.markets.data_models import BetAmount
 from prediction_market_agent_tooling.markets.markets import MarketType
 from prediction_market_agent_tooling.markets.omen.omen import (
-    redeem_positions_from_all_omen_markets,
+    redeem_positions_from_all_user_bets,
 )
 from prediction_market_agent_tooling.monitor.monitor_app import (
     MARKET_TYPE_TO_DEPLOYED_AGENT,
 )
 from prediction_market_agent_tooling.tools.utils import DatetimeWithTimezone, utcnow
 
 MAX_AVAILABLE_MARKETS = 20
@@ -180,15 +180,15 @@
 
     def before(self, market_type: MarketType) -> None:
         """
         Executes actions that occur before bets are placed.
         """
 
         if market_type == MarketType.OMEN:
-            redeem_positions_from_all_omen_markets()
+            redeem_positions_from_all_user_bets()
 
     def process_bets(self, market_type: MarketType, _place_bet: bool = True) -> None:
         """
         Processes bets placed by agents on a given market.
         """
         available_markets = self.get_markets(market_type)
         markets = self.pick_markets(available_markets)
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/agent_example.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/agent_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 from prediction_market_agent_tooling.markets.agent_market import AgentMarket
 
 
 class DeployableCoinFlipAgent(DeployableAgent):
     def pick_markets(self, markets: list[AgentMarket]) -> list[AgentMarket]:
         return random.sample(markets, 1)
 
-    def answer_binary_market(self, market: AgentMarket) -> bool:
+    def answer_binary_market(self, market: AgentMarket) -> bool | None:
         return random.choice([True, False])
 
 
 class DeployableAlwaysRaiseAgent(DeployableAgent):
-    def answer_binary_market(self, market: AgentMarket) -> bool:
+    def answer_binary_market(self, market: AgentMarket) -> bool | None:
         raise RuntimeError("I always raise!")
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/gcp/deploy.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/deploy.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/deploy/gcp/utils.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/deploy/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/gtypes.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/gtypes.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/agent_market.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/agent_market.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/categorize.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/categorize.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/data_models.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/api.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/data_models.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/manifold.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/manifold/utils.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/manifold/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/markets.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/markets.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/data_models.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/data_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,34 +66,44 @@
     @property
     def n_outcomes(self) -> int:
         return len(self.outcomes)
 
 
 class OmenPosition(BaseModel):
     id: HexBytes
-    conditionIds: t.List[HexBytes]
+    conditionIds: list[HexBytes]
+    collateralTokenAddress: HexAddress
+    indexSets: list[int]
+
+    @property
+    def collateral_token_contract_address_checksummed(self) -> ChecksumAddress:
+        return Web3.to_checksum_address(self.collateralTokenAddress)
 
 
 class OmenUserPosition(BaseModel):
     id: HexBytes
     position: OmenPosition
+    balance: Wei
+    wrappedBalance: Wei
+    totalBalance: Wei
 
 
 class OmenMarket(BaseModel):
     """
     https://aiomen.eth.limo
     """
 
     BET_AMOUNT_CURRENCY: t.ClassVar[Currency] = Currency.xDai
 
     id: HexAddress
     title: str
     creator: HexAddress
     category: str
     collateralVolume: Wei
+    liquidityMeasure: Wei
     usdVolume: USD
     collateralToken: HexAddress
     outcomes: list[str]
     outcomeTokenAmounts: list[OmenOutcomeToken]
     outcomeTokenMarginalPrices: t.Optional[list[xDai]]
     fee: t.Optional[Wei]
     resolutionTimestamp: t.Optional[int] = None
@@ -118,18 +128,21 @@
     @property
     def is_resolved(self) -> bool:
         return (
             # Finalized on Realitio (e.g. 24h has passed since the last answer was submitted)
             self.answerFinalizedTimestamp is not None
             # Resolved on Oracle (e.g. resolved after it was finalized)
             and self.resolutionTimestamp is not None
-            and self.has_valid_answer
         )
 
     @property
+    def is_resolved_with_valid_answer(self) -> bool:
+        return self.is_resolved and self.has_valid_answer
+
+    @property
     def question_title(self) -> str:
         return self.title
 
     @property
     def creation_datetime(self) -> datetime | None:
         return (
             datetime.fromtimestamp(self.creationTimestamp)
@@ -216,22 +229,22 @@
 
     @property
     def boolean_outcome(self) -> bool:
         if not self.is_binary:
             raise ValueError(
                 f"Market with title {self.title} is not binary, it has {len(self.outcomes)} outcomes."
             )
-        if not self.is_resolved:
+        if not self.is_resolved_with_valid_answer:
             raise ValueError(f"Bet with title {self.title} is not resolved.")
 
         outcome: str = self.outcomes[check_not_none(self.answer_index)]
         return get_boolean_outcome(outcome)
 
     def get_resolution_enum(self) -> t.Optional[Resolution]:
-        if not self.is_resolved:
+        if not self.is_resolved_with_valid_answer:
             return None
         if self.boolean_outcome:
             return Resolution.YES
         else:
             return Resolution.NO
 
     @property
@@ -278,15 +291,15 @@
         profit -= wei_to_xdai(self.feeAmount)
         return ProfitAmount(
             amount=profit,
             currency=Currency.xDai,
         )
 
     def to_generic_resolved_bet(self) -> ResolvedBet:
-        if not self.fpmm.is_resolved:
+        if not self.fpmm.is_resolved_with_valid_answer:
             raise ValueError(
                 f"Bet with title {self.title} is not resolved. It has no resolution time."
             )
 
         return ResolvedBet(
             amount=BetAmount(
                 amount=Decimal(self.collateralAmountUSD), currency=Currency.xDai
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     OmenFixedProductMarketMakerFactoryContract,
     OmenOracleContract,
     OmenRealitioContract,
 )
 from prediction_market_agent_tooling.markets.omen.omen_subgraph_handler import (
     OmenSubgraphHandler,
 )
+from prediction_market_agent_tooling.tools.balances import get_balances
 from prediction_market_agent_tooling.tools.web3_utils import (
     add_fraction,
     private_key_to_public_key,
     remove_fraction,
     wei_to_xdai,
     xdai_to_wei,
 )
@@ -70,14 +71,20 @@
     market_maker_contract_address_checksummed: ChecksumAddress
     condition: Condition
 
     INVALID_MARKET_ANSWER: HexStr = HexStr(
         "0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF"
     )
 
+    def get_liquidity(self) -> Wei:
+        return self.get_contract().totalSupply()
+
+    def get_liquidity_in_xdai(self) -> xDai:
+        return wei_to_xdai(self.get_liquidity())
+
     def get_tiny_bet_amount(self) -> BetAmount:
         return BetAmount(amount=Decimal(0.00001), currency=self.currency)
 
     def place_bet(
         self, outcome: bool, amount: BetAmount, omen_auto_deposit: bool = True
     ) -> None:
         if amount.currency != self.currency:
@@ -199,34 +206,38 @@
     else:
         raise ValueError(f"Unknown sort_by: {sort_by}")
 
 
 def get_omen_binary_markets(
     limit: int | None,
     sort_by: SortBy,
-    filter_by: FilterBy = FilterBy.OPEN,
+    filter_by: FilterBy,
     created_after: t.Optional[datetime] = None,
     opened_before: t.Optional[datetime] = None,
+    opened_after: t.Optional[datetime] = None,
     finalized_before: t.Optional[datetime] = None,
     finalized: bool | None = None,
     resolved: bool | None = None,
     creator: t.Optional[HexAddress] = None,
+    liquidity_bigger_than: Wei | None = None,
     excluded_questions: set[str] | None = None,
 ) -> list[OmenMarket]:
     subgraph_handler = OmenSubgraphHandler()
     return subgraph_handler.get_omen_binary_markets(
         limit=limit,
         sort_by=sort_by,
         created_after=created_after,
         opened_before=opened_before,
+        opened_after=opened_after,
         finalized_before=finalized_before,
         finalized=finalized,
         resolved=resolved,
         filter_by=filter_by,
         creator=creator,
+        liquidity_bigger_than=liquidity_bigger_than,
         excluded_questions=excluded_questions,
     )
 
 
 def pick_binary_market(
     sort_by: SortBy = SortBy.CLOSING_SOONEST, filter_by: FilterBy = FilterBy.OPEN
 ) -> OmenMarket:
@@ -524,26 +535,23 @@
 
     parent_collection_id = build_parent_collection_id()
 
     if not market.is_resolved():
         logger.debug("Cannot redeem winnings if market is not yet resolved. Exiting.")
         return
 
-    amount_wei = get_conditional_tokens_balance_for_market(market, from_address, web3)
+    amount_per_index = get_conditional_tokens_balance_for_market(
+        market, from_address, web3
+    )
+    amount_wei = sum(amount_per_index.values())
     if amount_wei == 0:
         logger.debug("No balance to claim. Exiting.")
         return
 
-    # check if condition has already been resolved by oracle
-    payout_for_condition = conditional_token_contract.payoutDenominator(
-        market.condition.id
-    )
-    if not payout_for_condition > 0:
-        # from ConditionalTokens.redeemPositions:
-        # uint den = payoutDenominator[conditionId]; require(den > 0, "result for condition not received yet");
+    if not conditional_token_contract.is_condition_resolved(market.condition.id):
         logger.debug("Market not yet resolved, not possible to claim")
         return
 
     conditional_token_contract.redeemPositions(
         from_private_key=from_private_key,
         collateral_token_address=market.collateral_token_contract_address_checksummed,
         condition_id=market.condition.id,
@@ -553,53 +561,58 @@
     )
 
 
 def get_conditional_tokens_balance_for_market(
     market: OmenAgentMarket,
     from_address: ChecksumAddress,
     web3: Web3 | None = None,
-) -> Wei:
+) -> dict[int, Wei]:
     """
     We derive the withdrawable balance from the ConditionalTokens contract through CollectionId -> PositionId (which
     also serves as tokenId) -> TokenBalances.
     """
+    balance_per_index_set: dict[int, Wei] = {}
     conditional_token_contract = OmenConditionalTokenContract()
     parent_collection_id = build_parent_collection_id()
-    balance = wei_type(0)
 
     for index_set in market.condition.index_sets:
         collection_id = conditional_token_contract.getCollectionId(
             parent_collection_id, market.condition.id, index_set, web3=web3
         )
         # Note that collection_id is returned as bytes, which is accepted by the contract calls downstream.
         position_id: int = conditional_token_contract.getPositionId(
             market.collateral_token_contract_address_checksummed,
             collection_id,
             web3=web3,
         )
         balance_for_position = conditional_token_contract.balanceOf(
             from_address=from_address, position_id=position_id, web3=web3
         )
-        balance = wei_type(balance + balance_for_position)
+        balance_per_index_set[index_set] = wei_type(balance_for_position)
 
-    return balance
+    return balance_per_index_set
 
 
 def omen_remove_fund_market_tx(
     market: OmenAgentMarket,
     shares: Wei | None,
     from_private_key: PrivateKey,
     web3: Web3 | None = None,
 ) -> None:
     """
     Removes funding from a given OmenMarket (moving the funds from the OmenMarket to the
     ConditionalTokens contract), and finally calls the `mergePositions` method which transfers collateralToken from the ConditionalTokens contract to the address corresponding to `from_private_key`.
+
+    Warning: Liquidity removal works on the principle of getting market's shares, not the collateral token itself.
+    After we remove funding, using the `mergePositions` we get `min(shares per index)` of wxDai back, but the remaining shares can be converted back only after the market is resolved.
+    That can be done using the `redeem_from_all_user_positions` function below.
     """
     from_address = private_key_to_public_key(from_private_key)
     market_contract = market.get_contract()
+    original_balances = get_balances(from_address)
 
     total_shares = market_contract.balanceOf(from_address, web3=web3)
     if total_shares == 0:
         logger.info("No shares to remove.")
         return
 
     if shares is None or shares > total_shares:
@@ -610,29 +623,94 @@
 
     market_contract.removeFunding(
         remove_funding=shares, from_private_key=from_private_key, web3=web3
     )
 
     conditional_tokens = OmenConditionalTokenContract()
     parent_collection_id = build_parent_collection_id()
+    amount_per_index_set = get_conditional_tokens_balance_for_market(
+        market, from_address, web3
+    )
+    # We fetch the minimum balance of outcome token - for ex, in this tx (https://gnosisscan.io/tx/0xc31c4e9bc6a60cf7db9991a40ec2f2a06e3539f8cb8dd81b6af893cef6f40cd7#eventlog) - event #460, this should yield 9804940144070370149. This amount matches what is displayed in the Omen UI.
+    # See similar logic from Olas
+    # https://github.com/valory-xyz/market-creator/blob/4bc47f696fb5ecb61c3b7ec8c001ff2ab6c60fcf/packages/valory/skills/market_creation_manager_abci/behaviours.py#L1308
+    amount_to_merge = min(amount_per_index_set.values())
+
     result = conditional_tokens.mergePositions(
         from_private_key=from_private_key,
         collateral_token_address=market.collateral_token_contract_address_checksummed,
         parent_collection_id=parent_collection_id,
         conditionId=market.condition.id,
         index_sets=market.condition.index_sets,
-        amount=shares,
+        amount=amount_to_merge,
         web3=web3,
     )
+    new_balances = get_balances(from_address)
+
     logger.debug(f"Result from merge positions {result}")
+    logger.info(
+        f"Withdrawn {new_balances.wxdai - original_balances.wxdai} wxDai from liquidity at {market.url=}."
+    )
 
 
-def redeem_positions_from_all_omen_markets() -> None:
+def redeem_from_all_user_positions(
+    from_private_key: PrivateKey,
+    web3: Web3 | None = None,
+) -> None:
+    """
+    Redeems from all user positions where the user didn't redeem yet.
     """
-    Redeems positions from all resolved Omen markets.
+    public_key = private_key_to_public_key(from_private_key)
+
+    conditional_token_contract = OmenConditionalTokenContract()
+    user_positions = OmenSubgraphHandler().get_user_positions(
+        public_key,
+        # After redeem, this will became zero and we won't re-process it.
+        total_balance_bigger_than=wei_type(0),
+    )
+
+    for index, user_position in enumerate(user_positions):
+        # I didn't find any example where this wouldn't hold, but keeping this double-check here in case something changes in the future.
+        if len(user_position.position.conditionIds) != 1:
+            raise ValueError(
+                f"Bug in the logic, please investigate why zero or multiple conditions are returned for {user_position.id=}"
+            )
+        condition_id = user_position.position.conditionIds[0]
+
+        if not conditional_token_contract.is_condition_resolved(condition_id):
+            logger.info(
+                f"[{index+1} / {len(user_positions)}] Skipping redeem, {user_position.id=} isn't resolved yet."
+            )
+            continue
+
+        logger.info(
+            f"[{index+1} / {len(user_positions)}] Processing redeem from {user_position.id=}."
+        )
+
+        original_balances = get_balances(public_key)
+        conditional_token_contract.redeemPositions(
+            from_private_key=from_private_key,
+            collateral_token_address=user_position.position.collateral_token_contract_address_checksummed,
+            condition_id=condition_id,
+            parent_collection_id=build_parent_collection_id(),
+            index_sets=user_position.position.indexSets,
+            web3=web3,
+        )
+        new_balances = get_balances(public_key)
+
+        logger.info(
+            f"Redeemed {new_balances.wxdai - original_balances.wxdai} wxDai from position {user_position.id=}."
+        )
+
+
+def redeem_positions_from_all_user_bets() -> None:
+    """
+    Redeems positions from all resolved Omen markets where the user placed a bet.
+
+    Note: This function is very similar to `redeem_from_all_user_positions`, but it will redeem only positions obtained from bets, not from liquidity withdrawals.
     """
     keys = APIKeys()
     omen_subgraph_handler = OmenSubgraphHandler()
     resolved_omen_bets = omen_subgraph_handler.get_resolved_bets(
         better_address=keys.bet_from_address,
         start_time=datetime(2020, 1, 1),
     )
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_contracts.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,23 @@
 
     def does_condition_exists(
         self,
         condition_id: HexBytes,
     ) -> bool:
         return self.getOutcomeSlotCount(condition_id) > 0
 
+    def is_condition_resolved(
+        self,
+        condition_id: HexBytes,
+    ) -> bool:
+        # from ConditionalTokens.redeemPositions:
+        # uint den = payoutDenominator[conditionId]; require(den > 0, "result for condition not received yet");
+        payout_for_condition = self.payoutDenominator(condition_id)
+        return payout_for_condition > 0
+
     def payoutDenominator(self, condition_id: HexBytes) -> int:
         payoutForCondition: int = self.call(
             "payoutDenominator",
             [condition_id],
         )
         return payoutForCondition
 
@@ -357,14 +366,19 @@
             from_private_key=from_private_key,
             function_name="removeFunding",
             function_params=[remove_funding],
             tx_params=tx_params,
             web3=web3,
         )
 
+    def totalSupply(self) -> Wei:
+        # This is the liquidity you seen on the Omen website (but in Wei).
+        total_supply: Wei = self.call("totalSupply")
+        return total_supply
+
 
 class WrappedxDaiContract(ContractERC20OnGnosisChain):
     # File content taken from https://gnosisscan.io/address/0xe91d153e0b41518a2ce8dd3d7944fa863463a97d#code.
     abi: ABI = abi_field_validator(
         os.path.join(
             os.path.dirname(os.path.realpath(__file__)), "../../abis/wxdai.abi.json"
         )
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import sys
 import typing as t
 from datetime import datetime
 
 from eth_typing import ChecksumAddress
 from subgrounds import FieldPath, Subgrounds
 
-from prediction_market_agent_tooling.gtypes import HexAddress, HexBytes
+from prediction_market_agent_tooling.gtypes import HexAddress, HexBytes, Wei
 from prediction_market_agent_tooling.markets.agent_market import FilterBy, SortBy
 from prediction_market_agent_tooling.markets.omen.data_models import (
     OMEN_FALSE_OUTCOME,
     OMEN_TRUE_OUTCOME,
     OmenBet,
     OmenMarket,
     OmenUserPosition,
     RealityAnswer,
     RealityQuestion,
 )
+from prediction_market_agent_tooling.tools.singleton import SingletonMeta
 from prediction_market_agent_tooling.tools.utils import to_int_timestamp, utcnow
 from prediction_market_agent_tooling.tools.web3_utils import ZERO_BYTES
 
 
-class OmenSubgraphHandler:
+class OmenSubgraphHandler(metaclass=SingletonMeta):
+
     """
     Class responsible for handling interactions with Omen subgraphs (trades, conditionalTokens).
     """
 
     OMEN_TRADES_SUBGRAPH = "https://api.thegraph.com/subgraphs/name/protofire/omen-xdai"
     CONDITIONAL_TOKENS_SUBGRAPH = (
         "https://api.thegraph.com/subgraphs/name/gnosis/conditional-tokens-gc"
@@ -91,14 +93,15 @@
         # Since it's still not working, we hardcode the schema to be fetched below.
         return [
             markets_field.id,
             markets_field.title,
             markets_field.creator,
             markets_field.collateralVolume,
             markets_field.usdVolume,
+            markets_field.liquidityMeasure,
             markets_field.collateralToken,
             markets_field.outcomes,
             markets_field.outcomeTokenAmounts,
             markets_field.outcomeTokenMarginalPrices,
             markets_field.fee,
             markets_field.answerFinalizedTimestamp,
             markets_field.resolutionTimestamp,
@@ -120,42 +123,59 @@
     def _build_where_statements(
         self,
         filter_by: FilterBy,
         creator: t.Optional[HexAddress] = None,
         outcomes: list[str] = [OMEN_TRUE_OUTCOME, OMEN_FALSE_OUTCOME],
         created_after: t.Optional[datetime] = None,
         opened_before: t.Optional[datetime] = None,
+        opened_after: t.Optional[datetime] = None,
         finalized_before: t.Optional[datetime] = None,
         finalized: bool | None = None,
         resolved: bool | None = None,
+        liquidity_bigger_than: Wei | None = None,
+        condition_id_in: list[HexBytes] | None = None,
         excluded_questions: set[str] | None = None,
     ) -> dict[str, t.Any]:
         where_stms: dict[str, t.Any] = {
             "isPendingArbitration": False,
             "outcomes": outcomes,
             "title_not": None,
             "question_": {},
+            "condition_": {},
         }
 
         if creator:
             where_stms["creator"] = creator
 
         if created_after:
             where_stms["creationTimestamp_gt"] = to_int_timestamp(created_after)
 
         if opened_before:
             where_stms["openingTimestamp_lt"] = to_int_timestamp(opened_before)
 
+        if opened_after:
+            where_stms["openingTimestamp_gt"] = to_int_timestamp(opened_after)
+
+        if liquidity_bigger_than is not None:
+            where_stms["liquidityMeasure_gt"] = liquidity_bigger_than
+
+        if condition_id_in is not None:
+            where_stms["condition_"]["id_in"] = [x.hex() for x in condition_id_in]
+
         if filter_by == FilterBy.RESOLVED:
             finalized = True
             resolved = True
         elif filter_by == FilterBy.OPEN:
             where_stms["currentAnswer"] = None
             finalized = False
             resolved = False
+        elif filter_by == FilterBy.NONE:
+            pass
+        else:
+            raise ValueError(f"Unknown filter_by: {filter_by}")
 
         if resolved is not None:
             if resolved:
                 where_stms["resolutionTimestamp_not"] = None
             else:
                 where_stms["resolutionTimestamp"] = None
 
@@ -193,31 +213,37 @@
     def get_omen_binary_markets(
         self,
         limit: t.Optional[int],
         sort_by: SortBy,
         filter_by: FilterBy,
         created_after: t.Optional[datetime] = None,
         opened_before: t.Optional[datetime] = None,
+        opened_after: t.Optional[datetime] = None,
         finalized_before: t.Optional[datetime] = None,
         finalized: bool | None = None,
         resolved: bool | None = None,
         creator: t.Optional[HexAddress] = None,
+        liquidity_bigger_than: Wei | None = None,
+        condition_id_in: list[HexBytes] | None = None,
         excluded_questions: set[str] | None = None,  # question titles
         outcomes: list[str] = [OMEN_TRUE_OUTCOME, OMEN_FALSE_OUTCOME],
     ) -> t.List[OmenMarket]:
         where_stms = self._build_where_statements(
             filter_by=filter_by,
             creator=creator,
             outcomes=outcomes,
             created_after=created_after,
             opened_before=opened_before,
+            opened_after=opened_after,
             finalized_before=finalized_before,
             finalized=finalized,
             resolved=resolved,
+            condition_id_in=condition_id_in,
             excluded_questions=excluded_questions,
+            liquidity_bigger_than=liquidity_bigger_than,
         )
 
         sort_direction = self._build_sort_direction(sort_by)
         markets = self.trades_subgraph.Query.fixedProductMarketMakers(
             orderBy=self.trades_subgraph.FixedProductMarketMaker.creationTimestamp,
             orderDirection=sort_direction,
             first=(
@@ -259,28 +285,43 @@
                 # subgrounds might pack all items as a list, indexed by a key, or pack it as a dictionary (if one single element)
                 if isinstance(v, dict):
                     items.extend([v])
                 else:
                     items.extend(v)
         return items
 
+    def _get_fields_for_user_positions(self, positions: FieldPath) -> list[FieldPath]:
+        return [
+            positions.id,
+            positions.position.id,
+            positions.position.conditionIds,
+            positions.position.collateralTokenAddress,
+            positions.position.indexSets,
+            positions.balance,
+            positions.wrappedBalance,
+            positions.totalBalance,
+        ]
+
     def get_user_positions(
-        self, better_address: ChecksumAddress
+        self,
+        better_address: ChecksumAddress,
+        total_balance_bigger_than: Wei | None = None,
     ) -> list[OmenUserPosition]:
-        positions = self.conditional_tokens_subgraph.Query.userPositions(
-            first=sys.maxsize,
-            where=[
-                self.conditional_tokens_subgraph.UserPosition.user
-                == better_address.lower()
-            ],
-        )
+        where_stms: dict[str, t.Any] = {
+            "user": better_address.lower(),
+        }
 
-        result = self.sg.query_json(
-            [positions.id, positions.position.id, positions.position.conditionIds]
+        if total_balance_bigger_than is not None:
+            where_stms["totalBalance_gt"] = total_balance_bigger_than
+
+        positions = self.conditional_tokens_subgraph.Query.userPositions(
+            first=sys.maxsize, where=where_stms
         )
+        fields = self._get_fields_for_user_positions(positions)
+        result = self.sg.query_json(fields)
         items = self._parse_items_from_json(result)
         return [OmenUserPosition.model_validate(i) for i in items]
 
     def get_bets(
         self,
         better_address: ChecksumAddress,
         start_time: datetime,
@@ -321,15 +362,15 @@
         omen_bets = self.get_bets(
             better_address=better_address,
             start_time=start_time,
             end_time=end_time,
             market_id=market_id,
             filter_by_answer_finalized_not_null=True,
         )
-        return [b for b in omen_bets if b.fpmm.is_resolved]
+        return [b for b in omen_bets if b.fpmm.is_resolved_with_valid_answer]
 
     def get_questions(
         self,
         user: HexAddress | None = None,
         claimed: bool | None = None,
         current_answer_before: datetime | None = None,
     ) -> list[RealityQuestion]:
```

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/api.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/data_models.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/data_models_web.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/markets/polymarket/utils.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/markets/polymarket/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/markets/manifold.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/markets/omen.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/omen.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/markets/polymarket.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/markets/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/monitor.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/monitor/monitor_app.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/monitor/monitor_app.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/balances.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/balances.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/contract.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/contract.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/gnosis_rpc.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/gnosis_rpc.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/google.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/google.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/hexbytes_custom.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/hexbytes_custom.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/is_predictable.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/is_predictable.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/parallelism.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/parallelism.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/utils.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/prediction_market_agent_tooling/tools/web3_utils.py` & `prediction_market_agent_tooling-0.9.0/prediction_market_agent_tooling/tools/web3_utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.8.0/pyproject.toml` & `prediction_market_agent_tooling-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prediction-market-agent-tooling"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tools to benchmark, deploy and monitor prediction market agents."
 authors = ["Gnosis"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 buy_omen = "scripts.bet_omen:buy"
 sell_omen = "scripts.bet_omen:sell"
```

### Comparing `prediction_market_agent_tooling-0.8.0/PKG-INFO` & `prediction_market_agent_tooling-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prediction-market-agent-tooling
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools to benchmark, deploy and monitor prediction market agents.
 Author: Gnosis
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
@@ -93,15 +93,15 @@
 
 ```python
 import random
 from prediction_market_agent_tooling.deploy.agent import DeployableAgent
 from prediction_market_agent_tooling.markets.agent_market import AgentMarket
 
 class DeployableCoinFlipAgent(DeployableAgent):
-    def answer_binary_market(self, market: AgentMarket) -> bool:
+    def answer_binary_market(self, market: AgentMarket) -> bool | None:
         return random.choice([True, False])
 
 DeployableCoinFlipAgent().deploy_gcp(...)
 ```
 
 ## Monitoring
```

