# Comparing `tmp/cylc-flow-8.2.4.tar.gz` & `tmp/cylc-flow-8.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-flow-8.2.4.tar", last modified: Thu Jan 11 15:35:08 2024, max compression
+gzip compressed data, was "cylc-flow-8.2.5.tar", last modified: Thu Apr  4 14:40:36 2024, max compression
```

## Comparing `cylc-flow-8.2.4.tar` & `cylc-flow-8.2.5.tar`

### file list

```diff
@@ -1,320 +1,320 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.932190 cylc-flow-8.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-01-11 15:35:08.932190 cylc-flow-8.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.872189 cylc-flow-8.2.4/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.892189 cylc-flow-8.2.4/cylc/flow/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/async_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/broadcast_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/broadcast_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/c3mro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.896190 cylc-flow-8.2.4/cylc/flow/cfgspec/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cfgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cfgspec/glbl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    73203 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cfgspec/globalcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    85291 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cfgspec/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/command_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)    99371 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/context_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.896190 cylc-flow-8.2.4/cylc/flow/cycling/
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cycling/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cycling/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cycling/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cycling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/cylc_subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/data_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   103056 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/data_store_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/dbstatecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.896190 cylc-flow-8.2.4/cylc/flow/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/cylc
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/cylc-completion.bash
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/job.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.896190 cylc-flow-8.2.4/cylc/flow/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc-mode.el
--rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc.lang
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc.vim
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.896190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.896190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4248 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7216 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6453 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3721 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.876189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4248 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7216 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6453 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3721 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.876189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/forecast-script/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.876189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/message-trigger-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.900189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/retries-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/retries-tutorial/.validate
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4248 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9151 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7216 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6453 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3721 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.876189 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35829 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/flow_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    35677 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/graphnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/host_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/hostuserutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/id.py
--rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/id_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.904190 cylc-flow-8.2.4/cylc/flow/install_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/install_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/install_plugins/log_vc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.876189 cylc-flow-8.2.4/cylc/flow/jinja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.908190 cylc-flow-8.2.4/cylc/flow/jinja/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/jinja/filters/duration_as.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/jinja/filters/pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/jinja/filters/strftime.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.908190 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/at.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/background.py
--rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/loadleveler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_handlers/slurm_packjob.py
--rw-r--r--   0 runner    (1001) docker     (127)    33926 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/job_runner_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/listify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/log_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/loggingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.908190 cylc-flow-8.2.4/cylc/flow/main_loop/
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/log_data_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/log_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/log_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/log_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/main_loop/reset_bad_hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.912190 cylc-flow-8.2.4/cylc/flow/network/
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/replier.py
--rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    80335 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/ssh_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/network/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)    30925 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/option_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/param_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.912190 cylc-flow-8.2.4/cylc/flow/parsec/
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/empysupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/fileparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/include.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/jinja2support.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    42818 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/parsec/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17207 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/pathutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/pipe_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/prerequisite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/print_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    40419 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/rundb.py
--rw-r--r--   0 runner    (1001) docker     (127)    87059 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scheduler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.920190 cylc-flow-8.2.4/cylc/flow/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15346 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/broadcast.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21078 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/cat_log.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4986 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/check_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/completion_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8932 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/cycle_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/cylc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5986 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8083 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/dump.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4460 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/ext_trigger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1491 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/function_run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/get_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1871 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/get_workflow_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2311 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/get_workflow_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4438 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10942 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/install.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/jobs_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/jobs_poll.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/jobs_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2503 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40990 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/lint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6417 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/pause.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/play.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/reinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3266 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/reload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/remote_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/remote_tidy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13206 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/report_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3516 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/set_outputs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/set_verbosity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13108 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/show.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8380 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3658 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/subscribe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5272 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/tui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6436 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/validate_install_play.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/validate_reinstall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/view.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10264 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/scripts/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/subprocctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/subprocpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_action_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    65662 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_events_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55839 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_job_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80634 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_qualifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.924190 cylc-flow-8.2.4/cylc/flow/task_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_queues/independent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_remote_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    25369 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_remote_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_state_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/task_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/taskdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/templatevars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.924190 cylc-flow-8.2.4/cylc/flow/tui/
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/tui/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/tui/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/tui/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/unicode_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/wallclock.py
--rw-r--r--   0 runner    (1001) docker     (127)    32437 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/workflow_db_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/workflow_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    34081 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/workflow_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/workflow_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/xtrigger_mgr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.924190 cylc-flow-8.2.4/cylc/flow/xtriggers/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/xtriggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/xtriggers/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/xtriggers/wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/xtriggers/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/cylc/flow/xtriggers/xrandom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 15:35:08.924190 cylc-flow-8.2.4/cylc_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-01-11 15:35:08.000000 cylc-flow-8.2.4/cylc_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-01-11 15:35:08.000000 cylc-flow-8.2.4/cylc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 15:35:08.000000 cylc-flow-8.2.4/cylc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-01-11 15:35:08.000000 cylc-flow-8.2.4/cylc_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-01-11 15:35:08.000000 cylc-flow-8.2.4/cylc_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-11 15:35:08.000000 cylc-flow-8.2.4/cylc_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-01-11 15:35:08.932190 cylc-flow-8.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-11 15:35:05.000000 cylc-flow-8.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.799552 cylc-flow-8.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-04 14:40:36.799552 cylc-flow-8.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.755551 cylc-flow-8.2.5/cylc/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/async_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/broadcast_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/broadcast_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/c3mro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.755551 cylc-flow-8.2.5/cylc/flow/cfgspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/glbl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73203 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/globalcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85291 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/command_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99069 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/context_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/cycling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cylc_subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/data_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103056 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/data_store_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/dbstatecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/cylc
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/cylc-completion.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/job.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc-mode.el
+-rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.lang
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.vim
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/message-trigger-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/.validate
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.739550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35829 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/flow_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36301 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/graphnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/hostuserutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/id_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/install_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/install_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/install_plugins/log_vc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.739550 cylc-flow-8.2.5/cylc/flow/jinja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.771551 cylc-flow-8.2.5/cylc/flow/jinja/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/jinja/filters/duration_as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/jinja/filters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/jinja/filters/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.771551 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/loadleveler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm_packjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33926 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/listify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/log_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/loggingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.771551 cylc-flow-8.2.5/cylc/flow/main_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/reset_bad_hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.775551 cylc-flow-8.2.5/cylc/flow/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/replier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80335 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/ssh_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30974 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/option_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/param_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.779551 cylc-flow-8.2.5/cylc/flow/parsec/
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/empysupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/fileparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/jinja2support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43559 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/pathutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/pipe_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/prerequisite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/print_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39982 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86592 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20823 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scheduler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.787551 cylc-flow-8.2.5/cylc/flow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15378 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/broadcast.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21078 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/cat_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4986 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/check_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/completion_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8932 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/cycle_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/cylc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5986 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8083 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4460 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/ext_trigger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1491 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/function_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/get_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1871 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2311 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4638 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10942 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/jobs_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/jobs_poll.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/jobs_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2503 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40990 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/lint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6417 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/pause.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/play.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/reinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3266 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/remote_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/remote_tidy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13206 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/report_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3516 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/set_outputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/set_verbosity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13108 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/show.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8380 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3658 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/subscribe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5272 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/tui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6488 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/validate_install_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/validate_reinstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/view.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10163 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/subprocctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/subprocpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_action_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_events_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55839 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_job_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80634 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_qualifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.787551 cylc-flow-8.2.5/cylc/flow/task_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_queues/independent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_remote_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_remote_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_state_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/taskdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/templatevars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.787551 cylc-flow-8.2.5/cylc/flow/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/unicode_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/wallclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_db_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34487 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtrigger_mgr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.791552 cylc-flow-8.2.5/cylc/flow/xtriggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/xrandom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.791552 cylc-flow-8.2.5/cylc_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-04 14:40:36.799552 cylc-flow-8.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/setup.py
```

### Comparing `cylc-flow-8.2.4/COPYING` & `cylc-flow-8.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/PKG-INFO` & `cylc-flow-8.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.2.4
+Version: 8.2.5
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
@@ -36,15 +36,15 @@
 Requires-Dist: jinja2==3.0.*
 Requires-Dist: metomi-isodatetime<1!3.2.0,>=1!3.0.0
 Requires-Dist: protobuf<4.22.0,>=4.21.2
 Requires-Dist: psutil>=5.6.0
 Requires-Dist: pyzmq>=22
 Requires-Dist: setuptools!=67.*,>=49
 Requires-Dist: importlib_metadata; python_version < "3.8"
-Requires-Dist: urwid==2.*
+Requires-Dist: urwid!=2.6.2,!=2.6.3,==2.*
 Requires-Dist: rx
 Requires-Dist: promise
 Requires-Dist: tomli>=2; python_version < "3.11"
 Provides-Extra: empy
 Requires-Dist: EmPy==3.3.*; extra == "empy"
 Provides-Extra: graph
 Requires-Dist: pillow; extra == "graph"
@@ -69,15 +69,15 @@
 Requires-Dist: flake8-bugbear>=21.0.0; extra == "tests"
 Requires-Dist: flake8-builtins>=1.5.0; extra == "tests"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "tests"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "tests"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "tests"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "tests"
 Requires-Dist: flake8>=3.0.0; extra == "tests"
-Requires-Dist: mypy>=0.910; extra == "tests"
+Requires-Dist: mypy<1.9,>=0.910; extra == "tests"
 Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "tests"
 Requires-Dist: pytest-cov>=2.8.0; extra == "tests"
 Requires-Dist: pytest-xdist>=2; extra == "tests"
 Requires-Dist: pytest-env>=0.6.2; extra == "tests"
 Requires-Dist: pytest-mock>=3.7; extra == "tests"
 Requires-Dist: pytest>=6; extra == "tests"
 Requires-Dist: testfixtures>=6.11.0; extra == "tests"
@@ -108,15 +108,15 @@
 Requires-Dist: flake8-bugbear>=21.0.0; extra == "all"
 Requires-Dist: flake8-builtins>=1.5.0; extra == "all"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "all"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "all"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "all"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "all"
 Requires-Dist: flake8>=3.0.0; extra == "all"
-Requires-Dist: mypy>=0.910; extra == "all"
+Requires-Dist: mypy<1.9,>=0.910; extra == "all"
 Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "all"
 Requires-Dist: pytest-cov>=2.8.0; extra == "all"
 Requires-Dist: pytest-xdist>=2; extra == "all"
 Requires-Dist: pytest-env>=0.6.2; extra == "all"
 Requires-Dist: pytest-mock>=3.7; extra == "all"
 Requires-Dist: pytest>=6; extra == "all"
 Requires-Dist: testfixtures>=6.11.0; extra == "all"
```

### Comparing `cylc-flow-8.2.4/README.md` & `cylc-flow-8.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/__init__.py` & `cylc-flow-8.2.5/cylc/flow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # running pre-5.0 cylc via the posix nohup command; is it still the
     # case in post-5.0 daemon-mode cylc?)
     os.environ['PYTHONUNBUFFERED'] = 'true'
 
 
 environ_init()
 
-__version__ = '8.2.4'
+__version__ = '8.2.5'
 
 
 def iter_entry_points(entry_point_name):
     """Iterate over Cylc entry points."""
     import pkg_resources
     yield from (
         entry_point
```

### Comparing `cylc-flow-8.2.4/cylc/flow/async_util.py` & `cylc-flow-8.2.5/cylc/flow/async_util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/broadcast_mgr.py` & `cylc-flow-8.2.5/cylc/flow/broadcast_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/broadcast_report.py` & `cylc-flow-8.2.5/cylc/flow/broadcast_report.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/c3mro.py` & `cylc-flow-8.2.5/cylc/flow/c3mro.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cfgspec/__init__.py` & `cylc-flow-8.2.5/cylc/flow/cfgspec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cfgspec/glbl_cfg.py` & `cylc-flow-8.2.5/cylc/flow/cfgspec/glbl_cfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cfgspec/globalcfg.py` & `cylc-flow-8.2.5/cylc/flow/cfgspec/globalcfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cfgspec/workflow.py` & `cylc-flow-8.2.5/cylc/flow/cfgspec/workflow.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/clean.py` & `cylc-flow-8.2.5/cylc/flow/clean.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/command_polling.py` & `cylc-flow-8.2.5/cylc/flow/command_polling.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/config.py` & `cylc-flow-8.2.5/cylc/flow/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 from cylc.flow.wallclock import (
     get_current_time_string, set_utc_mode, get_utc_mode)
 from cylc.flow.workflow_files import (
     NO_TITLE,
     WorkflowFiles,
     check_deprecation,
 )
+from cylc.flow.workflow_status import RunMode
 from cylc.flow.xtrigger_mgr import XtriggerManager
 
 if TYPE_CHECKING:
     from optparse import Values
     from cylc.flow.cycling import IntervalBase, PointBase, SequenceBase
 
 RE_CLOCK_OFFSET = re.compile(
@@ -516,15 +517,15 @@
 
         self.mem_log("config.py: before load_graph()")
         self.load_graph()
         self.mem_log("config.py: after load_graph()")
 
         self.process_runahead_limit()
 
-        if self.run_mode('simulation', 'dummy'):
+        if self.run_mode() in {'simulation', 'dummy'}:
             self.configure_sim_modes()
 
         self.configure_workflow_state_polling_tasks()
 
         self._check_task_event_handlers()
         self._check_special_tasks()  # adds to self.implicit_tasks
         self._check_explicit_cycling()
@@ -1543,28 +1544,17 @@
         os.environ['CYLC_WORKFLOW_FINAL_CYCLE_POINT'] = str(self.final_point)
         os.environ['CYLC_CYCLING_MODE'] = self.cfg['scheduling'][
             'cycling mode']
         # Add workflow bin directory to PATH for workflow and event handlers
         os.environ['PATH'] = os.pathsep.join([
             os.path.join(self.fdir, 'bin'), os.environ['PATH']])
 
-    def run_mode(self, *reqmodes):
-        """Return the run mode.
-
-        Combine command line option with configuration setting.
-        If "reqmodes" is specified, return the boolean (mode in reqmodes).
-        Otherwise, return the mode as a str.
-        """
-        mode = getattr(self.options, 'run_mode', None)
-        if not mode:
-            mode = 'live'
-        if reqmodes:
-            return mode in reqmodes
-        else:
-            return mode
+    def run_mode(self) -> str:
+        """Return the run mode."""
+        return RunMode.get(self.options)
 
     def _check_task_event_handlers(self):
         """Check custom event handler templates can be expanded.
 
         Ensures that any %(template_variables)s in task event handlers
         are present in the data that will be passed to them when called
         (otherwise they will fail).
```

### Comparing `cylc-flow-8.2.4/cylc/flow/context_node.py` & `cylc-flow-8.2.5/cylc/flow/context_node.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cycling/__init__.py` & `cylc-flow-8.2.5/cylc/flow/cycling/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cycling/integer.py` & `cylc-flow-8.2.5/cylc/flow/cycling/integer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cycling/iso8601.py` & `cylc-flow-8.2.5/cylc/flow/cycling/iso8601.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cycling/loader.py` & `cylc-flow-8.2.5/cylc/flow/cycling/loader.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cycling/util.py` & `cylc-flow-8.2.5/cylc/flow/cycling/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/cylc_subproc.py` & `cylc-flow-8.2.5/cylc/flow/cylc_subproc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/daemonize.py` & `cylc-flow-8.2.5/cylc/flow/daemonize.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/data_messages_pb2.py` & `cylc-flow-8.2.5/cylc/flow/data_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/data_store_mgr.py` & `cylc-flow-8.2.5/cylc/flow/data_store_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/dbstatecheck.py` & `cylc-flow-8.2.5/cylc/flow/dbstatecheck.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/cylc` & `cylc-flow-8.2.5/cylc/flow/etc/cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/cylc-completion.bash` & `cylc-flow-8.2.5/cylc/flow/etc/cylc-completion.bash`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/job.sh` & `cylc-flow-8.2.5/cylc/flow/etc/job.sh`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc-mode.el` & `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc-mode.el`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc.lang` & `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.lang`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc.vim` & `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.vim`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/syntax/cylc.xml` & `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.xml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/.validate` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files 2% similar despite different names*

```diff
@@ -111,8 +111,9 @@
 
     # Write wind data to csv.
     util.field_to_csv(wind_x, x_range, y_range, 'wind_x.csv')
     util.field_to_csv(wind_y, x_range, y_range, 'wind_y.csv')
 
 
 if __name__ == '__main__':
+    util.sleep()
     main()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 
     # Generate html page from forecast data.
     util.generate_html_map(map_file, map_template, forecasts, domain,
                            resolution)
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = [int(sys.argv[1]), int(sys.argv[2])]
     except IndexError:
         print(__doc__)
         sys.exit(1)
 
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from datetime import datetime
 import json
 import os
 import re
 
 import requests
 
+import util
+
 
 BASE_URL = ('http://datapoint.metoffice.gov.uk/public/data/'
             'val/wxobs/all/json/{site_id}'
             '?res=hourly&time={time}&key={api_key}')
 
 # Compass bearings for ordinate directions.
 # NOTE: We measure direction by where the winds have come from!
@@ -211,9 +213,10 @@
 
     # Write observations.
     with open('wind.csv', 'w+') as data_file:
         data_file.write(', '.join(obs))
 
 
 if __name__ == '__main__':
+    util.sleep()
     main(os.environ['SITE_ID'],
          os.environ.get('API_KEY'))
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files 1% similar despite different names*

```diff
@@ -191,8 +191,9 @@
         get_archived_radar_image('rainfall-radar.png', time)
 
     data = process_rainfall_data('rainfall-radar.png', resolution, domain)
     util.write_csv('rainfall.csv', data)
 
 
 if __name__ == '__main__':
+    util.sleep(2)  # make the tutorial run a little slower
     main()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files 2% similar despite different names*

```diff
@@ -97,13 +97,14 @@
     # Write out forecast summary.
     with open('summary.txt', 'w+') as summary_file:
         summary_file.write('The outlook at %s UTC for %s is "%s"' % (
             forecast_time.strftime('%Y-%m-%dT%H:%M'), site_name, message))
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = (sys.argv[1].lower(), int(sys.argv[2]))
     except IndexError:
         print(__doc__)
         sys.exit(1)
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
 from copy import copy
 from contextlib import suppress
 import math
-import jinja2
+import os
 import sys
+import time
 
+import jinja2
 
 R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
@@ -297,7 +299,16 @@
                 resolution=resolution,
                 lng1=domain['lng1'],
                 lng2=domain['lng2'],
                 lat1=domain['lat1'],
                 lat2=domain['lat2'],
                 data=data
             ))
+
+
+def sleep(secs=4):
+    """Make the tutorials run a little slower so users can follow along.
+
+    (Only if not running in CI).
+    """
+    if 'CI' not in os.environ:
+        time.sleep(secs)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations`

 * *Files 2% similar despite different names*

```diff
@@ -111,8 +111,9 @@
 
     # Write wind data to csv.
     util.field_to_csv(wind_x, x_range, y_range, 'wind_x.csv')
     util.field_to_csv(wind_y, x_range, y_range, 'wind_y.csv')
 
 
 if __name__ == '__main__':
+    util.sleep()
     main()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 
     # Generate html page from forecast data.
     util.generate_html_map(map_file, map_template, forecasts, domain,
                            resolution)
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = [int(sys.argv[1]), int(sys.argv[2])]
     except IndexError:
         print(__doc__)
         sys.exit(1)
 
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from datetime import datetime
 import json
 import os
 import re
 
 import requests
 
+import util
+
 
 BASE_URL = ('http://datapoint.metoffice.gov.uk/public/data/'
             'val/wxobs/all/json/{site_id}'
             '?res=hourly&time={time}&key={api_key}')
 
 # Compass bearings for ordinate directions.
 # NOTE: We measure direction by where the winds have come from!
@@ -211,9 +213,10 @@
 
     # Write observations.
     with open('wind.csv', 'w+') as data_file:
         data_file.write(', '.join(obs))
 
 
 if __name__ == '__main__':
+    util.sleep()
     main(os.environ['SITE_ID'],
          os.environ.get('API_KEY'))
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files 1% similar despite different names*

```diff
@@ -191,8 +191,9 @@
         get_archived_radar_image('rainfall-radar.png', time)
 
     data = process_rainfall_data('rainfall-radar.png', resolution, domain)
     util.write_csv('rainfall.csv', data)
 
 
 if __name__ == '__main__':
+    util.sleep(2)  # make the tutorial run a little slower
     main()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files 2% similar despite different names*

```diff
@@ -97,13 +97,14 @@
     # Write out forecast summary.
     with open('summary.txt', 'w+') as summary_file:
         summary_file.write('The outlook at %s UTC for %s is "%s"' % (
             forecast_time.strftime('%Y-%m-%dT%H:%M'), site_name, message))
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = (sys.argv[1].lower(), int(sys.argv[2]))
     except IndexError:
         print(__doc__)
         sys.exit(1)
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
 from copy import copy
 from contextlib import suppress
 import math
-import jinja2
+import os
 import sys
+import time
 
+import jinja2
 
 R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
@@ -297,7 +299,16 @@
                 resolution=resolution,
                 lng1=domain['lng1'],
                 lng2=domain['lng2'],
                 lat1=domain['lat1'],
                 lat2=domain['lat2'],
                 data=data
             ))
+
+
+def sleep(secs=4):
+    """Make the tutorials run a little slower so users can follow along.
+
+    (Only if not running in CI).
+    """
+    if 'CI' not in os.environ:
+        time.sleep(secs)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/forecast-script/forecast` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/forecast`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 
     # Generate html page from forecast data.
     util.generate_html_map(map_file, map_template, forecasts, domain,
                            resolution)
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = [int(sys.argv[1]), int(sys.argv[2])]
     except IndexError:
         print(__doc__)
         sys.exit(1)
 
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/forecast-script/util.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
 from copy import copy
 from contextlib import suppress
 import math
-import jinja2
+import os
 import sys
+import time
 
+import jinja2
 
 R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
@@ -297,7 +299,16 @@
                 resolution=resolution,
                 lng1=domain['lng1'],
                 lng2=domain['lng2'],
                 lat1=domain['lat1'],
                 lat2=domain['lat2'],
                 data=data
             ))
+
+
+def sleep(secs=4):
+    """Make the tutorials run a little slower so users can follow along.
+
+    (Only if not running in CI).
+    """
+    if 'CI' not in os.environ:
+        time.sleep(secs)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/map-template/map-template.html` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/retries-tutorial/.validate` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/.validate` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files 2% similar despite different names*

```diff
@@ -111,8 +111,9 @@
 
     # Write wind data to csv.
     util.field_to_csv(wind_x, x_range, y_range, 'wind_x.csv')
     util.field_to_csv(wind_y, x_range, y_range, 'wind_y.csv')
 
 
 if __name__ == '__main__':
+    util.sleep()
     main()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 
     # Generate html page from forecast data.
     util.generate_html_map(map_file, map_template, forecasts, domain,
                            resolution)
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = [int(sys.argv[1]), int(sys.argv[2])]
     except IndexError:
         print(__doc__)
         sys.exit(1)
 
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from datetime import datetime
 import json
 import os
 import re
 
 import requests
 
+import util
+
 
 BASE_URL = ('http://datapoint.metoffice.gov.uk/public/data/'
             'val/wxobs/all/json/{site_id}'
             '?res=hourly&time={time}&key={api_key}')
 
 # Compass bearings for ordinate directions.
 # NOTE: We measure direction by where the winds have come from!
@@ -211,9 +213,10 @@
 
     # Write observations.
     with open('wind.csv', 'w+') as data_file:
         data_file.write(', '.join(obs))
 
 
 if __name__ == '__main__':
+    util.sleep()
     main(os.environ['SITE_ID'],
          os.environ.get('API_KEY'))
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files 1% similar despite different names*

```diff
@@ -191,8 +191,9 @@
         get_archived_radar_image('rainfall-radar.png', time)
 
     data = process_rainfall_data('rainfall-radar.png', resolution, domain)
     util.write_csv('rainfall.csv', data)
 
 
 if __name__ == '__main__':
+    util.sleep(2)  # make the tutorial run a little slower
     main()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files 2% similar despite different names*

```diff
@@ -97,13 +97,14 @@
     # Write out forecast summary.
     with open('summary.txt', 'w+') as summary_file:
         summary_file.write('The outlook at %s UTC for %s is "%s"' % (
             forecast_time.strftime('%Y-%m-%dT%H:%M'), site_name, message))
 
 
 if __name__ == '__main__':
+    util.sleep()
     try:
         args = (sys.argv[1].lower(), int(sys.argv[2]))
     except IndexError:
         print(__doc__)
         sys.exit(1)
     main(*args)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!jinja2
 [scheduler]
     UTC mode = True
+    allow implicit tasks = True  # TODO: remove at end of exercise
 
 [scheduling]
     # TODO: Set initial cycle point
     # TODO: Set final cycle point
     [[graph]]
         # Repeat every three hours starting at the initial cycle point.
         PT3H = """
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
 from copy import copy
 from contextlib import suppress
 import math
-import jinja2
+import os
 import sys
+import time
 
+import jinja2
 
 R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
@@ -297,7 +299,16 @@
                 resolution=resolution,
                 lng1=domain['lng1'],
                 lng2=domain['lng2'],
                 lat1=domain['lat1'],
                 lat2=domain['lat2'],
                 data=data
             ))
+
+
+def sleep(secs=4):
+    """Make the tutorials run a little slower so users can follow along.
+
+    (Only if not running in CI).
+    """
+    if 'CI' not in os.environ:
+        time.sleep(secs)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/runtime-tutorial/runtime` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/rainfall.csv` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/exceptions.py` & `cylc-flow-8.2.5/cylc/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/flags.py` & `cylc-flow-8.2.5/cylc/flow/flags.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/flow_mgr.py` & `cylc-flow-8.2.5/cylc/flow/flow_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/graph_parser.py` & `cylc-flow-8.2.5/cylc/flow/graph_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,16 +458,20 @@
                 # Auto-trigger lone nodes and initial nodes in a chain.
                 if not item[0].startswith(self.__class__.XTRIG):
                     pairs.add((None, ''.join(item)))
 
             for i in range(0, len(chain) - 1):
                 pairs.add((chain[i], chain[i + 1]))
 
+        # Get a set of RH nodes which are not at the LH of another pair:
+        pairs_dict = dict(pairs)
+        terminals = set(pairs_dict.values()).difference(pairs_dict.keys())
+
         for pair in pairs:
-            self._proc_dep_pair(pair)
+            self._proc_dep_pair(pair, terminals)
 
     @classmethod
     def _report_invalid_lines(cls, lines: List[str]) -> None:
         """Raise GraphParseError in a consistent format when there are
         lines with bad syntax.
 
         The list of bad lines are inserted into the error message to show
@@ -489,27 +493,31 @@
             " {NAME(<PARAMS>) can also be: "
             "<PARAMS>NAME or NAME<PARAMS>NAME_CONTINUED}\n"
             " or\n"
             " NAME(<REMOTE-WORKFLOW-QUALIFIER>)(:QUALIFIER)")
 
     def _proc_dep_pair(
         self,
-        pair: Tuple[Optional[str], str]
+        pair: Tuple[Optional[str], str],
+        terminals: Set[str],
     ) -> None:
         """Process a single dependency pair 'left => right'.
 
-        'left' can be a logical expression of qualified node names.
-        'left' can be None, when triggering a left-side or lone node.
-        'left' can be "", if null task name in graph error (a => => b).
-        'right' can be one or more node names joined by AND.
-        'right' can't be None or "".
         A node is an xtrigger, or a task or a family name.
         A qualified name is NAME([CYCLE-POINT-OFFSET])(:QUALIFIER).
-        Trigger qualifiers, but not cycle offsets, are ignored on the right to
-        allow chaining.
+
+        Args:
+            pair:
+                'left' can be a logical expression of qualified node names.
+                'left' can be None, when triggering a left-side or lone node.
+                'left' can be "", if null task name in graph error (a => => b).
+                'right' can be one or more node names joined by AND.
+                'right' can't be None or "".
+            terminals:
+                Nodes which are _only_ on the RH end of chains.
         """
         left, right = pair
         # Raise error for right-hand-side OR operators.
         if self.__class__.OP_OR in right:
             raise GraphParseError(f"Illegal OR on right side: {right}")
 
         # Raise error if suicide triggers on the left of the trigger.
@@ -521,18 +529,25 @@
         # Check that parentheses match.
         mismatch_msg = 'Mismatched parentheses in: "{}"'
         if left and left.count("(") != left.count(")"):
             raise GraphParseError(mismatch_msg.format(left))
         if right.count("(") != right.count(")"):
             raise GraphParseError(mismatch_msg.format(right))
 
-        # Ignore cycle point offsets on the right side.
-        # (Note we can't ban this; all nodes get process as left and right.)
+        # Raise error for cycle point offsets at the end of chains
         if '[' in right:
-            return
+            if left and (right in terminals):
+                # This right hand side is at the end of a chain:
+                raise GraphParseError(
+                    'Invalid cycle point offsets only on right hand '
+                    'side of a dependency (must be on left hand side):'
+                    f' {left} => {right}')
+            else:
+                # This RHS is also a LHS in a chain:
+                return
 
         # Split right side on AND.
         rights = right.split(self.__class__.OP_AND)
         if '' in rights or right and not all(rights):
             raise GraphParseError(
                 f"Null task name in graph: {left} => {right}")
```

### Comparing `cylc-flow-8.2.4/cylc/flow/graphnode.py` & `cylc-flow-8.2.5/cylc/flow/graphnode.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/host_select.py` & `cylc-flow-8.2.5/cylc/flow/host_select.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/hostuserutil.py` & `cylc-flow-8.2.5/cylc/flow/hostuserutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/id.py` & `cylc-flow-8.2.5/cylc/flow/id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/id_cli.py` & `cylc-flow-8.2.5/cylc/flow/id_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,15 @@
     src: bool = False,
     match_workflows: bool = False,
     match_active: Optional[bool] = True,
     infer_latest_runs: bool = True,
     constraint: str = 'tasks',
     max_workflows: Optional[int] = None,
     max_tasks: Optional[int] = None,
+    alt_run_dir: Optional[str] = None,
 ) -> Tuple[Dict[str, List[Tokens]], Any]:
     """Parse IDs from the command line.
 
     Args:
         ids:
             Collection of IDs to parse.
         src:
@@ -233,14 +234,16 @@
             mixed - permit tasks not to be defined.
         max_workflows:
             Specify the maximum number of workflows permitted to be specified
             in the ids.
         max_tasks:
             Specify the maximum number of tasks permitted to be specified
             in the ids.
+        alt_run_dir:
+            Specify a non-standard cylc-run location, e.g. for another user.
 
     Returns:
         With src=True":
             (workflows, flow_file_path)
         Else:
             (workflow, multi_mode)
         Where:
@@ -295,15 +298,16 @@
 
     if not multi_mode:
         # check how many workflows we are working on
         multi_mode = contains_multiple_workflows(tokens_list)
 
     # infer the run number if not specified the ID (and if possible)
     if infer_latest_runs:
-        _infer_latest_runs(*tokens_list, src_path=src_path)
+        _infer_latest_runs(
+            *tokens_list, src_path=src_path, alt_run_dir=alt_run_dir)
 
     _validate_number(
         *tokens_list,
         max_workflows=max_workflows,
         max_tasks=max_tasks,
     )
 
@@ -410,20 +414,21 @@
                 cycle=tokens['task'],
                 task=tokens['job'],
             )
             LOG.warning(f'Did you mean: {suggested.id}')
         detect_both_flow_and_suite(src_path)
 
 
-def _infer_latest_runs(*tokens_list, src_path):
+def _infer_latest_runs(*tokens_list, src_path, alt_run_dir=None):
     for ind, tokens in enumerate(tokens_list):
         if ind == 0 and src_path:
             # source workflow passed in as a path
             continue
-        tokens['workflow'] = infer_latest_run_from_id(tokens['workflow'])
+        tokens['workflow'] = infer_latest_run_from_id(
+            tokens['workflow'], alt_run_dir)
         pass
 
 
 def _validate_number(*tokens_list, max_workflows=None, max_tasks=None):
     if not max_workflows and not max_tasks:
         return
     workflows_count = 0
```

### Comparing `cylc-flow-8.2.4/cylc/flow/id_match.py` & `cylc-flow-8.2.5/cylc/flow/id_match.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/install.py` & `cylc-flow-8.2.5/cylc/flow/install.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/install_plugins/__init__.py` & `cylc-flow-8.2.5/cylc/flow/install_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/install_plugins/log_vc_info.py` & `cylc-flow-8.2.5/cylc/flow/install_plugins/log_vc_info.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/jinja/filters/duration_as.py` & `cylc-flow-8.2.5/cylc/flow/jinja/filters/duration_as.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/jinja/filters/pad.py` & `cylc-flow-8.2.5/cylc/flow/jinja/filters/pad.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/jinja/filters/strftime.py` & `cylc-flow-8.2.5/cylc/flow/jinja/filters/strftime.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_file.py` & `cylc-flow-8.2.5/cylc/flow/job_file.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/__init__.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/at.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/at.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/background.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/background.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/documentation.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,14 +415,22 @@
         Args:
             job_file_path: The job file for this submission.
             submit_opts: Job submission options.
 
         Returns:
             (ret_code, out, err)
 
+            ret_code:
+                Subprocess return code.
+            out:
+                Subprocess standard output, note this should be newline
+                terminated.
+            err:
+                Subprocess standard error.
+
         """
         raise NotImplementedError()
 
     def manip_job_id(self, job_id: str) -> str:
         """Modify the job ID that is returned by the job submit command.
 
         Args:
```

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/loadleveler.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/loadleveler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/lsf.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/lsf.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/moab.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/moab.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/pbs.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/pbs_multi_cluster.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs_multi_cluster.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/sge.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/sge.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/slurm.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_handlers/slurm_packjob.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm_packjob.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/job_runner_mgr.py` & `cylc-flow-8.2.5/cylc/flow/job_runner_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/listify.py` & `cylc-flow-8.2.5/cylc/flow/listify.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/log_diagnosis.py` & `cylc-flow-8.2.5/cylc/flow/log_diagnosis.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/loggingutil.py` & `cylc-flow-8.2.5/cylc/flow/loggingutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/__init__.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/auto_restart.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/auto_restart.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/health_check.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/health_check.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/log_data_store.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/log_data_store.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/log_db.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/log_db.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/log_main_loop.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/log_main_loop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/log_memory.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/log_memory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/main_loop/reset_bad_hosts.py` & `cylc-flow-8.2.5/cylc/flow/main_loop/reset_bad_hosts.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/__init__.py` & `cylc-flow-8.2.5/cylc/flow/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/authentication.py` & `cylc-flow-8.2.5/cylc/flow/network/authentication.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/authorisation.py` & `cylc-flow-8.2.5/cylc/flow/network/authorisation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/client.py` & `cylc-flow-8.2.5/cylc/flow/network/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/client_factory.py` & `cylc-flow-8.2.5/cylc/flow/network/client_factory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/graphql.py` & `cylc-flow-8.2.5/cylc/flow/network/graphql.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/multi.py` & `cylc-flow-8.2.5/cylc/flow/network/multi.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/publisher.py` & `cylc-flow-8.2.5/cylc/flow/network/publisher.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/replier.py` & `cylc-flow-8.2.5/cylc/flow/network/replier.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/resolvers.py` & `cylc-flow-8.2.5/cylc/flow/network/resolvers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/scan.py` & `cylc-flow-8.2.5/cylc/flow/network/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/schema.py` & `cylc-flow-8.2.5/cylc/flow/network/schema.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/server.py` & `cylc-flow-8.2.5/cylc/flow/network/server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/ssh_client.py` & `cylc-flow-8.2.5/cylc/flow/network/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/network/subscriber.py` & `cylc-flow-8.2.5/cylc/flow/network/subscriber.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/option_parsers.py` & `cylc-flow-8.2.5/cylc/flow/option_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,35 +324,35 @@
 
 
 class CylcOptionParser(OptionParser):
 
     """Common options for all cylc CLI commands."""
 
     MULTITASK_USAGE = cparse(dedent('''
-        This command can operate on multiple tasks, globs and selectors may
-        be used:
+        This command can operate on multiple tasks. Globs and selectors may
+        be used to match active tasks:
             Multiple Tasks:
                 <dim># Operate on two tasks</dim>
                 workflow //cycle-1/task-1 //cycle-2/task-2
 
             Globs (note: globs should be quoted and only match active tasks):
-                <dim># Match any the active task "foo" in all cycles</dim>
+                <dim># Match any active task "foo" in all cycles</dim>
                 '//*/foo'
 
                 <dim># Match the tasks "foo-1" and "foo-2"</dim>
                 '//*/foo-[12]'
 
             Selectors (note: selectors only match active tasks):
                 <dim># match all failed tasks in cycle "1"</dim>
                 //1:failed
 
             See `cylc help id` for more details.
     '''))
     MULTIWORKFLOW_USAGE = cparse(dedent('''
-        This command can operate on multiple workflows, globs may also be used:
+        This command can operate on multiple workflows. Globs may be used:
             Multiple Workflows:
                 <dim># Operate on two workflows</dim>
                 workflow-1 workflow-2
 
             Globs (note: globs should be quoted):
                 <dim># Match all workflows</dim>
                 '*'
@@ -417,20 +417,21 @@
             ),
             action='append', default=[], dest='templatevars', useif='jset'
         ),
         OptionSettings(
             ['-z', '--set-list', '--template-list'],
             metavar='NAME=VALUE1,VALUE2,...',
             help=(
-                'Set the value of a Jinja2 template variable in the'
-                ' workflow definition as a comma separated'
-                ' list of Python strings.'
-                ' Values containing commas must be quoted.'
-                " e.g. '+s STR=a,b,c' => ['a', 'b', 'c']"
-                " or '+ s STR=a,\"b,c\"' => ['a', 'b,c']"
+                'A more convenient alternative to --set for defining a list'
+                ' of strings. E.G.'
+                ' "-z FOO=a,b,c" is shorthand for'
+                ' "-s FOO=[\'a\',\'b\',\'c\']".'
+                ' Commas can be present in values if quoted, e.g.'
+                ' "-z FOO=a,\'b,c\'" is shorthand for'
+                ' "-s FOO=[\'a\',\'b,c\']".'
                 + CAN_BE_USED_MULTIPLE
                 + NOTE_PERSIST_ACROSS_RESTARTS
             ),
             action='append', default=[], dest='templatevars_lists',
             useif='jset'
         ),
         OptionSettings(
@@ -873,17 +874,17 @@
 
     new_args = filter_sysargv(sys.argv, unwanted_simple, unwanted_compound)
 
     # replace compound script name:
     new_args[1] = script_name
 
     # replace source path with workflow ID.
-    if str(source) in sys.argv:
+    if str(source) in new_args:
         new_args.remove(str(source))
-    if workflow_id not in sys.argv:
+    if workflow_id not in new_args:
         new_args.append(workflow_id)
 
     sys.argv = new_args
 
 
 def filter_sysargv(
     sysargs, unwanted_simple: List, unwanted_compound: List
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cylc-flow-8.2.4/cylc/flow/param_expand.py` & `cylc-flow-8.2.5/cylc/flow/param_expand.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/OrderedDict.py` & `cylc-flow-8.2.5/cylc/flow/parsec/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/__init__.py` & `cylc-flow-8.2.5/cylc/flow/parsec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/config.py` & `cylc-flow-8.2.5/cylc/flow/parsec/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/empysupport.py` & `cylc-flow-8.2.5/cylc/flow/parsec/empysupport.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/exceptions.py` & `cylc-flow-8.2.5/cylc/flow/parsec/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/fileparse.py` & `cylc-flow-8.2.5/cylc/flow/parsec/fileparse.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/include.py` & `cylc-flow-8.2.5/cylc/flow/parsec/include.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/jinja2support.py` & `cylc-flow-8.2.5/cylc/flow/parsec/jinja2support.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/upgrade.py` & `cylc-flow-8.2.5/cylc/flow/parsec/upgrade.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/util.py` & `cylc-flow-8.2.5/cylc/flow/parsec/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/parsec/validate.py` & `cylc-flow-8.2.5/cylc/flow/parsec/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Also provides default values from the spec as a nested dict.
 """
 
 import re
 import shlex
 from collections import deque
 from textwrap import dedent
-from typing import List, Dict, Any, Tuple
+from typing import List, Dict, Any, Optional, Tuple
 
 from metomi.isodatetime.data import Duration, TimePoint
 from metomi.isodatetime.dumpers import TimePointDumper
 from metomi.isodatetime.parsers import TimePointParser, DurationParser
 from metomi.isodatetime.exceptions import IsodatetimeError, ISO8601SyntaxError
 
 from cylc.flow.parsec.exceptions import (
@@ -369,27 +369,27 @@
                 value,
                 msg='Integer range must be in the format min..max',
             )
         min_, max_ = match.groups()[0:2]
         return Range((int(min_), int(max_)))
 
     @classmethod
-    def coerce_str(cls, value, keys):
+    def coerce_str(cls, value, keys) -> str:
         """Coerce value to a string.
 
         Examples:
             >>> ParsecValidator.coerce_str('abc', None)
             'abc'
             >>> ParsecValidator.coerce_str(['abc', 'def'], None)
             'abc\\ndef'
 
         """
         if isinstance(value, list):
             # handle graph string merging
-            vraw = []
+            vraw: List[str] = []
             vals = [value]
             while vals:
                 val = vals.pop()
                 if isinstance(val, list):
                     vals.extend(reversed(val))  # reverse to preserve order
                 else:
                     vraw.append(cls.strip_and_unquote(keys, val))
@@ -508,49 +508,54 @@
             if not step:
                 step = 1
             return list(range(int(lower), int(upper) + 1, int(step)))
         else:
             return None
 
     @classmethod
-    def strip_and_unquote(cls, keys, value):
+    def _unquote(cls, keys: List[str], value: str) -> Optional[str]:
+        """Unquote value."""
+        for substr, rec in (
+            ("'''", cls._REC_MULTI_LINE_SINGLE),
+            ('"""', cls._REC_MULTI_LINE_DOUBLE),
+            ('"', cls._REC_DQ_VALUE),
+            ("'", cls._REC_SQ_VALUE)
+        ):
+            if value.startswith(substr):
+                match = rec.match(value)
+                if not match:
+                    raise IllegalValueError("string", keys, value)
+                return match[1]
+        return None
+
+    @classmethod
+    def strip_and_unquote(cls, keys: List[str], value: str) -> str:
         """Remove leading and trailing spaces and unquote value.
 
         Args:
-            keys (list):
+            keys:
                 Keys in nested dict that represents the raw configuration.
-            value (str):
+            value:
                 String value in raw configuration.
 
-        Return (str):
+        Return:
             Processed value.
 
         Examples:
             >>> ParsecValidator.strip_and_unquote(None, '" foo "')
             'foo'
 
         """
-        for substr, rec in [
-                ["'''", cls._REC_MULTI_LINE_SINGLE],
-                ['"""', cls._REC_MULTI_LINE_DOUBLE],
-                ['"', cls._REC_DQ_VALUE],
-                ["'", cls._REC_SQ_VALUE]]:
-            if value.startswith(substr):
-                match = rec.match(value)
-                if not match:
-                    raise IllegalValueError("string", keys, value)
-                value = match.groups()[0]
-                break
-        else:
-            # unquoted
-            value = value.split(r'#', 1)[0]
+        val = cls._unquote(keys, value)
+        if val is None:
+            val = value.split(r'#', 1)[0]
 
         # Note strip() removes leading and trailing whitespace, including
         # initial newlines on a multiline string:
-        return dedent(value).strip()
+        return dedent(val).strip()
 
     @classmethod
     def strip_and_unquote_list(cls, keys, value):
         """Remove leading and trailing spaces and unquote list value.
 
         Args:
             keys (list):
@@ -1132,32 +1137,34 @@
                     val = True
                 else:
                     # Leave as string.
                     val = cls.strip_and_unquote([], value)
         return val
 
 
-# BACK COMPAT: BroadcastConfigValidator
-# The DB at 8.0.x stores Interval values as neither ISO8601 duration
-# string or DurationFloat. This has been fixed at 8.1.0, and
-# the following class acts as a bridge between fixed and broken.
-# url:
-#     https://github.com/cylc/cylc-flow/pull/5138
-# from:
-#    8.0.x
-# to:
-#    8.1.x
-# remove at:
-#    8.x
 class BroadcastConfigValidator(CylcConfigValidator):
     """Validate and Coerce DB loaded broadcast config to internal objects."""
     def __init__(self):
         CylcConfigValidator.__init__(self)
 
     @classmethod
+    def coerce_str(cls, value, keys) -> str:
+        """Coerce value to a string. Unquotes & strips lead/trail whitespace.
+
+        Prevents ParsecValidator from assuming '#' means comments;
+        '#' has valid uses in shell script such as parameter substitution.
+
+        Examples:
+            >>> BroadcastConfigValidator.coerce_str('echo "${FOO#*bar}"', None)
+            'echo "${FOO#*bar}"'
+        """
+        val = ParsecValidator._unquote(keys, value) or value
+        return dedent(val).strip()
+
+    @classmethod
     def strip_and_unquote_list(cls, keys, value):
         """Remove leading and trailing spaces and unquote list value.
 
         Args:
             keys (list):
                 Keys in nested dict that represents the raw configuration.
             value (str):
@@ -1173,14 +1180,26 @@
             ... )
             ['1, 2', '3']
         """
         if value.startswith('[') and value.endswith(']'):
             value = value.lstrip('[').rstrip(']')
         return ParsecValidator.strip_and_unquote_list(keys, value)
 
+    # BACK COMPAT: BroadcastConfigValidator.coerce_interval
+    # The DB at 8.0.x stores Interval values as neither ISO8601 duration
+    # string or DurationFloat. This has been fixed at 8.1.0, and
+    # the following method acts as a bridge between fixed and broken.
+    # url:
+    #     https://github.com/cylc/cylc-flow/pull/5138
+    # from:
+    #    8.0.x
+    # to:
+    #    8.1.x
+    # remove at:
+    #    8.x
     @classmethod
     def coerce_interval(cls, value, keys):
         """Coerce an ISO 8601 interval into seconds.
 
         Examples:
             >>> BroadcastConfigValidator.coerce_interval('PT1H', None)
             3600.0
```

### Comparing `cylc-flow-8.2.4/cylc/flow/pathutil.py` & `cylc-flow-8.2.5/cylc/flow/pathutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,25 +67,38 @@
     workflow_id: Union[Path, str], *args: Union[Path, str]
 ) -> str:
     """Return remote workflow job log directory, joining any extra args,
     NOT expanding vars or user."""
     return get_remote_workflow_run_dir(workflow_id, 'log', 'job', *args)
 
 
-def get_cylc_run_dir() -> str:
-    """Return the cylc-run dir path with vars/user expanded."""
-    return expand_path(_CYLC_RUN_DIR)
+def get_cylc_run_dir(alt_run_dir: Optional[str] = None) -> str:
+    """Return the cylc-run dir, or alt path, with vars/user expanded."""
+    return expand_path(alt_run_dir or _CYLC_RUN_DIR)
+
+
+def get_alt_workflow_run_dir(
+    alt_run_dir: Union[Path, str],
+    workflow_id: Union[Path, str],
+    *args: Union[Path, str]
+) -> str:
+    """Return alternate workflow run directory.
+
+    Join any extra args, and expand vars and user.
+    Does not check that the directory exists.
+    """
+    return expand_path(alt_run_dir, workflow_id, *args)
 
 
 def get_workflow_run_dir(
     workflow_id: Union[Path, str], *args: Union[Path, str]
 ) -> str:
-    """Return local workflow run directory, joining any extra args, and
-    expanding vars and user.
+    """Return local workflow run directory.
 
+    Join any extra args, and expand vars and user.
     Does not check that the directory exists.
     """
     return expand_path(_CYLC_RUN_DIR, workflow_id, *args)
 
 
 def get_workflow_run_job_dir(workflow, *args):
     """Return workflow run job (log) directory, join any extra args."""
```

### Comparing `cylc-flow-8.2.4/cylc/flow/pipe_poller.py` & `cylc-flow-8.2.5/cylc/flow/pipe_poller.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/platforms.py` & `cylc-flow-8.2.5/cylc/flow/platforms.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/prerequisite.py` & `cylc-flow-8.2.5/cylc/flow/prerequisite.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/print_tree.py` & `cylc-flow-8.2.5/cylc/flow/print_tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/profiler.py` & `cylc-flow-8.2.5/cylc/flow/profiler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/remote.py` & `cylc-flow-8.2.5/cylc/flow/remote.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/resources.py` & `cylc-flow-8.2.5/cylc/flow/resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/rundb.py` & `cylc-flow-8.2.5/cylc/flow/rundb.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,27 +604,14 @@
                 {self.TABLE_WORKFLOW_PARAMS}
             WHERE
                 key == 'n_restart'
         """  # nosec (table name is code constant)
         result = self.connect().execute(stmt).fetchone()
         return int(result[0]) if result else 0
 
-    def select_workflow_params_run_mode(self):
-        """Return original run_mode for workflow_params."""
-        stmt = rf"""
-            SELECT
-                value
-            FROM
-                {self.TABLE_WORKFLOW_PARAMS}
-            WHERE
-                key == 'run_mode'
-        """  # nosec (table name is code constant)
-        result = self.connect().execute(stmt).fetchone()
-        return result[0] if result else None
-
     def select_workflow_template_vars(self, callback):
         """Select from workflow_template_vars.
 
         Invoke callback(row_idx, row) on each row, where each row contains:
             [key,value]
         """
         for row_idx, row in enumerate(self.connect().execute(
```

### Comparing `cylc-flow-8.2.4/cylc/flow/scheduler.py` & `cylc-flow-8.2.5/cylc/flow/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 )
 from cylc.flow.profiler import Profiler
 from cylc.flow.resources import get_resources
 from cylc.flow.subprocpool import SubProcPool
 from cylc.flow.templatevars import eval_var
 from cylc.flow.workflow_db_mgr import WorkflowDatabaseManager
 from cylc.flow.workflow_events import WorkflowEventHandler
-from cylc.flow.workflow_status import StopMode, AutoRestartMode
+from cylc.flow.workflow_status import RunMode, StopMode, AutoRestartMode
 from cylc.flow import workflow_files
 from cylc.flow.taskdef import TaskDef
 from cylc.flow.task_events_mgr import TaskEventsManager
 from cylc.flow.task_id import TaskID
 from cylc.flow.task_job_mgr import TaskJobManager
 from cylc.flow.task_pool import TaskPool
 from cylc.flow.task_remote_mgr import (
@@ -421,36 +421,31 @@
             LOG.info(f"Workflow: {self.workflow}")
 
         self.profiler.log_memory("scheduler.py: start configure")
 
         self._check_startup_opts()
 
         if self.is_restart:
+            run_mode = self.get_run_mode()
             self._set_workflow_params(params)
+            # Prevent changing run mode on restart:
+            og_run_mode = self.get_run_mode()
+            if run_mode != og_run_mode:
+                raise InputError(
+                    f'This workflow was originally run in {og_run_mode} mode:'
+                    f' Will not restart in {run_mode} mode.')
 
         self.profiler.log_memory("scheduler.py: before load_flow_file")
         try:
             cfg = self.load_flow_file()
             self.apply_new_config(cfg, is_reload=False)
         except ParsecError as exc:
             # Mark this exc as expected (see docstring for .schd_expected):
             exc.schd_expected = True
             raise exc
-
-        # Prevent changing mode on restart.
-        if self.is_restart:
-            # check run mode against db
-            og_run_mode = self.workflow_db_mgr.get_pri_dao(
-            ).select_workflow_params_run_mode() or 'live'
-            run_mode = self.config.run_mode()
-            if run_mode != og_run_mode:
-                raise InputError(
-                    f'This workflow was originally run in {og_run_mode} mode:'
-                    f' Will not restart in {run_mode} mode.')
-
         self.profiler.log_memory("scheduler.py: after load_flow_file")
 
         self.workflow_db_mgr.on_workflow_start(self.is_restart)
 
         if not self.is_restart:
             # Set workflow params that would otherwise be loaded from database:
             self.options.utc_mode = get_utc_mode()
@@ -599,15 +594,15 @@
                 f'Cylc version: {CYLC_VERSION}',
                 extra=RotatingLogFileHandler.header_extra
             )
 
             # Note that the following lines must be present at the top of
             # the workflow log file for use in reference test runs.
             LOG.info(
-                f'Run mode: {self.config.run_mode()}',
+                f'Run mode: {self.get_run_mode()}',
                 extra=RotatingLogFileHandler.header_extra
             )
             LOG.info(
                 f'Initial point: {self.config.initial_point}',
                 extra=RotatingLogFileHandler.header_extra
             )
             if self.config.start_point != self.config.initial_point:
@@ -646,15 +641,16 @@
                 )
             )
             self.server.publish_queue.put(
                 self.data_store_mgr.publish_deltas)
             # Non-async sleep - yield to other threads rather than event loop
             sleep(0)
             self.profiler.start()
-            await self.main_loop()
+            while True:  # MAIN LOOP
+                await self._main_loop()
 
         except SchedulerStop as exc:
             # deliberate stop
             await self.shutdown(exc)
             try:
                 if self.auto_restart_mode == AutoRestartMode.RESTART_NORMAL:
                     self.workflow_auto_restart()
@@ -1036,24 +1032,24 @@
 
     def command_resume(self) -> None:
         """Resume paused workflow."""
         self.resume_workflow()
 
     def command_poll_tasks(self, items: List[str]) -> int:
         """Poll pollable tasks or a task or family if options are provided."""
-        if self.config.run_mode('simulation'):
+        if self.get_run_mode() == RunMode.SIMULATION:
             return 0
         itasks, _, bad_items = self.pool.filter_task_proxies(items)
         self.task_job_mgr.poll_task_jobs(self.workflow, itasks)
         return len(bad_items)
 
     def command_kill_tasks(self, items: List[str]) -> int:
         """Kill all tasks or a task/family if options are provided."""
         itasks, _, bad_items = self.pool.filter_task_proxies(items)
-        if self.config.run_mode('simulation'):
+        if self.get_run_mode() == RunMode.SIMULATION:
             for itask in itasks:
                 if itask.state(*TASK_STATUSES_ACTIVE):
                     itask.state_reset(TASK_STATUS_FAILED)
                     self.data_store_mgr.delta_task_state(itask)
             return len(bad_items)
         self.task_job_mgr.kill_task_jobs(self.workflow, itasks)
         return len(bad_items)
@@ -1263,14 +1259,18 @@
         # Preserve contact data in memory, for regular health check.
         workflow_files.dump_contact_file(self.workflow, contact_data)
         self.contact_data = contact_data
 
     def load_flow_file(self, is_reload=False):
         """Load, and log the workflow definition."""
         # Local workflow environment set therein.
+        # Allow -S and -D to take effect in Cylc VR.
+        # https://github.com/cylc/cylc-flow/issues/5968
+        self.options.rose_template_vars = []
+        self.options.defines = []
         return WorkflowConfig(
             self.workflow,
             self.flow_file,
             self.options,
             self.template_vars,
             xtrigger_mgr=self.xtrigger_mgr,
             mem_log_func=self.profiler.log_memory,
@@ -1339,14 +1339,17 @@
         * Stop task.
         * Workflow UUID.
         * A flag to indicate if the workflow should be paused or not.
         * Original workflow run time zone.
         """
         LOG.info('LOADING workflow parameters')
         for key, value in params:
+            if key == self.workflow_db_mgr.KEY_RUN_MODE:
+                self.options.run_mode = value or RunMode.LIVE
+                LOG.info(f"+ run mode = {value}")
             if value is None:
                 continue
             if key in self.workflow_db_mgr.KEY_INITIAL_CYCLE_POINT_COMPATS:
                 self.options.icp = value
                 LOG.info(f"+ initial point = {value}")
             elif key in self.workflow_db_mgr.KEY_START_CYCLE_POINT_COMPATS:
                 self.options.startcp = value
@@ -1359,20 +1362,14 @@
                     LOG.info(f"+ final point = {value}")
             elif key == self.workflow_db_mgr.KEY_STOP_CYCLE_POINT:
                 if self.is_restart and self.options.stopcp == 'reload':
                     LOG.debug(f"- stop point = {value} (ignored)")
                 elif self.options.stopcp is None:
                     self.options.stopcp = value
                     LOG.info(f"+ stop point = {value}")
-            elif (
-                key == self.workflow_db_mgr.KEY_RUN_MODE
-                and self.options.run_mode is None
-            ):
-                self.options.run_mode = value
-                LOG.info(f"+ run mode = {value}")
             elif key == self.workflow_db_mgr.KEY_UUID_STR:
                 self.uuid_str = value
                 LOG.info(f"+ workflow UUID = {value}")
             elif key == self.workflow_db_mgr.KEY_PAUSED:
                 bool_val = bool(int(value))
                 if bool_val and not self.options.paused_start:
                     self.options.paused_start = bool_val
@@ -1410,20 +1407,16 @@
             self.template_vars[key] = eval_var(value)
 
     def run_event_handlers(self, event, reason=""):
         """Run a workflow event handler.
 
         Run workflow events in simulation and dummy mode ONLY if enabled.
         """
-        conf = self.config
-        with suppress(KeyError):
-            if (
-                conf.run_mode('simulation', 'dummy')
-            ):
-                return
+        if self.get_run_mode() in {RunMode.SIMULATION, RunMode.DUMMY}:
+            return
         self.workflow_event_handler.handle(self, event, str(reason))
 
     def release_queued_tasks(self) -> bool:
         """Release queued tasks, and submit jobs.
 
         The task queue manages references to task proxies in the task pool.
 
@@ -1488,15 +1481,15 @@
         if self.options.reftest or self.options.genref:
             log = LOG.info
         for itask in self.task_job_mgr.submit_task_jobs(
             self.workflow,
             pre_prep_tasks,
             self.server.curve_auth,
             self.server.client_pub_key_dir,
-            is_simulation=self.config.run_mode('simulation')
+            is_simulation=(self.get_run_mode() == RunMode.SIMULATION)
         ):
             if itask.flow_nums:
                 flow = ','.join(str(i) for i in itask.flow_nums)
             else:
                 flow = FLOW_NONE
             log(
                 f"{itask.identity} -triggered off "
@@ -1539,15 +1532,15 @@
         with suppress(KeyError):
             self.timers[self.EVENT_INACTIVITY_TIMEOUT].reset()
 
     def timeout_check(self):
         """Check workflow and task timers."""
         self.check_workflow_timers()
         # check submission and execution timeout and polling timers
-        if not self.config.run_mode('simulation'):
+        if self.get_run_mode() != RunMode.SIMULATION:
             self.task_job_mgr.check_task_jobs(self.workflow, self.pool)
 
     async def workflow_shutdown(self):
         """Determines if the workflow can be shutdown yet."""
         if self.pool.check_abort_on_task_fails():
             self._set_stop(StopMode.AUTO_ON_TASK_FAILURE)
 
@@ -1689,150 +1682,149 @@
         if now - self.previous_profile_point >= 60:
             # Only get this every minute.
             self.previous_profile_point = now
             self.profiler.log_memory("scheduler.py: loop #%d: %s" % (
                 self.count, get_current_time_string()))
         self.count += 1
 
-    async def main_loop(self) -> None:
-        """The scheduler main loop."""
-        while True:  # MAIN LOOP
-            tinit = time()
-
-            # Useful for debugging core scheduler issues:
-            # self.pool.log_task_pool(logging.CRITICAL)
-            if self.incomplete_ri_map:
-                self.manage_remote_init()
+    async def _main_loop(self) -> None:
+        """A single iteration of the main loop."""
+        tinit = time()
+
+        # Useful for debugging core scheduler issues:
+        # self.pool.log_task_pool(logging.CRITICAL)
+        if self.incomplete_ri_map:
+            self.manage_remote_init()
 
-            await self.process_command_queue()
-            self.proc_pool.process()
+        await self.process_command_queue()
+        self.proc_pool.process()
 
-            # Unqueued tasks with satisfied prerequisites must be waiting on
-            # xtriggers or ext_triggers. Check these and queue tasks if ready.
-            for itask in self.pool.get_tasks():
-                if (
-                    not itask.state(TASK_STATUS_WAITING)
-                    or itask.state.is_queued
-                    or itask.state.is_runahead
-                ):
-                    continue
+        # Unqueued tasks with satisfied prerequisites must be waiting on
+        # xtriggers or ext_triggers. Check these and queue tasks if ready.
+        for itask in self.pool.get_tasks():
+            if (
+                not itask.state(TASK_STATUS_WAITING)
+                or itask.state.is_queued
+                or itask.state.is_runahead
+            ):
+                continue
 
-                if (
-                    itask.state.xtriggers
-                    and not itask.state.xtriggers_all_satisfied()
-                ):
-                    self.xtrigger_mgr.call_xtriggers_async(itask)
+            if (
+                itask.state.xtriggers
+                and not itask.state.xtriggers_all_satisfied()
+            ):
+                self.xtrigger_mgr.call_xtriggers_async(itask)
 
-                if (
-                    itask.state.external_triggers
-                    and not itask.state.external_triggers_all_satisfied()
-                ):
-                    self.broadcast_mgr.check_ext_triggers(
-                        itask, self.ext_trigger_queue)
+            if (
+                itask.state.external_triggers
+                and not itask.state.external_triggers_all_satisfied()
+            ):
+                self.broadcast_mgr.check_ext_triggers(
+                    itask, self.ext_trigger_queue)
 
-                if all(itask.is_ready_to_run()):
-                    self.pool.queue_task(itask)
+            if all(itask.is_ready_to_run()):
+                self.pool.queue_task(itask)
 
-            if self.xtrigger_mgr.do_housekeeping:
-                self.xtrigger_mgr.housekeep(self.pool.get_tasks())
+        if self.xtrigger_mgr.do_housekeeping:
+            self.xtrigger_mgr.housekeep(self.pool.get_tasks())
 
-            self.pool.set_expired_tasks()
-            self.release_queued_tasks()
+        self.pool.set_expired_tasks()
+        self.release_queued_tasks()
 
-            if self.pool.sim_time_check(self.message_queue):
-                # A simulated task state change occurred.
-                self.reset_inactivity_timer()
+        if self.pool.sim_time_check(self.message_queue):
+            # A simulated task state change occurred.
+            self.reset_inactivity_timer()
 
-            self.broadcast_mgr.expire_broadcast(self.pool.get_min_point())
-            self.late_tasks_check()
+        self.broadcast_mgr.expire_broadcast(self.pool.get_min_point())
+        self.late_tasks_check()
 
-            self.process_queued_task_messages()
-            await self.process_command_queue()
-            self.task_events_mgr.process_events(self)
+        self.process_queued_task_messages()
+        await self.process_command_queue()
+        self.task_events_mgr.process_events(self)
 
-            # Update state summary, database, and uifeed
-            self.workflow_db_mgr.put_task_event_timers(self.task_events_mgr)
+        # Update state summary, database, and uifeed
+        self.workflow_db_mgr.put_task_event_timers(self.task_events_mgr)
 
-            # List of task whose states have changed.
-            updated_task_list = [
-                t for t in self.pool.get_tasks() if t.state.is_updated]
-            has_updated = updated_task_list or self.is_updated
+        # List of task whose states have changed.
+        updated_task_list = [
+            t for t in self.pool.get_tasks() if t.state.is_updated]
+        has_updated = updated_task_list or self.is_updated
 
-            if updated_task_list and self.is_restart_timeout_wait:
-                # Stop restart timeout if action has been triggered.
-                with suppress(KeyError):
-                    self.timers[self.EVENT_RESTART_TIMEOUT].stop()
-                    self.is_restart_timeout_wait = False
+        if updated_task_list and self.is_restart_timeout_wait:
+            # Stop restart timeout if action has been triggered.
+            with suppress(KeyError):
+                self.timers[self.EVENT_RESTART_TIMEOUT].stop()
+                self.is_restart_timeout_wait = False
 
-            if has_updated or self.data_store_mgr.updates_pending:
-                # Update the datastore.
-                await self.update_data_structure()
-
-            if has_updated:
-                if not self.is_reloaded:
-                    # (A reload cannot un-stall workflow by itself)
-                    self.is_stalled = False
-                self.is_reloaded = False
-
-                # Reset workflow and task updated flags.
-                self.is_updated = False
-                for itask in updated_task_list:
-                    itask.state.is_updated = False
+        if has_updated or self.data_store_mgr.updates_pending:
+            # Update the datastore.
+            await self.update_data_structure()
 
-                if not self.is_stalled:
-                    # Stop the stalled timer.
-                    with suppress(KeyError):
-                        self.timers[self.EVENT_STALL_TIMEOUT].stop()
+        if has_updated:
+            if not self.is_reloaded:
+                # (A reload cannot un-stall workflow by itself)
+                self.is_stalled = False
+            self.is_reloaded = False
+
+            # Reset workflow and task updated flags.
+            self.is_updated = False
+            for itask in updated_task_list:
+                itask.state.is_updated = False
 
-            self.process_workflow_db_queue()
+            if not self.is_stalled:
+                # Stop the stalled timer.
+                with suppress(KeyError):
+                    self.timers[self.EVENT_STALL_TIMEOUT].stop()
 
-            # If public database is stuck, blast it away by copying the content
-            # of the private database into it.
-            self.database_health_check()
+        self.process_workflow_db_queue()
 
-            # Shutdown workflow if timeouts have occurred
-            self.timeout_check()
+        # If public database is stuck, blast it away by copying the content
+        # of the private database into it.
+        self.database_health_check()
 
-            # Does the workflow need to shutdown on task failure?
-            await self.workflow_shutdown()
+        # Shutdown workflow if timeouts have occurred
+        self.timeout_check()
 
-            if self.options.profile_mode:
-                self.update_profiler_logs(tinit)
+        # Does the workflow need to shutdown on task failure?
+        await self.workflow_shutdown()
 
-            # Run plugin functions
-            await asyncio.gather(
-                *main_loop.get_runners(
-                    self.main_loop_plugins,
-                    main_loop.CoroTypes.Periodic,
-                    self
-                )
+        if self.options.profile_mode:
+            self.update_profiler_logs(tinit)
+
+        # Run plugin functions
+        await asyncio.gather(
+            *main_loop.get_runners(
+                self.main_loop_plugins,
+                main_loop.CoroTypes.Periodic,
+                self
             )
+        )
 
-            if not has_updated and not self.stop_mode:
-                # Has the workflow stalled?
-                self.check_workflow_stalled()
-
-            # Sleep a bit for things to catch up.
-            # Quick sleep if there are items pending in process pool.
-            # (Should probably use quick sleep logic for other queues?)
-            elapsed = time() - tinit
-            quick_mode = self.proc_pool.is_not_done()
-            if (elapsed >= self.INTERVAL_MAIN_LOOP or
-                    quick_mode and elapsed >= self.INTERVAL_MAIN_LOOP_QUICK):
-                # Main loop has taken quite a bit to get through
-                # Still yield control to other threads by sleep(0.0)
-                duration: float = 0
-            elif quick_mode:
-                duration = self.INTERVAL_MAIN_LOOP_QUICK - elapsed
-            else:
-                duration = self.INTERVAL_MAIN_LOOP - elapsed
-            await asyncio.sleep(duration)
-            # Record latest main loop interval
-            self.main_loop_intervals.append(time() - tinit)
-            # END MAIN LOOP
+        if not has_updated and not self.stop_mode:
+            # Has the workflow stalled?
+            self.check_workflow_stalled()
+
+        # Sleep a bit for things to catch up.
+        # Quick sleep if there are items pending in process pool.
+        # (Should probably use quick sleep logic for other queues?)
+        elapsed = time() - tinit
+        quick_mode = self.proc_pool.is_not_done()
+        if (elapsed >= self.INTERVAL_MAIN_LOOP or
+                quick_mode and elapsed >= self.INTERVAL_MAIN_LOOP_QUICK):
+            # Main loop has taken quite a bit to get through
+            # Still yield control to other threads by sleep(0.0)
+            duration: float = 0
+        elif quick_mode:
+            duration = self.INTERVAL_MAIN_LOOP_QUICK - elapsed
+        else:
+            duration = self.INTERVAL_MAIN_LOOP - elapsed
+        await asyncio.sleep(duration)
+        # Record latest main loop interval
+        self.main_loop_intervals.append(time() - tinit)
+        # END MAIN LOOP
 
     def _update_workflow_state(self):
         """Update workflow state in the data store and push out any deltas.
 
         A cut-down version of update_data_structure which only considers
         workflow state changes e.g. status, status message, state totals, etc.
         """
@@ -1863,20 +1855,19 @@
             sleep(0)
 
     def check_workflow_timers(self):
         """Check timers, and abort or run event handlers as configured."""
         for event, timer in self.timers.items():
             if not timer.timed_out():
                 continue
+            self.run_event_handlers(event)
             abort_conf = f"abort on {event}"
             if self._get_events_conf(abort_conf):
                 # "cylc play" needs to exit with error status here.
                 raise SchedulerError(f'"{abort_conf}" is set')
-            if self._get_events_conf(f"{event} handlers") is not None:
-                self.run_event_handlers(event)
             if event == self.EVENT_RESTART_TIMEOUT:
                 # Unset wait flag to allow normal shutdown.
                 self.is_restart_timeout_wait = False
 
     def check_workflow_stalled(self) -> bool:
         """Check if workflow is stalled or not."""
         if self.is_stalled:  # already reported
@@ -2200,14 +2191,17 @@
         if not self.is_restart:
             for opt in ('fcp', 'stopcp'):
                 if getattr(self.options, opt, None) == 'reload':
                     raise InputError(
                         f"option --{opt}=reload is only valid for restart"
                     )
 
+    def get_run_mode(self) -> str:
+        return RunMode.get(self.options)
+
     async def handle_exception(self, exc: BaseException) -> NoReturn:
         """Gracefully shut down the scheduler given a caught exception.
 
         Re-raises the exception to be caught higher up (sets the exit code).
 
         Args:
             exc: The caught exception to be logged during the shutdown.
```

### Comparing `cylc-flow-8.2.4/cylc/flow/scheduler_cli.py` & `cylc-flow-8.2.5/cylc/flow/scheduler_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     get_workflow_srv_dir,
 )
 from cylc.flow.terminal import (
     cli_function,
     is_terminal,
     prompt,
 )
+from cylc.flow.workflow_status import RunMode
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
 PLAY_DOC = r"""cylc play [OPTIONS] ARGS
 
@@ -126,15 +127,15 @@
 PLAY_ICP_OPTION = deepcopy(ICP_OPTION)
 PLAY_ICP_OPTION.sources = {'play'}
 
 RUN_MODE = OptionSettings(
     ["-m", "--mode"],
     help="Run mode: live, dummy, simulation (default live).",
     metavar="STRING", action='store', dest="run_mode",
-    choices=['live', 'dummy', 'simulation'],
+    choices=[RunMode.LIVE, RunMode.DUMMY, RunMode.SIMULATION],
 )
 
 PLAY_RUN_MODE = deepcopy(RUN_MODE)
 PLAY_RUN_MODE.sources = {'play'}
 
 PLAY_OPTIONS = [
     OptionSettings(
```

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/__init__.py` & `cylc-flow-8.2.5/cylc/flow/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/broadcast.py` & `cylc-flow-8.2.5/cylc/flow/scripts/broadcast.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 
 Broadcast cannot change [runtime] inheritance.
 """
 
 from ansimarkup import parse as cparse
 from copy import deepcopy
 from functools import partial
+import os.path
 import re
 import sys
 from tempfile import NamedTemporaryFile
 from typing import Any, Dict, TYPE_CHECKING
 
 from cylc.flow.broadcast_report import (
     get_broadcast_bad_options_report,
@@ -199,15 +200,15 @@
     for setting_file in setting_files:
         if setting_file == '-':
             with NamedTemporaryFile() as handle:
                 handle.write(sys.stdin.read().encode())
                 handle.seek(0, 0)
                 cfg.loadcfg(handle.name)
         else:
-            cfg.loadcfg(setting_file)
+            cfg.loadcfg(os.path.abspath(setting_file))
     stack = [([], cfg.get(sparse=True))]
     while stack:
         keys, item = stack.pop()
         if isinstance(item, dict):
             for key, value in item.items():
                 stack.append((keys + [key], value))
         else:
```

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/cat_log.py` & `cylc-flow-8.2.5/cylc/flow/scripts/cat_log.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/check_versions.py` & `cylc-flow-8.2.5/cylc/flow/scripts/check_versions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/clean.py` & `cylc-flow-8.2.5/cylc/flow/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/client.py` & `cylc-flow-8.2.5/cylc/flow/scripts/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/common.py` & `cylc-flow-8.2.5/cylc/flow/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/completion_server.py` & `cylc-flow-8.2.5/cylc/flow/scripts/completion_server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/config.py` & `cylc-flow-8.2.5/cylc/flow/scripts/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/cycle_point.py` & `cylc-flow-8.2.5/cylc/flow/scripts/cycle_point.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/cylc.py` & `cylc-flow-8.2.5/cylc/flow/scripts/cylc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/diff.py` & `cylc-flow-8.2.5/cylc/flow/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/dump.py` & `cylc-flow-8.2.5/cylc/flow/scripts/dump.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/ext_trigger.py` & `cylc-flow-8.2.5/cylc/flow/scripts/ext_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/function_run.py` & `cylc-flow-8.2.5/cylc/flow/scripts/function_run.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/get_resources.py` & `cylc-flow-8.2.5/cylc/flow/scripts/get_resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/get_workflow_contact.py` & `cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_contact.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/get_workflow_version.py` & `cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_version.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/graph.py` & `cylc-flow-8.2.5/cylc/flow/scripts/graph.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/hold.py` & `cylc-flow-8.2.5/cylc/flow/scripts/hold.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,21 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """cylc hold [OPTIONS] ARGS
 
 Hold task(s) in a workflow.
 
-Held tasks do not submit their jobs even if ready to run.
+Held tasks do not submit jobs even if ready.
+
+Any task can be held.
+
+Note: a held running task will not submit more jobs itself (e.g. by retries)
+until released, but the running job may still complete outputs that cause
+non-held downstream tasks to trigger.
 
 To pause an entire workflow use "cylc pause".
 
 Examples:
   # Hold mytask at cycle point 1234 in my_workflow (if it has not yet spawned,
   # it will hold as soon as it spawns):
   $ cylc hold my_workflow//1234/mytask
```

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/install.py` & `cylc-flow-8.2.5/cylc/flow/scripts/install.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/jobs_kill.py` & `cylc-flow-8.2.5/cylc/flow/scripts/jobs_kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/jobs_poll.py` & `cylc-flow-8.2.5/cylc/flow/scripts/jobs_poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/jobs_submit.py` & `cylc-flow-8.2.5/cylc/flow/scripts/jobs_submit.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/kill.py` & `cylc-flow-8.2.5/cylc/flow/scripts/kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/lint.py` & `cylc-flow-8.2.5/cylc/flow/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/list.py` & `cylc-flow-8.2.5/cylc/flow/scripts/list.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/message.py` & `cylc-flow-8.2.5/cylc/flow/scripts/message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/pause.py` & `cylc-flow-8.2.5/cylc/flow/scripts/pause.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/ping.py` & `cylc-flow-8.2.5/cylc/flow/scripts/ping.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/play.py` & `cylc-flow-8.2.5/cylc/flow/scripts/play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/poll.py` & `cylc-flow-8.2.5/cylc/flow/scripts/poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/psutil.py` & `cylc-flow-8.2.5/cylc/flow/scripts/psutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/reinstall.py` & `cylc-flow-8.2.5/cylc/flow/scripts/reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/release.py` & `cylc-flow-8.2.5/cylc/flow/scripts/release.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/reload.py` & `cylc-flow-8.2.5/cylc/flow/scripts/reload.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/remote_init.py` & `cylc-flow-8.2.5/cylc/flow/scripts/remote_init.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/remote_tidy.py` & `cylc-flow-8.2.5/cylc/flow/scripts/remote_tidy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/remove.py` & `cylc-flow-8.2.5/cylc/flow/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/report_timings.py` & `cylc-flow-8.2.5/cylc/flow/scripts/report_timings.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/scan.py` & `cylc-flow-8.2.5/cylc/flow/scripts/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/set_outputs.py` & `cylc-flow-8.2.5/cylc/flow/scripts/set_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/set_verbosity.py` & `cylc-flow-8.2.5/cylc/flow/scripts/set_verbosity.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/show.py` & `cylc-flow-8.2.5/cylc/flow/scripts/show.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/stop.py` & `cylc-flow-8.2.5/cylc/flow/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/subscribe.py` & `cylc-flow-8.2.5/cylc/flow/scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/trigger.py` & `cylc-flow-8.2.5/cylc/flow/scripts/trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/tui.py` & `cylc-flow-8.2.5/cylc/flow/scripts/tui.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/validate.py` & `cylc-flow-8.2.5/cylc/flow/scripts/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     ICP_OPTION,
 )
 from cylc.flow.profiler import Profiler
 from cylc.flow.task_proxy import TaskProxy
 from cylc.flow.templatevars import get_template_vars
 from cylc.flow.terminal import cli_function
 from cylc.flow.scheduler_cli import RUN_MODE
+from cylc.flow.workflow_status import RunMode
 
 
 VALIDATE_RUN_MODE = deepcopy(RUN_MODE)
 VALIDATE_RUN_MODE.sources = {'validate'}
 VALIDATE_ICP_OPTION = deepcopy(ICP_OPTION)
 VALIDATE_ICP_OPTION.sources = {'validate'}
 VALIDATE_AGAINST_SOURCE_OPTION = deepcopy(AGAINST_SOURCE_OPTION)
@@ -119,15 +120,15 @@
 
 ValidateOptions = Options(
     get_option_parser(),
     # defaults
     {
         'check_circular': False,
         'profile_mode': False,
-        'run_mode': 'live'
+        'run_mode': RunMode.LIVE
     }
 )
 
 
 @cli_function(get_option_parser)
 def main(parser: COP, options: 'Values', workflow_id: str) -> None:
     _main(parser, options, workflow_id)
```

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/validate_install_play.py` & `cylc-flow-8.2.5/cylc/flow/scripts/validate_install_play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/validate_reinstall.py` & `cylc-flow-8.2.5/cylc/flow/scripts/validate_reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/view.py` & `cylc-flow-8.2.5/cylc/flow/scripts/view.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/scripts/workflow_state.py` & `cylc-flow-8.2.5/cylc/flow/scripts/workflow_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,25 +54,25 @@
 import sqlite3
 import sys
 from time import sleep
 from typing import TYPE_CHECKING
 
 from cylc.flow.exceptions import CylcError, InputError
 import cylc.flow.flags
-from cylc.flow.id_cli import parse_id
 from cylc.flow.option_parsers import (
     WORKFLOW_ID_ARG_DOC,
     CylcOptionParser as COP,
 )
 from cylc.flow.dbstatecheck import CylcWorkflowDBChecker
 from cylc.flow.command_polling import Poller
 from cylc.flow.task_state import TASK_STATUSES_ORDERED
 from cylc.flow.terminal import cli_function
 from cylc.flow.cycling.util import add_offset
-from cylc.flow.pathutil import expand_path, get_cylc_run_dir
+from cylc.flow.pathutil import get_cylc_run_dir
+from cylc.flow.workflow_files import infer_latest_run_from_id
 
 from metomi.isodatetime.parsers import TimePointParser
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
@@ -158,15 +158,15 @@
         action="store_true", dest="use_task_point", default=False)
 
     parser.add_option(
         "-d", "--run-dir",
         help="The top level cylc run directory if non-standard. The "
              "database should be DIR/WORKFLOW_ID/log/db. Use to interrogate "
              "workflows owned by others, etc.; see note above.",
-        metavar="DIR", action="store", dest="run_dir", default=None)
+        metavar="DIR", action="store", dest="alt_run_dir", default=None)
 
     parser.add_option(
         "-s", "--offset",
         help="Specify an offset to add to the targeted cycle point",
         action="store", dest="offset", default=None)
 
     conds = ("Valid triggering conditions to check for include: '" +
@@ -192,18 +192,14 @@
     WorkflowPoller.add_to_cmd_options(parser)
 
     return parser
 
 
 @cli_function(get_option_parser, remove_opts=["--db"])
 def main(parser: COP, options: 'Values', workflow_id: str) -> None:
-    workflow_id, *_ = parse_id(
-        workflow_id,
-        constraint='workflows',
-    )
 
     if options.use_task_point and options.cycle:
         raise InputError(
             "cannot specify a cycle point and use environment variable")
 
     if options.use_task_point:
         if "CYLC_TASK_CYCLE_POINT" not in os.environ:
@@ -227,23 +223,19 @@
 
     # Exit if an invalid status is requested
     if (options.status and
             options.status not in TASK_STATUSES_ORDERED and
             options.status not in CylcWorkflowDBChecker.STATE_ALIASES):
         raise InputError(f"invalid status '{options.status}'")
 
-    # this only runs locally
-    if options.run_dir:
-        run_dir = expand_path(options.run_dir)
-    else:
-        run_dir = get_cylc_run_dir()
+    workflow_id = infer_latest_run_from_id(workflow_id, options.alt_run_dir)
 
     pollargs = {
         'workflow_id': workflow_id,
-        'run_dir': run_dir,
+        'run_dir': get_cylc_run_dir(alt_run_dir=options.alt_run_dir),
         'task': options.task,
         'cycle': options.cycle,
         'status': options.status,
         'message': options.msg,
     }
 
     spoller = WorkflowPoller(
@@ -252,15 +244,15 @@
         options.max_polls,
         args=pollargs,
     )
 
     connected, formatted_pt = spoller.connect()
 
     if not connected:
-        raise CylcError("cannot connect to the workflow_id DB")
+        raise CylcError(f"Cannot connect to the {workflow_id} DB")
 
     if options.status and options.task and options.cycle:
         # check a task status
         spoller.condition = options.status
         if not asyncio.run(spoller.poll()):
             sys.exit(1)
     elif options.msg:
```

### Comparing `cylc-flow-8.2.4/cylc/flow/subprocctx.py` & `cylc-flow-8.2.5/cylc/flow/subprocctx.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/subprocpool.py` & `cylc-flow-8.2.5/cylc/flow/subprocpool.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_action_timer.py` & `cylc-flow-8.2.5/cylc/flow/task_action_timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_events_mgr.py` & `cylc-flow-8.2.5/cylc/flow/task_events_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     get_seconds_as_interval_string as intvl_as_str
 )
 from cylc.flow.workflow_events import (
     EventData as WorkflowEventData,
     get_template_variables as get_workflow_template_variables,
     process_mail_footer,
 )
+from cylc.flow.workflow_status import RunMode
 
 
 if TYPE_CHECKING:
     from cylc.flow.task_proxy import TaskProxy
     from cylc.flow.scheduler import Scheduler
 
 
@@ -663,25 +664,25 @@
             if (
                     flag == self.FLAG_RECEIVED
                     and itask.state.is_gt(TASK_STATUS_SUBMITTED)
             ):
                 return True
             if (
                 itask.state.status == TASK_STATUS_PREPARING
-                or itask.tdef.run_mode == 'simulation'
+                or itask.tdef.run_mode == RunMode.SIMULATION
             ):
                 # If not in the preparing state we already assumed and handled
                 # job submission under the started event above...
                 # (sim mode does not have the job prep state)
                 self._process_message_submitted(itask, event_time)
                 self.spawn_func(itask, TASK_OUTPUT_SUBMITTED)
 
             # ... but either way update the job ID in the job proxy (it only
             # comes in via the submission message).
-            if itask.tdef.run_mode != 'simulation':
+            if itask.tdef.run_mode != RunMode.SIMULATION:
                 job_tokens = itask.tokens.duplicate(
                     job=str(itask.submit_num)
                 )
                 self.data_store_mgr.delta_job_attr(
                     job_tokens, 'job_id', itask.summary['submit_method_id'])
 
         elif message.startswith(FAIL_MESSAGE_PREFIX):
@@ -820,15 +821,15 @@
         }:
             severity = DEBUG
         LOG.log(severity, f"[{itask}] {flag}{message}{timestamp}")
         return True
 
     def setup_event_handlers(self, itask, event, message):
         """Set up handlers for a task event."""
-        if itask.tdef.run_mode != 'live':
+        if itask.tdef.run_mode != RunMode.LIVE:
             return
         msg = ""
         if message != f"job {event}":
             msg = message
         self._db_events_insert(itask, event, msg)
         self._setup_job_logs_retrieval(itask, event)
         self._setup_event_mail(itask, event)
@@ -1238,15 +1239,15 @@
                 f"[{itask}] submitted to "
                 f"{summary['platforms_used'][itask.submit_num]}:"
                 f"{summary['job_runner_name']}"
                 f"[{summary['submit_method_id']}]"
             )
 
         itask.set_summary_time('submitted', event_time)
-        if itask.tdef.run_mode == 'simulation':
+        if itask.tdef.run_mode == RunMode.SIMULATION:
             # Simulate job started as well.
             itask.set_summary_time('started', event_time)
             if itask.state_reset(TASK_STATUS_RUNNING):
                 self.data_store_mgr.delta_task_state(itask)
             itask.state.outputs.set_completion(TASK_OUTPUT_STARTED, True)
             self.data_store_mgr.delta_task_output(itask, TASK_OUTPUT_STARTED)
         else:
@@ -1273,15 +1274,15 @@
         self._insert_task_job(itask, event_time, self.JOB_SUBMIT_SUCCESS_FLAG)
         job_tokens = itask.tokens.duplicate(job=str(itask.submit_num))
         self.data_store_mgr.delta_job_time(
             job_tokens,
             'submitted',
             event_time,
         )
-        if itask.tdef.run_mode == 'simulation':
+        if itask.tdef.run_mode == RunMode.SIMULATION:
             # Simulate job started as well.
             self.data_store_mgr.delta_job_time(
                 job_tokens,
                 'started',
                 event_time,
             )
         else:
```

### Comparing `cylc-flow-8.2.4/cylc/flow/task_id.py` & `cylc-flow-8.2.5/cylc/flow/task_id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_job_logs.py` & `cylc-flow-8.2.5/cylc/flow/task_job_logs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_job_mgr.py` & `cylc-flow-8.2.5/cylc/flow/task_job_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_message.py` & `cylc-flow-8.2.5/cylc/flow/task_message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_outputs.py` & `cylc-flow-8.2.5/cylc/flow/task_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_pool.py` & `cylc-flow-8.2.5/cylc/flow/task_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1727,15 +1727,15 @@
                 # De-queue it to run now.
                 self.task_queue_mgr.force_release_task(itask)
 
         return len(unmatched)
 
     def sim_time_check(self, message_queue: 'Queue[TaskMsg]') -> bool:
         """Simulation mode: simulate task run times and set states."""
-        if not self.config.run_mode('simulation'):
+        if self.config.run_mode() != 'simulation':
             return False
         sim_task_state_changed = False
         now = time()
         for itask in self.get_tasks():
             if itask.state.status != TASK_STATUS_RUNNING:
                 continue
             # Started time is not set on restart
```

### Comparing `cylc-flow-8.2.4/cylc/flow/task_proxy.py` & `cylc-flow-8.2.5/cylc/flow/task_proxy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_qualifiers.py` & `cylc-flow-8.2.5/cylc/flow/task_qualifiers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_queues/__init__.py` & `cylc-flow-8.2.5/cylc/flow/task_queues/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_queues/independent.py` & `cylc-flow-8.2.5/cylc/flow/task_queues/independent.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_remote_cmd.py` & `cylc-flow-8.2.5/cylc/flow/task_remote_cmd.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_remote_mgr.py` & `cylc-flow-8.2.5/cylc/flow/task_remote_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             *verbosity_to_opts(cylc.flow.flags.verbosity),
             str(install_target),
             get_remote_workflow_run_dir(self.workflow)
         ]
         dirs_to_symlink = get_dirs_to_symlink(install_target, self.workflow)
         for key, value in dirs_to_symlink.items():
             if value is not None:
-                cmd.append(f"{key}={quote(value)} ")
+                cmd.append(f"{key}={quote(value)}")
         # Create the ssh command
         try:
             host = get_host_from_platform(
                 platform, bad_hosts=self.bad_hosts
             )
         except NoHostsError as exc:
             LOG.error(
```

### Comparing `cylc-flow-8.2.4/cylc/flow/task_state.py` & `cylc-flow-8.2.5/cylc/flow/task_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_state_prop.py` & `cylc-flow-8.2.5/cylc/flow/task_state_prop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/task_trigger.py` & `cylc-flow-8.2.5/cylc/flow/task_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/taskdef.py` & `cylc-flow-8.2.5/cylc/flow/taskdef.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/templatevars.py` & `cylc-flow-8.2.5/cylc/flow/templatevars.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/terminal.py` & `cylc-flow-8.2.5/cylc/flow/terminal.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/time_parser.py` & `cylc-flow-8.2.5/cylc/flow/time_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/timer.py` & `cylc-flow-8.2.5/cylc/flow/timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/tui/__init__.py` & `cylc-flow-8.2.5/cylc/flow/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/tui/app.py` & `cylc-flow-8.2.5/cylc/flow/tui/app.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/tui/data.py` & `cylc-flow-8.2.5/cylc/flow/tui/data.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/tui/overlay.py` & `cylc-flow-8.2.5/cylc/flow/tui/overlay.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/tui/tree.py` & `cylc-flow-8.2.5/cylc/flow/tui/tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/tui/util.py` & `cylc-flow-8.2.5/cylc/flow/tui/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/unicode_rules.py` & `cylc-flow-8.2.5/cylc/flow/unicode_rules.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/util.py` & `cylc-flow-8.2.5/cylc/flow/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/wallclock.py` & `cylc-flow-8.2.5/cylc/flow/wallclock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/workflow_db_mgr.py` & `cylc-flow-8.2.5/cylc/flow/workflow_db_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,17 +401,18 @@
                     "timeout": timer.timeout
                 })
             task_events_mgr.event_timers_updated = False
 
     def put_xtriggers(self, sat_xtrig):
         """Put statements to update external triggers table."""
         for sig, res in sat_xtrig.items():
-            self.db_inserts_map[self.TABLE_XTRIGGERS].append({
-                "signature": sig,
-                "results": json.dumps(res)})
+            if not sig.startswith('wall_clock('):
+                self.db_inserts_map[self.TABLE_XTRIGGERS].append({
+                    "signature": sig,
+                    "results": json.dumps(res)})
 
     def put_update_task_state(self, itask):
         """Update task_states table for current state of itask.
 
         NOTE the task_states table is normally updated along with the task pool
         table. This method is only needed as a final update for finished tasks,
         when they get removed from the task_pool.
```

### Comparing `cylc-flow-8.2.4/cylc/flow/workflow_events.py` & `cylc-flow-8.2.5/cylc/flow/workflow_events.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/workflow_files.py` & `cylc-flow-8.2.5/cylc/flow/workflow_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     get_user,
     is_remote_host,
 )
 from cylc.flow.pathutil import (
     expand_path,
     get_cylc_run_dir,
     get_workflow_run_dir,
+    get_alt_workflow_run_dir,
     make_localhost_symlinks,
 )
 from cylc.flow.remote import (
     construct_cylc_server_ssh_cmd,
 )
 from cylc.flow.terminal import parse_dirty_json
 from cylc.flow.unicode_rules import WorkflowNameValidator
@@ -836,51 +837,61 @@
     for dir_name in Path(name).parts:
         if dir_name in WorkflowFiles.RESERVED_NAMES:
             raise WorkflowFilesError(err_msg.format(dir_name))
         if re.match(r'^run\d+$', dir_name):
             raise WorkflowFilesError(err_msg.format('run<number>'))
 
 
-def infer_latest_run_from_id(workflow_id: str) -> str:
-    run_dir = Path(get_workflow_run_dir(workflow_id))
-    _, id_ = infer_latest_run(run_dir)
+def infer_latest_run_from_id(
+    workflow_id: str, alt_run_dir: Optional[str] = None
+) -> str:
+    """Wrapper to make the workflow run-dir absolute."""
+    if alt_run_dir is not None:
+        run_dir = Path(get_alt_workflow_run_dir(alt_run_dir, workflow_id))
+    else:
+        run_dir = Path(get_workflow_run_dir(workflow_id))
+    _, id_ = infer_latest_run(run_dir, alt_run_dir=alt_run_dir)
     return id_
 
 
 def infer_latest_run(
     path: Path,
     implicit_runN: bool = True,
     warn_runN: bool = True,
+    alt_run_dir: Optional[str] = None,
 ) -> Tuple[Path, str]:
     """Infer the numbered run dir if the workflow has a runN symlink.
 
     Args:
         path: Absolute path to the workflow dir, run dir or runN dir.
         implicit_runN: If True, add runN on the end of the path if the path
             doesn't include it.
         warn_runN: If True, warn that explicit use of runN is unnecessary.
+        alt_run_dir: Path to alternate cylc-run location (e.g. for other user).
 
     Returns:
         path: Absolute path of the numbered run dir if applicable, otherwise
             the input arg path.
         id_: The workflow name (including the numbered run if applicable).
 
     Raises:
         - WorkflowFilesError if the runN symlink is not valid.
         - InputError if the path does not exist.
     """
-    cylc_run_dir = get_cylc_run_dir()
+    cylc_run_dir = get_cylc_run_dir(alt_run_dir)
     try:
         id_ = str(path.relative_to(cylc_run_dir))
     except ValueError:
         raise ValueError(f"{path} is not in the cylc-run directory")
+
     if not path.exists():
         raise InputError(
             f'Workflow ID not found: {id_}\n(Directory not found: {path})'
         )
+
     if path.name == WorkflowFiles.RUN_N:
         runN_path = path
         if warn_runN:
             LOG.warning(
                 f"You do not need to include {WorkflowFiles.RUN_N} in the "
                 "workflow ID; Cylc will select the latest run if just the "
                 "workflow name is used"
```

### Comparing `cylc-flow-8.2.4/cylc/flow/workflow_status.py` & `cylc-flow-8.2.5/cylc/flow/workflow_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from enum import Enum
 from typing import Tuple, TYPE_CHECKING
 
 from cylc.flow.wallclock import get_time_string_from_unix_time as time2str
 
 if TYPE_CHECKING:
+    from optparse import Values
     from cylc.flow.scheduler import Scheduler
 
 # Keys for identify API call
 KEY_GROUP = "group"
 KEY_META = "meta"
 KEY_NAME = "name"
 KEY_OWNER = "owner"
@@ -194,7 +195,25 @@
             WORKFLOW_STATUS_RUNNING_TO_STOP %
             schd.config.final_point)
     else:
         # fallback - running indefinitely
         status_msg = 'running'
 
     return (status.value, status_msg)
+
+
+class RunMode:
+    """The possible run modes of a workflow."""
+
+    LIVE = 'live'
+    """Workflow will run normally."""
+
+    SIMULATION = 'simulation'
+    """Workflow will run in simulation mode."""
+
+    DUMMY = 'dummy'
+    """Workflow will run in dummy mode."""
+
+    @staticmethod
+    def get(options: 'Values') -> str:
+        """Return the run mode from the options."""
+        return getattr(options, 'run_mode', None) or RunMode.LIVE
```

### Comparing `cylc-flow-8.2.4/cylc/flow/xtrigger_mgr.py` & `cylc-flow-8.2.5/cylc/flow/xtrigger_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/xtriggers/__init__.py` & `cylc-flow-8.2.5/cylc/flow/xtriggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/xtriggers/echo.py` & `cylc-flow-8.2.5/cylc/flow/xtriggers/echo.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/xtriggers/wall_clock.py` & `cylc-flow-8.2.5/cylc/flow/xtriggers/wall_clock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc/flow/xtriggers/workflow_state.py` & `cylc-flow-8.2.5/cylc/flow/xtriggers/workflow_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from pathlib import Path
 import sqlite3
 from typing import Dict, Optional, Tuple
 
 from metomi.isodatetime.parsers import TimePointParser
 
 from cylc.flow.cycling.util import add_offset
 from cylc.flow.dbstatecheck import CylcWorkflowDBChecker
-from cylc.flow.pathutil import expand_path, get_cylc_run_dir
-from cylc.flow.workflow_files import infer_latest_run
+from cylc.flow.pathutil import get_cylc_run_dir
+from cylc.flow.workflow_files import infer_latest_run_from_id
 
 
 def workflow_state(
     workflow: str,
     task: str,
     point: str,
     offset: Optional[str] = None,
@@ -54,17 +53,16 @@
         status:
             The task status required for this xtrigger to be satisfied.
         message:
             The custom task output required for this xtrigger to be satisfied.
             .. note::
 
                This cannot be specified in conjunction with ``status``.
-
         cylc_run_dir:
-            The directory in which the workflow to interrogate.
+            Alternate cylc-run directory, e.g. for another user.
 
             .. note::
 
                This only needs to be supplied if the workflow is running in a
                different location to what is specified in the global
                configuration (usually ``~/cylc-run``).
 
@@ -74,21 +72,20 @@
         satisfied:
             True if ``satisfied`` else ``False``.
         results:
             Dictionary containing the args / kwargs which were provided
             to this xtrigger.
 
     """
-    if cylc_run_dir:
-        cylc_run_dir = expand_path(cylc_run_dir)
-    else:
-        cylc_run_dir = get_cylc_run_dir()
+    workflow = infer_latest_run_from_id(workflow, cylc_run_dir)
+    cylc_run_dir = get_cylc_run_dir(cylc_run_dir)
+
     if offset is not None:
         point = str(add_offset(point, offset))
-    _, workflow = infer_latest_run(Path(cylc_run_dir, workflow))
+
     try:
         checker = CylcWorkflowDBChecker(cylc_run_dir, workflow)
     except (OSError, sqlite3.Error):
         # Failed to connect to DB; target workflow may not be started.
         return (False, None)
     try:
         fmt = checker.get_remote_point_format()
```

### Comparing `cylc-flow-8.2.4/cylc/flow/xtriggers/xrandom.py` & `cylc-flow-8.2.5/cylc/flow/xtriggers/xrandom.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc_flow.egg-info/PKG-INFO` & `cylc-flow-8.2.5/cylc_flow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.2.4
+Version: 8.2.5
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
@@ -36,15 +36,15 @@
 Requires-Dist: jinja2==3.0.*
 Requires-Dist: metomi-isodatetime<1!3.2.0,>=1!3.0.0
 Requires-Dist: protobuf<4.22.0,>=4.21.2
 Requires-Dist: psutil>=5.6.0
 Requires-Dist: pyzmq>=22
 Requires-Dist: setuptools!=67.*,>=49
 Requires-Dist: importlib_metadata; python_version < "3.8"
-Requires-Dist: urwid==2.*
+Requires-Dist: urwid!=2.6.2,!=2.6.3,==2.*
 Requires-Dist: rx
 Requires-Dist: promise
 Requires-Dist: tomli>=2; python_version < "3.11"
 Provides-Extra: empy
 Requires-Dist: EmPy==3.3.*; extra == "empy"
 Provides-Extra: graph
 Requires-Dist: pillow; extra == "graph"
@@ -69,15 +69,15 @@
 Requires-Dist: flake8-bugbear>=21.0.0; extra == "tests"
 Requires-Dist: flake8-builtins>=1.5.0; extra == "tests"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "tests"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "tests"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "tests"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "tests"
 Requires-Dist: flake8>=3.0.0; extra == "tests"
-Requires-Dist: mypy>=0.910; extra == "tests"
+Requires-Dist: mypy<1.9,>=0.910; extra == "tests"
 Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "tests"
 Requires-Dist: pytest-cov>=2.8.0; extra == "tests"
 Requires-Dist: pytest-xdist>=2; extra == "tests"
 Requires-Dist: pytest-env>=0.6.2; extra == "tests"
 Requires-Dist: pytest-mock>=3.7; extra == "tests"
 Requires-Dist: pytest>=6; extra == "tests"
 Requires-Dist: testfixtures>=6.11.0; extra == "tests"
@@ -108,15 +108,15 @@
 Requires-Dist: flake8-bugbear>=21.0.0; extra == "all"
 Requires-Dist: flake8-builtins>=1.5.0; extra == "all"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "all"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "all"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "all"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "all"
 Requires-Dist: flake8>=3.0.0; extra == "all"
-Requires-Dist: mypy>=0.910; extra == "all"
+Requires-Dist: mypy<1.9,>=0.910; extra == "all"
 Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "all"
 Requires-Dist: pytest-cov>=2.8.0; extra == "all"
 Requires-Dist: pytest-xdist>=2; extra == "all"
 Requires-Dist: pytest-env>=0.6.2; extra == "all"
 Requires-Dist: pytest-mock>=3.7; extra == "all"
 Requires-Dist: pytest>=6; extra == "all"
 Requires-Dist: testfixtures>=6.11.0; extra == "all"
```

### Comparing `cylc-flow-8.2.4/cylc_flow.egg-info/SOURCES.txt` & `cylc-flow-8.2.5/cylc_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc_flow.egg-info/entry_points.txt` & `cylc-flow-8.2.5/cylc_flow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/cylc_flow.egg-info/requires.txt` & `cylc-flow-8.2.5/cylc_flow.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 graphene<3,>=2.1
 jinja2==3.0.*
 metomi-isodatetime<1!3.2.0,>=1!3.0.0
 protobuf<4.22.0,>=4.21.2
 psutil>=5.6.0
 pyzmq>=22
 setuptools!=67.*,>=49
-urwid==2.*
+urwid!=2.6.2,!=2.6.3,==2.*
 rx
 promise
 
 [:python_version < "3.11"]
 tomli>=2
 
 [:python_version < "3.8"]
@@ -32,15 +32,15 @@
 flake8-bugbear>=21.0.0
 flake8-builtins>=1.5.0
 flake8-comprehensions>=3.5.0
 flake8-debugger>=4.0.0
 flake8-mutable>=1.2.0
 flake8-simplify>=0.14.0
 flake8>=3.0.0
-mypy>=0.910
+mypy<1.9,>=0.910
 pytest-asyncio!=0.23.*,>=0.17
 pytest-cov>=2.8.0
 pytest-xdist>=2
 pytest-env>=0.6.2
 pytest-mock>=3.7
 pytest>=6
 testfixtures>=6.11.0
@@ -84,15 +84,15 @@
 flake8-bugbear>=21.0.0
 flake8-builtins>=1.5.0
 flake8-comprehensions>=3.5.0
 flake8-debugger>=4.0.0
 flake8-mutable>=1.2.0
 flake8-simplify>=0.14.0
 flake8>=3.0.0
-mypy>=0.910
+mypy<1.9,>=0.910
 pytest-asyncio!=0.23.*,>=0.17
 pytest-cov>=2.8.0
 pytest-xdist>=2
 pytest-env>=0.6.2
 pytest-mock>=3.7
 pytest>=6
 testfixtures>=6.11.0
```

### Comparing `cylc-flow-8.2.4/pyproject.toml` & `cylc-flow-8.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.4/setup.cfg` & `cylc-flow-8.2.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 	jinja2==3.0.*
 	metomi-isodatetime>=1!3.0.0,<1!3.2.0
 	protobuf>=4.21.2,<4.22.0
 	psutil>=5.6.0
 	pyzmq>=22
 	setuptools>=49,!=67.*
 	importlib_metadata; python_version < "3.8"
-	urwid==2.*
+	urwid==2.*,!=2.6.2,!=2.6.3
 	rx
 	promise
 	tomli>=2; python_version < "3.11"
 
 [options.packages.find]
 include = cylc*
 
@@ -90,15 +90,15 @@
 	flake8-bugbear>=21.0.0
 	flake8-builtins>=1.5.0
 	flake8-comprehensions>=3.5.0
 	flake8-debugger>=4.0.0
 	flake8-mutable>=1.2.0
 	flake8-simplify>=0.14.0
 	flake8>=3.0.0
-	mypy>=0.910
+	mypy>=0.910,<1.9
 	pytest-asyncio>=0.17,!=0.23.*
 	pytest-cov>=2.8.0
 	pytest-xdist>=2
 	pytest-env>=0.6.2
 	pytest-mock>=3.7
 	pytest>=6
 	testfixtures>=6.11.0
```

### Comparing `cylc-flow-8.2.4/setup.py` & `cylc-flow-8.2.5/setup.py`

 * *Files identical despite different names*

