# Comparing `tmp/sbcli-release-1.0.4.zip` & `tmp/sbcli-release-1.0.5.zip`

## zipinfo {}

```diff
@@ -1,130 +1,146 @@
-Zip file size: 152541 bytes, number of entries: 128
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_cli/
--rw-r--r--  2.0 unx      730 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/README.md
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/setup.cfg
--rw-r--r--  2.0 unx       84 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/pyproject.toml
--rw-r--r--  2.0 unx     1133 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/PKG-INFO
--rw-r--r--  2.0 unx     2159 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/setup.py
--rw-r--r--  2.0 unx      184 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/env_var
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/templates/
--rw-r--r--  2.0 unx     1205 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/app.py
--rw-r--r--  2.0 unx      660 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx      646 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     5078 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      668 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1624 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1377 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx     5897 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx    12058 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     2895 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5361 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     8560 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     7699 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx      975 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx    11242 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      417 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      322 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      463 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      507 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/
--rw-r--r--  2.0 unx     1361 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/constants.py
--rw-r--r--  2.0 unx    19841 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx      938 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx     3181 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx     3414 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     7557 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     6262 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx    70490 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx    20292 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     8048 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     1550 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx      917 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     3219 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2011 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     2531 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     3707 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2328 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      632 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx    39059 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     6240 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx    10807 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    23858 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     3094 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    10136 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1308 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      280 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx       54 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     6628 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx     5304 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     1493 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      648 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     2270 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2257 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     7047 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx      837 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4664 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     5992 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      173 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     1918 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     3049 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5391 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2849 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     1492 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     4322 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     5290 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     2047 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx       49 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/requires.txt
--rw-r--r--  2.0 unx     1133 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     4443 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       59 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/sbcli_release.egg-info/entry_points.txt
--rw-r--r--  2.0 unx    73366 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Mar-04 01:20 sbcli-release-1.0.4/simplyblock_cli/main.py
-128 files, 545724 bytes uncompressed, 128473 bytes compressed:  76.5%
+Zip file size: 178996 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/
+-rw-r--r--  2.0 unx      154 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/env_var
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/setup.cfg
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/pyproject.toml
+-rw-r--r--  2.0 unx     1133 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     5078 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx     1890 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     5392 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx     8654 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8169 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx    76335 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx       59 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/requires.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     5097 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     1133 b- defN 24-Apr-04 20:22 sbcli-release-1.0.5/sbcli_release.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/controllers/
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    63054 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx     6262 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx    21428 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/compute_node_ops.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-04 20:22 sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/stack_deploy_wait.sh
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     4853 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     7218 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6245 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     3222 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    46636 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx    10787 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx    13535 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1427 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-04 20:21 sbcli-release-1.0.5/simplyblock_core/controllers/pool_controller.py
+144 files, 983387 bytes uncompressed, 151652 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -1,385 +1,433 @@
-Filename: sbcli-release-1.0.4/
+Filename: sbcli-release-1.0.5/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/
+Filename: sbcli-release-1.0.5/simplyblock_web/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/
+Filename: sbcli-release-1.0.5/simplyblock_cli/
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_cli/
+Filename: sbcli-release-1.0.5/simplyblock_core/
 Comment: 
 
-Filename: sbcli-release-1.0.4/README.md
+Filename: sbcli-release-1.0.5/env_var
 Comment: 
 
-Filename: sbcli-release-1.0.4/setup.cfg
+Filename: sbcli-release-1.0.5/setup.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/pyproject.toml
+Filename: sbcli-release-1.0.5/setup.cfg
 Comment: 
 
-Filename: sbcli-release-1.0.4/PKG-INFO
+Filename: sbcli-release-1.0.5/README.md
 Comment: 
 
-Filename: sbcli-release-1.0.4/setup.py
+Filename: sbcli-release-1.0.5/pyproject.toml
 Comment: 
 
-Filename: sbcli-release-1.0.4/env_var
+Filename: sbcli-release-1.0.5/PKG-INFO
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/
+Filename: sbcli-release-1.0.5/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/
+Filename: sbcli-release-1.0.5/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/templates/
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/app.py
+Filename: sbcli-release-1.0.5/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/caching_node_app.py
+Filename: sbcli-release-1.0.5/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/snode_app.py
+Filename: sbcli-release-1.0.5/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/utils.py
+Filename: sbcli-release-1.0.5/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/node_utils.py
+Filename: sbcli-release-1.0.5/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli-release-1.0.5/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/auth_middleware.py
+Filename: sbcli-release-1.0.5/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/node_webapp.py
+Filename: sbcli-release-1.0.5/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli-release-1.0.5/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli-release-1.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/csi.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/is_up.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/list_deps.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/deploy.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/tst.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/rpac.yaml
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/static/delete.py
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/
+Filename: sbcli-release-1.0.5/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/
+Filename: sbcli-release-1.0.5/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/constants.py
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/rpc_client.py
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/pci_utils.py
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/snode_client.py
+Filename: sbcli-release-1.0.5/sbcli_release.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/shell_utils.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/compute_node_ops.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/cnode_client.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/utils.py
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/distr_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/storage_node_ops.py
+Filename: sbcli-release-1.0.5/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli-release-1.0.5/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/cluster_ops.py
+Filename: sbcli-release-1.0.5/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/kv_store.py
+Filename: sbcli-release-1.0.5/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/pool.py
+Filename: sbcli-release-1.0.5/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/iface.py
+Filename: sbcli-release-1.0.5/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/compute_node.py
+Filename: sbcli-release-1.0.5/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/storage_node.py
+Filename: sbcli-release-1.0.5/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/base_model.py
+Filename: sbcli-release-1.0.5/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/global_settings.py
+Filename: sbcli-release-1.0.5/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/stats.py
+Filename: sbcli-release-1.0.5/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/nvme_device.py
+Filename: sbcli-release-1.0.5/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/port_stat.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/events.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/cluster.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/caching_node.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/lvol_model.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/mgmt_node.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/models/snapshot.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/health_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/storage_events.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/events_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli-release-1.0.5/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli-release-1.0.5/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/log_agg_service.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/install_service.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/health_check_service.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/remove_service.sh
+Filename: sbcli-release-1.0.5/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/device_monitor.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli-release-1.0.5/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/__init__.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/capacity_collector.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/cap_monitor.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_core/services/service_template.service
+Filename: sbcli-release-1.0.5/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/top_level.txt
+Filename: sbcli-release-1.0.5/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/dependency_links.txt
+Filename: sbcli-release-1.0.5/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/requires.txt
+Filename: sbcli-release-1.0.5/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/PKG-INFO
+Filename: sbcli-release-1.0.5/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/SOURCES.txt
+Filename: sbcli-release-1.0.5/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/sbcli_release.egg-info/entry_points.txt
+Filename: sbcli-release-1.0.5/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_cli/cli.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli-release-1.0.4/simplyblock_cli/main.py
+Filename: sbcli-release-1.0.5/simplyblock_core/models/base_model.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/models/lvol_model.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/__init__.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/storage_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/cluster_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/events_controller.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/lvol_controller.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/pool_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/caching_node_controller.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/snapshot_controller.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/mgmt_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/device_controller.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/lvol_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/device_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/snapshot_events.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/health_controller.py
+Comment: 
+
+Filename: sbcli-release-1.0.5/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli-release-1.0.4/README.md` & `sbcli-release-1.0.5/README.md`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/PKG-INFO` & `sbcli-release-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-release
-Version: 1.0.4
+Version: 1.0.5
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-release-1.0.4/setup.py` & `sbcli-release-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 COMMAND_NAME = get_env_var("SIMPLY_BLOCK_COMMAND_NAME", "sbcli")
 VERSION = get_env_var("SIMPLY_BLOCK_VERSION", "1")
 
 data_files = gen_data_files(
         "simplyblock_core/controllers",
         "simplyblock_core/models",
         "simplyblock_core/scripts",
+        "simplyblock_core/scripts/alerting",
+        "simplyblock_core/scripts/dashboards",
         "simplyblock_core/services",
         "simplyblock_web/blueprints",
         "simplyblock_web/static",
         "simplyblock_web/templates")
 
 data_files.append(('', ['env_var']))
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/app.py` & `sbcli-release-1.0.5/simplyblock_web/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 from flask import Flask
 
 import utils
 from blueprints import csi, web_api_cluster, web_api_mgmt_node, web_api_device, \
     web_api_lvol, web_api_storage_node, web_api_pool, web_api_caching_node
 from auth_middleware import token_required
+from simplyblock_core import constants
 
 logger_handler = logging.StreamHandler()
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 logger = logging.getLogger()
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
@@ -40,8 +41,8 @@
 @app.route('/', methods=['GET'])
 def status():
     return utils.get_response("Live")
 
 
 app.config['JSONIFY_PRETTYPRINT_REGULAR'] = True
 if __name__ == '__main__':
-    app.run(host='0.0.0.0', debug=True)
+    app.run(host='0.0.0.0', debug=constants.LOG_WEB_DEBUG)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/caching_node_app.py` & `sbcli-release-1.0.5/simplyblock_web/caching_node_app_k8s.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
 from flask import Flask
 
 import utils
-
+from simplyblock_core import constants
 
 logger_handler = logging.StreamHandler()
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 logger = logging.getLogger()
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
@@ -19,15 +19,15 @@
 
 @app.route('/', methods=['GET'])
 def status():
     return utils.get_response("Live")
 
 
 # Add snode_ops routes
-from blueprints import caching_node_ops
-app.register_blueprint(caching_node_ops.bp)
+from blueprints import caching_node_ops_k8s
+app.register_blueprint(caching_node_ops_k8s.bp)
 
 
 app.config['JSONIFY_PRETTYPRINT_REGULAR'] = True
 
 if __name__ == '__main__':
-    app.run(host='0.0.0.0', debug=True)
+    app.run(host='0.0.0.0', debug=constants.LOG_WEB_DEBUG)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/snode_app.py` & `sbcli-release-1.0.5/simplyblock_web/snode_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
 from flask import Flask
 
 import utils
-
+from simplyblock_core import constants
 
 logger_handler = logging.StreamHandler()
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 logger = logging.getLogger()
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
@@ -26,8 +26,8 @@
 from blueprints import snode_ops
 app.register_blueprint(snode_ops.bp)
 
 
 app.config['JSONIFY_PRETTYPRINT_REGULAR'] = True
 
 if __name__ == '__main__':
-    app.run(host='0.0.0.0', debug=True)
+    app.run(host='0.0.0.0', debug=constants.LOG_WEB_DEBUG)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/utils.py` & `sbcli-release-1.0.5/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/node_utils.py` & `sbcli-release-1.0.5/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/caching_node_app_k8s.py` & `sbcli-release-1.0.5/simplyblock_web/caching_node_app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
 from flask import Flask
 
 import utils
-
+from simplyblock_core import constants
 
 logger_handler = logging.StreamHandler()
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 logger = logging.getLogger()
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
@@ -19,15 +19,15 @@
 
 @app.route('/', methods=['GET'])
 def status():
     return utils.get_response("Live")
 
 
 # Add snode_ops routes
-from blueprints import caching_node_ops_k8s
-app.register_blueprint(caching_node_ops_k8s.bp)
+from blueprints import caching_node_ops
+app.register_blueprint(caching_node_ops.bp)
 
 
 app.config['JSONIFY_PRETTYPRINT_REGULAR'] = True
 
 if __name__ == '__main__':
-    app.run(host='0.0.0.0', debug=True)
+    app.run(host='0.0.0.0', debug=constants.LOG_WEB_DEBUG)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/auth_middleware.py` & `sbcli-release-1.0.5/simplyblock_web/auth_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,22 @@
             return {
                 "message": "Authentication Token is missing!",
                 "data": None,
                 "error": "Unauthorized"
             }, 401
         try:
             db_controller = kv_store.DBController()
-            cls = db_controller.get_clusters(cluster_id)
-            if not cls:
+            cluster = db_controller.get_cluster_by_id(cluster_id)
+            if not cluster:
                 return {
                     "message": "Invalid Cluster ID",
                     "data": None,
                     "error": "Unauthorized"
                 }, 401
-            if cls[0].secret != cluster_secret:
+            if cluster.secret != cluster_secret:
                 return {
                     "message": "Invalid Cluster secret",
                     "data": None,
                     "error": "Unauthorized"
                 }, 401
         except Exception as e:
             return {
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/node_webapp.py` & `sbcli-release-1.0.5/simplyblock_web/node_webapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # encoding: utf-8
 import argparse
 import logging
 
 from flask import Flask
 
 import utils
-
+from simplyblock_core import constants
 
 logger_handler = logging.StreamHandler()
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 logger = logging.getLogger()
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
@@ -49,8 +49,8 @@
         app.register_blueprint(node_api_basic.bp)
         app.register_blueprint(node_api_caching_ks.bp)
 
     if mode == "storage_node":
         from blueprints import snode_ops
         app.register_blueprint(snode_ops.bp)
 
-    app.run(host='0.0.0.0', debug=True)
+    app.run(host='0.0.0.0', debug=constants.LOG_WEB_DEBUG)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,103 +66,82 @@
 
     return utils.get_response(c.to_dict()), 201
 
 
 @bp.route('/cluster', methods=['GET'], defaults={'uuid': None})
 @bp.route('/cluster/<string:uuid>', methods=['GET'])
 def list_clusters(uuid):
+    clusters_list = []
     if uuid:
-        cls = db_controller.get_clusters(uuid)
-        if not cls:
+        cl = db_controller.get_cluster_by_id(uuid)
+        if cl:
+            clusters_list.append(cl)
+        else:
             return utils.get_response_error(f"Cluster not found: {uuid}", 404)
     else:
         cls = db_controller.get_clusters()
+        if cls:
+            clusters_list.extend(cls)
 
     data = []
-
-    for cl in cls:
-        d = cl.get_clean_dict()
-        d['status_code'] = cl.get_status_code()
+    for cluster in clusters_list:
+        d = cluster.get_clean_dict()
+        d['status_code'] = cluster.get_status_code()
         data.append(d)
     return utils.get_response(data)
 
 
 @bp.route('/cluster/capacity/<string:uuid>/history/<string:history>', methods=['GET'])
 @bp.route('/cluster/capacity/<string:uuid>', methods=['GET'], defaults={'history': None})
 def cluster_capacity(uuid, history):
-    cls = db_controller.get_clusters(id=uuid)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(uuid)
+    if not cluster:
         logger.error(f"Cluster not found {uuid}")
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    cl = cls[0]
 
     ret = cluster_ops.get_capacity(uuid, history, parse_sizes=False)
     return utils.get_response(ret)
 
 
 @bp.route('/cluster/iostats/<string:uuid>/history/<string:history>', methods=['GET'])
 @bp.route('/cluster/iostats/<string:uuid>', methods=['GET'], defaults={'history': None})
 def cluster_iostats(uuid, history):
-    cls = db_controller.get_clusters(id=uuid)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(uuid)
+    if not cluster:
         logger.error(f"Cluster not found {uuid}")
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
 
     out = cluster_ops.get_iostats_history(uuid, history, parse_sizes=False)
     return utils.get_response(out)
 
 
 @bp.route('/cluster/status/<string:uuid>', methods=['GET'])
 def cluster_status(uuid):
-    cls = db_controller.get_clusters(id=uuid)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(uuid)
+    if not cluster:
         logger.error(f"Cluster not found {uuid}")
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    cl = cls[0]
     data = cluster_ops.show_cluster(uuid, is_json=True)
     return utils.get_response(json.loads(data))
 
 
 @bp.route('/cluster/enable/<string:uuid>', methods=['PUT'])
 def cluster_enable(uuid):
     return utils.get_response("Not Implemented!")
-    cls = db_controller.get_clusters(id=uuid)
-    if not cls:
-        return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    cl = cls[0]
-    if cl.status == cl.STATUS_ACTIVE:
-        return utils.get_response("Cluster already active")
-
-    cl.status = Cluster.STATUS_ACTIVE
-    cl.write_to_db(db_controller.kv_store)
-
-    return utils.get_response(cl.get_clean_dict())
 
 
 @bp.route('/cluster/disable/<string:uuid>', methods=['PUT'])
 def cluster_disable(uuid):
     return utils.get_response("Not Implemented!")
-    cls = db_controller.get_clusters(id=uuid)
-    if not cls:
-        return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    cl = cls[0]
-    if cl.status == cl.STATUS_INACTIVE:
-        return utils.get_response("Cluster already inactive")
-
-    cl.status = Cluster.STATUS_INACTIVE
-    cl.write_to_db(db_controller.kv_store)
-
-    return utils.get_response(cl.get_clean_dict())
 
 
 @bp.route('/cluster/get-logs/<string:uuid>', methods=['GET'])
 def cluster_get_logs(uuid):
-    cls = db_controller.get_clusters(id=uuid)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(uuid)
+    if not cluster:
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    cl = cls[0]
-    if cl.status == cl.STATUS_INACTIVE:
+    if cluster.status == Cluster.STATUS_INACTIVE:
         return utils.get_response("Cluster already inactive")
 
     data = cluster_ops.get_logs(uuid, is_json=True)
     return utils.get_response(json.loads(data))
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import cpuinfo
 import docker
 from docker.types import LogConfig
 from flask import Blueprint
 from flask import request
 
-from simplyblock_web import utils
+from simplyblock_web import utils, node_utils
 from simplyblock_core import scripts, constants
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("caching_node", __name__, url_prefix="/cnode")
 
 
@@ -176,14 +176,15 @@
         privileged=True,
         network_mode="host",
         log_config=LogConfig(type=LogConfig.types.JOURNALD),
         volumes=[
             '/var/tmp:/var/tmp',
             '/dev:/dev',
             '/lib/modules/:/lib/modules/',
+            '/var/lib/systemd/coredump/:/var/lib/systemd/coredump/',
             '/sys:/sys'],
         # restart_policy={"Name": "on-failure", "MaximumRetryCount": 99}
     )
 
     server_ip = data['server_ip']
     rpc_port = data['rpc_port']
     rpc_username = data['rpc_username']
@@ -290,14 +291,15 @@
         "system_id": system_id,
 
         "cpu_count": cpuinfo.get_cpu_info()['count'],
         "cpu_hz": cpuinfo.get_cpu_info()['hz_advertised'][0],
 
         "memory": get_memory(),
         "hugepages": get_huge_memory(),
+        "memory_details": node_utils.get_memory_details(),
 
         "nvme_devices": _get_nvme_devices(),
         "nvme_pcie_list": _get_nvme_pcie_list(),
 
         "spdk_devices": _get_spdk_devices(),
         "spdk_pcie_list": _get_spdk_pcie_list(),
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_device.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
 
 from flask import Blueprint
 
+from simplyblock_core.controllers import device_controller
 from simplyblock_web import utils
 
-from simplyblock_core import kv_store, storage_node_ops
+from simplyblock_core import kv_store
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("device", __name__)
 db_controller = kv_store.DBController()
 
 
@@ -46,43 +47,43 @@
 @bp.route('/device/capacity/<string:uuid>/history/<string:history>', methods=['GET'])
 @bp.route('/device/capacity/<string:uuid>', methods=['GET'], defaults={'history': None})
 def device_capacity(uuid, history):
     device = db_controller.get_storage_devices(uuid)
     if not device:
         return utils.get_response_error(f"devices not found: {uuid}", 404)
 
-    records = storage_node_ops.get_device_capacity(uuid, history, parse_sizes=False)
+    records = device_controller.get_device_capacity(uuid, history, parse_sizes=False)
     return utils.get_response(records)
 
 
 @bp.route('/device/iostats/<string:uuid>/history/<string:history>', methods=['GET'])
 @bp.route('/device/iostats/<string:uuid>', methods=['GET'], defaults={'history': None})
 def device_iostats(uuid, history):
     devices = db_controller.get_storage_devices(uuid)
     if not devices:
         return utils.get_response_error(f"devices not found: {uuid}", 404)
 
-    data = storage_node_ops.get_device_iostats(uuid, history, parse_sizes=False)
+    data = device_controller.get_device_iostats(uuid, history, parse_sizes=False)
     if data:
         return utils.get_response(data)
     else:
         return utils.get_response(False)
 
 
 @bp.route('/device/reset/<string:uuid>', methods=['GET'])
 def device_reset(uuid):
     devices = db_controller.get_storage_devices(uuid)
     if not devices:
         return utils.get_response_error(f"devices not found: {uuid}", 404)
 
-    data = storage_node_ops.reset_storage_device(uuid)
+    data = device_controller.reset_storage_device(uuid)
     return utils.get_response(data)
 
 
 @bp.route('/device/remove/<string:uuid>', methods=['GET'])
 def device_remove(uuid):
     devices = db_controller.get_storage_devices(uuid)
     if not devices:
         return utils.get_response_error(f"devices not found: {uuid}", 404)
 
-    data = storage_node_ops.device_remove(uuid)
+    data = device_controller.device_remove(uuid)
     return utils.get_response(data)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     cluster_id = cl_data['cluster_id']
     node_ip = cl_data['node_ip']
     iface_name = cl_data['iface_name']
 
     data_nics_list = []
     spdk_cpu_mask = None
     spdk_mem = None
+    spdk_image = None
 
     if 'spdk_cpu_mask' in cl_data:
         spdk_cpu_mask = cl_data['spdk_cpu_mask']
 
     if 'spdk_mem' in cl_data:
         mem = cl_data['spdk_mem']
         spdk_mem = utils.parse_size(mem)
@@ -45,15 +46,16 @@
 
     if 'spdk_image' in cl_data:
         spdk_image = cl_data['spdk_image']
 
     if 'spdk_image' in cl_data:
         spdk_image = cl_data['spdk_image']
 
-    ret = caching_node_controller.add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image)
+    ret = caching_node_controller.add_node(
+        cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image)
 
     return utils.get_response(ret)
 
 
 @bp.route('/cachingnode', methods=['GET'], defaults={'uuid': None})
 @bp.route('/cachingnode/<string:uuid>', methods=['GET'])
 def list_caching_nodes(uuid):
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/snode_ops.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/snode_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 @bp.route('/spdk_process_start', methods=['POST'])
 def spdk_process_start():
     try:
         data = request.get_json()
     except:
         data = {}
 
-    cmd_params = None
-    if 'cmd_params' in data and data['cmd_params']:
-        cmd_params = data['cmd_params']
+    set_debug = None
+    if 'spdk_debug' in data and data['spdk_debug']:
+        set_debug = data['spdk_debug']
 
     spdk_cpu_mask = None
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
     spdk_mem = None
     if 'spdk_mem' in data:
         spdk_mem = data['spdk_mem']
@@ -85,41 +85,43 @@
     for node in nodes:
         if node.attrs["Name"] in ["/spdk", "/spdk_proxy"]:
             logger.info(f"{node.attrs['Name']} container found, removing...")
             node.stop()
             node.remove(force=True)
             time.sleep(2)
 
-    params_line = ""
-    if cmd_params:
-        params_line = " ".join(cmd_params)
+    spdk_debug = 0
+    if set_debug:
+        spdk_debug = 1
 
     spdk_image = constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE
     if 'spdk_image' in data and data['spdk_image']:
         spdk_image = data['spdk_image']
-        node_docker.images.pull(spdk_image)
+        # node_docker.images.pull(spdk_image)
 
     if "cluster_ip" in data and data['cluster_ip']:
         cluster_ip = data['cluster_ip']
         log_config = LogConfig(type=LogConfig.types.GELF, config={"gelf-address": f"udp://{cluster_ip}:12201"})
     else:
         log_config = LogConfig(type=LogConfig.types.JOURNALD)
 
     container = node_docker.containers.run(
         spdk_image,
-        f"/root/scripts/run_distr.sh {spdk_cpu_mask} {spdk_mem} {params_line}",
+        f"/root/scripts/run_distr.sh {spdk_cpu_mask} {spdk_mem} {spdk_debug}",
         name="spdk",
         detach=True,
         privileged=True,
         network_mode="host",
         log_config=log_config,
         volumes=[
+            '/etc/simplyblock:/etc/simplyblock',
             '/var/tmp:/var/tmp',
             '/dev:/dev',
             '/lib/modules/:/lib/modules/',
+            '/var/lib/systemd/coredump/:/var/lib/systemd/coredump/',
             '/sys:/sys'],
         # restart_policy={"Name": "on-failure", "MaximumRetryCount": 99}
     )
     container2 = node_docker.containers.run(
         constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE,
         "python /root/scripts/spdk_http_proxy.py",
         name="spdk_proxy",
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,28 @@
     if 'spdk_image' in data and data['spdk_image']:
         spdk_image = data['spdk_image']
 
     if _is_pod_up():
         logger.info("SPDK deployment found, removing...")
         spdk_process_kill()
 
+    node_name = os.environ.get("HOSTNAME")
+    logger.debug(f"deploying caching node spdk on worker: {node_name}")
+
     env = Environment(loader=FileSystemLoader(os.path.join(TOP_DIR, 'templates')), trim_blocks=True, lstrip_blocks=True)
     template = env.get_template('deploy_spdk.yaml.j2')
     values = {
         'SPDK_IMAGE': spdk_image,
         'SPDK_CPU_MASK': spdk_cpu_mask,
         'SPDK_MEM': spdk_mem,
         'SERVER_IP': data['server_ip'],
         'RPC_PORT': data['rpc_port'],
         'RPC_USERNAME': data['rpc_username'],
         'RPC_PASSWORD': data['rpc_password'],
+        'HOSTNAME': node_name,
     }
     dep = yaml.safe_load(template.render(values))
     resp = k8s_apps_v1.create_namespaced_deployment(body=dep, namespace=namespace)
     logger.info(f"Deployment created: '{resp.metadata.name}'")
 
     retries = 20
     while retries > 0:
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,17 +166,17 @@
     node_ip = req_data['node_ip']
     ifname = req_data['ifname']
 
     spdk_image = None
     if 'spdk_image' in req_data:
         spdk_image = req_data['spdk_image']
 
-    cmd_params = None
-    if 'cmd_params' in req_data:
-        cmd_params = req_data['cmd_params']
+    spdk_debug = None
+    if 'spdk_debug' in req_data:
+        spdk_debug = req_data['spdk_debug']
 
     data_nics = None
     if 'data_nics' in req_data:
         data_nics = req_data['data_nics']
         data_nics = data_nics.split(",")
 
     spdk_cpu_mask = None
@@ -192,10 +192,10 @@
         mem = req_data['spdk_mem']
         spdk_mem = utils.parse_size(mem)
         if spdk_mem < 1 * 1024 * 1024:
             return utils.get_response_error(f"SPDK memory:{mem} must be larger than 1G", 400)
 
     out = storage_node_ops.add_node(
         cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem,
-        spdk_image=spdk_image, cmd_params=cmd_params)
+        spdk_image=spdk_image, spdk_debug=spdk_debug)
 
     return utils.get_response(out)
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_basic.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/csi.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/csi.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,19 @@
     logger.debug(f"Headers:secret={secret}")
     if not cl_id:
         logger.error("no 'cluster' key found in the request headers")
         return False
     if not secret:
         logger.error("no 'secret' key found in the request headers")
         return False
-    cluster = db_controller.get_clusters(cl_id)
+    cluster = db_controller.get_cluster_by_id(cl_id)
     if not cluster:
         logger.error(f"Cluster not found: {cl_id}")
         return False
-    if cluster[0].secret == secret:
+    if cluster.secret == secret:
         return True
 
 
 @bp.route('/csi/get_pools', methods=['GET'])
 def csi_get_pools():
     if not validate_header_data():
         return utils.get_csi_response(None, "Invalid Auth data, see API logs for more details.")
```

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/web_api_pool.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli-release-1.0.5/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/static/deploy_spdk.yaml` & `sbcli-release-1.0.5/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/static/deploy.py` & `sbcli-release-1.0.5/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/static/delete.py` & `sbcli-release-1.0.5/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli-release-1.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/constants.py` & `sbcli-release-1.0.5/simplyblock_core/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 KVD_DB_VERSION = 730
 KVD_DB_FILE_PATH = '/etc/foundationdb/fdb.cluster'
 KVD_DB_TIMEOUT_MS = 10000
 SPK_DIR = '/home/ec2-user/spdk'
 RPC_HTTP_PROXY_PORT = 8080
 LOG_LEVEL = logging.INFO
+LOG_WEB_DEBUG = True
 
 FILE_DIR = os.path.dirname(os.path.realpath(__file__))
 INSTALL_DIR = os.path.dirname(FILE_DIR)
 TOP_DIR = os.path.dirname(INSTALL_DIR)
 
 NODE_MONITOR_INTERVAL_SEC = 3
 DEVICE_MONITOR_INTERVAL_SEC = 5
 STAT_COLLECTOR_INTERVAL_SEC = 60*5  # 5 minutes
 LVOL_STAT_COLLECTOR_INTERVAL_SEC = 2
 LVOL_MONITOR_INTERVAL_SEC = 60
 DEV_MONITOR_INTERVAL_SEC = 10
 DEV_STAT_COLLECTOR_INTERVAL_SEC = 2
 PROT_STAT_COLLECTOR_INTERVAL_SEC = 2
 DISTR_EVENT_COLLECTOR_INTERVAL_SEC = 2
+CAP_MONITOR_INTERVAL_SEC = 30
 SSD_VENDOR_WHITE_LIST = ["1d0f:cd01", "1d0f:cd00"]
 
 PMEM_DIR = '/tmp/pmem'
 
 NVME_PROGRAM_FAIL_COUNT = 50
 NVME_ERASE_FAIL_COUNT = 50
 NVME_CRC_ERROR_COUNT = 50
@@ -45,9 +47,11 @@
 # To use 75% of hugepages to calculate ssd size to use for the ocf bdev
 CACHING_NODE_MEMORY_FACTOR = 0.75
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
 
 SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:v1.0.4"
-SIMPLY_BLOCK_SPDK_CORE_IMAGE = "hamdykhader/spdk:core"
-SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "hamdykhader/spdk:latest"
+SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
+SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
+
+GELF_PORT = 12201
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/rpc_client.py` & `sbcli-release-1.0.5/simplyblock_core/rpc_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.message = message
 
 
 class RPCClient:
 
     # ref: https://spdk.io/doc/jsonrpc.html
 
-    def __init__(self, ip_address, port, username, password, timeout=30, retry=3):
+    def __init__(self, ip_address, port, username, password, timeout=60, retry=10):
         self.ip_address = ip_address
         self.port = port
         self.url = 'http://%s:%s/' % (self.ip_address, self.port)
         self.username = username
         self.password = password
         self.timeout = timeout
         self.session = requests.session()
@@ -364,15 +364,15 @@
             "pba_init_mode": pba_init_mode,
             "pba_page_size": 2097152,
             "uuid": uuid,
             # "use_scheduling": True,
             "use_optimized": True,
             "pba_nbalign": 4096
         }
-        return self._request2("bdev_alceml_create", params)
+        return self._request("bdev_alceml_create", params)
 
     def bdev_distrib_create(self, name, vuid, ndcs, npcs, num_blocks, block_size, jm_names,
                             chunk_size, ha_comm_addrs=None, ha_inode_self=None, pba_page_size=2097152):
         """"
             // Optional (not specified = no HA)
             // Comma-separated communication addresses, for each node, e.g. "192.168.10.1:45001,192.168.10.1:32768".
             // Number of addresses in the list is exactly the number of nodes in HA group,
@@ -504,19 +504,20 @@
         params = {
             "pt_name": name
         }
         return self._request("bdev_passtest_delete", params)
 
     def bdev_nvme_set_options(self):
         params = {
-            "action_on_timeout": "none",
+            "bdev_retry_count": 0,
+            "transport_retry_count": 0,
             "ctrlr_loss_timeout_sec": -1,
-            "reconnect_delay_sec": 15,
-            "transport_retry_count": 1,
-            "bdev_retry_count": 1}
+            "fast_io_fail_timeout_sec": 5,
+            "reconnect_delay_sec": 5,
+        }
         return self._request("bdev_nvme_set_options", params)
 
     def bdev_set_options(self, bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size):
         params = {}
         if bdev_io_pool_size > 0:
             params['bdev_io_pool_size'] = bdev_io_pool_size
         if bdev_io_cache_size > 0:
@@ -526,14 +527,30 @@
         if iobuf_small_cache_size > 0:
             params['iobuf_large_cache_size'] = iobuf_large_cache_size
         if params:
             return self._request("bdev_set_options", params)
         else:
             return False
 
+    def iobuf_set_options(self, small_pool_count, large_pool_count, small_bufsize, large_bufsize):
+        params = {}
+        if small_pool_count > 0:
+            params['small_pool_count'] = small_pool_count
+        if large_pool_count > 0:
+            params['large_pool_count'] = large_pool_count
+        if small_bufsize > 0:
+            params['small_bufsize'] = small_bufsize
+        if large_bufsize > 0:
+            params['large_bufsize'] = large_bufsize
+        if params:
+            return self._request("iobuf_set_options", params)
+        else:
+            return False
+
+
     def distr_status_events_get(self):
         return self._request("distr_status_events_get")
 
     def alceml_get_capacity(self, name):
         params = {"name": name}
         return self._request("alceml_get_pages_usage", params)
 
@@ -577,25 +594,54 @@
         return self._request("ultra21_lvol_mount", params)
 
     def ultra21_lvol_mount_lvol(self, lvol_name, base_bdev, label, desc):
         params = {
             "modus": "BASE",
             "lvol_bdev": lvol_name,
             "base_bdev": base_bdev,
-            "label": label,
-            "desc": desc
+            # "label": label,
+            # "desc": desc
         }
         return self._request("ultra21_lvol_mount", params)
 
+    def ultra21_lvol_dismount(self, lvol_name):
+        params = {
+            "lvol_bdev": lvol_name
+        }
+        return self._request("ultra21_lvol_dismount", params)
+
     def bdev_jm_create(self, name, name_storage1, block_size=4096):
         params = {
             "name": name,
             "name_storage1": name_storage1,
             "block_size": block_size
         }
         return self._request("bdev_jm_create", params)
 
-
     def bdev_jm_delete(self, name):
         params = {"name": name}
         return self._request("bdev_jm_delete", params)
 
+    def ultra21_util_get_malloc_stats(self):
+        params = {"socket_id": 0}
+        return self._request("ultra21_util_get_malloc_stats", params)
+
+    def ultra21_lvol_mount_clone(self, clone_name, snap_bdev, base_bdev):
+        params = {
+            "modus": "CLONE",
+            "lvol_bdev": clone_name,
+            "base_bdev": base_bdev,
+            "snapshot_bdev": snap_bdev
+        }
+        return self._request("ultra21_lvol_mount", params)
+
+    def alceml_unmap_vuid(self, name, vuid):
+        params = {"name": name, "vuid": vuid}
+        return self._request("alceml_unmap_vuid", params)
+
+    def jm_delete(self):
+        params = {"name": 0, "vuid": 0}
+        return self._request("jm_delete", params)
+
+    def framework_start_init(self):
+        return self._request("framework_start_init")
+
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/pci_utils.py` & `sbcli-release-1.0.5/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/snode_client.py` & `sbcli-release-1.0.5/simplyblock_core/snode_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class SNodeClientException(Exception):
     def __init__(self, message):
         self.message = message
 
 
 class SNodeClient:
 
-    def __init__(self, ip_address, timeout=30, retry=3):
+    def __init__(self, ip_address, timeout=60, retry=5):
         self.ip_address = ip_address
         self.url = 'http://%s/snode/' % self.ip_address
         self.timeout = timeout
         self.session = requests.session()
         self.session.verify = False
         self.session.timeout = self.timeout
         self.session.headers['Content-Type'] = "application/json"
@@ -32,15 +32,15 @@
         try:
             logger.debug("Requesting path: %s, params: %s", path, params)
             dt = None
             if params:
                 dt = json.dumps(params)
             response = self.session.request(method, self.url+path, data=dt, timeout=self.timeout)
         except Exception as e:
-            raise e
+            return None, str(e)
 
         logger.debug("Response: status_code: %s, content: %s",
                      response.status_code, response.content)
         ret_code = response.status_code
 
         result = None
         error = None
@@ -66,24 +66,24 @@
 
     def is_live(self):
         return self._request("GET", "")
 
     def info(self):
         return self._request("GET", "info")
 
-    def spdk_process_start(self, spdk_cpu_mask, spdk_mem, spdk_image=None, cmd_params=None, cluster_ip=None):
+    def spdk_process_start(self, spdk_cpu_mask, spdk_mem, spdk_image=None, spdk_debug=None, cluster_ip=None):
         params = {"cluster_ip": cluster_ip}
         if spdk_cpu_mask:
             params['spdk_cpu_mask'] = spdk_cpu_mask
         if spdk_mem:
             params['spdk_mem'] = spdk_mem
         if spdk_image:
             params['spdk_image'] = spdk_image
-        if cmd_params:
-            params['cmd_params'] = cmd_params
+        if spdk_debug:
+            params['spdk_debug'] = spdk_debug
         return self._request("POST", "spdk_process_start", params)
 
     def join_swarm(self, cluster_ip, join_token, db_connection, cluster_id):
         params = {
             "cluster_ip": cluster_ip,
             "cluster_id": cluster_id,
             "join_token": join_token,
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/compute_node_ops.py` & `sbcli-release-1.0.5/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/cnode_client.py` & `sbcli-release-1.0.5/simplyblock_core/cnode_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         logger.error("Unknown http status: %s", ret_code)
         return None, None
 
     def is_live(self):
         return self._request("GET", "")
 
     def info(self):
-        return self._request("GET", "info")
+        return self._request("GET", "cnode/info")
 
     def spdk_process_start(self, spdk_cpu_mask, spdk_mem, spdk_image, server_ip, rpc_port, rpc_username, rpc_password):
         params = {
             "spdk_cpu_mask": spdk_cpu_mask,
             "spdk_mem": spdk_mem,
             "spdk_image": spdk_image,
             "server_ip": server_ip,
@@ -89,19 +89,19 @@
         return self._request("GET", "cnode/spdk_process_kill")
 
     def connect_nvme(self, ip, port, nqn):
         params = {
             "ip": ip,
             "port": port,
             "nqn": nqn}
-        return self._request("POST", "nvme_connect", params)
+        return self._request("POST", "cnode/nvme_connect", params)
 
     def disconnect_device(self, dev_path):
         params = {"dev_path": dev_path}
-        return self._request("POST", "disconnect_device", params)
+        return self._request("POST", "cnode/disconnect_device", params)
 
     def disconnect_nqn(self, nqn):
         params = {"nqn": nqn}
-        return self._request("POST", "disconnect_nqn", params)
+        return self._request("POST", "cnode/disconnect_nqn", params)
 
     def disconnect_all(self):
-        return self._request("POST", "disconnect_all")
+        return self._request("POST", "cnode/disconnect_all")
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/utils.py` & `sbcli-release-1.0.5/simplyblock_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     if out and ifname in out:
         return out[ifname]['ip']
     return False
 
 
 def print_table(data: list):
     if data:
-        x = PrettyTable(field_names=data[0].keys())
+        x = PrettyTable(field_names=data[0].keys(), max_width=70)
         x.align = 'l'
         for node_data in data:
             row = []
             for key in node_data:
                 row.append(node_data[key])
             x.add_row(row)
         return x.__str__()
@@ -272,7 +272,11 @@
     elif len(records) == 1:
         return records[0]
     else:
         total = records[0]
         for rec in records[1:]:
             total += rec
         return total
+
+
+def get_random_vuid():
+    return 1 + int(random.random() * 10000)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/distr_controller.py` & `sbcli-release-1.0.5/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/storage_node_ops.py` & `sbcli-release-1.0.5/simplyblock_core/storage_node_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import time
 import uuid
 
 import docker
 
 from simplyblock_core import constants, scripts, distr_controller
 from simplyblock_core import utils
-from simplyblock_core.controllers import lvol_controller, storage_events, snapshot_controller
+from simplyblock_core.controllers import lvol_controller, storage_events, snapshot_controller, device_events, \
+    device_controller
 from simplyblock_core.kv_store import DBController
 from simplyblock_core import shell_utils
 from simplyblock_core.models.iface import IFace
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.pci_utils import get_nvme_devices, bind_spdk_driver
 from simplyblock_core.rpc_client import RPCClient
@@ -88,15 +89,15 @@
         ctr_map = {}
 
     for index, pcie in enumerate(devs):
 
         if pcie in ctr_map:
             nvme_bdev = ctr_map[pcie] + "n1"
         else:
-            name = "nvme_%s" % pcie.split(":")[2].split(".")[0]
+            name = "nvme_%s" % index
             ret, err = rpc_client.bdev_nvme_controller_attach(name, pcie)
             time.sleep(2)
             nvme_bdev = f"{name}n1"
 
         ret = rpc_client.get_bdevs(nvme_bdev)
         if ret:
             nvme_dict = ret[0]
@@ -116,14 +117,19 @@
                     'pcie_address': nvme_driver_data['pci_address'],
                     'model_id': model_number,
                     'serial_number': nvme_driver_data['ctrlr_data']['serial_number'],
                     'nvme_bdev': nvme_bdev,
                     'alloc_bdev': nvme_bdev,
                     'node_id': snode.get_id(),
                     'cluster_id': snode.cluster_id,
+
+                    # 'nvmf_nqn': subsystem_nqn,
+                    # 'nvmf_ip': IP,
+                    # 'nvmf_port': 4420,
+
                     'status': 'online'
                 }))
             sequential_number += device_partitions_count
     return devices
 
 
 def _get_nvme_list(cluster):
@@ -206,16 +212,16 @@
     db_controller = DBController()
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     for index, nvme in enumerate(snode.nvme_devices):
-        if nvme.status != NVMeDevice.STATUS_ONLINE:
-            logger.debug(f"Device is not online: {nvme.get_id()}, status: {nvme.status}")
+        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
+            logger.debug(f"Device is not online or unavailable: {nvme.get_id()}, status: {nvme.status}")
             continue
 
         test_name = f"{nvme.nvme_bdev}_test"
         # create testing bdev
         ret = rpc_client.bdev_passtest_create(test_name, nvme.nvme_bdev)
 
         alceml_id = nvme.get_id()
@@ -259,20 +265,28 @@
                 break
         logger.info(f"add {pt_name} to subsystem")
         ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, pt_name)
         if not ret:
             logger.error(f"Failed to add: {pt_name} to the subsystem: {subsystem_nqn}")
             return False
 
+        # create jm
+        if nvme.jm_bdev:
+            ret = rpc_client.bdev_jm_create(nvme.jm_bdev, alceml_name)
+            if not ret:
+                logger.error(f"Failed to create JM bdev: {snode.nvme_devices[0].jm_bdev}")
+                return False
+
         nvme.testing_bdev = test_name
         nvme.alceml_bdev = alceml_name
         nvme.pt_bdev = pt_name
         nvme.nvmf_nqn = subsystem_nqn
         nvme.nvmf_ip = IP
         nvme.nvmf_port = 4420
+        nvme.io_error = False
         nvme.status = NVMeDevice.STATUS_ONLINE
     snode.write_to_db(db_controller.kv_store)
     return True
 
 
 def _connect_to_remote_devs(this_node):
     db_controller = DBController()
@@ -299,27 +313,29 @@
                 continue
             dev.remote_bdev = f"{name}n1"
             remote_devices.append(dev)
     return remote_devices
 
 
 def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask,
-             spdk_mem, dev_split=1, spdk_image=None, cmd_params=None,
-             bdev_io_pool_size=0, bdev_io_cache_size=0, iobuf_small_cache_size=0, iobuf_large_cache_size=0):
+             spdk_mem, dev_split=1, spdk_image=None, spdk_debug=False,
+             small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
-    clusters = db_controller.get_clusters(cluster_id)
-    if not clusters:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
-    cluster = clusters[0]
 
     logger.info(f"Adding Storage node: {node_ip}")
-    snode_api = SNodeClient(node_ip)
+    timeout = 60
+    if spdk_image:
+        timeout = 5*60
+    snode_api = SNodeClient(node_ip, timeout=timeout)
     node_info, _ = snode_api.info()
     logger.info(f"Node found: {node_info['hostname']}")
     if "cluster_id" in node_info and node_info['cluster_id']:
         if node_info['cluster_id'] != cluster_id:
             logger.error(f"This node is part of another cluster: {node_info['cluster_id']}")
             return False
 
@@ -348,15 +364,15 @@
         cluster_id=cluster_id)
 
     if not results:
         logger.error(f"Failed to Join docker swarm: {err}")
         return False
 
     logger.info("Deploying SPDK")
-    results, err = snode_api.spdk_process_start(spdk_cpu_mask, spdk_mem, spdk_image, cmd_params, cluster_ip)
+    results, err = snode_api.spdk_process_start(spdk_cpu_mask, spdk_mem, spdk_image, spdk_debug, cluster_ip)
     time.sleep(10)
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
 
     hostname = node_info['hostname']
     snode = db_controller.get_storage_node_by_hostname(hostname)
@@ -406,31 +422,38 @@
         snode.memory = node_info['memory']
     if 'hugepages' in node_info:
         snode.hugepages = node_info['hugepages']
 
     snode.spdk_cpu_mask = spdk_cpu_mask or ""
     snode.spdk_mem = spdk_mem or 0
     snode.spdk_image = spdk_image or ""
-    snode.cmd_params = cmd_params or []
+    snode.spdk_debug = spdk_debug or 0
     snode.write_to_db(kv_store)
 
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
-    bdev_io_pool_size = bdev_io_pool_size or 0
-    bdev_io_cache_size = bdev_io_cache_size or 0
-    iobuf_small_cache_size = iobuf_small_cache_size or 0
-    iobuf_large_cache_size = iobuf_large_cache_size or 0
+    small_pool_count = small_pool_count or 0
+    large_pool_count = large_pool_count or 0
+    small_bufsize = small_bufsize or 0
+    large_bufsize = large_bufsize or 0
     # set bdev options
-    rpc_client.bdev_set_options(
-        bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size)
+    # rpc_client.bdev_set_options(
+    #     bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size)
+
+    # 1- set iobuf options
+    rpc_client.iobuf_set_options(
+        small_pool_count, large_pool_count, small_bufsize, large_bufsize)
 
-    # set nvme bdev options
+    # 2- start spdk framework
+    rpc_client.framework_start_init()
+
+    # 3- set nvme bdev options
     rpc_client.bdev_nvme_set_options()
 
     # get new node info after starting spdk
     node_info, _ = snode_api.info()
     # adding devices
     nvme_devs = addNvmeDevices(cluster, rpc_client, node_info['spdk_pcie_list'], snode)
     if not nvme_devs:
@@ -454,25 +477,28 @@
         snode.nvme_devices = nvme_devs
 
     # Set device cluster order
     dev_order = get_next_cluster_device_order(db_controller)
     for index, nvme in enumerate(snode.nvme_devices):
         nvme.cluster_device_order = dev_order
         dev_order += 1
+        device_events.device_create(nvme)
+
+    # create jm
+    snode.nvme_devices[0].jm_bdev = f"jm_{snode.get_id()}"
+
+    # save object
     snode.write_to_db(db_controller.kv_store)
 
     # prepare devices
     ret = _prepare_cluster_devices(snode)
     if not ret:
         logger.error("Failed to prepare cluster devices")
         return False
 
-    # create jm
-    rpc_client.bdev_jm_create(f"jm_{snode.get_id()}", snode.nvme_devices[0].alceml_bdev)
-
     logger.info("Connecting to remote devices")
     remote_devices = _connect_to_remote_devs(snode)
     snode.remote_devices = remote_devices
 
     logger.info("Setting node status to Active")
     snode.status = StorageNode.STATUS_ONLINE
     snode.write_to_db(kv_store)
@@ -538,19 +564,18 @@
 
 
 # Deprecated
 def add_storage_node(cluster_id, iface_name, data_nics):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
-    clusters = db_controller.get_clusters(cluster_id)
-    if not clusters:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
-    cluster = clusters[0]
 
     logger.info("Add Storage node")
 
     hostname = utils.get_hostname()
     snode = db_controller.get_storage_node_by_hostname(hostname)
     if snode:
         logger.error("Node already exists, try remove it first.")
@@ -685,14 +710,18 @@
 def remove_storage_node(node_id, force_remove=False, force_migrate=False):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
+    if snode.status == StorageNode.STATUS_ONLINE:
+        logger.error(f"Can not remove online node: {node_id}")
+        return False
+
     if snode.lvols:
         if force_migrate:
             for lvol_id in snode.lvols:
                 lvol_controller.migrate(lvol_id)
         elif force_remove:
             for lvol_id in snode.lvols:
                 lvol_controller.delete_lvol(lvol_id, True)
@@ -719,14 +748,17 @@
 
     if snode.nvme_devices:
         for dev in snode.nvme_devices:
             if dev.status == 'online':
                 distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
             distr_controller.disconnect_device(dev)
 
+    for lvol in db_controller.get_lvols():
+        lvol_controller.send_cluster_map(lvol.get_id())
+
     logger.info("Removing storage node")
 
     logger.debug("Leaving swarm...")
     try:
         node_docker = docker.DockerClient(base_url=f"tcp://{snode.mgmt_ip}:2375", version="auto")
         cluster_docker = utils.get_docker_client(snode.cluster_id)
         cluster_docker.nodes.get(node_docker.info()["Swarm"]["NodeID"]).remove(force=True)
@@ -742,28 +774,36 @@
 
     snode.remove(db_controller.kv_store)
     storage_events.snode_remove(snode)
     logger.info("done")
 
 
 def restart_storage_node(
-        node_id, spdk_cpu_mask, spdk_mem,
-        spdk_image, cmd_params,
-        bdev_io_pool_size, bdev_io_cache_size,
-        iobuf_small_cache_size, iobuf_large_cache_size):
+        node_id,
+        spdk_cpu_mask=None,
+        spdk_mem=None,
+        spdk_image=None,
+        set_spdk_debug=None,
+        small_pool_count=0, large_pool_count=0,
+        small_bufsize=0, large_bufsize=0):
+
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     db_controller = DBController()
     logger.info("Restarting storage node")
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
+    if snode.status == StorageNode.STATUS_ONLINE:
+        logger.error(f"Can not restart online node: {node_id}")
+        return False
+
     logger.info("Setting node state to restarting")
     snode.status = StorageNode.STATUS_RESTARTING
     snode.write_to_db(kv_store)
 
     logger.info(f"Restarting Storage node: {snode.mgmt_ip}")
     snode_api = SNodeClient(snode.api_endpoint)
 
@@ -779,47 +819,50 @@
     if spdk_mem:
         mem = spdk_mem
         snode.spdk_mem = mem
     img = snode.spdk_image
     if spdk_image:
         img = spdk_image
         snode.spdk_image = img
-    params = snode.cmd_params
-    if cmd_params:
-        params = cmd_params
-        snode.cmd_params = params
+    spdk_debug = snode.spdk_debug
+    if set_spdk_debug:
+        spdk_debug = spdk_debug
+        snode.spdk_debug = spdk_debug
 
     cluster_docker = utils.get_docker_client(snode.cluster_id)
     cluster_ip = cluster_docker.info()["Swarm"]["NodeAddr"]
-    results, err = snode_api.spdk_process_start(cpu, mem, img, params, cluster_ip)
+    results, err = snode_api.spdk_process_start(cpu, mem, img, spdk_debug, cluster_ip)
 
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
     time.sleep(3)
 
     snode.write_to_db(db_controller.kv_store)
 
-    clusters = db_controller.get_clusters(snode.cluster_id)
-    cluster = clusters[0]
+    cluster = db_controller.get_cluster_by_id(snode.cluster_id)
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password,
         timeout=10 * 60, retry=5)
 
-    bdev_io_pool_size = bdev_io_pool_size or 0
-    bdev_io_cache_size = bdev_io_cache_size or 0
-    iobuf_small_cache_size = iobuf_small_cache_size or 0
-    iobuf_large_cache_size = iobuf_large_cache_size or 0
-    # set bdev options
-    rpc_client.bdev_set_options(
-        bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size)
+    small_pool_count = small_pool_count or 0
+    large_pool_count = large_pool_count or 0
+    small_bufsize = small_bufsize or 0
+    large_bufsize = large_bufsize or 0
+
+    # 1- set iobuf options
+    rpc_client.iobuf_set_options(
+        small_pool_count, large_pool_count, small_bufsize, large_bufsize)
+
+    # 2- start spdk framework
+    rpc_client.framework_start_init()
 
-    # set nvme bdev options
+    # 3- set nvme bdev options
     rpc_client.bdev_nvme_set_options()
 
     node_info, _ = snode_api.info()
     nvme_devs = addNvmeDevices(cluster, rpc_client, node_info['spdk_pcie_list'], snode)
     if not nvme_devs:
         logger.error("No NVMe devices was found!")
         return False
@@ -835,15 +878,16 @@
     known_devices_sn = []
     devices_sn = [d.serial_number for d in nvme_devs]
     for db_dev in snode.nvme_devices:
         known_devices_sn.append(db_dev.serial_number)
         if db_dev.serial_number in devices_sn:
             logger.info(f"Device found: {db_dev.get_id()}")
             active_devices.append(db_dev)
-            db_dev.status = NVMeDevice.STATUS_ONLINE
+            if db_dev.status == NVMeDevice.STATUS_UNAVAILABLE:
+                db_dev.status = NVMeDevice.STATUS_ONLINE
         else:
             logger.info(f"Device not found: {db_dev.get_id()}")
             db_dev.status = NVMeDevice.STATUS_REMOVED
             distr_controller.send_dev_status_event(db_dev.cluster_device_order, "offline")
 
     for dev in nvme_devs:
         if dev.serial_number not in known_devices_sn:
@@ -859,17 +903,14 @@
 
     # prepare devices
     ret = _prepare_cluster_devices(snode, after_restart=True)
     if not ret:
         logger.error("Failed to prepare cluster devices")
         return False
 
-    # create jm
-    rpc_client.bdev_jm_create(f"jm_{snode.get_id()}", snode.nvme_devices[0].alceml_bdev)
-
     logger.info("Connecting to remote devices")
     remote_devices = _connect_to_remote_devs(snode)
     snode.remote_devices = remote_devices
 
     # make other nodes connect to the new devices
     logger.info("Make other nodes connect to the node devices")
     snodes = db_controller.get_storage_nodes()
@@ -933,14 +974,15 @@
 
     for lvol_id in snode.lvols:
         lvol = lvol_controller.recreate_lvol(lvol_id, snode)
         if not lvol:
             logger.error(f"Failed to create LVol: {lvol_id}")
             return False
         lvol.status = lvol.STATUS_ONLINE
+        lvol.io_error = False
         lvol.write_to_db(db_controller.kv_store)
 
     logger.info("Setting node status to Online")
     old_status = snode.status
     snode.status = StorageNode.STATUS_ONLINE
     snode.write_to_db(kv_store)
 
@@ -954,20 +996,24 @@
     nodes = db_controller.get_storage_nodes()
     data = []
     output = ""
 
     for node in nodes:
         logger.debug(node)
         logger.debug("*" * 20)
+        total_devices = len(node.nvme_devices)
+        online_devices = 0
+        for dev in node.nvme_devices:
+            if dev.status == NVMeDevice.STATUS_ONLINE:
+                online_devices += 1
         data.append({
             "UUID": node.uuid,
             "Hostname": node.hostname,
             "Management IP": node.mgmt_ip,
-            # "Subsystem": node.subsystem,
-            "NVMe Devs": f"{len(node.nvme_devices)}",
+            "Devices": f"{total_devices}/{online_devices}",
             "LVOLs": f"{len(node.lvols)}",
             "Data NICs": "\n".join([d.if_name for d in node.data_nics]),
             "Status": node.status,
             "Health": node.health_check,
 
             "Updated At": datetime.datetime.strptime(node.updated_at, "%Y-%m-%d %H:%M:%S.%f").strftime(
                 "%H:%M:%S, %d/%m/%Y"),
@@ -1001,14 +1047,15 @@
             "Size": utils.humanbytes(device.size),
             # "Sequential Number": device.sequential_number,
             # "Partitions Count": device.partitions_count,
             # "Model ID": device.model_id,
             "Serial Number": device.serial_number,
             "PCIe": device.pcie_address,
             "Status": device.status,
+            "IO Err": device.io_error,
             "Health": device.health_check,
 
         })
 
     if sort and sort in ['node-seq', 'dev-seq', 'serial']:
         if sort == 'serial':
             sort_key = "Serial Number"
@@ -1047,29 +1094,31 @@
     #         online_nodes += 1
     # if cls[0].ha_type == "ha" and online_nodes <= 3:
     #     logger.warning(f"Cluster mode is HA but online storage nodes are less than 3")
     #     if force is False:
     #         return False
 
     logger.info("Shutting down node")
+    old_status = snode.status
     snode.status = StorageNode.STATUS_IN_SHUTDOWN
     snode.write_to_db(db_controller.kv_store)
+    storage_events.snode_status_change(snode, snode.status, old_status)
 
     logger.debug("Setting LVols to offline")
     for lvol_id in snode.lvols:
         logger.debug(lvol_id)
         lvol = db_controller.get_lvol_by_id(lvol_id)
         if lvol:
             lvol.status = lvol.STATUS_OFFLINE
             lvol.write_to_db(db_controller.kv_store)
 
     distr_controller.send_node_status_event(snode.get_id(), "in_shutdown")
     for dev in snode.nvme_devices:
-        dev.status = 'unavailable'
-        distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
+        if dev.status == NVMeDevice.STATUS_ONLINE:
+            device_controller.device_set_unavailable(dev.get_id())
 
     # shutdown node
     # make other nodes disconnect from this node
     logger.info("disconnect all other nodes connections to this node")
     for dev in snode.nvme_devices:
         distr_controller.disconnect_device(dev)
 
@@ -1083,14 +1132,15 @@
     logger.info("Stopping SPDK")
     snode_api = SNodeClient(snode.api_endpoint)
     results, err = snode_api.spdk_process_kill()
 
     distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_OFFLINE)
 
     logger.info("Setting node status to offline")
+    snode = db_controller.get_storage_node_by_id(node_id)
     old_status = snode.status
     snode.status = StorageNode.STATUS_OFFLINE
     snode.write_to_db(db_controller.kv_store)
 
     # send event log
     storage_events.snode_status_change(snode, snode.status, old_status)
     logger.info("Done")
@@ -1105,34 +1155,34 @@
         return False
 
     logger.info("Node found: %s in state: %s", snode.hostname, snode.status)
     if snode.status != StorageNode.STATUS_ONLINE:
         logger.error("Node is not in online state")
         return False
 
-    cls = db_controller.get_clusters(id=snode.cluster_id)
+    cluster = db_controller.get_cluster_by_id(snode.cluster_id)
     snodes = db_controller.get_storage_nodes()
     online_nodes = 0
     for node in snodes:
         if node.status == node.STATUS_ONLINE:
             online_nodes += 1
-    if cls[0].ha_type == "ha" and online_nodes <= 3 and cls[0].status == cls[0].STATUS_ACTIVE:
+    if cluster.ha_type == "ha" and online_nodes <= 3 and cluster.status == cluster.STATUS_ACTIVE:
         logger.warning(f"Cluster mode is HA but online storage nodes are less than 3")
         if force is False:
             return False
 
-    if cls[0].ha_type == "ha" and cls[0].status == cls[0].STATUS_DEGRADED and force is False:
+    if cluster.ha_type == "ha" and cluster.status == cluster.STATUS_DEGRADED and force is False:
         logger.warning(f"Cluster status is degraded, use --force but this will suspend the cluster")
         return False
 
     logger.info("Suspending node")
     distr_controller.send_node_status_event(snode.get_id(), "suspended")
     for dev in snode.nvme_devices:
-        dev.status = 'unavailable'
-        distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
+        if dev.status == NVMeDevice.STATUS_ONLINE:
+            device_controller.device_set_unavailable(dev.get_id())
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     logger.debug("Setting LVols to offline")
     for lvol_id in snode.lvols:
@@ -1140,43 +1190,44 @@
         lvol = db_controller.get_lvol_by_id(lvol_id)
         if lvol:
             ret = rpc_client.nvmf_subsystem_remove_ns(lvol.nqn, 1)
             lvol.status = lvol.STATUS_OFFLINE
             lvol.write_to_db(db_controller.kv_store)
 
     logger.info("Setting node status to suspended")
+    snode = db_controller.get_storage_node_by_id(node_id)
     old_status = snode.status
     snode.status = StorageNode.STATUS_SUSPENDED
     snode.write_to_db(db_controller.kv_store)
 
     storage_events.snode_status_change(snode, snode.status, old_status)
     logger.info("Done")
     return True
 
 
 def resume_storage_node(node_id):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error("This storage node is not part of the cluster")
-        exit(1)
+        return False
 
     logger.info("Node found: %s in state: %s", snode.hostname, snode.status)
     if snode.status != StorageNode.STATUS_SUSPENDED:
         logger.error("Node is not in suspended state")
-        exit(1)
+        return False
 
     logger.info("Resuming node")
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
-        dev.status = 'online'
-        distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
+        if dev.status == NVMeDevice.STATUS_UNAVAILABLE:
+            device_controller.device_set_online(dev.get_id())
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     logger.debug("Setting LVols to online")
     for lvol_id in snode.lvols:
@@ -1184,44 +1235,24 @@
         lvol = db_controller.get_lvol_by_id(lvol_id)
         if lvol:
             ret = rpc_client.nvmf_subsystem_add_ns(lvol.nqn, lvol.top_bdev, lvol.uuid, lvol.guid)
             lvol.status = lvol.STATUS_ONLINE
             lvol.write_to_db(db_controller.kv_store)
 
     logger.info("Setting node status to online")
+    snode = db_controller.get_storage_node_by_id(node_id)
     old_status = snode.status
     snode.status = StorageNode.STATUS_ONLINE
     snode.write_to_db(db_controller.kv_store)
 
     storage_events.snode_status_change(snode, snode.status, old_status)
     logger.info("Done")
     return True
 
 
-def reset_storage_device(dev_id):
-    db_controller = DBController()
-    device = db_controller.get_storage_devices(dev_id)
-    if not device:
-        logger.error("device not found")
-        return False
-
-    snode = db_controller.get_storage_node_by_id(device.node_id)
-    if not snode:
-        logger.error("node not found")
-        return False
-
-    logger.info("Resetting device")
-
-    rpc_client = RPCClient(
-        snode.mgmt_ip, snode.rpc_port,
-        snode.rpc_username, snode.rpc_password)
-
-    response = rpc_client.reset_device(device.nvme_bdev[:-2])
-    return response
-
 
 def run_test_storage_device(kv_store, dev_name):
     db_controller = DBController(kv_store)
     baseboard_sn = utils.get_baseboard_sn()
     snode = db_controller.get_storage_node_by_id(baseboard_sn)
     if not snode:
         logger.error("This storage node is not part of the cluster")
@@ -1268,19 +1299,18 @@
     logger.info("Done")
 
 
 # Deprecated
 def add_storage_device(dev_name, node_id, cluster_id):
     db_controller = DBController()
     kv_store = db_controller.kv_store
-    clusters = db_controller.get_clusters(cluster_id)
-    if not clusters:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
-    cluster = clusters[0]
 
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error("Node is not part of the cluster: %s", node_id)
         exit(1)
 
     for node_nvme_device in snode.nvme_devices:
@@ -1383,89 +1413,14 @@
     return True
 
 
 def replace_node(kv_store, old_node_name, iface_name):
     return "Not implemented!"
 
 
-def get_device(device_id):
-    db_controller = DBController()
-    device = db_controller.get_storage_devices(device_id)
-    if not device:
-        logger.error("device not found")
-        return False
-    out = [device.get_clean_dict()]
-    return utils.print_table(out)
-
-
-def get_device_capacity(device_id, history, records_count=20, parse_sizes=True):
-    db_controller = DBController()
-    device = db_controller.get_storage_devices(device_id)
-    if not device:
-        logger.error("device not found")
-
-    if history:
-        records_number = utils.parse_history_param(history)
-        if not records_number:
-            return False
-    else:
-        records_number = 20
-
-    records = db_controller.get_device_capacity(device, records_number)
-    records_list = utils.process_records(records, records_count)
-
-    if not parse_sizes:
-        return records_list
-
-    out = []
-    for record in records_list:
-        out.append({
-            "Date": time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(record['date'])),
-            "Absolut": utils.humanbytes(record['size_total']),
-            "Used": utils.humanbytes(record['size_used']),
-            "Free": utils.humanbytes(record['size_free']),
-            "Util %": f"{record['size_util']}%",
-        })
-    return out
-
-
-def get_device_iostats(device_id, history, records_count=20, parse_sizes=True):
-    db_controller = DBController()
-    device = db_controller.get_storage_devices(device_id)
-    if not device:
-        logger.error(f"Device not found: {device_id}")
-        return False
-
-    if history:
-        records_number = utils.parse_history_param(history)
-        if not records_number:
-            logger.error(f"Error parsing history string: {history}")
-            return False
-    else:
-        records_number = 20
-
-    records_list = db_controller.get_device_stats(device, records_number)
-    new_records = utils.process_records(records_list, records_count)
-
-    if not parse_sizes:
-        return new_records
-
-    out = []
-    for record in new_records:
-        out.append({
-            "Date": time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(record['date'])),
-            "Read speed": utils.humanbytes(record['read_bytes_ps']),
-            "Read IOPS": record["read_io_ps"],
-            "Read lat": record["read_latency_ps"],
-            "Write speed": utils.humanbytes(record["write_bytes_ps"]),
-            "Write IOPS": record["write_io_ps"],
-            "Write lat": record["write_latency_ps"],
-        })
-    return out
-
 
 def get_node_capacity(node_id, history, records_count=20, parse_sizes=True):
     db_controller = DBController()
     this_node = db_controller.get_storage_node_by_id(node_id)
     if not this_node:
         logger.error("Storage node Not found")
         return
@@ -1631,218 +1586,19 @@
     logger.debug(constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE)
     logger.debug(constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE)
     node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE)
     node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE)
     return f"{dev_ip}:5000"
 
 
-def device_set_unavailable(device_id):
-    db_controller = DBController()
-    dev = db_controller.get_storage_devices(device_id)
-    if not dev:
-        logger.error("device not found")
-
-    snode = db_controller.get_storage_node_by_id(dev.node_id)
-    if not snode:
-        logger.error("node not found")
-        return False
-
-    for dev in snode.nvme_devices:
-        if dev.get_id() == device_id:
-            device = dev
-            break
-
-    device.status = 'unavailable'
-    distr_controller.send_dev_status_event(device.cluster_device_order, "unavailable")
-    snode.write_to_db(db_controller.kv_store)
-    return True
-
-
-def device_remove(device_id):
-    db_controller = DBController()
-    dev = db_controller.get_storage_devices(device_id)
-    if not dev:
-        logger.error("device not found")
-
-    snode = db_controller.get_storage_node_by_id(dev.node_id)
-    if not snode:
-        logger.error("node not found")
-        return False
-
-    for dev in snode.nvme_devices:
-        if dev.get_id() == device_id:
-            device = dev
-            break
-
-    # 1- send events
-    # 2- make other nodes disconnect
-    # 3- remove nvmeof
-    # 4- remove pt, alceml, test
-
-    logger.info("Sending device event")
-    distr_controller.send_dev_status_event(device.cluster_device_order, "removed")
-
-    logger.info("Disconnecting device from all nodes")
-    distr_controller.disconnect_device(device)
-
-    logger.info("Removing device fabric")
-    rpc_client = RPCClient(
-        snode.mgmt_ip, snode.rpc_port,
-        snode.rpc_username, snode.rpc_password)
-    ret = rpc_client.subsystem_delete(device.nvmf_nqn)
-
-    logger.info("Removing device bdevs")
-    ret = rpc_client.bdev_PT_NoExcl_delete(f"{device.alceml_bdev}_PT")
-    ret = rpc_client.bdev_alceml_delete(device.alceml_bdev)
-    ret = rpc_client.bdev_passtest_delete(device.testing_bdev)
-
-    device.status = 'removed'
-    snode.write_to_db(db_controller.kv_store)
-
-    for lvol in db_controller.get_lvols():
-        lvol_controller.send_cluster_map(lvol.get_id())
-
-    return True
-
-
-def set_device_testing_mode(device_id, mode):
-    db_controller = DBController()
-    device = db_controller.get_storage_devices(device_id)
-    if not device:
-        logger.error("device not found")
-
-    snode = db_controller.get_storage_node_by_id(device.node_id)
-    if not snode:
-        logger.error("node not found")
-        return False
-
-    logger.info(f"Set device:{device_id} Test mode:{mode}")
-    # creating RPCClient instance
-    rpc_client = RPCClient(
-        snode.mgmt_ip, snode.rpc_port,
-        snode.rpc_username, snode.rpc_password)
-
-    ret = rpc_client.bdev_passtest_mode(device.testing_bdev, mode)
-    return ret
-
-
 def deploy_cleaner():
     scripts.deploy_cleaner()
     return True
 
 
-def restart_device(device_id):
-    db_controller = DBController()
-    dev = db_controller.get_storage_devices(device_id)
-    if not dev:
-        logger.error("device not found")
-
-    snode = db_controller.get_storage_node_by_id(dev.node_id)
-    if not snode:
-        logger.error("node not found")
-        return False
-
-    device_obj = None
-    for dev in snode.nvme_devices:
-        if dev.get_id() == device_id:
-            device_obj = dev
-            break
-
-    device_obj.status = 'restarting'
-    snode.write_to_db(db_controller.kv_store)
-
-    logger.info(f"Restarting device {device_id}")
-
-    rpc_client = RPCClient(
-        snode.mgmt_ip, snode.rpc_port,
-        snode.rpc_username, snode.rpc_password)
-
-    test_name = f"{device_obj.nvme_bdev}_test"
-    # create testing bdev
-    ret = rpc_client.bdev_passtest_create(test_name, device_obj.nvme_bdev)
-
-    alceml_id = device_obj.get_id()
-    node_id_mini = snode.get_id().split("-")[-1]
-    alceml_id_mini = alceml_id.split("-")[-1]
-    alceml_name = f"node_{node_id_mini}_dev_{alceml_id_mini}"
-    logger.info(f"adding {alceml_name}")
-    ret = rpc_client.bdev_alceml_create(alceml_name, test_name, alceml_id)
-    if not ret:
-        logger.error(f"Failed to create alceml bdev: {alceml_name}")
-
-    # add pass through
-    pt_name = f"{alceml_name}_PT"
-    ret = rpc_client.bdev_PT_NoExcl_create(pt_name, alceml_name)
-    if not ret:
-        logger.error(f"Failed to create pt noexcl bdev: {pt_name}")
-
-    subsystem_nqn = snode.subsystem + ":dev:" + alceml_id
-    logger.info("Creating subsystem %s", subsystem_nqn)
-    ret = rpc_client.subsystem_create(subsystem_nqn, 'sbcli-cn', alceml_id)
-    IP = None
-    for iface in snode.data_nics:
-        if iface.ip4_address:
-            tr_type = iface.get_transport_type()
-            ret = rpc_client.transport_list()
-            found = False
-            if ret:
-                for ty in ret:
-                    if ty['trtype'] == tr_type:
-                        found = True
-            if found is False:
-                ret = rpc_client.transport_create(tr_type)
-            # logger.info("adding listener for %s on IP %s" % (subsystem_nqn, iface.ip4_address))
-            ret = rpc_client.listeners_create(subsystem_nqn, tr_type, iface.ip4_address, "4420")
-            IP = iface.ip4_address
-            break
-    logger.info(f"Adding {pt_name} to the subsystem")
-    ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, pt_name)
-
-    device_obj.testing_bdev = test_name
-    device_obj.alceml_bdev = alceml_name
-    device_obj.pt_bdev = pt_name
-    device_obj.nvmf_nqn = subsystem_nqn
-    device_obj.nvmf_ip = IP
-    device_obj.nvmf_port = 4420
-    device_obj.status = NVMeDevice.STATUS_ONLINE
-    snode.write_to_db(db_controller.kv_store)
-
-    logger.info("Make other nodes connect to the device")
-    snodes = db_controller.get_storage_nodes()
-    for node_index, node in enumerate(snodes):
-        if node.get_id() == snode.get_id():
-            continue
-        if node.status != snode.STATUS_ONLINE:
-            continue
-
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        name = f"remote_{device_obj.alceml_bdev}"
-        ret = rpc_client.bdev_nvme_attach_controller_tcp(name, device_obj.nvmf_nqn, device_obj.nvmf_ip,
-                                                         device_obj.nvmf_port)
-        if not ret:
-            logger.error(f"Failed to connect to device: {name}")
-            continue
-
-        device_obj.remote_bdev = f"{name}n1"
-        idx = -1
-        for i, d in enumerate(node.remote_devices):
-            if d.get_id() == device_obj.get_id():
-                idx = i
-                break
-        if idx >= 0:
-            node.remote_devices[idx] = device_obj
-        else:
-            node.remote_devices.append(device_obj)
-        node.write_to_db(db_controller.kv_store)
-
-    logger.info("Sending device event")
-    distr_controller.send_dev_status_event(device_obj.cluster_device_order, "online")
-
-    return "Done"
-
 
 def get_host_secret(node_id):
     db_controller = DBController()
     node = db_controller.get_storage_node_by_id(node_id)
     if not node:
         logger.error("node not found")
         return False
@@ -1954,27 +1710,57 @@
         return False
 
     snode_api = SNodeClient(f"{snode.mgmt_ip}:5000")
     node_info, _ = snode_api.info()
     return json.dumps(node_info, indent=2)
 
 
-def device_set_read_only(device_id):
+def get_spdk_info(node_id):
     db_controller = DBController()
-    dev = db_controller.get_storage_devices(device_id)
-    if not dev:
-        logger.error("device not found")
 
-    snode = db_controller.get_storage_node_by_id(dev.node_id)
+    snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
-        logger.error("node not found")
+        logger.error(f"Can not find storage node: {node_id}")
         return False
 
-    for dev in snode.nvme_devices:
-        if dev.get_id() == device_id:
-            device = dev
-            break
+    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+    ret = rpc_client.ultra21_util_get_malloc_stats()
+    if not ret:
+        logger.error(f"Failed to get SPDK info for node {node_id}")
+        return False
+    data = []
+    for key in ret.keys():
+        data.append({
+            "Key": key,
+            "Value": ret[key],
+            "Parsed": utils.humanbytes(ret[key])
+        })
+    return utils.print_table(data)
 
-    device.status = device.STATUS_READONLY
-    distr_controller.send_dev_status_event(device.cluster_device_order, device.status)
-    snode.write_to_db(db_controller.kv_store)
-    return True
+
+def update(node_id, key, value):
+    db_controller = DBController()
+
+    snode = db_controller.get_storage_node_by_id(node_id)
+    if not snode:
+        logger.error(f"Can not find storage node: {node_id}")
+        return False
+
+    if key in snode._attribute_map:
+        setattr(snode, key, value)
+        snode.write_to_db(db_controller.kv_store)
+        return True
+    else:
+        logger.error("Key not found")
+        return False
+
+
+def get(node_id):
+    db_controller = DBController()
+
+    snode = db_controller.get_storage_node_by_id(node_id)
+    if not snode:
+        logger.error(f"Can not find storage node: {node_id}")
+        return False
+
+    data = snode.get_clean_dict()
+    return json.dumps(data, indent=2)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/mgmt_node_ops.py` & `sbcli-release-1.0.5/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/cluster_ops.py` & `sbcli-release-1.0.5/simplyblock_core/cluster_ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 import os
 import time
 import uuid
 
 import docker
 import requests
 
-from simplyblock_core import utils, scripts, constants, mgmt_node_ops, storage_node_ops
-from simplyblock_core.controllers import cluster_events
+from simplyblock_core import utils, scripts, constants, mgmt_node_ops, storage_node_ops, shell_utils
+from simplyblock_core.controllers import cluster_events, device_controller
 from simplyblock_core.kv_store import DBController
 from simplyblock_core.models.cluster import Cluster
+from simplyblock_core.models.nvme_device import NVMeDevice
+from simplyblock_core.models.storage_node import StorageNode
 
 logger = logging.getLogger()
 
 
 def _add_graylog_input(cluster_ip, password):
     url = f"http://{cluster_ip}:9000/api/system/inputs"
     payload = json.dumps({
@@ -39,15 +41,14 @@
     }
     session = requests.session()
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
-
 def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
                    auth_hosts_only, cli_pass, model_ids,
                    cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
 
@@ -102,15 +103,15 @@
         c.cap_crit = cap_crit
     if prov_cap_warn and prov_cap_warn > 0:
         c.prov_cap_warn = prov_cap_warn
     if prov_cap_crit and prov_cap_crit > 0:
         c.prov_cap_crit = prov_cap_crit
 
     logger.info("Deploying swarm stack ...")
-    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret)
+    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid)
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
 
     _add_graylog_input(DEV_IP, c.secret)
@@ -121,14 +122,18 @@
     c.updated_at = int(time.time())
     c.write_to_db(db_controller.kv_store)
 
     cluster_events.cluster_create(c)
 
     mgmt_node_ops.add_mgmt_node(DEV_IP, c.uuid)
 
+    logger.info("Applying dashboard...")
+    ret = scripts.apply_dashboard(c.secret)
+    logger.info("Applying dashboard > Done")
+
     logger.info("New Cluster has been created")
     logger.info(c.uuid)
     return c.uuid
 
 
 # Deprecated
 def deploy_spdk(node_docker, spdk_cpu_mask, spdk_mem):
@@ -268,15 +273,15 @@
         time.sleep(5)
 
     except Exception as e:
         raise e
 
     if role == 'management':
         mgmt_node_ops.add_mgmt_node(DEV_IP, cluster_id)
-        cluster_obj = db_controller.get_clusters(cluster_id)[0]
+        cluster_obj = db_controller.get_cluster_by_id(cluster_id)
         nodes = db_controller.get_mgmt_nodes(cluster_id=cluster_id)
         if len(nodes) >= 3:
             logger.info("Waiting for FDB container to be active...")
             fdb_cont = None
             retries = 30
             while retries > 0 and fdb_cont is None:
                 logger.info("Looking for FDB container...")
@@ -374,81 +379,106 @@
     c.write_to_db(db_controller.kv_store)
     logger.info("New Cluster has been created")
     logger.info(c.uuid)
 
 
 def show_cluster(cl_id, is_json=False):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cl_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
         logger.error(f"Cluster not found {cl_id}")
         return False
 
-    cluster = cls[0]
     st = db_controller.get_storage_nodes()
     data = []
     for node in st:
         for dev in node.nvme_devices:
             data.append({
                 "UUID": dev.get_id(),
                 "Storage ID": dev.cluster_device_order,
                 "Size": utils.humanbytes(dev.size),
                 "Hostname": node.hostname,
-                "Status": dev.status
+                "Status": dev.status,
+                "IO Error": dev.io_error,
+                "Health": dev.health_check
             })
     data = sorted(data, key=lambda x: x["Storage ID"])
     if is_json:
         return json.dumps(data, indent=2)
     else:
         return utils.print_table(data)
 
 
-def suspend_cluster(cl_id):
+def set_cluster_status(cl_id, status):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cl_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
         logger.error(f"Cluster not found {cl_id}")
         return False
-    cl = cls[0]
-    old_status = cl.status
-    cl.status = Cluster.STATUS_SUSPENDED
-    cl.write_to_db(db_controller.kv_store)
 
-    cluster_events.cluster_status_change(cl, cl.status, old_status)
-    return "Done"
+    if cluster.status == status:
+        return True
+
+    old_status = cluster.status
+    cluster.status = status
+    cluster.write_to_db(db_controller.kv_store)
+    cluster_events.cluster_status_change(cluster, cluster.status, old_status)
+    return True
+
+
+def suspend_cluster(cl_id):
+    return set_cluster_status(cl_id, Cluster.STATUS_SUSPENDED)
 
 
 def unsuspend_cluster(cl_id):
+    return set_cluster_status(cl_id, Cluster.STATUS_ACTIVE)
+
+
+def degrade_cluster(cl_id):
+    return set_cluster_status(cl_id, Cluster.STATUS_DEGRADED)
+
+
+def cluster_set_read_only(cl_id):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cl_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
         logger.error(f"Cluster not found {cl_id}")
         return False
-    cl = cls[0]
-    old_status = cl.status
-    cl.status = Cluster.STATUS_ACTIVE
-    cl.write_to_db(db_controller.kv_store)
 
-    cluster_events.cluster_status_change(cl, cl.status, old_status)
-    return "Done"
+    if cluster.status == Cluster.STATUS_READONLY:
+        return True
 
+    ret = set_cluster_status(cl_id, Cluster.STATUS_READONLY)
+    if ret:
+        st = db_controller.get_storage_nodes()
+        for node in st:
+            for dev in node.nvme_devices:
+                if dev.status == NVMeDevice.STATUS_ONLINE:
+                    device_controller.device_set_read_only(dev.get_id())
+    return True
 
-def degrade_cluster(cl_id):
+
+def cluster_set_active(cl_id):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cl_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
         logger.error(f"Cluster not found {cl_id}")
         return False
-    cl = cls[0]
-    old_status = cl.status
-    cl.status = Cluster.STATUS_DEGRADED
-    cl.write_to_db(db_controller.kv_store)
 
-    cluster_events.cluster_status_change(cl, cl.status, old_status)
-    return "Done"
+    if cluster.status == Cluster.STATUS_ACTIVE:
+        return True
+
+    ret = set_cluster_status(cl_id, Cluster.STATUS_ACTIVE)
+    if ret:
+        st = db_controller.get_storage_nodes()
+        for node in st:
+            for dev in node.nvme_devices:
+                if dev.status == NVMeDevice.STATUS_READONLY:
+                    device_controller.device_set_online(dev.get_id())
+    return True
 
 
 def list():
     db_controller = DBController()
     cls = db_controller.get_clusters()
     st = db_controller.get_storage_nodes()
     mt = db_controller.get_mgmt_nodes()
@@ -463,36 +493,35 @@
             "mgmt nodes": len(mt),
             "storage nodes": len(st),
             "Status": cl.status,
         })
     return utils.print_table(data)
 
 
-def get_capacity(cluster_id, history, records_count=20, parse_sizes=True):
+def get_capacity(cluster_id, history, records_count=20, is_json=False):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cluster_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
-    cl = cls[0]
 
     if history:
         records_number = utils.parse_history_param(history)
         if not records_number:
             logger.error(f"Error parsing history string: {history}")
             return False
     else:
         records_number = 20
 
-    records = db_controller.get_cluster_capacity(cl, records_number)
+    records = db_controller.get_cluster_capacity(cluster, records_number)
 
     new_records = utils.process_records(records, records_count)
 
-    if not parse_sizes:
-        return new_records
+    if is_json:
+        return json.dumps(new_records, indent=2)
 
     out = []
     for record in new_records:
         out.append({
             "Date": time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(record['date'])),
             "Absolut": utils.humanbytes(record['size_total']),
             "Provisioned": utils.humanbytes(record['size_prov']),
@@ -502,34 +531,33 @@
             "Prov Util %": f"{record['size_prov_util']}%",
         })
     return out
 
 
 def get_iostats_history(cluster_id, history_string, records_count=20, parse_sizes=True):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cluster_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
-    cl = cls[0]
 
     nodes = db_controller.get_storage_nodes_by_cluster_id(cluster_id)
     if not nodes:
         logger.error("no nodes found")
         return False
 
     if history_string:
         records_number = utils.parse_history_param(history_string)
         if not records_number:
             logger.error(f"Error parsing history string: {history_string}")
             return False
     else:
         records_number = 20
 
-    records = db_controller.get_cluster_stats(cl, records_number)
+    records = db_controller.get_cluster_stats(cluster, records_number)
 
     # combine records
     new_records = utils.process_records(records, records_count)
 
     if not parse_sizes:
         return new_records
 
@@ -545,56 +573,52 @@
             "Write lat": record["write_latency_ps"],
         })
     return out
 
 
 def get_ssh_pass(cluster_id):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cluster_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
-    cl = cls[0]
-    return cl.cli_pass
+    return cluster.cli_pass
 
 
 def get_secret(cluster_id):
     db_controller = DBController()
-    cls = db_controller.get_clusters(id=cluster_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
-    cl = cls[0]
-    return cl.secret
+    return cluster.secret
 
 
 def set_secret(cluster_id, secret):
     db_controller = DBController()
-    cls = db_controller.get_clusters(cluster_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
-    cl = cls[0]
 
     secret = secret.strip()
     if len(secret) < 20:
         return "Secret must be at least 20 char"
 
-    cl.secret = secret
-    cl.write_to_db(db_controller.kv_store)
+    cluster.secret = secret
+    cluster.write_to_db(db_controller.kv_store)
     return "Done"
 
 
 def get_logs(cluster_id, is_json=False):
     db_controller = DBController()
-    cls = db_controller.get_clusters(cluster_id)
-    if not cls:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
-    cl = cls[0]
 
     events = db_controller.get_events(cluster_id)
     out = []
     for record in events:
         logger.debug(record)
         Storage_ID = None
         if 'storage_ID' in record.object_dict:
@@ -614,7 +638,58 @@
             "VUID": str(vuid),
             "Status": record.status,
         })
     if is_json:
         return json.dumps(out, indent=2)
     else:
         return utils.print_table(out)
+
+
+def get_cluster(cl_id):
+    db_controller = DBController()
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
+        logger.error(f"Cluster not found {cl_id}")
+        return False
+
+    return json.dumps(cluster.get_clean_dict(), indent=2)
+
+
+def update_cluster(cl_id):
+    db_controller = DBController()
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
+        logger.error(f"Cluster not found {cl_id}")
+        return False
+
+    try:
+        out, _, ret_code = shell_utils.run_command("pip install sbcli-dev --upgrade")
+        if ret_code == 0:
+            logger.info("sbcli-dev is upgraded")
+    except Exception as e:
+        logger.error(e)
+
+    try:
+        logger.info("Updating mgmt cluster")
+        cluster_docker = utils.get_docker_client(cl_id)
+        logger.info(f"Pulling image {constants.SIMPLY_BLOCK_DOCKER_IMAGE}")
+        cluster_docker.images.pull(constants.SIMPLY_BLOCK_DOCKER_IMAGE)
+        for service in cluster_docker.services.list():
+            if service.attrs['Spec']['Labels']['com.docker.stack.image'] == constants.SIMPLY_BLOCK_DOCKER_IMAGE:
+                logger.info(f"Updating service {service.name}")
+                service.update(image=constants.SIMPLY_BLOCK_DOCKER_IMAGE, force_update=True)
+        logger.info("Done")
+    except Exception as e:
+        print(e)
+
+    for node in db_controller.get_storage_nodes():
+        node_docker = docker.DockerClient(base_url=f"tcp://{node.mgmt_ip}:2375", version="auto")
+        logger.info(f"Pulling image {constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE}")
+        node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE)
+        if node.status == StorageNode.STATUS_ONLINE:
+            storage_node_ops.shutdown_storage_node(node.get_id(), force=True)
+            time.sleep(3)
+        storage_node_ops.restart_storage_node(node.get_id())
+
+    logger.info("Done")
+    return True
+
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/kv_store.py` & `sbcli-release-1.0.5/simplyblock_core/kv_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,16 +225,21 @@
         return stats
 
     def get_device_capacity(self, device, limit=1):
         stats = DeviceStatObject().read_from_db(
             self.kv_store, id="%s/%s" % (device.cluster_id, device.get_id()), limit=limit, reverse=True)
         return stats
 
-    def get_clusters(self, id=""):
-        return Cluster().read_from_db(self.kv_store, id=id)
+    def get_clusters(self):
+        return Cluster().read_from_db(self.kv_store)
+
+    def get_cluster_by_id(self, cluster_id):
+        ret = Cluster().read_from_db(self.kv_store, id=cluster_id)
+        if ret:
+            return ret[0]
 
     def get_port_stats(self, node_id, port_id, limit=20):
         stats = PortStat().read_from_db(self.kv_store, id="%s/%s" % (node_id, port_id), limit=limit, reverse=True)
         return stats
 
     def get_events(self, event_id=""):
         return EventObj().read_from_db(self.kv_store, id=event_id)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/pool.py` & `sbcli-release-1.0.5/simplyblock_core/models/pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     STATUS_ACTIVE = "active"
     STATUS_INACTIVE = "inactive"
 
     attributes = {
         "pool_name": {"type": str, 'default': ""},
         "id": {"type": str, 'default': ""},
+        "cluster_id": {"type": str, 'default': ""},
         "users": {"type": List[str], 'default': []},
         "groups": {"type": List[str], 'default': []},
         "pool_max_size": {"type": int, 'default': 0},
         "lvol_max_size": {"type": int, 'default': 0},
         "lvols": {"type": List[str], 'default': []},
         "status": {"type": str, 'default': ""},
         "secret": {"type": str, 'default': ""},
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/iface.py` & `sbcli-release-1.0.5/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/compute_node.py` & `sbcli-release-1.0.5/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/storage_node.py` & `sbcli-release-1.0.5/simplyblock_core/models/caching_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,40 @@
 # coding=utf-8
 
 from datetime import datetime
 from typing import List
 
 from simplyblock_core.models.base_model import BaseModel
 from simplyblock_core.models.iface import IFace
+from simplyblock_core.models.lvol_model import LVol
 from simplyblock_core.models.nvme_device import NVMeDevice
 
 
-class StorageNode(BaseModel):
+class CachedLVol(BaseModel):
+
+    attributes = {
+        "uuid": {"type": str, 'default': ""},
+        "lvol_id": {"type": str, 'default': ""},
+        "lvol": {"type": LVol, 'default': None},
+        "hostname": {"type": str, 'default': ""},
+        "local_nqn": {"type": str, 'default': ""},
+        "ocf_bdev": {"type": str, 'default': ""},
+        "device_path": {"type": str, 'default': ""},
+    }
+
+    def __init__(self, data=None):
+        super(CachedLVol, self).__init__()
+        self.set_attrs(self.attributes, data)
+        self.object_type = "object"
+
+    def get_id(self):
+        return self.uuid
+
+
+class CachingNode(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
     STATUS_SUSPENDED = 'suspended'
     STATUS_IN_CREATION = 'in_creation'
     STATUS_IN_SHUTDOWN = 'in_shutdown'
     STATUS_RESTARTING = 'restarting'
@@ -48,38 +70,35 @@
         "create_dt": {"type": str, 'default': str(datetime.now())},
         "remove_dt": {"type": str, 'default': str(datetime.now())},
         "mgmt_ip": {"type": str, 'default': ""},
         "rpc_port": {"type": int, 'default': -1},
         "rpc_username": {"type": str, 'default': ""},
         "rpc_password": {"type": str, 'default': ""},
         "data_nics": {"type": List[IFace], 'default': []},
-        "lvols": {"type": List[str], 'default': []},
+        "lvols": {"type": List[CachedLVol], 'default': []},
         "node_lvs": {"type": str, 'default': "lvs"},
         "services": {"type": List[str], 'default': []},
         "cluster_id": {"type": str, 'default': ""},
         "api_endpoint": {"type": str, 'default': ""},
         "remote_devices": {"type": List[NVMeDevice], 'default': []},
         "host_secret": {"type": str, "default": ""},
         "ctrl_secret": {"type": str, "default": ""},
 
+        "cache_bdev": {"type": str, "default": ""},
+        "cache_size": {"type": int, "default": 0},
+        "cache_split_factor": {"type": int, "default": 0},
         "cpu": {"type": int, "default": 0},
         "cpu_hz": {"type": int, "default": 0},
         "memory": {"type": int, "default": 0},
         "hugepages": {"type": int, "default": 0},
-        "health_check": {"type": bool, "default": True},
 
-        # spdk params
-        "spdk_cpu_mask": {"type": str, "default": ""},
-        "spdk_mem": {"type": int, "default": 0},
-        "spdk_image": {"type": str, "default": ""},
-        "cmd_params": {"type": List, "default": []},
     }
 
     def __init__(self, data=None):
-        super(StorageNode, self).__init__()
+        super(CachingNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
 
     def get_id(self):
         return self.uuid
 
     def get_status_code(self):
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/base_model.py` & `sbcli-release-1.0.5/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/global_settings.py` & `sbcli-release-1.0.5/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/stats.py` & `sbcli-release-1.0.5/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/nvme_device.py` & `sbcli-release-1.0.5/simplyblock_core/models/nvme_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # coding=utf-8
+from typing import List
 
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_AVAILABLE = 'available'
     STATUS_UNAVAILABLE = 'unavailable'
-    STATUS_READONLY = 'read-only'
+    STATUS_READONLY = 'read_only'
     STATUS_OVERLOADED = 'overloaded'
     STATUS_FAILED = 'failed'
     STATUS_REMOVED = 'removed'
     STATUS_RESETTING = 'resetting'
     STATUS_UNRECOGNIZED = 'unrecognized'
 
     attributes = {
@@ -33,18 +34,23 @@
         "node_id": {"type": str, 'default': ""},
         "pt_bdev": {"type": str, 'default': ""},
         "nvmf_nqn": {"type": str, 'default': ""},
         "nvmf_ip": {"type": str, 'default': ""},
         "nvmf_port": {"type": int, 'default': 0},
         "remote_bdev": {"type": str, 'default': ""},
         "testing_bdev": {"type": str, 'default': ""},
+        "jm_bdev": {"type": str, 'default': ""},
         "cluster_device_order": {"type": int, 'default': 0},
         "health_check": {"type": bool, "default": True},
         "cluster_id": {"type": str, 'default': ""},
 
+        "bdev_stack": {"type": List, 'default': []},
+
+        "io_error": {"type": bool, 'default': False},
+
     }
 
     def __init__(self, data=None):
         super(NVMeDevice, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/port_stat.py` & `sbcli-release-1.0.5/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/events.py` & `sbcli-release-1.0.5/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/cluster.py` & `sbcli-release-1.0.5/simplyblock_core/models/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from simplyblock_core.models.base_model import BaseModel
 from simplyblock_core.models.storage_node import StorageNode
 
 
 class Cluster(BaseModel):
 
     STATUS_ACTIVE = "active"
+    STATUS_READONLY = 'read_only'
     STATUS_INACTIVE = "inactive"
     STATUS_SUSPENDED = "suspended"
     STATUS_DEGRADED = "degraded"
 
     STATUS_CODE_MAP = {
         STATUS_ACTIVE: 0,
         STATUS_INACTIVE: 1,
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/caching_node.py` & `sbcli-release-1.0.5/simplyblock_core/models/storage_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,18 @@
 # coding=utf-8
 
 from datetime import datetime
 from typing import List
 
 from simplyblock_core.models.base_model import BaseModel
 from simplyblock_core.models.iface import IFace
-from simplyblock_core.models.lvol_model import LVol
 from simplyblock_core.models.nvme_device import NVMeDevice
 
 
-class CachedLVol(BaseModel):
-
-    attributes = {
-        "uuid": {"type": str, 'default': ""},
-        "lvol_id": {"type": str, 'default': ""},
-        "lvol": {"type": LVol, 'default': None},
-        "hostname": {"type": str, 'default': ""},
-        "local_nqn": {"type": str, 'default': ""},
-        "ocf_bdev": {"type": str, 'default': ""},
-        "device_path": {"type": str, 'default': ""},
-    }
-
-    def __init__(self, data=None):
-        super(CachedLVol, self).__init__()
-        self.set_attrs(self.attributes, data)
-        self.object_type = "object"
-
-    def get_id(self):
-        return self.uuid
-
-
-class CachingNode(BaseModel):
+class StorageNode(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
     STATUS_SUSPENDED = 'suspended'
     STATUS_IN_CREATION = 'in_creation'
     STATUS_IN_SHUTDOWN = 'in_shutdown'
     STATUS_RESTARTING = 'restarting'
@@ -70,34 +48,38 @@
         "create_dt": {"type": str, 'default': str(datetime.now())},
         "remove_dt": {"type": str, 'default': str(datetime.now())},
         "mgmt_ip": {"type": str, 'default': ""},
         "rpc_port": {"type": int, 'default': -1},
         "rpc_username": {"type": str, 'default': ""},
         "rpc_password": {"type": str, 'default': ""},
         "data_nics": {"type": List[IFace], 'default': []},
-        "lvols": {"type": List[CachedLVol], 'default': []},
+        "lvols": {"type": List[str], 'default': []},
         "node_lvs": {"type": str, 'default': "lvs"},
         "services": {"type": List[str], 'default': []},
         "cluster_id": {"type": str, 'default': ""},
         "api_endpoint": {"type": str, 'default': ""},
         "remote_devices": {"type": List[NVMeDevice], 'default': []},
         "host_secret": {"type": str, "default": ""},
         "ctrl_secret": {"type": str, "default": ""},
 
-        "cache_bdev": {"type": str, "default": ""},
-        "cache_size": {"type": int, "default": 0},
         "cpu": {"type": int, "default": 0},
         "cpu_hz": {"type": int, "default": 0},
         "memory": {"type": int, "default": 0},
         "hugepages": {"type": int, "default": 0},
+        "health_check": {"type": bool, "default": True},
 
+        # spdk params
+        "spdk_cpu_mask": {"type": str, "default": ""},
+        "spdk_mem": {"type": int, "default": 0},
+        "spdk_image": {"type": str, "default": ""},
+        "spdk_debug": {"type": bool, "default": False},
     }
 
     def __init__(self, data=None):
-        super(CachingNode, self).__init__()
+        super(StorageNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
 
     def get_id(self):
         return self.uuid
 
     def get_status_code(self):
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/lvol_model.py` & `sbcli-release-1.0.5/simplyblock_core/models/lvol_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from simplyblock_core.models.nvme_device import NVMeDevice
 
 
 class LVol(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
+    STATUS_IN_DELETION = 'in_deletion'
 
     attributes = {
         "lvol_name": {"type": str, 'default': ""},
         "size": {"type": int, 'default': 0},
+        "max_size": {"type": int, 'default': 0},
         "uuid": {"type": str, 'default': ""},
         "guid": {"type": str, 'default': ""},
         "ha_type": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
 
         "base_bdev": {"type": str, 'default': ""},
         "lvol_bdev": {"type": str, 'default': ""},
@@ -52,14 +54,18 @@
         "distr_bs": {"type": int, 'default': 0},
         "distr_chunk_bs": {"type": int, 'default': 0},
         "distr_page_size": {"type": int, 'default': 0},
 
         "health_check": {"type": bool, "default": True},
 
         "snapshot_name": {"type": str, 'default': ""},
+        "mem_diff": {"type": dict, 'default': {}},
+        "io_error": {"type": bool, 'default': False},
+
+        "deletion_status": {"type": str, 'default': ""},
 
     }
 
     def __init__(self, data=None):
         super(LVol, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/mgmt_node.py` & `sbcli-release-1.0.5/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/models/snapshot.py` & `sbcli-release-1.0.5/simplyblock_core/models/snapshot.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from simplyblock_core.models.base_model import BaseModel
 from simplyblock_core.models.lvol_model import LVol
 
 
 class SnapShot(BaseModel):
     attributes = {
         "uuid": {"type": str, 'default': ""},
-        "snap_name": {"type": str, 'default': 0},
-        "snap_bdev": {"type": str, 'default': 0},
+        "snap_name": {"type": str, 'default': ""},
+        "base_bdev": {"type": str, 'default': ""},
+        "snap_bdev": {"type": str, 'default': ""},
         "lvol": {"type": LVol, 'default': None},
         "created_at": {"type": int, 'default': 0},
+        "mem_diff": {"type": dict, 'default': {}},
     }
 
     def __init__(self, data=None):
         super(SnapShot, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/lvol_controller.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/lvol_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 import string
 import random
 import sys
 import time
 import uuid
 
 from simplyblock_core import utils, constants, distr_controller
-from simplyblock_core.controllers import snapshot_controller, pool_controller
+from simplyblock_core.controllers import snapshot_controller, pool_controller, lvol_events
 from simplyblock_core.kv_store import DBController
+from simplyblock_core.models.cluster import Cluster
+from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.pool import Pool
 from simplyblock_core.models.lvol_model import LVol
+from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.rpc_client import RPCClient
 
 
 logger = lg.getLogger()
 db_controller = DBController()
 
 
@@ -163,14 +166,15 @@
     return True, ""
 
 
 def get_jm_names(snode):
     return [f"jm_{snode.get_id()}"]
 
 
+# Deprecated
 def add_lvol(name, size, host_id_or_name, pool_id_or_name, use_comp, use_crypto,
              distr_vuid, distr_ndcs, distr_npcs,
              max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
              distr_bs=None, distr_chunk_bs=None):
     logger.info("adding LVol")
 
     snode = db_controller.get_storage_node_by_id(host_id_or_name)
@@ -183,15 +187,15 @@
     for p in db_controller.get_pools():
         if pool_id_or_name == p.id or pool_id_or_name == p.pool_name:
             pool = p
             break
     if not pool:
         return False, f"Pool not found: {pool_id_or_name}"
 
-    cl = db_controller.get_clusters(snode.cluster_id)[0]
+    cl = db_controller.get_cluster_by_id(snode.cluster_id)
     if cl.status not in [cl.STATUS_ACTIVE, cl.STATUS_DEGRADED]:
         return False, f"Cluster is not active, status: {cl.status}"
 
     max_rw_iops = max_rw_iops or 0
     max_rw_mbytes = max_rw_mbytes or 0
     max_r_mbytes = max_r_mbytes or 0
     max_w_mbytes = max_w_mbytes or 0
@@ -428,15 +432,15 @@
     else:
         return online_nodes
 
 
 def add_lvol_ha(name, size, host_id_or_name, ha_type, pool_id_or_name, use_comp, use_crypto,
                 distr_vuid, distr_ndcs, distr_npcs,
                 max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
-                distr_bs=None, distr_chunk_bs=None):
+                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0):
 
     logger.info(f"Adding LVol: {name}")
     host_node = None
     if host_id_or_name:
         host_node = db_controller.get_storage_node_by_id(host_id_or_name)
         if not host_node:
             host_node = db_controller.get_storage_node_by_hostname(host_id_or_name)
@@ -491,43 +495,70 @@
         logger.error("Storage nodes are less than 3 in ha cluster")
         return False, "Storage nodes are less than 3 in ha cluster"
 
     if len(online_nodes) == 0:
         logger.error("No online Storage nodes found")
         return False, "No online Storage nodes found"
 
+    cluster_size_prov = 0
+    cluster_size_total = 0
+    for lvol in db_controller.get_lvols():
+        cluster_size_prov += lvol.size
+
+    for dev in db_controller.get_storage_devices():
+        if dev.status == NVMeDevice.STATUS_ONLINE:
+            cluster_size_total += dev.size
+
+    cluster_size_prov_util = int(((cluster_size_prov+size) / cluster_size_total) * 100)
+
+    if cl.prov_cap_crit and cl.prov_cap_crit < cluster_size_prov_util:
+        msg = f"Cluster provisioned cap critical would be, util: {cluster_size_prov_util}% of cluster util: {cl.prov_cap_crit}"
+        logger.error(msg)
+        return False, msg
+
+    elif cl.prov_cap_warn and cl.prov_cap_warn < cluster_size_prov_util:
+        logger.warning(f"Cluster provisioned cap warning, util: {cluster_size_prov_util}% of cluster util: {cl.prov_cap_warn}")
+
     if distr_vuid == 0:
-        vuid = 1 + int(random.random() * 10000)
+        vuid = utils.get_random_vuid()
     else:
         vuid = distr_vuid
 
-    node_count = 0
-    for node in db_controller.get_storage_nodes():
-        if node.status == node.STATUS_ONLINE:
-            node_count += 1
     if distr_ndcs == 0 and distr_npcs == 0:
         if ha_type == "single":
             distr_ndcs = 4
             distr_npcs = 1
         else:
 
-            if node_count == 3:
+            if dev_count == 3:
                 distr_ndcs = 1
-            elif node_count in [4, 5]:
+            elif dev_count in [4, 5]:
                 distr_ndcs = 2
-            elif node_count >= 6:
+            elif dev_count >= 6:
                 distr_ndcs = 4
             distr_npcs = 1
     else:
-        if distr_ndcs + distr_npcs >= node_count:
-            return False, f"ndcs+npcs: {distr_ndcs+distr_npcs} must be less than online node count: {node_count}"
+        if distr_ndcs + distr_npcs >= dev_count:
+            return False, f"ndcs+npcs: {distr_ndcs+distr_npcs} must be less than online devices count: {dev_count}"
+
+    if max_size:
+        if max_size < size:
+            return False, f"Max size:{max_size} must be larger than size {size}"
+    else:
+        records = db_controller.get_cluster_capacity(cl)
+        if records:
+            max_size = records[0]['size_total']
+        else:
+            max_size = size * 10
 
+    logger.info(f"Max size: {utils.humanbytes(max_size)}")
     lvol = LVol()
     lvol.lvol_name = name
     lvol.size = size
+    lvol.max_size = max_size
     lvol.status = LVol.STATUS_ONLINE
     lvol.ha_type = ha_type
     lvol.bdev_stack = []
     lvol.uuid = str(uuid.uuid4())
     lvol.guid = _generate_hex_string(16)
     lvol.vuid = vuid
     lvol.lvol_bdev = f"LVS_{vuid}/{name}"
@@ -535,36 +566,89 @@
 
     lvol.crypto_bdev = ''
     lvol.comp_bdev = ''
 
     lvol.mode = 'read-write'
     lvol.lvol_type = 'lvol'
     lvol.nqn = cl.nqn + ":lvol:" + lvol.uuid
+
     lvol.ndcs = distr_ndcs
     lvol.npcs = distr_npcs
     lvol.distr_bs = distr_bs
     lvol.distr_chunk_bs = distr_chunk_bs
     lvol.distr_page_size = cl.page_size_in_blocks
+
     lvol.base_bdev = f"distr_{lvol.vuid}_{name}"
-    # lvol.top_bdev = lvol.lvol_bdev
     lvol.top_bdev = lvol.base_bdev
 
-    lvol.bdev_stack.append({"type": "distr", "name": lvol.base_bdev})
-    # lvol.bdev_stack.append({"type": "lvs", "name": lvol.lvs_name})
-    # lvol.bdev_stack.append({"type": "lvol", "name": lvol.lvol_bdev})
+    lvol.bdev_stack.append({
+        "type": "bdev_distr",
+        "name": lvol.base_bdev,
+        "params": {
+            "name": lvol.base_bdev,
+            "vuid": lvol.vuid,
+            "ndcs": lvol.ndcs,
+            "npcs": lvol.npcs,
+            "num_blocks": int(lvol.size / lvol.distr_bs),
+            "block_size": lvol.distr_bs,
+            "chunk_size": lvol.distr_chunk_bs,
+            "pba_page_size":  lvol.distr_page_size,
+        }
+    })
+
+    if with_snapshot:
+        lvol.bdev_stack.append({
+            "type": "bmap_init",
+            "name": lvol.base_bdev,
+            "params": {
+                "bdev_name": lvol.base_bdev,
+                "num_blocks": int(lvol.size / lvol.distr_bs),
+                "block_len": lvol.distr_bs,
+                "page_len": int(lvol.distr_page_size / lvol.distr_bs),
+                "max_num_blocks": int(lvol.max_size / lvol.distr_bs)
+            }
+        })
+        lvol.snapshot_name = f"snapshot_{lvol.vuid}_{name}"
+        lvol.top_bdev = f"lvol_{lvol.vuid}_{lvol.lvol_name}"
+        lvol.bdev_stack.append({
+            "type": "ultra_lvol",
+            "name": lvol.top_bdev,
+            "params": {
+                "lvol_name": lvol.top_bdev,
+                "base_bdev": lvol.base_bdev,
+                "label": "label",
+                "desc": "desc"
+            }
+        })
 
     if use_crypto is True:
         lvol.crypto_bdev = f"crypto_{lvol.lvol_name}"
-        lvol.bdev_stack.append({"type": "crypto", "name": lvol.crypto_bdev})
+        lvol.bdev_stack.append({
+            "type": "crypto",
+            "name": lvol.crypto_bdev,
+            "params": {
+                "name": lvol.crypto_bdev,
+                "base_name": lvol.lvol_bdev
+            }
+        })
         lvol.lvol_type += ',crypto'
         lvol.top_bdev = lvol.crypto_bdev
 
     if use_comp is True:
+        base_bdev = lvol.lvol_bdev
+        if lvol.crypto_bdev:
+            base_bdev = lvol.crypto_bdev
         lvol.comp_bdev = f"comp_{lvol.lvol_name}"
-        lvol.bdev_stack.append({"type": "comp", "name": lvol.comp_bdev})
+        lvol.bdev_stack.append({
+            "type": "comp",
+            "name": lvol.comp_bdev,
+            "params": {
+                "base_bdev_name": base_bdev
+            }
+        })
         lvol.lvol_type += ',compress'
         lvol.top_bdev = lvol.comp_bdev
 
     nodes = _get_next_3_nodes()
     if host_node:
         nodes.insert(0, host_node)
     else:
@@ -598,48 +682,81 @@
     host_node.write_to_db(db_controller.kv_store)
 
     lvol.pool_uuid = pool.id
     pool.lvols.append(lvol.uuid)
     pool.write_to_db(db_controller.kv_store)
 
     lvol.write_to_db(db_controller.kv_store)
+    lvol_events.lvol_create(lvol)
 
     # set QOS
     if max_rw_iops or max_rw_mbytes or max_r_mbytes or max_w_mbytes:
         set_lvol(lvol.uuid, max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes)
     return lvol.uuid, None
 
 
-def add_lvol_on_node(lvol, snode, ha_comm_addrs=None, ha_inode_self=None):
-    jm_names = get_jm_names(snode)
+def _create_bdev_stack(lvol, snode, ha_comm_addrs, ha_inode_self):
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
-    num_blocks = int(lvol.size / lvol.distr_bs)
-    ret = rpc_client.bdev_distrib_create(
-        lvol.base_bdev, lvol.vuid, lvol.ndcs, lvol.npcs, num_blocks,
-        lvol.distr_bs, jm_names, lvol.distr_chunk_bs, ha_comm_addrs, ha_inode_self, lvol.distr_page_size)
-    if not ret:
-        logger.error("Failed to create Distr bdev")
-        return False, "Failed to create Distr bdev"
-    if ret == "?":
-        logger.error(f"Failed to create Distr bdev, ret={ret}")
-        # return False
 
-    if lvol.crypto_bdev:
-        crypto_bdev = _create_crypto_lvol(rpc_client, lvol.crypto_bdev, lvol.lvol_bdev)
-        if not crypto_bdev:
-            return False, "Error creating crypto bdev"
+    created_bdevs = []
+    for bdev in lvol.bdev_stack:
+        # if 'status' in bdev and bdev['status'] == 'created':
+        #     continue
 
-    if lvol.comp_bdev:
-        base_bdev = lvol.lvol_bdev
-        if lvol.crypto_bdev:
-            base_bdev = lvol.crypto_bdev
+        type = bdev['type']
+        name = bdev['name']
+        params = bdev['params']
+        ret = None
 
-        comp_bdev = _create_compress_lvol(rpc_client, base_bdev)
-        if not comp_bdev:
-            return False, "Error creating comp bdev"
+        if type == "bdev_distr":
+            params['jm_names'] = get_jm_names(snode)
+            params['ha_comm_addrs'] = ha_comm_addrs
+            params['ha_inode_self'] = ha_inode_self
+            ret = rpc_client.bdev_distrib_create(**params)
+
+            snodes = db_controller.get_storage_nodes()
+            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
+            cluster_map_data['UUID_node_target'] = snode.get_id()
+            rpc_client.distr_send_cluster_map(cluster_map_data)
+
+        elif type == "bmap_init":
+            ret = rpc_client.ultra21_lvol_bmap_init(**params)
+
+        elif type == "ultra_lvol":
+            ret = rpc_client.ultra21_lvol_mount_lvol(**params)
+
+        elif type == "crypto":
+            ret = _create_crypto_lvol(rpc_client, **params)
+
+        elif type == "comp":
+            ret = _create_compress_lvol(rpc_client, **params)
+
+        else:
+            logger.debug(f"Unknown BDev type: {type}")
+            continue
+
+        if ret:
+            bdev['status'] = "created"
+            created_bdevs.append(bdev)
+        else:
+            if created_bdevs:
+                # rollback
+                _remove_bdev_stack(created_bdevs, rpc_client)
+            return False, f"Failed to create BDev: {name}"
+
+    return True, None
+
+
+def add_lvol_on_node(lvol, snode, ha_comm_addrs=None, ha_inode_self=None):
+    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+    spdk_mem_info_before = rpc_client.ultra21_util_get_malloc_stats()
+
+    ret, msg = _create_bdev_stack(lvol, snode, ha_comm_addrs, ha_inode_self)
+    if not ret:
+        return False, msg
 
     logger.info("creating subsystem %s", lvol.nqn)
     ret = rpc_client.subsystem_create(lvol.nqn, 'sbcli-cn', lvol.uuid)
     logger.debug(ret)
 
     # add listeners
     logger.info("adding listeners")
@@ -659,23 +776,37 @@
             is_optimized = False
             # if lvol.node_id == snode.get_id():
             #     is_optimized = True
             logger.info(f"Setting ANA state: {is_optimized}")
             ret = rpc_client.nvmf_subsystem_listener_set_ana_state(
                 lvol.nqn, iface.ip4_address, "4420", is_optimized)
 
-    logger.info("add lvol to subsystem")
+    logger.info("Add BDev to subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(lvol.nqn, lvol.top_bdev, lvol.uuid, lvol.guid)
+    if not ret:
+        return False, "Failed to add bdev to subsystem"
 
-    logger.info("Sending cluster map to the lvol")
+    logger.info("Sending cluster map to LVol")
     snodes = db_controller.get_storage_nodes()
     cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
     cluster_map_data['UUID_node_target'] = snode.get_id()
     ret = rpc_client.distr_send_cluster_map(cluster_map_data)
 
+    spdk_mem_info_after = rpc_client.ultra21_util_get_malloc_stats()
+    logger.debug("ultra21_util_get_malloc_stats:")
+    logger.debug(spdk_mem_info_after)
+
+    diff = {}
+    for key in spdk_mem_info_after.keys():
+        diff[key] = spdk_mem_info_after[key] - spdk_mem_info_before[key]
+
+    logger.info("spdk mem diff:")
+    logger.info(json.dumps(diff, indent=2))
+    lvol.mem_diff = diff
+
     return True, None
 
 
 def recreate_lvol(lvol_id, snode):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"lvol not found: {lvol_id}")
@@ -699,61 +830,79 @@
             is_created, error = add_lvol_on_node(lvol, sn, ha_address, index)
             if error:
                 return False
 
     return lvol
 
 
-def delete_lvol_from_node(lvol, node_id):
-    snode = db_controller.get_storage_node_by_id(node_id)
-    logger.debug(f"Deleting LVol:{lvol.get_id()} from node:{snode.get_id()}")
-    rpc_client = RPCClient(
-        snode.mgmt_ip, snode.rpc_port,
-        snode.rpc_username, snode.rpc_password)
+def _remove_bdev_stack(bdev_stack, rpc_client):
+    for bdev in bdev_stack:
+        if 'status' in bdev and bdev['status'] == 'deleted':
+            continue
 
-    for bdev in lvol.bdev_stack[::-1]:
         type = bdev['type']
         name = bdev['name']
-        if type == "alceml":
-            ret = rpc_client.bdev_alceml_delete(name)
-            if not ret:
-                logger.error(f"failed to delete alceml: {name}")
-            continue
-        if type == "distr":
+        ret = None
+        # if type == "alceml":
+        #     ret = rpc_client.bdev_alceml_delete(name)
+        if type == "bdev_distr":
             ret = rpc_client.bdev_distrib_delete(name)
-            if not ret:
-                logger.error(f"failed to delete distr: {name}")
-            continue
-        if type == "lvs":
-            ret = rpc_client.bdev_lvol_delete_lvstore(name)
-            if not ret:
-                logger.error(f"failed to delete lvs: {name}")
-            continue
-        if type == "lvol":
-            ret = rpc_client.delete_lvol(name)
-            if not ret:
-                logger.error(f"failed to delete lvol bdev {name}")
-            continue
-        if type == "ultra_pt":
-            ret = rpc_client.ultra21_bdev_pass_delete(name)
-            if not ret:
-                logger.error(f"failed to delete ultra pt {name}")
-            continue
-        if type == "comp":
+        # elif type == "lvs":
+        #     ret = rpc_client.bdev_lvol_delete_lvstore(name)
+        # elif type == "lvol":
+        #     ret = rpc_client.delete_lvol(name)
+        # elif type == "ultra_pt":
+        #     ret = rpc_client.ultra21_bdev_pass_delete(name)
+        elif type == "ultra_lvol":
+            ret = rpc_client.ultra21_lvol_dismount(name)
+        elif type == "comp":
             ret = rpc_client.lvol_compress_delete(name)
-            if not ret:
-                logger.error(f"failed to delete comp bdev {name}")
-            continue
-        if type == "crypto":
+        elif type == "crypto":
             ret = rpc_client.lvol_crypto_delete(name)
-            if not ret:
-                logger.error(f"failed to delete crypto bdev {name}")
+        else:
+            logger.debug(f"Unknown BDev type: {type}")
             continue
 
+        if not ret:
+            logger.error(f"Failed to delete BDev {name}")
+
+        bdev['status'] = 'deleted'
+        time.sleep(1)
+
+
+def delete_lvol_from_node(lvol_id, node_id, clear_data=True):
+    lvol = db_controller.get_lvol_by_id(lvol_id)
+    snode = db_controller.get_storage_node_by_id(node_id)
+    logger.debug(f"Deleting LVol:{lvol.get_id()} from node:{snode.get_id()}")
+    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+
+    # 1- remove bdevs
+    _remove_bdev_stack(lvol.bdev_stack[::-1], rpc_client)
+    lvol.deletion_status = 'bdevs_deleted'
+    lvol.write_to_db(db_controller.kv_store)
+
+    # 2- remove subsystem
     ret = rpc_client.subsystem_delete(lvol.nqn)
+
+    # 3- clear alceml devices
+    if clear_data:
+        for node in db_controller.get_storage_nodes():
+            if node.status == StorageNode.STATUS_ONLINE:
+                rpc_node = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+                for dev in node.nvme_devices:
+                    ret = rpc_node.alceml_unmap_vuid(dev.alceml_bdev, lvol.vuid)
+
+    lvol.deletion_status = 'alceml_unmapped'
+    lvol.write_to_db(db_controller.kv_store)
+
+    # 4- clear JM
+    # ret = rpc_client.alceml_unmap_vuid(name, lvol.vuid)
+    # lvol.deletion_status = 'jm_unmapped'
+    lvol.write_to_db(db_controller.kv_store)
+
     return True
 
 
 def delete_lvol(uuid, force_delete=False):
     lvol = db_controller.get_lvol_by_id(uuid)
     if not lvol:
         logger.error(f"lvol not found: {uuid}")
@@ -780,21 +929,25 @@
             logger.warning(f"Soft delete LVol that has snapshots. Snapshot:{snap.get_id()}")
             ret = rpc_client.subsystem_delete(lvol.nqn)
             logger.debug(ret)
             lvol.deleted = True
             lvol.write_to_db(db_controller.kv_store)
             return True
 
+    # set status
+    lvol.status = LVol.STATUS_IN_DELETION
+    lvol.write_to_db(db_controller.kv_store)
+
     if lvol.ha_type == 'single':
-        ret = delete_lvol_from_node(lvol, lvol.node_id)
+        ret = delete_lvol_from_node(lvol.get_id(), lvol.node_id)
         if not ret:
             return False
     elif lvol.ha_type == "ha":
         for nodes_id in lvol.nodes:
-            ret = delete_lvol_from_node(lvol, nodes_id)
+            ret = delete_lvol_from_node(lvol.get_id(), nodes_id)
             if not ret:
                 return False
 
     # remove from storage node
     snode.lvols.remove(uuid)
     snode.write_to_db(db_controller.kv_store)
 
@@ -811,14 +964,15 @@
             lvols_count = 0
             for lvol in db_controller.get_lvols():
                 if lvol.cloned_from_snap == snap.get_id():
                     lvols_count += 1
             if lvols_count == 0:
                 snapshot_controller.delete(snap.get_id())
 
+    lvol_events.lvol_delete(lvol)
     logger.info("Done")
     return True
 
 
 def set_lvol(uuid, max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes, name=None):
     lvol = db_controller.get_lvol_by_id(uuid)
     if not lvol:
@@ -874,34 +1028,65 @@
     lvols = db_controller.get_lvols()
     data = []
     for lvol in lvols:
         if lvol.deleted is True:
             continue
         logger.debug(lvol)
         data.append({
+            "Id": lvol.uuid,
+            "Name": lvol.lvol_name,
+            "Size": utils.humanbytes(lvol.size),
+            "Hostname": lvol.hostname,
+            "HA": lvol.ha_type,
+            "VUID": lvol.vuid,
+            "Mod": f"{lvol.ndcs}x{lvol.npcs}",
+            "Status": lvol.status,
+            "IO Err": lvol.io_error,
+            "Health": lvol.health_check,
+        })
+
+    if is_json:
+        return json.dumps(data, indent=2)
+    else:
+        return utils.print_table(data)
+
+
+def list_lvols_mem(is_json, is_csv):
+    lvols = db_controller.get_lvols()
+    data = []
+    for lvol in lvols:
+        if lvol.deleted is True:
+            continue
+        logger.debug(lvol)
+        data.append({
             "id": lvol.uuid,
-            "name": lvol.lvol_name,
             "size": utils.humanbytes(lvol.size),
-            "pool": lvol.pool_uuid,
-            "hostname": lvol.hostname,
-            "ha type": lvol.ha_type,
-            "status": lvol.status,
-            "health": lvol.health_check,
+            "max_size": utils.humanbytes(lvol.max_size),
+            **lvol.mem_diff
         })
 
     if is_json:
         return json.dumps(data, indent=2)
+    elif is_csv:
+        print(";".join(data[0].keys()))
+        for d in data:
+            print(";".join([str(v) for v in d.values()]))
     else:
         return utils.print_table(data)
 
 
-def get_lvol(lvol_id, is_json):
-    lvol = db_controller.get_lvol_by_id(lvol_id)
+def get_lvol(lvol_id_or_name, is_json):
+    lvol = None
+    for lv in db_controller.get_lvols():
+        if lv.get_id() == lvol_id_or_name or lv.lvol_name == lvol_id_or_name:
+            lvol = lv
+            break
+
     if not lvol:
-        logger.error(f"lvol not found: {lvol_id}")
+        logger.error(f"LVol id or name not found: {lvol_id_or_name}")
         return False
 
     data = lvol.get_clean_dict()
 
     del data['nvme_dev']
 
     if is_json:
@@ -1009,17 +1194,20 @@
         snode.rpc_username,
         snode.rpc_password)
 
     ret = rpc_client.lvol_read_only(lvol.lvol_bdev)
     if not ret:
         return "Error"
 
+    old_status = lvol.mode
     lvol.mode = 'read-only'
     lvol.write_to_db(db_controller.kv_store)
     logger.info("Done")
+    lvol_events.lvol_status_change(lvol, lvol.mode, old_status)
+
     return True
 
 
 def create_snapshot(lvol_id, snapshot_name):
     return snapshot_controller.add(lvol_id, snapshot_name)
 
 
@@ -1109,23 +1297,27 @@
         return False
     logger.info(ret)
     print("*"*100)
     results, is_passed = distr_controller.parse_distr_cluster_map(ret)
     return utils.print_table(results)
 
 
-def migrate(lvol_id):
+def migrate(lvol_id, node_id):
 
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"lvol not found: {lvol_id}")
         return False
 
+    old_node = lvol.node_id
     nodes = _get_next_3_nodes()
 
+    if node_id:
+        nodes[0] = db_controller.get_storage_node_by_id(node_id)
+
     host_node = nodes[0]
     lvol.hostname = host_node.hostname
     lvol.node_id = host_node.get_id()
 
     if lvol.ha_type == 'single':
         ret = add_lvol_on_node(lvol, host_node)
         if not ret:
@@ -1146,8 +1338,54 @@
             if not ret:
                 return ret
         lvol.nodes = nodes_ids
 
     host_node.lvols.append(lvol.uuid)
     host_node.write_to_db(db_controller.kv_store)
     lvol.write_to_db(db_controller.kv_store)
+
+    lvol_events.lvol_migrate(lvol, old_node, lvol.node_id)
+
     return True
+
+
+def move(lvol_id, node_id, force=False):
+    lvol = db_controller.get_lvol_by_id(lvol_id)
+    if not lvol:
+        logger.error(f"lvol not found: {lvol_id}")
+        return False
+
+    target_node = db_controller.get_storage_node_by_id(node_id)
+    if not target_node:
+        logger.error(f"Node not found: {target_node}")
+        return False
+
+    if lvol.node_id == target_node.get_id():
+        return True
+
+    if target_node.status != StorageNode.STATUS_ONLINE:
+        logger.error(f"Node is not online!: {target_node}, status: {target_node.status}")
+        return False
+
+    src_node = db_controller.get_storage_node_by_id(lvol.node_id)
+
+    if src_node.status == StorageNode.STATUS_ONLINE:
+        if not force:
+            logger.error(f"Node is online!: {src_node.get_id()}, use --force to force move")
+            return False
+
+    if migrate(lvol_id, node_id):
+        if src_node.status == StorageNode.STATUS_ONLINE:
+            # delete lvol
+            if lvol.ha_type == 'single':
+                delete_lvol_from_node(lvol_id, lvol.node_id, clear_data=False)
+            elif lvol.ha_type == "ha":
+                for nodes_id in lvol.nodes:
+                    delete_lvol_from_node(lvol_id, nodes_id, clear_data=False)
+
+            # remove from storage node
+            src_node.lvols.remove(lvol_id)
+            src_node.write_to_db(db_controller.kv_store)
+        return True
+    else:
+        logger.error("Failed to migrate lvol")
+        return False
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/health_controller.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/health_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 def check_node(node_id, with_devices=True):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error("node not found")
         return False
 
+    if snode.status in [StorageNode.STATUS_OFFLINE, StorageNode.STATUS_REMOVED]:
+        logger.info(f"Skipping ,node status is {snode.status}")
+        return True
+
     logger.info(f"Checking node {node_id}, status: {snode.status}")
 
     print("*" * 100)
 
     # passed = True
 
     # 1- check node ping
@@ -136,15 +140,16 @@
 
     if not node_rpc_check:
         logger.info("Skipping devices checks because RPC check failed")
     else:
         logger.info(f"Node device count: {len(snode.nvme_devices)}")
         for dev in snode.nvme_devices:
             ret = check_device(dev.get_id())
-            node_devices_check &= ret
+            if dev.status in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
+                node_devices_check &= ret
             print("*" * 100)
 
         logger.info(f"Node remote device: {len(snode.remote_devices)}")
 
         rpc_client = RPCClient(
             snode.mgmt_ip, snode.rpc_port,
             snode.rpc_username, snode.rpc_password,
@@ -168,22 +173,31 @@
         return False
 
     snode = db_controller.get_storage_node_by_id(device.node_id)
     if not snode:
         logger.error("node not found")
         return False
 
+    if snode.status in [StorageNode.STATUS_OFFLINE, StorageNode.STATUS_REMOVED]:
+        logger.info(f"Skipping ,node status is {snode.status}")
+        return True
+
+    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_UNRECOGNIZED]:
+        logger.info(f"Skipping ,device status is {device.status}")
+        return True
+
     passed = True
     try:
         rpc_client = RPCClient(
             snode.mgmt_ip, snode.rpc_port,
-            snode.rpc_username, snode.rpc_password,
-            timeout=3, retry=1)
+            snode.rpc_username, snode.rpc_password)
 
         bdevs_stack = [device.nvme_bdev, device.testing_bdev, device.alceml_bdev, device.pt_bdev]
+        if device.jm_bdev:
+            bdevs_stack.append(device.jm_bdev)
         logger.info(f"Checking Device: {device_id}, status:{device.status}")
         problems = 0
         for bdev in bdevs_stack:
             if not bdev:
                 continue
             ret = rpc_client.get_bdevs(bdev)
             if ret:
@@ -222,33 +236,30 @@
         logger.error("device not found")
         return False
     snode = db_controller.get_storage_node_by_id(device.node_id)
     if not snode:
         logger.error("node not found")
         return False
 
-    # if device.status is not NVMeDevice.STATUS_ONLINE:
-    #     logger.error("device is not online")
-    #     return False
-
+    result = True
     for node in db_controller.get_storage_nodes():
         if node.status == StorageNode.STATUS_ONLINE:
             if node.get_id() == snode.get_id():
                 continue
             logger.info(f"Connecting to node: {node.get_id()}")
             rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
             name = f"remote_{device.alceml_bdev}n1"
             ret = rpc_client.get_bdevs(name)
             if ret:
                 logger.info(f"Checking bdev: {device.alceml_bdev} ... ok")
             else:
                 logger.info(f"Checking bdev: {device.alceml_bdev} ... not found")
-                # return False
-    # logger.info("All good")
-    return True
+                result = False
+
+    return result
 
 
 def check_lvol_on_node(lvol_id, node_id):
 
     db_controller = DBController()
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
@@ -262,25 +273,25 @@
 
     passed = True
     try:
         for bdev_info in lvol.bdev_stack:
             bdev_name = bdev_info['name']
             ret = rpc_client.get_bdevs(bdev_name)
             if ret:
-                logger.info(f"Checking LVol: {lvol_id} ... ok")
+                logger.info(f"Checking bdev: {bdev_name} ... ok")
             else:
-                logger.error(f"Checking LVol: {lvol_id} ... failed")
+                logger.error(f"Checking LVol: {bdev_name} ... failed")
                 passed = False
 
-            ret = rpc_client.subsystem_list(lvol.nqn)
-            if ret:
-                logger.info(f"Checking subsystem ... ok")
-            else:
-                logger.info(f"Checking subsystem ... not found")
-                passed = False
+        ret = rpc_client.subsystem_list(lvol.nqn)
+        if ret:
+            logger.info(f"Checking subsystem ... ok")
+        else:
+            logger.info(f"Checking subsystem ... not found")
+            passed = False
 
         logger.info("Checking Distr map ...")
         ret = rpc_client.distr_get_cluster_map(lvol.base_bdev)
         if not ret:
             logger.error("Failed to get cluster map")
             passed = False
         else:
@@ -299,19 +310,19 @@
     # then change its status to offline if fails this check
     online_devices = 0
     for node in db_controller.get_storage_nodes():
         for dev in node.nvme_devices:
             if dev.status == dev.STATUS_ONLINE:
                 online_devices += 1
 
-    if lvol.ndcs + lvol.npcs < online_devices:
-        logger.info(f"Checking Distr ndcs+npcs: {lvol.ndcs}+{lvol.npcs}, online devices: {online_devices} ... ok")
-    else:
-        logger.info(f"Checking Distr ndcs+npcs: {lvol.ndcs}+{lvol.npcs}, online devices: {online_devices} ... failed")
-        passed = False
+    # if lvol.ndcs + lvol.npcs < online_devices:
+    #     logger.info(f"Checking Distr ndcs+npcs: {lvol.ndcs}+{lvol.npcs}, online devices: {online_devices} ... ok")
+    # else:
+    #     logger.info(f"Checking Distr ndcs+npcs: {lvol.ndcs}+{lvol.npcs}, online devices: {online_devices} ... failed")
+        # passed = False
 
     return passed
 
 
 def check_lvol(lvol_id):
     db_controller = DBController()
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/caching_node_controller.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/caching_node_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,35 +75,33 @@
     return devices
 
 
 def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image=None):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
-    clusters = db_controller.get_clusters(cluster_id)
-    if not clusters:
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
-    cluster = clusters[0]
 
     logger.info(f"Add Caching node: {node_ip}")
     snode_api = CNodeClient(node_ip)
 
     node_info, _ = snode_api.info()
     logger.info(f"Node found: {node_info['hostname']}")
 
     hostname = node_info['hostname']
     snode = db_controller.get_storage_node_by_hostname(hostname)
     if snode:
         logger.error("Node already exists, try remove it first.")
         return False
 
-
     node_info, _ = snode_api.info()
-    # results, err = snode_api.join_db(db_connection=cluster.db_connection)
+    results, err = snode_api.join_db(db_connection=cluster.db_connection)
 
     data_nics = []
     names = data_nics_list or [iface_name]
     for nic in names:
         device = node_info['network_interface'][nic]
         data_nics.append(
             IFace({
@@ -202,15 +200,17 @@
     cache_size = 0
     cache_bdev = None
     if supported_ssd_size < ssd_size:
         logger.info(f"SSD size is bigger than the supported size, will use split bdev: {split_factor}")
         ret = rpc_client.bdev_split(ssd_dev.nvme_bdev, split_factor)
         cache_bdev = ret[0]
         cache_size = int(ssd_dev.size/split_factor)
+        snode.cache_split_factor = split_factor
     else:
+        snode.cache_split_factor = 0
         cache_bdev = ssd_dev.nvme_bdev
         cache_size = ssd_dev.size
 
     logger.info(f"Cache size: {utils.humanbytes(cache_size)}")
 
     snode.cache_bdev = cache_bdev
     snode.cache_size = cache_size
@@ -237,19 +237,18 @@
 def recreate(node_id):
     db_controller = DBController()
     snode = db_controller.get_caching_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find caching node: {node_id}")
         return False
 
-    clusters = db_controller.get_clusters(snode.cluster_id)
-    if not clusters:
+    cluster = db_controller.get_cluster_by_id(snode.cluster_id)
+    if not cluster:
         logger.error("Cluster not found: %s", snode.cluster_id)
         return False
-    cluster = clusters[0]
 
     logger.info(f"Recreating caching node: {node_id}, status: {snode.status}")
     snode_api = CNodeClient(f"{snode.mgmt_ip}:5000")
 
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
@@ -265,56 +264,27 @@
         return False
 
     snode.nvme_devices = nvme_devs
     # snode.write_to_db(db_controller.kv_store)
 
     ssd_dev = nvme_devs[0]
 
-    # get node hugepages memory
-    mem = node_info['memory_details']['huge_free']
-    logger.info(f"Free hugepages detected: {utils.humanbytes(mem)}")
-    if mem < 1024*1024:
-        logger.error("Hugepages must be larger than 1G")
-        return False
-
-    mem = int(mem*constants.CACHING_NODE_MEMORY_FACTOR)
-    snode.hugepages = mem
-    logger.info(f"Hugepages to be used: {utils.humanbytes(mem)}")
-
-    ssd_size = ssd_dev.size
-    supported_ssd_size = mem * 100 / 2
-    split_factor = math.ceil(ssd_size/supported_ssd_size)
-
-    logger.info(f"Supported SSD size: {utils.humanbytes(supported_ssd_size)}")
-    logger.info(f"Current SSD size: {utils.humanbytes(ssd_size)}")
-
-    cache_size = 0
-    cache_bdev = None
-    if supported_ssd_size < ssd_size:
-        logger.info(f"SSD size is bigger than the supported size, will use split bdev: {split_factor}")
-        ret = rpc_client.bdev_split(ssd_dev.nvme_bdev, split_factor)
-        cache_bdev = ret[0]
-        cache_size = int(ssd_dev.size/split_factor)
-    else:
-        cache_bdev = ssd_dev.nvme_bdev
-        cache_size = ssd_dev.size
-
-    logger.info(f"Cache size: {utils.humanbytes(cache_size)}")
+    if snode.cache_split_factor > 1:
+        ret = rpc_client.bdev_split(ssd_dev.nvme_bdev, snode.cache_split_factor)
 
-    snode.cache_bdev = cache_bdev
-    snode.cache_size = cache_size
+    logger.info(f"Cache size: {utils.humanbytes(snode.cache_size)}")
 
     # create tmp ocf
     logger.info(f"Creating first ocf bdev...")
 
     ret = rpc_client.bdev_malloc_create("malloc_tmp", 512, int((100 * 1024 * 1024) / 512))
     if not ret:
         logger.error("Failed ot create tmp malloc")
         return False
-    ret = rpc_client.bdev_ocf_create("ocf_tmp", 'wt', cache_bdev, "malloc_tmp")
+    ret = rpc_client.bdev_ocf_create("ocf_tmp", 'wt', snode.cache_bdev, "malloc_tmp")
     if not ret:
         logger.error("Failed ot create tmp OCF BDev")
         return False
 
     if snode.lvols:
         for lvol in snode.lvols:
             ret = connect(snode.get_id(), lvol.lvol_id)
@@ -327,15 +297,14 @@
     snode.status = CachingNode.STATUS_ONLINE
     snode.write_to_db(db_controller.kv_store)
 
     logger.info("Done")
     return True
 
 
-
 def connect(caching_node_id, lvol_id):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
 
     if lvol.status != lvol.STATUS_ONLINE:
@@ -578,15 +547,15 @@
             node.stop()
             node.remove(force=True)
             time.sleep(2)
 
     logger.info("Creating CachingNodeAPI container")
     container = node_docker.containers.run(
         constants.SIMPLY_BLOCK_DOCKER_IMAGE,
-        "python simplyblock_web/node_webapp.py caching_docker_node",
+        "python simplyblock_web/caching_node_app.py",
         detach=True,
         privileged=True,
         name="CachingNodeAPI",
         network_mode="host",
         volumes=[
             '/etc/foundationdb:/etc/foundationdb',
             '/var/tmp:/var/tmp',
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/storage_events.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/storage_events.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,49 +47,8 @@
         event=ec.EVENT_STATUS_CHANGE,
         db_object=node,
         caused_by=caused_by,
         message=f"Storage node health check changed from: {old_status} to: {new_state}",
         node_id=node.get_id())
 
 
-def device_health_check_change(cluster_id, device, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
-    ec.log_event_cluster(
-        cluster_id=cluster_id,
-        domain=ec.DOMAIN_CLUSTER,
-        event=ec.EVENT_STATUS_CHANGE,
-        db_object=device,
-        caused_by=caused_by,
-        message=f"Device health check changed from: {old_status} to: {new_state}",
-        node_id=device.get_id())
-
-
-def lvol_health_check_change(cluster_id, lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
-    ec.log_event_cluster(
-        cluster_id=cluster_id,
-        domain=ec.DOMAIN_CLUSTER,
-        event=ec.EVENT_STATUS_CHANGE,
-        db_object=lvol,
-        caused_by=caused_by,
-        message=f"LVol health check changed from: {old_status} to: {new_state}",
-        node_id=lvol.get_id())
-
 
-def lvol_status_change(cluster_id, lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
-    ec.log_event_cluster(
-        cluster_id=cluster_id,
-        domain=ec.DOMAIN_CLUSTER,
-        event=ec.EVENT_STATUS_CHANGE,
-        db_object=lvol,
-        caused_by=caused_by,
-        message=f"LVol status changed from: {old_status} to: {new_state}",
-        node_id=lvol.get_id())
-
-
-def device_status_change(cluster_id, device, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
-    ec.log_event_cluster(
-        cluster_id=cluster_id,
-        domain=ec.DOMAIN_CLUSTER,
-        event=ec.EVENT_STATUS_CHANGE,
-        db_object=device,
-        caused_by=caused_by,
-        message=f"Device status changed from: {old_status} to: {new_state}",
-        node_id=device.get_id())
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/events_controller.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/cluster_events.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/pool_controller.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/pool_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import random
 import string
 import time
 import uuid
 
 from simplyblock_core import utils
+from simplyblock_core.controllers import pool_events
 from simplyblock_core.kv_store import DBController
 from simplyblock_core.models.pool import Pool
 
 logger = lg.getLogger()
 
 db_controller = DBController()
 
@@ -41,28 +42,32 @@
     max_w_mbytes = max_w_mbytes or 0
 
     if max_rw_mbytes > 0:
         if max_r_mbytes > max_rw_mbytes or max_w_mbytes > max_rw_mbytes:
             logger.error("max_rw_mbytes must be greater than max_w_mbytes and max_r_mbytes")
             return False
 
+    cluster = db_controller.get_clusters()[0]
     logger.info("Adding pool")
     pool = Pool()
     pool.id = str(uuid.uuid4())
+    pool.cluster_id = cluster.get_id()
     pool.pool_name = name
     if has_secret:
         pool.secret = _generate_string(20)
     pool.pool_max_size = pool_max
     pool.lvol_max_size = lvol_max
     pool.max_rw_ios_per_sec = max_rw_iops
     pool.max_rw_mbytes_per_sec = max_rw_mbytes
     pool.max_r_mbytes_per_sec = max_r_mbytes
     pool.max_w_mbytes_per_sec = max_w_mbytes
     pool.status = "active"
     pool.write_to_db(db_controller.kv_store)
+
+    pool_events.pool_add(pool)
     logger.info("Done")
     return pool.id
 
 
 def set_pool_value_if_above(pool, key, value):
     logger.info(f"Updating pool {key}: {value}")
     current_value = getattr(pool, key)
@@ -102,14 +107,15 @@
         if not set_pool_value_if_above(pool, "max_r_mbytes_per_sec", max_r_mbytes):
             return False
     if max_w_mbytes:
         if not set_pool_value_if_above(pool, "max_w_mbytes_per_sec", max_w_mbytes):
             return False
 
     pool.write_to_db(db_controller.kv_store)
+    pool_events.pool_updated(pool)
     logger.info("Done")
     return True
 
 
 def delete_pool(uuid):
     pool = db_controller.get_pool_by_id(uuid)
     if not pool:
@@ -120,14 +126,15 @@
         return False
 
     if pool.lvols:
         logger.error(f"Pool is not empty {uuid}")
         return False
 
     logger.info(f"Deleting pool {pool.id}")
+    pool_events.pool_remove(pool)
     pool.remove(db_controller.kv_store)
     logger.info("Done")
     return True
 
 
 def list_pools(is_json):
     pools = db_controller.get_pools()
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/controllers/mgmt_events.py` & `sbcli-release-1.0.5/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/scripts/install_deps.sh` & `sbcli-release-1.0.5/simplyblock_core/scripts/install_deps.sh`

 * *Files 6% similar despite different names*

```diff
@@ -30,7 +30,12 @@
 sudo service sshd restart
 sudo modprobe nvme-tcp
 
 sudo sysctl -w net.ipv6.conf.all.disable_ipv6=1
 
 # required for graylog
 sudo sysctl -w vm.max_map_count=262144
+
+sudo mkdir -p /etc/simplyblock
+sudo chmod 777 /etc/simplyblock
+
+sudo sh -c 'echo 1 >  /proc/sys/vm/drop_caches'
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli-release-1.0.5/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,14 @@
       - "/etc/foundationdb/logs:/var/fdb/logs"
 
     deploy:
       mode: global
       placement:
         constraints: [ node.role == manager ]
 
-
   WebAppAPI:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     command: "python simplyblock_web/app.py"
     deploy:
       endpoint_mode: dnsrr
       mode: global
       placement:
@@ -118,38 +117,35 @@
       - 8081:8080
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
     deploy:
       placement:
         constraints: [node.role == manager]
 
-
   HAProxy:
     image: haproxytech/haproxy-debian:latest
     deploy:
       mode: global
       placement:
         constraints: [node.role == manager]
     ports:
       - 80:80
       - 8404:8404
     volumes:
       - "$DIR/haproxy.cfg:/usr/local/etc/haproxy/haproxy.cfg"
 
-
   CapacityAndStatsCollector:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     command: "python simplyblock_core/services/capacity_and_stats_collector.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
 
-
   CapacityMonitor:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     command: "python simplyblock_core/services/cap_monitor.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
@@ -178,15 +174,15 @@
     command: "python simplyblock_core/services/lvol_monitor.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
 
-
+  ### monitoring ###
   mongodb:
     image: "mongo:5.0"
     volumes:
       - "mongodb_data:/data/db"
     deploy:
       placement:
         constraints: [node.role == manager]
@@ -232,17 +228,73 @@
     volumes:
       - "graylog_data:/usr/share/graylog/data/data"
       - "graylog_journal:/usr/share/graylog/data/journal"
     deploy:
       placement:
         constraints: [node.role == manager]
 
+  promagent:
+    image: simplyblock/promagent
+    environment:
+      ClusterID: "${CLUSTER_ID}"
+      ClusterIP: "${CLUSTER_IP}"
+      ClusterSecret: "${CLUSTER_SECRET}"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  pushgateway:
+    image: prom/pushgateway
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  prometheus:
+    image: prom/prometheus:v2.44.0
+    user: root
+    volumes:
+      - ./prometheus.yml:/etc/prometheus/prometheus.yml
+      - prometheus_data:/prometheus
+    command:
+      - "--config.file=/etc/prometheus/prometheus.yml"
+      - "--storage.tsdb.path=/prometheus"
+    restart: "always"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  grafana:
+    image: grafana/grafana:10.0.12
+    environment:
+      GF_SECURITY_ADMIN_USER: "admin"
+      GF_SECURITY_ADMIN_PASSWORD: "${CLUSTER_SECRET}"
+      GF_ALERTING_ENABLED: "true"
+      GF_PATHS_PROVISIONING: "/etc/grafana/provisioning"
+    volumes:
+      - ./datasource.yml:/etc/grafana/provisioning/datasources/datasource.yaml
+      - grafana_data:/var/lib/grafana
+      - ./alerting:/etc/grafana/provisioning/alerting
+    restart: "always"
+    ports:
+      - target: 3000
+        published: 3000
+        protocol: tcp
+        mode: host
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  ### monitoring ###
+
 volumes:
   mongodb_data:
   os_data:
   graylog_data:
   graylog_journal:
+  grafana_data:
+  prometheus_data:
+  alertmanager_data:
 
 networks:
   hostnet:
     external: true
     name: host
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli-release-1.0.5/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 set -e
 trap "{ exit 1; }" TERM INT
 opt_h=0
 opt_l=""
 opt_r=0
 opt_s=5
-opt_t=240 # 4 min
+opt_t=600 # 10 min
 
 start_epoc=$(date +%s)
 cmd_min_timeout=15
 
 usage() {
   echo "$(basename $0) [opts] stack_name"
   echo "  -f filter: only wait for services matching filter, may be passed multiple"
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/scripts/haproxy.cfg` & `sbcli-release-1.0.5/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/scripts/__init__.py` & `sbcli-release-1.0.5/simplyblock_core/scripts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,18 +26,22 @@
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'install_deps.sh')])
 
 
 def configure_docker(docker_ip):
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'config_docker.sh'), docker_ip])
 
 
-def deploy_stack(cli_pass, dev_ip, image_name, graylog_password):
+def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id):
     pass_hash = hashlib.sha256(graylog_password.encode('utf-8')).hexdigest()
     return __run_script(
-        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash])
+        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id])
+
+def apply_dashboard(grafanaPassword):
+    return __run_script(
+        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'apply_dashboard.sh'), grafanaPassword])
 
 
 def deploy_cleaner():
     return __run_script(['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'clean_local_storage_deploy.sh')])
 
 
 def set_db_config(DEV_IP):
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/port_stat_collector.py` & `sbcli-release-1.0.5/simplyblock_core/services/port_stat_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import psutil
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.port_stat import PortStat
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 def update_port_stats(snode, nic, stats):
     now = int(time.time())
     data = {
         "uuid": nic.get_id(),
         "node_id": snode.get_id(),
         "date": now,
@@ -37,15 +39,17 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
 hostname = utils.get_hostname()
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/log_agg_service.py` & `sbcli-release-1.0.5/simplyblock_core/services/log_agg_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 import time
 import sys
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting Log aggregation service ...")
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli-release-1.0.5/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import time
 import sys
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 last_object_record = {}
 
 
 def add_device_stats(cl, device, capacity_dict, stats_dict):
     now = int(time.time())
     data = {
         "cluster_id": cl.get_id(),
         "uuid": device.get_id(),
         "date": now}
 
-    if capacity_dict['res'] == 1:
+    if capacity_dict and capacity_dict['res'] == 1:
         size_total = int(capacity_dict['npages_nmax']*capacity_dict['pba_page_size'])
         size_used = int(capacity_dict['npages_used']*capacity_dict['pba_page_size'])
         size_free = size_total - size_used
         size_util = 0
         if size_total > 0:
             size_util = int((size_used / size_total) * 100)
 
@@ -145,15 +147,17 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting capacity and stats collector...")
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/install_service.sh` & `sbcli-release-1.0.5/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/lvol_stat_collector.py` & `sbcli-release-1.0.5/simplyblock_core/services/lvol_stat_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import sys
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.stats import LVolStatObject, PoolStatObject
 from simplyblock_core.rpc_client import RPCClient
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 last_object_record = {}
 
 
 def add_lvol_stats(pool, lvol, stats_dict):
     now = int(time.time())
     data = {
@@ -86,15 +88,17 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/health_check_service.py` & `sbcli-release-1.0.5/simplyblock_core/services/health_check_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 # coding=utf-8
 import logging
-import os
 
 import time
 import sys
 from datetime import datetime
 
 
-from simplyblock_core.controllers import health_controller, storage_events
+from simplyblock_core.controllers import health_controller, storage_events, device_events
 from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core import constants, kv_store
 
-
-def set_node_status(snode, target_status):
-    if target_status == StorageNode.STATUS_ONLINE:
-        if snode.status == StorageNode.STATUS_ONLINE:
-            return
-    if target_status == StorageNode.STATUS_UNREACHABLE:
-        if snode.status == StorageNode.STATUS_UNREACHABLE:
-            return
-    snode = db_controller.get_storage_node_by_id(snode.get_id())
-    old_status = snode.status
-    snode.status = target_status
-    snode.updated_at = str(datetime.now())
-    snode.write_to_db(db_store)
-    storage_events.snode_status_change(snode, snode.status, old_status, caused_by="monitor")
-
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 def set_node_health_check(snode, health_check_status):
     snode = db_controller.get_storage_node_by_id(snode.get_id())
     if snode.health_check == health_check_status:
         return
     old_status = snode.health_check
     snode.health_check = health_check_status
@@ -46,33 +32,24 @@
     for node in nodes:
         if node.nvme_devices:
             for dev in node.nvme_devices:
                 if dev.get_id() == device.get_id():
                     old_status = dev.health_check
                     dev.health_check = health_check_status
                     node.write_to_db(db_store)
-                    storage_events.device_health_check_change(cluster_id, dev, dev.health_check, old_status, caused_by="monitor")
-
-
-def set_lvol_health_check(cluster_id, lvol, health_check_status):
-    lvol = db_controller.get_lvol_by_id(lvol.get_id())
-    if lvol.health_check == health_check_status:
-        return
-    old_status = lvol.health_check
-    lvol.health_check = health_check_status
-    lvol.updated_at = str(datetime.now())
-    lvol.write_to_db(db_store)
-    # todo: set lvol offline or online
-    storage_events.lvol_health_check_change(cluster_id, lvol, lvol.health_check, old_status, caused_by="monitor")
+                    device_events.device_health_check_change(
+                        dev, dev.health_check, old_status, caused_by="monitor")
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
 db_controller = kv_store.DBController()
 
@@ -84,69 +61,76 @@
         cluster_id = cl[0].get_id()
 
     snodes = db_controller.get_storage_nodes()
     if not snodes:
         logger.error("storage nodes list is empty")
 
     for snode in snodes:
-        logger.info("Node: %s", snode.get_id())
+        logger.info("Node: %s, status %s", snode.get_id(), snode.status)
+
+        if snode.status not in [StorageNode.STATUS_ONLINE, StorageNode.STATUS_UNREACHABLE]:
+            logger.info(f"Node status is: {snode.status}, skipping")
+            continue
 
         # 1- check node ping
         ping_check = health_controller._check_node_ping(snode.mgmt_ip)
         logger.info(f"Check: ping mgmt ip {snode.mgmt_ip} ... {ping_check}")
 
         # 2- check node API
         node_api_check = health_controller._check_node_api(snode.mgmt_ip)
         logger.info(f"Check: node API {snode.mgmt_ip}:5000 ... {node_api_check}")
 
+        if snode.status == StorageNode.STATUS_OFFLINE:
+            set_node_health_check(snode, ping_check & node_api_check)
+            continue
+
         # 3- check node RPC
         node_rpc_check = health_controller._check_node_rpc(
             snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
         logger.info(f"Check: node RPC {snode.mgmt_ip}:{snode.rpc_port} ... {node_rpc_check}")
 
         # 4- docker API
         node_docker_check = health_controller._check_node_docker_api(snode.mgmt_ip)
         logger.info(f"Check: node docker API {snode.mgmt_ip}:2375 ... {node_docker_check}")
 
         is_node_online = ping_check and node_api_check and node_rpc_check and node_docker_check
-        # if is_node_online:
-        #     set_node_status(snode, StorageNode.STATUS_ONLINE)
-        # else:
-        #     set_node_status(snode, StorageNode.STATUS_UNREACHABLE)
 
         health_check_status = is_node_online
         if not node_rpc_check:
             logger.info("Putting all devices to unavailable state because RPC check failed")
             for dev in snode.nvme_devices:
+                if dev.io_error:
+                    logger.debug(f"Skipping Device action because of io_error {dev.get_id()}")
+                    continue
                 set_device_health_check(cluster_id, dev, False)
         else:
             logger.info(f"Node device count: {len(snode.nvme_devices)}")
             node_devices_check = True
             node_remote_devices_check = True
 
             for dev in snode.nvme_devices:
+                if dev.io_error:
+                    logger.debug(f"Skipping Device check because of io_error {dev.get_id()}")
+                    continue
                 ret = health_controller.check_device(dev.get_id())
                 set_device_health_check(cluster_id, dev, ret)
-                node_devices_check &= ret
+                if dev.status == dev.STATUS_ONLINE:
+                    node_devices_check &= ret
 
             logger.info(f"Node remote device: {len(snode.remote_devices)}")
             rpc_client = RPCClient(
                 snode.mgmt_ip, snode.rpc_port,
                 snode.rpc_username, snode.rpc_password,
-                timeout=3, retry=1)
+                timeout=5, retry=3)
             for remote_device in snode.remote_devices:
                 ret = rpc_client.get_bdevs(remote_device.remote_bdev)
                 if ret:
                     logger.info(f"Checking bdev: {remote_device.remote_bdev} ... ok")
                 else:
                     logger.info(f"Checking bdev: {remote_device.remote_bdev} ... not found")
                 node_remote_devices_check &= bool(ret)
 
             health_check_status = is_node_online and node_devices_check and node_remote_devices_check
         set_node_health_check(snode, health_check_status)
 
-    for lvol in db_controller.get_lvols():
-        ret = health_controller.check_lvol(lvol.get_id())
-        set_lvol_health_check(cluster_id, lvol, ret)
-
     time.sleep(constants.HEALTH_CHECK_INTERVAL_SEC)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/device_monitor.py` & `sbcli-release-1.0.5/simplyblock_core/services/device_monitor.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,57 +2,67 @@
 import logging
 import os
 
 import time
 import sys
 
 
-from simplyblock_core import constants, kv_store
-from simplyblock_core.controllers import health_controller, storage_events
+from simplyblock_core import constants, kv_store, storage_node_ops
+from simplyblock_core.controllers import health_controller,  device_controller
 from simplyblock_core.models.nvme_device import NVMeDevice
+from simplyblock_core.models.storage_node import StorageNode
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 def set_dev_status(device, status):
-    if device.status != status:
-        nodes = db_controller.get_storage_nodes()
-        for node in nodes:
-            if node.nvme_devices:
-                for dev in node.nvme_devices:
-                    if dev.get_id() == device.get_id():
-                        old_status = dev.status
-                        dev.status = status
-                        node.write_to_db(db_store)
-                        storage_events.device_status_change(dev.cluster_id, dev,  dev.status, old_status)
-                        return
+    node = db_controller.get_storage_node_by_id(device.node_id)
+    if node.status != StorageNode.STATUS_ONLINE:
+        logger.error(f"Node is not online, {node.get_id()}, status: {node.status}, "
+                     f"skipping device status change")
+        return
+
+    for dev in node.nvme_devices:
+        if dev.get_id() == device.get_id():
+            if dev.status in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
+                device_controller.device_set_state(device.get_id(), status)
+            break
+    return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
 db_controller = kv_store.DBController()
 
 
 logger.info("Starting Device monitor...")
 while True:
-    devices = db_controller.get_storage_devices()
-    if not devices:
-        logger.error("devices list is empty")
-
-    for dev in devices:
-        if dev.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
-            logger.warning(f"Device status is not online or unavailable, id: {dev.get_id()}, status: {dev.status}")
+    nodes = db_controller.get_storage_nodes()
+    for node in nodes:
+        if node.status != StorageNode.STATUS_ONLINE:
+            logger.warning(f"Node status is not online, id: {node.get_id()}, status: {node.status}")
             continue
-
-        ret = health_controller.check_device(dev.get_id())
-        logger.info(f"Device: {dev.get_id()}, is healthy: {ret}")
-        if ret:
-            set_dev_status(dev, NVMeDevice.STATUS_ONLINE)
-        else:
-            set_dev_status(dev, NVMeDevice.STATUS_UNAVAILABLE)
+        for dev in node.nvme_devices:
+            if dev.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
+                logger.warning(f"Device status is not online or unavailable, id: {dev.get_id()}, status: {dev.status}")
+                continue
+            if dev.io_error:
+                logger.debug(f"Skipping Device check because of io_error {dev.get_id()}")
+                continue
+
+            ret = health_controller.check_device(dev.get_id())
+            logger.info(f"Device: {dev.get_id()}, is healthy: {ret}")
+            if ret:
+                set_dev_status(dev, NVMeDevice.STATUS_ONLINE)
+            else:
+                set_dev_status(dev, NVMeDevice.STATUS_UNAVAILABLE)
 
     time.sleep(constants.DEV_MONITOR_INTERVAL_SEC)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/caching_node_monitor.py` & `sbcli-release-1.0.5/simplyblock_core/services/caching_node_monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,23 @@
 from datetime import datetime
 
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.caching_node import CachingNode
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
+
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
 db_store = kv_store.KVStore()
 db_controller = kv_store.DBController(kv_store=db_store)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli-release-1.0.5/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,23 @@
 from datetime import datetime
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.controllers import mgmt_events
 from simplyblock_core.models.mgmt_node import MgmtNode
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
+
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
 db_store = kv_store.KVStore()
 db_controller = kv_store.DBController(kv_store=db_store)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/distr_event_collector.py` & `sbcli-release-1.0.5/simplyblock_core/services/distr_event_collector.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 import logging
 import os
 
 import time
 import sys
 
 
-from simplyblock_core import constants, kv_store, utils, rpc_client, storage_node_ops
-from simplyblock_core.controllers import events_controller, storage_events
+from simplyblock_core import constants, kv_store, utils, rpc_client
+from simplyblock_core.controllers import events_controller, device_controller, lvol_events
 from simplyblock_core.models.lvol_model import LVol
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
+
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
 
@@ -29,71 +34,82 @@
         nodes = db_controller.get_storage_nodes()
         device_id = None
         for node in nodes:
             for dev in node.nvme_devices:
                 if dev.cluster_device_order == storage_id:
                     if dev.status != "online":
                         logger.info(f"The storage device is not online, skipping. status: {dev.status}")
+                        event.status = 'skipped'
+                        return
+
+                    if node.get_id() != node_id:
+                        logger.info(f"The storage device is remote, skipping")
+                        event.status = 'skipped-remote'
                         return
-                    # if node.get_id() != node_id:
-                    #     logger.info(f"The storage device not on this node, skipping. device node: {node.get_id()}")
-                    #     return
+
                     device_id = dev.get_id()
                     break
 
-        if device_id:
-            if event.message == 'SPDK_BDEV_EVENT_REMOVE':
-                logger.info(f"Removing storage id: {storage_id} from node: {node_id}")
-                storage_node_ops.device_remove(device_id)
-            elif event.message == 'error_write':
-                logger.info(f"Setting device to read-only")
-                storage_node_ops.device_set_read_only(device_id)
-            event.status = 'processed'
-
-        else:
+        if not device_id:
             logger.info(f"Device not found!, storage id: {storage_id} from node: {node_id}")
             event.status = 'device_not_found'
-        event.write_to_db(db_controller.kv_store)
+            return
+
+        if event.message == 'SPDK_BDEV_EVENT_REMOVE':
+            logger.info(f"Removing storage id: {storage_id} from node: {node_id}")
+            device_controller.device_remove(device_id)
+        elif event.message == 'error_write':
+            logger.info(f"Setting device to read-only")
+            device_controller.device_set_read_only(device_id)
+            device_controller.device_set_io_error(device_id, True)
+        else:
+            logger.info(f"Setting device to unavailable")
+            device_controller.device_set_unavailable(device_id)
+            device_controller.device_set_io_error(device_id, True)
+
+        event.status = 'processed'
 
 
 def process_lvol_event(event):
     if event.message in ["error_open", 'error_read', "error_write", "error_unmap"]:
         vuid = event.object_dict['vuid']
         lvol = None
         for lv in db_controller.get_lvols():
             if lv.vuid == vuid:
                 lvol = lv
                 break
+
         if not lvol:
             logger.error(f"LVol with vuid {vuid} not found")
-            return
-
-        if lvol.status == LVol.STATUS_ONLINE:
-            logger.info("Setting LVol to offline")
-            old_status = lvol.status
-            lvol.status = LVol.STATUS_OFFLINE
-            lvol.write_to_db(db_controller.kv_store)
-            storage_events.lvol_status_change(event.cluster_uuid, lvol, lvol.status, old_status, caused_by="monitor")
-
-        event.status = 'processed'
-        event.write_to_db(db_controller.kv_store)
-
+            event.status = 'lvol_not_found'
+        else:
+            lvol.io_error = True
+            if lvol.status == LVol.STATUS_ONLINE:
+                logger.info("Setting LVol to offline")
+                old_status = lvol.status
+                lvol.status = LVol.STATUS_OFFLINE
+                lvol.write_to_db(db_controller.kv_store)
+                lvol_events.lvol_status_change(lvol, lvol.status, old_status, caused_by="monitor")
+            event.status = 'processed'
     else:
         logger.error(f"Unknown LVol event message: {event.message}")
+        event.status = "event_unknown"
 
 
 def process_event(event_id):
     event = db_controller.get_events(event_id)[0]
     if event.event == "device_status":
         if event.storage_id >= 0:
             process_device_event(event)
 
         if event.vuid >= 0:
             process_lvol_event(event)
 
+    event.write_to_db(db_controller.kv_store)
+
 
 hostname = utils.get_hostname()
 logger.info("Starting Distr event collector...")
 logger.info(f"Node:{hostname}")
 while True:
     time.sleep(constants.DISTR_EVENT_COLLECTOR_INTERVAL_SEC)
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/__init__.py` & `sbcli-release-1.0.5/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/capacity_collector.py` & `sbcli-release-1.0.5/simplyblock_core/services/capacity_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import sys
 import uuid
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.stats import CapacityStat
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 def add_cluster_stats(cl, records):
 
     if not records:
         return False
 
     size_total = 0
@@ -127,15 +129,17 @@
 
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting device capacity collector...")
```

## Comparing `sbcli-release-1.0.4/simplyblock_core/services/cap_monitor.py` & `sbcli-release-1.0.5/simplyblock_core/services/cap_monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # coding=utf-8
 import logging
-import os
 
 import time
 import sys
-import uuid
 
 
 
-from simplyblock_core import kv_store
+from simplyblock_core import kv_store, constants, cluster_ops
 from simplyblock_core.controllers import cluster_events
+from simplyblock_core.models.cluster import Cluster
 
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
+logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
+### script to test connection once connection is ascertain
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting capacity monitoring service...")
 while True:
     clusters = db_controller.get_clusters()
     for cl in clusters:
@@ -31,24 +35,33 @@
         if not records:
             logger.error("Cluster capacity record not found!")
             continue
 
         size_util = records[0].size_util
         size_prov = records[0].size_prov_util
         logger.debug(f"cluster abs util: {size_util}, prov util: {size_prov}")
+        if cl.cap_crit:
+            if cl.cap_crit < size_util:
+                logger.warning(f"Cluster absolute cap critical, util: {size_util}% of cluster util: {cl.cap_crit}, "
+                               f"putting the cluster in read_only mode")
+                cluster_events.cluster_cap_crit(cl, size_util)
+                cluster_ops.cluster_set_read_only(cl.get_id())
+            else:
+                if cl.status == Cluster.STATUS_READONLY:
+                    cluster_ops.cluster_set_active(cl.get_id())
+
+        if cl.cap_warn:
+            if cl.cap_warn < size_util < cl.cap_crit:
+                logger.warning(f"Cluster absolute cap warning, util: {size_util}% of cluster util: {cl.cap_warn}")
+                cluster_events.cluster_cap_warn(cl, size_util)
+
+        if cl.prov_cap_crit:
+            if cl.prov_cap_crit < size_prov:
+                logger.warning(f"Cluster provisioned cap critical, util: {size_prov}% of cluster util: {cl.prov_cap_crit}")
+                cluster_events.cluster_prov_cap_crit(cl, size_prov)
+
+        if cl.prov_cap_warn:
+            if cl.prov_cap_warn < size_prov < cl.prov_cap_crit:
+                logger.warning(f"Cluster provisioned cap warning, util: {size_prov}% of cluster util: {cl.prov_cap_warn}")
+                cluster_events.cluster_prov_cap_warn(cl, size_prov)
 
-        if cl.cap_crit and cl.cap_crit < size_util:
-            logger.warning(f"Cluster absolute cap critical, util: {size_util}% of cluster util: {cl.cap_crit}")
-            cluster_events.cluster_cap_crit(cl, size_util)
-        elif cl.cap_warn and cl.cap_warn < size_util:
-            logger.warning(f"Cluster absolute cap warning, util: {size_util}% of cluster util: {cl.cap_warn}")
-            cluster_events.cluster_cap_warn(cl, size_util)
-
-        if cl.prov_cap_crit and cl.prov_cap_crit < size_prov:
-            logger.warning(f"Cluster provisioned cap critical, util: {size_prov}% of cluster util: {cl.prov_cap_crit}")
-            cluster_events.cluster_prov_cap_crit(cl, size_prov)
-        elif cl.prov_cap_warn and cl.prov_cap_warn < size_prov:
-            logger.warning(f"Cluster provisioned cap warning, util: {size_prov}% of cluster util: {cl.prov_cap_warn}")
-            cluster_events.cluster_prov_cap_warn(cl, size_prov)
-
-    # time.sleep(constants.DEV_STAT_COLLECTOR_INTERVAL_SEC)
-    time.sleep(60)
+    time.sleep(constants.CAP_MONITOR_INTERVAL_SEC)
```

## Comparing `sbcli-release-1.0.4/sbcli_release.egg-info/PKG-INFO` & `sbcli-release-1.0.5/sbcli_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-release
-Version: 1.0.4
+Version: 1.0.5
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-release-1.0.4/sbcli_release.egg-info/SOURCES.txt` & `sbcli-release-1.0.5/sbcli_release.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,25 @@
 simplyblock_core/shell_utils.py
 simplyblock_core/snode_client.py
 simplyblock_core/storage_node_ops.py
 simplyblock_core/utils.py
 simplyblock_core/controllers/__init__.py
 simplyblock_core/controllers/caching_node_controller.py
 simplyblock_core/controllers/cluster_events.py
+simplyblock_core/controllers/device_controller.py
+simplyblock_core/controllers/device_events.py
 simplyblock_core/controllers/events_controller.py
 simplyblock_core/controllers/health_controller.py
 simplyblock_core/controllers/lvol_controller.py
+simplyblock_core/controllers/lvol_events.py
 simplyblock_core/controllers/mgmt_events.py
 simplyblock_core/controllers/pool_controller.py
+simplyblock_core/controllers/pool_events.py
 simplyblock_core/controllers/snapshot_controller.py
+simplyblock_core/controllers/snapshot_events.py
 simplyblock_core/controllers/storage_events.py
 simplyblock_core/models/__init__.py
 simplyblock_core/models/base_model.py
 simplyblock_core/models/caching_node.py
 simplyblock_core/models/cluster.py
 simplyblock_core/models/compute_node.py
 simplyblock_core/models/events.py
@@ -47,25 +52,34 @@
 simplyblock_core/models/nvme_device.py
 simplyblock_core/models/pool.py
 simplyblock_core/models/port_stat.py
 simplyblock_core/models/snapshot.py
 simplyblock_core/models/stats.py
 simplyblock_core/models/storage_node.py
 simplyblock_core/scripts/__init__.py
+simplyblock_core/scripts/apply_dashboard.sh
 simplyblock_core/scripts/clean_local_storage_deploy.sh
 simplyblock_core/scripts/config_docker.sh
+simplyblock_core/scripts/datasource.yml
 simplyblock_core/scripts/db_config_double.sh
 simplyblock_core/scripts/db_config_single.sh
 simplyblock_core/scripts/deploy_stack.sh
 simplyblock_core/scripts/docker-compose-swarm.yml
 simplyblock_core/scripts/haproxy.cfg
 simplyblock_core/scripts/install_deps.sh
+simplyblock_core/scripts/prometheus.yml
 simplyblock_core/scripts/run_ssh.sh
 simplyblock_core/scripts/set_db_config.sh
 simplyblock_core/scripts/stack_deploy_wait.sh
+simplyblock_core/scripts/alerting/alert_resources.yaml
+simplyblock_core/scripts/alerting/alert_rules.yaml
+simplyblock_core/scripts/dashboards/cluster.json
+simplyblock_core/scripts/dashboards/devices.json
+simplyblock_core/scripts/dashboards/lvols.json
+simplyblock_core/scripts/dashboards/nodes.json
 simplyblock_core/services/__init__.py
 simplyblock_core/services/caching_node_monitor.py
 simplyblock_core/services/cap_monitor.py
 simplyblock_core/services/capacity_and_stats_collector.py
 simplyblock_core/services/capacity_collector.py
 simplyblock_core/services/device_monitor.py
 simplyblock_core/services/distr_event_collector.py
```

## Comparing `sbcli-release-1.0.4/simplyblock_cli/cli.py` & `sbcli-release-1.0.5/simplyblock_cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from simplyblock_core import cluster_ops, utils
 from simplyblock_core import kv_store
 from simplyblock_core import compute_node_ops as compute_ops
 from simplyblock_core import storage_node_ops as storage_ops
 from simplyblock_core import mgmt_node_ops as mgmt_ops
 from simplyblock_core import constants
-from simplyblock_core.controllers import pool_controller, lvol_controller, snapshot_controller
+from simplyblock_core.controllers import pool_controller, lvol_controller, snapshot_controller, device_controller
 from simplyblock_core.controllers import caching_node_controller, health_controller
 from simplyblock_core.models.pool import Pool
 
 
 class CLIWrapper:
 
     def __init__(self):
@@ -43,48 +43,56 @@
         sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G', dest='spdk_mem')
         sub_command.add_argument("--dev-split", help='Split nvme devices by this factor, can be 2 or more',
                                  dest='dev_split', type=int, default=1)
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
-        sub_command.add_argument("--spdk-cmd-params", help='Extra params for SPDK app command', nargs='+', dest='cmd_params')
+        sub_command.add_argument("--spdk-debug", help='Enable spdk debug logs', dest='spdk_debug', required=False, action='store_true')
 
-        sub_command.add_argument("--bdev_io_pool_size", help='bdev_set_options param', dest='bdev_io_pool_size',  type=int, default=0)
-        sub_command.add_argument("--bdev_io_cache_size", help='bdev_set_options param', dest='bdev_io_cache_size',  type=int, default=0)
-        sub_command.add_argument("--iobuf_small_cache_size", help='bdev_set_options param', dest='iobuf_small_cache_size',  type=int, default=0)
-        sub_command.add_argument("--iobuf_large_cache_size", help='bdev_set_options param', dest='iobuf_large_cache_size',  type=int, default=0)
+        sub_command.add_argument("--iobuf_small_pool_count", help='bdev_set_options param', dest='small_pool_count',  type=int, default=0)
+        sub_command.add_argument("--iobuf_large_pool_count", help='bdev_set_options param', dest='large_pool_count',  type=int, default=0)
+        sub_command.add_argument("--iobuf_small_bufsize", help='bdev_set_options param', dest='small_bufsize',  type=int, default=0)
+        sub_command.add_argument("--iobuf_large_bufsize", help='bdev_set_options param', dest='large_bufsize',  type=int, default=0)
 
         # remove storage node
         sub_command = self.add_sub_command(subparser, "remove", 'Remove storage node')
         sub_command.add_argument("node_id", help='UUID of storage node')
         sub_command.add_argument("--force-remove", help='Force remove all LVols and snapshots',
                                  dest='force_remove', required=False, action='store_true')
         sub_command.add_argument("--force-migrate", help='Force migrate All LVols to other nodes',
                                  dest='force_migrate', required=False, action='store_true')
         # List all storage nodes
         sub_command = self.add_sub_command(subparser, "list", 'List storage nodes')
         sub_command.add_argument("--cluster-id", help='id of the cluster for which nodes are listed')
         sub_command.add_argument("--json", help='Print outputs in json format', action='store_true')
 
+        sub_command = self.add_sub_command(subparser, "get", 'Get storage node info')
+        sub_command.add_argument("id", help='UUID of storage node')
+
+        sub_command = self.add_sub_command(subparser, "update", 'Update storage node db info')
+        sub_command.add_argument("id", help='UUID of storage node')
+        sub_command.add_argument("key", help='Key')
+        sub_command.add_argument("value", help='Value')
+
         # Restart storage node
         sub_command = self.add_sub_command(
             subparser, "restart", 'Restart a storage node. All functions and device drivers will be reset. '
                                   'During restart, the node does not accept IO. In a high-availability setup, '
                                   'this will not impact operations.')
         sub_command.add_argument("node_id", help='UUID of storage node')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found', dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G', dest='spdk_mem')
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
-        sub_command.add_argument("--spdk-cmd-params", help='Extra params for SPDK app command', nargs='+', dest='cmd_params')
+        sub_command.add_argument("--spdk-debug", help='Enable spdk debug logs', dest='spdk_debug', required=False, action='store_true')
 
-        sub_command.add_argument("--bdev_io_pool_size", help='bdev_set_options param', dest='bdev_io_pool_size',  type=int, default=0)
-        sub_command.add_argument("--bdev_io_cache_size", help='bdev_set_options param', dest='bdev_io_cache_size',  type=int, default=0)
-        sub_command.add_argument("--iobuf_small_cache_size", help='bdev_set_options param', dest='iobuf_small_cache_size',  type=int, default=0)
-        sub_command.add_argument("--iobuf_large_cache_size", help='bdev_set_options param', dest='iobuf_large_cache_size',  type=int, default=0)
+        sub_command.add_argument("--iobuf_small_pool_count", help='bdev_set_options param', dest='small_pool_count',  type=int, default=0)
+        sub_command.add_argument("--iobuf_large_pool_count", help='bdev_set_options param', dest='large_pool_count',  type=int, default=0)
+        sub_command.add_argument("--iobuf_small_bufsize", help='bdev_set_options param', dest='small_bufsize',  type=int, default=0)
+        sub_command.add_argument("--iobuf_large_bufsize", help='bdev_set_options param', dest='large_bufsize',  type=int, default=0)
 
         # sub_command.add_argument("-t", '--test', help='Run smart test on the NVMe devices', action='store_true')
 
         # Shutdown storage node
         sub_command = self.add_sub_command(
             subparser, "shutdown", 'Shutdown a storage node. Once the command is issued, the node will stop accepting '
                                    'IO,but IO, which was previously received, will still be processed. '
@@ -165,14 +173,15 @@
 
         sub_command = self.add_sub_command(
             subparser, 'remove-device', 'Remove a storage device. The device will become unavailable, independently '
                                         'if it was physically removed from the server. This function can be used if '
                                         'auto-detection of removal did not work or if the device must be maintained '
                                         'otherwise while remaining inserted into the server. ')
         sub_command.add_argument("device_id", help='Storage device ID')
+        sub_command.add_argument("--force", help='Force device remove', required=False, action='store_true')
 
         sub_command = self.add_sub_command(subparser, 'set-ro-device', 'Set storage device read only')
         sub_command.add_argument("device_id", help='Storage device ID')
 
         sub_command = self.add_sub_command(
             subparser, 'set-failed-device', 'Set storage device to failed state. This command can be used, '
                                             'if an administrator believes that the device must be changed, '
@@ -251,14 +260,18 @@
         sub_command = self.add_sub_command(subparser, "check-device", 'Health check device')
         sub_command.add_argument("id", help='device UUID')
 
         # node info
         sub_command = self.add_sub_command(subparser, "info", 'Get node information')
         sub_command.add_argument("id", help='Node UUID')
 
+        # node info-spdk
+        sub_command = self.add_sub_command(subparser, "info-spdk", 'Get SPDK memory information')
+        sub_command.add_argument("id", help='Node UUID')
+
         # Initialize cluster parser
         subparser = self.add_command('cluster', 'Cluster commands')
 
         sub_command = self.add_sub_command(subparser, 'create',
                                            'Create an new cluster with this node as mgmt (local run)')
         sub_command.add_argument(
             "--blk_size", help='The block size in bytes', type=int, choices=[512, 4096], default=512)
@@ -307,14 +320,18 @@
         # sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G',  dest='spdk_mem')
 
         # show cluster info
         sub_command = self.add_sub_command(
             subparser, 'status', 'Show cluster status')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
 
+        # show cluster info
+        sub_command = self.add_sub_command(subparser, 'get', 'Show cluster info')
+        sub_command.add_argument("id", help='the cluster UUID')
+
         sub_command = self.add_sub_command(
             subparser, 'suspend', 'Suspend cluster. The cluster will stop processing all IO. '
                                   'Attention! This will cause an "all paths down" event for nvmeof/iscsi volumes '
                                   'on all hosts connected to the cluster.')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
 
         sub_command = self.add_sub_command(
@@ -355,14 +372,15 @@
         sub_command.add_argument("host-nqn", help='NQN of the host to remove from the allowed hosts list')
 
         sub_command = self.add_sub_command(
             subparser, 'get-capacity', 'Returns the current total available capacity, utilized capacity '
                                        '(in percent and absolute) and provisioned capacity (in percent and absolute) '
                                        'in GB in the cluster.')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
+        sub_command.add_argument("--json", help='Print json output', required=False, action='store_true')
         sub_command.add_argument("--history", help='(XXdYYh), list history records (one for every 15 minutes) '
                                                    'for XX days and YY hours (up to 10 days in total).')
 
         sub_command = self.add_sub_command(
             subparser, 'get-io-stats', 'Returns the io statistics. If --history is not selected, this is a monitor, '
                                        'which updates current statistics records every two seconds '
                                        '(similar to ping):read-iops write-iops total-iops read-mbs write-mbs total-mbs')
@@ -401,22 +419,29 @@
         sub_command.add_argument("cluster_id", help='cluster uuid')
         sub_command.add_argument("secret", help='new 20 characters password')
 
         # check cluster
         sub_command = self.add_sub_command(subparser, "check", 'Health check cluster')
         sub_command.add_argument("id", help='cluster UUID')
 
+        # update cluster
+        sub_command = self.add_sub_command(subparser, "update", 'Update cluster mgmt services')
+        sub_command.add_argument("id", help='cluster UUID')
+
         # lvol ops
         subparser = self.add_command('lvol', 'LVol commands')
         # add lvol
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new logical volume')
         sub_command.add_argument("name", help='LVol name or id')
         sub_command.add_argument("size", help='LVol size: 10M, 10G, 10(bytes)')
         sub_command.add_argument("pool", help='Pool UUID or name')
-        sub_command.add_argument("--host_id", help='Primary storage node UUID or Hostname')
+        sub_command.add_argument("--snapshot", "-s", help='Make LVol with snapshot capability, default is False',
+                                 required=False, action='store_true')
+        sub_command.add_argument("--max-size", help='LVol max size', dest='max_size', default="0")
+        sub_command.add_argument("--host-id", help='Primary storage node UUID or Hostname', dest='host_id')
         sub_command.add_argument("--ha-type", help='LVol HA type (single, ha), default is cluster HA type',
                                  dest='ha_type', choices=["single", "ha", "default"], default='default')
 
         sub_command.add_argument("--compress",
                                  help='Use inline data compression and de-compression on the logical volume',
                                  required=False, action='store_true')
         sub_command.add_argument("--encrypt", help='Use inline data encryption and de-cryption on the logical volume',
@@ -450,17 +475,21 @@
         sub_command.add_argument("--max-r-mbytes", help='Maximum Read Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-w-mbytes", help='Maximum Write Mega Bytes Per Second', type=int)
 
         # list lvols
         sub_command = self.add_sub_command(subparser, 'list', 'List all LVols')
         sub_command.add_argument("--cluster-id", help='List LVols in particular cluster')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
+        # list lvols
+        sub_command = self.add_sub_command(subparser, 'list-mem', 'List all LVols')
+        sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
+        sub_command.add_argument("--csv", help='Print outputs in csv format', required=False, action='store_true')
         # get lvol
         sub_command = self.add_sub_command(subparser, 'get', 'Get LVol details')
-        sub_command.add_argument("id", help='LVol id')
+        sub_command.add_argument("id", help='LVol id or name')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
         # delete lvol
         sub_command = self.add_sub_command(
             subparser, 'delete', 'Delete LVol. This is only possible, if no more snapshots and non-inflated clones '
                                  'of the volume exist. The volume must be suspended before it can be deleted. ')
         sub_command.add_argument("id", help='LVol id or ids', nargs='+')
         sub_command.add_argument("--force", help='Force delete LVol from the cluster', required=False,
@@ -509,18 +538,19 @@
         # lvol clone
         sub_command = self.add_sub_command(subparser, 'clone', 'create LVol based on a snapshot')
         sub_command.add_argument("snapshot_id", help='snapshot UUID')
         sub_command.add_argument("clone_name", help='clone name')
 
         # lvol move
         sub_command = self.add_sub_command(
-            subparser, 'move', 'Moves a full copy of the logical volume between clusters')
-        sub_command.add_argument("id", help='LVol id')
-        sub_command.add_argument("cluster-id", help='Destination Cluster ID')
-        sub_command.add_argument("node-id", help='Destination Node ID')
+            subparser, 'move', 'Moves a full copy of the logical volume between nodes')
+        sub_command.add_argument("id", help='LVol UUID')
+        # sub_command.add_argument("cluster-id", help='Destination Cluster ID')
+        sub_command.add_argument("node_id", help='Destination Node UUID')
+        sub_command.add_argument("--force", help='Force LVol delete from source node', required=False, action='store_true')
 
         # lvol replicate
         sub_command = self.add_sub_command(
             subparser, 'replicate', 'Create a replication path between two volumes in two clusters')
         sub_command.add_argument("id", help='LVol id')
         sub_command.add_argument("cluster-a", help='A Cluster ID')
         sub_command.add_argument("cluster-b", help='B Cluster ID')
@@ -719,14 +749,16 @@
     def add_sub_command(self, parent_parser, command, help):
         return parent_parser.add_parser(command, description=help, help=help)
 
     def run(self):
         args = self.parser.parse_args()
         if args.debug:
             self.logger.setLevel(logging.DEBUG)
+        else:
+            self.logger.setLevel(constants.LOG_LEVEL)
         logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
 
         args_dict = args.__dict__
         ret = ""
         if args.command in ['storage-node', 'sn']:
             sub_command = args_dict['storage-node']
 
@@ -746,20 +778,20 @@
             elif sub_command == "add-node":
                 cluster_id = args.cluster_id
                 node_ip = args.node_ip
                 ifname = args.ifname
                 data_nics = args.data_nics
                 dev_split = args.dev_split
                 spdk_image = args.spdk_image
-                cmd_params = args.cmd_params
+                spdk_debug = args.spdk_debug
 
-                bdev_io_pool_size = args.bdev_io_pool_size
-                bdev_io_cache_size = args.bdev_io_cache_size
-                iobuf_small_cache_size = args.iobuf_small_cache_size
-                iobuf_large_cache_size = args.iobuf_large_cache_size
+                small_pool_count = args.small_pool_count
+                large_pool_count = args.large_pool_count
+                small_bufsize = args.small_bufsize
+                large_bufsize = args.large_bufsize
 
                 spdk_cpu_mask = None
                 if args.spdk_cpu_mask:
                     if self.validate_cpu_mask(args.spdk_cpu_mask):
                         spdk_cpu_mask = args.spdk_cpu_mask
                     else:
                         return f"Invalid cpu mask value: {args.spdk_cpu_mask}"
@@ -767,29 +799,29 @@
                 spdk_mem = None
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 out = storage_ops.add_node(
-                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, dev_split, spdk_image, cmd_params,
-                bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size)
+                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, dev_split, spdk_image, spdk_debug,
+                    small_pool_count, large_pool_count, small_bufsize, large_bufsize)
                 return out
 
             elif sub_command == "list":
                 ret = storage_ops.list_storage_nodes(self.db_store, args.json)
 
             elif sub_command == "remove":
                 ret = storage_ops.remove_storage_node(args.node_id, args.force_remove, args.force_migrate)
 
             elif sub_command == "restart":
                 node_id = args.node_id
 
                 spdk_image = args.spdk_image
-                cmd_params = args.cmd_params
+                spdk_debug = args.spdk_debug
 
                 cpu_mask = None
                 if args.spdk_cpu_mask:
                     if self.validate_cpu_mask(args.spdk_cpu_mask):
                         cpu_mask = args.spdk_cpu_mask
                     else:
                         return f"Invalid cpu mask value: {args.spdk_cpu_mask}"
@@ -797,50 +829,50 @@
                 spdk_mem = None
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
 
-                bdev_io_pool_size = args.bdev_io_pool_size
-                bdev_io_cache_size = args.bdev_io_cache_size
-                iobuf_small_cache_size = args.iobuf_small_cache_size
-                iobuf_large_cache_size = args.iobuf_large_cache_size
+                small_pool_count = args.small_pool_count
+                large_pool_count = args.large_pool_count
+                small_bufsize = args.small_bufsize
+                large_bufsize = args.large_bufsize
 
                 ret = storage_ops.restart_storage_node(
                     node_id, cpu_mask, spdk_mem,
-                    spdk_image, cmd_params,
-                    bdev_io_pool_size, bdev_io_cache_size,
-                    iobuf_small_cache_size, iobuf_large_cache_size)
+                    spdk_image, spdk_debug,
+                    small_pool_count, large_pool_count,
+                    small_bufsize, large_bufsize)
 
             elif sub_command == "list-devices":
                 ret = self.storage_node_list_devices(args)
 
             elif sub_command == "device-testing-mode":
-                ret = storage_ops.set_device_testing_mode(args.device_id, args.mode)
+                ret = device_controller.set_device_testing_mode(args.device_id, args.mode)
 
             elif sub_command == "remove-device":
-                ret = storage_ops.device_remove(args.device_id)
+                ret = device_controller.device_remove(args.device_id, args.force)
 
             elif sub_command == "shutdown":
                 # answer = self.query_yes_no("Are you sure?", default=None)
                 # if answer is True:
                 ret = storage_ops.shutdown_storage_node(args.node_id, args.force)
 
             elif sub_command == "suspend":
                 ret = storage_ops.suspend_storage_node(args.node_id, args.force)
 
             elif sub_command == "resume":
                 ret = storage_ops.resume_storage_node(args.node_id)
 
             elif sub_command == "reset-device":
-                ret = storage_ops.reset_storage_device(args.device_id)
+                ret = device_controller.reset_storage_device(args.device_id)
 
             elif sub_command == "restart-device":
-                ret = storage_ops.restart_device(args.id)
+                ret = device_controller.restart_device(args.id)
 
             elif sub_command == "run-smart":
                 dev_name = args.name
                 ret = storage_ops.run_test_storage_device(self.db_store, dev_name)
 
             elif sub_command == "add-device":
                 dev_name = args.name
@@ -852,27 +884,27 @@
                 old_node_name = args.name
                 ifname = args.ifname
                 ret = storage_ops.replace_node(self.db_store, old_node_name, ifname)
 
             elif sub_command == "get-capacity-device":
                 device_id = args.device_id
                 history = args.history
-                data = storage_ops.get_device_capacity(device_id, history)
+                data = device_controller.get_device_capacity(device_id, history)
                 if data:
                     ret = utils.print_table(data)
                 else:
                     return False
             elif sub_command == "get-device":
                 device_id = args.device_id
-                ret = storage_ops.get_device(device_id)
+                ret = device_controller.get_device(device_id)
 
             elif sub_command == "get-io-stats-device":
                 device_id = args.device_id
                 history = args.history
-                data = storage_ops.get_device_iostats(device_id, history)
+                data = device_controller.get_device_iostats(device_id, history)
                 if data:
                     ret = utils.print_table(data)
                 else:
                     return False
             elif sub_command == "get-capacity":
                 node_id = args.node_id
                 history = args.history
@@ -917,14 +949,24 @@
                 device_id = args.id
                 ret = health_controller.check_device(device_id)
 
             elif sub_command == "info":
                 node_id = args.id
                 ret = storage_ops.get_info(node_id)
 
+            elif sub_command == "info-spdk":
+                node_id = args.id
+                ret = storage_ops.get_spdk_info(node_id)
+
+            elif sub_command == "update":
+                ret = storage_ops.update(args.id, args.key, args.value)
+
+            elif sub_command == "get":
+                ret = storage_ops.get(args.id)
+
             else:
                 self.parser.print_help()
 
         elif args.command == 'cluster':
             sub_command = args_dict[args.command]
             if sub_command in ["add-dev-model", "rm-dev-model", "add-host-auth",
                                "rm-host-auth", "set-log-level"]:
@@ -945,19 +987,20 @@
                 ret = cluster_ops.suspend_cluster(cluster_id)
             elif sub_command == 'unsuspend':
                 cluster_id = args.cluster_id
                 ret = cluster_ops.unsuspend_cluster(cluster_id)
             elif sub_command == "get-capacity":
                 cluster_id = args.cluster_id
                 history = args.history
-                data = cluster_ops.get_capacity(cluster_id, history)
-                if data:
-                    ret = utils.print_table(data)
+                is_json = args.json
+                data = cluster_ops.get_capacity(cluster_id, history, is_json=is_json)
+                if is_json:
+                    ret = data
                 else:
-                    return False
+                    ret = utils.print_table(data)
 
             elif sub_command == "get-io-stats":
                 data = cluster_ops.get_iostats_history(args.cluster_id, args.history, args.records)
                 if data:
                     ret = utils.print_table(data)
                 else:
                     return False
@@ -973,14 +1016,18 @@
                 ret = cluster_ops.set_secret(cluster_id, secret)
             elif sub_command == "get-logs":
                 cluster_id = args.cluster_id
                 ret = cluster_ops.get_logs(cluster_id)
             elif sub_command == "check":
                 cluster_id = args.id
                 ret = health_controller.check_cluster(cluster_id)
+            elif sub_command == "get":
+                ret = cluster_ops.get_cluster(args.id)
+            elif sub_command == "update":
+                ret = cluster_ops.update_cluster(args.id)
             else:
                 self.parser.print_help()
 
         elif args.command == 'compute-node':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 ret = compute_ops.add_compute_node(self.db_store)
@@ -1000,45 +1047,51 @@
                 self.parser.print_help()
 
         elif args.command == 'lvol':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 name = args.name
                 size = self.parse_size(args.size)
+                max_size = self.parse_size(args.max_size)
                 host_id = args.host_id
                 ha_type = args.ha_type
                 pool = args.pool
                 comp = args.compress
                 crypto = args.encrypt
                 distr_vuid = args.distr_vuid
                 distr_ndcs = args.distr_ndcs
                 distr_npcs = args.distr_npcs
                 distr_bs = args.distr_bs
                 distr_chunk_bs = args.distr_chunk_bs
+                with_snapshot = args.snapshot
                 results, error = lvol_controller.add_lvol_ha(
                     name, size, host_id, ha_type, pool, comp, crypto,
                     distr_vuid, distr_ndcs, distr_npcs,
                     args.max_rw_iops,
                     args.max_rw_mbytes,
                     args.max_r_mbytes,
                     args.max_w_mbytes,
                     distr_bs,
-                    distr_chunk_bs)
+                    distr_chunk_bs,
+                    with_snapshot=with_snapshot,
+                    max_size=max_size)
                 if results:
                     ret = results
                 else:
                     ret = error
             elif sub_command == "add-distr":
                 pass
             elif sub_command == "qos-set":
                 ret = lvol_controller.set_lvol(
                     args.id, args.max_rw_iops, args.max_rw_mbytes,
                     args.max_r_mbytes, args.max_w_mbytes)
             elif sub_command == "list":
                 ret = lvol_controller.list_lvols(args.json)
+            elif sub_command == "list-mem":
+                ret = lvol_controller.list_lvols_mem(args.json, args.csv)
             elif sub_command == "get":
                 ret = lvol_controller.get_lvol(args.id, args.json)
             elif sub_command == "delete":
                 for id in args.id:
                     force = args.force
                     ret = lvol_controller.delete_lvol(id, force)
             elif sub_command == "connect":
@@ -1079,14 +1132,16 @@
                 ret = lvol_controller.send_cluster_map(id)
             elif sub_command == "get-cluster-map":
                 id = args.id
                 ret = lvol_controller.get_cluster_map(id)
             elif sub_command == "check":
                 id = args.id
                 ret = health_controller.check_lvol(id)
+            elif sub_command == 'move':
+                ret = lvol_controller.move(args.id, args.node_id, args.force)
             else:
                 self.parser.print_help()
 
         elif args.command == 'mgmt':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 cluster_id = args.cluster_id
```

