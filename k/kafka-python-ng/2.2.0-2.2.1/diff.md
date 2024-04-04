# Comparing `tmp/kafka-python-ng-2.2.0.tar.gz` & `tmp/kafka-python-ng-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-python-ng-2.2.0.tar", last modified: Wed Mar 27 01:52:55 2024, max compression
+gzip compressed data, was "kafka-python-ng-2.2.1.tar", last modified: Thu Apr  4 15:56:52 2024, max compression
```

## Comparing `kafka-python-ng-2.2.0.tar` & `kafka-python-ng-2.2.1.tar`

### file list

```diff
@@ -1,394 +1,394 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.675806 kafka-python-ng-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.627806 kafka-python-ng-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.627806 kafka-python-ng-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    57213 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-03-27 01:52:55.675806 kafka-python-ng-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.627806 kafka-python-ng-2.2.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/consumer_performance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1618 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/load_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5205 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/producer_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/record_batch_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/record_batch_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/benchmarks/varint_speed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2694 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/build_integration.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.631806 kafka-python-ng-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.631806 kafka-python-ng-2.2.0/docs/apidoc/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/BrokerConnection.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/ClusterMetadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/KafkaAdminClient.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/KafkaClient.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/KafkaConsumer.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/KafkaProducer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/apidoc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)    59846 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/docs/usage.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1983 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.635805 kafka-python-ng-2.2.0/kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.635805 kafka-python-ng-2.2.0/kafka/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/admin/acl_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    64300 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/admin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/admin/config_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/admin/new_partitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/admin/new_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    45226 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/client_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    56539 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/conn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.635805 kafka-python-ng-2.2.0/kafka/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47504 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/consumer/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    59428 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/consumer/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/consumer/subscription_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.635805 kafka-python-ng-2.2.0/kafka/coordinator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.635805 kafka-python-ng-2.2.0/kafka/coordinator/assignors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/roundrobin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.639806 kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/partition_movements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/sorted_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    34038 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/sticky_assignor.py
--rw-r--r--   0 runner    (1001) docker     (127)    49041 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    39291 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/coordinator/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/future.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.639806 kafka-python-ng-2.2.0/kafka/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/compound_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/dict_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/kafka_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/measurable.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/measurable_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/metric_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/metric_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/metrics_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.643806 kafka-python-ng-2.2.0/kafka/metrics/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/avg.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/max_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/min_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/percentile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/sampled_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/metrics/stats/total.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.643806 kafka-python-ng-2.2.0/kafka/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/oauth/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.643806 kafka-python-ng-2.2.0/kafka/partitioner/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/partitioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/partitioner/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.643806 kafka-python-ng-2.2.0/kafka/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/producer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/producer/future.py
--rw-r--r--   0 runner    (1001) docker     (127)    37654 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/producer/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    24926 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/producer/record_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/producer/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.647806 kafka-python-ng-2.2.0/kafka/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    29905 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/produce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/protocol/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.647806 kafka-python-ng-2.2.0/kafka/record/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/README
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/_crc32c.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/default_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/legacy_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/memory_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/record/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.647806 kafka-python-ng-2.2.0/kafka/sasl/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/sasl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/sasl/gssapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/sasl/msk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/sasl/oauthbearer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/sasl/plain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/sasl/scram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/scram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.647806 kafka-python-ng-2.2.0/kafka/serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/serializer/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.671806 kafka-python-ng-2.2.0/kafka_python_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-03-27 01:52:55.000000 kafka-python-ng-2.2.0/kafka_python_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-03-27 01:52:55.000000 kafka-python-ng-2.2.0/kafka_python_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 01:52:55.000000 kafka-python-ng-2.2.0/kafka_python_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 01:52:55.000000 kafka-python-ng-2.2.0/kafka_python_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 01:52:55.000000 kafka-python-ng-2.2.0/kafka_python_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/pylint.rc
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.10.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.647806 kafka-python-ng-2.2.0/servers/0.10.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.10.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.651806 kafka-python-ng-2.2.0/servers/0.10.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.10.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.651806 kafka-python-ng-2.2.0/servers/0.10.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.1.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.10.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.651806 kafka-python-ng-2.2.0/servers/0.10.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.10.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.651806 kafka-python-ng-2.2.0/servers/0.10.2.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.2/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.10.2.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.11.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.651806 kafka-python-ng-2.2.0/servers/0.11.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.11.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.651806 kafka-python-ng-2.2.0/servers/0.11.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.11.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.11.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.2/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.11.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.11.0.3/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.3/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.3/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.3/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.11.0.3/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.8.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.8.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.619805 kafka-python-ng-2.2.0/servers/0.8.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.8.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/0.8.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.8.2.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/0.8.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.8.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/0.8.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.655806 kafka-python-ng-2.2.0/servers/0.8.2.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.8.2.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/0.9.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/0.9.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.9.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.9.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.9.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/0.9.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/0.9.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.9.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.9.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/0.9.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/1.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/1.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/1.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.2/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.0.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/1.1.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.659806 kafka-python-ng-2.2.0/servers/1.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/1.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.1.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.2.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.2.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.2.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.2.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.3.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.3.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.3.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.3.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.663806 kafka-python-ng-2.2.0/servers/2.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.4.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.4.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.4.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.4.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.667806 kafka-python-ng-2.2.0/servers/2.5.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.5.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.5.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.5.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.5.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/2.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.667806 kafka-python-ng-2.2.0/servers/2.6.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.6.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.6.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.6.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/2.6.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.623805 kafka-python-ng-2.2.0/servers/trunk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.667806 kafka-python-ng-2.2.0/servers/trunk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/trunk/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/trunk/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/trunk/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/servers/trunk/resources/zookeeper.properties
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-27 01:52:55.675806 kafka-python-ng-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.671806 kafka-python-ng-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    26996 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:52:55.671806 kafka-python-ng-2.2.0/test/record/
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/record/test_default_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/record/test_legacy_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/record/test_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/record/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_acl_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_admin_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_api_object_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_assignors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_client_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_consumer_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    26676 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_msk.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_object_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_partition_movements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_partitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_sasl_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/test_subscription_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/test/testutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-03-27 01:52:49.000000 kafka-python-ng-2.2.0/travis_java_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.051602 kafka-python-ng-2.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.051602 kafka-python-ng-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    57213 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.051602 kafka-python-ng-2.2.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/consumer_performance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1618 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/load_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5205 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/producer_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/record_batch_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/record_batch_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/varint_speed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2694 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/build_integration.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.055602 kafka-python-ng-2.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.055602 kafka-python-ng-2.2.1/docs/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/BrokerConnection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/ClusterMetadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaAdminClient.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaClient.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaConsumer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaProducer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    59846 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1983 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.059602 kafka-python-ng-2.2.1/kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.059602 kafka-python-ng-2.2.1/kafka/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/acl_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64300 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/new_partitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/new_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45437 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/client_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56893 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/conn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.059602 kafka-python-ng-2.2.1/kafka/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47504 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59428 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/subscription_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/coordinator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/coordinator/assignors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/roundrobin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/partition_movements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sorted_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34038 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sticky_assignor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49041 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39291 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/future.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/compound_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/dict_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/kafka_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/measurable_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metric_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metric_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metrics_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/metrics/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/max_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/min_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/sampled_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/total.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/oauth/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/partitioner/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/partitioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/partitioner/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37865 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24926 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/record_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.071602 kafka-python-ng-2.2.1/kafka/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29905 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/produce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/kafka/record/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/README
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/_crc32c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/default_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/legacy_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/memory_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/kafka/sasl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/gssapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/msk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/oauthbearer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/plain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/scram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/scram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/kafka/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/serializer/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-04 15:56:52.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/pylint.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.8.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.8.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.8.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.8.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.9.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.9.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.1.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/1.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.1.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.2.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.3.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.6.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/trunk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/trunk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/zookeeper.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.099603 kafka-python-ng-2.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26996 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/test/record/
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_default_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_legacy_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_acl_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_admin_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_api_object_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_assignors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_client_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_consumer_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26676 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_msk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_object_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_partition_movements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_partitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_sasl_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_subscription_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/travis_java_install.sh
```

### Comparing `kafka-python-ng-2.2.0/.github/workflows/codeql-analysis.yml` & `kafka-python-ng-2.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/.github/workflows/python-package.yml` & `kafka-python-ng-2.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/.travis.yml` & `kafka-python-ng-2.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/AUTHORS.md` & `kafka-python-ng-2.2.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/CHANGES.md` & `kafka-python-ng-2.2.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/LICENSE` & `kafka-python-ng-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/Makefile` & `kafka-python-ng-2.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/PKG-INFO` & `kafka-python-ng-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-python-ng
-Version: 2.2.0
+Version: 2.2.1
 Summary: Pure Python client for Apache Kafka
 Home-page: https://github.com/wbarnha/kafka-python-ng
 Author: Dana Powers
 Author-email: dana.powers@gmail.com
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 License: Apache License 2.0
```

### Comparing `kafka-python-ng-2.2.0/README.rst` & `kafka-python-ng-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/benchmarks/consumer_performance.py` & `kafka-python-ng-2.2.1/benchmarks/consumer_performance.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/benchmarks/load_example.py` & `kafka-python-ng-2.2.1/benchmarks/load_example.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/benchmarks/producer_performance.py` & `kafka-python-ng-2.2.1/benchmarks/producer_performance.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/benchmarks/record_batch_compose.py` & `kafka-python-ng-2.2.1/benchmarks/record_batch_compose.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/benchmarks/record_batch_read.py` & `kafka-python-ng-2.2.1/benchmarks/record_batch_read.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/benchmarks/varint_speed.py` & `kafka-python-ng-2.2.1/benchmarks/varint_speed.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/build_integration.sh` & `kafka-python-ng-2.2.1/build_integration.sh`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/Makefile` & `kafka-python-ng-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/changelog.rst` & `kafka-python-ng-2.2.1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/compatibility.rst` & `kafka-python-ng-2.2.1/docs/compatibility.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/conf.py` & `kafka-python-ng-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/index.rst` & `kafka-python-ng-2.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/install.rst` & `kafka-python-ng-2.2.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/make.bat` & `kafka-python-ng-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/tests.rst` & `kafka-python-ng-2.2.1/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/docs/usage.rst` & `kafka-python-ng-2.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/example.py` & `kafka-python-ng-2.2.1/example.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/__init__.py` & `kafka-python-ng-2.2.1/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/admin/__init__.py` & `kafka-python-ng-2.2.1/kafka/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/admin/acl_resource.py` & `kafka-python-ng-2.2.1/kafka/admin/acl_resource.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/admin/client.py` & `kafka-python-ng-2.2.1/kafka/admin/client.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/admin/config_resource.py` & `kafka-python-ng-2.2.1/kafka/admin/config_resource.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/admin/new_partitions.py` & `kafka-python-ng-2.2.1/kafka/admin/new_partitions.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/admin/new_topic.py` & `kafka-python-ng-2.2.1/kafka/admin/new_topic.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/client_async.py` & `kafka-python-ng-2.2.1/kafka/client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
             repeatedly failed to connect. If provided, the backoff per host
             will increase exponentially for each consecutive connection
             failure, up to this maximum. Once the maximum is reached,
             reconnection attempts will continue periodically with this fixed
             rate. To avoid connection storms, a randomization factor of 0.2
             will be applied to the backoff resulting in a random range between
             20% below and 20% above the computed value. Default: 1000.
+        connection_timeout_ms (int): Connection timeout in milliseconds.
+            Default: None, which defaults it to the same value as 
+            request_timeout_ms.
         request_timeout_ms (int): Client request timeout in milliseconds.
             Default: 30000.
         connections_max_idle_ms: Close idle connections after the number of
             milliseconds specified by this config. The broker closes idle
             connections after connections.max.idle.ms, so this avoids hitting
             unexpected socket disconnected errors on the client.
             Default: 540000
@@ -141,14 +144,15 @@
             upon socket error during wakeup(). Default: False
     """
 
     DEFAULT_CONFIG = {
         'bootstrap_servers': 'localhost',
         'bootstrap_topics_filter': set(),
         'client_id': 'kafka-python-' + __version__,
+        'connection_timeout_ms': None,
         'request_timeout_ms': 30000,
         'wakeup_timeout_ms': 3000,
         'connections_max_idle_ms': 9 * 60 * 1000,
         'reconnect_backoff_ms': 50,
         'reconnect_backoff_max_ms': 1000,
         'max_in_flight_requests_per_connection': 5,
         'receive_buffer_bytes': None,
```

### Comparing `kafka-python-ng-2.2.0/kafka/cluster.py` & `kafka-python-ng-2.2.1/kafka/cluster.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/codec.py` & `kafka-python-ng-2.2.1/kafka/codec.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/conn.py` & `kafka-python-ng-2.2.1/kafka/conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,21 +64,14 @@
     import gssapi
     from gssapi.raw.misc import GSSError
 except (ImportError, OSError):
     #no gssapi available, will disable gssapi mechanism
     gssapi = None
     GSSError = None
 
-# needed for AWS_MSK_IAM authentication:
-try:
-    from botocore.session import Session as BotoSession
-except ImportError:
-    # no botocore available, will disable AWS_MSK_IAM mechanism
-    BotoSession = None
-
 AFI_NAMES = {
     socket.AF_UNSPEC: "unspecified",
     socket.AF_INET: "IPv4",
     socket.AF_INET6: "IPv6",
 }
 
 
@@ -108,14 +101,17 @@
             repeatedly failed to connect. If provided, the backoff per host
             will increase exponentially for each consecutive connection
             failure, up to this maximum. Once the maximum is reached,
             reconnection attempts will continue periodically with this fixed
             rate. To avoid connection storms, a randomization factor of 0.2
             will be applied to the backoff resulting in a random range between
             20% below and 20% above the computed value. Default: 1000.
+        connection_timeout_ms (int): Connection timeout in milliseconds.
+            Default: None, which defaults it to the same value as
+            request_timeout_ms.
         request_timeout_ms (int): Client request timeout in milliseconds.
             Default: 30000.
         max_in_flight_requests_per_connection (int): Requests are pipelined
             to kafka brokers up to this number of maximum requests per
             broker connection. Default: 5.
         receive_buffer_bytes (int): The size of the TCP receive buffer
             (SO_RCVBUF) to use when reading data. Default: None (relies on
@@ -184,14 +180,15 @@
             instance. (See kafka.oauth.abstract). Default: None
     """
 
     DEFAULT_CONFIG = {
         'client_id': 'kafka-python-' + __version__,
         'node_id': 0,
         'request_timeout_ms': 30000,
+        'connection_timeout_ms': None,
         'reconnect_backoff_ms': 50,
         'reconnect_backoff_max_ms': 1000,
         'max_in_flight_requests_per_connection': 5,
         'receive_buffer_bytes': None,
         'send_buffer_bytes': None,
         'socket_options': [(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)],
         'sock_chunk_bytes': 4096,  # undocumented experimental option
@@ -228,41 +225,40 @@
         self._api_versions = None
 
         self.config = copy.copy(self.DEFAULT_CONFIG)
         for key in self.config:
             if key in configs:
                 self.config[key] = configs[key]
 
+        if self.config['connection_timeout_ms'] is None:
+            self.config['connection_timeout_ms'] = self.config['request_timeout_ms']
+
         self.node_id = self.config.pop('node_id')
 
         if self.config['receive_buffer_bytes'] is not None:
             self.config['socket_options'].append(
                 (socket.SOL_SOCKET, socket.SO_RCVBUF,
                  self.config['receive_buffer_bytes']))
         if self.config['send_buffer_bytes'] is not None:
             self.config['socket_options'].append(
                  (socket.SOL_SOCKET, socket.SO_SNDBUF,
                  self.config['send_buffer_bytes']))
 
         assert self.config['security_protocol'] in self.SECURITY_PROTOCOLS, (
             'security_protocol must be in ' + ', '.join(self.SECURITY_PROTOCOLS))
 
-
         if self.config['security_protocol'] in ('SSL', 'SASL_SSL'):
             assert ssl_available, "Python wasn't built with SSL support"
 
-        if self.config['sasl_mechanism'] == 'AWS_MSK_IAM':
-            assert BotoSession is not None, 'AWS_MSK_IAM requires the "botocore" package'
-            assert self.config['security_protocol'] == 'SASL_SSL', 'AWS_MSK_IAM requires SASL_SSL'
-        
         if self.config['security_protocol'] in ('SASL_PLAINTEXT', 'SASL_SSL'):
             assert self.config['sasl_mechanism'] in sasl.MECHANISMS, (
                 'sasl_mechanism must be one of {}'.format(', '.join(sasl.MECHANISMS.keys()))
             )
             sasl.MECHANISMS[self.config['sasl_mechanism']].validate_config(self)
+
         # This is not a general lock / this class is not generally thread-safe yet
         # However, to avoid pushing responsibility for maintaining
         # per-connection locks to the upstream client, we will use this lock to
         # make sure that access to the protocol buffer is synchronized
         # when sends happen on multiple threads
         self._lock = threading.Lock()
 
@@ -280,15 +276,18 @@
         self._reset_reconnect_backoff()
         self._sock = None
         self._send_buffer = b''
         self._ssl_context = None
         if self.config['ssl_context'] is not None:
             self._ssl_context = self.config['ssl_context']
         self._sasl_auth_future = None
-        self.last_attempt = 0
+        self.last_activity = 0
+        # This value is not used for internal state, but it is left to allow backwards-compatability
+        # The variable last_activity is now used instead, but is updated more often may therefore break compatability with some hacks.
+        self.last_attempt= 0
         self._gai = []
         self._sensors = None
         if self.config['metrics']:
             self._sensors = BrokerConnectionMetrics(self.config['metrics'],
                                                     self.config['metric_group_prefix'],
                                                     self.node_id)
 
@@ -358,14 +357,15 @@
                 self._sock.setsockopt(*option)
 
             self._sock.setblocking(False)
             self.state = ConnectionStates.CONNECTING
             self.config['state_change_callback'](self.node_id, self._sock, self)
             log.info('%s: connecting to %s:%d [%s %s]', self, self.host,
                      self.port, self._sock_addr, AFI_NAMES[self._sock_afi])
+            self.last_activity = time.time()
 
         if self.state is ConnectionStates.CONNECTING:
             # in non-blocking mode, use repeated calls to socket.connect_ex
             # to check connection status
             ret = None
             try:
                 ret = self._sock.connect_ex(self._sock_addr)
@@ -390,14 +390,15 @@
 
                 else:
                     # security_protocol PLAINTEXT
                     log.info('%s: Connection complete.', self)
                     self.state = ConnectionStates.CONNECTED
                     self._reset_reconnect_backoff()
                     self.config['state_change_callback'](self.node_id, self._sock, self)
+                self.last_activity = time.time()
 
             # Connection failed
             # WSAEINVAL == 10022, but errno.WSAEINVAL is not available on non-win systems
             elif ret not in (errno.EINPROGRESS, errno.EALREADY, errno.EWOULDBLOCK, 10022):
                 log.error('Connect attempt to %s returned error %s.'
                           ' Disconnecting.', self, ret)
                 errstr = errno.errorcode.get(ret, 'UNKNOWN')
@@ -415,30 +416,32 @@
                     log.debug('%s: initiating SASL authentication', self)
                     self.state = ConnectionStates.AUTHENTICATING
                 else:
                     log.info('%s: Connection complete.', self)
                     self.state = ConnectionStates.CONNECTED
                     self._reset_reconnect_backoff()
                 self.config['state_change_callback'](self.node_id, self._sock, self)
+                self.last_activity = time.time()
 
         if self.state is ConnectionStates.AUTHENTICATING:
             assert self.config['security_protocol'] in ('SASL_PLAINTEXT', 'SASL_SSL')
             if self._try_authenticate():
                 # _try_authenticate has side-effects: possibly disconnected on socket errors
                 if self.state is ConnectionStates.AUTHENTICATING:
                     log.info('%s: Connection complete.', self)
                     self.state = ConnectionStates.CONNECTED
                     self._reset_reconnect_backoff()
                     self.config['state_change_callback'](self.node_id, self._sock, self)
+                    self.last_activity = time.time()
 
         if self.state not in (ConnectionStates.CONNECTED,
                               ConnectionStates.DISCONNECTED):
             # Connection timed out
-            request_timeout = self.config['request_timeout_ms'] / 1000.0
-            if time.time() > request_timeout + self.last_attempt:
+            request_timeout = self.config['connection_timeout_ms'] / 1000.0
+            if time.time() > request_timeout + self.last_activity:
                 log.error('Connection attempt to %s timed out', self)
                 self.close(Errors.KafkaConnectionError('timeout'))
                 return self.state
 
         return self.state
 
     def _wrap_ssl(self):
@@ -591,26 +594,26 @@
 
     def blacked_out(self):
         """
         Return true if we are disconnected from the given node and can't
         re-establish a connection yet
         """
         if self.state is ConnectionStates.DISCONNECTED:
-            if time.time() < self.last_attempt + self._reconnect_backoff:
+            if time.time() < self.last_activity + self._reconnect_backoff:
                 return True
         return False
 
     def connection_delay(self):
         """
         Return the number of milliseconds to wait, based on the connection
         state, before attempting to send data. When disconnected, this respects
         the reconnect backoff time. When connecting or connected, returns a very
         large number to handle slow/stalled connections.
         """
-        time_waited = time.time() - (self.last_attempt or 0)
+        time_waited = time.time() - (self.last_activity or 0)
         if self.state is ConnectionStates.DISCONNECTED:
             return max(self._reconnect_backoff - time_waited, 0) * 1000
         else:
             # When connecting or connected, we should be able to delay
             # indefinitely since other events (connection or data acked) will
             # cause a wakeup once data can be sent.
             return float('inf')
```

### Comparing `kafka-python-ng-2.2.0/kafka/consumer/fetcher.py` & `kafka-python-ng-2.2.1/kafka/consumer/fetcher.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/consumer/group.py` & `kafka-python-ng-2.2.1/kafka/consumer/group.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/consumer/subscription_state.py` & `kafka-python-ng-2.2.1/kafka/consumer/subscription_state.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/assignors/abstract.py` & `kafka-python-ng-2.2.1/kafka/coordinator/assignors/abstract.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/assignors/range.py` & `kafka-python-ng-2.2.1/kafka/coordinator/assignors/range.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/assignors/roundrobin.py` & `kafka-python-ng-2.2.1/kafka/coordinator/assignors/roundrobin.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/partition_movements.py` & `kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/partition_movements.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/sorted_set.py` & `kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sorted_set.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/assignors/sticky/sticky_assignor.py` & `kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sticky_assignor.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/base.py` & `kafka-python-ng-2.2.1/kafka/coordinator/base.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/consumer.py` & `kafka-python-ng-2.2.1/kafka/coordinator/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/heartbeat.py` & `kafka-python-ng-2.2.1/kafka/coordinator/heartbeat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/coordinator/protocol.py` & `kafka-python-ng-2.2.1/kafka/coordinator/protocol.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/errors.py` & `kafka-python-ng-2.2.1/kafka/errors.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/future.py` & `kafka-python-ng-2.2.1/kafka/future.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/__init__.py` & `kafka-python-ng-2.2.1/kafka/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/compound_stat.py` & `kafka-python-ng-2.2.1/kafka/metrics/compound_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/dict_reporter.py` & `kafka-python-ng-2.2.1/kafka/metrics/dict_reporter.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/kafka_metric.py` & `kafka-python-ng-2.2.1/kafka/metrics/kafka_metric.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/measurable.py` & `kafka-python-ng-2.2.1/kafka/metrics/measurable.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/metric_config.py` & `kafka-python-ng-2.2.1/kafka/metrics/metric_config.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/metric_name.py` & `kafka-python-ng-2.2.1/kafka/metrics/metric_name.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/metrics.py` & `kafka-python-ng-2.2.1/kafka/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/metrics_reporter.py` & `kafka-python-ng-2.2.1/kafka/metrics/metrics_reporter.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/quota.py` & `kafka-python-ng-2.2.1/kafka/metrics/quota.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stat.py` & `kafka-python-ng-2.2.1/kafka/metrics/stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/__init__.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/avg.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/avg.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/histogram.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/histogram.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/max_stat.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/max_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/min_stat.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/min_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/percentiles.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/percentiles.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/rate.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/rate.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/sampled_stat.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/sampled_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/metrics/stats/sensor.py` & `kafka-python-ng-2.2.1/kafka/metrics/stats/sensor.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/oauth/abstract.py` & `kafka-python-ng-2.2.1/kafka/oauth/abstract.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/partitioner/default.py` & `kafka-python-ng-2.2.1/kafka/partitioner/default.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/producer/buffer.py` & `kafka-python-ng-2.2.1/kafka/producer/buffer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/producer/future.py` & `kafka-python-ng-2.2.1/kafka/producer/future.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/producer/kafka.py` & `kafka-python-ng-2.2.1/kafka/producer/kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,17 @@
             Default: 1048576.
         metadata_max_age_ms (int): The period of time in milliseconds after
             which we force a refresh of metadata even if we haven't seen any
             partition leadership changes to proactively discover any new
             brokers or partitions. Default: 300000
         retry_backoff_ms (int): Milliseconds to backoff when retrying on
             errors. Default: 100.
+        connection_timeout_ms (int): Connection timeout in milliseconds.
+            Default: None, which defaults it to the same value as 
+            request_timeout_ms.
         request_timeout_ms (int): Client request timeout in milliseconds.
             Default: 30000.
         receive_buffer_bytes (int): The size of the TCP receive buffer
             (SO_RCVBUF) to use when reading data. Default: None (relies on
             system defaults). Java client defaults to 32768.
         send_buffer_bytes (int): The size of the TCP send buffer
             (SO_SNDBUF) to use when sending data. Default: None (relies on
@@ -296,14 +299,15 @@
         'partitioner': DefaultPartitioner(),
         'buffer_memory': 33554432,
         'connections_max_idle_ms': 9 * 60 * 1000,
         'max_block_ms': 60000,
         'max_request_size': 1048576,
         'metadata_max_age_ms': 300000,
         'retry_backoff_ms': 100,
+        'connection_timeout_ms': None,
         'request_timeout_ms': 30000,
         'receive_buffer_bytes': None,
         'send_buffer_bytes': None,
         'socket_options': [(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)],
         'sock_chunk_bytes': 4096,  # undocumented experimental option
         'sock_chunk_buffer_count': 1000,  # undocumented experimental option
         'reconnect_backoff_ms': 50,
```

### Comparing `kafka-python-ng-2.2.0/kafka/producer/record_accumulator.py` & `kafka-python-ng-2.2.1/kafka/producer/record_accumulator.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/producer/sender.py` & `kafka-python-ng-2.2.1/kafka/producer/sender.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/__init__.py` & `kafka-python-ng-2.2.1/kafka/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/admin.py` & `kafka-python-ng-2.2.1/kafka/protocol/admin.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/api.py` & `kafka-python-ng-2.2.1/kafka/protocol/api.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/commit.py` & `kafka-python-ng-2.2.1/kafka/protocol/commit.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/fetch.py` & `kafka-python-ng-2.2.1/kafka/protocol/fetch.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/frame.py` & `kafka-python-ng-2.2.1/kafka/protocol/frame.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/group.py` & `kafka-python-ng-2.2.1/kafka/protocol/group.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/message.py` & `kafka-python-ng-2.2.1/kafka/protocol/message.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/metadata.py` & `kafka-python-ng-2.2.1/kafka/protocol/metadata.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/offset.py` & `kafka-python-ng-2.2.1/kafka/protocol/offset.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/parser.py` & `kafka-python-ng-2.2.1/kafka/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/pickle.py` & `kafka-python-ng-2.2.1/kafka/protocol/pickle.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/produce.py` & `kafka-python-ng-2.2.1/kafka/protocol/produce.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/struct.py` & `kafka-python-ng-2.2.1/kafka/protocol/struct.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/protocol/types.py` & `kafka-python-ng-2.2.1/kafka/protocol/types.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/record/_crc32c.py` & `kafka-python-ng-2.2.1/kafka/record/_crc32c.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/record/abc.py` & `kafka-python-ng-2.2.1/kafka/record/abc.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/record/default_records.py` & `kafka-python-ng-2.2.1/kafka/record/default_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/record/legacy_records.py` & `kafka-python-ng-2.2.1/kafka/record/legacy_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/record/memory_records.py` & `kafka-python-ng-2.2.1/kafka/record/memory_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/record/util.py` & `kafka-python-ng-2.2.1/kafka/record/util.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/sasl/__init__.py` & `kafka-python-ng-2.2.1/kafka/sasl/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/sasl/gssapi.py` & `kafka-python-ng-2.2.1/kafka/sasl/gssapi.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/sasl/msk.py` & `kafka-python-ng-2.2.1/kafka/sasl/msk.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,40 @@
 import struct
 import logging
 import urllib
 
 from kafka.protocol.types import Int32
 import kafka.errors as Errors
 
-from botocore.session import Session as BotoSession  # importing it in advance is not an option apparently...
+# needed for AWS_MSK_IAM authentication:
+try:
+    from botocore.session import Session as BotoSession
+except ImportError:
+    # no botocore available, will disable AWS_MSK_IAM mechanism
+    BotoSession = None
+
 from typing import Optional
 
 
+def validate_config(conn):
+    assert BotoSession is not None, 'AWS_MSK_IAM requires the "botocore" package'
+    assert conn.config.get('security_protocol') == 'SASL_SSL', 'AWS_MSK_IAM requires SASL_SSL'
+
 def try_authenticate(self, future):
 
     session = BotoSession()
     credentials = session.get_credentials().get_frozen_credentials()
     client = AwsMskIamClient(
         host=self.host,
         access_key=credentials.access_key,
         secret_key=credentials.secret_key,
         region=session.get_config_variable('region'),
         token=credentials.token,
     )
-    
+
     msg = client.first_message()
     size = Int32.encode(len(msg))
 
     err = None
     close = False
     with self._lock:
         if not self._can_send_recv():
```

### Comparing `kafka-python-ng-2.2.0/kafka/sasl/oauthbearer.py` & `kafka-python-ng-2.2.1/kafka/sasl/oauthbearer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/sasl/plain.py` & `kafka-python-ng-2.2.1/kafka/sasl/plain.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/sasl/scram.py` & `kafka-python-ng-2.2.1/kafka/sasl/scram.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/scram.py` & `kafka-python-ng-2.2.1/kafka/scram.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/structs.py` & `kafka-python-ng-2.2.1/kafka/structs.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka/util.py` & `kafka-python-ng-2.2.1/kafka/util.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/kafka_python_ng.egg-info/PKG-INFO` & `kafka-python-ng-2.2.1/kafka_python_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-python-ng
-Version: 2.2.0
+Version: 2.2.1
 Summary: Pure Python client for Apache Kafka
 Home-page: https://github.com/wbarnha/kafka-python-ng
 Author: Dana Powers
 Author-email: dana.powers@gmail.com
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 License: Apache License 2.0
```

### Comparing `kafka-python-ng-2.2.0/kafka_python_ng.egg-info/SOURCES.txt` & `kafka-python-ng-2.2.1/kafka_python_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.10.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.10.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.10.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.10.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.10.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.10.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.10.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.10.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.10.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.2.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.10.2.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.2.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.10.2.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.2.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.10.2.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.2.2/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.10.2.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.2.2/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.10.2.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.10.2.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.10.2.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.2/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.2/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.3/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.3/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.3/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.3/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.11.0.3/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.11.0.3/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.8.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.8.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.8.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.8.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.8.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.8.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.8.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.8.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.8.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.2/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.2/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.8.2.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.8.2.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.9.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.9.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.9.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.9.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.9.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.9.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.9.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/0.9.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.9.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/0.9.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/0.9.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/0.9.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/1.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/1.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/1.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/1.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/1.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/1.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.2/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/1.0.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.2/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/1.0.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.0.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/1.0.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.1.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/1.1.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.1.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/1.1.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.1.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/1.1.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/1.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/1.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/1.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/1.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.1.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.1.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.1.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.1.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.1.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.1.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.2.1/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.2.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.2.1/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.2.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.2.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.2.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.3.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.3.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.3.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.3.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.3.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.3.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.4.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.4.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.4.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.4.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.4.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.4.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.5.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.5.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.5.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.5.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.5.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.5.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.6.0/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/2.6.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.6.0/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/2.6.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/2.6.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/2.6.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/trunk/resources/kafka.properties` & `kafka-python-ng-2.2.1/servers/trunk/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/trunk/resources/log4j.properties` & `kafka-python-ng-2.2.1/servers/trunk/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/servers/trunk/resources/zookeeper.properties` & `kafka-python-ng-2.2.1/servers/trunk/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/setup.py` & `kafka-python-ng-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/conftest.py` & `kafka-python-ng-2.2.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/fixtures.py` & `kafka-python-ng-2.2.1/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/record/test_default_records.py` & `kafka-python-ng-2.2.1/test/record/test_default_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/record/test_legacy_records.py` & `kafka-python-ng-2.2.1/test/record/test_legacy_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/record/test_records.py` & `kafka-python-ng-2.2.1/test/record/test_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/record/test_util.py` & `kafka-python-ng-2.2.1/test/record/test_util.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/service.py` & `kafka-python-ng-2.2.1/test/service.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_acl_comparisons.py` & `kafka-python-ng-2.2.1/test/test_acl_comparisons.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_admin.py` & `kafka-python-ng-2.2.1/test/test_admin.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_admin_integration.py` & `kafka-python-ng-2.2.1/test/test_admin_integration.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_api_object_implementation.py` & `kafka-python-ng-2.2.1/test/test_api_object_implementation.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_assignors.py` & `kafka-python-ng-2.2.1/test/test_assignors.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_client_async.py` & `kafka-python-ng-2.2.1/test/test_client_async.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_cluster.py` & `kafka-python-ng-2.2.1/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_codec.py` & `kafka-python-ng-2.2.1/test/test_codec.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_consumer.py` & `kafka-python-ng-2.2.1/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_consumer_group.py` & `kafka-python-ng-2.2.1/test/test_consumer_group.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_consumer_integration.py` & `kafka-python-ng-2.2.1/test/test_consumer_integration.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_coordinator.py` & `kafka-python-ng-2.2.1/test/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_fetcher.py` & `kafka-python-ng-2.2.1/test/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_metrics.py` & `kafka-python-ng-2.2.1/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_msk.py` & `kafka-python-ng-2.2.1/test/test_msk.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_object_conversion.py` & `kafka-python-ng-2.2.1/test/test_object_conversion.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_package.py` & `kafka-python-ng-2.2.1/test/test_package.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_partition_movements.py` & `kafka-python-ng-2.2.1/test/test_partition_movements.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_partitioner.py` & `kafka-python-ng-2.2.1/test/test_partitioner.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_producer.py` & `kafka-python-ng-2.2.1/test/test_producer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_protocol.py` & `kafka-python-ng-2.2.1/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_sasl_integration.py` & `kafka-python-ng-2.2.1/test/test_sasl_integration.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_sender.py` & `kafka-python-ng-2.2.1/test/test_sender.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/test_subscription_state.py` & `kafka-python-ng-2.2.1/test/test_subscription_state.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/test/testutil.py` & `kafka-python-ng-2.2.1/test/testutil.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/tox.ini` & `kafka-python-ng-2.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.0/travis_java_install.sh` & `kafka-python-ng-2.2.1/travis_java_install.sh`

 * *Files identical despite different names*

