# Comparing `tmp/dagster-graphql-1.6.9.tar.gz` & `tmp/dagster-graphql-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.6.9.tar", last modified: Fri Mar  8 00:18:59 2024, max compression
+gzip compressed data, was "dagster-graphql-1.7.0.tar", last modified: Thu Apr  4 19:44:59 2024, max compression
```

## Comparing `dagster-graphql-1.6.9.tar` & `dagster-graphql-1.7.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.590130 dagster-graphql-1.6.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      691 2024-03-08 00:18:59.590130 dagster-graphql-1.6.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.562130 dagster-graphql-1.6.9/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7401 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.566130 dagster-graphql-1.6.9/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18331 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.570130 dagster-graphql-1.6.9/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12922 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/asset_checks_loader.py
--rw-r--r--   0 root         (0) root         (0)    19744 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.570130 dagster-graphql-1.6.9/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    14565 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12574 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4837 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4891 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7306 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)     4245 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_asset_checks.py
--rw-r--r--   0 root         (0) root         (0)     4926 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    28765 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12677 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14715 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     9078 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10361 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_ticks.py
--rw-r--r--   0 root         (0) root         (0)    15794 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     9780 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.582130 dagster-graphql-1.6.9/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8023 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    11979 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    54561 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/asset_selections.py
--rw-r--r--   0 root         (0) root         (0)    10990 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     2586 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    20865 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    17941 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    18888 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    13772 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)    11532 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28784 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/instigation.py
--rw-r--r--   0 root         (0) root         (0)      232 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/instigators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.582130 dagster-graphql-1.6.9/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    21701 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4813 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)      529 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/partition_mappings.py
--rw-r--r--   0 root         (0) root         (0)    17811 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.586130 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11058 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39334 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     9021 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.586130 dagster-graphql-1.6.9/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    32263 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    46584 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5088 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     6523 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.586130 dagster-graphql-1.6.9/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     4945 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9133 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)    10192 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    30053 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.590130 dagster-graphql-1.6.9/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:59.562130 dagster-graphql-1.6.9/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      691 2024-03-08 00:18:59.000000 dagster-graphql-1.6.9/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4726 2024-03-08 00:18:59.000000 dagster-graphql-1.6.9/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:18:59.000000 dagster-graphql-1.6.9/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-03-08 00:18:59.000000 dagster-graphql-1.6.9/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-08 00:18:59.000000 dagster-graphql-1.6.9/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-08 00:18:59.000000 dagster-graphql-1.6.9/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-03-08 00:18:59.590130 dagster-graphql-1.6.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1531 2024-03-08 00:17:46.000000 dagster-graphql-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.955944 dagster-graphql-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      691 2024-04-04 19:44:59.955944 dagster-graphql-1.7.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.943944 dagster-graphql-1.7.0/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.943944 dagster-graphql-1.7.0/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.947944 dagster-graphql-1.7.0/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/asset_checks_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20532 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.947944 dagster-graphql-1.7.0/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    28943 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10352 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_ticks.py
+-rw-r--r--   0 root         (0) root         (0)    15798 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.951944 dagster-graphql-1.7.0/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8116 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    54797 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/asset_selections.py
+-rw-r--r--   0 root         (0) root         (0)    10990 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    20849 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    17941 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18785 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13742 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    11731 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28766 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/instigation.py
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/instigators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.951944 dagster-graphql-1.7.0/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    21701 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/partition_mappings.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.955944 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    40100 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     9025 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.955944 dagster-graphql-1.7.0/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    32162 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    46505 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.955944 dagster-graphql-1.7.0/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.955944 dagster-graphql-1.7.0/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7078 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:59.943944 dagster-graphql-1.7.0/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      691 2024-04-04 19:44:59.000000 dagster-graphql-1.7.0/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-04-04 19:44:59.000000 dagster-graphql-1.7.0/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:44:59.000000 dagster-graphql-1.7.0/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-04 19:44:59.000000 dagster-graphql-1.7.0/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-04 19:44:59.000000 dagster-graphql-1.7.0/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 19:44:59.000000 dagster-graphql-1.7.0/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-04 19:44:59.959944 dagster-graphql-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-04-04 19:44:07.000000 dagster-graphql-1.7.0/setup.py
```

### Comparing `dagster-graphql-1.6.9/LICENSE` & `dagster-graphql-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/PKG-INFO` & `dagster-graphql-1.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.6.9
+Version: 1.7.0
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/cli.py` & `dagster-graphql-1.7.0/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/client/client.py` & `dagster-graphql-1.7.0/dagster_graphql/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 import requests.exceptions
 from dagster import DagsterRunStatus
 from dagster._annotations import deprecated, public
 from dagster._core.definitions.run_config import RunConfig, convert_config_input
-from dagster._core.definitions.utils import validate_tags
+from dagster._core.definitions.utils import normalize_tags
 from gql import Client, gql
 from gql.transport import Transport
 from gql.transport.requests import RequestsHTTPTransport
 
 from .client_queries import (
     CLIENT_GET_REPO_LOCATIONS_NAMES_AND_PIPELINES_QUERY,
     CLIENT_SUBMIT_PIPELINE_RUN_MUTATION,
@@ -139,15 +139,15 @@
 
         # The following invariant will never fail when a job is executed
         check.invariant(
             (mode is not None and run_config is not None) or preset is not None,
             "Either a mode and run_config or a preset must be specified in order to "
             f"submit the pipeline {pipeline_name} for execution",
         )
-        tags = validate_tags(tags)
+        tags = normalize_tags(tags).tags
 
         pipeline_or_job = "Job" if is_using_job_op_graph_apis else "Pipeline"
 
         if not repository_location_name or not repository_name:
             job_info_lst = self._get_repo_locations_and_names_with_pipeline(pipeline_name)
             if len(job_info_lst) == 0:
                 raise DagsterGraphQLClientError(
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.7.0/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/client/query.py` & `dagster-graphql-1.7.0/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/client/utils.py` & `dagster-graphql-1.7.0/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/asset_checks_loader.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/asset_checks_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 from dagster import (
     _check as check,
 )
 from dagster._core.definitions.asset_check_evaluation import AssetCheckEvaluation
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.selector import RepositorySelector
-from dagster._core.host_representation.code_location import CodeLocation
-from dagster._core.host_representation.external import ExternalRepository
-from dagster._core.host_representation.external_data import ExternalAssetCheck
 from dagster._core.instance import DagsterInstance
+from dagster._core.remote_representation.code_location import CodeLocation
+from dagster._core.remote_representation.external import ExternalRepository
+from dagster._core.remote_representation.external_data import ExternalAssetCheck
 from dagster._core.storage.asset_check_execution_record import (
     AssetCheckExecutionRecord,
     AssetCheckExecutionResolvedStatus,
     AssetCheckInstanceSupport,
 )
 from dagster._core.storage.event_log.base import AssetRecord
 from dagster._core.workspace.context import WorkspaceRequestContext
@@ -121,26 +120,26 @@
             for external_checks in external_checks_by_asset_key.values()
             for external_check in external_checks
         ]
         execution_loader = AssetChecksExecutionForLatestMaterializationLoader(
             self._context.instance, check_keys=all_check_keys
         )
 
-        asset_graph = ExternalAssetGraph.from_workspace(self._context)
+        asset_graph = self._context.asset_graph
         graphene_checks: Mapping[AssetKey, AssetChecksOrErrorUnion] = {}
         for asset_key in self._asset_keys:
             if asset_key in errors:
                 graphene_checks[asset_key] = errors[asset_key]
             else:
                 graphene_checks_for_asset = []
                 for external_check in external_checks_by_asset_key.get(asset_key, []):
                     can_execute_individually = (
                         GrapheneAssetCheckCanExecuteIndividually.CAN_EXECUTE
                         if len(
-                            asset_graph.get_required_asset_and_check_keys(external_check.key) or []
+                            asset_graph.get_execution_set_asset_and_check_keys(external_check.key)
                         )
                         <= 1
                         # NOTE: once we support multi checks, we'll need to add a case for
                         # non subsettable multi checks
                         else GrapheneAssetCheckCanExecuteIndividually.REQUIRES_MATERIALIZATION
                     )
                     graphene_checks_for_asset.append(
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/events.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
     NotebookMetadataValue,
     NullMetadataValue,
     PathMetadataValue,
     PythonArtifactMetadataValue,
     TableMetadataValue,
     TableSchemaMetadataValue,
     TextMetadataValue,
+    TimestampMetadataValue,
     UrlMetadataValue,
 )
 from dagster._core.definitions.asset_check_evaluation import AssetCheckEvaluationPlanned
 from dagster._core.definitions.metadata import (
     DagsterRunMetadataValue,
     MetadataValue,
+    TableColumnLineageMetadataValue,
 )
 from dagster._core.events import (
     DagsterEventType,
     HandledOutputData,
     LoadedInputData,
     StepExpectationResultData,
 )
@@ -49,17 +51,20 @@
         GrapheneJsonMetadataEntry,
         GrapheneMarkdownMetadataEntry,
         GrapheneNotebookMetadataEntry,
         GrapheneNullMetadataEntry,
         GraphenePathMetadataEntry,
         GraphenePipelineRunMetadataEntry,
         GraphenePythonArtifactMetadataEntry,
+        GrapheneTableColumnLineageEntry,
+        GrapheneTableColumnLineageMetadataEntry,
         GrapheneTableMetadataEntry,
         GrapheneTableSchemaMetadataEntry,
         GrapheneTextMetadataEntry,
+        GrapheneTimestampMetadataEntry,
         GrapheneUrlMetadataEntry,
     )
     from ..schema.table import GrapheneTable, GrapheneTableSchema
 
     check.mapping_param(metadata, "metadata", key_type=str)
     for key, value in metadata.items():
         if isinstance(value, PathMetadataValue):
@@ -159,14 +164,26 @@
             yield GrapheneTableSchemaMetadataEntry(
                 label=key,
                 schema=GrapheneTableSchema(
                     constraints=value.schema.constraints,
                     columns=value.schema.columns,
                 ),
             )
+        elif isinstance(value, TableColumnLineageMetadataValue):
+            yield GrapheneTableColumnLineageMetadataEntry(
+                label=key,
+                lineage=[
+                    GrapheneTableColumnLineageEntry(
+                        column_name=column_name, column_deps=column_deps
+                    )
+                    for column_name, column_deps in value.column_lineage.deps_by_column.items()
+                ],
+            )
+        elif isinstance(value, TimestampMetadataValue):
+            yield GrapheneTimestampMetadataEntry(label=key, timestamp=value.value)
         else:
             # skip rest for now
             check.not_implemented(f"{type(value)} unsupported metadata entry for now")
 
 
 def _to_metadata_entries(metadata: Mapping[str, MetadataValue]) -> Sequence[Any]:
     return list(iterate_metadata_entries(metadata or {}))
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/execution/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,15 @@
     can_cancel_run = run.status in CANCELABLE_RUN_STATUSES
 
     valid_status = not run.is_finished and (force_mark_as_canceled or can_cancel_run)
 
     if not valid_status:
         return GrapheneTerminateRunFailure(
             run=graphene_run,
-            message="Run {run_id} could not be terminated due to having status {status}.".format(
-                run_id=run.run_id, status=run.status.value
-            ),
+            message=f"Run {run.run_id} could not be terminated due to having status {run.status.value}.",
         )
 
     if force_mark_as_canceled:
         try:
             if instance.run_coordinator and can_cancel_run:
                 instance.run_coordinator.cancel_run(run_id)
         except:
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/execution/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import TYPE_CHECKING, List, Sequence, Union, cast
 
 import dagster._check as check
 import pendulum
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.selector import PartitionsByAssetSelector, RepositorySelector
 from dagster._core.errors import (
     DagsterError,
     DagsterInvariantViolationError,
     DagsterUserCodeProcessError,
 )
 from dagster._core.events import AssetKey
 from dagster._core.execution.asset_backfill import create_asset_backfill_data_from_asset_partitions
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
 from dagster._core.execution.job_backfill import submit_backfill_runs
-from dagster._core.host_representation.external_data import ExternalPartitionExecutionErrorData
+from dagster._core.remote_representation.external_data import ExternalPartitionExecutionErrorData
 from dagster._core.utils import make_new_backfill_id
 from dagster._core.workspace.permissions import Permissions
 from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
 from ..utils import (
     AssetBackfillPreviewParams,
@@ -42,15 +41,15 @@
 
 
 def get_asset_backfill_preview(
     graphene_info: "ResolveInfo", backfill_preview_params: AssetBackfillPreviewParams
 ) -> Sequence["GrapheneAssetPartitions"]:
     from ...schema.backfill import GrapheneAssetPartitions
 
-    asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+    asset_graph = graphene_info.context.asset_graph
 
     check.invariant(backfill_preview_params.get("assetSelection") is not None)
     check.invariant(backfill_preview_params.get("partitionNames") is not None)
 
     asset_selection = [
         cast(AssetKey, AssetKey.from_graphql_input(asset_key))
         for asset_key in backfill_preview_params["assetSelection"]
@@ -60,15 +59,15 @@
     asset_backfill_data = create_asset_backfill_data_from_asset_partitions(
         asset_graph, asset_selection, partition_names, graphene_info.context.instance
     )
 
     asset_partitions = []
 
     for asset_key in asset_backfill_data.get_targeted_asset_keys_topological_order(asset_graph):
-        if asset_graph.get_partitions_def(asset_key):
+        if asset_graph.get(asset_key).partitions_def:
             partitions_subset = asset_backfill_data.target_subset.partitions_subsets_by_asset_key[
                 asset_key
             ]
             asset_partitions.append(
                 GrapheneAssetPartitions(asset_key=asset_key, partitions_subset=partitions_subset)
             )
         else:
@@ -131,17 +130,15 @@
             if partition_set.name == partition_set_selector.get("partitionSetName")
         ]
         if not matches:
             return GraphenePartitionSetNotFoundError(partition_set_name)
 
         if len(matches) != 1:
             raise DagsterInvariantViolationError(
-                "Partition set names must be unique: found {num} matches for {partition_set_name}".format(
-                    num=len(matches), partition_set_name=partition_set_name
-                )
+                f"Partition set names must be unique: found {len(matches)} matches for {partition_set_name}"
             )
         external_partition_set = next(iter(matches))
 
         if backfill_params.get("allPartitions"):
             result = graphene_info.context.get_external_partition_names(
                 external_partition_set, instance=graphene_info.context.instance
             )
@@ -194,15 +191,15 @@
             raise DagsterError(
                 "forceSynchronousSubmission is not supported for pure asset backfills"
             )
 
         if backfill_params.get("fromFailure"):
             raise DagsterError("fromFailure is not supported for pure asset backfills")
 
-        asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+        asset_graph = graphene_info.context.asset_graph
 
         assert_permission_for_asset_graph(
             graphene_info, asset_graph, asset_selection, Permissions.LAUNCH_PARTITION_BACKFILL
         )
 
         backfill = PartitionBackfill.from_asset_partitions(
             asset_graph=asset_graph,
@@ -223,15 +220,15 @@
             raise DagsterError(
                 "forceSynchronousSubmission is not supported for pure asset backfills"
             )
 
         if backfill_params.get("fromFailure"):
             raise DagsterError("fromFailure is not supported for pure asset backfills")
 
-        asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+        asset_graph = graphene_info.context.asset_graph
         assert_permission_for_asset_graph(
             graphene_info, asset_graph, asset_selection, Permissions.LAUNCH_PARTITION_BACKFILL
         )
         backfill = PartitionBackfill.from_partitions_by_assets(
             backfill_id=backfill_id,
             asset_graph=asset_graph,
             backfill_timestamp=backfill_timestamp,
@@ -261,15 +258,15 @@
     from ...schema.backfill import GrapheneCancelBackfillSuccess
 
     backfill = graphene_info.context.instance.get_backfill(backfill_id)
     if not backfill:
         check.failed(f"No backfill found for id: {backfill_id}")
 
     if backfill.is_asset_backfill:
-        asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+        asset_graph = graphene_info.context.asset_graph
         assert_permission_for_asset_graph(
             graphene_info,
             asset_graph,
             backfill.asset_selection,
             Permissions.CANCEL_PARTITION_BACKFILL,
         )
         graphene_info.context.instance.update_backfill(
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from ...schema.inputs import GrapheneRepositorySelector
     from ...schema.partition_sets import GrapheneAddDynamicPartitionSuccess
 
 
 def _repository_contains_dynamic_partitions_def(
     graphene_info, repository_selector: RepositorySelector, partitions_def_name: str
 ) -> bool:
-    from dagster._core.host_representation.external_data import (
+    from dagster._core.remote_representation.external_data import (
         ExternalDynamicPartitionsDefinitionData,
         ExternalMultiPartitionsDefinitionData,
         ExternalPartitionsDefinitionData,
     )
 
     def _is_matching_partitions_def(partitions_def_data: ExternalPartitionsDefinitionData):
         if isinstance(partitions_def_data, ExternalDynamicPartitionsDefinitionData):
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 
     instance: DagsterInstance = graphene_info.context.instance
     parent_run = check.not_none(
         instance.get_run_by_id(parent_run_id), f"Could not find parent run with id: {parent_run_id}"
     )
     origin = check.not_none(parent_run.external_job_origin)
     selector = JobSubsetSelector(
-        location_name=origin.external_repository_origin.code_location_origin.location_name,
-        repository_name=origin.external_repository_origin.repository_name,
+        location_name=origin.repository_origin.code_location_origin.location_name,
+        repository_name=origin.repository_origin.repository_name,
         job_name=parent_run.job_name,
         asset_selection=parent_run.asset_selection,
         asset_check_selection=parent_run.asset_check_selection,
         op_selection=None,
     )
 
     assert_permission_for_location(
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple, cast
 
 import dagster._check as check
 from dagster._core.errors import DagsterRunNotFoundError
 from dagster._core.execution.plan.state import KnownExecutionState
-from dagster._core.host_representation import CodeLocation
-from dagster._core.host_representation.external import ExternalJob
 from dagster._core.instance import DagsterInstance
+from dagster._core.remote_representation import CodeLocation
+from dagster._core.remote_representation.external import ExternalJob
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
 from dagster._core.storage.tags import RESUME_RETRY_TAG
 from dagster._core.utils import make_new_run_id
 from dagster._utils.merger import merge_dicts
 
 from ..external import ensure_valid_config, get_external_execution_plan_or_raise
 from ..utils import ExecutionParams
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/external.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._config import validate_config_from_snap
 from dagster._core.definitions.selector import JobSubsetSelector, RepositorySelector
 from dagster._core.execution.plan.state import KnownExecutionState
-from dagster._core.host_representation import ExternalJob
-from dagster._core.host_representation.external import ExternalExecutionPlan
+from dagster._core.remote_representation import ExternalJob
+from dagster._core.remote_representation.external import ExternalExecutionPlan
 from dagster._core.workspace.context import BaseWorkspaceRequestContext, WorkspaceRequestContext
 from dagster._utils.error import serializable_error_info_from_exc_info
 
 from .utils import UserFacingGraphQLError
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.errors import GrapheneRepositoryNotFoundError
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_asset_checks.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_asset_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TYPE_CHECKING, Iterator, List, Mapping, Optional, Sequence, Tuple
 
 import dagster._check as check
 from dagster import AssetKey
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
-from dagster._core.host_representation.code_location import CodeLocation
-from dagster._core.host_representation.external import ExternalRepository
-from dagster._core.host_representation.external_data import ExternalAssetCheck
 from dagster._core.instance import DagsterInstance
+from dagster._core.remote_representation.code_location import CodeLocation
+from dagster._core.remote_representation.external import ExternalRepository
+from dagster._core.remote_representation.external_data import ExternalAssetCheck
 from dagster._core.storage.asset_check_execution_record import (
     AssetCheckExecutionRecord,
     AssetCheckExecutionRecordStatus,
     AssetCheckExecutionResolvedStatus,
 )
 from dagster._core.storage.dagster_run import DagsterRunStatus, RunsFilter
 from dagster._core.workspace.context import WorkspaceRequestContext
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_asset_condition_evaluations.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     AssetKey,
     DagsterInstance,
     MultiPartitionsDefinition,
     _check as check,
 )
 from dagster._core.definitions.asset_graph_differ import AssetGraphDiffer
 from dagster._core.definitions.data_time import CachingDataTimeResolver
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import (
     CachingDynamicPartitionsLoader,
     PartitionsDefinition,
     PartitionsSubset,
 )
 from dagster._core.definitions.time_window_partitions import (
     BaseTimeWindowPartitionsSubset,
@@ -35,18 +34,18 @@
     TimeWindowPartitionsDefinition,
     TimeWindowPartitionsSubset,
     fetch_flattened_time_window_ranges,
 )
 from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.events import ASSET_EVENTS
 from dagster._core.events.log import EventLogEntry
-from dagster._core.host_representation.code_location import CodeLocation
-from dagster._core.host_representation.external import ExternalRepository
-from dagster._core.host_representation.external_data import ExternalAssetNode
 from dagster._core.instance import DynamicPartitionsStore
+from dagster._core.remote_representation.code_location import CodeLocation
+from dagster._core.remote_representation.external import ExternalRepository
+from dagster._core.remote_representation.external_data import ExternalAssetNode
 from dagster._core.storage.event_log.sql_event_log import get_max_event_records_limit
 from dagster._core.storage.partition_status_cache import (
     build_failed_and_in_progress_partition_subset,
     get_and_update_asset_status_cache_value,
     get_materialized_multipartitions,
     get_validated_partition_keys,
     is_cacheable_partition_type,
@@ -141,24 +140,25 @@
 
 def get_additional_required_keys(
     graphene_info: "ResolveInfo", asset_keys: AbstractSet[AssetKey]
 ) -> List["AssetKey"]:
     asset_nodes_by_key = get_asset_nodes_by_asset_key(graphene_info)
 
     # the set of atomic execution ids that any of the input asset keys are a part of
-    required_atomic_execution_ids = {
-        asset_nodes_by_key[asset_key].external_asset_node.atomic_execution_unit_id
+    required_execution_set_identifiers = {
+        asset_nodes_by_key[asset_key].external_asset_node.execution_set_identifier
         for asset_key in asset_keys
     } - {None}
 
-    # the set of all asset keys that are part of the required atomic execution units
+    # the set of all asset keys that are part of the required execution sets
     required_asset_keys = {
         asset_node.external_asset_node.asset_key
         for asset_node in asset_nodes_by_key.values()
-        if asset_node.external_asset_node.atomic_execution_unit_id in required_atomic_execution_ids
+        if asset_node.external_asset_node.execution_set_identifier
+        in required_execution_set_identifiers
     }
 
     return list(required_asset_keys - asset_keys)
 
 
 def get_asset_node_definition_collisions(
     graphene_info: "ResolveInfo", asset_keys: AbstractSet[AssetKey]
@@ -206,27 +206,31 @@
     from ..schema.asset_graph import GrapheneAssetNode
     from .asset_checks_loader import AssetChecksLoader
 
     depended_by_loader = CrossRepoAssetDependedByLoader(context=graphene_info.context)
 
     stale_status_loader = StaleStatusLoader(
         instance=graphene_info.context.instance,
-        asset_graph=lambda: ExternalAssetGraph.from_workspace(graphene_info.context),
+        asset_graph=lambda: graphene_info.context.asset_graph,
     )
 
     dynamic_partitions_loader = CachingDynamicPartitionsLoader(graphene_info.context.instance)
 
     asset_nodes_by_asset_key: Dict[
         AssetKey, Tuple[CodeLocation, ExternalRepository, ExternalAssetNode]
     ] = {}
     for repo_loc, repo, external_asset_node in asset_node_iter(graphene_info):
         _, _, preexisting_asset_node = asset_nodes_by_asset_key.get(
             external_asset_node.asset_key, (None, None, None)
         )
-        if preexisting_asset_node is None or preexisting_asset_node.is_source:
+        # If an asset node is already in the dict, we only overwrite it if that preexisting node is
+        # not executable in some manner (i.e. it is a source asset that is not an observable)
+        if preexisting_asset_node is None or (
+            preexisting_asset_node.is_source and not preexisting_asset_node.is_observable
+        ):
             if asset_keys is None or external_asset_node.asset_key in asset_keys:
                 asset_nodes_by_asset_key[external_asset_node.asset_key] = (
                     repo_loc,
                     repo,
                     external_asset_node,
                 )
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dagster_graphql.schema.env_vars import (
     GrapheneEnvVarWithConsumers,
     GrapheneEnvVarWithConsumersList,
     GrapheneEnvVarWithConsumersListOrError,
 )
 
 if TYPE_CHECKING:
-    from dagster._core.host_representation.code_location import CodeLocation
+    from dagster._core.remote_representation.code_location import CodeLocation
 
 
 def get_utilized_env_vars_or_error(
     graphene_info, repository_selector
 ) -> GrapheneEnvVarWithConsumersListOrError:
     check.inst_param(graphene_info, "graphene_info", ResolveInfo)
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections import defaultdict
 from typing import TYPE_CHECKING, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._core.definitions.selector import RepositorySelector
 from dagster._core.errors import DagsterUserCodeProcessError
-from dagster._core.host_representation import (
+from dagster._core.remote_representation import (
     ExternalPartitionSet,
     RepositoryHandle,
 )
-from dagster._core.host_representation.external_data import (
+from dagster._core.remote_representation.external_data import (
     ExternalPartitionExecutionErrorData,
     ExternalPartitionNamesData,
 )
 from dagster._core.storage.dagster_run import DagsterRunStatus, RunPartitionData, RunsFilter
 from dagster._core.storage.tags import (
     PARTITION_NAME_TAG,
     PARTITION_SET_TAG,
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import dagster._check as check
 from dagster._core.definitions.selector import RepositorySelector, ResourceSelector
 from graphene import ResolveInfo
 
 from .utils import UserFacingGraphQLError
 
 if TYPE_CHECKING:
-    from dagster._core.host_representation.code_location import CodeLocation
+    from dagster._core.remote_representation.code_location import CodeLocation
 
     from ..schema.resources import GrapheneResourceDetails, GrapheneResourceDetailsList
 
 
 def get_top_level_resources_or_error(
     graphene_info: "ResolveInfo", repository_selector: RepositorySelector
 ) -> "GrapheneResourceDetailsList":
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             if get_tag_type(tag_key) != TagType.HIDDEN
         ]
     )
 
 
 def get_run_tags(
     graphene_info: "ResolveInfo",
-    tag_keys: Optional[List[str]] = None,
+    tag_keys: List[str],
     value_prefix: Optional[str] = None,
     limit: Optional[int] = None,
 ) -> "GrapheneRunTags":
     from ..schema.runs import GrapheneRunTags
     from ..schema.tags import GraphenePipelineTagAndValues
 
     instance = graphene_info.context.instance
@@ -202,14 +202,27 @@
             if asset_record.asset_entry.last_materialization
             and asset_record.asset_entry.asset_key in step_keys_by_asset
             else None
         )
         for asset_record in asset_records
     }
 
+    # Build a lookup table of asset keys to last materialization run IDs. We will filter these
+    # run IDs out of the "in progress" run lists that are generated below since they have already
+    # emitted an output for the run.
+    latest_materialization_run_id_by_asset: Dict[AssetKey, Optional[str]] = {
+        asset_record.asset_entry.asset_key: (
+            asset_record.asset_entry.last_materialization.run_id
+            if asset_record.asset_entry.last_materialization
+            and asset_record.asset_entry.asset_key in step_keys_by_asset
+            else None
+        )
+        for asset_record in asset_records
+    }
+
     latest_run_ids_by_asset: Dict[
         AssetKey, str
     ] = {  # last_run_id column is written to upon run creation (via ASSET_MATERIALIZATION_PLANNED event)
         asset_record.asset_entry.asset_key: asset_record.asset_entry.last_run_id
         for asset_record in asset_records
         if asset_record.asset_entry.last_run_id
     }
@@ -223,15 +236,20 @@
             if run_record.dagster_run.status in PENDING_STATUSES:
                 in_progress_records.append(run_record)
             run_records_by_run_id[run_record.dagster_run.run_id] = run_record
 
     (
         in_progress_run_ids_by_asset,
         unstarted_run_ids_by_asset,
-    ) = _get_in_progress_runs_for_assets(graphene_info, in_progress_records, step_keys_by_asset)
+    ) = _get_in_progress_runs_for_assets(
+        graphene_info,
+        in_progress_records,
+        step_keys_by_asset,
+        latest_materialization_run_id_by_asset,
+    )
 
     from .fetch_assets import get_unique_asset_id
 
     return [
         GrapheneAssetLatestInfo(
             (
                 get_unique_asset_id(
@@ -259,14 +277,15 @@
     ]
 
 
 def _get_in_progress_runs_for_assets(
     graphene_info: "ResolveInfo",
     in_progress_records: Sequence[RunRecord],
     step_keys_by_asset: Mapping[AssetKey, Sequence[str]],
+    latest_materialization_run_id_by_asset: Dict[AssetKey, Optional[str]],
 ) -> Tuple[Mapping[AssetKey, AbstractSet[str]], Mapping[AssetKey, AbstractSet[str]]]:
     # Build mapping of step key to the assets it generates
     asset_key_by_step_key = defaultdict(set)
     for asset_key, step_keys in step_keys_by_asset.items():
         for step_key in step_keys:
             asset_key_by_step_key[step_key].add(asset_key)
 
@@ -293,14 +312,16 @@
             # Build mapping of asset to all the step stats that generate the asset
             step_stats_by_asset: Dict[AssetKey, List[RunStepKeyStatsSnapshot]] = defaultdict(list)
             for step_stat in step_stats:
                 for asset_key in asset_key_by_step_key[step_stat.step_key]:
                     step_stats_by_asset[asset_key].append(step_stat)
 
             for asset in selected_assets:
+                if latest_materialization_run_id_by_asset.get(asset) == run.run_id:
+                    continue
                 asset_step_stats = step_stats_by_asset.get(asset)
                 if asset_step_stats:
                     # asset_step_stats will contain all steps that are in progress or complete
                     if any(
                         [
                             step_stat.status == StepEventStatus.IN_PROGRESS
                             for step_stat in asset_step_stats
@@ -309,14 +330,16 @@
                         in_progress_run_ids_by_asset[asset].add(record.dagster_run.run_id)
                     # else if step_stats exist and none are in progress, the step has completed
                 else:  # if step stats is none, then the step has not started
                     unstarted_run_ids_by_asset[asset].add(record.dagster_run.run_id)
         else:
             # the run never began execution, all steps are unstarted
             for asset in selected_assets:
+                if latest_materialization_run_id_by_asset.get(asset) == run.run_id:
+                    continue
                 unstarted_run_ids_by_asset[asset].add(record.dagster_run.run_id)
 
     return in_progress_run_ids_by_asset, unstarted_run_ids_by_asset
 
 
 def get_runs_count(graphene_info: "ResolveInfo", filters: Optional[RunsFilter]) -> int:
     return graphene_info.context.instance.get_runs_count(filters)
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     graphene_info: ResolveInfo, schedule_state: InstigatorState
 ) -> Optional["GrapheneDryRunInstigationTick"]:
     from ..schema.instigation import GrapheneDryRunInstigationTick
 
     if not schedule_state.is_running:
         return None
 
-    repository_origin = schedule_state.origin.external_repository_origin
+    repository_origin = schedule_state.origin.repository_origin
     if not graphene_info.context.has_code_location(
         repository_origin.code_location_origin.location_name
     ):
         return None
     code_location = graphene_info.context.get_code_location(
         repository_origin.code_location_origin.location_name
     )
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 def get_sensor_next_tick(
     graphene_info: ResolveInfo, sensor_state: InstigatorState
 ) -> Optional["GrapheneDryRunInstigationTick"]:
     from ..schema.instigation import GrapheneDryRunInstigationTick
 
     check.inst_param(sensor_state, "sensor_state", InstigatorState)
 
-    repository_origin = sensor_state.origin.external_repository_origin
+    repository_origin = sensor_state.origin.repository_origin
     if not graphene_info.context.has_code_location(
         repository_origin.code_location_origin.location_name
     ):
         return None
 
     code_location = graphene_info.context.get_code_location(
         repository_origin.code_location_origin.location_name
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_solids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import OrderedDict, defaultdict
 
 import dagster._check as check
-from dagster._core.host_representation import ExternalRepository
+from dagster._core.remote_representation import ExternalRepository
 
 from .utils import GraphSelector
 
 
 def get_solid(repo, name):
     return get_used_solid_map(repo)[name]
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/fetch_ticks.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/fetch_ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     DagsterInstance,
     _check as check,
 )
 from dagster._core.definitions.asset_spec import AssetExecutionType
 from dagster._core.definitions.data_version import CachingStaleStatusResolver
 from dagster._core.definitions.events import AssetKey
 from dagster._core.events.log import EventLogEntry
-from dagster._core.host_representation import ExternalRepository
-from dagster._core.host_representation.external_data import (
+from dagster._core.remote_representation import ExternalRepository
+from dagster._core.remote_representation.external_data import (
     ExternalAssetDependedBy,
     ExternalAssetDependency,
     ExternalAssetNode,
 )
 from dagster._core.scheduler.instigation import InstigatorState, InstigatorType
 from dagster._core.storage.dagster_run import RunRecord, RunsFilter
 from dagster._core.workspace.context import WorkspaceRequestContext
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/run_config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Mapping, Optional
 
 import dagster._check as check
 from dagster._config import validate_config_from_snap
-from dagster._core.host_representation import RepresentedJob
-from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
+from dagster._core.remote_representation import RepresentedJob
+from dagster._core.remote_representation.external_data import DEFAULT_MODE_NAME
 
 from dagster_graphql.schema.errors import GrapheneModeNotFoundError
 from dagster_graphql.schema.util import ResolveInfo
 
 from .external import get_external_job_or_raise
 from .utils import JobSubsetSelector, UserFacingGraphQLError
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.7.0/dagster_graphql/implementation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
+from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
 from dagster._core.definitions.selector import GraphSelector, JobSubsetSelector
 from dagster._core.workspace.context import BaseWorkspaceRequestContext
 from dagster._utils.error import serializable_error_info_from_exc_info
 from typing_extensions import ParamSpec, TypeAlias
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.errors import GrapheneError, GraphenePythonError
@@ -84,15 +84,15 @@
     context = cast(BaseWorkspaceRequestContext, graphene_info.context)
     if not context.has_permission(permission):
         raise UserFacingGraphQLError(GrapheneUnauthorizedError())
 
 
 def assert_permission_for_asset_graph(
     graphene_info: "ResolveInfo",
-    asset_graph: ExternalAssetGraph,
+    asset_graph: RemoteAssetGraph,
     asset_selection: Optional[Sequence[AssetKey]],
     permission: str,
 ) -> None:
     asset_keys = set(asset_selection or [])
 
     # If any of the asset keys don't map to a location (e.g. because they are no longer in the
     # graph) need deployment-wide permissions - no valid code location to check
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/asset_checks.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/asset_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dagster import EventLogEntry
 from dagster._core.definitions.asset_check_evaluation import (
     AssetCheckEvaluation,
     AssetCheckEvaluationTargetMaterializationData,
 )
 from dagster._core.definitions.asset_check_spec import AssetCheckKey, AssetCheckSeverity
 from dagster._core.events import DagsterEventType
-from dagster._core.host_representation.external_data import ExternalAssetCheck
+from dagster._core.remote_representation.external_data import ExternalAssetCheck
 from dagster._core.storage.asset_check_execution_record import (
     AssetCheckExecutionRecord,
     AssetCheckExecutionResolvedStatus,
 )
 
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.schema.errors import GrapheneError
@@ -55,14 +55,15 @@
         graphene.NonNull(graphene.Float), description="When the check evaluation was stored"
     )
     checkName = graphene.NonNull(graphene.String)
     assetKey = graphene.NonNull(GrapheneAssetKey)
     targetMaterialization = graphene.Field(GrapheneAssetCheckEvaluationTargetMaterializationData)
     metadataEntries = non_null_list(GrapheneMetadataEntry)
     severity = graphene.NonNull(GrapheneAssetCheckSeverity)
+    description = graphene.String()
 
     # NOTE: this should be renamed passed
     success = graphene.NonNull(graphene.Boolean)
 
     class Meta:
         name = "AssetCheckEvaluation"
 
@@ -81,14 +82,15 @@
         )
 
         self.metadataEntries = list(iterate_metadata_entries(evaluation_data.metadata))
         self.severity = evaluation_data.severity
         self.success = evaluation_data.passed
         self.checkName = evaluation_data.check_name
         self.assetKey = evaluation_data.asset_key
+        self.description = evaluation_data.description
 
 
 class GrapheneAssetCheckExecution(graphene.ObjectType):
     id = graphene.NonNull(graphene.String)
     runId = graphene.NonNull(graphene.String)
     status = graphene.NonNull(GrapheneAssetCheckExecutionResolvedStatus)
     evaluation = graphene.Field(GrapheneAssetCheckEvaluation)
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/asset_condition_evaluations.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 import graphene
 from dagster import (
     AssetKey,
     _check as check,
 )
 from dagster._core.definitions.asset_graph_differ import AssetGraphDiffer, ChangeReason
-from dagster._core.definitions.assets_job import ASSET_BASE_JOB_PREFIX
+from dagster._core.definitions.asset_job import ASSET_BASE_JOB_PREFIX
 from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.data_version import (
     NULL_DATA_VERSION,
     StaleCauseCategory,
     StaleStatus,
 )
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader, PartitionsDefinition
 from dagster._core.definitions.partition_mapping import PartitionMapping
+from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
 from dagster._core.definitions.sensor_definition import (
     SensorType,
 )
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.event_api import EventRecordsFilter
 from dagster._core.events import DagsterEventType
-from dagster._core.host_representation import CodeLocation, ExternalRepository
-from dagster._core.host_representation.external import ExternalJob, ExternalSensor
-from dagster._core.host_representation.external_data import (
+from dagster._core.remote_representation import CodeLocation, ExternalRepository
+from dagster._core.remote_representation.external import ExternalJob, ExternalSensor
+from dagster._core.remote_representation.external_data import (
     ExternalAssetNode,
     ExternalDynamicPartitionsDefinitionData,
     ExternalMultiPartitionsDefinitionData,
     ExternalPartitionsDefinitionData,
     ExternalStaticPartitionsDefinitionData,
     ExternalTimeWindowPartitionsDefinitionData,
 )
@@ -57,14 +57,15 @@
 from dagster_graphql.schema.schedules import GrapheneSchedule
 from dagster_graphql.schema.sensors import GrapheneSensor
 from dagster_graphql.schema.solids import (
     GrapheneCompositeSolidDefinition,
     GrapheneResourceRequirement,
     GrapheneSolidDefinition,
 )
+from dagster_graphql.schema.tags import GrapheneDefinitionTag
 
 from ..implementation.fetch_assets import (
     build_partition_statuses,
     get_freshness_info,
     get_partition_subsets,
 )
 from ..implementation.loader import (
@@ -282,15 +283,15 @@
     dependencies = non_null_list(GrapheneAssetDependency)
     dependencyKeys = non_null_list(GrapheneAssetKey)
     description = graphene.String()
     freshnessInfo = graphene.Field(GrapheneAssetFreshnessInfo)
     freshnessPolicy = graphene.Field(GrapheneFreshnessPolicy)
     autoMaterializePolicy = graphene.Field(GrapheneAutoMaterializePolicy)
     graphName = graphene.String()
-    groupName = graphene.String()
+    groupName = graphene.NonNull(graphene.String)
     owners = non_null_list(GrapheneAssetOwner)
     id = graphene.NonNull(graphene.ID)
     isExecutable = graphene.NonNull(graphene.Boolean)
     isObservable = graphene.NonNull(graphene.Boolean)
     isPartitioned = graphene.NonNull(graphene.Boolean)
     isSource = graphene.NonNull(graphene.Boolean)
     jobNames = non_null_list(graphene.String)
@@ -299,14 +300,15 @@
         graphene.NonNull(graphene.List(GrapheneMaterializationEvent)),
         partitions=graphene.List(graphene.NonNull(graphene.String)),
     )
     latestRunForPartition = graphene.Field(GrapheneRun, partition=graphene.NonNull(graphene.String))
     assetPartitionStatuses = graphene.NonNull(GrapheneAssetPartitionStatuses)
     partitionStats = graphene.Field(GraphenePartitionStats)
     metadata_entries = non_null_list(GrapheneMetadataEntry)
+    tags = non_null_list(GrapheneDefinitionTag)
     op = graphene.Field(GrapheneSolidDefinition)
     opName = graphene.String()
     opNames = non_null_list(graphene.String)
     opVersion = graphene.String()
     partitionDefinition = graphene.Field(GraphenePartitionDefinition)
     partitionKeys = non_null_list(graphene.String)
     partitionKeysByDimension = graphene.Field(
@@ -561,15 +563,15 @@
         graphene_info: ResolveInfo,
         timestampMillis: str,
     ) -> Sequence[GrapheneMaterializationUpstreamDataVersion]:
         if not timestampMillis:
             return []
 
         instance = graphene_info.context.instance
-        asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
+        asset_graph = self._external_repository.asset_graph
         asset_key = self._external_asset_node.asset_key
 
         # in the future, we can share this same CachingInstanceQueryer across all
         # GrapheneMaterializationEvent which share an external repository for improved performance
         instance_queryer = CachingInstanceQueryer(
             instance=graphene_info.context.instance, asset_graph=asset_graph
         )
@@ -879,15 +881,15 @@
             for dep in self._external_asset_node.dependencies
         ]
 
     def resolve_freshnessInfo(
         self, graphene_info: ResolveInfo
     ) -> Optional[GrapheneAssetFreshnessInfo]:
         if self._external_asset_node.freshness_policy:
-            asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
+            asset_graph = self._external_repository.asset_graph
             return get_freshness_info(
                 asset_key=self._external_asset_node.asset_key,
                 # in the future, we can share this same CachingInstanceQueryer across all
                 # GrapheneAssetNodes which share an external repository for improved performance
                 data_time_resolver=CachingDataTimeResolver(
                     instance_queryer=CachingInstanceQueryer(
                         instance=graphene_info.context.instance,
@@ -908,30 +910,30 @@
         self, _graphene_info: ResolveInfo
     ) -> Optional[GrapheneAutoMaterializePolicy]:
         if self._external_asset_node.auto_materialize_policy:
             return GrapheneAutoMaterializePolicy(self._external_asset_node.auto_materialize_policy)
         return None
 
     def _sensor_targets_asset(
-        self, sensor: ExternalSensor, asset_graph: ExternalAssetGraph, job_names: Set[str]
+        self, sensor: ExternalSensor, asset_graph: RemoteAssetGraph, job_names: Set[str]
     ) -> bool:
         asset_key = self._external_asset_node.asset_key
 
         if sensor.asset_selection is not None and (
             asset_key in sensor.asset_selection.resolve(asset_graph)
         ):
             return True
 
         return any(target.job_name in job_names for target in sensor.get_external_targets())
 
     def resolve_targetingInstigators(self, graphene_info) -> Sequence[GrapheneSensor]:
         external_sensors = self._external_repository.get_external_sensors()
         external_schedules = self._external_repository.get_external_schedules()
 
-        asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
+        asset_graph = self._external_repository.asset_graph
 
         job_names = {
             job_name
             for job_name in self._external_asset_node.job_names
             if not job_name.startswith(ASSET_BASE_JOB_PREFIX)
         }
 
@@ -953,15 +955,15 @@
                     external_schedule.selector_id,
                 )
                 results.append(GrapheneSchedule(external_schedule, schedule_state))
 
         return results
 
     def _get_auto_materialize_external_sensor(self) -> Optional[ExternalSensor]:
-        asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
+        asset_graph = self._external_repository.asset_graph
 
         asset_key = self._external_asset_node.asset_key
         matching_sensors = [
             sensor
             for sensor in self._external_repository.get_external_sensors()
             if sensor.sensor_type == SensorType.AUTO_MATERIALIZE
             and asset_key in check.not_none(sensor.asset_selection).resolve(asset_graph)
@@ -1186,14 +1188,20 @@
             return None
 
     def resolve_metadata_entries(
         self, _graphene_info: ResolveInfo
     ) -> Sequence[GrapheneMetadataEntry]:
         return list(iterate_metadata_entries(self._external_asset_node.metadata))
 
+    def resolve_tags(self, _graphene_info: ResolveInfo) -> Sequence[GrapheneDefinitionTag]:
+        return [
+            GrapheneDefinitionTag(key, value)
+            for key, value in (self._external_asset_node.tags or {}).items()
+        ]
+
     def resolve_op(
         self, _graphene_info: ResolveInfo
     ) -> Optional[Union[GrapheneSolidDefinition, GrapheneCompositeSolidDefinition]]:
         if self.is_source_asset():
             return None
         external_pipeline = self.get_external_job()
         node_def_snap = self.get_node_definition_snap()
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/asset_selections.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/asset_selections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import graphene
 from dagster._core.definitions.asset_selection import AssetSelection
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
-from dagster._core.host_representation.external import ExternalRepository
+from dagster._core.remote_representation.external import ExternalRepository
 
 from ..implementation.fetch_assets import get_asset_nodes_by_asset_key
 from .asset_key import GrapheneAssetKey
 from .util import non_null_list
 
 
 class GrapheneAssetSelection(graphene.ObjectType):
@@ -17,24 +16,24 @@
         self._asset_selection = asset_selection
         self._external_repository = external_repository
 
     def resolve_assetSelectionString(self, _graphene_info):
         return str(self._asset_selection)
 
     def resolve_assetKeys(self, _graphene_info):
-        asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
+        asset_graph = self._external_repository.asset_graph
         return [
             GrapheneAssetKey(path=asset_key.path)
             for asset_key in self._asset_selection.resolve(asset_graph)
         ]
 
     def resolve_assets(self, graphene_info):
         from dagster_graphql.schema.pipelines.pipeline import GrapheneAsset
 
-        asset_graph = ExternalAssetGraph.from_external_repository(self._external_repository)
+        asset_graph = self._external_repository.asset_graph
         asset_nodes_by_asset_key = get_asset_nodes_by_asset_key(graphene_info)
 
         return [
             GrapheneAsset(key=asset_key, definition=asset_nodes_by_asset_key.get(asset_key))
             for asset_key in self._asset_selection.resolve(asset_graph)
         ]
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     PartitionedAssetBackfillStatus,
     UnpartitionedAssetBackfillStatus,
 )
 from dagster._core.execution.backfill import (
     BulkActionStatus,
     PartitionBackfill,
 )
-from dagster._core.host_representation.external import ExternalPartitionSet
+from dagster._core.remote_representation.external import ExternalPartitionSet
 from dagster._core.storage.dagster_run import RunPartitionData, RunRecord, RunsFilter
 from dagster._core.storage.tags import BACKFILL_ID_TAG, TagType, get_tag_type
 from dagster._core.workspace.permissions import Permissions
 
 from ..implementation.fetch_partition_sets import (
     partition_status_counts_from_run_partition_data,
     partition_statuses_from_run_partition_data,
@@ -297,16 +297,16 @@
         )
 
     def _get_partition_set(self, graphene_info: ResolveInfo) -> Optional[ExternalPartitionSet]:
         if self._backfill_job.partition_set_origin is None:
             return None
 
         origin = self._backfill_job.partition_set_origin
-        location_name = origin.external_repository_origin.code_location_origin.location_name
-        repository_name = origin.external_repository_origin.repository_name
+        location_name = origin.repository_origin.code_location_origin.location_name
+        repository_name = origin.repository_origin.repository_name
         if not graphene_info.context.has_code_location(location_name):
             return None
 
         location = graphene_info.context.get_code_location(location_name)
         if not location.has_repository(repository_name):
             return None
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/env_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Sequence
 
 import graphene
-from dagster._core.host_representation.external_data import (
+from dagster._core.remote_representation.external_data import (
     EnvVarConsumer,
 )
 
 from dagster_graphql.schema.errors import (
     GraphenePythonError,
 )
 from dagster_graphql.schema.util import non_null_list
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/errors.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/execution.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dagster._check as check
 import graphene
-from dagster._core.host_representation import ExternalExecutionPlan
+from dagster._core.remote_representation import ExternalExecutionPlan
 from dagster._core.snap import ExecutionStepInputSnap, ExecutionStepOutputSnap, ExecutionStepSnap
 
 from .metadata import GrapheneMetadataItemDefinition
 from .util import ResolveInfo, non_null_list
 
 
 class GrapheneExecutionStepOutput(graphene.ObjectType):
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/external.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 
 import graphene
 from dagster import (
     DagsterInstance,
     _check as check,
 )
 from dagster._core.definitions.asset_graph_differ import AssetGraphDiffer
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader
 from dagster._core.definitions.sensor_definition import (
     SensorType,
 )
-from dagster._core.host_representation import (
+from dagster._core.remote_representation import (
     CodeLocation,
     ExternalRepository,
     GrpcServerCodeLocation,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
-from dagster._core.host_representation.feature_flags import get_feature_flags_for_location
-from dagster._core.host_representation.grpc_server_state_subscriber import (
+from dagster._core.remote_representation.feature_flags import get_feature_flags_for_location
+from dagster._core.remote_representation.grpc_server_state_subscriber import (
     LocationStateChangeEvent,
     LocationStateChangeEventType,
     LocationStateSubscriber,
 )
 from dagster._core.workspace.context import (
     BaseWorkspaceRequestContext,
     WorkspaceProcessContext,
@@ -49,15 +48,15 @@
 from .resources import GrapheneResourceDetails
 from .schedules import GrapheneSchedule
 from .sensors import GrapheneSensor, GrapheneSensorType
 from .used_solid import GrapheneUsedSolid
 from .util import ResolveInfo, non_null_list
 
 if TYPE_CHECKING:
-    from dagster._core.host_representation.external_data import ExternalAssetNode
+    from dagster._core.remote_representation.external_data import ExternalAssetNode
 
 GrapheneLocationStateChangeEventType = graphene.Enum.from_enum(LocationStateChangeEventType)
 
 
 class GrapheneDagsterLibraryVersion(graphene.ObjectType):
     name = graphene.NonNull(graphene.String)
     version = graphene.NonNull(graphene.String)
@@ -271,15 +270,15 @@
         self._repository_location = check.inst_param(
             repository_location, "repository_location", CodeLocation
         )
         check.inst_param(instance, "instance", DagsterInstance)
         self._batch_loader = RepositoryScopedBatchLoader(instance, repository)
         self._stale_status_loader = StaleStatusLoader(
             instance=instance,
-            asset_graph=lambda: ExternalAssetGraph.from_external_repository(repository),
+            asset_graph=lambda: repository.asset_graph,
         )
         self._dynamic_partitions_loader = CachingDynamicPartitionsLoader(instance)
 
         self._asset_graph_differ = None
         # get_base_deployment_context is cached so there will only be one context per query
         base_deployment_context = workspace_context.get_base_deployment_context()
         if base_deployment_context is not None:
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,14 @@
         description = (
             """This type represents the fields necessary to identify a top-level resource."""
         )
         name = "ResourceSelector"
 
 
 class GrapheneExecutionMetadata(graphene.InputObjectType):
-    runId = graphene.String()
     tags = graphene.List(graphene.NonNull(GrapheneExecutionTag))
     rootRunId = graphene.String(
         description="""The ID of the run at the root of the run group. All partial /
         full re-executions should use the first run as the rootRunID so they are
         grouped together."""
     )
     parentRunId = graphene.String(
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/instance.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
     def resolve_pendingSteps(self, _graphene_info: ResolveInfo):
         return [GraphenePendingConcurrencyStep(step) for step in self._pending_steps]
 
 
 class GrapheneRunQueueConfig(graphene.ObjectType):
     maxConcurrentRuns = graphene.NonNull(graphene.Int)
     tagConcurrencyLimitsYaml = graphene.String()
+    isOpConcurrencyAware = graphene.Boolean()
 
     class Meta:
         name = "RunQueueConfig"
 
     def __init__(self, run_queue_config: "RunQueueConfig"):
         super().__init__()
         self._run_queue_config = run_queue_config
@@ -192,14 +193,17 @@
         return yaml.dump(
             self._run_queue_config.tag_concurrency_limits,
             default_flow_style=False,
             allow_unicode=True,
             sort_keys=True,
         )
 
+    def resolve_isOpConcurrencyAware(self, _graphene_info: ResolveInfo):
+        return self._run_queue_config.should_block_op_concurrency_limited_runs
+
 
 class GrapheneInstance(graphene.ObjectType):
     id = graphene.NonNull(graphene.String)
     info = graphene.Field(graphene.String)
     runLauncher = graphene.Field(GrapheneRunLauncher)
     runQueuingSupported = graphene.NonNull(graphene.Boolean)
     runQueueConfig = graphene.Field(GrapheneRunQueueConfig)
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/instigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,15 +584,15 @@
                 GrapheneInstigationStatus.RUNNING
                 if instigator_state.is_running
                 else GrapheneInstigationStatus.STOPPED
             ),
         )
 
     def resolve_repositoryOrigin(self, _graphene_info: ResolveInfo):
-        origin = self._instigator_state.origin.external_repository_origin
+        origin = self._instigator_state.origin.repository_origin
         return GrapheneRepositoryOrigin(origin)
 
     def resolve_repositoryName(self, _graphene_info: ResolveInfo):
         return self._instigator_state.repository_selector.repository_name
 
     def resolve_repositoryLocationName(self, _graphene_info: ResolveInfo):
         return self._instigator_state.repository_selector.location_name
@@ -631,15 +631,15 @@
             return GrapheneScheduleData(self._instigator_state.instigator_data)
 
         return None
 
     def resolve_runs(self, graphene_info: ResolveInfo, limit: Optional[int] = None):
         from .pipelines.pipeline import GrapheneRun
 
-        repository_label = self._instigator_state.origin.external_repository_origin.get_label()
+        repository_label = self._instigator_state.origin.repository_origin.get_label()
         if self._instigator_state.instigator_type == InstigatorType.SENSOR:
             filters = RunsFilter(
                 tags={
                     **DagsterRun.tags_for_sensor(self._instigator_state),
                     REPOSITORY_LABEL_TAG: repository_label,
                 }
             )
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import graphene
 
 from .asset_key import GrapheneAssetKey
-from .table import GrapheneTable, GrapheneTableSchema
+from .table import (
+    GrapheneTable,
+    GrapheneTableColumnLineageEntry,
+    GrapheneTableSchema,
+)
+from .util import non_null_list
 
 
 class GrapheneMetadataItemDefinition(graphene.ObjectType):
     key = graphene.NonNull(graphene.String)
     value = graphene.NonNull(graphene.String)
 
     class Meta:
@@ -48,14 +53,22 @@
     schema = graphene.NonNull(GrapheneTableSchema)
 
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "TableSchemaMetadataEntry"
 
 
+class GrapheneTableColumnLineageMetadataEntry(graphene.ObjectType):
+    lineage = non_null_list(GrapheneTableColumnLineageEntry)
+
+    class Meta:
+        interfaces = (GrapheneMetadataEntry,)
+        name = "TableColumnLineageMetadataEntry"
+
+
 class GrapheneJsonMetadataEntry(graphene.ObjectType):
     jsonString = graphene.NonNull(graphene.String)
 
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "JsonMetadataEntry"
 
@@ -151,17 +164,26 @@
 
 class GrapheneNullMetadataEntry(graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "NullMetadataEntry"
 
 
+class GrapheneTimestampMetadataEntry(graphene.ObjectType):
+    timestamp = graphene.NonNull(graphene.Float)
+
+    class Meta:
+        interfaces = (GrapheneMetadataEntry,)
+        name = "TimestampMetadataEntry"
+
+
 def types():
     return [
         GrapheneMetadataEntry,
+        GrapheneTableColumnLineageMetadataEntry,
         GrapheneTableSchemaMetadataEntry,
         GrapheneTableMetadataEntry,
         GrapheneFloatMetadataEntry,
         GrapheneIntMetadataEntry,
         GrapheneJsonMetadataEntry,
         GrapheneBoolMetadataEntry,
         GrapheneMarkdownMetadataEntry,
@@ -171,8 +193,9 @@
         GraphenePythonArtifactMetadataEntry,
         GrapheneTextMetadataEntry,
         GrapheneUrlMetadataEntry,
         GraphenePipelineRunMetadataEntry,
         GrapheneAssetMetadataEntry,
         GrapheneJobMetadataEntry,
         GrapheneNullMetadataEntry,
+        GrapheneTimestampMetadataEntry,
     ]
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/partition_mappings.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/partition_mappings.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/partition_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, cast
 
 import dagster._check as check
 import graphene
 from dagster import MultiPartitionsDefinition
-from dagster._core.host_representation import ExternalPartitionSet, RepositoryHandle
-from dagster._core.host_representation.external_data import (
+from dagster._core.remote_representation import ExternalPartitionSet, RepositoryHandle
+from dagster._core.remote_representation.external_data import (
     ExternalDynamicPartitionsDefinitionData,
     ExternalMultiPartitionsDefinitionData,
     ExternalPartitionsDefinitionData,
     ExternalStaticPartitionsDefinitionData,
     ExternalTimeWindowPartitionsDefinitionData,
 )
 from dagster._core.storage.dagster_run import RunsFilter
@@ -338,29 +338,29 @@
     def resolve_partitionStatusesOrError(self, graphene_info: ResolveInfo):
         return get_partition_set_partition_statuses(
             graphene_info,
             self._external_partition_set,
         )
 
     def resolve_repositoryOrigin(self, _):
-        origin = self._external_partition_set.get_external_origin().external_repository_origin
+        origin = self._external_partition_set.get_external_origin().repository_origin
         return GrapheneRepositoryOrigin(origin)
 
     def resolve_backfills(
         self, graphene_info: ResolveInfo, cursor: Optional[str] = None, limit: Optional[int] = None
     ):
         matching = [
             backfill
             for backfill in graphene_info.context.instance.get_backfills(
                 cursor=cursor,
             )
             if backfill.partition_set_origin
             and backfill.partition_set_origin.partition_set_name
             == self._external_partition_set.name
-            and backfill.partition_set_origin.external_repository_origin.repository_name
+            and backfill.partition_set_origin.repository_origin.repository_name
             == self._external_repository_handle.repository_name
         ]
         return [GraphenePartitionBackfill(backfill) for backfill in matching[:limit]]
 
 
 class GraphenePartitionSetOrError(graphene.Union):
     class Meta:
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     FieldNotDefinedErrorData,
     FieldsNotDefinedErrorData,
     MissingFieldErrorData,
     MissingFieldsErrorData,
     RuntimeMismatchErrorData,
     SelectorTypeErrorData,
 )
-from dagster._core.host_representation.represented import RepresentedJob
+from dagster._core.remote_representation.represented import RepresentedJob
 from dagster._utils.error import SerializableErrorInfo
 from graphene.types.generic import GenericScalar
 
 from ..config_types import GrapheneConfigTypeField
 from ..util import non_null_list
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Optional, Sequence
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.time_window_partitions import PartitionRangeStatus
 from dagster._core.events import DagsterEventType
-from dagster._core.host_representation.external import ExternalExecutionPlan, ExternalJob
-from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME, ExternalPresetData
-from dagster._core.host_representation.represented import RepresentedJob
+from dagster._core.remote_representation.external import ExternalExecutionPlan, ExternalJob
+from dagster._core.remote_representation.external_data import DEFAULT_MODE_NAME, ExternalPresetData
+from dagster._core.remote_representation.represented import RepresentedJob
 from dagster._core.storage.dagster_run import (
     DagsterRunStatsSnapshot,
     DagsterRunStatus,
     RunRecord,
     RunsFilter,
 )
 from dagster._core.storage.tags import REPOSITORY_LABEL_TAG, TagType, get_tag_type
@@ -375,14 +375,16 @@
     startTime = graphene.Float()
     endTime = graphene.Float()
     updateTime = graphene.Float()
     hasReExecutePermission = graphene.NonNull(graphene.Boolean)
     hasTerminatePermission = graphene.NonNull(graphene.Boolean)
     hasDeletePermission = graphene.NonNull(graphene.Boolean)
     hasConcurrencyKeySlots = graphene.NonNull(graphene.Boolean)
+    rootConcurrencyKeys = graphene.List(graphene.NonNull(graphene.String))
+    hasUnconstrainedRootNodes = graphene.NonNull(graphene.Boolean)
 
     class Meta:
         interfaces = (GraphenePipelineRun,)
         name = "Run"
 
     def __init__(self, record: RunRecord):
         check.inst_param(record, "record", RunRecord)
@@ -419,17 +421,15 @@
         return self._get_permission_value(Permissions.DELETE_PIPELINE_RUN, graphene_info)
 
     def resolve_id(self, _graphene_info: ResolveInfo):
         return self.dagster_run.run_id
 
     def resolve_repositoryOrigin(self, _graphene_info: ResolveInfo):
         return (
-            GrapheneRepositoryOrigin(
-                self.dagster_run.external_job_origin.external_repository_origin
-            )
+            GrapheneRepositoryOrigin(self.dagster_run.external_job_origin.repository_origin)
             if self.dagster_run.external_job_origin
             else None
         )
 
     def resolve_pipeline(self, graphene_info: ResolveInfo):
         return get_job_reference_or_raise(graphene_info, self.dagster_run)
 
@@ -597,14 +597,32 @@
         instance = graphene_info.context.instance
         if not instance.event_log_storage.supports_global_concurrency_limits:
             return False
 
         active_run_ids = instance.event_log_storage.get_concurrency_run_ids()
         return self.runId in active_run_ids
 
+    def resolve_hasUnconstrainedRootNodes(self, graphene_info: ResolveInfo):
+        if not self.dagster_run.run_op_concurrency:
+            return True
+
+        if self.dagster_run.run_op_concurrency.has_unconstrained_root_nodes:
+            return True
+
+        return False
+
+    def resolve_rootConcurrencyKeys(self, graphene_info: ResolveInfo):
+        if not self.dagster_run.run_op_concurrency:
+            return None
+
+        root_concurrency_keys = []
+        for concurrency_key, count in self.dagster_run.run_op_concurrency.root_key_counts.items():
+            root_concurrency_keys.extend([concurrency_key] * count)
+        return root_concurrency_keys
+
 
 class GrapheneIPipelineSnapshotMixin:
     # Mixin this class to implement IPipelineSnapshot
     #
     # Graphene has some strange properties that make it so that you cannot
     # implement ABCs nor use properties in an overridable way. So the way
     # the mixin works is that the target classes have to have a method
@@ -746,15 +764,15 @@
     ) -> Sequence[GrapheneRun]:
         pipeline = self.get_represented_job()
         if isinstance(pipeline, ExternalJob):
             runs_filter = RunsFilter(
                 job_name=pipeline.name,
                 tags={
                     REPOSITORY_LABEL_TAG: (
-                        pipeline.get_external_origin().external_repository_origin.get_label()
+                        pipeline.get_external_origin().repository_origin.get_label()
                     )
                 },
             )
         else:
             runs_filter = RunsFilter(job_name=pipeline.name)
         return get_runs(graphene_info, runs_filter, cursor, limit)
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dagster._check as check
 import graphene
-from dagster._core.host_representation import RepresentedJob
+from dagster._core.remote_representation import RepresentedJob
 
 from ..errors import (
     GraphenePipelineNotFoundError,
     GraphenePipelineSnapshotNotFoundError,
     GraphenePythonError,
 )
 from ..solids import GrapheneSolidContainer
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/repository_origin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Sequence
 
 import dagster._check as check
 import graphene
-from dagster._core.host_representation import ExternalRepositoryOrigin
+from dagster._core.remote_representation import RemoteRepositoryOrigin
 
 from .util import ResolveInfo, non_null_list
 
 
 class GrapheneRepositoryMetadata(graphene.ObjectType):
     key = graphene.NonNull(graphene.String)
     value = graphene.NonNull(graphene.String)
@@ -20,17 +20,17 @@
     repository_location_name = graphene.NonNull(graphene.String)
     repository_name = graphene.NonNull(graphene.String)
     repository_location_metadata = non_null_list(GrapheneRepositoryMetadata)
 
     class Meta:
         name = "RepositoryOrigin"
 
-    def __init__(self, origin: ExternalRepositoryOrigin):
+    def __init__(self, origin: RemoteRepositoryOrigin):
         super().__init__()
-        self._origin = check.inst_param(origin, "origin", ExternalRepositoryOrigin)
+        self._origin = check.inst_param(origin, "origin", RemoteRepositoryOrigin)
 
     def resolve_id(self, _graphene_info: ResolveInfo) -> str:
         return self._origin.get_id()
 
     def resolve_repository_location_name(self, _graphene_info: ResolveInfo) -> str:
         return self._origin.code_location_origin.location_name
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/resources.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING, List
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.selector import ResourceSelector
-from dagster._core.host_representation.external import ExternalRepository, ExternalResource
-from dagster._core.host_representation.external_data import (
+from dagster._core.remote_representation.external import ExternalRepository, ExternalResource
+from dagster._core.remote_representation.external_data import (
     ExternalResourceConfigEnvVar,
     ExternalResourceValue,
     NestedResourceType,
     ResourceJobUsageEntry,
 )
 
 from dagster_graphql.schema.asset_key import GrapheneAssetKey
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional, Sequence, Union
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.nux import get_has_seen_nux, set_nux_seen
 from dagster._core.workspace.permissions import Permissions
 from dagster._daemon.asset_daemon import set_auto_materialize_paused
 
 from dagster_graphql.implementation.execution.backfill import (
     cancel_partition_backfill,
@@ -723,15 +722,15 @@
         event_type = eventParams["eventType"].to_dagster_event_type()
         asset_key = AssetKey.from_graphql_input(eventParams["assetKey"])
         partition_keys = eventParams.get("partitionKeys", None)
         description = eventParams.get("description", None)
 
         reporting_user_tags = {**graphene_info.context.get_reporting_user_tags()}
 
-        asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
+        asset_graph = graphene_info.context.asset_graph
 
         assert_permission_for_asset_graph(
             graphene_info, asset_graph, [asset_key], Permissions.REPORT_RUNLESS_ASSET_EVENTS
         )
 
         return report_runless_asset_events(
             graphene_info,
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Mapping, Optional, Sequence, cast
 
 import dagster._check as check
 import graphene
 from dagster import AssetCheckKey
 from dagster._core.definitions.asset_graph_differ import AssetGraphDiffer
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader
+from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
 from dagster._core.definitions.selector import (
     InstigatorSelector,
     RepositorySelector,
     ResourceSelector,
     ScheduleSelector,
     SensorSelector,
 )
@@ -799,15 +799,15 @@
     def resolve_runTagKeysOrError(self, graphene_info: ResolveInfo):
         return get_run_tag_keys(graphene_info)
 
     @capture_error
     def resolve_runTagsOrError(
         self,
         graphene_info: ResolveInfo,
-        tagKeys: Optional[List[str]] = None,
+        tagKeys: List[str],
         valuePrefix: Optional[str] = None,
         limit: Optional[int] = None,
     ):
         return get_run_tags(graphene_info, tagKeys, valuePrefix, limit)
 
     @capture_error
     def resolve_runGroupOrError(self, graphene_info: ResolveInfo, runId):
@@ -946,19 +946,19 @@
         asset_checks_loader = AssetChecksLoader(
             context=graphene_info.context,
             asset_keys=[node.assetKey for node in results],
         )
 
         depended_by_loader = CrossRepoAssetDependedByLoader(context=graphene_info.context)
 
-        def load_asset_graph() -> ExternalAssetGraph:
+        def load_asset_graph() -> RemoteAssetGraph:
             if repo is not None:
-                return ExternalAssetGraph.from_external_repository(repo)
+                return repo.asset_graph
             else:
-                return ExternalAssetGraph.from_workspace(graphene_info.context)
+                return graphene_info.context.asset_graph
 
         stale_status_loader = StaleStatusLoader(
             instance=graphene_info.context.instance,
             asset_graph=load_asset_graph,
         )
 
         base_deployment_context = graphene_info.context.get_base_deployment_context()
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/run_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Any, Optional
 
 import dagster._check as check
 import graphene
-from dagster._core.host_representation import RepresentedJob
-from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
+from dagster._core.remote_representation import RepresentedJob
+from dagster._core.remote_representation.external_data import DEFAULT_MODE_NAME
 from dagster._core.snap.snap_to_yaml import default_values_yaml_from_type_snap
 
 from ..implementation.run_config_schema import resolve_is_run_config_valid
 from ..implementation.utils import capture_error
 from .config_types import GrapheneConfigType, to_config_type
 from .errors import (
     GrapheneInvalidSubsetError,
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/runs.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/schedules/schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 
 import dagster._check as check
 import graphene
 from dagster import DefaultScheduleStatus
-from dagster._core.host_representation import ExternalSchedule
+from dagster._core.remote_representation import ExternalSchedule
 from dagster._core.scheduler.instigation import InstigatorState, InstigatorStatus
 from dagster._seven import get_current_datetime_in_utc, get_timestamp_from_utc_datetime
 
 from dagster_graphql.implementation.loader import RepositoryScopedBatchLoader
 
 from ..errors import (
     GraphenePythonError,
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import dagster._check as check
 import graphene
 from dagster import DefaultSensorStatus
 from dagster._core.definitions.selector import SensorSelector
 from dagster._core.definitions.sensor_definition import (
     SensorType,
 )
-from dagster._core.host_representation import ExternalSensor, ExternalTargetData
-from dagster._core.host_representation.external import ExternalRepository
+from dagster._core.remote_representation import ExternalSensor, ExternalTargetData
+from dagster._core.remote_representation.external import ExternalRepository
 from dagster._core.scheduler.instigation import InstigatorState, InstigatorStatus
 from dagster._core.workspace.permissions import Permissions
 
 from dagster_graphql.implementation.loader import RepositoryScopedBatchLoader
 from dagster_graphql.implementation.utils import (
     assert_permission_for_location,
     capture_error,
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/solids.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/solids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import lru_cache
 from typing import TYPE_CHECKING, List, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions import NodeHandle
 from dagster._core.definitions.asset_graph_differ import AssetGraphDiffer
-from dagster._core.host_representation import RepresentedJob
-from dagster._core.host_representation.external import ExternalJob
-from dagster._core.host_representation.historical import HistoricalJob
+from dagster._core.remote_representation import RepresentedJob
+from dagster._core.remote_representation.external import ExternalJob
+from dagster._core.remote_representation.historical import HistoricalJob
 from dagster._core.snap import DependencyStructureIndex, GraphDefSnap, OpDefSnap
 from dagster._core.snap.node import InputMappingSnap, OutputMappingSnap
 from dagster._core.storage.dagster_run import RunsFilter
 
 from dagster_graphql.implementation.asset_checks_loader import AssetChecksLoader
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.schema.logs.events import GrapheneRunStepStats
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/tags.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,31 @@
     class Meta:
         name = "PipelineTag"
 
     def __init__(self, key, value):
         super().__init__(key=key, value=value)
 
 
-class GrapheneAssetTag(graphene.ObjectType):
+class GrapheneEventTag(graphene.ObjectType):
     key = graphene.NonNull(graphene.String)
     value = graphene.NonNull(graphene.String)
 
     class Meta:
-        name = "AssetTag"
+        name = "EventTag"
 
     def __init__(self, key, value):
         super().__init__(key=key, value=value)
 
 
-class GrapheneEventTag(graphene.ObjectType):
+class GrapheneDefinitionTag(graphene.ObjectType):
     key = graphene.NonNull(graphene.String)
     value = graphene.NonNull(graphene.String)
 
     class Meta:
-        name = "EventTag"
+        name = "DefinitionTag"
 
     def __init__(self, key, value):
         super().__init__(key=key, value=value)
 
 
 class GraphenePipelineTagAndValues(graphene.ObjectType):
     class Meta:
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/test.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/test.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/schema/util.py` & `dagster-graphql-1.7.0/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/dagster_graphql/test/utils.py` & `dagster-graphql-1.7.0/dagster_graphql/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Dict, Iterator, Mapping, Optional, Sequence
 
 import dagster._check as check
 import graphene
-from dagster._core.host_representation.external import ExternalRepository
 from dagster._core.instance import DagsterInstance
+from dagster._core.remote_representation.external import ExternalRepository
 from dagster._core.test_utils import wait_for_runs_to_finish
 from dagster._core.workspace.context import WorkspaceProcessContext, WorkspaceRequestContext
 from dagster._core.workspace.load_target import PythonFileTarget
 from typing_extensions import Protocol, TypeAlias, TypedDict
 
 from dagster_graphql import __file__ as dagster_graphql_init_py
 from dagster_graphql.schema import create_schema
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.7.0/dagster_graphql.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.6.9
+Version: 1.7.0
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.6.9/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.7.0/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.6.9/setup.py` & `dagster-graphql-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
+        "dagster==1.7.0",
         "graphene>=3,<4",
         "gql[requests]>=3,<4",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

