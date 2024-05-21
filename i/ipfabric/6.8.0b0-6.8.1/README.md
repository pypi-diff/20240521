# Comparing `tmp/ipfabric-6.8.0b0.tar.gz` & `tmp/ipfabric-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.8.0b0.tar", max compression
+gzip compressed data, was "ipfabric-6.8.1.tar", max compression
```

## Comparing `ipfabric-6.8.0b0.tar` & `ipfabric-6.8.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.8.0b0/ipfabric/__init__.py
--rw-r--r--   0        0        0    11041 2024-04-29 16:40:32.514746 ipfabric-6.8.0b0/ipfabric/api.py
--rw-r--r--   0        0        0    10300 2024-04-29 17:45:57.981047 ipfabric-6.8.0b0/ipfabric/auth.py
--rw-r--r--   0        0        0    23030 2024-04-29 16:40:32.515823 ipfabric-6.8.0b0/ipfabric/client.py
--rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.8.0b0/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0    18216 2024-03-29 13:49:06.793074 ipfabric-6.8.0b0/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.8.0b0/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/shared_view.py
--rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.8.0b0/ipfabric/exceptions.py
--rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.8.0b0/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    21375 2024-04-29 16:47:05.807340 ipfabric-6.8.0b0/ipfabric/models/device.py
--rw-r--r--   0        0        0     7677 2024-03-20 16:35:10.771408 ipfabric-6.8.0b0/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.8.0b0/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.8.0b0/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5827 2024-04-29 19:22:26.698442 ipfabric-6.8.0b0/ipfabric/models/jobs.py
--rw-r--r--   0        0        0     4128 2024-03-20 16:35:10.774564 ipfabric-6.8.0b0/ipfabric/models/oas.py
--rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.8.0b0/ipfabric/models/rbac.py
--rw-r--r--   0        0        0    27947 2024-04-29 19:17:05.216570 ipfabric-6.8.0b0/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0     5755 2024-04-29 19:17:05.207890 ipfabric-6.8.0b0/ipfabric/models/snapshots.py
--rw-r--r--   0        0        0    23837 2024-03-20 16:35:10.776646 ipfabric-6.8.0b0/ipfabric/models/table.py
--rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.8.0b0/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.8.0b0/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.8.0b0/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.8.0b0/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.8.0b0/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.8.0b0/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.8.0b0/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.8.0b0/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.8.0b0/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.8.0b0/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.8.0b0/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.8.0b0/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.8.0b0/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.8.0b0/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.8.0b0/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.8.0b0/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.8.0b0/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.8.0b0/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.8.0b0/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.8.0b0/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.8.0b0/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.8.0b0/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.8.0b0/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.8.0b0/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.8.0b0/ipfabric/models/users.py
--rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.8.0b0/ipfabric/oas/__init__.py
--rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.8.0b0/ipfabric/oas/v6.7.json
--rw-r--r--   0        0        0   390704 2024-04-29 17:19:57.796133 ipfabric-6.8.0b0/ipfabric/oas/v6.8.json
--rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.8.0b0/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3641 2024-03-20 16:35:10.805129 ipfabric-6.8.0b0/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     7679 2024-04-30 12:35:22.770023 ipfabric-6.8.0b0/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     9119 2024-03-20 16:35:10.808322 ipfabric-6.8.0b0/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1394 2024-03-20 16:35:10.809455 ipfabric-6.8.0b0/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     3266 2024-03-20 16:35:10.810505 ipfabric-6.8.0b0/ipfabric/settings/local_users.py
--rw-r--r--   0        0        0    14522 2024-03-29 13:49:06.795074 ipfabric-6.8.0b0/ipfabric/settings/rbac.py
--rw-r--r--   0        0        0     2284 2024-03-20 16:35:10.811555 ipfabric-6.8.0b0/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.8.0b0/ipfabric/settings/settings.py
--rw-r--r--   0        0        0     2102 2024-03-20 16:35:10.813841 ipfabric-6.8.0b0/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     4487 2024-03-20 16:35:10.814866 ipfabric-6.8.0b0/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     9192 2024-04-30 12:41:49.057227 ipfabric-6.8.0b0/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      644 2024-03-20 16:35:10.817051 ipfabric-6.8.0b0/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     8583 2024-03-20 16:35:10.818051 ipfabric-6.8.0b0/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5656 2024-03-20 16:35:10.819099 ipfabric-6.8.0b0/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/__init__.py
--rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/policies.json
--rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/roles.json
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/__init__.py
--rw-r--r--   0        0        0    37983 2024-04-29 17:29:33.012935 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/policies.json
--rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/roles.json
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/__init__.py
--rw-r--r--   0        0        0     4730 2024-01-25 18:33:47.054282 ipfabric-6.8.0b0/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.8.0b0/ipfabric/tools/rbac.py
--rw-r--r--   0        0        0     4260 2024-03-20 16:35:10.822260 ipfabric-6.8.0b0/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0    22669 2024-03-20 16:35:10.823261 ipfabric-6.8.0b0/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.8.0b0/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.8.0b0/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.8.0b0/LICENSE
--rw-r--r--   0        0        0     3469 2024-04-29 16:40:32.512687 ipfabric-6.8.0b0/NOTICES.md
--rw-r--r--   0        0        0     3336 2024-05-01 15:35:30.792374 ipfabric-6.8.0b0/pyproject.toml
--rw-r--r--   0        0        0     6227 2024-04-29 16:40:32.513685 ipfabric-6.8.0b0/README.md
--rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 ipfabric-6.8.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.8.1/ipfabric/__init__.py
+-rw-r--r--   0        0        0    11009 2024-05-14 16:42:35.403692 ipfabric-6.8.1/ipfabric/api.py
+-rw-r--r--   0        0        0    10301 2024-05-14 16:42:35.403692 ipfabric-6.8.1/ipfabric/auth.py
+-rw-r--r--   0        0        0    22945 2024-05-14 16:42:35.403692 ipfabric-6.8.1/ipfabric/client.py
+-rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.8.1/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0    18233 2024-05-14 16:42:35.403692 ipfabric-6.8.1/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.8.1/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.8.1/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.8.1/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.8.1/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.8.1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.8.1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.8.1/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.8.1/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.8.1/ipfabric/diagrams/input_models/shared_view.py
+-rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.8.1/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.8.1/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.8.1/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.8.1/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.8.1/ipfabric/exceptions.py
+-rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.8.1/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    21346 2024-05-14 16:42:35.419308 ipfabric-6.8.1/ipfabric/models/device.py
+-rw-r--r--   0        0        0     7694 2024-05-14 16:42:35.419308 ipfabric-6.8.1/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.8.1/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.8.1/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5827 2024-05-14 16:42:35.419308 ipfabric-6.8.1/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0     4160 2024-05-14 16:42:35.419308 ipfabric-6.8.1/ipfabric/models/oas.py
+-rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.8.1/ipfabric/models/rbac.py
+-rw-r--r--   0        0        0    27813 2024-05-14 16:42:35.419308 ipfabric-6.8.1/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0     5759 2024-05-14 16:42:35.419308 ipfabric-6.8.1/ipfabric/models/snapshots.py
+-rw-r--r--   0        0        0    25314 2024-05-21 13:56:20.176258 ipfabric-6.8.1/ipfabric/models/table.py
+-rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.8.1/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.8.1/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.8.1/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.8.1/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.8.1/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.8.1/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.8.1/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.8.1/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.8.1/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.8.1/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.8.1/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.8.1/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.8.1/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.8.1/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.8.1/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.8.1/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.8.1/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.8.1/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.8.1/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.8.1/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.8.1/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.8.1/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.8.1/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.8.1/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.8.1/ipfabric/models/users.py
+-rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.8.1/ipfabric/oas/__init__.py
+-rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.8.1/ipfabric/oas/v6.7.json
+-rw-r--r--   0        0        0   390704 2024-05-14 16:42:35.426959 ipfabric-6.8.1/ipfabric/oas/v6.8.json
+-rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.8.1/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3611 2024-05-14 16:42:35.426959 ipfabric-6.8.1/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     7607 2024-05-14 16:42:35.426959 ipfabric-6.8.1/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     9074 2024-05-14 16:42:35.433180 ipfabric-6.8.1/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1411 2024-05-14 16:42:35.435187 ipfabric-6.8.1/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     3232 2024-05-14 16:42:35.435876 ipfabric-6.8.1/ipfabric/settings/local_users.py
+-rw-r--r--   0        0        0    14484 2024-05-14 16:42:35.435876 ipfabric-6.8.1/ipfabric/settings/rbac.py
+-rw-r--r--   0        0        0     2255 2024-05-14 16:42:35.435876 ipfabric-6.8.1/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.8.1/ipfabric/settings/settings.py
+-rw-r--r--   0        0        0     2111 2024-05-14 16:42:35.435876 ipfabric-6.8.1/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     4367 2024-05-14 16:42:35.442401 ipfabric-6.8.1/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     9192 2024-05-14 16:42:35.442401 ipfabric-6.8.1/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      687 2024-05-14 16:42:35.442401 ipfabric-6.8.1/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     8587 2024-05-14 16:42:35.442401 ipfabric-6.8.1/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5652 2024-05-14 16:42:35.442401 ipfabric-6.8.1/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.8.1/ipfabric/tools/managed_rbac/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/7/__init__.py
+-rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/7/policies.json
+-rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/7/roles.json
+-rw-r--r--   0        0        0        0 2024-05-14 16:42:35.442401 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/8/__init__.py
+-rw-r--r--   0        0        0    37983 2024-05-14 16:42:35.450957 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/8/policies.json
+-rw-r--r--   0        0        0     3383 2024-05-14 16:42:35.450957 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/8/roles.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/__init__.py
+-rw-r--r--   0        0        0     7166 2024-05-21 13:57:32.894570 ipfabric-6.8.1/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.8.1/ipfabric/tools/rbac.py
+-rw-r--r--   0        0        0     4210 2024-05-14 16:42:35.452449 ipfabric-6.8.1/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0    24152 2024-05-14 16:42:35.452449 ipfabric-6.8.1/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.8.1/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.8.1/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.8.1/LICENSE
+-rw-r--r--   0        0        0     3469 2024-05-14 16:42:35.403692 ipfabric-6.8.1/NOTICES.md
+-rw-r--r--   0        0        0     3334 2024-05-21 13:57:32.894570 ipfabric-6.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6227 2024-05-14 16:42:35.403692 ipfabric-6.8.1/README.md
+-rw-r--r--   0        0        0     8375 1970-01-01 00:00:00.000000 ipfabric-6.8.1/PKG-INFO
```

### Comparing `ipfabric-6.8.0b0/ipfabric/__init__.py` & `ipfabric-6.8.1/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/api.py` & `ipfabric-6.8.1/ipfabric/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from httpx._types import CertTypes, VerifyTypes
 from pydantic import ConfigDict, Field, InstanceOf
 from pydantic.dataclasses import dataclass
 
 from ipfabric.auth import Setup, ProxyTypes, TimeoutTypes, ProxiesTypes
 from ipfabric.exceptions import api_insuf_rights
 from ipfabric.models import Snapshot, OAS, Endpoint, Snapshots, Methods, User
-from ipfabric.tools import VALID_REFS, trigger_backup
+from ipfabric.tools import VALID_REFS, trigger_backup, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 LAST_ID, PREV_ID, LASTLOCKED_ID = VALID_REFS
 
 
 @dataclass(config=ConfigDict(arbitrary_types_allowed=True))
@@ -242,20 +242,18 @@
 
     def get_user(self) -> User:
         """Gets current logged in user information.
 
         Returns:
             User: User model of logged in user
         """
-        resp = self.get("users/me")
-        resp.raise_for_status()
+        resp = raise_for_status(self.get("users/me"))
         user = User(**resp.json())
         if not (user.is_admin and user.token):  # TODO: NIM-14008: Implement logic after obtaining scopes for tokens
-            resp = self.get("users/me/scopes/api")
-            resp.raise_for_status()
+            resp = raise_for_status(self.get("users/me/scopes/api"))
             user.scopes = resp.json()["data"]
         return user
 
     def _ipf_pager(
         self,
         url: str,
         payload: dict,
@@ -270,16 +268,15 @@
         :return: list: List of dictionaries
         """
         payload["pagination"] = dict(limit=limit)
         data = list()
 
         def page(s):
             payload["pagination"]["start"] = s
-            r = self.post(url, json=payload)
-            r.raise_for_status()
+            r = raise_for_status(self.post(url, json=payload))
             return r.json()["data"]
 
         r_data = page(start)
         data.extend(r_data)
         while limit == len(r_data):
             start = start + limit
             r_data = page(start)
```

### Comparing `ipfabric-6.8.0b0/ipfabric/auth.py` & `ipfabric-6.8.1/ipfabric/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from httpx import Client, BaseTransport, URL, Request, Response, Auth, Timeout, post, Proxy
 from httpx._client import EventHook
 from httpx._types import CertTypes, VerifyTypes, URLTypes
 from pydantic import field_validator, Field, AliasChoices, PrivateAttr, InstanceOf
 from pydantic_settings import BaseSettings, SettingsConfigDict, PydanticBaseSettingsSource, InitSettingsSource
 
-from ipfabric.tools import VALID_REFS
+from ipfabric.tools import VALID_REFS, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 RE_VERSION = re.compile(r"v?(\d(\.\d)?)")
 ProxyTypes = Union[None, URLTypes, InstanceOf[Proxy]]
 ProxiesTypes = Union[ProxyTypes, Dict[URLTypes, Union[None, ProxyTypes]]]
 TimeoutTypes = Union[
@@ -47,29 +47,29 @@
 
     def auth_flow(self, request: Request) -> Generator[Request, Response, None]:
         response = yield request
 
         if response.status_code == 401:
             response.read()
             if "API_EXPIRED_ACCESS_TOKEN" in response.text:
-                # Use refreshToken in Cookies to get new accessToken
-                resp = post(response.url.join("/api/auth/token"), cookies=self.cookie_jar)
-                resp.raise_for_status()  # Response updates accessToken in shared CookieJar
+                # Use refreshToken in Cookies to get new accessToken & Response updates accessToken in shared CookieJar
+                resp = raise_for_status(post(response.url.join("/api/auth/token"), cookies=self.cookie_jar))
                 request.headers["Cookie"] = "accessToken=" + resp.cookies["accessToken"]  # Update request
                 yield request
         return response
 
     def _login(self, username: str, password: str, base_url: URL, verify: VerifyTypes) -> None:
-        resp = post(
-            base_url.join("auth/login"),
-            json=dict(username=username, password=password),
-            cookies=self.cookie_jar,
-            verify=verify,
+        raise_for_status(
+            post(
+                base_url.join("auth/login"),
+                json=dict(username=username, password=password),
+                cookies=self.cookie_jar,
+                verify=verify,
+            )
         )
-        resp.raise_for_status()
 
 
 class MyInitSettingsSource(InitSettingsSource):
     def __init__(self, settings_cls, init_kwargs: Dict[str, Any]):
         timeout = init_kwargs.pop("timeout", "DEFAULT")
         init_kwargs = {k: v for k, v in init_kwargs.items() if v is not None}
         if timeout != "DEFAULT":
@@ -167,16 +167,15 @@
         """Checks API Version and returns the version to use in the URL and the OS Version
 
         Returns:
             api_version, os_version
         """
         cfg_version = self.api_version.lstrip("v").split(".")
 
-        resp = self.client.get("/api/version")
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.get("/api/version"))
         os_api_version = resp.json()["apiVersion"].lstrip("v").split(".")
         api_version = f"v{cfg_version[0]}.{cfg_version[1]}" if len(cfg_version) > 1 else f"v{cfg_version[0]}"
         if len(cfg_version) == 1 and cfg_version[0] > os_api_version[0]:
             logger.warning(
                 f"Specified API or SDK Version (v{cfg_version[0]}) is greater then "
                 f"OS API Version. Using OS Version:  (v{os_api_version[0]})"
             )
```

### Comparing `ipfabric-6.8.0b0/ipfabric/client.py` & `ipfabric-6.8.1/ipfabric/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pydantic import ConfigDict
 from pydantic.dataclasses import dataclass
 
 from ipfabric.api import IPFabricAPI
 from ipfabric.diagrams import Diagram
 from ipfabric.models import Technology, Inventory, Jobs, Intent, Devices
 from ipfabric.settings import Settings
-from ipfabric.tools import TIMEZONES
+from ipfabric.tools import TIMEZONES, raise_for_status
 from .exceptions import deprecated_args_decorator
 
 try:
     from pandas import DataFrame
 except ImportError:
     DataFrame = None
 
@@ -39,15 +39,15 @@
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == "timeout":
             self._client.timeout = value
         elif name == "snapshot_id":
             value = self._switch_snapshot(value)
             self.__dict__[name] = value
-            if value and self.snapshot.disabled_intent_verification is False and self._intent and self.intent.loaded:
+            if value and self.snapshot.disabled_intent_verification is False and self._intent:
                 self._intent = Intent(client=self)
             if value and self._devices:
                 self._devices = self.load_devices()
             return None
         super().__setattr__(name, value)
 
     def __repr__(self):
@@ -203,16 +203,15 @@
         export = payload.get("format", {}).get("dataType", "json")
         data = False
         if export == "csv" or (self.streaming and get_all):
             data = self._stream(url, payload, export)
         elif get_all and data is False:
             data = self._ipf_pager(url, payload)
         elif data is False:
-            res = self.post(url, json=payload)
-            res.raise_for_status()
+            res = raise_for_status(self.post(url, json=payload))
             data = res.json()["data"]
         return data
 
     def get_columns(self, url: str, ui: bool = False) -> List[str]:
         """Checks OAS to find available columns.
 
         Args:
@@ -246,16 +245,15 @@
             snapshot: Set to False for some tables like management endpoints.
         Returns:
             int: a count of rows
         """
         snapshot_id = snapshot_id or self.snapshot_id if snapshot else None
         url, payload = self._check_url_payload(url, snapshot_id, filters, None, None, attr_filters, None, None)
         payload.update({"columns": ["id"], "pagination": {"limit": 1, "start": 0}})
-        res = self.post(url, json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.post(url, json=payload))
         return res.json()["_meta"]["count"]
 
     def _fetch_setup(self, url, export, columns, snapshot_id, filters, reports, sort, attr_filters, csv_tz, snapshot):
         if export == "df" and DataFrame is None:
             raise ImportError("pandas not installed. Run `pip install ipfabric[pd]`.")
         snapshot_id = snapshot_id or self.snapshot_id if snapshot else None
         if "color" in dumps(filters) and not reports:
@@ -350,16 +348,15 @@
             url, export, columns, snapshot_id, filters, reports, sort, attr_filters, csv_tz, snapshot
         )
         payload["pagination"] = dict(start=start, limit=limit)
         data = False
         if export == "csv" or self.streaming:
             data = self._stream(url, payload, export)
         if data is False:
-            res = self.post(url, json=payload)
-            res.raise_for_status()
+            res = raise_for_status(self.post(url, json=payload))
             data = res.json()["data"]
         if export == "df":
             data = DataFrame.from_records(data) if export == "df" else data
         return data
 
     @overload
     def fetch_all(
@@ -456,16 +453,15 @@
                 url_id = parsed_url.path.split("/")[-1]
             else:
                 raise SyntaxError("Wrong endpoint selected.")
         if table:
             resp = self.get(f"/tables/url/{url_id}")
         else:
             resp = self.get(f"/graphs/urls/{url_id}")
-        resp.raise_for_status()
-        return resp.json()
+        return raise_for_status(resp).json()
 
     def shared_view(self, url: Union[int, str], data=True, reports: bool = True) -> Union[str, list]:
         """Takes a shared table view link and returns the data or the code to implement in python.
 
         Args:
             url: Id of the shared view (1453653298) or full/partial URL (`/inventory/devices?copyId=1453653298`)
             data: Defaults to return the data instead of printing the code
@@ -540,10 +536,9 @@
             "autoSizedColumns": auto_size,
             "columnVisibility": _columns,
             "webEndpoint": web_endpoint,
             "filters": loads(filters) if isinstance(filters, str) else filters,
         }
         payload.update({"columnWidth": col_width} if col_width else {})
         payload.update({"sort": sort} if sort else {})
-        resp = self.post("tables/url", json=payload)
-        resp.raise_for_status()
+        resp = raise_for_status(self.post("tables/url", json=payload))
         return str(self.base_url.join(web_endpoint)) + f"?copyId={resp.json()['id']}"
```

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/__init__.py` & `ipfabric-6.8.1/ipfabric/diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/graphs.py` & `ipfabric-6.8.1/ipfabric/diagrams/graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Union, Dict, List, Optional, Literal, Any
 from warnings import warn
 
 from pydantic import BaseModel
 
 from ipfabric.api import IPFabricAPI
+from ipfabric.tools import raise_for_status
 from .input_models import (
     Unicast,
     Multicast,
     Host2GW,
     Network,
     NetworkSettings,
     PathLookupSettings,
@@ -85,16 +86,15 @@
             payload["overlay"] = self._format_overlay(overlay, snapshot_id)
         if graph_settings:
             payload["settings"] = graph_settings
         if attr_filters or self.ipf.attribute_filters:
             payload["attributeFilters"] = attr_filters or self.ipf.attribute_filters
         if positions:
             payload["positions"] = {k: dict(v) for k, v in positions.items()}
-        res = self.ipf.post(url, json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.ipf.post(url, json=payload))
         return res.json() if image == "json" else res.content
 
     def json(
         self,
         parameters: Union[Unicast, Multicast, Host2GW, Network],
         snapshot_id: str = None,
         overlay: Union[Overlay, dict] = None,
@@ -187,16 +187,15 @@
                 "positions": {k: v["position"] for k, v in resp["graphResult"]["graphData"]["nodes"].items()},
                 "settings": resp["graphResult"]["settings"],
             },
             "snapshot": self._check_snapshot_id(snapshot_id),
         }
         if overlay:
             payload["graphView"]["overlay"] = self._format_overlay(overlay, snapshot_id)
-        res = self.ipf.post("graphs/urls", json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.ipf.post("graphs/urls", json=payload))
         return str(self.ipf.base_url.join(f"/diagrams/share/{res.json()['id']}"))
 
     def model(
         self,
         parameters: Union[Unicast, Multicast, Host2GW, Network],
         snapshot_id: str = None,
         overlay: Overlay = None,
```

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/icmp.py` & `ipfabric-6.8.1/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/__init__.py` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/constants.py` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/shared_view.py` & `ipfabric-6.8.1/ipfabric/diagrams/input_models/shared_view.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric-6.8.1/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/output_models/protocols.py` & `ipfabric-6.8.1/ipfabric/diagrams/output_models/protocols.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/diagrams/output_models/trace.py` & `ipfabric-6.8.1/ipfabric/diagrams/output_models/trace.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/exceptions.py` & `ipfabric-6.8.1/ipfabric/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/__init__.py` & `ipfabric-6.8.1/ipfabric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/device.py` & `ipfabric-6.8.1/ipfabric/models/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ipfabric.settings.attributes import Attributes
 from httpx import HTTPStatusError
 from typing import Optional, List, Union, Dict, DefaultDict, Set, overload, Literal, Any
 from ipaddress import IPv4Interface
 from collections import defaultdict
 from case_insensitive_dict import CaseInsensitiveDict
 from ipfabric.models.technology import Technology
-from ipfabric.tools.shared import create_filter
+from ipfabric.tools.shared import create_filter, raise_for_status
 
 from pydantic import BaseModel, Field, PrivateAttr
 
 logger = logging.getLogger("ipfabric")
 
 
 class DeviceConfig(BaseModel):
@@ -99,24 +99,21 @@
     @classmethod
     def check_attribute(cls, attribute) -> True:
         if attribute not in cls.model_fields:
             raise AttributeError(f"Attribute {attribute} not in Device class.")
         return True
 
     def get_log_file(self) -> str:
-        res = self.client.get("/os/logs/task/" + self.task_key)
-        res.raise_for_status()
-        return res.text
+        return raise_for_status(self.client.get("/os/logs/task/" + self.task_key)).text
 
     def get_config(self) -> Union[None, DeviceConfig]:
         if not self.blob_key:
             logger.warning("Device Config not in Snapshot File. Please try using ipfabric.tools.DeviceConfigs")
             return None
-        res = self.client.get("blobs/device-configuration/" + str(self.blob_key))
-        res.raise_for_status()
+        res = raise_for_status(self.client.get("blobs/device-configuration/" + str(self.blob_key)))
         return DeviceConfig(**res.json())
 
     def interfaces(self) -> list:
         return self.fetch_all("tables/inventory/interfaces")
 
     def pn(self) -> list:
         return self.fetch_all("tables/inventory/pn")
```

### Comparing `ipfabric-6.8.0b0/ipfabric/models/intent.py` & `ipfabric-6.8.1/ipfabric/models/intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import defaultdict
 from typing import Any, Union, List, Dict, Optional
 from warnings import warn
 
 from httpx import HTTPStatusError
 from pydantic import BaseModel, PrivateAttr, Field
 
+from ipfabric.tools import raise_for_status
 from .intent_check import Group, IntentCheck
 
 logger = logging.getLogger("ipfabric")
 COLOR_DICT = dict(nan=-1, green=0, blue=10, amber=20, red=30)
 
 
 class Intent(BaseModel):
@@ -53,17 +54,16 @@
         if not snapshot.loaded:
             raise ValueError(f"Snapshot {snapshot.snapshot_id} is not loaded; cannot pull Intent Rules.")
         if snapshot.disabled_intent_verification is True:
             raise ValueError(
                 f"Snapshot {snapshot.snapshot_id} has Intent Verification computation disabled; "
                 "cannot pull Intent Rules."
             )
-        res = self.client.get("reports", params=dict(snapshot=snapshot.snapshot_id))
+        res = raise_for_status(self.client.get("reports", params=dict(snapshot=snapshot.snapshot_id)))
         try:
-            res.raise_for_status()
             return [IntentCheck(**check) for check in res.json()]
         except HTTPStatusError:
             logger.warning(self.client._api_insuf_rights + 'on GET "/reports". Will not load Intents.')
             return list()
 
     def load_intent(self, snapshot_id: str = None):
         """Loads intent checks into the class.
@@ -73,23 +73,21 @@
         """
         self.snapshot_id = snapshot_id or self.client.snapshot_id
         self._intent_checks = self.get_intent_checks(snapshot_id)
         self._groups = self.get_groups()
 
     def get_groups(self) -> list:
         """
-
         Returns:
             list: list of groups
         """
         res = self.client.get("reports/groups")
-        try:
-            res.raise_for_status()
+        if res.status_code == 200:
             return [Group(**group) for group in res.json()]
-        except HTTPStatusError:
+        else:  # TODO: Fix this error
             logger.warning(self.client._api_insuf_rights + 'on GET "/reports/groups". Will not load Intent Groups.')
             return list()
 
     @property
     def custom(self) -> List[IntentCheck]:
         return [c for c in self.intent_checks if c.custom]
```

### Comparing `ipfabric-6.8.0b0/ipfabric/models/intent_check.py` & `ipfabric-6.8.1/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/inventory.py` & `ipfabric-6.8.1/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/jobs.py` & `ipfabric-6.8.1/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/oas.py` & `ipfabric-6.8.1/ipfabric/models/oas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Optional, List, Any, Dict
 
 from pydantic import BaseModel, PrivateAttr, TypeAdapter, computed_field, Field
 
+from ipfabric.tools import raise_for_status
+
 try:
     from importlib.resources import files
 except ImportError:
     from importlib_resources import files
 
 OAS_DIR = files("ipfabric.oas")
 
@@ -95,16 +97,15 @@
             ]
             data.nested_columns = [k for k, v in columns.items() if "type" in v and v["type"] == "array"]
         except KeyError:
             pass
         return data
 
     def _parse_oas(self) -> Dict[str, Methods]:
-        resp = self.client.get(self.client.base_url.join("/api/oas/openapi-extended.json"))
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.get(self.client.base_url.join("/api/oas/openapi-extended.json")))
 
         endpoints = dict()
         for endpoint, methods in resp.json()["paths"].items():
             methods_obj = Methods(api_endpoint=endpoint)
             for method, spec in methods.items():
                 data = Endpoint(
                     api_endpoint=endpoint[1:],
```

### Comparing `ipfabric-6.8.0b0/ipfabric/models/rbac.py` & `ipfabric-6.8.1/ipfabric/models/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/snapshot.py` & `ipfabric-6.8.1/ipfabric/models/snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,17 @@
     from ipfabric import IPFClient
     from ipfabric.api import IPFabricAPI
 
 import logging
 from datetime import datetime
 from time import sleep
 from typing import Optional, List, Union, Set, Dict, Literal, Any
-from httpx import HTTPError
 from pathlib import Path
 from ipfabric.models import Device
-from ipfabric.tools import validate_ip_network_str, VALID_IP
+from ipfabric.tools import validate_ip_network_str, VALID_IP, raise_for_status
 from ipfabric.settings.attributes import Attributes
 
 from pydantic import BaseModel, Field, PrivateAttr
 from .jobs import Jobs
 from ipfabric.exceptions import deprecated_args_decorator
 
 logger = logging.getLogger("ipfabric")
@@ -62,15 +61,15 @@
 def snapshot_upload(ipf: IPFClient, filename: str):
     data = {"file": (Path(filename).name, open(filename, "rb"), "application/x-tar")}
     resp = ipf.post("snapshots/upload", files=data)
     if resp.status_code == 400:
         if resp.json()["code"] == "API_SNAPSHOT_CONFLICT":
             logger.warning(f"SNAPSHOT ID {resp.json()['data']['snapshot']} already uploaded")
             return
-    resp.raise_for_status()
+    raise_for_status(resp)
     return resp.json()
 
 
 class Error(BaseModel):
     error_type: str = Field(None, alias="errorType")
     count: int
 
@@ -130,26 +129,24 @@
     def errors_dict(self):
         return {_.error_type: _.count for _ in self.errors}
 
     @deprecated_args_decorator(version="6.9.0")
     @loaded_status
     def lock(self, ipf: IPFClient = None) -> bool:
         if not self.locked:
-            res = self.client.post(f"snapshots/{self.snapshot_id}/lock")
-            res.raise_for_status()
+            raise_for_status(self.client.post(f"snapshots/{self.snapshot_id}/lock"))
             self.locked = True
         else:
             logger.warning(f"Snapshot {self.snapshot_id} is already locked.")
         return True
 
     @deprecated_args_decorator(version="6.9.0")
     def unlock(self, ipf: IPFClient = None) -> bool:
         if self.locked and self.loaded:
-            res = self.client.post(f"snapshots/{self.snapshot_id}/unlock")
-            res.raise_for_status()
+            raise_for_status(self.client.post(f"snapshots/{self.snapshot_id}/unlock"))
             self.locked = False
         else:
             logger.warning(f"Snapshot {self.snapshot_id} is already unlocked.")
         return True
 
     @property
     def loaded(self):
@@ -161,16 +158,15 @@
 
     @deprecated_args_decorator(version="6.9.0", arg_type="IPFClient", no_args=False)
     def unload(self, ipf: IPFClient = None, wait_for_unload: bool = False, timeout: int = 60, retry: int = 5) -> bool:
         if not self.loaded:
             logger.warning(f"Snapshot {self.snapshot_id} is already unloaded.")
             return True
         ts = int(datetime.now().timestamp() * 1000)
-        res = self.client.post("snapshots/unload", json=[dict(jobDetail=ts, id=self.snapshot_id)])
-        res.raise_for_status()
+        raise_for_status(self.client.post("snapshots/unload", json=[dict(jobDetail=ts, id=self.snapshot_id)]))
         if wait_for_unload:
             if not self._jobs.check_snapshot_job(self.snapshot_id, ts, "unload", retry, timeout):
                 logger.error("Snapshot Unload did not finish.")
                 return False
         self._refresh_status()
         return True
 
@@ -183,16 +179,15 @@
         timeout: int = 60,
         retry: int = 5,
     ) -> bool:
         if self.loaded:
             logger.warning(f"Snapshot {self.snapshot_id} is already loaded.")
             return True
         ts = int(datetime.now().timestamp() * 1000)
-        res = self.client.post("snapshots/load", json=[dict(jobDetail=ts, id=self.snapshot_id)])
-        res.raise_for_status()
+        raise_for_status(self.client.post("snapshots/load", json=[dict(jobDetail=ts, id=self.snapshot_id)]))
         if wait_for_load or wait_for_assurance:
             if not self._check_load_status(ts, wait_for_assurance, timeout, retry):
                 return False
         self._refresh_status()
         return True
 
     def _refresh_status(self):
@@ -210,15 +205,15 @@
 
     def _check_load_status(
         self,
         ts: int,
         wait_for_assurance: bool = True,
         timeout: int = 60,
         retry: int = 5,
-        action: str = 'load',
+        action: str = "load",
     ):
         load_job = self._jobs.check_snapshot_job(
             self.snapshot_id, started=ts, action=action, timeout=timeout, retry=retry
         )
         if load_job and wait_for_assurance:
             return self._check_assurance_status(load_job["startedAt"], timeout, retry)
         elif not load_job:
@@ -268,16 +263,15 @@
         elif not isinstance(path, Path):
             path = Path(f"{path}")
         if not path.name.endswith(".tar"):
             path = Path(f"{path.name}.tar")
 
         # start download job
         ts = int(datetime.now().timestamp() * 1000)
-        resp = self.client.get(f"/snapshots/{self.snapshot_id}/download")
-        resp.raise_for_status()
+        raise_for_status(self.client.get(f"/snapshots/{self.snapshot_id}/download"))
 
         # waiting for download job to process
         job = self._jobs.check_snapshot_job(
             self.snapshot_id, started=ts, action="download", retry=retry, timeout=timeout
         )
         if job:
             filename = self.client.get(f"jobs/{job['id']}/download")
@@ -285,28 +279,29 @@
                 fp.write(filename.read())
             return path
         logger.error(f"Download job did not finish within {retry * timeout} seconds, could not get file.")
         return None
 
     @deprecated_args_decorator(version="6.9.0", arg_type=("IPFClient", "IPFabricAPI"), no_args=False)
     @loaded_status
-    def get_snapshot_settings(self, ipf: Union[IPFClient, IPFabricAPI] = None) -> Union[dict, bool]:
+    def get_snapshot_settings(self, ipf: Union[IPFClient, IPFabricAPI] = None) -> Union[dict, None]:
         settings = None
         msg = "API_INSUFFICIENT_RIGHTS to `snapshots/:key/settings` " + self.client.user.error_msg
 
         if self.client.user.snapshots_settings is False:
             logger.debug(f"Could not get Snapshot {self.snapshot_id} Settings:" + msg)
             return settings
+
         res = self.client.get(f"/snapshots/{self.snapshot_id}/settings")
-        try:
-            res.raise_for_status()
+        if res.status_code == 200:
             settings = res.json()
             if self.client.user.snapshots_settings is None:
                 self.client.user.snapshots_settings = True
-        except HTTPError:
+
+        else:
             logger.debug(f"Could not get Snapshot {self.snapshot_id} Settings:" + msg)
             logger.warning(msg)
             self.client.user.snapshots_settings = False
         return settings
 
     @deprecated_args_decorator(version="6.9.0", arg_type=("IPFClient", "IPFabricAPI"), no_args=False)
     @loaded_status
@@ -347,18 +342,19 @@
         disabled, ae_settings = self._calculate_new_ae_settings(
             current, disabled_graph_cache, disabled_historical_data, disabled_intent_verification
         )
         if disabled == current:
             logger.info("No changes to Assurance Engine Settings required.")
             return True
         ts = int(datetime.now().timestamp() * 1000)
-        res = self.client.patch(
-            f"/snapshots/{self.snapshot_id}/settings", json=dict(disabledPostDiscoveryActions=list(disabled))
+        raise_for_status(
+            self.client.patch(
+                f"/snapshots/{self.snapshot_id}/settings", json=dict(disabledPostDiscoveryActions=list(disabled))
+            )
         )
-        res.raise_for_status()
         if wait_for_assurance and current - disabled:
             ae_status = self._jobs.check_snapshot_assurance_jobs(
                 self.snapshot_id, ae_settings, started=ts, timeout=timeout, retry=retry
             )
             if not ae_status:
                 logger.error("Assurance Engine tasks did not complete")
                 return False
@@ -520,15 +516,15 @@
         ts = int(datetime.now().timestamp() * 1000)
         if action == "delete":
             resp = self.client.request("DELETE", f"snapshots/{self.snapshot_id}/devices", json=sn)
         else:
             resp = self.client.post(
                 f"snapshots/{self.snapshot_id}/devices", json=dict(snList=sn, vendorSettingsMap=dict())
             )
-        resp.raise_for_status()
+        raise_for_status(resp)
         if not wait_for_discovery:
             self._change_snapshot()
             return resp.json()["success"]
 
         return self._check_modification_status(wait_for_assurance, ts, timeout, retry, action)
 
     def _vendor_apis(self):
@@ -581,15 +577,15 @@
                 raise ValueError(f"IP Network {i} is larger than /23.")
             ips.append(i)
 
         payload = {"ipList": ips, "retryTimedOut": retry_timed_out, "vendorApi": vendors}
 
         ts = int(datetime.now().timestamp() * 1000)
         resp = self.client.post(f"snapshots/{self.snapshot_id}/devices", json=payload)
-        resp.raise_for_status()
+        raise_for_status(resp)
         if not wait_for_discovery:
             self._change_snapshot()
             return resp.json()["success"]
         return self._check_modification_status(wait_for_assurance, ts, timeout, retry, "add")
 
     def _change_snapshot(self):
         logger.warning(f"Snapshot {self.snapshot_id} is discovering switching to $last.")
```

### Comparing `ipfabric-6.8.0b0/ipfabric/models/snapshots.py` & `ipfabric-6.8.1/ipfabric/models/snapshots.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Union
 from typing import OrderedDict as OrderedDictType
 from uuid import UUID
 
 from pydantic import BaseModel, PrivateAttr, Field
 
 from ipfabric.models import Snapshot, SNAPSHOT_COLUMNS
-from ipfabric.tools import VALID_REFS
+from ipfabric.tools import VALID_REFS, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 LAST_ID, PREV_ID, LASTLOCKED_ID = VALID_REFS
 
 
 class Snapshots(BaseModel):
@@ -110,16 +110,15 @@
         Need to do a GET and POST to get all Snapshot data. See NIM-7223
         POST Missing:
         licensedDevCount
         errors
         version
         initialVersion
         """
-        res = self.client.get("/snapshots")
-        res.raise_for_status()
+        res = raise_for_status(self.client.get("/snapshots"))
         return {s["id"]: s for s in res.json()}
 
     def get_snapshots(self) -> OrderedDictType[str, Snapshot]:
         """Gets all snapshots from IP Fabric and returns a dictionary of {ID: Snapshot_info}
 
         Returns:
             Dictionary with ID as key and dictionary with info as the value
```

### Comparing `ipfabric-6.8.0b0/ipfabric/models/table.py` & `ipfabric-6.8.1/ipfabric/models/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Optional, Dict, List, Any, Union, overload, Literal
+from typing import Optional, Dict, List, Any, Union, overload, Literal, Tuple, Set
 
 import deepdiff
 from pydantic import BaseModel, Field, computed_field
 
 from ipfabric.tools.shared import create_filter
 
 try:
@@ -573,46 +573,79 @@
             for hashed_str in hashed_data_compare.keys()
             if hashed_str not in hashed_data.keys()
         ]
         return_dict["added"] = added
         return_dict["removed"] = removed
         return return_dict
 
-    def join_table(self, on_column: str, join_table_path: str) -> Dict:
+    def join_table(
+        self,
+        on_column: Union[str, Dict[str, str], List[str], Tuple[str], Set[str]],
+        join_table_path: str,
+        how: Literal["right", "left"] = "right",
+    ) -> Dict:
         """
-        performs a join operation on on_columns, assuming on_columns are columns that
+        Performs a join operation on on_columns, assuming on_columns are columns that
         exist in both self and join_table_path. If on_columns are not columns in
         set(self.client.get_columns(self.endpoint)), ValueError is raised.
 
         Args:
-            on_column: str : name of column to use for join operation
+            on_column: Union[str, Dict[str, str], List[str], Tuple[str], Set[str]] : column(s) to use for join operation
             join_table_path: URL of table to use for join operation
+            how: str : type of join operation ('right' or 'left')
 
         Returns: dict: Dictionary of result of joined table.
-         possible keys <join_table_path>, self.endpoint, joined, no_matches
+            possible keys <join_table_path>, self.endpoint, joined, no_matches
         """
+        if isinstance(on_column, str):
+            on_column = {on_column: on_column}
+        elif isinstance(on_column, (list, set, tuple)):
+            on_column = {col: col for col in on_column}
+
         self_cols = set(self.client.get_columns(self.endpoint))
-        if not {on_column}.issubset(self_cols):
-            raise ValueError(f"Column {on_column}, is not subset of {self_cols}.")
+        join_table_path = self.client._check_url(join_table_path)
+        join_cols = set(self.client.get_columns(join_table_path))
+
+        for col_self, col_join in on_column.items():
+            if col_self not in self_cols:
+                raise ValueError(f"Column {col_self} is not in self table columns {self_cols}.")
+            if col_join not in join_cols:
+                raise ValueError(f"Column {col_join} is not in join table columns {join_cols}.")
+
         self_table = self.client.fetch_all(self.endpoint)
         join_table = self.client.fetch_all(join_table_path)
 
-        joined_data = [
-            {**self_dict, **join_dict}
-            for self_dict in self_table
-            for join_dict in join_table
-            if self_dict[on_column] == join_dict[on_column]
-        ]
+        def match_rows(self_dict, join_dict):
+            return all(self_dict[col_self] == join_dict[col_join] for col_self, col_join in on_column.items())
 
-        no_matches = [
-            join_dict
-            for join_dict in join_table
-            if join_dict[on_column] not in (entry[on_column] for entry in joined_data)
-        ]
+        if how == "right":
+            joined_data = [
+                {**self_dict, **join_dict}
+                for join_dict in join_table
+                for self_dict in self_table
+                if match_rows(self_dict, join_dict)
+            ]
+            no_matches = [
+                self_dict
+                for self_dict in self_table
+                if not any(match_rows(self_dict, join_dict) for join_dict in join_table)
+            ]
+        else:
+            joined_data = [
+                {**join_dict, **self_dict}
+                for self_dict in self_table
+                for join_dict in join_table
+                if match_rows(self_dict, join_dict)
+            ]
+            no_matches = [
+                join_dict
+                for join_dict in join_table
+                if not any(match_rows(self_dict, join_dict) for self_dict in self_table)
+            ]
 
         dict_for_return = {
             "joined": joined_data,
-            f"{self.endpoint}": self_table,
-            f"{join_table_path}": join_table,
+            self.endpoint: self_table,
+            join_table_path: join_table,
             "no_matches": no_matches,
         }
         return dict_for_return
```

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/__init__.py` & `ipfabric-6.8.1/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/addressing.py` & `ipfabric-6.8.1/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/cloud.py` & `ipfabric-6.8.1/ipfabric/models/technology/cloud.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/dhcp.py` & `ipfabric-6.8.1/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/fhrp.py` & `ipfabric-6.8.1/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/interfaces.py` & `ipfabric-6.8.1/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.8.1/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/managed_networks.py` & `ipfabric-6.8.1/ipfabric/models/technology/managed_networks.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/management.py` & `ipfabric-6.8.1/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/mpls.py` & `ipfabric-6.8.1/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/multicast.py` & `ipfabric-6.8.1/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/neighbors.py` & `ipfabric-6.8.1/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/oam.py` & `ipfabric-6.8.1/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/platforms.py` & `ipfabric-6.8.1/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/port_channels.py` & `ipfabric-6.8.1/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/qos.py` & `ipfabric-6.8.1/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/routing.py` & `ipfabric-6.8.1/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/sdn.py` & `ipfabric-6.8.1/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/sdwan.py` & `ipfabric-6.8.1/ipfabric/models/technology/sdwan.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/security.py` & `ipfabric-6.8.1/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/stp.py` & `ipfabric-6.8.1/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/vlans.py` & `ipfabric-6.8.1/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/technology/wireless.py` & `ipfabric-6.8.1/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/models/users.py` & `ipfabric-6.8.1/ipfabric/models/users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/oas/v6.7.json` & `ipfabric-6.8.1/ipfabric/oas/v6.7.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/oas/v6.8.json` & `ipfabric-6.8.1/ipfabric/oas/v6.8.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/__init__.py` & `ipfabric-6.8.1/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/api_tokens.py` & `ipfabric-6.8.1/ipfabric/settings/api_tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Any, Union, Optional, List
 
 from pydantic import Field, BaseModel
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
-from ipfabric.tools.shared import date_parser
+from ipfabric.tools.shared import date_parser, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 
 class Token(BaseModel):
     description: str
     usage: int
@@ -43,16 +43,15 @@
         return {t.token_id: t for t in self.tokens}
 
     @property
     def tokens_by_description(self):
         return {t.description: t for t in self.tokens}
 
     def get_tokens(self) -> List[Token]:
-        res = self.client.get("api-tokens")
-        res.raise_for_status()
+        res = raise_for_status(self.client.get("api-tokens"))
         return [Token(**t) for t in res.json()]
 
     def _check_roles(self, role_ids: list, role_names: list):
         if not role_names and not role_ids:
             raise SyntaxError("No Role Ids or Names provided.")
         checked_roles = list()
         for role in role_ids:
@@ -75,24 +74,22 @@
         expires: Optional[Union[str, int]] = None,
     ):
         payload = dict(
             description=descr,
             expires=int(date_parser(expires).timestamp() * 1000) if expires else None,
             roleIds=self._check_roles(role_ids or list(), role_names or list()),
         )
-        res = self.client.post("api-tokens", json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.client.post("api-tokens", json=payload))
         return Token(**res.json())
 
     def delete_token(self, token_id: [int, str, Token]):
         token_id = token_id.token_id if isinstance(token_id, Token) else str(token_id)
         if token_id not in self.tokens_by_id:
             raise ValueError(f"Could not find token matching ID '{token_id}'.")
-        res = self.client.delete("api-tokens/" + token_id)
-        res.raise_for_status()
+        raise_for_status(self.client.delete("api-tokens/" + token_id))
         self._tokens = self.get_tokens()
         return self.tokens
 
     def delete_token_by_description(self, token_description: str):
         if token_description not in self.tokens_by_description:
             raise ValueError(f"Could not find token matching description '{token_description}'.")
         return self.delete_token(self.tokens_by_description[token_description].token_id)
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/attributes.py` & `ipfabric-6.8.1/ipfabric/settings/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime
 from typing import Optional, List, Any
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
+from ipfabric.tools import raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 ATTR_REGEX = re.compile(r"^[a-zA-Z]\w*[a-zA-Z0-9]+$")
 
 
 @deprecated_args_decorator(version="6.10", no_args=False, kwargs_only=True)
@@ -83,31 +84,29 @@
         :param value: str: Attribute value (case sensitive)
         :return:
         """
         self.check_attribute_name({name})
         attribute = dict(name=name, sn=serial_number, value=value)
         if self.snapshot_id:
             return self.set_attributes_by_sn([attribute])
-        resp = self.client.post(self.endpoint, json=attribute)
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.post(self.endpoint, json=attribute))
         return resp.json()
 
     def set_attributes_by_sn(self, attributes: List[dict]):
         """
         Sets a list of Attributes for devices based on serial numbers.
         Will Add or Update Attributes.
         :param attributes: list: [{'sn': 'IPF SERIAL NUMBER', 'name': 'attributeName', 'value': 'SITE NAME'}]
         :return:
         """
         self.check_attribute_name({v["name"] for v in attributes})
         payload = dict(attributes=attributes)
         if self.snapshot_id:
             payload["snapshot"] = self.snapshot_id
-        resp = self.client.put(self.endpoint, json=payload)
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.put(self.endpoint, json=payload))
         return resp.json()
 
     def set_site_by_sn(self, serial_number, site_name):
         """
         Set a single site by serial number
         If Global will Error if already set.
         If Local will not error and either Add or Update
@@ -131,70 +130,70 @@
 
         Args:
             serial_numbers: Serial Numbers
         """
         payload = dict(attributes=dict(sn=[str(i) for i in serial_numbers]))
         if self.snapshot_id:
             payload["snapshot"] = self.snapshot_id
-        resp = self.client.request("DELETE", self.endpoint, json=payload)
-        resp.raise_for_status()
+        raise_for_status(self.client.request("DELETE", self.endpoint, json=payload))
         return True
 
     def delete_attribute_by_id(self, *attribute_ids):
         """Deletes attributes by Attribute ID(s)
 
         Args:
             attribute_ids: Attribute IDs
         """
         payload = dict(attributes=dict(id=[str(i) for i in attribute_ids]))
         if self.snapshot_id:
             payload["snapshot"] = self.snapshot_id
-        resp = self.client.request("DELETE", self.endpoint, json=payload)
-        resp.raise_for_status()
+        raise_for_status(self.client.request("DELETE", self.endpoint, json=payload))
         return True
 
     def delete_attribute(self, *attributes):
         """
         Deletes attributes by Attribute
         :param attributes: dict: Attribute dictionaries
         :return:
         """
         return self.delete_attribute_by_id(*[str(i["id"]) for i in attributes])
 
     def update_local_attr_from_global(
         self,
         wait_for_load: bool = True,
-        # wait_for_assurance: bool = True,  # TODO: NIM-14475 - 6.8.2 fix
+        wait_for_assurance: bool = True,
         timeout: int = 60,
         retry: int = 5,
     ) -> bool:
         """
         Updates Snapshot Local Attributes based on Global.
         Returns True is successfully completed, False if the snapshot load did not complete if required.
         """
-        wait_for_assurance = False
         if not self.snapshot_id:
             raise ImportError("Please initialize Attributes class with a snapshot_id.")
         recalc = self.check_sites_recalculation()
         ts = int(datetime.now().timestamp() * 1000)
-        resp = self.client.post("/attributes/local/update-from-global", json={"snapshot": self.snapshot_id})
-        resp.raise_for_status()
+        raise_for_status(self.client.post("/attributes/local/update-from-global", json={"snapshot": self.snapshot_id}))
 
-        if recalc and (wait_for_load or wait_for_assurance):
-            if not self.client.snapshots[self.snapshot_id]._check_load_status(
-                    ts, wait_for_assurance, timeout, retry, 'recalculate'
-            ):
-                return False
+        if (
+            recalc
+            and (wait_for_load or wait_for_assurance)
+            and not self.client.snapshots[self.snapshot_id]._check_load_status(
+                ts, wait_for_assurance, timeout, retry, "recalculate"
+            )
+        ):
+            return False
         self.client.snapshots[self.snapshot_id]._refresh_status()
         if self.client.snapshots[self.snapshot_id].loaded and self.client.snapshot_id == self.snapshot_id:
             self.client.devices.update()
         return True
 
     def check_sites_recalculation(self) -> bool:
         """Checks if updating local attributes requires recalculation."""
         if not self.snapshot_id:
             raise ImportError("Please initialize Attributes class with a snapshot_id.")
-        resp = self.client.post(
-            "/attributes/local/update-from-global/check-sites-recalculation", json={"snapshot": self.snapshot_id}
+        resp = raise_for_status(
+            self.client.post(
+                "/attributes/local/update-from-global/check-sites-recalculation", json={"snapshot": self.snapshot_id}
+            )
         )
-        resp.raise_for_status()
         return resp.json()["needsRecalculation"]
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/authentication.py` & `ipfabric-6.8.1/ipfabric/settings/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional, Any, Union, ClassVar, Dict
 
 from dateutil import parser
 from pydantic import BaseModel, Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
+from ipfabric.tools import raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 
 class Expiration(BaseModel):
     enabled: bool
     value: Optional[datetime] = None
@@ -62,25 +63,23 @@
         return self._enables
 
     def get_credentials(self) -> Dict[str, Credential]:
         """
         Get all credentials and sets them in the Authentication.credentials
         :return: self.credentials
         """
-        res = self.client.get(self._cred_url)
-        res.raise_for_status()
+        res = raise_for_status(self.client.get(self._cred_url))
         return {cred["priority"]: Credential(**cred) for cred in res.json()["data"]}
 
     def get_enables(self) -> Dict[str, Privilege]:
         """
         Get all privileges (enable passwords) and sets them in the Authentication.enables
         :return:
         """
-        res = self.client.get(self._priv_url)
-        res.raise_for_status()
+        res = raise_for_status(self.client.get(self._priv_url))
         return {priv["priority"]: Privilege(**priv) for priv in res.json()["data"]}
 
     def _create_payload(self, username, password, notes, network, excluded, expiration):
         networks = network or ["0.0.0.0/0"]
         excluded = excluded or list()
         if expiration:
             expires = dict(
@@ -121,16 +120,15 @@
         :param config_mgmt: bool: Default False - do not use for configuration management
         :param expiration: str: Optional date for expiration, if none then do not expire.
                                 To ensure correct date use YYYYMMDD or MM/DD/YYYY formats
         :return: Credential: Obj: Credential Obj with ID and encrypted password
         """
         payload = self._create_payload(username, password, notes, networks, excluded, expiration)
         payload.update({"syslog": config_mgmt})
-        res = self.client.post(self._cred_url, json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.client.post(self._cred_url, json=payload))
         self.get_credentials()
         cred = Credential(**res.json())
         logger.info(f"Created credential with username {cred.username} and ID of {cred.credential_id}")
         return cred
 
     def create_enable(
         self,
@@ -152,65 +150,60 @@
         :param excluded: list: Optional list of networks to exclude
         :param expiration: str: Optional date for expiration, if none then do not expire.
                                 To ensure correct date use YYYYMMDD or MM/DD/YYYY formats
         :return: Privilege: Obj: Privilege Obj with ID and encrypted password
         """
         payload = self._create_payload(username, password, notes, networks, excluded, expiration)
         payload["includeNetworks"] = payload.pop("network")
-        res = self.client.post(self._priv_url, json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.client.post(self._priv_url, json=payload))
         self.get_enables()
         priv = Privilege(**res.json())
         logger.info(f"Created enable password with username {priv.username} and ID of {priv.privilege_id}")
         return priv
 
-    def delete_credential(self, credential: Union[Credential, str]) -> None:
+    def delete_credential(self, credential: Union[Credential, str]) -> None:  # TODO: Change return
         """
         Deletes a credential and updates Authentication.credentials with new priorities.
         :param credential: Union[Credential, str]: Cred ID in a string or Credential object
         :return:
         """
         cred = credential.credential_id if isinstance(credential, Credential) else credential
-        res = self.client.request("DELETE", self._cred_url, json=[cred])
-        res.raise_for_status()
+        raise_for_status(self.client.request("DELETE", self._cred_url, json=[cred]))
         self.get_credentials()
         logger.warning(f"Deleted credential ID {cred}")
 
-    def delete_enable(self, enable: Union[Privilege, str]) -> None:
+    def delete_enable(self, enable: Union[Privilege, str]) -> None:  # TODO: Change return
         """
         Deletes an enable password (privilege account) and updates Authentication.enable with new priorities.
         :param enable: Union[Privilege, str]: Enable ID in a string or Privilege object
         :return:
         """
         priv = enable.privilege_id if isinstance(enable, Privilege) else enable
-        res = self.client.request("DELETE", self._priv_url, json=[priv])
-        res.raise_for_status()
+        raise_for_status(self.client.request("DELETE", self._priv_url, json=[priv]))
         self.get_enables()
         logger.warning(f"Deleted enable password ID {priv}")
 
     def update_cred_priority(self, credentials: dict) -> dict:
         """
         Updates the priority of credentials.  Reorder Authentication.credentials dictionary and submit to this method.
         :param credentials: dict: {priority: Credential}
         :return: self.credentials: dict: {priority: Credential}
         """
         payload = [dict(id=c.credential_id, priority=p) for p, c in credentials.items()]
-        res = self.client.patch(self._cred_url, json=payload)
-        res.raise_for_status()
+        raise_for_status(self.client.patch(self._cred_url, json=payload))
         self.get_credentials()
         return self.credentials
 
     def update_enable_priority(self, enables: dict) -> dict:
         """
         Updates the priority of enable passwords.  Reorder Authentication.enables dictionary and submit to this method.
         :param enables: dict: {priority: Privilege}
         :return: self.enables: dict: {priority: Privilege}
         """
         payload = [dict(id=e.privilege_id, priority=p) for p, e in enables.items()]
-        res = self.client.patch(self._priv_url, json=payload)
-        res.raise_for_status()
+        raise_for_status(self.client.patch(self._priv_url, json=payload))
         self.get_enables()
         return self.enables
 
     @staticmethod
     def _check_networks(subnets):
         return [IPv4Network(network).with_prefixlen for network in subnets]
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/discovery.py` & `ipfabric-6.8.1/ipfabric/settings/discovery.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Any, Optional, List
 
 from pydantic import BaseModel, Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
+from ipfabric.tools import raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 
 class Networks(BaseModel):
     exclude: List[str]
     include: List[str]
@@ -24,23 +25,21 @@
         self._networks = self._get_networks()
 
     @property
     def networks(self):
         return self._networks
 
     def _get_networks(self):
-        res = self.client.get("settings")
-        res.raise_for_status()
+        res = raise_for_status(self.client.get("settings"))
         return Networks(**res.json()["networks"])
 
     def update_discovery_networks(self, subnets: list, include: bool = False):
         payload = dict()
         payload["networks"] = dict()
         if include:
             payload["networks"]["include"] = subnets
             payload["networks"]["exclude"] = self.networks.exclude
         else:
             payload["networks"]["exclude"] = subnets
             payload["networks"]["include"] = self.networks.include
-        res = self.client.patch("settings", json=payload)
-        res.raise_for_status()
+        res = raise_for_status(self.client.patch("settings", json=payload))
         return Networks(**res.json()["networks"])
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/local_users.py` & `ipfabric-6.8.1/ipfabric/settings/local_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Any, Optional, List, Dict
 
 from httpx import HTTPStatusError
 from pydantic import Field, BaseModel
 
 from ipfabric.models import User
-from ipfabric.tools.shared import TIMEZONES
+from ipfabric.tools.shared import TIMEZONES, raise_for_status
 from .rbac import Roles
 
 logger = logging.getLogger("ipfabric")
 
 
 class LocalUsers(BaseModel):
     client: Any = Field(exclude=True)
@@ -45,16 +45,15 @@
 
     def get_user_by_id(self, user_id: str):
         """
         Gets a user by ID
         :param user_id: Union[str, int]: User ID to filter
         :return: User
         """
-        resp = self.client.get("users/" + str(user_id))
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.get("users/" + str(user_id)))
         user = resp.json()
         return User(**user)
 
     def add_user(
         self,
         username: str,
         password: str,
@@ -77,22 +76,20 @@
             "username": username,
             "password": password,
             "roleIds": roles,
         }
         if timezone.lower() not in TIMEZONES:
             raise ValueError(f"Timezone `{timezone}` is not located. Please see `ipfabric.tools.shared.TIMEZONES`.")
         payload["timezone"] = TIMEZONES[timezone.lower()]
-        resp = self.client.post("users", json=payload)
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.post("users", json=payload))
         self._users = self.get_users()
         return self.users_by_id[resp.json()["id"]]
 
     def delete_user(self, user_id: str) -> bool:
         """
         Deletes a user and returns list of remaining users
         :param user_id:
         :return:
         """
-        resp = self.client.delete("users/" + str(user_id))
-        resp.raise_for_status()
+        raise_for_status(self.client.delete("users/" + str(user_id)))
         self._users = self.get_users()
         return True
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/rbac.py` & `ipfabric-6.8.1/ipfabric/settings/rbac.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Optional, List, Dict, Union
 
 from httpx import HTTPStatusError
 from pydantic import BaseModel, Field, PrivateAttr
 
 from ipfabric.models.oas import Endpoint
 from ipfabric.models.rbac import Role, Policy
-from ipfabric.tools import valid_slug
+from ipfabric.tools import valid_slug, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 
 class Policies(BaseModel):
     client: Any = Field(exclude=True)
     _policies: Optional[List[Policy]] = PrivateAttr(None)
@@ -90,16 +90,15 @@
             "description": description,
         }
         if api_scope_ids:
             payload["apiScopeIds"] = fmt_api_scopes
         else:
             payload["attributeFilters"] = attribute_filters
 
-        resp = self.client.post(f"policies/scopes/{'api' if api_scope_ids else 'attributes'}", json=payload)
-        resp.raise_for_status()
+        raise_for_status(self.client.post(f"policies/scopes/{'api' if api_scope_ids else 'attributes'}", json=payload))
         return self.get_policies(name)
 
     def create_policy(
         self,
         name: str,
         description: str,
         api_scope_ids: List[Union[int, str, Endpoint]] = None,
@@ -139,16 +138,17 @@
         """Deletes a Role.
 
         Args:
             policy: Policy ID or Policy object
 
         Returns: True
         """
-        resp = self.client.delete(f"policies/{policy.policy_id if isinstance(policy, Policy) else str(policy)}")
-        resp.raise_for_status()
+        raise_for_status(
+            self.client.delete(f"policies/{policy.policy_id if isinstance(policy, Policy) else str(policy)}")
+        )
         return True
 
     def delete_policy(self, policy: Union[int, str, Policy]) -> bool:
         _ = self._delete_policy(policy)
         self.update()
         return _
 
@@ -188,27 +188,28 @@
             api_scope_ids = set(self._fmt_api_scopes(api_scope_ids))
             if not replace_api_scopes:
                 api_scope_ids.update(set(policy.api_scope_ids))
             payload["apiScopeIds"] = list(api_scope_ids)
         else:
             payload["attributeFilters"] = attribute_filters
 
-        resp = self.client.patch(
-            f"policies/scopes/{'api' if policy.scope_type == 'apiScopes' else 'attributes'}/{policy.policy_id}",
-            json=payload,
+        resp = raise_for_status(
+            self.client.patch(
+                f"policies/scopes/{'api' if policy.scope_type == 'apiScopes' else 'attributes'}/{policy.policy_id}",
+                json=payload,
+            )
         )
-        resp.raise_for_status()
         self.update()
         return self.policies_by_id[resp.json()["id"]]
 
 
 class Roles(BaseModel):
     client: Any
     _roles: Optional[List[Role]] = None
-    _policies: Optional[Policy] = PrivateAttr(None)
+    _policies: Optional[Policies] = PrivateAttr(None)
 
     def model_post_init(self, __context: Any) -> None:
         self._policies = self.client.settings.policies
         self._roles = self.get_roles()
 
     def update(self):
         self._policies.update()
@@ -266,16 +267,15 @@
 
     def _create_role(self, name: str, description: str, policy_ids: List[Union[int, str, Policy]]) -> Role:
         payload = {
             "name": valid_slug(name),
             "description": description,
             "policyIds": [_.policy_id if isinstance(_, Policy) else str(_) for _ in policy_ids],
         }
-        resp = self.client.post("roles", json=payload)
-        resp.raise_for_status()
+        raise_for_status(self.client.post("roles", json=payload))
         return self.get_roles(name)
 
     def create_role(self, name: str, description: str, policy_ids: List[Union[int, str, Policy]]) -> Role:
         role = self._create_role(name, description, policy_ids)
         self.update()
         return role
 
@@ -312,16 +312,15 @@
         """Deletes a Role.
 
         Args:
             role: Role ID or Role object
 
         Returns: True
         """
-        resp = self.client.delete(f"roles/{role.role_id if isinstance(role, Role) else str(role)}")
-        resp.raise_for_status()
+        raise_for_status(self.client.delete(f"roles/{role.role_id if isinstance(role, Role) else str(role)}"))
         return True
 
     def delete_role(self, role: Union[int, str, Role]) -> bool:
         _ = self._delete_role(role)
         self.update()
         return _
 
@@ -363,11 +362,10 @@
         elif policy_ids:
             policies.update({_.policy_id if isinstance(_, Policy) else str(_) for _ in policy_ids})
         payload = {
             "description": description or role.description,
             "name": name or role.name,
             "policyIds": list(policies),
         }
-        resp = self.client.put(f"roles/{role.role_id}", json=payload)
-        resp.raise_for_status()
+        resp = raise_for_status(self.client.put(f"roles/{role.role_id}", json=payload))
         self.update()
         return self.roles_by_id[resp.json()["id"]]
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/seeds.py` & `ipfabric-6.8.1/ipfabric/settings/seeds.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from ipaddress import IPv4Interface, AddressValueError
 from typing import Any
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
+from ipfabric.tools import raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 
 @deprecated_args_decorator(version="6.10", no_args=False, kwargs_only=True)
 @dataclass
 class Seeds:
     client: Any = Field(exclude=True)
 
     @property
     def seeds(self):
-        res = self.client.get("settings/seed")
-        res.raise_for_status()
-        return res.json()
+        return raise_for_status(self.client.get("settings/seed")).json()
 
     @staticmethod
     def _check_seeds(seeds):
         valid = True
         for seed in seeds:
             try:
                 IPv4Interface(seed)
@@ -37,17 +36,15 @@
         Sets the seeds with supplied list, will override current configuration.
         :param seeds: list: List of IP addresses or networks
         :return: list: Updated list of configured seeds
         """
         if not isinstance(seeds, list):
             raise SyntaxError("Seeds must be a list of IP Addresses or networks")
         if self._check_seeds(seeds):
-            res = self.client.put("settings/seed", json=seeds)
-            res.raise_for_status()
-            return res.json()
+            return raise_for_status(self.client.put("settings/seed", json=seeds)).json()
 
     def add_seeds(self, seeds):
         """
         Adds a single seed or list of seeds to the current configuration
         :param seeds: list: List of IP addresses or networks
         :return: list: Updated list of configured seeds
         """
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/settings.py` & `ipfabric-6.8.1/ipfabric/settings/settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/site_separation.py` & `ipfabric-6.8.1/ipfabric/settings/site_separation.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Optional
 from warnings import warn
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
+from ipfabric.tools import raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 
 @deprecated_args_decorator(version="6.10", no_args=False, kwargs_only=True)
 @dataclass
 class SiteSeparation:
@@ -26,17 +27,15 @@
             logger.warning(msg)
             self.client = self.ipf
 
     def get_separation_rules(self):
         return self.client.get("settings/site-separation").json()
 
     def _post_rule(self, data):
-        resp = self.client.post("settings/site-separation/test-regex", json=data)
-        resp.raise_for_status()
-        return resp.json()
+        return raise_for_status(self.client.post("settings/site-separation/test-regex", json=data)).json()
 
     @staticmethod
     def _create_rule(transformation, regex):
         transformation = transformation.lower()
         if transformation not in ["uppercase", "lowercase", "none"]:
             raise SyntaxError('Transformation type is not in ["uppercase", "lowercase", "none"].')
         return {"regex": regex, "transformation": transformation}
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/vendor_api.py` & `ipfabric-6.8.1/ipfabric/settings/vendor_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Prisma,
     RuckusVirtualSmartZone,
     SilverPeak,
     Versa,
     Viptela,
     NSXT,
 )
+from ipfabric.tools import raise_for_status
 
 API_MODELS = (
     AWS,
     Azure,
     CheckPointApiKey,
     CheckPointUserAuth,
     CiscoAPIC,
@@ -66,43 +67,35 @@
     _api_url: ClassVar[str] = "settings/vendor-api"
 
     def get_vendor_apis(self) -> list:
         """
         Get all vendor apis and sets them in the Authentication.apis
         :return: self.credentials
         """
-        res = self.client.get(self._api_url)
-        res.raise_for_status()
-        return res.json()
+        return raise_for_status(self.client.get(self._api_url)).json()
 
     def add_vendor_api(self, api: Union[API_MODELS]) -> dict:
         params = api.model_dump()
-        res = self.client.post(self._api_url, json=params)
-        res.raise_for_status()
-        return res.json()
+        return raise_for_status(self.client.post(self._api_url, json=params)).json()
 
     @staticmethod
     def _return_api_id(api_id: Union[dict, str, int]) -> str:
         if isinstance(api_id, dict):
             api_id = api_id["id"]
         elif isinstance(api_id, int):
             api_id = str(api_id)
         return api_id
 
     def delete_vendor_api(self, api_id: Union[dict, str, int]):
         api_id = self._return_api_id(api_id)
-        res = self.client.delete(self._api_url + "/" + api_id)
-        res.raise_for_status()
-        return res.status_code
+        return raise_for_status(self.client.delete(self._api_url + "/" + api_id)).status_code
 
     def _enable_api(self, api_id: Union[dict, str, int], enable: bool = True) -> int:
         api_id = self._return_api_id(api_id)
-        res = self.client.patch(self._api_url + "/" + api_id, json={"isEnabled": enable})
-        res.raise_for_status()
-        return res.status_code
+        return raise_for_status(self.client.patch(self._api_url + "/" + api_id, json={"isEnabled": enable})).status_code
 
     def enable_vendor_api(self, api_id: Union[dict, str, int]) -> int:
         return self._enable_api(api_id)
 
     def disable_vendor_api(self, api_id: Union[dict, str, int]) -> int:
         return self._enable_api(api_id, False)
 
@@ -140,10 +133,8 @@
             default = {
                 k: v for k, v in vars(TYPE_TO_MODEL[params["type"]].model_construct()).items() if k in CONNECTION_PARAMS
             }
             params.update(default)
 
         self._validate_update(params)
 
-        res = self.client.put(self._api_url + "/" + str(api_id), json=params)
-        res.raise_for_status()
-        return res.json()
+        return raise_for_status(self.client.put(self._api_url + "/" + str(api_id), json=params)).json()
```

### Comparing `ipfabric-6.8.0b0/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.8.1/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/__init__.py` & `ipfabric-6.8.1/ipfabric/tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .configuration import DeviceConfigs, trigger_backup
 from .discovery_history import DiscoveryHistory
 from .restore_intents import RestoreIntents
-from .shared import parse_mac, TIMEZONES, VALID_REFS, validate_ip_network_str, VALID_IP, valid_slug
+from .shared import parse_mac, TIMEZONES, VALID_REFS, validate_ip_network_str, VALID_IP, valid_slug, raise_for_status
 from .site_seperation_report import map_devices_to_rules
 from .vulnerabilities import Vulnerabilities
 
 __all__ = [
     "DeviceConfigs",
     "trigger_backup",
     "Vulnerabilities",
@@ -14,8 +14,9 @@
     "map_devices_to_rules",
     "parse_mac",
     "TIMEZONES",
     "VALID_REFS",
     "validate_ip_network_str",
     "VALID_IP",
     "valid_slug",
+    "raise_for_status",
 ]
```

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/configuration.py` & `ipfabric-6.8.1/ipfabric/tools/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ipaddress import IPv4Address, AddressValueError
 from typing import Any, Union, Optional
 
 from pydantic import BaseModel, Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
-from ipfabric.tools.shared import date_parser
+from ipfabric.tools.shared import date_parser, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 DEFAULT_SNAPSHOT = "$last"
 NAMED_SNAPSHOTS = [DEFAULT_SNAPSHOT, "$prev", "$first"]
 
 
 def trigger_backup(ipf, sn: str = None, ip: str = None):
@@ -20,17 +20,15 @@
         payload = {"sn": sn}
     else:
         try:
             ip = str(IPv4Address(ip))
         except AddressValueError:
             raise ValueError(f"Invalid IP Address, CIDR is not allowed: {ip}")
         payload = {"ip": ip}
-    res = ipf.post("/discovery/trigger-config-backup", json=payload)
-    res.raise_for_status()
-    return res.status_code
+    return raise_for_status(ipf.post("/discovery/trigger-config-backup", json=payload)).status_code
 
 
 class Config(BaseModel):
     config_id: str = Field(None, alias="id")
     sn: str
     hostname: str
     config_hash: str = Field(None, alias="hash")
@@ -44,19 +42,20 @@
         Args:
             client: IPF Client
             sanitized: bool to determine to return sensitive data
 
         Returns:
             string containing config of a device
         """
-        res = client.get(
-            "/tables/management/configuration/download",
-            params=dict(hash=self.config_hash, sanitized=sanitized),
+        res = raise_for_status(
+            client.get(
+                "/tables/management/configuration/download",
+                params=dict(hash=self.config_hash, sanitized=sanitized),
+            )
         )
-        res.raise_for_status()
         self.text = res.text
         return res.text
 
 
 @deprecated_args_decorator(version="6.10", no_args=False, kwargs_only=True)
 @dataclass
 class DeviceConfigs:
@@ -168,19 +167,20 @@
         Args:
             cfg: Config from get_configuration method
             sanitized: bool to determine to return sensitive data
 
         Returns:
             string containing config of a device
         """
-        res = self.client.get(
-            "/tables/management/configuration/download",
-            params=dict(hash=cfg.config_hash, sanitized=sanitized),
+        res = raise_for_status(
+            self.client.get(
+                "/tables/management/configuration/download",
+                params=dict(hash=cfg.config_hash, sanitized=sanitized),
+            )
         )
-        res.raise_for_status()
         cfg.text = res.text
         return cfg
 
     @staticmethod
     def _get_hash(configs, date):
         if isinstance(date, tuple):
             start = date_parser(date[0])
@@ -217,10 +217,8 @@
     def get_log(self, device: str, snapshot_id: str = None):
         device = self._validate_device(device, snapshot_id=snapshot_id, log=True)
         if not device["sn"]:
             return None
         return self.get_text_log(device)
 
     def get_text_log(self, device: dict):
-        res = self.client.get("/os/logs/task/" + device["taskKey"])
-        res.raise_for_status()
-        return res.text
+        return raise_for_status(self.client.get("/os/logs/task/" + device["taskKey"])).text
```

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/discovery_history.py` & `ipfabric-6.8.1/ipfabric/tools/discovery_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Any, Union, List
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
-from ipfabric.tools.shared import convert_timestamp, date_parser
+from ipfabric.tools.shared import convert_timestamp, date_parser, raise_for_status
 
 logger = logging.getLogger("ipfabric")
 
 COLUMNS = ["id", "sn", "hostname", "loginIp", "loginType", "ts", "username", "usernameNotes"]
 
 
 @dataclass
@@ -101,16 +101,15 @@
             filters = {"ts": ["gte", int(date_parser(daterange).timestamp() * 1000)]}
         return self.get_all_history(columns=columns, sort=sort, filters=filters, ts_format=ts_format)
 
     def delete_history(self, history_id: Union[List[str], str]):
         if isinstance(history_id, str):
             history_id = [history_id]
 
-        resp = self.ipf.request("DELETE", "discovery/history", json=history_id)
-        resp.raise_for_status()
+        raise_for_status(self.ipf.request("DELETE", "discovery/history", json=history_id))
         logger.debug("Deleted the following discovery history IDs:")
         logger.debug(f"{history_id}")
         return True
 
     def delete_history_prior_to_ts(self, timestamp: Union[int, str]) -> list:
         """removes history from IPF based on the date passed to timestamp
```

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/policies.json` & `ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/7/policies.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/roles.json` & `ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/7/roles.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/policies.json` & `ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/8/policies.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/roles.json` & `ipfabric-6.8.1/ipfabric/tools/managed_rbac/v6/8/roles.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/rbac.py` & `ipfabric-6.8.1/ipfabric/tools/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/restore_intents.py` & `ipfabric-6.8.1/ipfabric/tools/restore_intents.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from datetime import datetime
 from os import path
 from typing import Any, Union
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
+from ipfabric.tools.shared import raise_for_status
+
 logger = logging.getLogger("ipfabric")
 
 
 @dataclass
 class RestoreIntents:
     ipf: Any = Field(exclude=True)
 
@@ -57,49 +59,44 @@
         old_intents = self.ipf.get("reports").json()
         old_intent_groups = self.ipf.get("reports/groups").json()
         old_dashboard = json.loads(self.ipf.get("settings/dashboard").text, object_pairs_hook=OrderedDict)
         self._save_to_file(old_intents, old_intent_groups, old_dashboard)
 
         logger.info("Deleting All Intents.")
         for i in old_intents:
-            res = self.ipf.delete(f"reports/{i['id']}")
-            res.raise_for_status()
+            raise_for_status(self.ipf.delete(f"reports/{i['id']}"))
         logger.info("Deleted All Intents.")
 
         logger.info("Deleting All Intent Groups.")
         for g in old_intent_groups:
-            res = self.ipf.delete(f"reports/groups/{g['id']}")
-            res.raise_for_status()
+            raise_for_status(self.ipf.delete(f"reports/groups/{g['id']}"))
         logger.info("Deleted All Intent Groups.")
 
         intent_mapping = {i["id"]: None for i in intents}
         logger.info("Creating Intent Verification Rules.")
         for i in intents:
             i["groups"] = []
             i.pop("custom", None)
             src_id = i.pop("id", None)
-            res = self.ipf.post("reports", json=i)
-            res.raise_for_status()
+            res = raise_for_status(self.ipf.post("reports", json=i))
             intent_mapping[src_id] = res.json()["id"]
         logger.info("Created Intent Verification Rules.")
 
         group_mapping = {g["id"]: None for g in groups}
         logger.info("Creating Intent Groups.")
         for g in groups:
             for c in g["children"]:
                 c["id"] = intent_mapping[c["id"]]
             src_id = g.pop("id", None)
             g.pop("custom", None)
-            res = self.ipf.post("reports/groups", json=g)
-            res.raise_for_status()
+            res = raise_for_status(self.ipf.post("reports/groups", json=g))
             group_mapping[src_id] = res.json()["id"]
         logger.info("Created Intent Groups.")
 
         raw_dashboard = json.dumps(dashboard)
         logger.info("Creating Dashboard.")
         for src_group, dst_group in group_mapping.items():
             raw_dashboard = raw_dashboard.replace(src_group, dst_group)
 
-        res = self.ipf.put("settings/dashboard", json=json.loads(raw_dashboard))
-        res.raise_for_status()
+        raise_for_status(self.ipf.put("settings/dashboard", json=json.loads(raw_dashboard)))
         logger.info("Created Dashboard.")
         return True
```

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/shared.py` & `ipfabric-6.8.1/ipfabric/tools/shared.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,67 @@
 import logging
 import re
 from datetime import datetime, timezone
 from ipaddress import IPv4Address, IPv4Network, IPv4Interface, AddressValueError
+from json import JSONDecodeError
 from typing import Union
 
 import macaddress
 from dateutil import parser
+from httpx import HTTPStatusError, Response
 from pytz import BaseTzInfo, utc
 
 logger = logging.getLogger("ipfabric")
 
 LAST_ID, PREV_ID, LASTLOCKED_ID = "$last", "$prev", "$lastLocked"
 VALID_REFS = [LAST_ID, PREV_ID, LASTLOCKED_ID]
 VALID_IP = Union[IPv4Address, IPv4Network, IPv4Interface]
 SLUG = re.compile(r"^[a-zA-Z0-9_\-.#:]*$")
 
 
+def raise_for_status(response: Response) -> Response:
+    """
+    Raise the `HTTPStatusError` if one occurred.
+    """
+    request = response._request
+    if request is None:
+        raise RuntimeError(
+            "Cannot call `raise_for_status` as the request " "instance has not been set on this response."
+        )
+
+    if response.is_success:
+        return response
+
+    if response.has_redirect_location:
+        message = (
+            "{error_type} '{0.status_code} {0.reason_phrase}' for url '{0.url}'\n"
+            "Redirect location: '{0.headers[location]}'"
+        )
+    else:
+        try:
+            msg = response.json()
+            message = (
+                "{error_type} '{0.status_code} {0.reason_phrase}' for url '{0.url}'\n"
+                f"{msg['code']}: {msg['message']}"
+            )
+        except (JSONDecodeError, TypeError, KeyError):
+            message = "{error_type} '{0.status_code} {0.reason_phrase}' for url '{0.url}'"
+
+    status_class = response.status_code // 100
+    error_types = {
+        1: "Informational response",
+        3: "Redirect response",
+        4: "Client error",
+        5: "Server error",
+    }
+    error_type = error_types.get(status_class, "Invalid status code")
+    message = message.format(response, error_type=error_type)
+    raise HTTPStatusError(message, request=request, response=response)
+
+
 def valid_slug(name: str):
     if not SLUG.match(name):
         raise ValueError(f"{name} is not a valid slug/name and must match regex {SLUG.pattern}.")
     return name
 
 
 def validate_ip_network(ip: Union[str, VALID_IP]) -> IPv4Network:
```

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.8.1/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.8.1/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/LICENSE` & `ipfabric-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/NOTICES.md` & `ipfabric-6.8.1/NOTICES.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/pyproject.toml` & `ipfabric-6.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.8.0b0"
+version = "v6.8.1"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `ipfabric-6.8.0b0/README.md` & `ipfabric-6.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.8.0b0/PKG-INFO` & `ipfabric-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.8.0b0
+Version: 6.8.1
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.8,<4.0
```

