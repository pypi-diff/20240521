# Comparing `tmp/sbcli_dev-2.6.6.zip` & `tmp/sbcli_dev-2.6.7.zip`

## zipinfo {}

```diff
@@ -1,148 +1,148 @@
-Zip file size: 213395 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/
--rw-r--r--  2.0 unx     1068 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/pyproject.toml
--rw-r--r--  2.0 unx     1489 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/PKG-INFO
--rw-r--r--  2.0 unx      148 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/env_var
--rw-r--r--  2.0 unx       38 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/setup.cfg
--rw-r--r--  2.0 unx     2269 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/setup.py
--rw-r--r--  2.0 unx    78538 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/templates/
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/app.py
--rw-r--r--  2.0 unx      725 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     8685 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     9713 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    12198 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     6209 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5547 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5188 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       73 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx       55 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/sbcli_dev.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/
--rw-r--r--  2.0 unx    24741 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8343 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21965 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx    66443 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1501 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx      837 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4118 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5268 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx    48950 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    13877 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    23245 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/models/port_stat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx     1420 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      118 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     5333 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      152 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/set_db_config.sh
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx      311 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      930 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       54 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx      453 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    88820 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    88911 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    88776 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    88868 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-21 00:22 sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/node-exporter.json
-146 files, 1881984 bytes uncompressed, 186817 bytes compressed:  90.1%
+Zip file size: 213603 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/pyproject.toml
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/PKG-INFO
+-rw-r--r--  2.0 unx      148 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/setup.py
+-rw-r--r--  2.0 unx    78538 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8685 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9713 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     6209 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5746 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5188 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/sbcli_dev.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    24741 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8343 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21965 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    66443 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1501 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    48950 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13877 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23245 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5333 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    88820 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    88911 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    88776 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    88868 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-21 16:53 sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/node-exporter.json
+146 files, 1882370 bytes uncompressed, 187025 bytes compressed:  90.1%
```

## zipnote {}

```diff
@@ -1,439 +1,439 @@
-Filename: sbcli_dev-2.6.6/
+Filename: sbcli_dev-2.6.7/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_cli/
+Filename: sbcli_dev-2.6.7/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/
+Filename: sbcli_dev-2.6.7/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/
+Filename: sbcli_dev-2.6.7/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/README.md
+Filename: sbcli_dev-2.6.7/README.md
 Comment: 
 
-Filename: sbcli_dev-2.6.6/pyproject.toml
+Filename: sbcli_dev-2.6.7/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/PKG-INFO
+Filename: sbcli_dev-2.6.7/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.6.6/env_var
+Filename: sbcli_dev-2.6.7/env_var
 Comment: 
 
-Filename: sbcli_dev-2.6.6/setup.cfg
+Filename: sbcli_dev-2.6.7/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.6.6/setup.py
+Filename: sbcli_dev-2.6.7/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.6.7/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_cli/main.py
+Filename: sbcli_dev-2.6.7/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/templates/
+Filename: sbcli_dev-2.6.7/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/utils.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/app.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.6.7/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.6/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.6.7/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/utils.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/constants.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.6.6/README.md` & `sbcli_dev-2.6.7/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/PKG-INFO` & `sbcli_dev-2.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.6.6
+Version: 2.6.7
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.6.6/setup.py` & `sbcli_dev-2.6.7/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_cli/cli.py` & `sbcli_dev-2.6.7/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/node_webapp.py` & `sbcli_dev-2.6.7/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/snode_app.py` & `sbcli_dev-2.6.7/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.6.7/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.6.7/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/node_utils.py` & `sbcli_dev-2.6.7/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/utils.py` & `sbcli_dev-2.6.7/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/app.py` & `sbcli_dev-2.6.7/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.6.7/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/static/delete.py` & `sbcli_dev-2.6.7/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.6.7/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/static/deploy.py` & `sbcli_dev-2.6.7/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 from simplyblock_core import scripts, constants
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("caching_node", __name__, url_prefix="/cnode")
 
 
+def get_docker_client():
+    ip = os.getenv("DOCKER_IP")
+    if not ip:
+        for ifname in node_utils.get_nics_data():
+            if ifname in ["eth0", "ens0"]:
+                ip = node_utils.get_nics_data()[ifname]['ip']
+                break
+    return docker.DockerClient(base_url=f"tcp://{ip}:2375", version="auto", timeout=60 * 5)
+
+
 def run_command(cmd):
     process = subprocess.Popen(
         cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = process.communicate()
     return stdout.strip().decode("utf-8"), stderr.strip(), process.returncode
 
 
@@ -150,15 +160,15 @@
         spdk_cpu_mask = hex(int(math.pow(2, node_cpu_count)) - 1)
 
     if spdk_mem:
         spdk_mem = int(spdk_mem / (1024 * 1024))
     else:
         spdk_mem = 64096
 
-    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    node_docker = get_docker_client()
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
         if node.attrs["Name"] in ["/spdk", "/spdk_proxy"]:
             logger.info(f"{node.attrs['Name']} container found, removing...")
             node.stop()
             node.remove(force=True)
             time.sleep(2)
@@ -224,26 +234,26 @@
     return utils.get_response(
         False, f"Container create max retries reached, Container status: {status}, Is Running: {is_running}")
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
     force = request.args.get('force', default=False, type=bool)
-    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    node_docker = get_docker_client()
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk" or cont.attrs['Name'] == "/spdk_proxy":
             cont.stop()
             cont.remove(force=force)
     return utils.get_response(True)
 
 
 @bp.route('/spdk_process_is_up', methods=['GET'])
 def spdk_process_is_up():
-    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    node_docker = get_docker_client()
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk":
             status = cont.attrs['State']["Status"]
             is_running = cont.attrs['State']["Running"]
             if is_running:
                 return utils.get_response(True)
@@ -313,15 +323,15 @@
     data = request.get_json()
     db_connection = data['db_connection']
 
     logger.info("Setting DB connection")
     ret = scripts.set_db_config(db_connection)
 
     try:
-        node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+        node_docker = get_docker_client()
         nodes = node_docker.containers.list(all=True)
         for node in nodes:
             if node.attrs["Name"] == "/spdk_proxy":
                 node_docker.containers.get(node.attrs["Id"]).restart()
                 break
     except:
         pass
```

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,22 +6,32 @@
 import time
 
 import docker
 from docker.types import LogConfig
 from flask import Blueprint
 from flask import request
 
-from simplyblock_web import utils
+from simplyblock_web import utils, node_utils
 from simplyblock_core import scripts, constants
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("node_api_caching_docker", __name__, url_prefix="/cnode")
 
 
+def get_docker_client():
+    ip = os.getenv("DOCKER_IP")
+    if not ip:
+        for ifname in node_utils.get_nics_data():
+            if ifname in ["eth0", "ens0"]:
+                ip = node_utils.get_nics_data()[ifname]['ip']
+                break
+    return docker.DockerClient(base_url=f"tcp://{ip}:2375", version="auto", timeout=60 * 5)
+
+
 @bp.route('/spdk_process_start', methods=['POST'])
 def spdk_process_start():
     data = request.get_json()
 
     spdk_cpu_mask = None
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
@@ -41,15 +51,15 @@
         spdk_cpu_mask = hex(int(math.pow(2, node_cpu_count)) - 1)
 
     if spdk_mem:
         spdk_mem = int(spdk_mem / (1024 * 1024))
     else:
         spdk_mem = 64096
 
-    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    node_docker = get_docker_client()
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
         if node.attrs["Name"] in ["/spdk", "/spdk_proxy"]:
             logger.info(f"{node.attrs['Name']} container found, removing...")
             node.stop()
             node.remove(force=True)
             time.sleep(2)
@@ -115,26 +125,26 @@
     return utils.get_response(
         False, f"Container create max retries reached, Container status: {status}, Is Running: {is_running}")
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
     force = request.args.get('force', default=False, type=bool)
-    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    node_docker = get_docker_client()
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk" or cont.attrs['Name'] == "/spdk_proxy":
             cont.stop()
             cont.remove(force=force)
     return utils.get_response(True)
 
 
 @bp.route('/spdk_process_is_up', methods=['GET'])
 def spdk_process_is_up():
-    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    node_docker = get_docker_client()
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk":
             status = cont.attrs['State']["Status"]
             is_running = cont.attrs['State']["Running"]
             if is_running:
                 return utils.get_response(True)
@@ -148,15 +158,15 @@
     data = request.get_json()
     db_connection = data['db_connection']
 
     logger.info("Setting DB connection")
     ret = scripts.set_db_config(db_connection)
 
     try:
-        node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
+        node_docker = get_docker_client()
         nodes = node_docker.containers.list(all=True)
         for node in nodes:
             if node.attrs["Name"] == "/spdk_proxy":
                 node_docker.containers.get(node.attrs["Id"]).restart()
                 break
     except:
         pass
```

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.6.7/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.6.7/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.6.7/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.6.7/sbcli_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.6.6
+Version: 2.6.7
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.6.6/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.6.7/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/pci_utils.py` & `sbcli_dev-2.6.7/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/snode_client.py` & `sbcli_dev-2.6.7/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/kv_store.py` & `sbcli_dev-2.6.7/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.6.7/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/rpc_client.py` & `sbcli_dev-2.6.7/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.6.7/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/utils.py` & `sbcli_dev-2.6.7/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/distr_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/cnode_client.py` & `sbcli_dev-2.6.7/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.6.7/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/constants.py` & `sbcli_dev-2.6.7/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.6.7/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.6.7/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/__init__.py` & `sbcli_dev-2.6.7/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.6.7/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.6.7/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.6.7/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.6.7/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.6.7/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.6.7/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.6.7/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.6.7/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.6.7/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.6.7/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.6.7/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.6.7/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.6.7/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.6.7/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.6.7/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.6.7/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/events.py` & `sbcli_dev-2.6.7/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.6.7/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/base_model.py` & `sbcli_dev-2.6.7/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.6.7/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.6.7/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.6.7/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/stats.py` & `sbcli_dev-2.6.7/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/pool.py` & `sbcli_dev-2.6.7/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/iface.py` & `sbcli_dev-2.6.7/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/cluster.py` & `sbcli_dev-2.6.7/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.6.7/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.6.7/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.6.7/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.6.7/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.6.7/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.6.7/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.6.7/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_dev-2.6.7/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.6.7/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.6.7/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.6/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_dev-2.6.7/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*
