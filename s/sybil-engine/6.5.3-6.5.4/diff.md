# Comparing `tmp/sybil_engine-6.5.3.tar.gz` & `tmp/sybil_engine-6.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil_engine-6.5.3.tar", last modified: Wed Apr  3 11:17:25 2024, max compression
+gzip compressed data, was "sybil_engine-6.5.4.tar", last modified: Thu Apr  4 19:49:04 2024, max compression
```

## Comparing `sybil_engine-6.5.3.tar` & `sybil_engine-6.5.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.258681 sybil_engine-6.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-03 11:17:25.258681 sybil_engine-6.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:17:25.258681 sybil_engine-6.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.246680 sybil_engine-6.5.3/sybil_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.246680 sybil_engine-6.5.3/sybil_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/config/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.246680 sybil_engine-6.5.3/sybil_engine/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/erc20_test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/erc20contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/transaction_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/contract/weth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.246680 sybil_engine-6.5.3/sybil_engine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/data/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/data/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/data/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/data/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/data/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.250681 sybil_engine-6.5.3/sybil_engine/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/account_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.250681 sybil_engine-6.5.3/sybil_engine/domain/balance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/balance/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/balance/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/dex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/domain/generic_swap_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.250681 sybil_engine-6.5.3/sybil_engine/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/module/execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/module/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/module/module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/module/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.254680 sybil_engine-6.5.3/sybil_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/app_account_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/arguments_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/binance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/cex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/fee_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/gas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/l0_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/okx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/scal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/validation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/wallet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/sybil_engine/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.258681 sybil_engine-6.5.3/sybil_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-03 11:17:25.000000 sybil_engine-6.5.3/sybil_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-03 11:17:25.000000 sybil_engine-6.5.3/sybil_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:17:25.000000 sybil_engine-6.5.3/sybil_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 11:17:25.000000 sybil_engine-6.5.3/sybil_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 11:17:25.000000 sybil_engine-6.5.3/sybil_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.254680 sybil_engine-6.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.254680 sybil_engine-6.5.3/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/data/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/data/test_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.254680 sybil_engine-6.5.3/test/module/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.254680 sybil_engine-6.5.3/test/module/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/contract/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/mock_fail_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/mock_not_enoguth_native_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/repeatable_mock_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.258681 sybil_engine-6.5.3/test/module/swap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/swap/mock_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/swap/mock_test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/swap/test_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/swap/test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/test_execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/test_module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/module/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:25.258681 sybil_engine-6.5.3/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/utils/test_binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/utils/test_create_app_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 11:17:18.000000 sybil_engine-6.5.3/test/utils/test_validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.043450 sybil_engine-6.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-04 19:49:04.043450 sybil_engine-6.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:49:04.043450 sybil_engine-6.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.027449 sybil_engine-6.5.4/sybil_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.027449 sybil_engine-6.5.4/sybil_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/config/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.031449 sybil_engine-6.5.4/sybil_engine/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/erc20_test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/erc20contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/transaction_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/contract/weth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.031449 sybil_engine-6.5.4/sybil_engine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/data/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/data/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/data/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/data/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/data/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.031449 sybil_engine-6.5.4/sybil_engine/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/account_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.031449 sybil_engine-6.5.4/sybil_engine/domain/balance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/balance/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/balance/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/domain/generic_swap_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.035450 sybil_engine-6.5.4/sybil_engine/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/module/execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/module/module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/module/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.039450 sybil_engine-6.5.4/sybil_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/app_account_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/arguments_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/binance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/cex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/fee_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/gas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/l0_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/okx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/scal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/validation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/wallet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/sybil_engine/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.043450 sybil_engine-6.5.4/sybil_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-04 19:49:04.000000 sybil_engine-6.5.4/sybil_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-04 19:49:04.000000 sybil_engine-6.5.4/sybil_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:49:04.000000 sybil_engine-6.5.4/sybil_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 19:49:04.000000 sybil_engine-6.5.4/sybil_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 19:49:04.000000 sybil_engine-6.5.4/sybil_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.039450 sybil_engine-6.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.039450 sybil_engine-6.5.4/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/data/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/data/test_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.039450 sybil_engine-6.5.4/test/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.039450 sybil_engine-6.5.4/test/module/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/contract/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/mock_fail_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/mock_not_enoguth_native_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/repeatable_mock_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.043450 sybil_engine-6.5.4/test/module/swap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/swap/mock_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/swap/mock_test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/swap/test_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/swap/test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/test_execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/test_module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/module/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:49:04.043450 sybil_engine-6.5.4/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/utils/test_binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/utils/test_create_app_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 19:48:59.000000 sybil_engine-6.5.4/test/utils/test_validation_utils.py
```

### Comparing `sybil_engine-6.5.3/PKG-INFO` & `sybil_engine-6.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.5.3
+Version: 6.5.4
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
```

### Comparing `sybil_engine-6.5.3/README.md` & `sybil_engine-6.5.4/README.md`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/setup.py` & `sybil_engine-6.5.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = file.readlines()
 
 setup(
     name='sybil_engine',
-    version='6.5.3',
+    version='6.5.4',
     py_modules=['sybil_engine'],
     packages=find_packages(),
     install_requires=requirements,
     data_files=[('', ['requirements.txt'])],
     author='Indeoo',
     author_email='indeooars@gmail.com',
     description='Engine for web3 smart contracts automatization.',
```

### Comparing `sybil_engine-6.5.3/sybil_engine/app.py` & `sybil_engine-6.5.4/sybil_engine/app.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/config/app_config.py` & `sybil_engine-6.5.4/sybil_engine/config/app_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/contract/contract.py` & `sybil_engine-6.5.4/sybil_engine/contract/contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/contract/erc20_test_contract.py` & `sybil_engine-6.5.4/sybil_engine/contract/erc20_test_contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/contract/erc20contract.py` & `sybil_engine-6.5.4/sybil_engine/contract/erc20contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/contract/send.py` & `sybil_engine-6.5.4/sybil_engine/contract/send.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/contract/transaction_executor.py` & `sybil_engine-6.5.4/sybil_engine/contract/transaction_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/contract/weth.py` & `sybil_engine-6.5.4/sybil_engine/contract/weth.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/data/contracts.py` & `sybil_engine-6.5.4/sybil_engine/data/contracts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/data/networks.py` & `sybil_engine-6.5.4/sybil_engine/data/networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/data/pairs.py` & `sybil_engine-6.5.4/sybil_engine/data/pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/data/tokens.py` & `sybil_engine-6.5.4/sybil_engine/data/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/domain/balance/balance.py` & `sybil_engine-6.5.4/sybil_engine/domain/balance/balance.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/domain/balance/balance_utils.py` & `sybil_engine-6.5.4/sybil_engine/domain/balance/balance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/domain/balance/tokens.py` & `sybil_engine-6.5.4/sybil_engine/domain/balance/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/domain/dex.py` & `sybil_engine-6.5.4/sybil_engine/domain/dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/domain/generic_swap_facade.py` & `sybil_engine-6.5.4/sybil_engine/domain/generic_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/module/execution_planner.py` & `sybil_engine-6.5.4/sybil_engine/module/execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/module/module.py` & `sybil_engine-6.5.4/sybil_engine/module/module.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/module/module_executor.py` & `sybil_engine-6.5.4/sybil_engine/module/module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/module/modules.py` & `sybil_engine-6.5.4/sybil_engine/module/modules.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/accumulator.py` & `sybil_engine-6.5.4/sybil_engine/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/app_account_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/app_account_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/arguments_parser.py` & `sybil_engine-6.5.4/sybil_engine/utils/arguments_parser.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/binance_prices.py` & `sybil_engine-6.5.4/sybil_engine/utils/binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/binance_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/binance_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from binance.error import ClientError
 from binance.spot import Spot
 
-from sybil_engine.utils.decryptor import decrypt_cex_data
+from sybil_engine.utils.decryptor import read_cex_data
 from sybil_engine.utils.utils import ConfigurationException
 
 
 networks = {
     'ZKSYNC': 'ZKSYNCERA',
     'BASE': 'BASE',
     'ARBITRUM': 'ARBITRUM',
@@ -45,33 +45,33 @@
                 {'asset': balance['asset'], 'free': balance['free']}
             )
 
     return assets
 
 
 def binance_transfer_from_sub_acc(password, binance_secret):
-    apiKey, secretKey = decrypt_cex_data(binance_secret, password)
+    apiKey, secretKey = read_cex_data(binance_secret, password)
 
     for sub_account in get_sub_accounts(apiKey, secretKey):
         assets = get_sub_account_balance(apiKey, secretKey, sub_account)
         transfer_sub_accounts(apiKey, secretKey, sub_account, assets)
 
 
 def binance_withdrawal(binance_secret, password, token, amount, address, chain):
-    apiKey, secretKey = decrypt_cex_data(binance_secret, password)
+    apiKey, secretKey = read_cex_data(binance_secret, password)
 
     client = Spot(api_key=apiKey, api_secret=secretKey)
     try:
         client.withdraw(token, amount, address, network=networks[chain])
     except ClientError as e:
         raise ConfigurationException(e.error_message)
 
 
 def get_binance_deposit_addresses(password, cex_data):
-    apiKey, secretKey = decrypt_cex_data(cex_data, password)
+    apiKey, secretKey = read_cex_data(cex_data, password)
 
     client = Spot(api_key=apiKey, api_secret=secretKey)
 
     emails = get_sub_accounts(apiKey, secretKey)
 
     deposit_addresses = []
```

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/configuration_loader.py` & `sybil_engine-6.5.4/sybil_engine/utils/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/decryptor.py` & `sybil_engine-6.5.4/sybil_engine/utils/decryptor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+from loguru import logger
 
 
 def generate_key(password):
     salt = b'\x87\x12\xac\xa3\x91\xb9\xfe\xb4\x08\x0c\xac\x19\xc6d\x85'
     kdf = PBKDF2HMAC(
         algorithm=hashes.SHA256(),
         length=32,
@@ -22,9 +23,13 @@
 def decrypt_private_key(encrypted_private_key, password):
     key = generate_key(password)
     fernet = Fernet(key)
     decrypted_private_key = fernet.decrypt(encrypted_private_key)
     return decrypted_private_key.decode()
 
 
-def decrypt_cex_data(encrypted_private_key, password):
-    return Fernet(generate_key(password)).decrypt(encrypted_private_key).decode('utf-8').split(',')
+def read_cex_data(cex_data, password):
+    try:
+        return Fernet(generate_key(password)).decrypt(cex_data).decode('utf-8').split(',')
+    except Exception as e:
+        logger.warning("Can't read encrypted CEX data, trying to read unencrypted")
+        return cex_data
```

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/fee_storage.py` & `sybil_engine-6.5.4/sybil_engine/utils/fee_storage.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/gas_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/gas_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/logs.py` & `sybil_engine-6.5.4/sybil_engine/utils/logs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/okx_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/okx_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ccxt
 from loguru import logger
 from okx import Funding, SubAccount
 
-from sybil_engine.utils.decryptor import decrypt_cex_data
+from sybil_engine.utils.decryptor import read_cex_data
 
 networks = {
     'ZKSYNC': 'zkSync Era',
     'LINEA': 'Linea',
     'ARBITRUM': 'Arbitrum One',
     'BASE': 'Base',
     'POLYGON': 'Polygon',
@@ -38,15 +38,15 @@
                             return 0
                         else:
                             return withdrawal_fee
     raise ValueError(f"     не могу получить сумму комиссии, проверьте значения symbolWithdraw и network")
 
 
 def withdrawal(addr, password, chain, cex_data, withdraw_amount, token='ETH'):
-    api_key, secret_key, passphrase = decrypt_cex_data(cex_data, password)
+    api_key, secret_key, passphrase = read_cex_data(cex_data, password)
     flag = "0"
 
     if chain == 'POLYGON' and token == 'USDC':
         network = networks["POLYGON_BRIDGED"]
     else:
         network = networks[chain]
 
@@ -56,36 +56,36 @@
 
     fee = get_withdrawal_fee(api_key, secret_key, passphrase, token, withdraw_network)
 
     fundingAPI.withdrawal(ccy=token, amt=withdraw_amount, dest=4, toAddr=addr, fee=fee, chain=withdraw_network)
 
 
 def get_sub_accounts(cex_data, password):
-    api_key, secret_key, passphrase = decrypt_cex_data(cex_data, password)
+    api_key, secret_key, passphrase = read_cex_data(cex_data, password)
 
     flag = "0"  # Production trading: 0, Demo trading: 1
 
     subAccountAPI = SubAccount.SubAccountAPI(api_key, secret_key, passphrase, False, flag, debug=False)
 
     # Get subaccount list
     return subAccountAPI.get_subaccount_list()
 
 
 def get_sub_account_balance(acc_name, token, cex_data, password):
-    api_key, secret_key, passphrase = decrypt_cex_data(cex_data, password)
+    api_key, secret_key, passphrase = read_cex_data(cex_data, password)
 
     flag = "0"
 
     subAccountAPI = SubAccount.SubAccountAPI(api_key, secret_key, passphrase, False, flag, debug=False)
 
     return float(subAccountAPI.get_funding_balance(acc_name, token)['data'][0]['bal'])
 
 
 def transfer_from_sub_acc(acc_name, amount, token, cex_data, password):
-    api_key, secret_key, passphrase = decrypt_cex_data(cex_data, password)
+    api_key, secret_key, passphrase = read_cex_data(cex_data, password)
 
     flag = "0"
 
     subAccountAPI = Funding.FundingAPI(api_key, secret_key, passphrase, False, flag, debug=False)
 
     return subAccountAPI.funds_transfer(token, amount, 6, 6, type='2', subAcct=acc_name)
 
@@ -101,15 +101,15 @@
     amount = get_sub_account_balance(acc_name, token, cex_data, okx_secret)
     if amount > 0:
         logger.info(f"Transfer {amount} {token} from {acc_name} to Main account")
         transfer_from_sub_acc(acc_name, amount, token, cex_data, okx_secret)
 
 
 def get_okx_deposit_addresses(password, cex_data):
-    api_key, secret_key, passphrase = decrypt_cex_data(cex_data, password)
+    api_key, secret_key, passphrase = read_cex_data(cex_data, password)
 
     flag = "0"
 
     subAccountAPI = Funding.FundingAPI(api_key, secret_key, passphrase, False, flag, debug=False)
     sub_accounts = subAccountAPI.get_deposit_address('ETH')['data']
 
     return [sub_account['addr'] for sub_account in sub_accounts]
```

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/retry.py` & `sybil_engine-6.5.4/sybil_engine/utils/retry.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/scal_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/scal_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/telegram.py` & `sybil_engine-6.5.4/sybil_engine/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/validation_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine/utils/web3_utils.py` & `sybil_engine-6.5.4/sybil_engine/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/sybil_engine.egg-info/PKG-INFO` & `sybil_engine-6.5.4/sybil_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.5.3
+Version: 6.5.4
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
```

### Comparing `sybil_engine-6.5.3/sybil_engine.egg-info/SOURCES.txt` & `sybil_engine-6.5.4/sybil_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/__init__.py` & `sybil_engine-6.5.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/data/test_networks.py` & `sybil_engine-6.5.4/test/data/test_networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/data/test_pairs.py` & `sybil_engine-6.5.4/test/data/test_pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/contract/mock_router.py` & `sybil_engine-6.5.4/test/module/contract/mock_router.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/swap/mock_dex.py` & `sybil_engine-6.5.4/test/module/swap/mock_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/swap/mock_test_swap_facade.py` & `sybil_engine-6.5.4/test/module/swap/mock_test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/swap/test_dex.py` & `sybil_engine-6.5.4/test/module/swap/test_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/swap/test_swap_facade.py` & `sybil_engine-6.5.4/test/module/swap/test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/test_execution_planner.py` & `sybil_engine-6.5.4/test/module/test_execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/module/test_module_executor.py` & `sybil_engine-6.5.4/test/module/test_module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/test_config.py` & `sybil_engine-6.5.4/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/utils/test_binance_prices.py` & `sybil_engine-6.5.4/test/utils/test_binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/utils/test_create_app_accounts.py` & `sybil_engine-6.5.4/test/utils/test_create_app_accounts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.5.3/test/utils/test_validation_utils.py` & `sybil_engine-6.5.4/test/utils/test_validation_utils.py`

 * *Files identical despite different names*

