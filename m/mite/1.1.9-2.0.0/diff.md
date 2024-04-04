# Comparing `tmp/mite-1.1.9.tar.gz` & `tmp/mite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mite-1.1.9.tar", last modified: Mon Dec 11 11:45:42 2023, max compression
+gzip compressed data, was "mite-2.0.0.tar", last modified: Thu Apr  4 11:04:09 2024, max compression
```

## Comparing `mite-1.1.9.tar` & `mite-2.0.0.tar`

### file list

```diff
@@ -1,178 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.822695 mite-1.1.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.794695 mite-1.1.9/.circleci/
--rw-r--r--   0 root         (0) root         (0)     5548 2023-12-11 11:45:28.000000 mite-1.1.9/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      233 2023-12-11 11:45:28.000000 mite-1.1.9/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.794695 mite-1.1.9/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.794695 mite-1.1.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      479 2023-12-11 11:45:28.000000 mite-1.1.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      604 2023-12-11 11:45:28.000000 mite-1.1.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 root         (0) root         (0)      115 2023-12-11 11:45:28.000000 mite-1.1.9/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1212 2023-12-11 11:45:28.000000 mite-1.1.9/.gitignore
--rw-r--r--   0 root         (0) root         (0)      138 2023-12-11 11:45:28.000000 mite-1.1.9/.isort.cfg
--rw-r--r--   0 root         (0) root         (0)      332 2023-12-11 11:45:28.000000 mite-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      696 2023-12-11 11:45:28.000000 mite-1.1.9/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     3230 2023-12-11 11:45:28.000000 mite-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     3929 2023-12-11 11:45:28.000000 mite-1.1.9/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     3082 2023-12-11 11:45:28.000000 mite-1.1.9/DEV.md
--rw-r--r--   0 root         (0) root         (0)     1444 2023-12-11 11:45:28.000000 mite-1.1.9/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      307 2023-12-11 11:45:28.000000 mite-1.1.9/Dockerfile.perftest
--rw-r--r--   0 root         (0) root         (0)     1100 2023-12-11 11:45:28.000000 mite-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       12 2023-12-11 11:45:28.000000 mite-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9827 2023-12-11 11:45:42.822695 mite-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8770 2023-12-11 11:45:28.000000 mite-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.794695 mite-1.1.9/cd-scripts/
--rwxr-xr-x   0 root         (0) root         (0)      526 2023-12-11 11:45:28.000000 mite-1.1.9/cd-scripts/cdBuild-1.sh
--rw-r--r--   0 root         (0) root         (0)     4138 2023-12-11 11:45:28.000000 mite-1.1.9/cd-scripts/cdRelease.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-12-11 11:45:28.000000 mite-1.1.9/cd.yml
--rw-r--r--   0 root         (0) root         (0)      103 2023-12-11 11:45:28.000000 mite-1.1.9/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1624 2023-12-11 11:45:28.000000 mite-1.1.9/docker_compose.yml
--rw-r--r--   0 root         (0) root         (0)      698 2023-12-11 11:45:28.000000 mite-1.1.9/docker_compose_monitoring.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.798695 mite-1.1.9/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-12-11 11:45:28.000000 mite-1.1.9/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     6220 2023-12-11 11:45:28.000000 mite-1.1.9/docs/components.rst
--rw-r--r--   0 root         (0) root         (0)     2165 2023-12-11 11:45:28.000000 mite-1.1.9/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-12-11 11:45:28.000000 mite-1.1.9/docs/config.rst
--rw-r--r--   0 root         (0) root         (0)     7835 2023-12-11 11:45:28.000000 mite-1.1.9/docs/design-deployment.rst
--rw-r--r--   0 root         (0) root         (0)      945 2023-12-11 11:45:28.000000 mite-1.1.9/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     3908 2023-12-11 11:45:28.000000 mite-1.1.9/docs/journeys.rst
--rw-r--r--   0 root         (0) root         (0)      168 2023-12-11 11:45:28.000000 mite-1.1.9/docs/notes.txt
--rw-r--r--   0 root         (0) root         (0)     2324 2023-12-11 11:45:28.000000 mite-1.1.9/docs/prometheus.rst
--rw-r--r--   0 root         (0) root         (0)     6507 2023-12-11 11:45:28.000000 mite-1.1.9/docs/stats.rst
--rw-r--r--   0 root         (0) root         (0)     1717 2023-12-11 11:45:28.000000 mite-1.1.9/docs/volume-model.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.798695 mite-1.1.9/grafana/
--rw-r--r--   0 root         (0) root         (0)      129 2023-12-11 11:45:28.000000 mite-1.1.9/grafana/Dockerfile
--rw-r--r--   0 root         (0) root         (0)       77 2023-12-11 11:45:28.000000 mite-1.1.9/grafana/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.778696 mite-1.1.9/grafana/provisioning/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.798695 mite-1.1.9/grafana/provisioning/dashboards/
--rw-r--r--   0 root         (0) root         (0)      145 2023-12-11 11:45:28.000000 mite-1.1.9/grafana/provisioning/dashboards/dashboards.yml
--rw-r--r--   0 root         (0) root         (0)    27978 2023-12-11 11:45:28.000000 mite-1.1.9/grafana/provisioning/dashboards/grafana_dashboard_template.json
--rw-r--r--   0 root         (0) root         (0)    28427 2023-12-11 11:45:28.000000 mite-1.1.9/grafana/provisioning/dashboards/mite_docker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.798695 mite-1.1.9/grafana/provisioning/datasources/
--rw-r--r--   0 root         (0) root         (0)      180 2023-12-11 11:45:28.000000 mite-1.1.9/grafana/provisioning/datasources/datasources.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.798695 mite-1.1.9/local/
--rw-r--r--   0 root         (0) root         (0)      628 2023-12-11 11:45:28.000000 mite-1.1.9/local/Makefile
--rw-r--r--   0 root         (0) root         (0)     1349 2023-12-11 11:45:28.000000 mite-1.1.9/local/README.md
--rw-r--r--   0 root         (0) root         (0)      678 2023-12-11 11:45:28.000000 mite-1.1.9/local/demo.py
--rwxr-xr-x   0 root         (0) root         (0)     1024 2023-12-11 11:45:28.000000 mite-1.1.9/local/run_mite.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.802695 mite-1.1.9/mite/
--rwxr-xr-x   0 root         (0) root         (0)     2353 2023-12-11 11:45:28.000000 mite-1.1.9/mite/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    15198 2023-12-11 11:45:28.000000 mite-1.1.9/mite/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.802695 mite-1.1.9/mite/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/cat.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/collector.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/common.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/duplicator.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/receiver.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/stats.py
--rw-r--r--   0 root         (0) root         (0)     6560 2023-12-11 11:45:28.000000 mite-1.1.9/mite/cli/test.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-12-11 11:45:28.000000 mite-1.1.9/mite/collector.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-12-11 11:45:28.000000 mite-1.1.9/mite/config.py
--rwxr-xr-x   0 root         (0) root         (0)     4815 2023-12-11 11:45:28.000000 mite-1.1.9/mite/context.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-12-11 11:45:28.000000 mite-1.1.9/mite/controller.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-12-11 11:45:28.000000 mite-1.1.9/mite/datapools.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-12-11 11:45:28.000000 mite-1.1.9/mite/example.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-12-11 11:45:28.000000 mite-1.1.9/mite/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-12-11 11:45:28.000000 mite-1.1.9/mite/har_to_mite.py
--rw-r--r--   0 root         (0) root         (0)     4804 2023-12-11 11:45:28.000000 mite-1.1.9/mite/logoutput.py
--rwxr-xr-x   0 root         (0) root         (0)     4591 2023-12-11 11:45:28.000000 mite-1.1.9/mite/nanomsg.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-12-11 11:45:28.000000 mite-1.1.9/mite/recorder.py
--rwxr-xr-x   0 root         (0) root         (0)     6986 2023-12-11 11:45:28.000000 mite-1.1.9/mite/runner.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-12-11 11:45:28.000000 mite-1.1.9/mite/scenario.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-12-11 11:45:28.000000 mite-1.1.9/mite/stats.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-12-11 11:45:28.000000 mite-1.1.9/mite/test.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-12-11 11:45:28.000000 mite-1.1.9/mite/utils.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-12-11 11:45:28.000000 mite-1.1.9/mite/volume_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.802695 mite-1.1.9/mite/web/
--rw-r--r--   0 root         (0) root         (0)      469 2023-12-11 11:45:28.000000 mite-1.1.9/mite/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3559 2023-12-11 11:45:28.000000 mite-1.1.9/mite/web/prometheus.py
--rwxr-xr-x   0 root         (0) root         (0)     6247 2023-12-11 11:45:28.000000 mite-1.1.9/mite/zmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.822695 mite-1.1.9/mite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9827 2023-12-11 11:45:42.000000 mite-1.1.9/mite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3460 2023-12-11 11:45:42.000000 mite-1.1.9/mite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-11 11:45:42.000000 mite-1.1.9/mite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-12-11 11:45:42.000000 mite-1.1.9/mite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-12-11 11:45:42.000000 mite-1.1.9/mite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-12-11 11:45:42.000000 mite-1.1.9/mite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.802695 mite-1.1.9/mite_amqp/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-12-11 11:45:28.000000 mite-1.1.9/mite_amqp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_browser/
--rwxr-xr-x   0 root         (0) root         (0)    17442 2023-12-11 11:45:28.000000 mite-1.1.9/mite_browser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_finagle/
--rw-r--r--   0 root         (0) root         (0)     8329 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/README.md
--rw-r--r--   0 root         (0) root         (0)     6504 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11258 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/mux.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_finagle/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_finagle/tests/foo_service/
--rwxr-xr-x   0 root         (0) root         (0)     2698 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/foo_service/Foo-remote
--rw-r--r--   0 root         (0) root         (0)     7560 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/foo_service/Foo.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/foo_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)      366 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/foo_service/constants.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/foo_service/ttypes.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/foo_service.thrift
--rw-r--r--   0 root         (0) root         (0)     3503 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     4738 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/test_mux.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/tests/test_thrift.py
--rw-r--r--   0 root         (0) root         (0)     9650 2023-12-11 11:45:28.000000 mite-1.1.9/mite_finagle/thrift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_http/
--rw-r--r--   0 root         (0) root         (0)     2964 2023-12-11 11:45:28.000000 mite-1.1.9/mite_http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-12-11 11:45:28.000000 mite-1.1.9/mite_http/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_selenium/
--rw-r--r--   0 root         (0) root         (0)    11427 2023-12-11 11:45:28.000000 mite-1.1.9/mite_selenium/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-12-11 11:45:28.000000 mite-1.1.9/mite_selenium/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/mite_websocket/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-12-11 11:45:28.000000 mite-1.1.9/mite_websocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.806695 mite-1.1.9/prometheus/
--rw-r--r--   0 root         (0) root         (0)      188 2023-12-11 11:45:28.000000 mite-1.1.9/prometheus/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      206 2023-12-11 11:45:28.000000 mite-1.1.9/prometheus/prometheus_config_docker.yml
--rw-r--r--   0 root         (0) root         (0)      136 2023-12-11 11:45:28.000000 mite-1.1.9/prometheus/prometheus_config_template.yml
--rw-r--r--   0 root         (0) root         (0)      165 2023-12-11 11:45:28.000000 mite-1.1.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       70 2023-12-11 11:45:28.000000 mite-1.1.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-12-11 11:45:42.822695 mite-1.1.9/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      114 2023-12-11 11:45:28.000000 mite-1.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.822695 mite-1.1.9/test/
--rw-r--r--   0 root         (0) root         (0)      124 2023-12-11 11:45:28.000000 mite-1.1.9/test/legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.822695 mite-1.1.9/test/mocks/
--rw-r--r--   0 root         (0) root         (0)      272 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_collector.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_context.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_direct_receiver.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_direct_runner_transport.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_recorder_msg_http.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_selenium.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-12-11 11:45:28.000000 mite-1.1.9/test/mocks/mock_sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-11 11:45:42.822695 mite-1.1.9/test/perf/
--rw-r--r--   0 root         (0) root         (0)        9 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1677 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/http_server.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/http_server_aiohttp.py
--rw-r--r--   0 root         (0) root         (0)      817 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/mite_perftest.py
--rwxr-xr-x   0 root         (0) root         (0)     4625 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/perftest.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/run-perftest.sh
--rw-r--r--   0 root         (0) root         (0)       35 2023-12-11 11:45:28.000000 mite-1.1.9/test/perf/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0) 10236043 2023-12-11 11:45:28.000000 mite-1.1.9/test/test.har
--rw-r--r--   0 root         (0) root         (0)     5240 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_collector.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_context.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_controller.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_datapools.py
--rw-r--r--   0 root         (0) root         (0)     7712 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_har_to_mite.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_mite_amqp.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_mite_browser.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_mite_http.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_mite_utils.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_mite_websockets.py
--rw-r--r--   0 root         (0) root         (0)     4015 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_prometheus_mite.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_recorder.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_runner_tracker.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_scenario.py
--rw-r--r--   0 root         (0) root         (0)     5867 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_stats.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_volume_model.py
--rw-r--r--   0 root         (0) root         (0)     8670 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_webdriver.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-12-11 11:45:28.000000 mite-1.1.9/test/test_work_tracker.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-12-11 11:45:28.000000 mite-1.1.9/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0) 10236043 2023-12-11 11:45:28.000000 mite-1.1.9/test.har
--rw-r--r--   0 root         (0) root         (0)     1860 2023-12-11 11:45:28.000000 mite-1.1.9/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.902150 mite-2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     5548 2024-04-04 11:04:01.000000 mite-2.0.0/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      233 2024-04-04 11:04:01.000000 mite-2.0.0/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-04 11:04:01.000000 mite-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-04 11:04:01.000000 mite-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 root         (0) root         (0)      115 2024-04-04 11:04:01.000000 mite-2.0.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-04 11:04:01.000000 mite-2.0.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-04 11:04:01.000000 mite-2.0.0/.isort.cfg
+-rw-r--r--   0 root         (0) root         (0)      332 2024-04-04 11:04:01.000000 mite-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-04 11:04:01.000000 mite-2.0.0/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)     3230 2024-04-04 11:04:01.000000 mite-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3929 2024-04-04 11:04:01.000000 mite-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-04-04 11:04:01.000000 mite-2.0.0/DEV.md
+-rw-r--r--   0 root         (0) root         (0)     1444 2024-04-04 11:04:01.000000 mite-2.0.0/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      307 2024-04-04 11:04:01.000000 mite-2.0.0/Dockerfile.perftest
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-04-04 11:04:01.000000 mite-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-04 11:04:01.000000 mite-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9891 2024-04-04 11:04:09.902150 mite-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8770 2024-04-04 11:04:01.000000 mite-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/cd-scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      526 2024-04-04 11:04:01.000000 mite-2.0.0/cd-scripts/cdBuild-1.sh
+-rw-r--r--   0 root         (0) root         (0)     4138 2024-04-04 11:04:01.000000 mite-2.0.0/cd-scripts/cdRelease.py
+-rw-r--r--   0 root         (0) root         (0)      517 2024-04-04 11:04:01.000000 mite-2.0.0/cd.yml
+-rw-r--r--   0 root         (0) root         (0)      103 2024-04-04 11:04:01.000000 mite-2.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-04 11:04:01.000000 mite-2.0.0/docker_compose.yml
+-rw-r--r--   0 root         (0) root         (0)      698 2024-04-04 11:04:01.000000 mite-2.0.0/docker_compose_monitoring.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-04 11:04:01.000000 mite-2.0.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-04-04 11:04:01.000000 mite-2.0.0/docs/components.rst
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-04-04 11:04:01.000000 mite-2.0.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2024-04-04 11:04:01.000000 mite-2.0.0/docs/config.rst
+-rw-r--r--   0 root         (0) root         (0)     7835 2024-04-04 11:04:01.000000 mite-2.0.0/docs/design-deployment.rst
+-rw-r--r--   0 root         (0) root         (0)      945 2024-04-04 11:04:01.000000 mite-2.0.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3908 2024-04-04 11:04:01.000000 mite-2.0.0/docs/journeys.rst
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-04 11:04:01.000000 mite-2.0.0/docs/notes.txt
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-04 11:04:01.000000 mite-2.0.0/docs/prometheus.rst
+-rw-r--r--   0 root         (0) root         (0)     6507 2024-04-04 11:04:01.000000 mite-2.0.0/docs/stats.rst
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-04-04 11:04:01.000000 mite-2.0.0/docs/volume-model.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/grafana/
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-04 11:04:01.000000 mite-2.0.0/grafana/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-04 11:04:01.000000 mite-2.0.0/grafana/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.870150 mite-2.0.0/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-04 11:04:01.000000 mite-2.0.0/grafana/provisioning/dashboards/dashboards.yml
+-rw-r--r--   0 root         (0) root         (0)    27978 2024-04-04 11:04:01.000000 mite-2.0.0/grafana/provisioning/dashboards/grafana_dashboard_template.json
+-rw-r--r--   0 root         (0) root         (0)    28427 2024-04-04 11:04:01.000000 mite-2.0.0/grafana/provisioning/dashboards/mite_docker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-04 11:04:01.000000 mite-2.0.0/grafana/provisioning/datasources/datasources.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.882150 mite-2.0.0/local/
+-rw-r--r--   0 root         (0) root         (0)      628 2024-04-04 11:04:01.000000 mite-2.0.0/local/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-04-04 11:04:01.000000 mite-2.0.0/local/README.md
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-04 11:04:01.000000 mite-2.0.0/local/demo.py
+-rwxr-xr-x   0 root         (0) root         (0)     1035 2024-04-04 11:04:01.000000 mite-2.0.0/local/run_mite.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.886150 mite-2.0.0/mite/
+-rwxr-xr-x   0 root         (0) root         (0)     2353 2024-04-04 11:04:01.000000 mite-2.0.0/mite/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15198 2024-04-04 11:04:01.000000 mite-2.0.0/mite/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.886150 mite-2.0.0/mite/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/cat.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/collector.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/duplicator.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/receiver.py
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/stats.py
+-rw-r--r--   0 root         (0) root         (0)     6560 2024-04-04 11:04:01.000000 mite-2.0.0/mite/cli/test.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2024-04-04 11:04:01.000000 mite-2.0.0/mite/collector.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-04 11:04:01.000000 mite-2.0.0/mite/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     4815 2024-04-04 11:04:01.000000 mite-2.0.0/mite/context.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2024-04-04 11:04:01.000000 mite-2.0.0/mite/controller.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-04 11:04:01.000000 mite-2.0.0/mite/datapools.py
+-rw-r--r--   0 root         (0) root         (0)      519 2024-04-04 11:04:01.000000 mite-2.0.0/mite/example.py
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-04 11:04:01.000000 mite-2.0.0/mite/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2024-04-04 11:04:01.000000 mite-2.0.0/mite/har_to_mite.py
+-rw-r--r--   0 root         (0) root         (0)     4804 2024-04-04 11:04:01.000000 mite-2.0.0/mite/logoutput.py
+-rwxr-xr-x   0 root         (0) root         (0)     4591 2024-04-04 11:04:01.000000 mite-2.0.0/mite/nanomsg.py
+-rw-r--r--   0 root         (0) root         (0)      968 2024-04-04 11:04:01.000000 mite-2.0.0/mite/recorder.py
+-rwxr-xr-x   0 root         (0) root         (0)     6986 2024-04-04 11:04:01.000000 mite-2.0.0/mite/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2024-04-04 11:04:01.000000 mite-2.0.0/mite/scenario.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2024-04-04 11:04:01.000000 mite-2.0.0/mite/stats.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2024-04-04 11:04:01.000000 mite-2.0.0/mite/test.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-04-04 11:04:01.000000 mite-2.0.0/mite/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2024-04-04 11:04:01.000000 mite-2.0.0/mite/volume_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.886150 mite-2.0.0/mite/web/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-04 11:04:01.000000 mite-2.0.0/mite/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3559 2024-04-04 11:04:01.000000 mite-2.0.0/mite/web/prometheus.py
+-rwxr-xr-x   0 root         (0) root         (0)     6247 2024-04-04 11:04:01.000000 mite-2.0.0/mite/zmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.902150 mite-2.0.0/mite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9891 2024-04-04 11:04:09.000000 mite-2.0.0/mite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-04-04 11:04:09.000000 mite-2.0.0/mite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 11:04:09.000000 mite-2.0.0/mite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-04 11:04:09.000000 mite-2.0.0/mite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      186 2024-04-04 11:04:09.000000 mite-2.0.0/mite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-04-04 11:04:09.000000 mite-2.0.0/mite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.886150 mite-2.0.0/mite_amqp/
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-04 11:04:01.000000 mite-2.0.0/mite_amqp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.886150 mite-2.0.0/mite_browser/
+-rwxr-xr-x   0 root         (0) root         (0)    17442 2024-04-04 11:04:01.000000 mite-2.0.0/mite_browser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.886150 mite-2.0.0/mite_finagle/
+-rw-r--r--   0 root         (0) root         (0)     8329 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/README.md
+-rw-r--r--   0 root         (0) root         (0)     6504 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11258 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/mux.py
+-rw-r--r--   0 root         (0) root         (0)      710 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/mite_finagle/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/mite_finagle/tests/foo_service/
+-rwxr-xr-x   0 root         (0) root         (0)     2698 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/foo_service/Foo-remote
+-rw-r--r--   0 root         (0) root         (0)     7560 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/foo_service/Foo.py
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/foo_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      366 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/foo_service/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/foo_service/ttypes.py
+-rw-r--r--   0 root         (0) root         (0)      263 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/foo_service.thrift
+-rw-r--r--   0 root         (0) root         (0)     3503 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/test_mux.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/tests/test_thrift.py
+-rw-r--r--   0 root         (0) root         (0)     9650 2024-04-04 11:04:01.000000 mite-2.0.0/mite_finagle/thrift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/mite_http/
+-rw-r--r--   0 root         (0) root         (0)     2964 2024-04-04 11:04:01.000000 mite-2.0.0/mite_http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-04-04 11:04:01.000000 mite-2.0.0/mite_http/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/mite_kafka/
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-04 11:04:01.000000 mite-2.0.0/mite_kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-04-04 11:04:01.000000 mite-2.0.0/mite_kafka/kafka_test_scenario.py
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-04 11:04:01.000000 mite-2.0.0/mite_kafka/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/mite_selenium/
+-rw-r--r--   0 root         (0) root         (0)    11427 2024-04-04 11:04:01.000000 mite-2.0.0/mite_selenium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-04 11:04:01.000000 mite-2.0.0/mite_selenium/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/mite_websocket/
+-rw-r--r--   0 root         (0) root         (0)     1381 2024-04-04 11:04:01.000000 mite-2.0.0/mite_websocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.890149 mite-2.0.0/prometheus/
+-rw-r--r--   0 root         (0) root         (0)      188 2024-04-04 11:04:01.000000 mite-2.0.0/prometheus/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-04 11:04:01.000000 mite-2.0.0/prometheus/prometheus_config_docker.yml
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-04 11:04:01.000000 mite-2.0.0/prometheus/prometheus_config_template.yml
+-rw-r--r--   0 root         (0) root         (0)      165 2024-04-04 11:04:01.000000 mite-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-04 11:04:01.000000 mite-2.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-04-04 11:04:09.902150 mite-2.0.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      114 2024-04-04 11:04:01.000000 mite-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.898149 mite-2.0.0/test/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-04 11:04:01.000000 mite-2.0.0/test/legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.902150 mite-2.0.0/test/mocks/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_collector.py
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_context.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_direct_receiver.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_direct_runner_transport.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_recorder_msg_http.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_selenium.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-04 11:04:01.000000 mite-2.0.0/test/mocks/mock_sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:04:09.902150 mite-2.0.0/test/perf/
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/http_server.py
+-rw-r--r--   0 root         (0) root         (0)      968 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/http_server_aiohttp.py
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/mite_perftest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4625 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/perftest.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/run-perftest.sh
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-04 11:04:01.000000 mite-2.0.0/test/perf/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0) 10236043 2024-04-04 11:04:01.000000 mite-2.0.0/test/test.har
+-rw-r--r--   0 root         (0) root         (0)     5240 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_collector.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_context.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_datapools.py
+-rw-r--r--   0 root         (0) root         (0)     7712 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_har_to_mite.py
+-rw-r--r--   0 root         (0) root         (0)      282 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_mite_amqp.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_mite_browser.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_mite_http.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_mite_kafka.py
+-rw-r--r--   0 root         (0) root         (0)      818 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_mite_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_mite_websockets.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_prometheus_mite.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_recorder.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_runner_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_scenario.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_stats.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_volume_model.py
+-rw-r--r--   0 root         (0) root         (0)     8670 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_webdriver.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-04 11:04:01.000000 mite-2.0.0/test/test_work_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-04 11:04:01.000000 mite-2.0.0/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0) 10236043 2024-04-04 11:04:01.000000 mite-2.0.0/test.har
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-04-04 11:04:01.000000 mite-2.0.0/tox.ini
```

### Comparing `mite-1.1.9/.circleci/config.yml` & `mite-2.0.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/.github/ISSUE_TEMPLATE/feature_request.md` & `mite-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/.gitignore` & `mite-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/.travis.yml` & `mite-2.0.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/CODE_OF_CONDUCT.md` & `mite-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/CONTRIBUTING.md` & `mite-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/DEV.md` & `mite-2.0.0/DEV.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/Dockerfile` & `mite-2.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/LICENSE` & `mite-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/PKG-INFO` & `mite-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mite
-Version: 1.1.9
+Version: 2.0.0
 Summary: A Python Performance Testing Framework
 Home-page: https://github.com/sky-uk/mite/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,14 +20,16 @@
 Requires-Dist: nanomsg
 Requires-Dist: pyzmq
 Requires-Dist: selenium<4
 Requires-Dist: uvloop
 Requires-Dist: websockets
 Provides-Extra: amqp
 Requires-Dist: aio_pika; extra == "amqp"
+Provides-Extra: kafka
+Requires-Dist: aiokafka; extra == "kafka"
 Provides-Extra: finagle
 Requires-Dist: thrift; extra == "finagle"
 Provides-Extra: selenium
 Requires-Dist: selenium; extra == "selenium"
 Provides-Extra: selenium-wire
 Requires-Dist: selenium-wire==4.6.5; extra == "selenium-wire"
```

### Comparing `mite-1.1.9/README.md` & `mite-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/cd-scripts/cdBuild-1.sh` & `mite-2.0.0/cd-scripts/cdBuild-1.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/cd-scripts/cdRelease.py` & `mite-2.0.0/cd-scripts/cdRelease.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/cd.yml` & `mite-2.0.0/cd.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docker_compose.yml` & `mite-2.0.0/docker_compose.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docker_compose_monitoring.yml` & `mite-2.0.0/docker_compose_monitoring.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/Makefile` & `mite-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/components.rst` & `mite-2.0.0/docs/components.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/conf.py` & `mite-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/config.rst` & `mite-2.0.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/design-deployment.rst` & `mite-2.0.0/docs/design-deployment.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/index.rst` & `mite-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/journeys.rst` & `mite-2.0.0/docs/journeys.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/prometheus.rst` & `mite-2.0.0/docs/prometheus.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/stats.rst` & `mite-2.0.0/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/docs/volume-model.rst` & `mite-2.0.0/docs/volume-model.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/grafana/provisioning/dashboards/grafana_dashboard_template.json` & `mite-2.0.0/grafana/provisioning/dashboards/grafana_dashboard_template.json`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/grafana/provisioning/dashboards/mite_docker.json` & `mite-2.0.0/grafana/provisioning/dashboards/mite_docker.json`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/local/Makefile` & `mite-2.0.0/local/Makefile`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/local/README.md` & `mite-2.0.0/local/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/local/demo.py` & `mite-2.0.0/local/demo.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/local/run_mite.sh` & `mite-2.0.0/local/run_mite.sh`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # the prometheus config -> mite/prometheus/prometheus_config_template.yml
 # grafana dashboard templates -> mite/grafana/provisioning/grafana_dashboard_template.json
 docker-compose -f docker_compose_monitoring.yml up -d
 
 # Run mite stack w/o controller
 mite runner --controller-socket=tcp://127.0.0.1:14301 --message-socket=tcp://127.0.0.1:14302 &
 mite duplicator --message-socket=tcp://0.0.0.0:14302 tcp://0.0.0.0:14303 &
-mite stats --stats-in-socket=tcp://127.0.0.1:14303 --stats-out-socket=tcp://0.0.0.0:14305 --stats-include-processors=mite,mite_http &
+mite stats --stats-in-socket=tcp://127.0.0.1:14303 --stats-out-socket=tcp://0.0.0.0:14305 --stats-include-processors=mite,mite_http,mite_kafka &
 mite prometheus_exporter --stats-out-socket=tcp://127.0.0.1:14305 --web-address=0.0.0.0:9301 &
 
 # Start a mock web server
 # python -m http.server 8000 &
 
 # Controller Command
 # mite controller --controller-socket=tcp://0.0.0.0:14301 --message-socket=tcp://127.0.0.1:14302 local.demo:scenario &
```

### Comparing `mite-1.1.9/mite/__init__.py` & `mite-2.0.0/mite/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/__main__.py` & `mite-2.0.0/mite/__main__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/cat.py` & `mite-2.0.0/mite/cli/cat.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/collector.py` & `mite-2.0.0/mite/cli/collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/common.py` & `mite-2.0.0/mite/cli/common.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/duplicator.py` & `mite-2.0.0/mite/cli/duplicator.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/receiver.py` & `mite-2.0.0/mite/cli/receiver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/stats.py` & `mite-2.0.0/mite/cli/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/cli/test.py` & `mite-2.0.0/mite/cli/test.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/collector.py` & `mite-2.0.0/mite/collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/config.py` & `mite-2.0.0/mite/config.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/context.py` & `mite-2.0.0/mite/context.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/controller.py` & `mite-2.0.0/mite/controller.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/datapools.py` & `mite-2.0.0/mite/datapools.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/example.py` & `mite-2.0.0/mite/example.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/har_to_mite.py` & `mite-2.0.0/mite/har_to_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/logoutput.py` & `mite-2.0.0/mite/logoutput.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/nanomsg.py` & `mite-2.0.0/mite/nanomsg.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/recorder.py` & `mite-2.0.0/mite/recorder.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/runner.py` & `mite-2.0.0/mite/runner.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/scenario.py` & `mite-2.0.0/mite/scenario.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/stats.py` & `mite-2.0.0/mite/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/test.py` & `mite-2.0.0/mite/test.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/utils.py` & `mite-2.0.0/mite/utils.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/volume_model.py` & `mite-2.0.0/mite/volume_model.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/web/prometheus.py` & `mite-2.0.0/mite/web/prometheus.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite/zmq.py` & `mite-2.0.0/mite/zmq.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite.egg-info/PKG-INFO` & `mite-2.0.0/mite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mite
-Version: 1.1.9
+Version: 2.0.0
 Summary: A Python Performance Testing Framework
 Home-page: https://github.com/sky-uk/mite/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,14 +20,16 @@
 Requires-Dist: nanomsg
 Requires-Dist: pyzmq
 Requires-Dist: selenium<4
 Requires-Dist: uvloop
 Requires-Dist: websockets
 Provides-Extra: amqp
 Requires-Dist: aio_pika; extra == "amqp"
+Provides-Extra: kafka
+Requires-Dist: aiokafka; extra == "kafka"
 Provides-Extra: finagle
 Requires-Dist: thrift; extra == "finagle"
 Provides-Extra: selenium
 Requires-Dist: selenium; extra == "selenium"
 Provides-Extra: selenium-wire
 Requires-Dist: selenium-wire==4.6.5; extra == "selenium-wire"
```

### Comparing `mite-1.1.9/mite.egg-info/SOURCES.txt` & `mite-2.0.0/mite.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 mite_finagle/tests/foo_service/Foo-remote
 mite_finagle/tests/foo_service/Foo.py
 mite_finagle/tests/foo_service/__init__.py
 mite_finagle/tests/foo_service/constants.py
 mite_finagle/tests/foo_service/ttypes.py
 mite_http/__init__.py
 mite_http/stats.py
+mite_kafka/__init__.py
+mite_kafka/kafka_test_scenario.py
+mite_kafka/stats.py
 mite_selenium/__init__.py
 mite_selenium/stats.py
 mite_websocket/__init__.py
 prometheus/Dockerfile
 prometheus/prometheus_config_docker.yml
 prometheus/prometheus_config_template.yml
 test/legacy.py
@@ -119,14 +122,15 @@
 test/test_controller.py
 test/test_datapools.py
 test/test_har_to_mite.py
 test/test_logging.py
 test/test_mite_amqp.py
 test/test_mite_browser.py
 test/test_mite_http.py
+test/test_mite_kafka.py
 test/test_mite_utils.py
 test/test_mite_websockets.py
 test/test_prometheus_mite.py
 test/test_recorder.py
 test/test_runner.py
 test/test_runner_tracker.py
 test/test_scenario.py
```

### Comparing `mite-1.1.9/mite_amqp/__init__.py` & `mite-2.0.0/mite_amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_browser/__init__.py` & `mite-2.0.0/mite_browser/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/README.md` & `mite-2.0.0/mite_finagle/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/__init__.py` & `mite-2.0.0/mite_finagle/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/mux.py` & `mite-2.0.0/mite_finagle/mux.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/stats.py` & `mite-2.0.0/mite_finagle/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/conftest.py` & `mite-2.0.0/mite_finagle/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/foo_service/Foo-remote` & `mite-2.0.0/mite_finagle/tests/foo_service/Foo-remote`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/foo_service/Foo.py` & `mite-2.0.0/mite_finagle/tests/foo_service/Foo.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/foo_service/ttypes.py` & `mite-2.0.0/mite_finagle/tests/foo_service/ttypes.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/test_integration.py` & `mite-2.0.0/mite_finagle/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/test_mux.py` & `mite-2.0.0/mite_finagle/tests/test_mux.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/tests/test_thrift.py` & `mite-2.0.0/mite_finagle/tests/test_thrift.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_finagle/thrift.py` & `mite-2.0.0/mite_finagle/thrift.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_http/__init__.py` & `mite-2.0.0/mite_http/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_http/stats.py` & `mite-2.0.0/mite_http/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_selenium/__init__.py` & `mite-2.0.0/mite_selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_selenium/stats.py` & `mite-2.0.0/mite_selenium/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/mite_websocket/__init__.py` & `mite-2.0.0/mite_websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/setup.cfg` & `mite-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 	websockets
 setup_requires = pytest-runner
 packages = find:
 
 [options.extras_require]
 amqp = 
 	aio_pika
+kafka = 
+	aiokafka
 finagle = 
 	thrift
 selenium = 
 	selenium
 selenium_wire = selenium-wire==4.6.5
 
 [options.entry_points]
 console_scripts = 
 	mite = mite.__main__:main
 mite_stats = 
 	mite = mite.stats:_MITE_STATS
 	mite_finagle = mite_finagle.stats:STATS
 	mite_http = mite_http.stats:STATS
 	mite_selenium = mite_selenium.stats:STATS
+	mite_kafka = mite_kafka.stats:_KAFKA_STATS
 
 [options.packages.find]
 exclude = 
 	acurl
 
 [flake8]
 ignore =
```

### Comparing `mite-1.1.9/test/mocks/mock_direct_receiver.py` & `mite-2.0.0/test/mocks/mock_direct_receiver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/mocks/mock_direct_runner_transport.py` & `mite-2.0.0/test/mocks/mock_direct_runner_transport.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/mocks/mock_recorder_msg_http.py` & `mite-2.0.0/test/mocks/mock_recorder_msg_http.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/mocks/mock_selenium.py` & `mite-2.0.0/test/mocks/mock_selenium.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/perf/http_server.py` & `mite-2.0.0/test/perf/http_server.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/perf/http_server_aiohttp.py` & `mite-2.0.0/test/perf/http_server_aiohttp.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/perf/mite_perftest.py` & `mite-2.0.0/test/perf/mite_perftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/perf/perftest.py` & `mite-2.0.0/test/perf/perftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/perf/run-perftest.sh` & `mite-2.0.0/test/perf/run-perftest.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test.har` & `mite-2.0.0/test/test.har`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_collector.py` & `mite-2.0.0/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_config.py` & `mite-2.0.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_context.py` & `mite-2.0.0/test/test_context.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_controller.py` & `mite-2.0.0/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_datapools.py` & `mite-2.0.0/test/test_datapools.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_har_to_mite.py` & `mite-2.0.0/test/test_har_to_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_mite_amqp.py` & `mite-2.0.0/test/test_mite_amqp.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_mite_browser.py` & `mite-2.0.0/test/test_mite_browser.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_mite_http.py` & `mite-2.0.0/test/test_mite_http.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_mite_utils.py` & `mite-2.0.0/test/test_mite_utils.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_mite_websockets.py` & `mite-2.0.0/test/test_mite_websockets.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_prometheus_mite.py` & `mite-2.0.0/test/test_prometheus_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_recorder.py` & `mite-2.0.0/test/test_recorder.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_runner.py` & `mite-2.0.0/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_runner_tracker.py` & `mite-2.0.0/test/test_runner_tracker.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_scenario.py` & `mite-2.0.0/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_stats.py` & `mite-2.0.0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_volume_model.py` & `mite-2.0.0/test/test_volume_model.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_webdriver.py` & `mite-2.0.0/test/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test/test_work_tracker.py` & `mite-2.0.0/test/test_work_tracker.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/test.har` & `mite-2.0.0/test.har`

 * *Files identical despite different names*

### Comparing `mite-1.1.9/tox.ini` & `mite-2.0.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 source =
     acurl
     mite
     mite_http
     mite_browser
     mite_selenium
     mite_amqp
+    mite_kafka
     mite_websocket
     mite_finagle
 plugins = Cython.Coverage
 
 [coverage:report]
 # Regexes for lines to exclude from consideration
 exclude_lines =
```

