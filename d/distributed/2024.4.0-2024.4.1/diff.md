# Comparing `tmp/distributed-2024.4.0.tar.gz` & `tmp/distributed-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-2024.4.0.tar", last modified: Mon Apr  1 19:35:18 2024, max compression
+gzip compressed data, was "distributed-2024.4.1.tar", last modified: Thu Apr  4 16:12:06 2024, max compression
```

## Comparing `distributed-2024.4.0.tar` & `distributed-2024.4.1.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.144368 distributed-2024.4.0/
--rw-r--r--   0 james      (501) staff       (20)      104 2023-07-17 19:50:47.000000 distributed-2024.4.0/AUTHORS.md
--rw-r--r--   0 james      (501) staff       (20)     1533 2023-07-17 19:51:10.000000 distributed-2024.4.0/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      633 2023-07-17 19:51:10.000000 distributed-2024.4.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     3344 2024-04-01 19:35:18.144070 distributed-2024.4.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1801 2023-07-17 19:51:10.000000 distributed-2024.4.0/README.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.092669 distributed-2024.4.0/distributed/
--rw-r--r--   0 james      (501) staff       (20)     4265 2024-01-26 22:03:47.000000 distributed-2024.4.0/distributed/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2090 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/_asyncio.py
--rw-r--r--   0 james      (501) staff       (20)     5528 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/_concurrent_futures_thread.py
--rw-r--r--   0 james      (501) staff       (20)     1325 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/_signals.py
--rw-r--r--   0 james      (501) staff       (20)     1459 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/_stories.py
--rw-r--r--   0 james      (501) staff       (20)      500 2024-04-01 19:35:18.144754 distributed-2024.4.0/distributed/_version.py
--rw-r--r--   0 james      (501) staff       (20)    29675 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/active_memory_manager.py
--rw-r--r--   0 james      (501) staff       (20)     9538 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/actor.py
--rw-r--r--   0 james      (501) staff       (20)     7342 2023-09-27 18:27:06.000000 distributed-2024.4.0/distributed/batched.py
--rw-r--r--   0 james      (501) staff       (20)      121 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/bokeh.py
--rw-r--r--   0 james      (501) staff       (20)     5742 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/cfexecutor.py
--rw-r--r--   0 james      (501) staff       (20)     1947 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/chaos.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.095509 distributed-2024.4.0/distributed/cli/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/cli/__init__.py
--rwxr-xr-x   0 james      (501) staff       (20)     7242 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/cli/dask_scheduler.py
--rw-r--r--   0 james      (501) staff       (20)     2104 2023-10-23 15:00:29.000000 distributed-2024.4.0/distributed/cli/dask_spec.py
--rwxr-xr-x   0 james      (501) staff       (20)     5468 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/cli/dask_ssh.py
--rwxr-xr-x   0 james      (501) staff       (20)    16153 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/cli/dask_worker.py
--rw-r--r--   0 james      (501) staff       (20)     1092 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/cli/utils.py
--rw-r--r--   0 james      (501) staff       (20)   213262 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/client.py
--rw-r--r--   0 james      (501) staff       (20)    10995 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/cluster_dump.py
--rw-r--r--   0 james      (501) staff       (20)     7099 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/collections.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.098050 distributed-2024.4.0/distributed/comm/
--rw-r--r--   0 james      (501) staff       (20)      759 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/comm/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     8597 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/comm/addressing.py
--rw-r--r--   0 james      (501) staff       (20)    12721 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/comm/core.py
--rw-r--r--   0 james      (501) staff       (20)    10518 2024-01-26 22:03:47.000000 distributed-2024.4.0/distributed/comm/inproc.py
--rw-r--r--   0 james      (501) staff       (20)     2815 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/comm/registry.py
--rw-r--r--   0 james      (501) staff       (20)    26549 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/comm/tcp.py
--rw-r--r--   0 james      (501) staff       (20)    23014 2023-11-07 17:11:41.000000 distributed-2024.4.0/distributed/comm/ucx.py
--rw-r--r--   0 james      (501) staff       (20)     3758 2023-11-07 17:11:41.000000 distributed-2024.4.0/distributed/comm/utils.py
--rw-r--r--   0 james      (501) staff       (20)    14903 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/comm/ws.py
--rw-r--r--   0 james      (501) staff       (20)    10114 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/compatibility.py
--rw-r--r--   0 james      (501) staff       (20)     7826 2023-09-27 18:27:06.000000 distributed-2024.4.0/distributed/config.py
--rw-r--r--   0 james      (501) staff       (20)    61536 2024-01-26 22:03:47.000000 distributed-2024.4.0/distributed/core.py
--rw-r--r--   0 james      (501) staff       (20)     2134 2023-10-23 15:00:29.000000 distributed-2024.4.0/distributed/counter.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.099918 distributed-2024.4.0/distributed/dashboard/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/dashboard/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.101951 distributed-2024.4.0/distributed/dashboard/components/
--rw-r--r--   0 james      (501) staff       (20)     1550 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/dashboard/components/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5775 2024-04-01 19:12:58.000000 distributed-2024.4.0/distributed/dashboard/components/nvml.py
--rw-r--r--   0 james      (501) staff       (20)     7154 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/dashboard/components/rmm.py
--rw-r--r--   0 james      (501) staff       (20)   162585 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/dashboard/components/scheduler.py
--rw-r--r--   0 james      (501) staff       (20)    19429 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/dashboard/components/shared.py
--rw-r--r--   0 james      (501) staff       (20)    15424 2023-10-27 21:35:57.000000 distributed-2024.4.0/distributed/dashboard/components/worker.py
--rw-r--r--   0 james      (501) staff       (20)     2232 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/dashboard/core.py
--rw-r--r--   0 james      (501) staff       (20)     2313 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/dashboard/export_tool.js
--rw-r--r--   0 james      (501) staff       (20)      763 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/dashboard/export_tool.py
--rw-r--r--   0 james      (501) staff       (20)     5908 2023-11-07 17:11:41.000000 distributed-2024.4.0/distributed/dashboard/scheduler.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.102430 distributed-2024.4.0/distributed/dashboard/templates/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/dashboard/templates/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      241 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/dashboard/templates/performance_report.html
--rw-r--r--   0 james      (501) staff       (20)      199 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/dashboard/theme.yaml
--rw-r--r--   0 james      (501) staff       (20)     1732 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/dashboard/utils.py
--rw-r--r--   0 james      (501) staff       (20)      840 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/dashboard/worker.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.104813 distributed-2024.4.0/distributed/deploy/
--rw-r--r--   0 james      (501) staff       (20)      466 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/deploy/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6702 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/deploy/adaptive.py
--rw-r--r--   0 james      (501) staff       (20)     7895 2023-09-27 18:27:06.000000 distributed-2024.4.0/distributed/deploy/adaptive_core.py
--rw-r--r--   0 james      (501) staff       (20)    21271 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/deploy/cluster.py
--rw-r--r--   0 james      (501) staff       (20)    10452 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/deploy/local.py
--rw-r--r--   0 james      (501) staff       (20)    15514 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/deploy/old_ssh.py
--rw-r--r--   0 james      (501) staff       (20)    23933 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/deploy/spec.py
--rw-r--r--   0 james      (501) staff       (20)    15265 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/deploy/ssh.py
--rw-r--r--   0 james      (501) staff       (20)     8543 2023-12-15 20:02:12.000000 distributed-2024.4.0/distributed/deploy/subprocess.py
--rw-r--r--   0 james      (501) staff       (20)      888 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/deploy/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.108091 distributed-2024.4.0/distributed/diagnostics/
--rw-r--r--   0 james      (501) staff       (20)      221 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1302 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/cluster_dump.py
--rw-r--r--   0 james      (501) staff       (20)      564 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/diagnostics/cudf.py
--rw-r--r--   0 james      (501) staff       (20)     2190 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/eventstream.py
--rw-r--r--   0 james      (501) staff       (20)     5207 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/diagnostics/graph_layout.py
--rw-r--r--   0 james      (501) staff       (20)     7017 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/diagnostics/memory_sampler.py
--rw-r--r--   0 james      (501) staff       (20)     8138 2023-08-21 21:55:47.000000 distributed-2024.4.0/distributed/diagnostics/memray.py
--rw-r--r--   0 james      (501) staff       (20)    10781 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/nvml.py
--rw-r--r--   0 james      (501) staff       (20)    33240 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/diagnostics/plugin.py
--rw-r--r--   0 james      (501) staff       (20)    13904 2023-10-23 15:00:29.000000 distributed-2024.4.0/distributed/diagnostics/progress.py
--rw-r--r--   0 james      (501) staff       (20)     6063 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/progress_stream.py
--rw-r--r--   0 james      (501) staff       (20)    15800 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/diagnostics/progressbar.py
--rw-r--r--   0 james      (501) staff       (20)     1124 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/rmm.py
--rw-r--r--   0 james      (501) staff       (20)     5677 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/diagnostics/task_stream.py
--rw-r--r--   0 james      (501) staff       (20)     2513 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/diagnostics/websocket.py
--rw-r--r--   0 james      (501) staff       (20)     9407 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/diskutils.py
--rw-r--r--   0 james      (501) staff       (20)    48005 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/distributed-schema.yaml
--rw-r--r--   0 james      (501) staff       (20)    15035 2024-03-15 18:22:29.000000 distributed-2024.4.0/distributed/distributed.yaml
--rw-r--r--   0 james      (501) staff       (20)     8536 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/event.py
--rw-r--r--   0 james      (501) staff       (20)      586 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/exceptions.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.109744 distributed-2024.4.0/distributed/http/
--rw-r--r--   0 james      (501) staff       (20)       84 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      273 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/http/health.py
--rw-r--r--   0 james      (501) staff       (20)     1480 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/prometheus.py
--rw-r--r--   0 james      (501) staff       (20)     4925 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/http/proxy.py
--rw-r--r--   0 james      (501) staff       (20)     2548 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/routing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.110715 distributed-2024.4.0/distributed/http/scheduler/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/scheduler/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2914 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/http/scheduler/api.py
--rw-r--r--   0 james      (501) staff       (20)     8359 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/http/scheduler/info.py
--rw-r--r--   0 james      (501) staff       (20)     2159 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/scheduler/json.py
--rw-r--r--   0 james      (501) staff       (20)      625 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/scheduler/missing_bokeh.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.111842 distributed-2024.4.0/distributed/http/scheduler/prometheus/
--rw-r--r--   0 james      (501) staff       (20)      291 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/scheduler/prometheus/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7080 2024-03-15 18:22:29.000000 distributed-2024.4.0/distributed/http/scheduler/prometheus/core.py
--rw-r--r--   0 james      (501) staff       (20)     3514 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/scheduler/prometheus/semaphore.py
--rw-r--r--   0 james      (501) staff       (20)     1617 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/scheduler/prometheus/stealing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.112126 distributed-2024.4.0/distributed/http/static/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.113600 distributed-2024.4.0/distributed/http/static/css/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/css/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2260 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/css/base.css
--rw-r--r--   0 james      (501) staff       (20)      250 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/css/gpu.css
--rw-r--r--   0 james      (501) staff       (20)      840 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/static/css/individual-cluster-map.css
--rw-r--r--   0 james      (501) staff       (20)     1557 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/http/static/css/sortable.min.css
--rw-r--r--   0 james      (501) staff       (20)     1012 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/css/status.css
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.115146 distributed-2024.4.0/distributed/http/static/images/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/dask-logo.svg
--rw-r--r--   0 james      (501) staff       (20)      552 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/static/images/fa-bars.svg
--rw-r--r--   0 james      (501) staff       (20)    15086 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/favicon.ico
--rw-r--r--   0 james      (501) staff       (20)    11002 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/jupyter.svg
--rw-r--r--   0 james      (501) staff       (20)    18663 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/numpy.png
--rw-r--r--   0 james      (501) staff       (20)     1213 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/pandas.png
--rw-r--r--   0 james      (501) staff       (20)   830916 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/images/python.png
--rw-r--r--   0 james      (501) staff       (20)      667 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/static/individual-cluster-map.html
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.118382 distributed-2024.4.0/distributed/http/static/js/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/static/js/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    17271 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/static/js/anime.min.js
--rw-r--r--   0 james      (501) staff       (20)     9337 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/static/js/individual-cluster-map.js
--rw-r--r--   0 james      (501) staff       (20)     3276 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/static/js/reconnecting-websocket.min.js
--rw-r--r--   0 james      (501) staff       (20)     1194 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/http/static/js/sortable.min.js
--rw-r--r--   0 james      (501) staff       (20)      223 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/statics.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.121247 distributed-2024.4.0/distributed/http/templates/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/templates/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2930 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/templates/base.html
--rw-r--r--   0 james      (501) staff       (20)      388 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/templates/call-stack.html
--rw-r--r--   0 james      (501) staff       (20)     1351 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/templates/exceptions.html
--rw-r--r--   0 james      (501) staff       (20)      404 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/templates/gpu.html
--rw-r--r--   0 james      (501) staff       (20)      276 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/templates/json-index.html
--rw-r--r--   0 james      (501) staff       (20)      116 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/templates/logs.html
--rw-r--r--   0 james      (501) staff       (20)      522 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/http/templates/main.html
--rw-r--r--   0 james      (501) staff       (20)       95 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/templates/simple.html
--rw-r--r--   0 james      (501) staff       (20)      635 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/templates/status.html
--rw-r--r--   0 james      (501) staff       (20)     5726 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/http/templates/task.html
--rw-r--r--   0 james      (501) staff       (20)     1601 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/http/templates/worker-table.html
--rw-r--r--   0 james      (501) staff       (20)     2034 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/http/templates/worker.html
--rw-r--r--   0 james      (501) staff       (20)      457 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/templates/workers.html
--rw-r--r--   0 james      (501) staff       (20)     1184 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.121411 distributed-2024.4.0/distributed/http/worker/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.0/distributed/http/worker/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.121686 distributed-2024.4.0/distributed/http/worker/prometheus/
--rw-r--r--   0 james      (501) staff       (20)      288 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/http/worker/prometheus/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    10039 2024-03-15 18:22:29.000000 distributed-2024.4.0/distributed/http/worker/prometheus/core.py
--rw-r--r--   0 james      (501) staff       (20)     1170 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/itertools.py
--rw-r--r--   0 james      (501) staff       (20)     5599 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/lock.py
--rwxr-xr-x   0 james      (501) staff       (20)    14386 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/metrics.py
--rw-r--r--   0 james      (501) staff       (20)     8044 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/multi_lock.py
--rw-r--r--   0 james      (501) staff       (20)    35163 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/nanny.py
--rw-r--r--   0 james      (501) staff       (20)     6710 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/node.py
--rw-r--r--   0 james      (501) staff       (20)     1449 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/objects.py
--rw-r--r--   0 james      (501) staff       (20)     8356 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/preloading.py
--rw-r--r--   0 james      (501) staff       (20)    12887 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/process.py
--rw-r--r--   0 james      (501) staff       (20)      931 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/proctitle.py
--rw-r--r--   0 james      (501) staff       (20)    16996 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/profile.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.126003 distributed-2024.4.0/distributed/protocol/
--rw-r--r--   0 james      (501) staff       (20)     3363 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1336 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/arrow.py
--rw-r--r--   0 james      (501) staff       (20)     6671 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/compression.py
--rw-r--r--   0 james      (501) staff       (20)     6831 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/protocol/core.py
--rw-r--r--   0 james      (501) staff       (20)     1181 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/cuda.py
--rw-r--r--   0 james      (501) staff       (20)     2931 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/cupy.py
--rw-r--r--   0 james      (501) staff       (20)      836 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/h5py.py
--rw-r--r--   0 james      (501) staff       (20)     1127 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/keras.py
--rw-r--r--   0 james      (501) staff       (20)     1466 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/netcdf4.py
--rw-r--r--   0 james      (501) staff       (20)     2139 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/numba.py
--rw-r--r--   0 james      (501) staff       (20)     7030 2024-01-26 22:03:47.000000 distributed-2024.4.0/distributed/protocol/numpy.py
--rw-r--r--   0 james      (501) staff       (20)     3041 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/protocol/pickle.py
--rw-r--r--   0 james      (501) staff       (20)     1507 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/rmm.py
--rw-r--r--   0 james      (501) staff       (20)      792 2024-01-26 22:03:47.000000 distributed-2024.4.0/distributed/protocol/scipy.py
--rw-r--r--   0 james      (501) staff       (20)    29225 2023-12-15 20:02:12.000000 distributed-2024.4.0/distributed/protocol/serialize.py
--rw-r--r--   0 james      (501) staff       (20)      955 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/sparse.py
--rw-r--r--   0 james      (501) staff       (20)     1993 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/protocol/torch.py
--rw-r--r--   0 james      (501) staff       (20)     8314 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/protocol/utils.py
--rw-r--r--   0 james      (501) staff       (20)      795 2023-11-07 17:11:41.000000 distributed-2024.4.0/distributed/protocol/utils_test.py
--rw-r--r--   0 james      (501) staff       (20)     3733 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/publish.py
--rw-r--r--   0 james      (501) staff       (20)    15643 2023-10-23 15:00:29.000000 distributed-2024.4.0/distributed/pubsub.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/py.typed
--rw-r--r--   0 james      (501) staff       (20)    10054 2023-10-23 15:00:29.000000 distributed-2024.4.0/distributed/queues.py
--rw-r--r--   0 james      (501) staff       (20)     7419 2023-09-13 17:55:47.000000 distributed-2024.4.0/distributed/recreate_tasks.py
--rw-r--r--   0 james      (501) staff       (20)   327306 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/scheduler.py
--rw-r--r--   0 james      (501) staff       (20)    13867 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/security.py
--rw-r--r--   0 james      (501) staff       (20)    20568 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/semaphore.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.129721 distributed-2024.4.0/distributed/shuffle/
--rw-r--r--   0 james      (501) staff       (20)      674 2023-08-21 21:39:28.000000 distributed-2024.4.0/distributed/shuffle/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6394 2024-04-01 19:12:58.000000 distributed-2024.4.0/distributed/shuffle/_arrow.py
--rw-r--r--   0 james      (501) staff       (20)     9330 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/shuffle/_buffer.py
--rw-r--r--   0 james      (501) staff       (20)     2481 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/shuffle/_comms.py
--rw-r--r--   0 james      (501) staff       (20)    17734 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/shuffle/_core.py
--rw-r--r--   0 james      (501) staff       (20)     7924 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/shuffle/_disk.py
--rw-r--r--   0 james      (501) staff       (20)      180 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/shuffle/_exceptions.py
--rw-r--r--   0 james      (501) staff       (20)     2798 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/shuffle/_limiter.py
--rw-r--r--   0 james      (501) staff       (20)     1531 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/shuffle/_memory.py
--rw-r--r--   0 james      (501) staff       (20)    14022 2024-03-15 18:22:29.000000 distributed-2024.4.0/distributed/shuffle/_merge.py
--rw-r--r--   0 james      (501) staff       (20)     1186 2023-11-07 17:11:41.000000 distributed-2024.4.0/distributed/shuffle/_pickle.py
--rw-r--r--   0 james      (501) staff       (20)    26857 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/shuffle/_rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    18440 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/shuffle/_scheduler_plugin.py
--rw-r--r--   0 james      (501) staff       (20)    18581 2024-03-15 18:22:29.000000 distributed-2024.4.0/distributed/shuffle/_shuffle.py
--rw-r--r--   0 james      (501) staff       (20)    14591 2024-03-13 20:03:34.000000 distributed-2024.4.0/distributed/shuffle/_worker_plugin.py
--rw-r--r--   0 james      (501) staff       (20)      670 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/sizeof.py
--rw-r--r--   0 james      (501) staff       (20)    23191 2024-01-12 19:19:58.000000 distributed-2024.4.0/distributed/spans.py
--rw-r--r--   0 james      (501) staff       (20)    13767 2023-12-15 20:02:12.000000 distributed-2024.4.0/distributed/spill.py
--rw-r--r--   0 james      (501) staff       (20)    19711 2024-03-15 18:22:29.000000 distributed-2024.4.0/distributed/stealing.py
--rw-r--r--   0 james      (501) staff       (20)     1952 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/system.py
--rw-r--r--   0 james      (501) staff       (20)     8971 2024-04-01 19:12:58.000000 distributed-2024.4.0/distributed/system_monitor.py
--rw-r--r--   0 james      (501) staff       (20)     7104 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/threadpoolexecutor.py
--rw-r--r--   0 james      (501) staff       (20)    58512 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/utils.py
--rw-r--r--   0 james      (501) staff       (20)    14792 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/utils_comm.py
--rw-r--r--   0 james      (501) staff       (20)     8050 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/utils_perf.py
--rw-r--r--   0 james      (501) staff       (20)    83804 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/utils_test.py
--rw-r--r--   0 james      (501) staff       (20)     8411 2023-08-31 20:57:51.000000 distributed-2024.4.0/distributed/variable.py
--rw-r--r--   0 james      (501) staff       (20)     5165 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/versions.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.129899 distributed-2024.4.0/distributed/widgets/
--rw-r--r--   0 james      (501) staff       (20)      267 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.132420 distributed-2024.4.0/distributed/widgets/templates/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2265 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/client.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1589 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/cluster.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1270 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/computation.html.j2
--rw-r--r--   0 james      (501) staff       (20)      518 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/future.html.j2
--rw-r--r--   0 james      (501) staff       (20)      544 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/has_what.html.j2
--rw-r--r--   0 james      (501) staff       (20)      234 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/local_cluster.html.j2
--rw-r--r--   0 james      (501) staff       (20)      636 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/log.html.j2
--rw-r--r--   0 james      (501) staff       (20)      168 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/logs.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1290 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/process_interface.html.j2
--rw-r--r--   0 james      (501) staff       (20)      317 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/scheduler.html.j2
--rw-r--r--   0 james      (501) staff       (20)     6705 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/scheduler_info.html.j2
--rw-r--r--   0 james      (501) staff       (20)      407 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/security.html.j2
--rw-r--r--   0 james      (501) staff       (20)      448 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/task_state.html.j2
--rw-r--r--   0 james      (501) staff       (20)      295 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/who_has.html.j2
--rw-r--r--   0 james      (501) staff       (20)      407 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/widgets/templates/worker_state.html.j2
--rw-r--r--   0 james      (501) staff       (20)   124786 2024-04-01 19:12:54.000000 distributed-2024.4.0/distributed/worker.py
--rw-r--r--   0 james      (501) staff       (20)     2568 2023-07-17 19:51:10.000000 distributed-2024.4.0/distributed/worker_client.py
--rw-r--r--   0 james      (501) staff       (20)    21243 2023-10-13 21:59:50.000000 distributed-2024.4.0/distributed/worker_memory.py
--rw-r--r--   0 james      (501) staff       (20)   142682 2023-12-01 22:10:13.000000 distributed-2024.4.0/distributed/worker_state_machine.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.143738 distributed-2024.4.0/distributed.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     3344 2024-04-01 19:35:18.000000 distributed-2024.4.0/distributed.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     8983 2024-04-01 19:35:18.000000 distributed-2024.4.0/distributed.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-01 19:35:18.000000 distributed-2024.4.0/distributed.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      335 2024-04-01 19:35:18.000000 distributed-2024.4.0/distributed.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-01 19:35:17.000000 distributed-2024.4.0/distributed.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      227 2024-04-01 19:35:18.000000 distributed-2024.4.0/distributed.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2024-04-01 19:35:18.000000 distributed-2024.4.0/distributed.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.068858 distributed-2024.4.0/docs/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.143230 distributed-2024.4.0/docs/source/
--rw-r--r--   0 james      (501) staff       (20)    11754 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/active_memory_manager.rst
--rw-r--r--   0 james      (501) staff       (20)     8000 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/actors.rst
--rw-r--r--   0 james      (501) staff       (20)     4343 2023-08-21 21:55:47.000000 distributed-2024.4.0/docs/source/api.rst
--rw-r--r--   0 james      (501) staff       (20)     3519 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/asynchronous.rst
--rw-r--r--   0 james      (501) staff       (20)   275148 2023-10-13 22:40:21.000000 distributed-2024.4.0/docs/source/changelog.rst
--rw-r--r--   0 james      (501) staff       (20)     7137 2023-08-21 21:39:28.000000 distributed-2024.4.0/docs/source/client.rst
--rw-r--r--   0 james      (501) staff       (20)     3770 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/communications.rst
--rw-r--r--   0 james      (501) staff       (20)     7049 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/develop.rst
--rw-r--r--   0 james      (501) staff       (20)     6823 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/diagnosing-performance.rst
--rw-r--r--   0 james      (501) staff       (20)     3392 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/efficiency.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-01 19:35:18.143394 distributed-2024.4.0/docs/source/examples/
--rw-r--r--   0 james      (501) staff       (20)     8953 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/examples/word-count.rst
--rw-r--r--   0 james      (501) staff       (20)       75 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/examples-overview.rst
--rw-r--r--   0 james      (501) staff       (20)     4228 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/faq.rst
--rw-r--r--   0 james      (501) staff       (20)     9303 2023-08-21 21:39:28.000000 distributed-2024.4.0/docs/source/fine-performance-metrics.rst
--rw-r--r--   0 james      (501) staff       (20)     4613 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/foundations.rst
--rw-r--r--   0 james      (501) staff       (20)     4016 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/http_services.rst
--rw-r--r--   0 james      (501) staff       (20)     4460 2023-08-21 21:39:28.000000 distributed-2024.4.0/docs/source/index.rst
--rw-r--r--   0 james      (501) staff       (20)     1182 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/install.rst
--rw-r--r--   0 james      (501) staff       (20)     7293 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/journey.rst
--rw-r--r--   0 james      (501) staff       (20)     6470 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/killed.rst
--rw-r--r--   0 james      (501) staff       (20)     1828 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/limitations.rst
--rw-r--r--   0 james      (501) staff       (20)     6458 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/locality.rst
--rw-r--r--   0 james      (501) staff       (20)     2807 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/logging.rst
--rw-r--r--   0 james      (501) staff       (20)     6546 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/manage-computation.rst
--rw-r--r--   0 james      (501) staff       (20)     8550 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/memory.rst
--rw-r--r--   0 james      (501) staff       (20)     4282 2023-12-01 22:10:13.000000 distributed-2024.4.0/docs/source/plugins.rst
--rw-r--r--   0 james      (501) staff       (20)     3265 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/priority.rst
--rw-r--r--   0 james      (501) staff       (20)     7800 2024-03-15 18:22:29.000000 distributed-2024.4.0/docs/source/prometheus.rst
--rw-r--r--   0 james      (501) staff       (20)    11199 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/protocol.rst
--rw-r--r--   0 james      (501) staff       (20)     3107 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/publish.rst
--rw-r--r--   0 james      (501) staff       (20)      402 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/queues.rst
--rw-r--r--   0 james      (501) staff       (20)     2942 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/quickstart.rst
--rw-r--r--   0 james      (501) staff       (20)     8773 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/related-work.rst
--rw-r--r--   0 james      (501) staff       (20)     3418 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/resilience.rst
--rw-r--r--   0 james      (501) staff       (20)     7021 2024-04-01 19:12:58.000000 distributed-2024.4.0/docs/source/resources.rst
--rw-r--r--   0 james      (501) staff       (20)    16084 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/scheduling-policies.rst
--rw-r--r--   0 james      (501) staff       (20)    16893 2023-08-31 20:57:51.000000 distributed-2024.4.0/docs/source/scheduling-state.rst
--rw-r--r--   0 james      (501) staff       (20)     6518 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/serialization.rst
--rw-r--r--   0 james      (501) staff       (20)     5463 2024-04-01 19:12:58.000000 distributed-2024.4.0/docs/source/spans.rst
--rw-r--r--   0 james      (501) staff       (20)     8343 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/task-launch.rst
--rw-r--r--   0 james      (501) staff       (20)     4190 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/tls.rst
--rw-r--r--   0 james      (501) staff       (20)     5557 2023-07-17 19:50:47.000000 distributed-2024.4.0/docs/source/work-stealing.rst
--rw-r--r--   0 james      (501) staff       (20)    13489 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/worker-memory.rst
--rw-r--r--   0 james      (501) staff       (20)    22542 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/worker-state.rst
--rw-r--r--   0 james      (501) staff       (20)     3467 2023-07-17 19:51:10.000000 distributed-2024.4.0/docs/source/worker.rst
--rw-r--r--   0 james      (501) staff       (20)    10199 2024-04-01 19:28:50.000000 distributed-2024.4.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2024-04-01 19:35:18.144446 distributed-2024.4.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      171 2023-07-17 19:51:10.000000 distributed-2024.4.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.674318 distributed-2024.4.1/
+-rw-r--r--   0 james      (501) staff       (20)      104 2023-07-17 19:50:47.000000 distributed-2024.4.1/AUTHORS.md
+-rw-r--r--   0 james      (501) staff       (20)     1533 2023-07-17 19:51:10.000000 distributed-2024.4.1/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      633 2023-07-17 19:51:10.000000 distributed-2024.4.1/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     3344 2024-04-04 16:12:06.674019 distributed-2024.4.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1801 2023-07-17 19:51:10.000000 distributed-2024.4.1/README.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.610854 distributed-2024.4.1/distributed/
+-rw-r--r--   0 james      (501) staff       (20)     4265 2024-01-26 22:03:47.000000 distributed-2024.4.1/distributed/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2090 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/_asyncio.py
+-rw-r--r--   0 james      (501) staff       (20)     5528 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/_concurrent_futures_thread.py
+-rw-r--r--   0 james      (501) staff       (20)     1325 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/_signals.py
+-rw-r--r--   0 james      (501) staff       (20)     1459 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/_stories.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2024-04-04 16:12:06.674579 distributed-2024.4.1/distributed/_version.py
+-rw-r--r--   0 james      (501) staff       (20)    29675 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/active_memory_manager.py
+-rw-r--r--   0 james      (501) staff       (20)     9538 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/actor.py
+-rw-r--r--   0 james      (501) staff       (20)     7342 2023-09-27 18:27:06.000000 distributed-2024.4.1/distributed/batched.py
+-rw-r--r--   0 james      (501) staff       (20)      121 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/bokeh.py
+-rw-r--r--   0 james      (501) staff       (20)     5742 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/cfexecutor.py
+-rw-r--r--   0 james      (501) staff       (20)     1947 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/chaos.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.614580 distributed-2024.4.1/distributed/cli/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/cli/__init__.py
+-rwxr-xr-x   0 james      (501) staff       (20)     7242 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/cli/dask_scheduler.py
+-rw-r--r--   0 james      (501) staff       (20)     2104 2023-10-23 15:00:29.000000 distributed-2024.4.1/distributed/cli/dask_spec.py
+-rwxr-xr-x   0 james      (501) staff       (20)     5468 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/cli/dask_ssh.py
+-rwxr-xr-x   0 james      (501) staff       (20)    16153 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/cli/dask_worker.py
+-rw-r--r--   0 james      (501) staff       (20)     1092 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/cli/utils.py
+-rw-r--r--   0 james      (501) staff       (20)   213262 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/client.py
+-rw-r--r--   0 james      (501) staff       (20)    10995 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/cluster_dump.py
+-rw-r--r--   0 james      (501) staff       (20)     7099 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/collections.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.617660 distributed-2024.4.1/distributed/comm/
+-rw-r--r--   0 james      (501) staff       (20)      759 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/comm/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     8597 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/comm/addressing.py
+-rw-r--r--   0 james      (501) staff       (20)    12721 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/comm/core.py
+-rw-r--r--   0 james      (501) staff       (20)    10518 2024-01-26 22:03:47.000000 distributed-2024.4.1/distributed/comm/inproc.py
+-rw-r--r--   0 james      (501) staff       (20)     2815 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/comm/registry.py
+-rw-r--r--   0 james      (501) staff       (20)    26549 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/comm/tcp.py
+-rw-r--r--   0 james      (501) staff       (20)    23014 2023-11-07 17:11:41.000000 distributed-2024.4.1/distributed/comm/ucx.py
+-rw-r--r--   0 james      (501) staff       (20)     3758 2023-11-07 17:11:41.000000 distributed-2024.4.1/distributed/comm/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    14903 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/comm/ws.py
+-rw-r--r--   0 james      (501) staff       (20)    10114 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)     7826 2023-09-27 18:27:06.000000 distributed-2024.4.1/distributed/config.py
+-rw-r--r--   0 james      (501) staff       (20)    61536 2024-01-26 22:03:47.000000 distributed-2024.4.1/distributed/core.py
+-rw-r--r--   0 james      (501) staff       (20)     2134 2023-10-23 15:00:29.000000 distributed-2024.4.1/distributed/counter.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.620067 distributed-2024.4.1/distributed/dashboard/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/dashboard/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.622702 distributed-2024.4.1/distributed/dashboard/components/
+-rw-r--r--   0 james      (501) staff       (20)     1550 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/dashboard/components/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5775 2024-04-01 19:12:58.000000 distributed-2024.4.1/distributed/dashboard/components/nvml.py
+-rw-r--r--   0 james      (501) staff       (20)     7154 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/dashboard/components/rmm.py
+-rw-r--r--   0 james      (501) staff       (20)   162585 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/dashboard/components/scheduler.py
+-rw-r--r--   0 james      (501) staff       (20)    19429 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/dashboard/components/shared.py
+-rw-r--r--   0 james      (501) staff       (20)    15424 2023-10-27 21:35:57.000000 distributed-2024.4.1/distributed/dashboard/components/worker.py
+-rw-r--r--   0 james      (501) staff       (20)     2232 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/dashboard/core.py
+-rw-r--r--   0 james      (501) staff       (20)     2313 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/dashboard/export_tool.js
+-rw-r--r--   0 james      (501) staff       (20)      763 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/dashboard/export_tool.py
+-rw-r--r--   0 james      (501) staff       (20)     5908 2023-11-07 17:11:41.000000 distributed-2024.4.1/distributed/dashboard/scheduler.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.623268 distributed-2024.4.1/distributed/dashboard/templates/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/dashboard/templates/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      241 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/dashboard/templates/performance_report.html
+-rw-r--r--   0 james      (501) staff       (20)      199 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/dashboard/theme.yaml
+-rw-r--r--   0 james      (501) staff       (20)     1732 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/dashboard/utils.py
+-rw-r--r--   0 james      (501) staff       (20)      840 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/dashboard/worker.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.627429 distributed-2024.4.1/distributed/deploy/
+-rw-r--r--   0 james      (501) staff       (20)      466 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/deploy/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6702 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/deploy/adaptive.py
+-rw-r--r--   0 james      (501) staff       (20)     7895 2023-09-27 18:27:06.000000 distributed-2024.4.1/distributed/deploy/adaptive_core.py
+-rw-r--r--   0 james      (501) staff       (20)    21271 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/deploy/cluster.py
+-rw-r--r--   0 james      (501) staff       (20)    10452 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/deploy/local.py
+-rw-r--r--   0 james      (501) staff       (20)    15514 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/deploy/old_ssh.py
+-rw-r--r--   0 james      (501) staff       (20)    23933 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/deploy/spec.py
+-rw-r--r--   0 james      (501) staff       (20)    15265 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/deploy/ssh.py
+-rw-r--r--   0 james      (501) staff       (20)     8543 2023-12-15 20:02:12.000000 distributed-2024.4.1/distributed/deploy/subprocess.py
+-rw-r--r--   0 james      (501) staff       (20)      888 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/deploy/utils.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.631464 distributed-2024.4.1/distributed/diagnostics/
+-rw-r--r--   0 james      (501) staff       (20)      221 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1302 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/cluster_dump.py
+-rw-r--r--   0 james      (501) staff       (20)      564 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/diagnostics/cudf.py
+-rw-r--r--   0 james      (501) staff       (20)     2190 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/eventstream.py
+-rw-r--r--   0 james      (501) staff       (20)     5207 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/diagnostics/graph_layout.py
+-rw-r--r--   0 james      (501) staff       (20)     7017 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/diagnostics/memory_sampler.py
+-rw-r--r--   0 james      (501) staff       (20)     8138 2023-08-21 21:55:47.000000 distributed-2024.4.1/distributed/diagnostics/memray.py
+-rw-r--r--   0 james      (501) staff       (20)    10781 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/nvml.py
+-rw-r--r--   0 james      (501) staff       (20)    33240 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/diagnostics/plugin.py
+-rw-r--r--   0 james      (501) staff       (20)    13904 2023-10-23 15:00:29.000000 distributed-2024.4.1/distributed/diagnostics/progress.py
+-rw-r--r--   0 james      (501) staff       (20)     6063 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/progress_stream.py
+-rw-r--r--   0 james      (501) staff       (20)    15800 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/diagnostics/progressbar.py
+-rw-r--r--   0 james      (501) staff       (20)     1124 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/rmm.py
+-rw-r--r--   0 james      (501) staff       (20)     5677 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/diagnostics/task_stream.py
+-rw-r--r--   0 james      (501) staff       (20)     2513 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/diagnostics/websocket.py
+-rw-r--r--   0 james      (501) staff       (20)     9407 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/diskutils.py
+-rw-r--r--   0 james      (501) staff       (20)    48005 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/distributed-schema.yaml
+-rw-r--r--   0 james      (501) staff       (20)    15035 2024-03-15 18:22:29.000000 distributed-2024.4.1/distributed/distributed.yaml
+-rw-r--r--   0 james      (501) staff       (20)     8536 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/event.py
+-rw-r--r--   0 james      (501) staff       (20)      586 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/exceptions.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.633395 distributed-2024.4.1/distributed/http/
+-rw-r--r--   0 james      (501) staff       (20)       84 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      273 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/http/health.py
+-rw-r--r--   0 james      (501) staff       (20)     1480 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/prometheus.py
+-rw-r--r--   0 james      (501) staff       (20)     4925 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/http/proxy.py
+-rw-r--r--   0 james      (501) staff       (20)     2548 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/routing.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.634591 distributed-2024.4.1/distributed/http/scheduler/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/scheduler/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2914 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/http/scheduler/api.py
+-rw-r--r--   0 james      (501) staff       (20)     8359 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/http/scheduler/info.py
+-rw-r--r--   0 james      (501) staff       (20)     2159 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/scheduler/json.py
+-rw-r--r--   0 james      (501) staff       (20)      625 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/scheduler/missing_bokeh.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.635560 distributed-2024.4.1/distributed/http/scheduler/prometheus/
+-rw-r--r--   0 james      (501) staff       (20)      291 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/scheduler/prometheus/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7080 2024-03-15 18:22:29.000000 distributed-2024.4.1/distributed/http/scheduler/prometheus/core.py
+-rw-r--r--   0 james      (501) staff       (20)     3514 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/scheduler/prometheus/semaphore.py
+-rw-r--r--   0 james      (501) staff       (20)     1617 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/scheduler/prometheus/stealing.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.635944 distributed-2024.4.1/distributed/http/static/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.637262 distributed-2024.4.1/distributed/http/static/css/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/css/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2260 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/css/base.css
+-rw-r--r--   0 james      (501) staff       (20)      250 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/css/gpu.css
+-rw-r--r--   0 james      (501) staff       (20)      840 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/static/css/individual-cluster-map.css
+-rw-r--r--   0 james      (501) staff       (20)     1557 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/http/static/css/sortable.min.css
+-rw-r--r--   0 james      (501) staff       (20)     1012 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/css/status.css
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.638913 distributed-2024.4.1/distributed/http/static/images/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1607 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/dask-logo.svg
+-rw-r--r--   0 james      (501) staff       (20)      552 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/static/images/fa-bars.svg
+-rw-r--r--   0 james      (501) staff       (20)    15086 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/favicon.ico
+-rw-r--r--   0 james      (501) staff       (20)    11002 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/jupyter.svg
+-rw-r--r--   0 james      (501) staff       (20)    18663 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/numpy.png
+-rw-r--r--   0 james      (501) staff       (20)     1213 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/pandas.png
+-rw-r--r--   0 james      (501) staff       (20)   830916 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/images/python.png
+-rw-r--r--   0 james      (501) staff       (20)      667 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/static/individual-cluster-map.html
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.640983 distributed-2024.4.1/distributed/http/static/js/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/static/js/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    17271 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/static/js/anime.min.js
+-rw-r--r--   0 james      (501) staff       (20)     9337 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/static/js/individual-cluster-map.js
+-rw-r--r--   0 james      (501) staff       (20)     3276 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/static/js/reconnecting-websocket.min.js
+-rw-r--r--   0 james      (501) staff       (20)     1194 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/http/static/js/sortable.min.js
+-rw-r--r--   0 james      (501) staff       (20)      223 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/statics.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.644864 distributed-2024.4.1/distributed/http/templates/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/templates/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2930 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/templates/base.html
+-rw-r--r--   0 james      (501) staff       (20)      388 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/templates/call-stack.html
+-rw-r--r--   0 james      (501) staff       (20)     1351 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/templates/exceptions.html
+-rw-r--r--   0 james      (501) staff       (20)      404 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/templates/gpu.html
+-rw-r--r--   0 james      (501) staff       (20)      276 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/templates/json-index.html
+-rw-r--r--   0 james      (501) staff       (20)      116 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/templates/logs.html
+-rw-r--r--   0 james      (501) staff       (20)      522 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/http/templates/main.html
+-rw-r--r--   0 james      (501) staff       (20)       95 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/templates/simple.html
+-rw-r--r--   0 james      (501) staff       (20)      635 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/templates/status.html
+-rw-r--r--   0 james      (501) staff       (20)     5726 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/http/templates/task.html
+-rw-r--r--   0 james      (501) staff       (20)     1601 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/http/templates/worker-table.html
+-rw-r--r--   0 james      (501) staff       (20)     2034 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/http/templates/worker.html
+-rw-r--r--   0 james      (501) staff       (20)      457 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/templates/workers.html
+-rw-r--r--   0 james      (501) staff       (20)     1184 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/utils.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.645061 distributed-2024.4.1/distributed/http/worker/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:50:47.000000 distributed-2024.4.1/distributed/http/worker/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.645366 distributed-2024.4.1/distributed/http/worker/prometheus/
+-rw-r--r--   0 james      (501) staff       (20)      288 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/http/worker/prometheus/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    10039 2024-03-15 18:22:29.000000 distributed-2024.4.1/distributed/http/worker/prometheus/core.py
+-rw-r--r--   0 james      (501) staff       (20)     1170 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/itertools.py
+-rw-r--r--   0 james      (501) staff       (20)     5599 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/lock.py
+-rwxr-xr-x   0 james      (501) staff       (20)    14386 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/metrics.py
+-rw-r--r--   0 james      (501) staff       (20)     8044 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/multi_lock.py
+-rw-r--r--   0 james      (501) staff       (20)    35163 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/nanny.py
+-rw-r--r--   0 james      (501) staff       (20)     6710 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/node.py
+-rw-r--r--   0 james      (501) staff       (20)     1449 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/objects.py
+-rw-r--r--   0 james      (501) staff       (20)     8356 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/preloading.py
+-rw-r--r--   0 james      (501) staff       (20)    12887 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/process.py
+-rw-r--r--   0 james      (501) staff       (20)      931 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/proctitle.py
+-rw-r--r--   0 james      (501) staff       (20)    16996 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/profile.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.649883 distributed-2024.4.1/distributed/protocol/
+-rw-r--r--   0 james      (501) staff       (20)     3363 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1336 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)     6671 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/compression.py
+-rw-r--r--   0 james      (501) staff       (20)     6831 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/protocol/core.py
+-rw-r--r--   0 james      (501) staff       (20)     1181 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/cuda.py
+-rw-r--r--   0 james      (501) staff       (20)     2931 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/cupy.py
+-rw-r--r--   0 james      (501) staff       (20)      836 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/h5py.py
+-rw-r--r--   0 james      (501) staff       (20)     1127 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/keras.py
+-rw-r--r--   0 james      (501) staff       (20)     1466 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/netcdf4.py
+-rw-r--r--   0 james      (501) staff       (20)     2139 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/numba.py
+-rw-r--r--   0 james      (501) staff       (20)     7030 2024-01-26 22:03:47.000000 distributed-2024.4.1/distributed/protocol/numpy.py
+-rw-r--r--   0 james      (501) staff       (20)     3041 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/protocol/pickle.py
+-rw-r--r--   0 james      (501) staff       (20)     1507 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/rmm.py
+-rw-r--r--   0 james      (501) staff       (20)      792 2024-01-26 22:03:47.000000 distributed-2024.4.1/distributed/protocol/scipy.py
+-rw-r--r--   0 james      (501) staff       (20)    29538 2024-04-04 15:04:51.000000 distributed-2024.4.1/distributed/protocol/serialize.py
+-rw-r--r--   0 james      (501) staff       (20)      955 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     1993 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/protocol/torch.py
+-rw-r--r--   0 james      (501) staff       (20)     8314 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/protocol/utils.py
+-rw-r--r--   0 james      (501) staff       (20)      795 2023-11-07 17:11:41.000000 distributed-2024.4.1/distributed/protocol/utils_test.py
+-rw-r--r--   0 james      (501) staff       (20)     3733 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/publish.py
+-rw-r--r--   0 james      (501) staff       (20)    15643 2023-10-23 15:00:29.000000 distributed-2024.4.1/distributed/pubsub.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/py.typed
+-rw-r--r--   0 james      (501) staff       (20)    10054 2023-10-23 15:00:29.000000 distributed-2024.4.1/distributed/queues.py
+-rw-r--r--   0 james      (501) staff       (20)     7419 2023-09-13 17:55:47.000000 distributed-2024.4.1/distributed/recreate_tasks.py
+-rw-r--r--   0 james      (501) staff       (20)   327306 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/scheduler.py
+-rw-r--r--   0 james      (501) staff       (20)    13867 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/security.py
+-rw-r--r--   0 james      (501) staff       (20)    20568 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/semaphore.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.654347 distributed-2024.4.1/distributed/shuffle/
+-rw-r--r--   0 james      (501) staff       (20)      674 2023-08-21 21:39:28.000000 distributed-2024.4.1/distributed/shuffle/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6394 2024-04-01 19:12:58.000000 distributed-2024.4.1/distributed/shuffle/_arrow.py
+-rw-r--r--   0 james      (501) staff       (20)     9330 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/shuffle/_buffer.py
+-rw-r--r--   0 james      (501) staff       (20)     2481 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/shuffle/_comms.py
+-rw-r--r--   0 james      (501) staff       (20)    17734 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/shuffle/_core.py
+-rw-r--r--   0 james      (501) staff       (20)     7924 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/shuffle/_disk.py
+-rw-r--r--   0 james      (501) staff       (20)      180 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/shuffle/_exceptions.py
+-rw-r--r--   0 james      (501) staff       (20)     2798 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/shuffle/_limiter.py
+-rw-r--r--   0 james      (501) staff       (20)     1531 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/shuffle/_memory.py
+-rw-r--r--   0 james      (501) staff       (20)    14022 2024-03-15 18:22:29.000000 distributed-2024.4.1/distributed/shuffle/_merge.py
+-rw-r--r--   0 james      (501) staff       (20)     1186 2023-11-07 17:11:41.000000 distributed-2024.4.1/distributed/shuffle/_pickle.py
+-rw-r--r--   0 james      (501) staff       (20)    26857 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/shuffle/_rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    18440 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/shuffle/_scheduler_plugin.py
+-rw-r--r--   0 james      (501) staff       (20)    18581 2024-03-15 18:22:29.000000 distributed-2024.4.1/distributed/shuffle/_shuffle.py
+-rw-r--r--   0 james      (501) staff       (20)    14591 2024-03-13 20:03:34.000000 distributed-2024.4.1/distributed/shuffle/_worker_plugin.py
+-rw-r--r--   0 james      (501) staff       (20)      670 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)    23191 2024-01-12 19:19:58.000000 distributed-2024.4.1/distributed/spans.py
+-rw-r--r--   0 james      (501) staff       (20)    13767 2023-12-15 20:02:12.000000 distributed-2024.4.1/distributed/spill.py
+-rw-r--r--   0 james      (501) staff       (20)    19711 2024-03-15 18:22:29.000000 distributed-2024.4.1/distributed/stealing.py
+-rw-r--r--   0 james      (501) staff       (20)     1952 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/system.py
+-rw-r--r--   0 james      (501) staff       (20)     8971 2024-04-01 19:12:58.000000 distributed-2024.4.1/distributed/system_monitor.py
+-rw-r--r--   0 james      (501) staff       (20)     7104 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/threadpoolexecutor.py
+-rw-r--r--   0 james      (501) staff       (20)    58512 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    14792 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/utils_comm.py
+-rw-r--r--   0 james      (501) staff       (20)     8050 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/utils_perf.py
+-rw-r--r--   0 james      (501) staff       (20)    83804 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/utils_test.py
+-rw-r--r--   0 james      (501) staff       (20)     8411 2023-08-31 20:57:51.000000 distributed-2024.4.1/distributed/variable.py
+-rw-r--r--   0 james      (501) staff       (20)     5165 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/versions.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.654636 distributed-2024.4.1/distributed/widgets/
+-rw-r--r--   0 james      (501) staff       (20)      267 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.658772 distributed-2024.4.1/distributed/widgets/templates/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2265 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/client.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1589 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/cluster.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1270 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/computation.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      518 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/future.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      544 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/has_what.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      234 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/local_cluster.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      636 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/log.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      168 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/logs.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1290 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/process_interface.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      317 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/scheduler.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     6705 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/scheduler_info.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      407 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/security.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      448 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/task_state.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      295 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/who_has.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      407 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/widgets/templates/worker_state.html.j2
+-rw-r--r--   0 james      (501) staff       (20)   124786 2024-04-01 19:12:54.000000 distributed-2024.4.1/distributed/worker.py
+-rw-r--r--   0 james      (501) staff       (20)     2568 2023-07-17 19:51:10.000000 distributed-2024.4.1/distributed/worker_client.py
+-rw-r--r--   0 james      (501) staff       (20)    21243 2023-10-13 21:59:50.000000 distributed-2024.4.1/distributed/worker_memory.py
+-rw-r--r--   0 james      (501) staff       (20)   142682 2023-12-01 22:10:13.000000 distributed-2024.4.1/distributed/worker_state_machine.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.673650 distributed-2024.4.1/distributed.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     3344 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     8983 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      335 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      227 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2024-04-04 16:12:06.000000 distributed-2024.4.1/distributed.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.583912 distributed-2024.4.1/docs/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.673105 distributed-2024.4.1/docs/source/
+-rw-r--r--   0 james      (501) staff       (20)    11754 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/active_memory_manager.rst
+-rw-r--r--   0 james      (501) staff       (20)     8000 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/actors.rst
+-rw-r--r--   0 james      (501) staff       (20)     4343 2023-08-21 21:55:47.000000 distributed-2024.4.1/docs/source/api.rst
+-rw-r--r--   0 james      (501) staff       (20)     3519 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/asynchronous.rst
+-rw-r--r--   0 james      (501) staff       (20)   275148 2023-10-13 22:40:21.000000 distributed-2024.4.1/docs/source/changelog.rst
+-rw-r--r--   0 james      (501) staff       (20)     7137 2023-08-21 21:39:28.000000 distributed-2024.4.1/docs/source/client.rst
+-rw-r--r--   0 james      (501) staff       (20)     3770 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/communications.rst
+-rw-r--r--   0 james      (501) staff       (20)     7049 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/develop.rst
+-rw-r--r--   0 james      (501) staff       (20)     6823 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/diagnosing-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)     3392 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/efficiency.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-04 16:12:06.673304 distributed-2024.4.1/docs/source/examples/
+-rw-r--r--   0 james      (501) staff       (20)     8953 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/examples/word-count.rst
+-rw-r--r--   0 james      (501) staff       (20)       75 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/examples-overview.rst
+-rw-r--r--   0 james      (501) staff       (20)     4228 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/faq.rst
+-rw-r--r--   0 james      (501) staff       (20)     9303 2023-08-21 21:39:28.000000 distributed-2024.4.1/docs/source/fine-performance-metrics.rst
+-rw-r--r--   0 james      (501) staff       (20)     4613 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/foundations.rst
+-rw-r--r--   0 james      (501) staff       (20)     4016 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/http_services.rst
+-rw-r--r--   0 james      (501) staff       (20)     4460 2023-08-21 21:39:28.000000 distributed-2024.4.1/docs/source/index.rst
+-rw-r--r--   0 james      (501) staff       (20)     1182 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/install.rst
+-rw-r--r--   0 james      (501) staff       (20)     7293 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/journey.rst
+-rw-r--r--   0 james      (501) staff       (20)     6470 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/killed.rst
+-rw-r--r--   0 james      (501) staff       (20)     1828 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/limitations.rst
+-rw-r--r--   0 james      (501) staff       (20)     6458 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/locality.rst
+-rw-r--r--   0 james      (501) staff       (20)     2807 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/logging.rst
+-rw-r--r--   0 james      (501) staff       (20)     6546 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/manage-computation.rst
+-rw-r--r--   0 james      (501) staff       (20)     8550 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/memory.rst
+-rw-r--r--   0 james      (501) staff       (20)     4282 2023-12-01 22:10:13.000000 distributed-2024.4.1/docs/source/plugins.rst
+-rw-r--r--   0 james      (501) staff       (20)     3265 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/priority.rst
+-rw-r--r--   0 james      (501) staff       (20)     7800 2024-03-15 18:22:29.000000 distributed-2024.4.1/docs/source/prometheus.rst
+-rw-r--r--   0 james      (501) staff       (20)    11199 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/protocol.rst
+-rw-r--r--   0 james      (501) staff       (20)     3107 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/publish.rst
+-rw-r--r--   0 james      (501) staff       (20)      402 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/queues.rst
+-rw-r--r--   0 james      (501) staff       (20)     2942 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/quickstart.rst
+-rw-r--r--   0 james      (501) staff       (20)     8773 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/related-work.rst
+-rw-r--r--   0 james      (501) staff       (20)     3418 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/resilience.rst
+-rw-r--r--   0 james      (501) staff       (20)     7021 2024-04-01 19:12:58.000000 distributed-2024.4.1/docs/source/resources.rst
+-rw-r--r--   0 james      (501) staff       (20)    16084 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/scheduling-policies.rst
+-rw-r--r--   0 james      (501) staff       (20)    16893 2023-08-31 20:57:51.000000 distributed-2024.4.1/docs/source/scheduling-state.rst
+-rw-r--r--   0 james      (501) staff       (20)     6518 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/serialization.rst
+-rw-r--r--   0 james      (501) staff       (20)     5463 2024-04-01 19:12:58.000000 distributed-2024.4.1/docs/source/spans.rst
+-rw-r--r--   0 james      (501) staff       (20)     8343 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/task-launch.rst
+-rw-r--r--   0 james      (501) staff       (20)     4190 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/tls.rst
+-rw-r--r--   0 james      (501) staff       (20)     5557 2023-07-17 19:50:47.000000 distributed-2024.4.1/docs/source/work-stealing.rst
+-rw-r--r--   0 james      (501) staff       (20)    13489 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/worker-memory.rst
+-rw-r--r--   0 james      (501) staff       (20)    22542 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/worker-state.rst
+-rw-r--r--   0 james      (501) staff       (20)     3467 2023-07-17 19:51:10.000000 distributed-2024.4.1/docs/source/worker.rst
+-rw-r--r--   0 james      (501) staff       (20)    10199 2024-04-04 16:08:24.000000 distributed-2024.4.1/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-04-04 16:12:06.674385 distributed-2024.4.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)      171 2023-07-17 19:51:10.000000 distributed-2024.4.1/setup.py
```

### Comparing `distributed-2024.4.0/LICENSE.txt` & `distributed-2024.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/MANIFEST.in` & `distributed-2024.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/PKG-INFO` & `distributed-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distributed
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Distributed scheduler for Dask
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://distributed.dask.org
 Project-URL: Source, https://github.com/dask/distributed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 Requires-Dist: click>=8.0
 Requires-Dist: cloudpickle>=1.5.0
-Requires-Dist: dask==2024.4.0
+Requires-Dist: dask==2024.4.1
 Requires-Dist: jinja2>=2.10.3
 Requires-Dist: locket>=1.0.0
 Requires-Dist: msgpack>=1.0.0
 Requires-Dist: packaging>=20.0
 Requires-Dist: psutil>=5.7.2
 Requires-Dist: pyyaml>=5.3.1
 Requires-Dist: sortedcontainers>=2.0.5
```

### Comparing `distributed-2024.4.0/README.rst` & `distributed-2024.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/__init__.py` & `distributed-2024.4.1/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/_asyncio.py` & `distributed-2024.4.1/distributed/_asyncio.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/_concurrent_futures_thread.py` & `distributed-2024.4.1/distributed/_concurrent_futures_thread.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/_signals.py` & `distributed-2024.4.1/distributed/_signals.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/_stories.py` & `distributed-2024.4.1/distributed/_stories.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/active_memory_manager.py` & `distributed-2024.4.1/distributed/active_memory_manager.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/actor.py` & `distributed-2024.4.1/distributed/actor.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/batched.py` & `distributed-2024.4.1/distributed/batched.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cfexecutor.py` & `distributed-2024.4.1/distributed/cfexecutor.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/chaos.py` & `distributed-2024.4.1/distributed/chaos.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cli/dask_scheduler.py` & `distributed-2024.4.1/distributed/cli/dask_scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cli/dask_spec.py` & `distributed-2024.4.1/distributed/cli/dask_spec.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cli/dask_ssh.py` & `distributed-2024.4.1/distributed/cli/dask_ssh.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cli/dask_worker.py` & `distributed-2024.4.1/distributed/cli/dask_worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cli/utils.py` & `distributed-2024.4.1/distributed/cli/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/client.py` & `distributed-2024.4.1/distributed/client.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/cluster_dump.py` & `distributed-2024.4.1/distributed/cluster_dump.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/collections.py` & `distributed-2024.4.1/distributed/collections.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/__init__.py` & `distributed-2024.4.1/distributed/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/addressing.py` & `distributed-2024.4.1/distributed/comm/addressing.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/core.py` & `distributed-2024.4.1/distributed/comm/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/inproc.py` & `distributed-2024.4.1/distributed/comm/inproc.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/registry.py` & `distributed-2024.4.1/distributed/comm/registry.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/tcp.py` & `distributed-2024.4.1/distributed/comm/tcp.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/ucx.py` & `distributed-2024.4.1/distributed/comm/ucx.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/utils.py` & `distributed-2024.4.1/distributed/comm/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/comm/ws.py` & `distributed-2024.4.1/distributed/comm/ws.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/compatibility.py` & `distributed-2024.4.1/distributed/compatibility.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/config.py` & `distributed-2024.4.1/distributed/config.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/core.py` & `distributed-2024.4.1/distributed/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/counter.py` & `distributed-2024.4.1/distributed/counter.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/components/__init__.py` & `distributed-2024.4.1/distributed/dashboard/components/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/components/nvml.py` & `distributed-2024.4.1/distributed/dashboard/components/nvml.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/components/rmm.py` & `distributed-2024.4.1/distributed/dashboard/components/rmm.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/components/scheduler.py` & `distributed-2024.4.1/distributed/dashboard/components/scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/components/shared.py` & `distributed-2024.4.1/distributed/dashboard/components/shared.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/components/worker.py` & `distributed-2024.4.1/distributed/dashboard/components/worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/core.py` & `distributed-2024.4.1/distributed/dashboard/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/export_tool.js` & `distributed-2024.4.1/distributed/dashboard/export_tool.js`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/export_tool.py` & `distributed-2024.4.1/distributed/dashboard/export_tool.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/scheduler.py` & `distributed-2024.4.1/distributed/dashboard/scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/utils.py` & `distributed-2024.4.1/distributed/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/dashboard/worker.py` & `distributed-2024.4.1/distributed/dashboard/worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/adaptive.py` & `distributed-2024.4.1/distributed/deploy/adaptive.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/adaptive_core.py` & `distributed-2024.4.1/distributed/deploy/adaptive_core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/cluster.py` & `distributed-2024.4.1/distributed/deploy/cluster.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/local.py` & `distributed-2024.4.1/distributed/deploy/local.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/old_ssh.py` & `distributed-2024.4.1/distributed/deploy/old_ssh.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/spec.py` & `distributed-2024.4.1/distributed/deploy/spec.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/ssh.py` & `distributed-2024.4.1/distributed/deploy/ssh.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/subprocess.py` & `distributed-2024.4.1/distributed/deploy/subprocess.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/deploy/utils.py` & `distributed-2024.4.1/distributed/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/cluster_dump.py` & `distributed-2024.4.1/distributed/diagnostics/cluster_dump.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/cudf.py` & `distributed-2024.4.1/distributed/diagnostics/cudf.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/eventstream.py` & `distributed-2024.4.1/distributed/diagnostics/eventstream.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/graph_layout.py` & `distributed-2024.4.1/distributed/diagnostics/graph_layout.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/memory_sampler.py` & `distributed-2024.4.1/distributed/diagnostics/memory_sampler.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/memray.py` & `distributed-2024.4.1/distributed/diagnostics/memray.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/nvml.py` & `distributed-2024.4.1/distributed/diagnostics/nvml.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/plugin.py` & `distributed-2024.4.1/distributed/diagnostics/plugin.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/progress.py` & `distributed-2024.4.1/distributed/diagnostics/progress.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/progress_stream.py` & `distributed-2024.4.1/distributed/diagnostics/progress_stream.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/progressbar.py` & `distributed-2024.4.1/distributed/diagnostics/progressbar.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/rmm.py` & `distributed-2024.4.1/distributed/diagnostics/rmm.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/task_stream.py` & `distributed-2024.4.1/distributed/diagnostics/task_stream.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diagnostics/websocket.py` & `distributed-2024.4.1/distributed/diagnostics/websocket.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/diskutils.py` & `distributed-2024.4.1/distributed/diskutils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/distributed-schema.yaml` & `distributed-2024.4.1/distributed/distributed-schema.yaml`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/distributed.yaml` & `distributed-2024.4.1/distributed/distributed.yaml`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/event.py` & `distributed-2024.4.1/distributed/event.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/exceptions.py` & `distributed-2024.4.1/distributed/exceptions.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/prometheus.py` & `distributed-2024.4.1/distributed/http/prometheus.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/proxy.py` & `distributed-2024.4.1/distributed/http/proxy.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/routing.py` & `distributed-2024.4.1/distributed/http/routing.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/api.py` & `distributed-2024.4.1/distributed/http/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/info.py` & `distributed-2024.4.1/distributed/http/scheduler/info.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/json.py` & `distributed-2024.4.1/distributed/http/scheduler/json.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/missing_bokeh.py` & `distributed-2024.4.1/distributed/http/scheduler/missing_bokeh.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/prometheus/core.py` & `distributed-2024.4.1/distributed/http/scheduler/prometheus/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/prometheus/semaphore.py` & `distributed-2024.4.1/distributed/http/scheduler/prometheus/semaphore.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/scheduler/prometheus/stealing.py` & `distributed-2024.4.1/distributed/http/scheduler/prometheus/stealing.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/css/base.css` & `distributed-2024.4.1/distributed/http/static/css/base.css`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/css/individual-cluster-map.css` & `distributed-2024.4.1/distributed/http/static/css/individual-cluster-map.css`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/css/sortable.min.css` & `distributed-2024.4.1/distributed/http/static/css/sortable.min.css`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/css/status.css` & `distributed-2024.4.1/distributed/http/static/css/status.css`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/dask-logo.svg` & `distributed-2024.4.1/distributed/http/static/images/dask-logo.svg`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/fa-bars.svg` & `distributed-2024.4.1/distributed/http/static/images/fa-bars.svg`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/favicon.ico` & `distributed-2024.4.1/distributed/http/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/jupyter.svg` & `distributed-2024.4.1/distributed/http/static/images/jupyter.svg`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/numpy.png` & `distributed-2024.4.1/distributed/http/static/images/numpy.png`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/pandas.png` & `distributed-2024.4.1/distributed/http/static/images/pandas.png`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/images/python.png` & `distributed-2024.4.1/distributed/http/static/images/python.png`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/individual-cluster-map.html` & `distributed-2024.4.1/distributed/http/static/individual-cluster-map.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/js/anime.min.js` & `distributed-2024.4.1/distributed/http/static/js/anime.min.js`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/js/individual-cluster-map.js` & `distributed-2024.4.1/distributed/http/static/js/individual-cluster-map.js`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/js/reconnecting-websocket.min.js` & `distributed-2024.4.1/distributed/http/static/js/reconnecting-websocket.min.js`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/static/js/sortable.min.js` & `distributed-2024.4.1/distributed/http/static/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/base.html` & `distributed-2024.4.1/distributed/http/templates/base.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/exceptions.html` & `distributed-2024.4.1/distributed/http/templates/exceptions.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/main.html` & `distributed-2024.4.1/distributed/http/templates/main.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/status.html` & `distributed-2024.4.1/distributed/http/templates/status.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/task.html` & `distributed-2024.4.1/distributed/http/templates/task.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/worker-table.html` & `distributed-2024.4.1/distributed/http/templates/worker-table.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/templates/worker.html` & `distributed-2024.4.1/distributed/http/templates/worker.html`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/utils.py` & `distributed-2024.4.1/distributed/http/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/http/worker/prometheus/core.py` & `distributed-2024.4.1/distributed/http/worker/prometheus/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/itertools.py` & `distributed-2024.4.1/distributed/itertools.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/lock.py` & `distributed-2024.4.1/distributed/lock.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/metrics.py` & `distributed-2024.4.1/distributed/metrics.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/multi_lock.py` & `distributed-2024.4.1/distributed/multi_lock.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/nanny.py` & `distributed-2024.4.1/distributed/nanny.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/node.py` & `distributed-2024.4.1/distributed/node.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/objects.py` & `distributed-2024.4.1/distributed/objects.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/preloading.py` & `distributed-2024.4.1/distributed/preloading.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/process.py` & `distributed-2024.4.1/distributed/process.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/proctitle.py` & `distributed-2024.4.1/distributed/proctitle.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/profile.py` & `distributed-2024.4.1/distributed/profile.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/__init__.py` & `distributed-2024.4.1/distributed/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/arrow.py` & `distributed-2024.4.1/distributed/protocol/arrow.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/compression.py` & `distributed-2024.4.1/distributed/protocol/compression.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/core.py` & `distributed-2024.4.1/distributed/protocol/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/cuda.py` & `distributed-2024.4.1/distributed/protocol/cuda.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/cupy.py` & `distributed-2024.4.1/distributed/protocol/cupy.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/h5py.py` & `distributed-2024.4.1/distributed/protocol/h5py.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/keras.py` & `distributed-2024.4.1/distributed/protocol/keras.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/netcdf4.py` & `distributed-2024.4.1/distributed/protocol/netcdf4.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/numba.py` & `distributed-2024.4.1/distributed/protocol/numba.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/numpy.py` & `distributed-2024.4.1/distributed/protocol/numpy.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/pickle.py` & `distributed-2024.4.1/distributed/protocol/pickle.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/rmm.py` & `distributed-2024.4.1/distributed/protocol/rmm.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/scipy.py` & `distributed-2024.4.1/distributed/protocol/scipy.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/serialize.py` & `distributed-2024.4.1/distributed/protocol/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import codecs
 import importlib
 import traceback
 from array import array
 from enum import Enum
 from functools import partial
+from pickle import PickleBuffer
 from types import ModuleType
 from typing import Any, Generic, Literal, TypeVar
 
 import msgpack
 
 import dask
 from dask.base import normalize_token
@@ -82,27 +83,35 @@
         "serializer": "pickle",
         "writeable": tuple(writeable),
     }
 
     return header, frames
 
 
-def pickle_loads(header, frames):
-    x, buffers = frames[0], frames[1:]
-
-    writeable = header.get("writeable")
-    if not writeable:
-        writeable = len(buffers) * (None,)
+def pickle_loads(
+    header: dict[str, Any], frames: list[bytes | bytearray | memoryview | PickleBuffer]
+) -> Any:
+    pik, buffers = frames[0], frames[1:]
+
+    def ensure_writeable_flag(mv: memoryview, w: bool) -> memoryview:
+        if w and mv.readonly:
+            # Can't avoid a deep copy
+            return memoryview(bytearray(mv))
+        elif not w and not mv.readonly:
+            # Zero copy - this is just a flag
+            return mv.toreadonly()
+        else:
+            return mv
 
     buffers = [
-        memoryview(bytearray(mv) if w else bytes(mv)) if w == mv.readonly else mv
-        for w, mv in zip(writeable, map(ensure_memoryview, buffers))
+        ensure_writeable_flag(ensure_memoryview(mv), w)
+        for mv, w in zip(buffers, header["writeable"])
     ]
 
-    return pickle.loads(x, buffers=buffers)
+    return pickle.loads(pik, buffers=buffers)
 
 
 def import_allowed_module(name):
     if name in _cached_allowed_modules:
         return _cached_allowed_modules[name]
 
     # Check for non-ASCII characters
```

### Comparing `distributed-2024.4.0/distributed/protocol/sparse.py` & `distributed-2024.4.1/distributed/protocol/sparse.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/torch.py` & `distributed-2024.4.1/distributed/protocol/torch.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/utils.py` & `distributed-2024.4.1/distributed/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/protocol/utils_test.py` & `distributed-2024.4.1/distributed/protocol/utils_test.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/publish.py` & `distributed-2024.4.1/distributed/publish.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/pubsub.py` & `distributed-2024.4.1/distributed/pubsub.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/queues.py` & `distributed-2024.4.1/distributed/queues.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/recreate_tasks.py` & `distributed-2024.4.1/distributed/recreate_tasks.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/scheduler.py` & `distributed-2024.4.1/distributed/scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/security.py` & `distributed-2024.4.1/distributed/security.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/semaphore.py` & `distributed-2024.4.1/distributed/semaphore.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/__init__.py` & `distributed-2024.4.1/distributed/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_arrow.py` & `distributed-2024.4.1/distributed/shuffle/_arrow.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_buffer.py` & `distributed-2024.4.1/distributed/shuffle/_buffer.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_comms.py` & `distributed-2024.4.1/distributed/shuffle/_comms.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_core.py` & `distributed-2024.4.1/distributed/shuffle/_core.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_disk.py` & `distributed-2024.4.1/distributed/shuffle/_disk.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_limiter.py` & `distributed-2024.4.1/distributed/shuffle/_limiter.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_memory.py` & `distributed-2024.4.1/distributed/shuffle/_memory.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_merge.py` & `distributed-2024.4.1/distributed/shuffle/_merge.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_pickle.py` & `distributed-2024.4.1/distributed/shuffle/_pickle.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_rechunk.py` & `distributed-2024.4.1/distributed/shuffle/_rechunk.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_scheduler_plugin.py` & `distributed-2024.4.1/distributed/shuffle/_scheduler_plugin.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_shuffle.py` & `distributed-2024.4.1/distributed/shuffle/_shuffle.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/shuffle/_worker_plugin.py` & `distributed-2024.4.1/distributed/shuffle/_worker_plugin.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/sizeof.py` & `distributed-2024.4.1/distributed/sizeof.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/spans.py` & `distributed-2024.4.1/distributed/spans.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/spill.py` & `distributed-2024.4.1/distributed/spill.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/stealing.py` & `distributed-2024.4.1/distributed/stealing.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/system.py` & `distributed-2024.4.1/distributed/system.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/system_monitor.py` & `distributed-2024.4.1/distributed/system_monitor.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/threadpoolexecutor.py` & `distributed-2024.4.1/distributed/threadpoolexecutor.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/utils.py` & `distributed-2024.4.1/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/utils_comm.py` & `distributed-2024.4.1/distributed/utils_comm.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/utils_perf.py` & `distributed-2024.4.1/distributed/utils_perf.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/utils_test.py` & `distributed-2024.4.1/distributed/utils_test.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/variable.py` & `distributed-2024.4.1/distributed/variable.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/versions.py` & `distributed-2024.4.1/distributed/versions.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/client.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/client.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/cluster.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/cluster.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/computation.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/computation.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/future.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/future.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/has_what.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/has_what.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/log.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/log.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/process_interface.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/process_interface.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/widgets/templates/scheduler_info.html.j2` & `distributed-2024.4.1/distributed/widgets/templates/scheduler_info.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/worker.py` & `distributed-2024.4.1/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/worker_client.py` & `distributed-2024.4.1/distributed/worker_client.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/worker_memory.py` & `distributed-2024.4.1/distributed/worker_memory.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed/worker_state_machine.py` & `distributed-2024.4.1/distributed/worker_state_machine.py`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/distributed.egg-info/PKG-INFO` & `distributed-2024.4.1/distributed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distributed
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Distributed scheduler for Dask
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://distributed.dask.org
 Project-URL: Source, https://github.com/dask/distributed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.md
 Requires-Dist: click>=8.0
 Requires-Dist: cloudpickle>=1.5.0
-Requires-Dist: dask==2024.4.0
+Requires-Dist: dask==2024.4.1
 Requires-Dist: jinja2>=2.10.3
 Requires-Dist: locket>=1.0.0
 Requires-Dist: msgpack>=1.0.0
 Requires-Dist: packaging>=20.0
 Requires-Dist: psutil>=5.7.2
 Requires-Dist: pyyaml>=5.3.1
 Requires-Dist: sortedcontainers>=2.0.5
```

### Comparing `distributed-2024.4.0/distributed.egg-info/SOURCES.txt` & `distributed-2024.4.1/distributed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/active_memory_manager.rst` & `distributed-2024.4.1/docs/source/active_memory_manager.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/actors.rst` & `distributed-2024.4.1/docs/source/actors.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/api.rst` & `distributed-2024.4.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/asynchronous.rst` & `distributed-2024.4.1/docs/source/asynchronous.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/changelog.rst` & `distributed-2024.4.1/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/client.rst` & `distributed-2024.4.1/docs/source/client.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/communications.rst` & `distributed-2024.4.1/docs/source/communications.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/develop.rst` & `distributed-2024.4.1/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/diagnosing-performance.rst` & `distributed-2024.4.1/docs/source/diagnosing-performance.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/efficiency.rst` & `distributed-2024.4.1/docs/source/efficiency.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/examples/word-count.rst` & `distributed-2024.4.1/docs/source/examples/word-count.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/faq.rst` & `distributed-2024.4.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/fine-performance-metrics.rst` & `distributed-2024.4.1/docs/source/fine-performance-metrics.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/foundations.rst` & `distributed-2024.4.1/docs/source/foundations.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/http_services.rst` & `distributed-2024.4.1/docs/source/http_services.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/index.rst` & `distributed-2024.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/install.rst` & `distributed-2024.4.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/journey.rst` & `distributed-2024.4.1/docs/source/journey.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/killed.rst` & `distributed-2024.4.1/docs/source/killed.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/limitations.rst` & `distributed-2024.4.1/docs/source/limitations.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/locality.rst` & `distributed-2024.4.1/docs/source/locality.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/logging.rst` & `distributed-2024.4.1/docs/source/logging.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/manage-computation.rst` & `distributed-2024.4.1/docs/source/manage-computation.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/memory.rst` & `distributed-2024.4.1/docs/source/memory.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/plugins.rst` & `distributed-2024.4.1/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/priority.rst` & `distributed-2024.4.1/docs/source/priority.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/prometheus.rst` & `distributed-2024.4.1/docs/source/prometheus.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/protocol.rst` & `distributed-2024.4.1/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/publish.rst` & `distributed-2024.4.1/docs/source/publish.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/quickstart.rst` & `distributed-2024.4.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/related-work.rst` & `distributed-2024.4.1/docs/source/related-work.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/resilience.rst` & `distributed-2024.4.1/docs/source/resilience.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/resources.rst` & `distributed-2024.4.1/docs/source/resources.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/scheduling-policies.rst` & `distributed-2024.4.1/docs/source/scheduling-policies.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/scheduling-state.rst` & `distributed-2024.4.1/docs/source/scheduling-state.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/serialization.rst` & `distributed-2024.4.1/docs/source/serialization.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/spans.rst` & `distributed-2024.4.1/docs/source/spans.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/task-launch.rst` & `distributed-2024.4.1/docs/source/task-launch.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/tls.rst` & `distributed-2024.4.1/docs/source/tls.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/work-stealing.rst` & `distributed-2024.4.1/docs/source/work-stealing.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/worker-memory.rst` & `distributed-2024.4.1/docs/source/worker-memory.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/worker-state.rst` & `distributed-2024.4.1/docs/source/worker-state.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/docs/source/worker.rst` & `distributed-2024.4.1/docs/source/worker.rst`

 * *Files identical despite different names*

### Comparing `distributed-2024.4.0/pyproject.toml` & `distributed-2024.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: System :: Distributed Computing",
 ]
 readme = "README.rst"
 requires-python = ">=3.9"
 dependencies = [
     "click >= 8.0",
     "cloudpickle >= 1.5.0",
-    "dask == 2024.4.0",
+    "dask == 2024.4.1",
     "jinja2 >= 2.10.3",
     "locket >= 1.0.0",
     "msgpack >= 1.0.0",
     "packaging >= 20.0",
     "psutil >= 5.7.2",
     "pyyaml >= 5.3.1",
     "sortedcontainers >= 2.0.5",
```

