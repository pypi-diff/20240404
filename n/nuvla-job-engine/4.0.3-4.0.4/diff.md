# Comparing `tmp/nuvla_job_engine-4.0.3.tar.gz` & `tmp/nuvla_job_engine-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla_job_engine-4.0.3.tar", max compression
+gzip compressed data, was "nuvla_job_engine-4.0.4.tar", max compression
```

## Comparing `nuvla_job_engine-4.0.3.tar` & `nuvla_job_engine-4.0.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    11357 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/LICENSE
--rw-r--r--   0        0        0     4575 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/README.md
--rw-r--r--   0        0        0        0 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/__init__.py
--rw-r--r--   0        0        0       24 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/__init__.py
--rw-r--r--   0        0        0     1340 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/connector.py
--rw-r--r--   0        0        0    11757 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_compose.py
--rw-r--r--   0        0        0    33689 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_machine.py
--rw-r--r--   0        0        0    15017 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_service.py
--rw-r--r--   0        0        0     8401 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_stack.py
--rwxr-xr-x   0        0        0     1412 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/install-rancher.sh
--rw-r--r--   0        0        0     1713 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/k8s-install.sh
--rw-r--r--   0        0        0     1432 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/portainer-k8s.yaml
--rw-r--r--   0        0        0      774 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/portainer-swarm.yaml
--rw-r--r--   0        0        0       68 2024-03-21 13:22:09.476678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/ssh-add-keys.sh
--rw-r--r--   0        0        0    47994 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/kubernetes.py
--rw-r--r--   0        0        0      322 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/machine/__init__.py
--rw-r--r--   0        0        0      641 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/machine/helper.py
--rw-r--r--   0        0        0    11681 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/machine/machine.py
--rw-r--r--   0        0        0    28807 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/nuvlabox.py
--rw-r--r--   0        0        0     5380 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/registry.py
--rw-r--r--   0        0        0     3670 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/connector/utils.py
--rw-r--r--   0        0        0       95 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/__init__.py
--rw-r--r--   0        0        0     1989 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/__init__.py
--rwxr-xr-x   0        0        0     2999 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/application_docker_compose_validate.py
--rwxr-xr-x   0        0        0      320 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
--rwxr-xr-x   0        0        0     1686 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
--rwxr-xr-x   0        0        0      322 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
--rwxr-xr-x   0        0        0      711 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
--rwxr-xr-x   0        0        0      692 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_stop_deployment.py
--rwxr-xr-x   0        0        0      908 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_update_deployment.py
--rwxr-xr-x   0        0        0     1298 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/cancel_children_jobs.py
--rwxr-xr-x   0        0        0     4269 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_provision.py
--rwxr-xr-x   0        0        0     1719 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_start.py
--rwxr-xr-x   0        0        0     1644 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_stop.py
--rwxr-xr-x   0        0        0     2601 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_terminate.py
--rwxr-xr-x   0        0        0     2982 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/component_image_state.py
--rwxr-xr-x   0        0        0     8667 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/credential_check.py
--rw-r--r--   0        0        0     3129 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/dct_check.py
--rw-r--r--   0        0        0     2979 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_log_fetch.py
--rwxr-xr-x   0        0        0      345 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_set_delete.py
--rwxr-xr-x   0        0        0      421 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_set_force_delete.py
--rwxr-xr-x   0        0        0     5402 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_start.py
--rwxr-xr-x   0        0        0     7298 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_state.py
--rw-r--r--   0        0        0     3207 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_stop.py
--rw-r--r--   0        0        0     4010 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_update.py
--rwxr-xr-x   0        0        0      366 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/dummy_test_action.py
--rw-r--r--   0        0        0      729 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/handle_trial_end.py
--rwxr-xr-x   0        0        0     1051 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/jobs_cleanup.py
--rw-r--r--   0        0        0     3553 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/monitor_bulk_job.py
--rw-r--r--   0        0        0      697 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/notify_coupon_end.py
--rwxr-xr-x   0        0        0     2901 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
--rwxr-xr-x   0        0        0      692 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_check_api.py
--rwxr-xr-x   0        0        0      867 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_cluster.py
--rwxr-xr-x   0        0        0     2100 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     4570 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_decommission.py
--rwxr-xr-x   0        0        0     1856 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
--rwxr-xr-x   0        0        0     1273 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
--rw-r--r--   0        0        0     1453 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
--rwxr-xr-x   0        0        0     1232 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_reboot.py
--rwxr-xr-x   0        0        0     4425 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1280 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
--rwxr-xr-x   0        0        0     2513 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
--rwxr-xr-x   0        0        0     2429 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
--rwxr-xr-x   0        0        0     1637 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_update.py
--rw-r--r--   0        0        0      849 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/register_usage_record.py
--rwxr-xr-x   0        0        0     3059 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/service_image_state.py
--rw-r--r--   0        0        0        0 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/__init__.py
--rw-r--r--   0        0        0     1574 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/bulk_action.py
--rwxr-xr-x   0        0        0      854 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/bulk_deployment.py
--rwxr-xr-x   0        0        0     8840 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
--rwxr-xr-x   0        0        0     1289 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
--rw-r--r--   0        0        0    11037 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/deployment_utils.py
--rw-r--r--   0        0        0     4009 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
--rwxr-xr-x   0        0        0     9633 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/vulnerabilities_database.py
--rw-r--r--   0        0        0     7390 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/base.py
--rw-r--r--   0        0        0     2107 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distribution.py
--rw-r--r--   0        0        0     1989 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/__init__.py
--rwxr-xr-x   0        0        0     1500 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/component_image_state.py
--rwxr-xr-x   0        0        0     2296 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/deployment_state.py
--rwxr-xr-x   0        0        0     1214 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/deployment_state_new.py
--rwxr-xr-x   0        0        0     2479 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/deployment_state_old.py
--rwxr-xr-x   0        0        0      408 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/dummy_action.py
--rwxr-xr-x   0        0        0     2907 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/handle_trial_end.py
--rwxr-xr-x   0        0        0      440 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/jobs_cleanup.py
--rwxr-xr-x   0        0        0     1803 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
--rwxr-xr-x   0        0        0     1754 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/notify_coupon_end.py
--rwxr-xr-x   0        0        0      487 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     1435 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/nuvlabox_offline.py
--rwxr-xr-x   0        0        0      475 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1210 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
--rwxr-xr-x   0        0        0     2464 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/register_usage_record.py
--rwxr-xr-x   0        0        0     3119 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
--rwxr-xr-x   0        0        0     1556 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/service_image_state.py
--rwxr-xr-x   0        0        0      503 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/vulnerabilities_database.py
--rw-r--r--   0        0        0        0 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributor/__init__.py
--rw-r--r--   0        0        0     1400 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributor/distributor.py
--rw-r--r--   0        0        0        0 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/executor/__init__.py
--rw-r--r--   0        0        0     4365 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/executor/executor.py
--rw-r--r--   0        0        0    10814 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/job.py
--rw-r--r--   0        0        0     1975 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/util.py
--rw-r--r--   0        0        0      186 2024-03-21 13:22:09.480678 nuvla_job_engine-4.0.3/nuvla/job_engine/job/version.py
--rwxr-xr-x   0        0        0     2708 2024-03-21 13:22:09.484678 nuvla_job_engine-4.0.3/nuvla/scripts/job_deployment_state_push.py
--rwxr-xr-x   0        0        0      208 2024-03-21 13:22:09.484678 nuvla_job_engine-4.0.3/nuvla/scripts/job_distributor.py
--rwxr-xr-x   0        0        0      197 2024-03-21 13:22:09.484678 nuvla_job_engine-4.0.3/nuvla/scripts/job_executor.py
--rwxr-xr-x   0        0        0     1967 2024-03-21 13:22:09.484678 nuvla_job_engine-4.0.3/nuvla/scripts/job_restore.py
--rwxr-xr-x   0        0        0      186 2024-03-21 13:22:09.484678 nuvla_job_engine-4.0.3/nuvla/scripts/pause.py
--rw-r--r--   0        0        0     1221 2024-03-21 13:22:09.484678 nuvla_job_engine-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 16:25:48.987583 nuvla_job_engine-4.0.4/LICENSE
+-rw-r--r--   0        0        0     4575 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/__init__.py
+-rw-r--r--   0        0        0     1340 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/connector.py
+-rw-r--r--   0        0        0    11757 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_compose.py
+-rw-r--r--   0        0        0    33689 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_machine.py
+-rw-r--r--   0        0        0    15017 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_service.py
+-rw-r--r--   0        0        0     8401 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_stack.py
+-rwxr-xr-x   0        0        0     1412 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/install-rancher.sh
+-rw-r--r--   0        0        0     1713 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/k8s-install.sh
+-rw-r--r--   0        0        0     1432 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-k8s.yaml
+-rw-r--r--   0        0        0      774 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-swarm.yaml
+-rw-r--r--   0        0        0       68 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/ssh-add-keys.sh
+-rw-r--r--   0        0        0    47994 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/kubernetes.py
+-rw-r--r--   0        0        0      322 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/__init__.py
+-rw-r--r--   0        0        0      641 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/helper.py
+-rw-r--r--   0        0        0    11681 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/machine.py
+-rw-r--r--   0        0        0    28734 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/nuvlabox.py
+-rw-r--r--   0        0        0     5380 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/registry.py
+-rw-r--r--   0        0        0     3670 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/utils.py
+-rw-r--r--   0        0        0       95 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/__init__.py
+-rw-r--r--   0        0        0     1989 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/__init__.py
+-rwxr-xr-x   0        0        0     2999 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/application_docker_compose_validate.py
+-rwxr-xr-x   0        0        0      320 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
+-rwxr-xr-x   0        0        0     1686 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
+-rwxr-xr-x   0        0        0      322 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
+-rwxr-xr-x   0        0        0      711 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
+-rwxr-xr-x   0        0        0      692 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_stop_deployment.py
+-rwxr-xr-x   0        0        0      908 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_update_deployment.py
+-rwxr-xr-x   0        0        0     1298 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/cancel_children_jobs.py
+-rwxr-xr-x   0        0        0     4269 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_provision.py
+-rwxr-xr-x   0        0        0     1719 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_start.py
+-rwxr-xr-x   0        0        0     1644 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_stop.py
+-rwxr-xr-x   0        0        0     2601 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_terminate.py
+-rwxr-xr-x   0        0        0     2982 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/component_image_state.py
+-rwxr-xr-x   0        0        0     8667 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/credential_check.py
+-rw-r--r--   0        0        0     3129 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/dct_check.py
+-rw-r--r--   0        0        0     2979 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_log_fetch.py
+-rwxr-xr-x   0        0        0      345 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_set_delete.py
+-rwxr-xr-x   0        0        0      421 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_set_force_delete.py
+-rwxr-xr-x   0        0        0     5402 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_start.py
+-rwxr-xr-x   0        0        0     7298 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_state.py
+-rw-r--r--   0        0        0     3207 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_stop.py
+-rw-r--r--   0        0        0     4010 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_update.py
+-rwxr-xr-x   0        0        0      366 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/dummy_test_action.py
+-rw-r--r--   0        0        0      729 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/handle_trial_end.py
+-rwxr-xr-x   0        0        0     1051 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/jobs_cleanup.py
+-rw-r--r--   0        0        0     3553 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/monitor_bulk_job.py
+-rw-r--r--   0        0        0      697 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0     2901 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
+-rwxr-xr-x   0        0        0      692 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_check_api.py
+-rwxr-xr-x   0        0        0      867 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster.py
+-rwxr-xr-x   0        0        0     2100 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     4570 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_decommission.py
+-rwxr-xr-x   0        0        0     1856 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
+-rwxr-xr-x   0        0        0     1273 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
+-rw-r--r--   0        0        0     1453 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
+-rwxr-xr-x   0        0        0     1232 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_reboot.py
+-rwxr-xr-x   0        0        0     4425 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1280 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
+-rwxr-xr-x   0        0        0     2513 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
+-rwxr-xr-x   0        0        0     2429 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
+-rwxr-xr-x   0        0        0     1637 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_update.py
+-rw-r--r--   0        0        0      849 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3059 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/service_image_state.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_action.py
+-rwxr-xr-x   0        0        0      854 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment.py
+-rwxr-xr-x   0        0        0     8840 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
+-rwxr-xr-x   0        0        0     1289 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
+-rw-r--r--   0        0        0    11037 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_utils.py
+-rw-r--r--   0        0        0     4009 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
+-rwxr-xr-x   0        0        0     9633 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/vulnerabilities_database.py
+-rw-r--r--   0        0        0     7390 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/base.py
+-rw-r--r--   0        0        0     2107 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distribution.py
+-rw-r--r--   0        0        0     1989 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/__init__.py
+-rwxr-xr-x   0        0        0     1500 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/component_image_state.py
+-rwxr-xr-x   0        0        0     2296 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state.py
+-rwxr-xr-x   0        0        0     1214 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_new.py
+-rwxr-xr-x   0        0        0     2479 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_old.py
+-rwxr-xr-x   0        0        0      408 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/dummy_action.py
+-rwxr-xr-x   0        0        0     2907 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/handle_trial_end.py
+-rwxr-xr-x   0        0        0      440 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/jobs_cleanup.py
+-rwxr-xr-x   0        0        0     1803 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
+-rwxr-xr-x   0        0        0     1754 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0      487 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     1435 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_offline.py
+-rwxr-xr-x   0        0        0      475 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1210 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
+-rwxr-xr-x   0        0        0     2464 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3119 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
+-rwxr-xr-x   0        0        0     1556 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/service_image_state.py
+-rwxr-xr-x   0        0        0      503 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/vulnerabilities_database.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributor/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributor/distributor.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/executor/__init__.py
+-rw-r--r--   0        0        0     4365 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/executor/executor.py
+-rw-r--r--   0        0        0    10814 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/job.py
+-rw-r--r--   0        0        0     1975 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/util.py
+-rw-r--r--   0        0        0      186 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/version.py
+-rwxr-xr-x   0        0        0     2708 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_deployment_state_push.py
+-rwxr-xr-x   0        0        0      208 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_distributor.py
+-rwxr-xr-x   0        0        0      197 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_executor.py
+-rwxr-xr-x   0        0        0     1967 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_restore.py
+-rwxr-xr-x   0        0        0      186 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/pause.py
+-rw-r--r--   0        0        0     1221 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.4/PKG-INFO
```

### Comparing `nuvla_job_engine-4.0.3/LICENSE` & `nuvla_job_engine-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/README.md` & `nuvla_job_engine-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/connector.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/connector.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_compose.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_compose.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_machine.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_service.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_service.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/docker_stack.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_stack.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/install-rancher.sh` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/install-rancher.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/k8s-install.sh` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/k8s-install.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/portainer-k8s.yaml` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-k8s.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/extra/portainer-swarm.yaml` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-swarm.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/kubernetes.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/kubernetes.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/machine/helper.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/helper.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/machine/machine.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/nuvlabox.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/nuvlabox.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,17 +144,15 @@
         self.ssl_file = create_tmp_file(secret)
         self.cert_file = create_tmp_file(credential['cert'])
         self.key_file = create_tmp_file(credential['key'])
         self.nuvlabox_api.cert = self.ssl_file.name
         self.docker_api_endpoint = is_endpoint
         tls_config = docker.tls.TLSConfig(
             client_cert=(self.cert_file.name, self.key_file.name),
-            verify=False,
-            assert_hostname=False,
-            assert_fingerprint=False)
+            verify=False)
         self.docker_client = docker.DockerClient(
             base_url=remove_protocol_from_url(is_endpoint),
             tls=tls_config)
 
         return True
 
     def get_installer_image_names(self, nuvlaedge_version):
```

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/registry.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/registry.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/connector/utils.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/utils.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/__init__.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/application_docker_compose_validate.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/application_docker_compose_validate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_stop_deployment.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_stop_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/bulk_update_deployment.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_update_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/cancel_children_jobs.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/cancel_children_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_provision.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_provision.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_start.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_stop.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/coe_terminate.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_terminate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/component_image_state.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/credential_check.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/credential_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/dct_check.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/dct_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_log_fetch.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_start.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_state.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_stop.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/deployment_update.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/handle_trial_end.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/jobs_cleanup.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/jobs_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/monitor_bulk_job.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/monitor_bulk_job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/notify_coupon_end.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_check_api.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_check_api.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_cluster.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_decommission.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_decommission.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_reboot.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_reboot.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_releases.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_releases.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/nuvlabox_update.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/register_usage_record.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/service_image_state.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/bulk_action.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_action.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/bulk_deployment.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/deployment_set_remove.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_set_remove.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/deployment_utils.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/utils/resource_log_fetch.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/resource_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/actions/vulnerabilities_database.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/vulnerabilities_database.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/base.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/base.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distribution.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distribution.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/__init__.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/component_image_state.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/deployment_state.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/deployment_state_new.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_new.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/deployment_state_old.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_old.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/handle_trial_end.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/notify_coupon_end.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/nuvlabox_offline.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_offline.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/register_usage_record.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributions/service_image_state.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/distributor/distributor.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributor/distributor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/executor/executor.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/executor/executor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/job.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/job_engine/job/util.py` & `nuvla_job_engine-4.0.4/nuvla/job_engine/job/util.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/scripts/job_deployment_state_push.py` & `nuvla_job_engine-4.0.4/nuvla/scripts/job_deployment_state_push.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/nuvla/scripts/job_restore.py` & `nuvla_job_engine-4.0.4/nuvla/scripts/job_restore.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.3/pyproject.toml` & `nuvla_job_engine-4.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuvla-job-engine"
-version = "4.0.3"
+version = "4.0.4"
 description = "Nuvla Job Engine."
 license = "Apache-2.0"
 authors = ["SixSq SA <support@sixsq.com>"]
 maintainers = ["Ignacio Penas <nacho@sixsq.com>"]
 readme = "README.md"
 repository = "https://github.com/nuvla/job-engine"
 classifiers = [
```

### Comparing `nuvla_job_engine-4.0.3/PKG-INFO` & `nuvla_job_engine-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvla-job-engine
-Version: 4.0.3
+Version: 4.0.4
 Summary: Nuvla Job Engine.
 Home-page: https://github.com/nuvla/job-engine
 License: Apache-2.0
 Author: SixSq SA
 Author-email: support@sixsq.com
 Maintainer: Ignacio Penas
 Maintainer-email: nacho@sixsq.com
```

