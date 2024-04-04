# Comparing `tmp/zerohertzLib-1.0.2.tar.gz` & `tmp/zerohertzLib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.2.tar", last modified: Wed Apr  3 17:13:59 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.3.tar", last modified: Thu Apr  4 12:29:28 2024, max compression
```

## Comparing `zerohertzLib-1.0.2.tar` & `zerohertzLib-1.0.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-03 17:13:53.000000 zerohertzLib-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-03 17:13:53.000000 zerohertzLib-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-03 17:13:53.000000 zerohertzLib-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     8841 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16557 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.556707 zerohertzLib-1.0.2/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    41316 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6964 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22648 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17510 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-04 12:29:22.000000 zerohertzLib-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 12:29:22.000000 zerohertzLib-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-04 12:29:22.000000 zerohertzLib-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.461173 zerohertzLib-1.0.3/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    41316 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.465173 zerohertzLib-1.0.3/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22648 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17510 2024-04-04 12:29:23.000000 zerohertzLib-1.0.3/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:29:28.457173 zerohertzLib-1.0.3/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 12:29:28.000000 zerohertzLib-1.0.3/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.2/LICENSE` & `zerohertzLib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/PKG-INFO` & `zerohertzLib-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.2 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.3 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.2/README.md` & `zerohertzLib-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/setup.py` & `zerohertzLib-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_algorithm.py` & `zerohertzLib-1.0.3/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_api.py` & `zerohertzLib-1.0.3/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_logging.py` & `zerohertzLib-1.0.3/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_plot.py` & `zerohertzLib-1.0.3/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_quant.py` & `zerohertzLib-1.0.3/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_util.py` & `zerohertzLib-1.0.3/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/test/test_vision.py` & `zerohertzLib-1.0.3/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/__init__.py` & `zerohertzLib-1.0.3/zerohertzLib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.2"
+__version__ = "v1.0.3"
```

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.3/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.3/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/api/github.py` & `zerohertzLib-1.0.3/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.3/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.3/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.3/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.3/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.3/zerohertzLib/logging/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,67 +21,75 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import logging
 from typing import Optional
 
+from rich.console import Console
 from rich.logging import RichHandler
 
 from .handler import DiscordHandler, SlackBotHandler, SlackWebhookHandler
 
 
 class Logger(logging.Logger):
     """이쁘게 log를 찍어보는 class
 
     Note:
         더 예뻐지고 싶습니다...
 
     Args:
         logger_name (``Optional[str]``): Logger의 이름
+        width (``Optional[int]``): Logger의 너비
+        show_path (``Optional[bool]``): Logger의 호출 경로 표시 여부
         file_name(``Optional[str]``): ``.log`` file의 이름 (미입력 시 미출력)
         discord (``Optional[str]``): Discord Webhook의 URL (``logger_level`` 적용)
         slack (``Optional[str]``): Slack Webhook의 URL 혹은 Bot의 token (``logger_level`` 적용)
         channel (``Optional[str]``): Slack Webhook 또는 Bot이 전송할 channel
         logger_level (``Optional[int]``): ``logging.Logger`` 의 level
         console_level (``Optional[int]``): ``rich.logging.RichHandler`` 의 level
         file_level (``Optional[int]``): ``logging.FileHandler`` 의 level
 
     Examples:
         >>> logger = zz.logging.Logger("TEST_1")
         >>> logger.debug("debug")
-        [03/13/24 15:09:45] DEBUG    [TEST_1] debug      <stdin>:1
+        [03/13/24 00:00:00] DEBUG    [TEST_1] debug                                  <stdin>:1
         >>> logger.info("info")
-        [03/13/24 15:09:49] INFO     [TEST_1] info       <stdin>:1
+        [03/13/24 00:00:00] INFO     [TEST_1] info                                   <stdin>:1
         >>> logger.warning("warning")
-        [03/13/24 15:09:53] WARNING  [TEST_1] warning    <stdin>:1
+        [03/13/24 00:00:00] WARNING  [TEST_1] warning                                <stdin>:1
         >>> logger.error("error")
-        [03/13/24 15:09:56] ERROR    [TEST_1] error      <stdin>:1
+        [03/13/24 00:00:00] ERROR    [TEST_1] error                                  <stdin>:1
         >>> logger.critical("critical")
-        [03/13/24 15:09:59] CRITICAL [TEST_1] critical   <stdin>:1
+        [03/13/24 00:00:00] CRITICAL [TEST_1] critical                               <stdin>:1
     """
 
     def __init__(
         self,
         logger_name: Optional[str] = None,
+        width: Optional[int] = None,
+        show_path: Optional[bool] = True,
         file_name: Optional[str] = None,
         discord: Optional[str] = None,
         slack: Optional[str] = None,
         channel: Optional[str] = None,
         logger_level: Optional[int] = logging.NOTSET,
         console_level: Optional[int] = logging.NOTSET,
         file_level: Optional[int] = logging.NOTSET,
     ) -> None:
         super().__init__(logger_name, logger_level)
         default_formatter = logging.Formatter(
             "%(asctime)s | %(levelname)-8s | %(name)s | %(message)s"
         )
         rich_formatter = logging.Formatter("[%(name)s] %(message)s")
         console_handler = RichHandler(
-            keywords=[f"[{logger_name}]"], rich_tracebacks=True
+            console=Console(width=width),
+            show_path=show_path,
+            rich_tracebacks=True,
+            keywords=[f"[{logger_name}]"],
         )
         console_handler.setLevel(console_level)
         console_handler.setFormatter(rich_formatter)
         self.addHandler(console_handler)
         if file_name is not None:
             file_handler = logging.FileHandler(f"{file_name}.log")
             file_handler.setLevel(file_level)
```

### Comparing `zerohertzLib-1.0.2/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.3/zerohertzLib/mlops/triton.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,17 @@
         port (``Optional[int]``): triton inference server의 gRPC 통신 port 번호
 
     Methods:
         __call__:
             Model 호출 수행
 
             Args:
-                model (``Union[int, str]``): 호출할 model의 이름
+                model (``Union[int, str]``): 호출할 model의 이름 및 ID
                 *args (``NDArray[DTypeLike]``): Model 호출 시 사용될 입력
+                renew: (``Optional[bool]``): 각 모델의 상태 조회 시 갱신 여부
 
             Returns:
                 ``Dict[str, NDArray[DTypeLike]]``: 호출된 model의 결과
 
     Examples:
         >>> tc = zz.mlops.TritonClientURL("localhost")
         >>> tc("YOLO", np.zeros((1, 3, 640, 640)))
@@ -75,24 +76,27 @@
         self.models = []
         for model in self.get_model_repository_index(as_json=True)["models"]:
             self.models.append(model["name"])
         self.logger = Logger("TritonClient", logger_level=20)
         self.emoji = {
             "LOADING": "🚀",
             "READY": "✅",
-            "UNLOADING": "🛠️",
+            "UNLOADING": "🛌",
             "UNAVAILABLE": "💤",
         }
 
     def __call__(
-        self, model: Union[int, str], *args: NDArray[DTypeLike]
+        self,
+        model: Union[int, str],
+        *args: NDArray[DTypeLike],
+        renew: Optional[bool] = False,
     ) -> Dict[str, NDArray[DTypeLike]]:
         if isinstance(model, int):
             model = self.models[model]
-        self._update_configs(model)
+        self._update_configs(model, renew)
         inputs = self.configs[model]["config"]["input"]
         outputs = self.configs[model]["config"]["output"]
         assert len(inputs) == len(args)
         triton_inputs = []
         for input_info, arg in zip(inputs, args):
             triton_inputs.append(self._set_input(input_info, arg))
         triton_outputs = []
@@ -103,16 +107,16 @@
         )
         response.get_response()
         triton_results = {}
         for output in outputs:
             triton_results[output["name"]] = response.as_numpy(output["name"])
         return triton_results
 
-    def _update_configs(self, model: str) -> None:
-        if model not in self.configs:
+    def _update_configs(self, model: str, renew: bool) -> None:
+        if renew or model not in self.configs:
             self.configs[model] = self.get_model_config(model, as_json=True)
 
     def _set_input(
         self, input_info: Dict[str, List[int]], value: NDArray[DTypeLike]
     ) -> grpcclient._infer_input.InferInput:
         if "dims" in input_info.keys() and len(input_info["dims"]) != len(value.shape):
             self.logger.warning(
@@ -125,26 +129,30 @@
         return grpcclient.InferInput(
             input_info["name"],
             value.shape,
             input_info["data_type"][5:],
         ).set_data_from_numpy(value)
 
     def status(
-        self, sortby: Optional[str] = "STATE", reverse: Optional[bool] = False
+        self,
+        renew: Optional[bool] = False,
+        sortby: Optional[str] = "STATE",
+        reverse: Optional[bool] = False,
     ) -> None:
         """Triton Inferece Server의 상태를 확인하는 함수
 
         Args:
+            renew: (``Optional[bool]``): 각 모델의 상태 조회 시 갱신 여부
             sortby (``Optional[str]``): 정렬 기준
             reverse (``Optional[bool]``): 정렬 역순 여부
 
         Examples:
             >>> tc.status()
 
-            .. image:: _static/examples/static/mlops.TritonClientURL.status.png
+            .. image:: _static/examples/static/mlops.TritonClientURL.status.gif
                 :align: center
                 :width: 700px
         """
         table = PrettyTable(
             ["STATE", "ID", "MODEL", "VERSION", "BACKEND", "INPUT", "OUTPUT"],
             title=f"Triton Inference Server Status [{self.url}]",
         )
@@ -152,15 +160,15 @@
             if model["name"] not in self.models:
                 self.models.append(model["name"])
             state = model.get("state", "UNAVAILABLE")
             if state in ["LOADING", "UNAVAILABLE"]:
                 _input, _output = ["-"], ["-"]
                 backend = "-"
             else:
-                self._update_configs(model["name"])
+                self._update_configs(model["name"], renew)
                 _input, _output = [], []
                 for inputs in self.configs[model["name"]]["config"]["input"]:
                     _input.append(
                         f"""{inputs["name"]} [{inputs["data_type"][5:]}: ({", ".join(inputs["dims"])})]"""
                     )
                 for outputs in self.configs[model["name"]]["config"]["output"]:
                     _output.append(
@@ -190,15 +198,15 @@
         config: Optional[str] = None,
         files: Optional[Dict] = None,
         client_timeout: Optional[float] = None,
     ) -> None:
         """Triton Inference Server 내 model을 load하는 함수
 
         Args:
-            model_name (``Union[int, str]``): Unload할 model의 이름 및 ID
+            model_name (``Union[int, str]``): Load할 model의 이름 또는 ID
             headers (``Optional[Dict]``): Request 전송 시 포함할 추가 HTTP header
             config (``Optional[str]``): Model load 시 사용될 config
             config (``Optional[Dict]``): Model load 시 override model directory에서 사용할 file
             client_timeout (``Optional[float]``): 초 단위의 timeout
 
         Examples:
             >>> tc.load_model(0)
@@ -214,15 +222,15 @@
         headers: Optional[Dict] = None,
         unload_dependents: Optional[bool] = False,
         client_timeout: Optional[float] = None,
     ) -> None:
         """Triton Inference Server 내 model을 unload하는 함수
 
         Args:
-            model_name (``Union[int, str]``): Unload할 model의 이름 및 ID
+            model_name (``Union[int, str]``): Unload할 model의 이름 또는 ID
             headers (``Optional[Dict]``): Request 전송 시 포함할 추가 HTTP header
             unload_dependents (``Optional[bool]``): Model unload 시 dependents의 unload 여부
             client_timeout (``Optional[float]``): 초 단위의 timeout
 
         Examples:
             >>> tc.unload_model(0)
             >>> tc.unload_model("MODEL_NAME")
@@ -241,16 +249,17 @@
         port (``Optional[int]``): triton inference server의 gRPC 통신 port 번호
 
     Methods:
         __call__:
             Model 호출 수행
 
             Args:
-                model (``Union[int, str]``): 호출할 model의 이름
+                model (``Union[int, str]``): 호출할 model의 이름 또는 ID
                 *args (``NDArray[DTypeLike]``): Model 호출 시 사용될 입력
+                renew: (``Optional[bool]``): 각 모델의 상태 조회 시 갱신 여부
 
             Returns:
                 ``Dict[str, NDArray[DTypeLike]]``: 호출된 model의 결과
 
     Examples:
         Kubernetes:
             >>> kubectl get svc -n yolo
@@ -274,14 +283,30 @@
 
 class BaseTritonPythonModel(ABC):
     """Triton Inference Server에서 Python backend 사용을 위한 class
 
     Note:
         Abstract Base Class: Model의 추론을 수행하는 abstract method ``_inference`` 정의 후 사용
 
+    Hint:
+        Logger의 색상 적용을 위해 아래와 같은 환경 변수 정의 필요
+
+        .. code-block:: yaml
+
+            spec:
+              template:
+                spec:
+                  containers:
+                    - name: ${NAME}
+                      ...
+                      env:
+                        - name: "FORCE_COLOR"
+                        value: "1"
+                      ...
+
     Attributes:
         logger (``zerohertzLib.logging.Logger``): Triton Inference Server 내 log를 출력하기 위한 instance
 
     Methods:
         _inference:
             Model 추론을 수행하는 private method (상속을 통한 재정의 필수)
 
@@ -300,47 +325,53 @@
                         super().initialize(args, 10)
                         self.model = Model(cfg)
 
                     def _inference(self, input_image):
                         return self.model(input_image)
 
         Normal Logs:
-            .. code-block:: python
+            .. code-block:: apl
 
-                2024-01-12 01:47:19,123 | INFO     | MODEL | Called
-                2024-01-12 01:47:19,124 | DEBUG    | MODEL | inputs: (2259, 1663, 3)
-                2024-01-12 01:47:19,124 | INFO     | MODEL | Inference start
-                2024-01-12 01:47:19,254 | DEBUG    | MODEL | outputs: (3, 4, 2) (3,)
-                2024-01-12 01:47:19,254 | INFO     | MODEL | Inference completed
+                [04/04/24 00:00:00] INFO     [MODEL] Initialize                        triton.py:*
+                [04/04/24 00:00:00] INFO     [MODEL] Called                            triton.py:*
+                                    DEBUG    [MODEL] inputs: (3, 3, 3)                 triton.py:*
+                                    INFO     [MODEL] Inference start                   triton.py:*
+                                    DEBUG    [MODEL] outputs: (10,) (20,)              triton.py:*
+                                    INFO     [MODEL] Inference completed               triton.py:*
 
         Error Logs:
-            .. code-block:: python
+            .. code-block:: apl
 
-                2024-01-12 02:03:24,288 | CRITICAL | MODEL | name 'test' is not defined
-                ====================================================================================================
-                Traceback (most recent call last):
-                File "/usr/local/lib/python3.8/dist-packages/zerohertzLib/mlops/triton.py", line *, in execute
-                    outputs = self._inference(*inputs)
-                File "/models/model/*/model.py", line *, in _inference
-                    return self.model(input_image)
-                File "/models/model/*/*.py", line *, in *
-                    test
-                NameError: name 'test' is not defined
-                ====================================================================================================
+                [04/04/24 00:00:00] INFO     [MODEL] Called                            triton.py:*
+                                    INFO     [MODEL] Inference start                   triton.py:*
+                                    CRITICAL [MODEL] Hello, World!                     triton.py:*
+                                            ====================================================================================================
+                                            Traceback (most recent call last):
+                                            File "/usr/local/lib/python3.8/dist-packages/zerohertzLib/mlops/triton.py", line *, in execute
+                                                outputs = self._inference(*inputs)
+                                            File "/models/model/*/model.py", line *, in _inference
+                                                raise Exception("Hello, World!")
+                                            Exception: Hello, World!
+                                            ====================================================================================================
     """
 
     def initialize(self, args: Dict[str, Any], level: Optional[int] = 20) -> None:
         """Triton Inference Server 시작 시 수행되는 method
 
         Args:
             args (``Dict[str, Any]``): ``config.pbtxt`` 에 포함된 model의 정보
             level (``Optional[int]``): Logger의 level
         """
         self.cfg = json.loads(args["model_config"])
-        self.logger = Logger(self.cfg["name"].upper(), level)
+        self.logger = Logger(
+            self.cfg["name"].upper(),
+            170,
+            file_name=self.cfg["name"],
+            logger_level=level,
+        )
         self.logger.info("Initialize")
 
     def execute(self, requests: List[Any]) -> List[Any]:
         """Triton Inference Server 호출 시 수행되는 method
 
         Args:
             requests (``List[pb_utils.InferenceRequest]``): Client에서 전송된 model inputs
@@ -354,28 +385,29 @@
                 self.logger.info("Called")
                 inputs = self._get_inputs(request)
                 self.logger.debug(
                     "inputs: %s", " ".join([str(input_.shape) for input_ in inputs])
                 )
                 self.logger.info("Inference start")
                 outputs = self._inference(*inputs)
+                if not isinstance(outputs, tuple):
+                    outputs = tuple([outputs])
                 self.logger.debug(
                     "outputs: %s", " ".join([str(output.shape) for output in outputs])
                 )
                 self.logger.info("Inference completed")
                 response = self._set_outputs(outputs)
                 responses.append(response)
             except Exception as error:
                 message = (
                     str(error)
                     + "\n"
                     + "=" * 100
                     + "\n"
                     + str(traceback.format_exc())
-                    + "\n"
                     + "=" * 100
                 )
                 self.logger.critical(message)
                 responses.append(
                     pb_utils.InferenceResponse(
                         output_tensors=[], error=pb_utils.TritonError(message)
                     )
@@ -386,20 +418,16 @@
         inputs = []
         for input_ in self.cfg["input"]:
             inputs.append(
                 pb_utils.get_input_tensor_by_name(request, input_["name"]).as_numpy()
             )
         return inputs
 
-    def _set_outputs(
-        self, outputs: Union[NDArray[DTypeLike], Tuple[NDArray[DTypeLike]]]
-    ) -> Any:
+    def _set_outputs(self, outputs: Tuple[NDArray[DTypeLike]]) -> Any:
         output_tensors = []
-        if not isinstance(outputs, tuple):
-            outputs = [outputs]
         for output, value in zip(self.cfg["output"], outputs):
             output_tensors.append(
                 pb_utils.Tensor(
                     output["name"],
                     value.astype(pb_utils.triton_string_to_numpy(output["data_type"])),
                 )
             )
```

### Comparing `zerohertzLib-1.0.2/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.3/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.3/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.3/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.3/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.3/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.3/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.3/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.3/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.3/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.3/zerohertzLib/quant/quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.3/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.3/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/util/data.py` & `zerohertzLib-1.0.3/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/util/json.py` & `zerohertzLib-1.0.3/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.3/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.2/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.3/zerohertzLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.2 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.3 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.2/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.3/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

