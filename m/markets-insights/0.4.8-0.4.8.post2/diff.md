# Comparing `tmp/markets_insights-0.4.8.tar.gz` & `tmp/markets_insights-0.4.8.post2.tar.gz`

## Comparing `markets_insights-0.4.8.tar` & `markets_insights-0.4.8.post2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 markets_insights-0.4.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 markets_insights-0.4.8/.vscode/launch.json
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 markets_insights-0.4.8/examples/aggregation.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 markets_insights-0.4.8/examples/arithmatic.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 markets_insights-0.4.8/examples/extending-datareader.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 markets_insights-0.4.8/examples/rsi-calculation.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 markets_insights-0.4.8/examples/test.py
--rw-r--r--   0        0        0  4036788 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/indices.csv
--rw-r--r--   0        0        0   117872 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY 100_Data.csv
--rw-r--r--   0        0        0    82385 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY 200_Data.csv
--rw-r--r--   0        0        0    23494 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY 50 ARBITRAGE_Data.csv
--rw-r--r--   0        0        0    65549 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY 50 FUTURES PR_Data.csv
--rw-r--r--   0        0        0   228864 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY 500_Data.csv
--rw-r--r--   0        0        0   263359 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY 50_Data.csv
--rw-r--r--   0        0        0    82126 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY AUTO_Data.csv
--rw-r--r--   0        0        0   148095 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY BANK_Data.csv
--rw-r--r--   0        0        0   111143 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY ENERGY_Data.csv
--rw-r--r--   0        0        0   155022 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY FMCG_Data.csv
--rw-r--r--   0        0        0    71336 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY HEALTHCARE_Data.csv
--rw-r--r--   0        0        0   190247 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY IT_Data(1).csv
--rw-r--r--   0        0        0   190247 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY IT_Data.csv
--rw-r--r--   0        0        0    64939 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY MEDIA_Data.csv
--rw-r--r--   0        0        0    87602 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY METAL_Data.csv
--rw-r--r--   0        0        0    71243 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY MICROCAP 250_Data.csv
--rw-r--r--   0        0        0   137050 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 100_Data.csv
--rw-r--r--   0        0        0    65521 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 150_Data(1).csv
--rw-r--r--   0        0        0    65521 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 150_Data.csv
--rw-r--r--   0        0        0   101170 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 50_Data.csv
--rw-r--r--   0        0        0   217315 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY NEXT 50_Data.csv
--rw-r--r--   0        0        0    71339 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY OIL & GAS_Data.csv
--rw-r--r--   0        0        0   114769 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY PHARMA_Data.csv
--rw-r--r--   0        0        0    65610 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY PRIVATE BANK_Data.csv
--rw-r--r--   0        0        0   162678 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY PSE_Data.csv
--rw-r--r--   0        0        0    85384 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY PSU BANK_Data.csv
--rw-r--r--   0        0        0    59354 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY REALTY_Data.csv
--rw-r--r--   0        0        0    82130 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY SMALLCAP 100_Data.csv
--rw-r--r--   0        0        0   136894 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY SMALLCAP 250_Data.csv
--rw-r--r--   0        0        0    71310 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY SMALLCAP 50_Data.csv
--rw-r--r--   0        0        0   173140 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY TOTAL MARKET_Data.csv
--rw-r--r--   0        0        0    23427 2020-02-02 00:00:00.000000 markets_insights-0.4.8/manual_data/Indices/NIFTY50 DIVIDEND POINTS_Data.csv
--rw-r--r--   0        0        0    35930 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/caching.ipynb
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/core.ipynb
--rw-r--r--   0        0        0   150141 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/equity.ipynb
--rw-r--r--   0        0        0   116346 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/examples.ipynb
--rw-r--r--   0        0        0   148847 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/index-nse.ipynb
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/index.ipynb
--rw-r--r--   0        0        0    13821 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/scratchpad.ipynb
--rw-r--r--   0        0        0   122869 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/derivatives/expiry-analysis.ipynb
--rw-r--r--   0        0        0    78498 2020-02-02 00:00:00.000000 markets_insights-0.4.8/notebooks/derivatives/rsi-trade-analysis.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/calculations/__init__.py
--rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/calculations/base.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/calculations/derivatives.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/calculations/equity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/core/__init__.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/core/column_definition.py
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/core/core.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/core/environment.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/core/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/dataprocess/__init__.py
--rw-r--r--   0        0        0    15825 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/dataprocess/data_processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/datareader/__init__.py
--rw-r--r--   0        0        0    33207 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/datareader/data_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/trade_builders/__init__.py
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/trade_builders/derivatives.py
--rw-r--r--   0        0        0     6899 2020-02-02 00:00:00.000000 markets_insights-0.4.8/src/markets_insights/trade_builders/results.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 markets_insights-0.4.8/tests/helper.py
--rw-r--r--   0        0        0    24098 2020-02-02 00:00:00.000000 markets_insights-0.4.8/tests/test_calculations.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 markets_insights-0.4.8/tests/test_dataprocess.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 markets_insights-0.4.8/tests/test_dataprocess_caching.py
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 markets_insights-0.4.8/tests/test_datareader.py
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 markets_insights-0.4.8/tests/test_datareader_has_data.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 markets_insights-0.4.8/.gitignore
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 markets_insights-0.4.8/LICENSE.MD
--rw-r--r--   0        0        0    18085 2020-02-02 00:00:00.000000 markets_insights-0.4.8/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 markets_insights-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    18247 2020-02-02 00:00:00.000000 markets_insights-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/.vscode/launch.json
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/examples/aggregation.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/examples/arithmatic.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/examples/extending-datareader.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/examples/rsi-calculation.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/examples/test.py
+-rw-r--r--   0        0        0  4036788 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/indices.csv
+-rw-r--r--   0        0        0   117872 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 100_Data.csv
+-rw-r--r--   0        0        0    82385 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 200_Data.csv
+-rw-r--r--   0        0        0    23494 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 50 ARBITRAGE_Data.csv
+-rw-r--r--   0        0        0    65549 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 50 FUTURES PR_Data.csv
+-rw-r--r--   0        0        0   228864 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 500_Data.csv
+-rw-r--r--   0        0        0   263359 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 50_Data.csv
+-rw-r--r--   0        0        0    82126 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY AUTO_Data.csv
+-rw-r--r--   0        0        0   148095 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY BANK_Data.csv
+-rw-r--r--   0        0        0   111143 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY ENERGY_Data.csv
+-rw-r--r--   0        0        0   155022 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY FMCG_Data.csv
+-rw-r--r--   0        0        0    71336 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY HEALTHCARE_Data.csv
+-rw-r--r--   0        0        0   190247 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY IT_Data(1).csv
+-rw-r--r--   0        0        0   190247 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY IT_Data.csv
+-rw-r--r--   0        0        0    64939 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MEDIA_Data.csv
+-rw-r--r--   0        0        0    87602 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY METAL_Data.csv
+-rw-r--r--   0        0        0    71243 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MICROCAP 250_Data.csv
+-rw-r--r--   0        0        0   137050 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 100_Data.csv
+-rw-r--r--   0        0        0    65521 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 150_Data(1).csv
+-rw-r--r--   0        0        0    65521 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 150_Data.csv
+-rw-r--r--   0        0        0   101170 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 50_Data.csv
+-rw-r--r--   0        0        0   217315 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY NEXT 50_Data.csv
+-rw-r--r--   0        0        0    71339 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY OIL & GAS_Data.csv
+-rw-r--r--   0        0        0   114769 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PHARMA_Data.csv
+-rw-r--r--   0        0        0    65610 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PRIVATE BANK_Data.csv
+-rw-r--r--   0        0        0   162678 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PSE_Data.csv
+-rw-r--r--   0        0        0    85384 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PSU BANK_Data.csv
+-rw-r--r--   0        0        0    59354 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY REALTY_Data.csv
+-rw-r--r--   0        0        0    82130 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY SMALLCAP 100_Data.csv
+-rw-r--r--   0        0        0   136894 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY SMALLCAP 250_Data.csv
+-rw-r--r--   0        0        0    71310 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY SMALLCAP 50_Data.csv
+-rw-r--r--   0        0        0   173140 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY TOTAL MARKET_Data.csv
+-rw-r--r--   0        0        0    23427 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/manual_data/Indices/NIFTY50 DIVIDEND POINTS_Data.csv
+-rw-r--r--   0        0        0    35930 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/caching.ipynb
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/core.ipynb
+-rw-r--r--   0        0        0   150141 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/equity.ipynb
+-rw-r--r--   0        0        0   116346 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/examples.ipynb
+-rw-r--r--   0        0        0   148847 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/index-nse.ipynb
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/index.ipynb
+-rw-r--r--   0        0        0    13821 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/scratchpad.ipynb
+-rw-r--r--   0        0        0   122869 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/derivatives/expiry-analysis.ipynb
+-rw-r--r--   0        0        0    78498 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/notebooks/derivatives/rsi-trade-analysis.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/calculations/__init__.py
+-rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/calculations/base.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/calculations/derivatives.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/calculations/equity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/core/__init__.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/core/column_definition.py
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/core/core.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/core/environment.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/core/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/dataprocess/__init__.py
+-rw-r--r--   0        0        0    15825 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/dataprocess/data_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/datareader/__init__.py
+-rw-r--r--   0        0        0    33230 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/datareader/data_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/trade_builders/__init__.py
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/trade_builders/derivatives.py
+-rw-r--r--   0        0        0     6899 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/src/markets_insights/trade_builders/results.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/tests/helper.py
+-rw-r--r--   0        0        0    24098 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/tests/test_calculations.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/tests/test_dataprocess.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/tests/test_dataprocess_caching.py
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/tests/test_datareader.py
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/tests/test_datareader_has_data.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/.gitignore
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/LICENSE.MD
+-rw-r--r--   0        0        0    18085 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/README.md
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/pyproject.toml
+-rw-r--r--   0        0        0    18253 2020-02-02 00:00:00.000000 markets_insights-0.4.8.post2/PKG-INFO
```

### Comparing `markets_insights-0.4.8/.github/workflows/python-publish.yml` & `markets_insights-0.4.8.post2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/examples/arithmatic.py` & `markets_insights-0.4.8.post2/examples/arithmatic.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/examples/extending-datareader.py` & `markets_insights-0.4.8.post2/examples/extending-datareader.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/examples/rsi-calculation.py` & `markets_insights-0.4.8.post2/examples/rsi-calculation.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/examples/test.py` & `markets_insights-0.4.8.post2/examples/test.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/indices.csv` & `markets_insights-0.4.8.post2/manual_data/indices.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY 100_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 100_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY 200_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 200_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY 50 ARBITRAGE_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 50 ARBITRAGE_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY 50 FUTURES PR_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 50 FUTURES PR_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY 500_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 500_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY 50_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY 50_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY AUTO_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY AUTO_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY BANK_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY BANK_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY ENERGY_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY ENERGY_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY FMCG_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY FMCG_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY HEALTHCARE_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY HEALTHCARE_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY IT_Data(1).csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY IT_Data(1).csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY IT_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY IT_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY MEDIA_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MEDIA_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY METAL_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY METAL_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY MICROCAP 250_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MICROCAP 250_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 100_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 100_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 150_Data(1).csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 150_Data(1).csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 150_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 150_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY MIDCAP 50_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY MIDCAP 50_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY NEXT 50_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY NEXT 50_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY OIL & GAS_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY OIL & GAS_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY PHARMA_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PHARMA_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY PRIVATE BANK_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PRIVATE BANK_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY PSE_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PSE_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY PSU BANK_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY PSU BANK_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY REALTY_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY REALTY_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY SMALLCAP 100_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY SMALLCAP 100_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY SMALLCAP 250_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY SMALLCAP 250_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY SMALLCAP 50_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY SMALLCAP 50_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY TOTAL MARKET_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY TOTAL MARKET_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/manual_data/Indices/NIFTY50 DIVIDEND POINTS_Data.csv` & `markets_insights-0.4.8.post2/manual_data/Indices/NIFTY50 DIVIDEND POINTS_Data.csv`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/caching.ipynb` & `markets_insights-0.4.8.post2/notebooks/caching.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/core.ipynb` & `markets_insights-0.4.8.post2/notebooks/core.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/equity.ipynb` & `markets_insights-0.4.8.post2/notebooks/equity.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/examples.ipynb` & `markets_insights-0.4.8.post2/notebooks/examples.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/index-nse.ipynb` & `markets_insights-0.4.8.post2/notebooks/index-nse.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/index.ipynb` & `markets_insights-0.4.8.post2/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/scratchpad.ipynb` & `markets_insights-0.4.8.post2/notebooks/scratchpad.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/derivatives/expiry-analysis.ipynb` & `markets_insights-0.4.8.post2/notebooks/derivatives/expiry-analysis.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/notebooks/derivatives/rsi-trade-analysis.ipynb` & `markets_insights-0.4.8.post2/notebooks/derivatives/rsi-trade-analysis.ipynb`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/calculations/base.py` & `markets_insights-0.4.8.post2/src/markets_insights/calculations/base.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/calculations/derivatives.py` & `markets_insights-0.4.8.post2/src/markets_insights/calculations/derivatives.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/calculations/equity.py` & `markets_insights-0.4.8.post2/src/markets_insights/calculations/equity.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/core/column_definition.py` & `markets_insights-0.4.8.post2/src/markets_insights/core/column_definition.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/core/core.py` & `markets_insights-0.4.8.post2/src/markets_insights/core/core.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/core/environment.py` & `markets_insights-0.4.8.post2/src/markets_insights/core/environment.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/core/settings.py` & `markets_insights-0.4.8.post2/src/markets_insights/core/settings.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/dataprocess/data_processor.py` & `markets_insights-0.4.8.post2/src/markets_insights/dataprocess/data_processor.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/datareader/data_reader.py` & `markets_insights-0.4.8.post2/src/markets_insights/datareader/data_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
             **({**EnvironmentSettings.Paths, **filenames})
         )
         primary_data_file_path = self.options.primary_data_path_template.substitute(
             **({**EnvironmentSettings.Paths, **filenames})
         )
 
         if not os.path.exists(output_file_path):
-            Instrumentation.debug(f"Downloading data for {for_date}")
+            Instrumentation.debug(f"Downloading data for {for_date.strftime('%Y, %m, %d')}")
             url = self.options.url_template.substitute(**({**date_parts, **filenames}))
 
             Instrumentation.debug(url)
 
             urldata = urlopen(url, timeout=self.options.download_timeout)
             with open(output_file_path, "wb") as output:
                 output.write(urldata.read())
```

### Comparing `markets_insights-0.4.8/src/markets_insights/trade_builders/derivatives.py` & `markets_insights-0.4.8.post2/src/markets_insights/trade_builders/derivatives.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/src/markets_insights/trade_builders/results.py` & `markets_insights-0.4.8.post2/src/markets_insights/trade_builders/results.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/tests/helper.py` & `markets_insights-0.4.8.post2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/tests/test_calculations.py` & `markets_insights-0.4.8.post2/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/tests/test_dataprocess.py` & `markets_insights-0.4.8.post2/tests/test_dataprocess.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/tests/test_dataprocess_caching.py` & `markets_insights-0.4.8.post2/tests/test_dataprocess_caching.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/tests/test_datareader.py` & `markets_insights-0.4.8.post2/tests/test_datareader.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/tests/test_datareader_has_data.py` & `markets_insights-0.4.8.post2/tests/test_datareader_has_data.py`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/README.md` & `markets_insights-0.4.8.post2/README.md`

 * *Files identical despite different names*

### Comparing `markets_insights-0.4.8/pyproject.toml` & `markets_insights-0.4.8.post2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "markets_insights"
-version = "0.4.8"
+version = "0.4.8-2"
 authors = [
   { name="Naresh Rohra", email="naresh.rohra@hotmail.com" },
 ]
 description = "This package retrieves and handles financial market data from the National Stock Exchange (NSE) in India."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `markets_insights-0.4.8/PKG-INFO` & `markets_insights-0.4.8.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: markets_insights
-Version: 0.4.8
+Version: 0.4.8.post2
 Summary: This package retrieves and handles financial market data from the National Stock Exchange (NSE) in India.
 Project-URL: Homepage, https://github.com/nareshrohra/markets_insights/
 Project-URL: Issues, https://github.com/nareshrohra/markets_insights/issues
 Author-email: Naresh Rohra <naresh.rohra@hotmail.com>
 License-File: LICENSE.MD
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

