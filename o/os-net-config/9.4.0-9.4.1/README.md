# Comparing `tmp/os-net-config-9.4.0.tar.gz` & `tmp/os-net-config-9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/os-net-config-9.4.0.tar", last modified: Fri Jun 21 13:56:12 2019, max compression
+gzip compressed data, was "dist/os-net-config-9.4.1.tar", last modified: Thu Sep 12 09:40:06 2019, max compression
```

## Comparing `os-net-config-9.4.0.tar` & `os-net-config-9.4.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/zuul.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      379 2019-06-21 13:51:35.000000 os-net-config-9.4.0/zuul.d/layout.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-06-21 13:51:32.000000 os-net-config-9.4.0/setup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      164 2019-06-21 13:51:35.000000 os-net-config-9.4.0/HACKING.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      103 2019-06-21 13:51:32.000000 os-net-config-9.4.0/.coveragerc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/releasenotes/notes/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      216 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/allow-list-of-routes-to-be-empty-323690796760630d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      236 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/retry_ovs-appctl-6734b087ab6db80b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      168 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/restart-ivs-nvfswitch-after-change-0825ea78aae8f138.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      382 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/log-mapping-file-8b2a9d8f6a81ba99.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      248 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/add_contrail_vrouter_vlan_linux_bond_type-0a89f3499a7ab08b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      522 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/policy-based-routing-3fa1200ae155bbee.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      346 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/add-neutron-route-schema-support-e8e20a8c3b79d14d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      533 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/modify-interface-without-restart-d55949572017d52f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      109 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/dpdk-on-mellanox-nics-1d8fdb843a4e2b60.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      175 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/enable-setting-domain-5557e2441c23a5a5.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      325 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/sriov-vf-in-hosts-529c2bf0cb3294b3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      460 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/log-info-nic-discovery-f54ace7639890fdf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      222 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/notes/check-ovs-ef665418762ca123.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/releasenotes/source/_static/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/source/_static/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      147 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/source/queens.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6461 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      106 2019-06-21 13:51:32.000000 os-net-config-9.4.0/releasenotes/source/unreleased.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      139 2019-06-21 13:51:35.000000 os-net-config-9.4.0/releasenotes/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      543 2019-06-21 13:51:35.000000 os-net-config-9.4.0/CONTRIBUTING.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       54 2019-06-21 13:51:32.000000 os-net-config-9.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2194 2019-06-21 13:56:12.000000 os-net-config-9.4.0/AUTHORS
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10142 2019-06-21 13:51:32.000000 os-net-config-9.4.0/LICENSE
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1013 2019-06-21 13:51:35.000000 os-net-config-9.4.0/tox.ini
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       16 2019-06-21 13:51:32.000000 os-net-config-9.4.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/etc/os-net-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/etc/os-net-config/samples/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      490 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/nfvswitch.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1308 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/routes.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      586 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      463 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_ovs_extra.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      800 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_vlan.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      281 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/vpp_interface.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      770 2019-06-21 13:51:35.000000 os-net-config-9.4.0/etc/os-net-config/samples/interface.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      525 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bond.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      325 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bond.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      427 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_vlan.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      280 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter_dpdk.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      464 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ib_interface.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      410 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter_dpdk_bond.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      606 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bond_mapped.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      342 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/mapping_mnemonic.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      687 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ivs.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1463 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk_bond.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      147 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/linux_bridge.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      740 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ovs_patch_port.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      249 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      460 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/vpp_bond.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5058 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      517 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/team.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      171 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_fail_mode.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      221 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_dhcp.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1208 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk_bond.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      734 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/nfvswitch.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3435 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      506 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/mapping.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      159 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter_vlan.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      365 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/team.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      398 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/vpp_bond.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      278 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter_vlan.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       75 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/mapping_report.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      456 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/linux_bond_networkmanager.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      198 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter_dpdk.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      761 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/vpp_interface.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2535 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_switchdev.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4757 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_ovs_dpdk.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      340 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_fail_mode.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3186 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_ovs_dpdk.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      530 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ovs_patch_port.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      448 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ivs.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      263 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_ovs_extra.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      231 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/linux_bond.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      308 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ib_interface.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      238 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/contrail_vrouter_dpdk_bond.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1084 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      573 2019-06-21 13:51:35.000000 os-net-config-9.4.0/etc/os-net-config/samples/interface.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2172 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_switchdev.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      412 2019-06-21 13:51:32.000000 os-net-config-9.4.0/etc/os-net-config/samples/bridge_dhcp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4714 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4575 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/doc/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       83 2019-06-21 13:51:32.000000 os-net-config-9.4.0/doc/source/usage.rst
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     2437 2019-06-21 13:51:35.000000 os-net-config-9.4.0/doc/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       74 2019-06-21 13:51:32.000000 os-net-config-9.4.0/doc/source/contributing.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       29 2019-06-21 13:51:32.000000 os-net-config-9.4.0/doc/source/readme.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      207 2019-06-21 13:51:32.000000 os-net-config-9.4.0/doc/source/installation.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      508 2019-06-21 13:51:32.000000 os-net-config-9.4.0/doc/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       88 2019-06-21 13:51:32.000000 os-net-config-9.4.0/.mailmap
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      731 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/impl_iproute.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13293 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      680 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/version.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    79220 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/objects.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7202 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/validator.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9896 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/impl_eni.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13783 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/sriov_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12914 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/cli.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    51039 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/schema.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    77034 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/impl_ifcfg.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:56:12.000000 os-net-config-9.4.0/os_net_config/tests/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/tests/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      825 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/tests/test_os_net_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    73201 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/tests/test_objects.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    84910 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/tests/test_impl_ifcfg.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16054 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/tests/test_impl_eni.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27368 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/tests/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2742 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/tests/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17842 2019-06-21 13:51:32.000000 os-net-config-9.4.0/os_net_config/tests/test_validator.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20415 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/tests/test_cli.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30618 2019-06-21 13:51:35.000000 os-net-config-9.4.0/os_net_config/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      564 2019-06-21 13:51:35.000000 os-net-config-9.4.0/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      497 2019-06-21 13:51:35.000000 os-net-config-9.4.0/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3135 2019-06-21 13:51:35.000000 os-net-config-9.4.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11314 2019-06-21 13:56:12.000000 os-net-config-9.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4714 2019-06-21 13:56:12.000000 os-net-config-9.4.0/PKG-INFO
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      902 2019-06-21 13:56:12.000000 os-net-config-9.4.0/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-09-12 09:39:08.000000 os-net-config-9.4.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2019-09-12 09:39:14.000000 os-net-config-9.4.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4714 2019-09-12 09:40:06.000000 os-net-config-9.4.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2019-09-12 09:39:14.000000 os-net-config-9.4.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2019-09-12 09:40:06.000000 os-net-config-9.4.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2019-09-12 09:39:14.000000 os-net-config-9.4.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2019-09-12 09:39:14.000000 os-net-config-9.4.1/zuul.d/layout.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11809 2019-09-12 09:40:06.000000 os-net-config-9.4.1/ChangeLog
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2437 2019-09-12 09:39:14.000000 os-net-config-9.4.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2019-09-12 09:39:08.000000 os-net-config-9.4.1/doc/source/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2019-09-12 09:39:08.000000 os-net-config-9.4.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2019-09-12 09:39:08.000000 os-net-config-9.4.1/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2019-09-12 09:39:08.000000 os-net-config-9.4.1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2019-09-12 09:39:08.000000 os-net-config-9.4.1/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2019-09-12 09:39:14.000000 os-net-config-9.4.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2019-09-12 09:39:14.000000 os-net-config-9.4.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-09-12 09:39:08.000000 os-net-config-9.4.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2019-09-12 09:40:06.000000 os-net-config-9.4.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2019-09-12 09:39:08.000000 os-net-config-9.4.1/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4575 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4714 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2019-09-12 09:39:08.000000 os-net-config-9.4.1/LICENSE
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77209 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/impl_ifcfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14477 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13522 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/os_net_config/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74305 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/tests/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/tests/test_os_net_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30161 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16054 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/tests/test_impl_eni.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17842 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/tests/test_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20415 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/tests/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    87422 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/tests/test_impl_ifcfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/impl_iproute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31634 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51119 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/schema.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7202 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18363 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/sriov_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9896 2019-09-12 09:39:08.000000 os-net-config-9.4.1/os_net_config/impl_eni.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    79361 2019-09-12 09:39:14.000000 os-net-config-9.4.1/os_net_config/objects.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/etc/os-net-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/etc/os-net-config/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/mapping.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_switchdev.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/mapping_report.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/nfvswitch.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2019-09-12 09:39:14.000000 os-net-config-9.4.1/etc/os-net-config/samples/interface.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_vlan.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter_dpdk.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ivs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bond_mapped.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2019-09-12 09:39:14.000000 os-net-config-9.4.1/etc/os-net-config/samples/interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/mapping_mnemonic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bond.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk_bond.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_dhcp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_ovs_extra.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/linux_bond_networkmanager.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_dhcp.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/nfvswitch.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/vpp_bond.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3435 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/vpp_bond.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ib_interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_fail_mode.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_vlan.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/linux_bridge.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter_dpdk_bond.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_ovs_dpdk.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter_dpdk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/routes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ovs_patch_port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_fail_mode.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/vpp_interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ivs.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ovs_patch_port.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bond.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_ovs_dpdk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/linux_bond.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2535 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_switchdev.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/bridge_ovs_extra.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk_bond.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/team.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/team.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ib_interface.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter_vlan.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/vpp_interface.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter_vlan.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2019-09-12 09:39:08.000000 os-net-config-9.4.1/etc/os-net-config/samples/contrail_vrouter_dpdk_bond.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2019-09-12 09:39:14.000000 os-net-config-9.4.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2019-09-12 09:39:08.000000 os-net-config-9.4.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2019-09-12 09:39:08.000000 os-net-config-9.4.1/.mailmap
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/source/queens.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6461 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2019-09-12 09:39:14.000000 os-net-config-9.4.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/source/unreleased.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-12 09:40:06.000000 os-net-config-9.4.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/add_contrail_vrouter_vlan_linux_bond_type-0a89f3499a7ab08b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/log-mapping-file-8b2a9d8f6a81ba99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/retry_ovs-appctl-6734b087ab6db80b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/add-neutron-route-schema-support-e8e20a8c3b79d14d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/check-ovs-ef665418762ca123.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/dpdk-on-mellanox-nics-1d8fdb843a4e2b60.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/sriov-vf-in-hosts-529c2bf0cb3294b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/enable-setting-domain-5557e2441c23a5a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/restart-ivs-nvfswitch-after-change-0825ea78aae8f138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/log-info-nic-discovery-f54ace7639890fdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/modify-interface-without-restart-d55949572017d52f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/policy-based-routing-3fa1200ae155bbee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-09-12 09:39:08.000000 os-net-config-9.4.1/releasenotes/notes/allow-list-of-routes-to-be-empty-323690796760630d.yaml
```

### Comparing `os-net-config-9.4.0/setup.py` & `os-net-config-9.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/releasenotes/notes/policy-based-routing-3fa1200ae155bbee.yaml` & `os-net-config-9.4.1/releasenotes/notes/policy-based-routing-3fa1200ae155bbee.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/releasenotes/notes/modify-interface-without-restart-d55949572017d52f.yaml` & `os-net-config-9.4.1/releasenotes/notes/modify-interface-without-restart-d55949572017d52f.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/releasenotes/source/conf.py` & `os-net-config-9.4.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/CONTRIBUTING.rst` & `os-net-config-9.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/AUTHORS` & `os-net-config-9.4.1/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -29,30 +29,34 @@
 James Polley <jp@jamezpolley.com>
 James Slagle <jslagle@redhat.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Ji-Wei <ji.wei3@zte.com.cn>
 John Trowbridge <trown@redhat.com>
 Juan Antonio Osorio Robles <jaosorior@redhat.com>
 Karthik S <ksundara@redhat.com>
+Keigo Noha <knoha@redhat.com>
 Matthew Flusche <mflusche@redhat.com>
 Michael Henkel <mhenkel@juniper.net>
 Monty Taylor <mordred@inaugust.com>
+Moshe Levi <moshele@mellanox.com>
+Noam Angel <noama@mellanox.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Pierre Blanc <pblanc@redhat.com>
 Sagi Shnaidman <sshnaidm@redhat.com>
 Sanjay Upadhyay <supadhya@redhat.com>
 Sarath Kumar <sarath.kutty@bigswitch.com>
 Saravanan KR <skramaja@redhat.com>
 Steven Hardy <shardy@redhat.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Tim Rozet <trozet@redhat.com>
 Tomoki Sekiyama <tomoki.sekiyama@hds.com>
 Tony Xu <hhktony@gmail.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 Zenghui Shi <zshi@redhat.com>
+alexey-mr <alexey.morlang@gmail.com>
 bdemers <bdemers@apache.org>
 huang.zhiping <huang.zhiping@99cloud.net>
 janonymous <janonymous.codevulture@gmail.com>
 karthik s <ksundara@redhat.com>
 marios <marios@redhat.com>
 melissaml <ma.lei@99cloud.net>
 qingszhao <zhao.daqing@99cloud.net>
```

### Comparing `os-net-config-9.4.0/LICENSE` & `os-net-config-9.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/tox.ini` & `os-net-config-9.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/routes.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/routes.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk.json` & `os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/bridge_vlan.json` & `os-net-config-9.4.1/etc/os-net-config/samples/bridge_vlan.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/interface.json` & `os-net-config-9.4.1/etc/os-net-config/samples/interface.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/bond.json` & `os-net-config-9.4.1/etc/os-net-config/samples/bond.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/bond_mapped.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/bond_mapped.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ivs.json` & `os-net-config-9.4.1/etc/os-net-config/samples/ivs.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk_bond.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk_bond.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ovs_patch_port.json` & `os-net-config-9.4.1/etc/os-net-config/samples/ovs_patch_port.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/team.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/team.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk_bond.json` & `os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk_bond.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/nfvswitch.json` & `os-net-config-9.4.1/etc/os-net-config/samples/nfvswitch.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf.json` & `os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/vpp_interface.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/vpp_interface.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_switchdev.json` & `os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_switchdev.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_ovs_dpdk.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_ovs_dpdk.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_ovs_dpdk.json` & `os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_ovs_dpdk.json`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ovs_patch_port.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/ovs_patch_port.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/ovs_dpdk.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/ovs_dpdk.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/interface.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/interface.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/etc/os-net-config/samples/sriov_pf_switchdev.yaml` & `os-net-config-9.4.1/etc/os-net-config/samples/sriov_pf_switchdev.yaml`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config.egg-info/PKG-INFO` & `os-net-config-9.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-net-config
-Version: 9.4.0
+Version: 9.4.1
 Summary: OpenStack network configuration
 Home-page: http://git.openstack.org/cgit/openstack/os-net-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: Apache License (2.0)
 Description: ========================
         Team and repository tags
```

### Comparing `os-net-config-9.4.0/os_net_config.egg-info/SOURCES.txt` & `os-net-config-9.4.1/os_net_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/doc/source/conf.py` & `os-net-config-9.4.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/impl_iproute.py` & `os-net-config-9.4.1/os_net_config/impl_iproute.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/__init__.py` & `os-net-config-9.4.1/os_net_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,18 @@
         logger.info('%s%s' % (self.log_prefix, msg))
         if not self.noop:
             os.remove(filename)
 
     def ifdown(self, interface, iftype='interface'):
         msg = 'running ifdown on %s: %s' % (iftype, interface)
         self.execute(msg, '/sbin/ifdown', interface, check_exit_code=False)
+        if utils.is_active_nic(interface):
+            msg = '%s %s is up, trying with ip command' % (iftype, interface)
+            self.execute(msg, '/sbin/ip',
+                         'link', 'set', 'dev', interface, 'down')
 
     def ifup(self, interface, iftype='interface'):
         """Run 'ifup' on the specified interface
 
         If a failure occurs when bringing up the interface it will be saved
         to self.errors for later handling.  This allows callers to continue
         trying to bring up interfaces even if one fails.
```

### Comparing `os-net-config-9.4.0/os_net_config/version.py` & `os-net-config-9.4.1/os_net_config/version.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/objects.py` & `os-net-config-9.4.1/os_net_config/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,27 +971,28 @@
     """Base class for Linux bonds."""
 
     def __init__(self, name, use_dhcp=False, use_dhcpv6=False, addresses=None,
                  routes=None, rules=None, mtu=None, primary=False,
                  members=None, bonding_options=None, nic_mapping=None,
                  persist_mapping=False, defroute=True, dhclient_args=None,
                  dns_servers=None, nm_controlled=False, onboot=True,
-                 domain=None):
+                 domain=None, ethtool_opts=None):
         addresses = addresses or []
         routes = routes or []
         rules = rules or []
         members = members or []
         dns_servers = dns_servers or []
         super(LinuxBond, self).__init__(name, use_dhcp, use_dhcpv6, addresses,
                                         routes, rules, mtu, primary,
                                         nic_mapping, persist_mapping, defroute,
                                         dhclient_args, dns_servers,
                                         nm_controlled, onboot, domain)
         self.members = members
         self.bonding_options = bonding_options
+        self.ethtool_opts = ethtool_opts
         for member in self.members:
             if isinstance(member, SriovVF):
                 LinuxBond.update_vf_config(member)
             member.linux_bond_name = name
             if member.primary:
                 if self.primary_interface_name:
                     msg = 'Only one primary interface allowed per bond.'
@@ -1025,26 +1026,27 @@
     def from_json(json):
         name = _get_required_field(json, 'name', 'LinuxBond')
         (use_dhcp, use_dhcpv6, addresses, routes, rules, mtu, nic_mapping,
          persist_mapping, defroute, dhclient_args, dns_servers, nm_controlled,
          onboot, domain) = _BaseOpts.base_opts_from_json(
              json, include_primary=False)
         bonding_options = json.get('bonding_options')
+        ethtool_opts = json.get('ethtool_opts', None)
 
         members = _update_members(json, nic_mapping, persist_mapping)
 
         return LinuxBond(name, use_dhcp=use_dhcp, use_dhcpv6=use_dhcpv6,
                          addresses=addresses, routes=routes, rules=rules,
                          mtu=mtu, members=members,
                          bonding_options=bonding_options,
                          nic_mapping=nic_mapping,
                          persist_mapping=persist_mapping, defroute=defroute,
                          dhclient_args=dhclient_args, dns_servers=dns_servers,
                          nm_controlled=nm_controlled, onboot=onboot,
-                         domain=domain)
+                         domain=domain, ethtool_opts=ethtool_opts)
 
 
 class OvsBond(_BaseOpts):
     """Base class for OVS bonds."""
 
     def __init__(self, name, use_dhcp=False, use_dhcpv6=False, addresses=None,
                  routes=None, rules=None, mtu=None, primary=False,
```

### Comparing `os-net-config-9.4.0/os_net_config/validator.py` & `os-net-config-9.4.1/os_net_config/validator.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/impl_eni.py` & `os-net-config-9.4.1/os_net_config/impl_eni.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/sriov_config.py` & `os-net-config-9.4.1/os_net_config/sriov_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,44 +24,34 @@
 import argparse
 import logging
 import os
 import pyudev
 import re
 from six.moves import queue as Queue
 import sys
+import time
 import yaml
 
 from oslo_concurrency import processutils
 
 logger = logging.getLogger(__name__)
 _SYS_CLASS_NET = '/sys/class/net'
-_UDEV_RULE_FILE = '/etc/udev/rules.d/70-persistent-net.rules'
-
+_UDEV_RULE_FILE = '/etc/udev/rules.d/80-persistent-os-net-config.rules'
+MAX_RETRIES = 10
+PF_FUNC_RE = re.compile(r"\.(\d+)$", 0)
 # In order to keep VF representor name consistent specially after the upgrade
 # proccess, we should have a udev rule to handle that.
 # The udev rule will rename the VF representor as "<sriov_pf_name>_<vf_num>"
 _REP_LINK_NAME_FILE = "/etc/udev/rep-link-name.sh"
 _REP_LINK_NAME_DATA = '''#!/bin/bash
-SWID="$1"
-PORT="$2"
-parent_phys_port_name=${PORT%vf*}
-parent_phys_port_name=${parent_phys_port_name//f}
-for i in `ls -1 /sys/class/net/*/phys_port_name`
-do
-    nic=`echo $i | cut -d/ -f 5`
-    sw_id=`cat /sys/class/net/$nic/phys_switch_id 2>/dev/null`
-    phys_port_name=`cat /sys/class/net/$nic/phys_port_name 2>/dev/null`
-    if [ "$parent_phys_port_name" = "$phys_port_name" ] &&
-       [ "$sw_id" = "$SWID" ]
-    then
-        echo "NAME=${nic}_${PORT##pf*vf}"
-        break
-        exit
-    fi
-done'''
+# This file is autogenerated by os-net-config
+set -x
+PORT="$1"
+echo "NUMBER=${PORT##pf*vf}"
+'''
 
 # Create a queue for passing the udev network events
 vf_queue = Queue.Queue()
 
 
 # File to contain the list of SR-IOV PF, VF and their configurations
 # Format of the file shall be
@@ -108,31 +98,57 @@
 
 def _get_sriov_map():
     contents = get_file_data(_SRIOV_CONFIG_FILE)
     sriov_map = yaml.safe_load(contents) if contents else []
     return sriov_map
 
 
-def configure_sriov_pf():
+def get_numvfs(ifname):
+    try:
+        sriov_numvfs_path = os.path.join(_SYS_CLASS_NET, ifname,
+                                         "device/sriov_numvfs")
+        with open(sriov_numvfs_path, 'r') as f:
+            return int(f.read())
+    except IOError:
+        msg = ("Unable to read numvfs for %s" % ifname)
+        raise SRIOVNumvfsException(msg)
+
+
+def restart_ovs_and_pfs_netdevs():
+    sriov_map = _get_sriov_map()
+    processutils.execute('/usr/bin/systemctl', 'restart', 'openvswitch')
+    for item in sriov_map:
+        if item['device_type'] == 'pf':
+            if_down_interface(item['name'])
+            if_up_interface(item['name'])
+
+
+def configure_sriov_pf(execution_from_cli=False, restart_openvswitch=False):
     # Create a context for pyudev and observe udev events for network
     context = pyudev.Context()
     monitor = pyudev.Monitor.from_netlink(context)
     monitor.filter_by('net')
     observer = pyudev.MonitorObserver(monitor, udev_event_handler)
     observer.start()
 
     sriov_map = _get_sriov_map()
     MLNX_UNBIND_FILE_PATH = "/sys/bus/pci/drivers/mlx5_core/unbind"
     MLNX_VENDOR_ID = "0x15b3"
+    trigger_udev_rule = False
     for item in sriov_map:
         if item['device_type'] == 'pf':
             _pf_interface_up(item)
             try:
-                sriov_numvfs_path = ("/sys/class/net/%s/device/sriov_numvfs"
-                                     % item['name'])
+                sriov_numvfs_path = os.path.join(_SYS_CLASS_NET, item['name'],
+                                                 "device/sriov_numvfs")
+                curr_numvfs = get_numvfs(item['name'])
+                if curr_numvfs == item['numvfs']:
+                    logger.info("Numvfs already configured for %s"
+                                % item['name'])
+                    continue
                 with open(sriov_numvfs_path, 'w') as f:
                     f.write("%d" % item['numvfs'])
             except IOError as exc:
                 msg = ("Unable to configure pf: %s with numvfs: %d\n%s"
                        % (item['name'], item['numvfs'], exc))
                 raise SRIOVNumvfsException(msg)
             # Wait for the creation of VFs for each PF
@@ -143,21 +159,46 @@
                     vendor_id == MLNX_VENDOR_ID):
                 vf_pcis_list = get_vf_pcis_list(item['name'])
                 for vf_pci in vf_pcis_list:
                     vf_pci_path = "/sys/bus/pci/devices/%s/driver" % vf_pci
                     if os.path.exists(vf_pci_path):
                         with open(MLNX_UNBIND_FILE_PATH, 'w') as f:
                             f.write("%s" % vf_pci)
+
+                # Adding a udev rule to make vf-representors unmanaged by
+                # NetworkManager
+                add_udev_rule_to_unmanage_vf_representors_by_nm()
+
                 # Adding a udev rule to save the sriov_pf name
-                add_udev_rule_for_sriov_pf(item['name'])
-                add_udev_rule_for_vf_representors()
+                trigger_udev_rule = add_udev_rule_for_sriov_pf(item['name'])\
+                    or trigger_udev_rule
+
                 configure_switchdev(item['name'])
-                if_up_interface(item['name'])
+
+                # Adding a udev rule to rename vf-representors
+                trigger_udev_rule = add_udev_rule_for_vf_representors(
+                    item['name']) or trigger_udev_rule
+
+                # Moving the sriov-PFs to switchdev mode will put the netdev
+                # interfaces in down state.
+                # In case we are running during initial deployment,
+                # bring the interfaces up.
+                # In case we are running as part of the sriov_config service
+                # after reboot, net config scripts, which run after
+                # sriov_config service will bring the interfaces up.
+                if execution_from_cli:
+                    if_up_interface(item['name'])
+
+    # Trigger udev rules if there is new rules written
+    if trigger_udev_rule:
+        trigger_udev_rules()
 
     observer.stop()
+    if restart_openvswitch:
+        restart_ovs_and_pfs_netdevs()
 
 
 def _wait_for_vf_creation(pf_name, numvfs):
     vf_count = 0
     vf_list = []
     while vf_count < numvfs:
         try:
@@ -171,70 +212,124 @@
                 if len(pf_nic) == 1 and pf_name == pf_nic[0]:
                     if vf_name not in vf_list:
                         vf_list.append(vf_name)
                         logger.info("VF: %s created for PF: %s"
                                     % (vf_name, pf_name))
                         vf_count = vf_count + 1
                 else:
-                    logger.error("Unable to parse event %s" % event["device"])
+                    logger.warning("Unable to parse event %s"
+                                   % event["device"])
             else:
-                logger.error("%s is not a directory" % pf_path)
+                logger.warning("%s is not a directory" % pf_path)
         except Queue.Empty:
             logger.info("Timeout in the creation of VFs for PF %s" % pf_name)
             return
     logger.info("Required VFs are created for PF %s" % pf_name)
 
 
+def _wait_for_uplink_rep_creation(pf_name):
+    uplink_rep_phys_switch_id_path = "/sys/class/net/%s/phys_switch_id" \
+                                     % pf_name
+
+    for i in range(MAX_RETRIES):
+        if get_file_data(uplink_rep_phys_switch_id_path):
+            logger.info("Uplink representor %s ready", pf_name)
+            break
+        time.sleep(1)
+    else:
+        raise RuntimeError("Timeout while waiting for uplink representor %s.",
+                           pf_name)
+
+
 def create_rep_link_name_script():
     with open(_REP_LINK_NAME_FILE, "w") as f:
         f.write(_REP_LINK_NAME_DATA)
     # Make the _REP_LINK_NAME_FILE executable
     os.chmod(_REP_LINK_NAME_FILE, 0o755)
 
 
 def add_udev_rule_for_sriov_pf(pf_name):
     pf_pci = get_pf_pci(pf_name)
     udev_data_line = 'SUBSYSTEM=="net", ACTION=="add", DRIVERS=="?*", '\
                      'KERNELS=="%s", NAME="%s"' % (pf_pci, pf_name)
-    add_udev_rule(udev_data_line, _UDEV_RULE_FILE)
+    return add_udev_rule(udev_data_line, _UDEV_RULE_FILE)
+
+
+def add_udev_rule_for_vf_representors(pf_name):
+    phys_switch_id_path = os.path.join(_SYS_CLASS_NET, pf_name,
+                                       "phys_switch_id")
+    phys_switch_id = get_file_data(phys_switch_id_path).strip()
+    pf_pci = get_pf_pci(pf_name)
+    pf_fun_num_match = PF_FUNC_RE.search(pf_pci)
+    if pf_fun_num_match:
+        pf_fun_num = pf_fun_num_match.group(1)
+    else:
+        logger.error("Failed to get function number for %s \n"
+                     "and so failed to create a udev rule for renaming "
+                     "its' vf-represent" % pf_name)
+        return
+
+    udev_data_line = 'SUBSYSTEM=="net", ACTION=="add", ATTR{phys_switch_id}'\
+                     '=="%s", ATTR{phys_port_name}=="pf%svf*", '\
+                     'IMPORT{program}="%s $attr{phys_port_name}", '\
+                     'NAME="%s_$env{NUMBER}"' % (phys_switch_id,
+                                                 pf_fun_num,
+                                                 _REP_LINK_NAME_FILE,
+                                                 pf_name)
+    create_rep_link_name_script()
+    return add_udev_rule(udev_data_line, _UDEV_RULE_FILE)
 
 
-def add_udev_rule_for_vf_representors():
+def add_udev_rule_to_unmanage_vf_representors_by_nm():
     udev_data_line = 'SUBSYSTEM=="net", ACTION=="add", ATTR{phys_switch_id}'\
                      '!="", ATTR{phys_port_name}=="pf*vf*", '\
-                     'IMPORT{program}="%s '\
-                     '$attr{phys_switch_id} $attr{phys_port_name}" '\
-                     'NAME="$env{NAME}"' % _REP_LINK_NAME_FILE
-    create_rep_link_name_script()
-    add_udev_rule(udev_data_line, _UDEV_RULE_FILE)
+                     'ENV{NM_UNMANAGED}="1"'
+    return add_udev_rule(udev_data_line, _UDEV_RULE_FILE)
 
 
 def add_udev_rule(udev_data, udev_file):
+    trigger_udev_rule = False
     udev_data = udev_data.strip()
     if not os.path.exists(udev_file):
         with open(udev_file, "w") as f:
-            f.write(udev_data + "\n")
+            data = "# This file is autogenerated by os-net-config\n%s\n"\
+                   % udev_data
+            f.write(data)
         reload_udev_rules()
+        trigger_udev_rule = True
     else:
         file_data = get_file_data(udev_file)
         udev_lines = file_data.split("\n")
         if udev_data not in udev_lines:
             with open(udev_file, "a") as f:
                 f.write(udev_data + "\n")
             reload_udev_rules()
+            trigger_udev_rule = True
+    return trigger_udev_rule
 
 
 def reload_udev_rules():
     try:
         processutils.execute('/usr/sbin/udevadm', 'control', '--reload-rules')
+        logger.info("udev rules reloaded successfully")
     except processutils.ProcessExecutionError:
         logger.error("Failed to reload udev rules")
         raise
 
 
+def trigger_udev_rules():
+    try:
+        processutils.execute('/usr/sbin/udevadm', 'trigger', '--action=add',
+                             '--attr-match=subsystem=net')
+        logger.info("udev rules triggered successfully")
+    except processutils.ProcessExecutionError:
+        logger.error("Failed to trigger udev rules")
+        raise
+
+
 def configure_switchdev(pf_name):
     pf_pci = get_pf_pci(pf_name)
     pf_device_id = get_pf_device_id(pf_name)
     if pf_device_id == "0x1013" or pf_device_id == "0x1015":
         try:
             processutils.execute('/usr/sbin/devlink', 'dev', 'eswitch', 'set',
                                  'pci/%s' % pf_pci, 'inline-mode', 'transport')
@@ -243,17 +338,26 @@
             raise
     try:
         processutils.execute('/usr/sbin/devlink', 'dev', 'eswitch', 'set',
                              'pci/%s' % pf_pci, 'mode', 'switchdev')
     except processutils.ProcessExecutionError:
         logger.error("Failed to set mode to switchdev")
         raise
+    logger.info("Device pci/%s set to switchdev mode." % pf_pci)
+
+    # WA to make sure that the uplink_rep is ready after moving to switchdev,
+    # as moving to switchdev will remove the sriov_pf and create uplink
+    # representor, so we need to make sure that uplink representor is ready
+    # before proceed
+    _wait_for_uplink_rep_creation(pf_name)
+
     try:
         processutils.execute('/usr/sbin/ethtool', '-K', pf_name,
                              'hw-tc-offload', 'on')
+        logger.info("Enabled \"hw-tc-offload\" for PF %s." % pf_name)
     except processutils.ProcessExecutionError:
         logger.error("Failed to enable hw-tc-offload")
         raise
 
 
 def run_ip_config_cmd(*cmd, **kwargs):
     logger.info("Running %s" % ' '.join(cmd))
@@ -304,14 +408,23 @@
             vf_info = get_file_data(os.path.join(_SYS_CLASS_NET, pf_name,
                                     "device", pf_file, "uevent"))
             vf_pcis_list.append(re.search(r'PCI_SLOT_NAME=(.*)',
                                           vf_info, re.MULTILINE).group(1))
     return vf_pcis_list
 
 
+def if_down_interface(device):
+    logger.info("Running /sbin/ifdown %s" % device)
+    try:
+        processutils.execute('/sbin/ifdown', device)
+    except processutils.ProcessExecutionError:
+        logger.error("Failed to ifdown  %s" % device)
+        raise
+
+
 def if_up_interface(device):
     logger.info("Running /sbin/ifup %s" % device)
     try:
         processutils.execute('/sbin/ifup', device)
     except processutils.ProcessExecutionError:
         logger.error("Failed to ifup  %s" % device)
         raise
```

### Comparing `os-net-config-9.4.0/os_net_config/cli.py` & `os-net-config-9.4.1/os_net_config/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from os_net_config import impl_iproute
 from os_net_config import objects
 from os_net_config import utils
 from os_net_config import validator
 from os_net_config import version
 
 logger = logging.getLogger(__name__)
+_SYSTEM_CTL_CONFIG_FILE = '/etc/sysctl.d/os-net-sysctl.conf'
 
 
 def parse_opts(argv):
     parser = argparse.ArgumentParser(
         description='Configure host network interfaces using a JSON'
         ' config file format.')
     parser.add_argument('-c', '--config-file', metavar='CONFIG_FILE',
@@ -139,21 +140,40 @@
         if isinstance(member, objects.SriovPF):
             configure_sriov = True
         elif hasattr(member, "members") and member.members is not None:
             configure_sriov = check_configure_sriov(member)
     return configure_sriov
 
 
+def disable_ipv6_for_netdevs(net_devices):
+    sysctl_conf = ""
+    for net_device in net_devices:
+        sysctl_conf += "net.ipv6.conf.%s.disable_ipv6 = 1\n" % net_device
+    utils.write_config(_SYSTEM_CTL_CONFIG_FILE, sysctl_conf)
+
+
+def get_sriovpf_member_of_bond_ovs_port(obj):
+    net_devs_list = []
+    if isinstance(obj, objects.OvsBridge):
+        for member in obj.members:
+            if isinstance(member, objects.LinuxBond):
+                for child_member in member.members:
+                    if isinstance(child_member, objects.SriovPF):
+                        if child_member.link_mode == 'switchdev':
+                            net_devs_list.append(child_member.name)
+    return net_devs_list
+
+
 def main(argv=sys.argv):
     opts = parse_opts(argv)
     configure_logger(opts.verbose, opts.debug)
     logger.info('Using config file at: %s' % opts.config_file)
     iface_array = []
     configure_sriov = False
-
+    sriovpf_member_of_bond_ovs_port_list = []
     provider = None
     if opts.provider:
         if opts.provider == 'ifcfg':
             provider = impl_ifcfg.IfcfgNetConfig(noop=opts.noop,
                                                  root_dir=opts.root_dir)
         elif opts.provider == 'eni':
             provider = impl_eni.ENINetConfig(noop=opts.noop,
@@ -274,25 +294,39 @@
             configure_sriov = True
             provider.add_object(obj)
         elif hasattr(obj, 'members') and obj.members is not None:
             if check_configure_sriov(obj):
                 configure_sriov = True
                 provider.add_object(obj)
 
+                sriovpf_member_of_bond_ovs_port_list.extend(
+                    get_sriovpf_member_of_bond_ovs_port(obj))
+
+    # After reboot, shared_block for pf interface in switchdev mode will be
+    # missing in case IPv6 is enabled on the slaves of the bond and that bond
+    # is an ovs port. This is due to the fact that OVS assumes another entity
+    # manages the slaves.
+    # So as a workaround for that case we are disabling IPv6 over pfs so that
+    # OVS creates the shared_blocks ingress
+    if sriovpf_member_of_bond_ovs_port_list:
+        disable_ipv6_for_netdevs(sriovpf_member_of_bond_ovs_port_list)
+
     if configure_sriov:
         # Apply the ifcfgs for PFs now, so that NM_CONTROLLED=no is applied
         # for each of the PFs before configuring the numvfs for the PF device.
         # This step allows the network manager to unmanage the created VFs.
         # In the second parse, when these ifcfgs for PFs are encountered,
         # os-net-config skips the ifup <ifcfg-pfs>, since the ifcfgs for PFs
         # wouldn't have changed.
         pf_files_changed = provider.apply(cleanup=opts.cleanup,
                                           activate=not opts.no_activate)
         if not opts.noop:
-            utils.configure_sriov_pfs()
+            utils.configure_sriov_pfs(
+                execution_from_cli=True,
+                restart_openvswitch=bool(sriovpf_member_of_bond_ovs_port_list))
 
     for iface_json in iface_array:
         # All objects other than the sriov_pf will be added here.
         # The VFs are expected to be available now and an exception
         # SriovVfNotFoundException shall be raised if not available.
         try:
             obj = objects.object_from_json(iface_json)
```

### Comparing `os-net-config-9.4.0/os_net_config/schema.yaml` & `os-net-config-9.4.1/os_net_config/schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1029,15 +1029,15 @@
                   - $ref: "#/definitions/int_or_param"
             bond_policy:
                 oneOf:
                   - $ref: "#/definitions/string_or_param"
                   - $ref: "#/definitions/int_or_param"
             driver:
                 $ref: "#/definitions/string_or_param"
-            coremask:
+            cpu_list:
                 $ref: "#/definitions/string_or_param"
             vlan_id:
                 oneOf:
                   - $ref: "#/definitions/string_or_param"
                   - $ref: "#/definitions/int_or_param"
             # common options:
             use_dhcp:
@@ -1161,14 +1161,16 @@
                 $ref: "#/definitions/list_of_ip_address_string_or_param"
             nm_controlled:
                 $ref: "#/definitions/bool_or_param"
             onboot:
                 $ref: "#/definitions/bool_or_param"
             domain:
                 $ref: "#/definitions/list_of_domain_name_string_or_domain_name_string"
+            ethtool_opts:
+                $ref: "#/definitions/string_or_param"
         required:
           - type
           - name
           - members
         additionalProperties: False
 
     linux_team:
```

### Comparing `os-net-config-9.4.0/os_net_config/impl_ifcfg.py` & `os-net-config-9.4.1/os_net_config/impl_ifcfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,14 +936,18 @@
         logger.info('adding sriov pf: %s' % sriov_pf.name)
         data = self._add_common(sriov_pf)
         logger.debug('sriov pf data: %s' % data)
         utils.update_sriov_pf_map(sriov_pf.name, sriov_pf.numvfs,
                                   self.noop, promisc=sriov_pf.promisc,
                                   link_mode=sriov_pf.link_mode)
         self.interface_data[sriov_pf.name] = data
+        if sriov_pf.routes:
+            self._add_routes(sriov_pf.name, sriov_pf.routes)
+        if sriov_pf.rules:
+            self._add_rules(sriov_pf.name, sriov_pf.rules)
 
     def add_sriov_vf(self, sriov_vf):
         """Add a SriovVF object to the net config object
 
         :param sriov_vf: The SriovVF object to add
         """
         logger.info('adding sriov vf: %s for pf: %s, vfid: %d'
```

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_os_net_config.py` & `os-net-config-9.4.1/os_net_config/tests/test_os_net_config.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_objects.py` & `os-net-config-9.4.1/os_net_config/tests/test_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1131,20 +1131,21 @@
     {
     "type": "interface",
     "name": "em2"
     }
 ]
 }
 """
-        bridge = objects.object_from_json(json.loads(data))
-        self.assertEqual("bond1", bridge.name)
-        self.assertTrue(bridge.use_dhcp)
-        interface1 = bridge.members[0]
+        bond = objects.object_from_json(json.loads(data))
+        self.assertEqual("bond1", bond.name)
+        self.assertTrue(bond.use_dhcp)
+        self.assertIsNone(bond.ethtool_opts)
+        interface1 = bond.members[0]
         self.assertEqual("em1", interface1.name)
-        interface2 = bridge.members[1]
+        interface2 = bond.members[1]
         self.assertEqual("em2", interface2.name)
 
     def test_from_json_dhcp_with_nic1_nic2(self):
 
         def dummy_mapped_nics(nic_mapping=None):
             return {"nic1": "em1", "nic2": "em2"}
         self.stub_out('os_net_config.objects.mapped_nics', dummy_mapped_nics)
@@ -1161,20 +1162,20 @@
     {
     "type": "interface",
     "name": "nic2"
     }
 ]
 }
 """
-        bridge = objects.object_from_json(json.loads(data))
-        self.assertEqual("bond1", bridge.name)
-        self.assertTrue(bridge.use_dhcp)
-        interface1 = bridge.members[0]
+        bond = objects.object_from_json(json.loads(data))
+        self.assertEqual("bond1", bond.name)
+        self.assertTrue(bond.use_dhcp)
+        interface1 = bond.members[0]
         self.assertEqual("em1", interface1.name)
-        interface2 = bridge.members[1]
+        interface2 = bond.members[1]
         self.assertEqual("em2", interface2.name)
 
     def test_linux_bond_with_vf_default(self):
         data = """{
 "type": "linux_bond",
 "name": "bond1",
 "use_dhcp": true,
@@ -1268,14 +1269,47 @@
                       test_get_vf_devname)
 
         objects.object_from_json(json.loads(data))
         contents = utils.get_file_data(sriov_config._SRIOV_CONFIG_FILE)
         vf_map = yaml.safe_load(contents) if contents else []
         self.assertListEqual(vf_final, vf_map)
 
+    def test_linux_bond_with_ethtool_opts(self):
+        data = """{
+"type": "linux_bond",
+"name": "bond1",
+"use_dhcp": true,
+"ethtool_opts": "-K ${DEVICE} tx-gre-csum-segmentation off",
+"members": [
+    {
+    "type": "interface",
+    "name": "em1",
+    "ethtool_opts": "-K ${DEVICE} tx-gre-csum-segmentation off"
+    },
+    {
+    "type": "interface",
+    "name": "em2",
+    "ethtool_opts": "-K ${DEVICE} tx-gre-csum-segmentation off"
+    }
+]
+}
+"""
+        bond = objects.object_from_json(json.loads(data))
+        self.assertEqual("bond1", bond.name)
+        self.assertEqual("-K ${DEVICE} tx-gre-csum-segmentation off",
+                         bond.ethtool_opts)
+        interface1 = bond.members[0]
+        interface2 = bond.members[1]
+        self.assertEqual("em1", interface1.name)
+        self.assertEqual("em2", interface2.name)
+        self.assertEqual("-K ${DEVICE} tx-gre-csum-segmentation off",
+                         interface1.ethtool_opts)
+        self.assertEqual("-K ${DEVICE} tx-gre-csum-segmentation off",
+                         interface2.ethtool_opts)
+
 
 class TestOvsTunnel(base.TestCase):
 
     def setUp(self):
         super(TestOvsTunnel, self).setUp()
 
         def stub_is_ovs_installed():
```

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_impl_ifcfg.py` & `os-net-config-9.4.1/os_net_config/tests/test_impl_ifcfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,19 @@
 _LINUX_BRIDGE_IFCFG = _BASE_IFCFG + "BRIDGE=br-ctlplane\nBOOTPROTO=none\n"
 
 _ROUTES = """default via 192.168.1.1 dev em1 metric 10
 172.19.0.0/24 via 192.168.1.1 dev em1
 172.20.0.0/24 via 192.168.1.5 dev em1 metric 100
 """
 
+_ROUTES_PF = """default via 192.168.1.1 dev enp3s0f0 metric 10
+172.19.0.0/24 via 192.168.1.1 dev enp3s0f0
+172.20.0.0/24 via 192.168.1.5 dev enp3s0f0 metric 100
+"""
+
 _ROUTES_WITH_TABLES = """172.19.0.0/24 via 192.168.1.1 dev em1 table table1
 172.20.0.0/24 via 192.168.1.1 dev em1 table 201
 172.21.0.0/24 via 192.168.1.1 dev em1 table 200
 """
 
 _ROUTE_RULES = """# This file is autogenerated by os-net-config
 # test comment
@@ -559,14 +564,25 @@
 ONBOOT=yes
 HOTPLUG=no
 NM_CONTROLLED=no
 PEERDNS=no
 BOOTPROTO=none
 """
 
+_V4_SRIOV_PF_IFCFG = """# This file is autogenerated by os-net-config
+DEVICE=enp3s0f0
+ONBOOT=yes
+HOTPLUG=no
+NM_CONTROLLED=no
+PEERDNS=no
+BOOTPROTO=static
+IPADDR=192.168.1.2
+NETMASK=255.255.255.0
+"""
+
 
 class TestIfcfgNetConfig(base.TestCase):
     def setUp(self):
         super(TestIfcfgNetConfig, self).setUp()
         rand = str(int(random.random() * 100000))
         sriov_config._SRIOV_CONFIG_FILE = '/tmp/sriov_config_' + rand + '.yaml'
 
@@ -1214,14 +1230,39 @@
     def test_ib_interface_ethtool_opts(self):
         ifc = objects.IbInterface('ib0', ethtool_opts='speed 1000 duplex full')
         self.provider.add_interface(ifc)
         ib_config = "".join((_IB_IFCFG,
                              "ETHTOOL_OPTS=\"speed 1000 duplex full\"\n"))
         self.assertEqual(ib_config, self.get_interface_config('ib0'))
 
+    def test_linux_bond_with_ethtool_opts(self):
+        interface1 = objects.Interface(
+            'em1',
+            ethtool_opts='-K ${DEVICE} tx-gre-csum-segmentation off')
+        interface2 = objects.Interface(
+            'em2',
+            ethtool_opts='-K ${DEVICE} tx-gre-csum-segmentation off')
+        bond = objects.LinuxBond(
+            'bond0', use_dhcp=True,
+            members=[interface1, interface2],
+            ethtool_opts='-K ${DEVICE} tx-gre-csum-segmentation off')
+        self.provider.add_linux_bond(bond)
+        self.provider.add_interface(interface1)
+        self.provider.add_interface(interface2)
+        bond_config = "".join(
+            (_LINUX_BOND_DHCP,
+             "ETHTOOL_OPTS=\"-K ${DEVICE} tx-gre-csum-segmentation off\"\n"))
+        interface_config = "".join(
+            (_LINUX_BOND_INTERFACE,
+             "ETHTOOL_OPTS=\"-K ${DEVICE} tx-gre-csum-segmentation off\"\n"))
+        self.assertEqual(bond_config,
+                         self.get_linux_bond_config('bond0'))
+        self.assertEqual(interface_config,
+                         self.get_interface_config('em1'))
+
     def test_interface_single_dns_server(self):
         interface1 = objects.Interface('em1', dns_servers=['1.2.3.4'])
         self.provider.add_interface(interface1)
         em1_config = """# This file is autogenerated by os-net-config
 DEVICE=em1
 ONBOOT=yes
 HOTPLUG=no
@@ -1923,14 +1964,36 @@
         self.provider.apply()
 
         ifcfg_data = utils.get_file_data(self.temp_ifcfg_file.name)
         self.assertEqual(_V4_IFCFG, ifcfg_data)
         route_data = utils.get_file_data(self.temp_route_file.name)
         self.assertEqual(_ROUTES, route_data)
 
+    def test_sriov_pf_network_apply(self):
+        def get_numvfs_stub(pf_name):
+            return 0
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
+        route1 = objects.Route('192.168.1.1', default=True,
+                               route_options="metric 10")
+        route2 = objects.Route('192.168.1.1', '172.19.0.0/24')
+        route3 = objects.Route('192.168.1.5', '172.20.0.0/24',
+                               route_options="metric 100")
+        v4_addr = objects.Address('192.168.1.2/24')
+        pf = objects.SriovPF('enp3s0f0', numvfs=10, addresses=[v4_addr],
+                             promisc=False, routes=[route1, route2, route3])
+        self.provider.add_sriov_pf(pf)
+
+        self.provider.apply()
+
+        ifcfg_data = utils.get_file_data(self.temp_ifcfg_file.name)
+        self.assertEqual(_V4_SRIOV_PF_IFCFG, ifcfg_data)
+        route_data = utils.get_file_data(self.temp_route_file.name)
+        self.assertEqual(_ROUTES_PF, route_data)
+
     def test_dhcp_ovs_bridge_network_apply(self):
         interface = objects.Interface('em1')
         bridge = objects.OvsBridge('br-ctlplane', use_dhcp=True,
                                    members=[interface])
         self.provider.add_interface(interface)
         self.provider.add_bridge(bridge)
         self.provider.apply()
```

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_impl_eni.py` & `os-net-config-9.4.1/os_net_config/tests/test_impl_eni.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_utils.py` & `os-net-config-9.4.1/os_net_config/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,53 +115,83 @@
         self.assertEqual('enp8s0', nics[5])
         self.assertEqual('enp10s0', nics[6])
         self.assertEqual('z1', nics[7])
 
         shutil.rmtree(tmpdir)
 
     def test_update_sriov_pf_map_new(self):
+        def get_numvfs_stub(pf_name):
+            return 0
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
         utils.update_sriov_pf_map('eth1', 10, False)
         contents = utils.get_file_data(sriov_config._SRIOV_CONFIG_FILE)
         sriov_pf_map = yaml.safe_load(contents) if contents else []
         self.assertEqual(1, len(sriov_pf_map))
         test_sriov_pf_map = [{'device_type': 'pf', 'link_mode': 'legacy',
                               'name': 'eth1', 'numvfs': 10}]
         self.assertListEqual(test_sriov_pf_map, sriov_pf_map)
 
+    def test_update_sriov_pf_map_with_same_numvfs(self):
+        def get_numvfs_stub(pf_name):
+            return 10
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
+        utils.update_sriov_pf_map('eth1', 10, False)
+        contents = utils.get_file_data(sriov_config._SRIOV_CONFIG_FILE)
+        sriov_pf_map = yaml.safe_load(contents) if contents else []
+        self.assertEqual(1, len(sriov_pf_map))
+        test_sriov_pf_map = [{'device_type': 'pf', 'link_mode': 'legacy',
+                              'name': 'eth1', 'numvfs': 10}]
+        self.assertListEqual(test_sriov_pf_map, sriov_pf_map)
+
+    def test_update_sriov_pf_map_with_diff_numvfs(self):
+        def get_numvfs_stub(pf_name):
+            return 12
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
+        self.assertRaises(sriov_config.SRIOVNumvfsException,
+                          utils.update_sriov_pf_map, 'eth1', 10, False)
+
     def test_update_sriov_pf_map_new_with_promisc(self):
+        def get_numvfs_stub(pf_name):
+            return 0
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
         utils.update_sriov_pf_map('eth1', 10, False, promisc='off')
         contents = utils.get_file_data(sriov_config._SRIOV_CONFIG_FILE)
         sriov_pf_map = yaml.safe_load(contents) if contents else []
         self.assertEqual(1, len(sriov_pf_map))
         test_sriov_pf_map = [{'device_type': 'pf', 'link_mode': 'legacy',
                               'name': 'eth1', 'numvfs': 10, 'promisc': 'off'}]
         self.assertListEqual(test_sriov_pf_map, sriov_pf_map)
 
     def test_update_sriov_pf_map_exist(self):
+        def get_numvfs_stub(pf_name):
+            return 10
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
         pf_initial = [{'device_type': 'pf', 'link_mode': 'legacy',
                        'name': 'eth1', 'numvfs': 10}]
         utils.write_yaml_config(sriov_config._SRIOV_CONFIG_FILE, pf_initial)
-
-        utils.update_sriov_pf_map('eth1', 20, False)
-        pf_final = [{'device_type': 'pf', 'link_mode': 'legacy',
-                     'name': 'eth1', 'numvfs': 20}]
-        contents = utils.get_file_data(sriov_config._SRIOV_CONFIG_FILE)
-
-        pf_map = yaml.safe_load(contents) if contents else []
-        self.assertEqual(1, len(pf_map))
-        self.assertListEqual(pf_final, pf_map)
+        self.assertRaises(sriov_config.SRIOVNumvfsException,
+                          utils.update_sriov_pf_map, 'eth1', 20, False)
 
     def test_update_sriov_pf_map_exist_with_promisc(self):
+        def get_numvfs_stub(pf_name):
+            return 10
+        self.stub_out('os_net_config.sriov_config.get_numvfs',
+                      get_numvfs_stub)
         pf_initial = [{'device_type': 'pf', 'link_mode': 'legacy',
                        'name': 'eth1', 'numvfs': 10, 'promisc': 'on'}]
         utils.write_yaml_config(sriov_config._SRIOV_CONFIG_FILE, pf_initial)
 
-        utils.update_sriov_pf_map('eth1', 20, False)
+        utils.update_sriov_pf_map('eth1', 10, False, promisc='off')
         pf_final = [{'device_type': 'pf', 'link_mode': 'legacy',
-                     'name': 'eth1', 'numvfs': 20, 'promisc': 'on'}]
+                     'name': 'eth1', 'numvfs': 10, 'promisc': 'off'}]
         contents = utils.get_file_data(sriov_config._SRIOV_CONFIG_FILE)
 
         pf_map = yaml.safe_load(contents) if contents else []
         self.assertEqual(1, len(pf_map))
         self.assertListEqual(pf_final, pf_map)
 
     def test_update_sriov_vf_map_minimal_new(self):
@@ -437,14 +467,44 @@
         self.stub_out('os_net_config.utils._get_dpdk_mac_address',
                       test_get_dpdk_mac_address)
 
         self.assertRaises(utils.OvsDpdkBindException,
                           utils.bind_dpdk_interfaces, 'eth2', 'vfio-pci',
                           False)
 
+    def test_bind_dpdk_interfaces_same_driver(self):
+        mocked_open = mock.mock_open(read_data='DRIVER=vfio-pci\n')
+        self.stub_out('os_net_config.utils.open', mocked_open)
+        mocked_logger = mock.Mock()
+        self.stub_out('os_net_config.utils.logger.info', mocked_logger)
+        try:
+            utils.bind_dpdk_interfaces('eth1', 'vfio-pci', False)
+        except utils.OvsDpdkBindException:
+            self.fail("Received OvsDpdkBindException unexpectedly")
+        msg = "Driver (vfio-pci) is already bound to the device (eth1)"
+        mocked_logger.assert_called_with(msg)
+
+    def test_get_interface_driver(self):
+        mocked_open = mock.mock_open(read_data='DRIVER=vfio-pci\n')
+        self.stub_out('os_net_config.utils.open', mocked_open)
+        driver = utils.get_interface_driver('eth1')
+        self.assertEqual(driver, 'vfio-pci')
+
+    def test_get_interface_driver_fail_none(self):
+        mocked_open = mock.mock_open(read_data='')
+        self.stub_out('os_net_config.utils.open', mocked_open)
+        driver = utils.get_interface_driver('eth1')
+        self.assertFalse(driver)
+
+    def test_get_interface_driver_fail_empty(self):
+        mocked_open = mock.mock_open(read_data='DRIVER\n')
+        self.stub_out('os_net_config.utils.open', mocked_open)
+        driver = utils.get_interface_driver('eth1')
+        self.assertFalse(driver)
+
     def test__update_dpdk_map_new(self):
         utils._update_dpdk_map('eth1', '0000:03:00.0', '01:02:03:04:05:06',
                                'vfio-pci')
         contents = utils.get_file_data(utils._DPDK_MAPPING_FILE)
 
         dpdk_map = yaml.safe_load(contents) if contents else []
         self.assertEqual(1, len(dpdk_map))
```

### Comparing `os-net-config-9.4.0/os_net_config/tests/base.py` & `os-net-config-9.4.1/os_net_config/tests/base.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_validator.py` & `os-net-config-9.4.1/os_net_config/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/tests/test_cli.py` & `os-net-config-9.4.1/os_net_config/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/os_net_config/utils.py` & `os-net-config-9.4.1/os_net_config/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,19 @@
     logger.debug("Diff file data:\n%s" % file_data)
     logger.debug("Diff data:\n%s" % data)
     # convert to string as JSON may have unicode in it
     return not file_data == data
 
 
 def bind_dpdk_interfaces(ifname, driver, noop):
+    iface_driver = get_interface_driver(ifname)
+    if iface_driver == driver:
+        logger.info("Driver (%s) is already bound to the device (%s)" %
+                    (driver, ifname))
+        return
     pci_address = get_pci_address(ifname, noop)
     if not noop:
         if pci_address:
             # modbprobe of the driver has to be done before binding.
             # for reboots, puppet will add the modprobe to /etc/rc.modules
             if 'vfio-pci' in driver:
                 try:
@@ -358,14 +363,28 @@
                   'r') as f:
             out = f.read().strip()
         return out
     except IOError:
         return
 
 
+def get_interface_driver(ifname):
+    try:
+        uevent = '%s/%s/device/uevent' % (_SYS_CLASS_NET, ifname)
+        with open(uevent, 'r') as f:
+            out = f.read().strip()
+            for line in out.split('\n'):
+                if 'DRIVER' in line:
+                    driver = line.split('=')
+                    if len(driver) == 2:
+                        return driver[1]
+    except IOError:
+        return
+
+
 def get_dpdk_devargs(ifname, noop):
     if not noop:
         vendor_id = get_vendor_id(ifname)
         device_id = get_device_id(ifname)
         if vendor_id == "0x15b3" and device_id == "0x1007":
             # Some NICs (i.e. Mellanox ConnectX-3) have only one PCI address
             # associated with multiple ports. Using a PCI device won’t work.
@@ -413,14 +432,18 @@
         if item['name'] == name:
             return item['mac_address']
 
 
 def update_sriov_pf_map(ifname, numvfs, noop, promisc=None,
                         link_mode='legacy'):
     if not noop:
+        cur_numvfs = sriov_config.get_numvfs(ifname)
+        if cur_numvfs > 0 and cur_numvfs != numvfs:
+            msg = ("Can't change the numvfs for %s" % ifname)
+            raise sriov_config.SRIOVNumvfsException(msg)
         sriov_map = _get_sriov_map()
         for item in sriov_map:
             if item['device_type'] == 'pf' and item['name'] == ifname:
                 item['numvfs'] = numvfs
                 if promisc is not None:
                     item['promisc'] = promisc
                 item['link_mode'] = link_mode
@@ -510,17 +533,18 @@
      during reboot of the nodes.
     """
     with open(_SRIOV_CONFIG_SERVICE_FILE, 'w') as f:
         f.write(_SRIOV_CONFIG_DEVICE_CONTENT)
     processutils.execute('systemctl', 'enable', 'sriov_config')
 
 
-def configure_sriov_pfs():
+def configure_sriov_pfs(execution_from_cli=False, restart_openvswitch=False):
     logger.info("Configuring PFs now")
-    sriov_config.configure_sriov_pf()
+    sriov_config.configure_sriov_pf(execution_from_cli=execution_from_cli,
+                                    restart_openvswitch=restart_openvswitch)
     _configure_sriov_config_service()
 
 
 def configure_sriov_vfs():
     logger.info("Configuring VFs now")
     sriov_config.configure_sriov_vf()
```

### Comparing `os-net-config-9.4.0/test-requirements.txt` & `os-net-config-9.4.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/README.rst` & `os-net-config-9.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `os-net-config-9.4.0/ChangeLog` & `os-net-config-9.4.1/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 CHANGES
 =======
 
+9.4.1
+-----
+
+* Replace coremask with cpu\_list in vrouter schema
+* fix missing shared\_block for PF interface in switchdev bond connected to ovs
+* Avoid driverctl run if the driver is already bound
+* Numvfs setting during update/upgrade
+* Add ETHTOOL\_OPTS support for LinuxBond class
+* ifdown does not work if no ifcfg file exist
+* Moving insignificant messages from error to warning in sriov\_config.py
+* Restructuring the method of vf-representor renaming
+* Fix handling of SR-IOV PF routes
+
 9.4.0
 -----
 
 * Fixed the false InvalidConfigException for vfid=0
 * [FUP] Update sriov\_pf.yaml samle with ethtool\_opt
 * Add support for ethtool options for sriov\_pf ports
 * Unify ethtool options logic
```

### Comparing `os-net-config-9.4.0/PKG-INFO` & `os-net-config-9.4.1/os_net_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-net-config
-Version: 9.4.0
+Version: 9.4.1
 Summary: OpenStack network configuration
 Home-page: http://git.openstack.org/cgit/openstack/os-net-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: Apache License (2.0)
 Description: ========================
         Team and repository tags
```

### Comparing `os-net-config-9.4.0/setup.cfg` & `os-net-config-9.4.1/setup.cfg`

 * *Files identical despite different names*

