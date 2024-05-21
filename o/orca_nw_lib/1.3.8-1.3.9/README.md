# Comparing `tmp/orca_nw_lib-1.3.8.tar.gz` & `tmp/orca_nw_lib-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orca_nw_lib-1.3.8.tar", max compression
+gzip compressed data, was "orca_nw_lib-1.3.9.tar", max compression
```

## Comparing `orca_nw_lib-1.3.8.tar` & `orca_nw_lib-1.3.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      626 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/LICENSE
--rw-r--r--   0        0        0      373 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/__init__.py
--rw-r--r--   0        0        0    13119 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/bgp.py
--rw-r--r--   0        0        0     8802 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/bgp_db.py
--rw-r--r--   0        0        0    11382 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/bgp_gnmi.py
--rw-r--r--   0        0        0     2466 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/common.py
--rw-r--r--   0        0        0      226 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/constants.py
--rw-r--r--   0        0        0     1938 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/device.py
--rw-r--r--   0        0        0      743 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/device_db.py
--rw-r--r--   0        0        0     4613 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/device_gnmi.py
--rw-r--r--   0        0        0     6464 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/discovery.py
--rw-r--r--   0        0        0     4276 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/generate_code.py
--rw-r--r--   0        0        0     2677 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py
--rw-r--r--   0        0        0     2711 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/github.com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2_grpc.py
--rw-r--r--   0        0        0    12062 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.py
--rw-r--r--   0        0        0    16347 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.pyi
--rw-r--r--   0        0        0     7757 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2_grpc.py
--rw-r--r--   0        0        0    13499 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_sub.py
--rw-r--r--   0        0        0     5522 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_util.py
--rw-r--r--   0        0        0     7697 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/graph_db_models.py
--rw-r--r--   0        0        0    12476 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/interface.py
--rw-r--r--   0        0        0     8327 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/interface_db.py
--rw-r--r--   0        0        0    18809 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/interface_gnmi.py
--rw-r--r--   0        0        0     7190 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/lldp.py
--rw-r--r--   0        0        0    12716 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/mclag.py
--rw-r--r--   0        0        0    11774 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/mclag_db.py
--rw-r--r--   0        0        0     7836 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/mclag_gnmi.py
--rw-r--r--   0        0        0       75 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/orca_exceptions.py
--rw-r--r--   0        0        0      777 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib.yml
--rw-r--r--   0        0        0      577 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib_logging.yml
--rw-r--r--   0        0        0     8967 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/port_chnl.py
--rw-r--r--   0        0        0     5712 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_db.py
--rw-r--r--   0        0        0     9590 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_gnmi.py
--rw-r--r--   0        0        0     5578 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/portgroup.py
--rw-r--r--   0        0        0     4539 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/portgroup_db.py
--rw-r--r--   0        0        0     3959 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/portgroup_gnmi.py
--rw-r--r--   0        0        0     4708 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/utils.py
--rw-r--r--   0        0        0     9703 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/vlan.py
--rw-r--r--   0        0        0     4507 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/vlan_db.py
--rw-r--r--   0        0        0    14539 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/vlan_gnmi.py
--rw-r--r--   0        0        0      508 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     7034 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/readme.md
--rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 orca_nw_lib-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0      626 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/LICENSE
+-rw-r--r--   0        0        0      373 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/__init__.py
+-rw-r--r--   0        0        0    13119 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/bgp.py
+-rw-r--r--   0        0        0     8802 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/bgp_db.py
+-rw-r--r--   0        0        0    11382 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/bgp_gnmi.py
+-rw-r--r--   0        0        0     2466 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/common.py
+-rw-r--r--   0        0        0      226 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/constants.py
+-rw-r--r--   0        0        0     1938 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/device.py
+-rw-r--r--   0        0        0      743 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/device_db.py
+-rw-r--r--   0        0        0     4613 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/device_gnmi.py
+-rw-r--r--   0        0        0     6464 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/discovery.py
+-rw-r--r--   0        0        0     4276 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/generate_code.py
+-rw-r--r--   0        0        0     2677 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py
+-rw-r--r--   0        0        0     2711 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/github.com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2_grpc.py
+-rw-r--r--   0        0        0    12062 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/gnmi_pb2.py
+-rw-r--r--   0        0        0    16347 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/gnmi_pb2.pyi
+-rw-r--r--   0        0        0     7757 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/gnmi_pb2_grpc.py
+-rw-r--r--   0        0        0    13499 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/gnmi_sub.py
+-rw-r--r--   0        0        0     5522 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/gnmi_util.py
+-rw-r--r--   0        0        0     7792 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/graph_db_models.py
+-rw-r--r--   0        0        0    12466 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/interface.py
+-rw-r--r--   0        0        0     8327 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/interface_db.py
+-rw-r--r--   0        0        0    18835 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/interface_gnmi.py
+-rw-r--r--   0        0        0     7190 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/lldp.py
+-rw-r--r--   0        0        0    12716 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/mclag.py
+-rw-r--r--   0        0        0    11774 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/mclag_db.py
+-rw-r--r--   0        0        0     7836 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/mclag_gnmi.py
+-rw-r--r--   0        0        0       75 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/orca_exceptions.py
+-rw-r--r--   0        0        0      777 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/orca_nw_lib.yml
+-rw-r--r--   0        0        0      577 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/orca_nw_lib_logging.yml
+-rw-r--r--   0        0        0     8967 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/port_chnl.py
+-rw-r--r--   0        0        0     5712 2024-05-21 07:47:14.034297 orca_nw_lib-1.3.9/orca_nw_lib/port_chnl_db.py
+-rw-r--r--   0        0        0    11613 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/port_chnl_gnmi.py
+-rw-r--r--   0        0        0     5578 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/portgroup.py
+-rw-r--r--   0        0        0     4539 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/portgroup_db.py
+-rw-r--r--   0        0        0     3959 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/portgroup_gnmi.py
+-rw-r--r--   0        0        0     4708 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/utils.py
+-rw-r--r--   0        0        0    10222 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/vlan.py
+-rw-r--r--   0        0        0     5785 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/vlan_db.py
+-rw-r--r--   0        0        0    15311 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/orca_nw_lib/vlan_gnmi.py
+-rw-r--r--   0        0        0      508 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     7072 2024-05-21 07:47:14.038297 orca_nw_lib-1.3.9/readme.md
+-rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 orca_nw_lib-1.3.9/PKG-INFO
```

### Comparing `orca_nw_lib-1.3.8/LICENSE` & `orca_nw_lib-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/bgp.py` & `orca_nw_lib-1.3.9/orca_nw_lib/bgp.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/bgp_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/bgp_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/bgp_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/bgp_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/common.py` & `orca_nw_lib-1.3.9/orca_nw_lib/common.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/device.py` & `orca_nw_lib-1.3.9/orca_nw_lib/device.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/device_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/device_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/device_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/device_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/discovery.py` & `orca_nw_lib-1.3.9/orca_nw_lib/discovery.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/generate_code.py` & `orca_nw_lib-1.3.9/orca_nw_lib/generate_code.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py` & `orca_nw_lib-1.3.9/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi` & `orca_nw_lib-1.3.9/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.py` & `orca_nw_lib-1.3.9/orca_nw_lib/gnmi_pb2.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.pyi` & `orca_nw_lib-1.3.9/orca_nw_lib/gnmi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2_grpc.py` & `orca_nw_lib-1.3.9/orca_nw_lib/gnmi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_sub.py` & `orca_nw_lib-1.3.9/orca_nw_lib/gnmi_sub.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_util.py` & `orca_nw_lib-1.3.9/orca_nw_lib/gnmi_util.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/graph_db_models.py` & `orca_nw_lib-1.3.9/orca_nw_lib/graph_db_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,15 @@
     autostate = StringProperty()
     ip_address = StringProperty()
     sag_ip_address = StringProperty()
     enabled = BooleanProperty()
     description = StringProperty()
 
     memberInterfaces = RelationshipTo("Interface", "MEMBER_IF", model=VlanMemRel)
+    memberPortChannel = RelationshipTo("PortChannel", "MEMBER_PORT_CHANNEL", model=VlanMemRel)
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.vlanid == other.vlanid
         return NotImplemented
 
     def __hash__(self):
```

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/interface.py` & `orca_nw_lib-1.3.9/orca_nw_lib/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     get_sub_interface_of_intfc_from_db,
     insert_device_interfaces_in_db,
 )
 from .interface_gnmi import (
     del_all_subinterfaces_of_all_interfaces_from_device,
     del_all_subinterfaces_of_interface_from_device,
     get_interface_from_device,
-    set_vlan_if_mode_on_device,
+    set_if_vlan_on_device,
     set_interface_config_on_device,
     remove_vlan_from_if_from_device,
 )
 from .portgroup import discover_port_groups
 from .portgroup_db import (
     get_port_group_id_of_device_interface_from_db,
     get_port_group_of_if_from_db,
@@ -346,15 +346,15 @@
         vlan_id (int): The VLAN ID to set.
 
     Returns:
         None
     """
     _logger.info(f"Setting interface mode {if_mode} on interface {if_name}.")
     try:
-        set_vlan_if_mode_on_device(device_ip, if_name, if_mode, vlan_id)
+        set_if_vlan_on_device(device_ip, if_name, if_mode, vlan_id)
     except Exception as e:
         _logger.error(
             f"Setting interface mode {if_mode} on interface {if_name} on device {device_ip} failed, Reason: {e}"
         )
         raise
     finally:
         discover_interfaces(device_ip, if_name)
```

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/interface_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/interface_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/interface_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/interface_gnmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         updates.append(
             create_gnmi_update(
                 get_sub_interface_path(if_name),
                 ip_payload,
             )
         )
     if if_mode and vlan_id:
-        updates.append(get_if_mode_req(vlan_id, if_name, if_mode))
+        updates.append(get_if_vlan_gnmi_update_req(vlan_id, if_name, if_mode))
     if updates:
         return send_gnmi_set(
             create_req_for_update(updates),
             device_ip,
         )
     else:
         return None
@@ -584,26 +584,27 @@
             get_gnmi_path(
                 f"/openconfig-interfaces:interfaces/interface[name={intfc_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/interface-mode"
             )
         ],
     )
 
 
-def get_if_mode_req(vlan_id: int, if_name: str, if_mode: IFMode):
+def get_if_vlan_gnmi_update_req(vlan_id: int, if_name: str, if_mode: IFMode):
     """
     Creates a GNMI update request for the interface mode.
 
     Args:
         vlan_id (int): The VLAN ID.
         if_name (str): The name of the interface.
         if_mode (IFMode): The interface mode.
 
     Returns:
         The GNMI update request.
     """
+
     return create_gnmi_update(
         get_gnmi_path(
             f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config"
         ),
         (
             {
                 "openconfig-vlan:config": {
@@ -618,27 +619,25 @@
                     "trunk-vlans": [vlan_id],
                 }
             }
         ),
     )
 
 
-def set_vlan_if_mode_on_device(
-    device_ip: str, if_name: str, if_mode: IFMode, vlan_id: int
-):
+def set_if_vlan_on_device(device_ip: str, if_name: str, if_mode: IFMode, vlan_id: int):
     """
     Sets the interface mode on a device.
 
     Args:
         device_ip (str): The IP address of the device.
         if_name (str): The name of the interface.
         if_mode (IFMode): The interface mode.
         vlan_id (int): The VLAN ID.
 
     Returns:
         The result of the GNMI set operation.
     """
 
     return send_gnmi_set(
-        create_req_for_update([get_if_mode_req(vlan_id, if_name, if_mode)]),
+        create_req_for_update([get_if_vlan_gnmi_update_req(vlan_id, if_name, if_mode)]),
         device_ip,
     )
```

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/lldp.py` & `orca_nw_lib-1.3.9/orca_nw_lib/lldp.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/mclag.py` & `orca_nw_lib-1.3.9/orca_nw_lib/mclag.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/mclag_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/mclag_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/mclag_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/mclag_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib.yml` & `orca_nw_lib-1.3.9/orca_nw_lib/orca_nw_lib.yml`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib_logging.yml` & `orca_nw_lib-1.3.9/orca_nw_lib/orca_nw_lib_logging.yml`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/port_chnl.py` & `orca_nw_lib-1.3.9/orca_nw_lib/port_chnl.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/port_chnl_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/port_chnl_gnmi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+from orca_nw_lib.common import IFMode
 from orca_nw_lib.gnmi_pb2 import PathElem
 from orca_nw_lib.gnmi_util import (
     create_gnmi_update,
     create_req_for_update,
     send_gnmi_get,
     send_gnmi_set,
 )
 from orca_nw_lib.portgroup_gnmi import get_port_chnl_mem_base_path
 from orca_nw_lib.utils import get_logging
 from .gnmi_pb2 import Path, PathElem
 from .gnmi_util import (
     create_gnmi_update,
     create_req_for_update,
     get_gnmi_del_req,
+    get_gnmi_path,
     send_gnmi_get,
     send_gnmi_set,
 )
 
 _logger = get_logging().getLogger(__name__)
 
+
 def get_port_chnl_root_path() -> Path:
     """
     Get the root path of the port channel configuration in the OpenConfig model.
 
     Returns:
         A Path object representing the root path of the port channel configuration.
     """
@@ -278,15 +281,15 @@
 
     Returns:
         str: The response from the send_gnmi_set function.
     """
     port_chnl_add = {"sonic-portchannel:PORTCHANNEL_MEMBER_LIST": []}
     for intf in ifnames:
         port_chnl_add.get("sonic-portchannel:PORTCHANNEL_MEMBER_LIST").append(
-            {"ifname": intf,"name": chnl_name}
+            {"ifname": intf, "name": chnl_name}
         )
     _logger.debug(f"Adding port channel member on device {device_ip} {port_chnl_add}")
     return send_gnmi_set(
         create_req_for_update(
             [create_gnmi_update(get_port_chnl_mem_list_path(), port_chnl_add)]
         ),
         device_ip,
@@ -321,7 +324,65 @@
     port_chnl_add.get("sonic-portchannel:PORTCHANNEL_LIST").append(port_chnl_item)
     return send_gnmi_set(
         create_req_for_update(
             [create_gnmi_update(get_port_chnl_list_path(), port_chnl_add)]
         ),
         device_ip,
     )
+
+
+def get_port_channel_vlan_gnmi_update_req(vlan_id: int, port_channel_name: str, if_mode: IFMode):
+    """
+    Generates a GNMI update request for configuring VLAN settings on a port channel.
+
+    Parameters:
+        vlan_id (int): The VLAN ID to be configured.
+        port_channel_name (str): The name of the port channel.
+        if_mode (IFMode): The interface mode to set, either ACCESS or TRUNK.
+
+    Returns:
+        The GNMI update request for setting VLAN configuration on the specified port channel.
+    """
+    return create_gnmi_update(
+        get_gnmi_path(
+            f"/openconfig-interfaces:interfaces/interface[name={port_channel_name}]/openconfig-if-aggregate:aggregation/openconfig-vlan:switched-vlan/config"
+        ),
+        (
+            {
+                "openconfig-vlan:config": {
+                    "interface-mode": str(if_mode),
+                    "access-vlan": vlan_id,
+                }
+            }
+            if if_mode == IFMode.ACCESS
+            else {
+                "openconfig-vlan:config": {
+                    "interface-mode": str(if_mode),
+                    "trunk-vlans": [vlan_id],
+                }
+            }
+        ),
+    )
+
+
+def set_port_channel_vlan_on_device(
+    device_ip: str, port_channel_name: str, if_mode: IFMode, vlan_id: int
+):
+    """
+    Sets the VLAN configuration on a port channel for a specified device.
+
+    Parameters:
+        device_ip (str): The IP address of the device.
+        port_channel_name (str): The name of the port channel.
+        if_mode (IFMode): The interface mode to set, either ACCESS or TRUNK.
+        vlan_id (int): The VLAN ID to be configured.
+
+    Returns:
+        The result of sending a GNMI set request for configuring the VLAN settings on the port channel.
+    """
+    
+    return send_gnmi_set(
+        create_req_for_update(
+            [get_port_channel_vlan_gnmi_update_req(vlan_id, port_channel_name, if_mode)]
+        ),
+        device_ip,
+    )
```

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/portgroup.py` & `orca_nw_lib-1.3.9/orca_nw_lib/portgroup.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/portgroup_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/portgroup_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/portgroup_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/portgroup_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/utils.py` & `orca_nw_lib-1.3.9/orca_nw_lib/utils.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/vlan.py` & `orca_nw_lib-1.3.9/orca_nw_lib/vlan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from orca_nw_lib.graph_db_models import Vlan
 from orca_nw_lib.vlan_gnmi import get_vlan_details_from_device
 
 from .common import IFMode, VlanAutoState
 
 from .device_db import get_device_db_obj
 from .vlan_db import (
+    get_vlan_member_port_channels_from_db,
     get_vlan_obj_from_db,
     get_vlan_mem_ifcs_from_db,
     insert_vlan_in_db,
 )
 from .vlan_gnmi import (
     add_vlan_mem_interface_on_device,
     config_vlan_on_device,
@@ -72,18 +73,18 @@
             )
         )
 
     for vlan in vlan_details.get("sonic-vlan:VLAN_TABLE_LIST") or []:
         for v in vlans:
             if v.name == vlan.get("name"):
                 v.mtu = vlan.get("mtu")
-                v.enabled = True if vlan.get("admin_status")== "up" else False
+                v.enabled = True if vlan.get("admin_status") == "up" else False
                 v.oper_status = vlan.get("oper_status")
                 v.autostate = vlan.get("autostate")
-                v.description=vlan.get("description")
+                v.description = vlan.get("description")
 
     vlans_obj_vs_mem = {}
     for v in vlans:
         members = []
         for item in vlan_details.get("sonic-vlan:VLAN_MEMBER_LIST") or []:
             if v.name == item.get("name"):
                 members.append(item)
@@ -251,21 +252,34 @@
     Args:
         device_ip (str): The IP address of the device.
         vlan_name (str): The name of the VLAN.
 
     Returns:
         dict: A dictionary mapping member interface names to their corresponding tagging mode.
     """
-    members = get_vlan_mem_ifcs_from_db(device_ip, vlan_name)
     mem_intf_vs_tagging_mode = {}
-    for mem in members or []:
+
+    member_ethernet = get_vlan_mem_ifcs_from_db(device_ip, vlan_name)
+    for mem in member_ethernet or []:
         mem_rel = get_vlan_obj_from_db(
             device_ip, vlan_name
         ).memberInterfaces.relationship(mem)
-        mem_intf_vs_tagging_mode[mem.name] = mem_rel.tagging_mode
+        mem_intf_vs_tagging_mode[mem.name] = (
+            IFMode.TRUNK if mem_rel.tagging_mode == "tagged" else IFMode.ACCESS
+        )
+
+    member_port_channel = get_vlan_member_port_channels_from_db(device_ip, vlan_name)
+    for mem in member_port_channel or []:
+        mem_rel = get_vlan_obj_from_db(
+            device_ip, vlan_name
+        ).memberPortChannel.relationship(mem)
+        mem_intf_vs_tagging_mode[mem.lag_name] = (
+            IFMode.TRUNK if mem_rel.tagging_mode == "tagged" else IFMode.ACCESS
+        )
+
     return mem_intf_vs_tagging_mode
 
 
 def del_vlan_mem(device_ip: str, vlan_id: int, if_name: str, if_mode: IFMode):
     """
     Deletes a VLAN member from a device.
 
@@ -274,16 +288,16 @@
         vlan_id (int): The ID of the VLAN.
         if_name (str): The name of the interface to be removed from the VLAN.
         if_mode (IFMode): The mode of the interface to be removed from the VLAN.
 
     Returns:
         None
     """
-    
-    try: 
+
+    try:
         del_vlan_mem_interface_on_device(device_ip, vlan_id, if_name, if_mode)
     except Exception as e:
         _logger.error(f"VLAN member deletion failed on device {device_ip}, Reason: {e}")
         raise
     finally:
         discover_vlan(device_ip)
```

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/vlan_db.py` & `orca_nw_lib-1.3.9/orca_nw_lib/vlan_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import List, Optional
+
+from orca_nw_lib.port_chnl_db import get_port_chnl_of_device_from_db
 from .device_db import get_device_db_obj
 from .graph_db_models import Device, Vlan
 from .interface_db import get_interface_of_device_from_db
 
 
 def del_vlan_from_db(device_ip, vlan_name: str = None):
     """
@@ -57,14 +59,34 @@
     return (
         v.memberInterfaces.all()
         if device and device.vlans and (v := device.vlans.get_or_none(name=vlan_name))
         else None
     )
 
 
+def get_vlan_member_port_channels_from_db(device_ip: str, vlan_name: str) -> Optional[List[str]]:
+    """
+    Retrieves the member port channels of a specific VLAN from the device database.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        vlan_name (str): The name of the VLAN.
+
+    Returns:
+        List[str]: A list of member port channels if the device and VLAN exist in the database,
+        otherwise None.
+    """
+
+    device: Device = get_device_db_obj(device_ip)
+    return (
+        v.memberPortChannel.all()
+        if device and device.vlans and (v := device.vlans.get_or_none(name=vlan_name))
+        else None
+    )
+
 def copy_vlan_obj_prop(target_vlan_obj: Vlan, source_vlan_obj: Vlan):
     """
     Copy the properties of one VLAN object to another.
 
     Args:
         target_vlan_obj (Vlan): The target VLAN object to copy the properties to.
         source_vlan_obj (Vlan): The source VLAN object to copy the properties from.
@@ -108,20 +130,31 @@
 
         saved_vlan = get_vlan_obj_from_db(device.mgt_ip, vlan.name)
         
         ## For updating vlan members in db, lets first disconnect any existing members and recreate membership in DB.
         ## It will cater case when vlan has members are in db but not on device.
         ## Also the case when members has been changed/updated.
         saved_vlan.memberInterfaces.disconnect_all()
+        saved_vlan.memberPortChannel.disconnect_all()
         for mem in members:
-            intf = get_interface_of_device_from_db(
-                        device.mgt_ip, mem.get("ifname")
-                    )
-            if saved_vlan and intf:
-                mem_rel = saved_vlan.memberInterfaces.connect(intf)
-                mem_rel.tagging_mode = mem.get("tagging_mode")
-                mem_rel.save()
+            if "ethernet" in mem.get("ifname").lower():
+                intf = get_interface_of_device_from_db(
+                            device.mgt_ip, mem.get("ifname")
+                        )
+                if saved_vlan and intf:
+                    mem_rel = saved_vlan.memberInterfaces.connect(intf)
+                    mem_rel.tagging_mode = mem.get("tagging_mode")
+                    mem_rel.save()
+            else:
+                ## Its a port channel.
+                intf = get_port_chnl_of_device_from_db(
+                            device.mgt_ip, mem.get("ifname")
+                        )
+                if saved_vlan and intf:
+                    mem_rel = saved_vlan.memberPortChannel.connect(intf)
+                    mem_rel.tagging_mode = mem.get("tagging_mode")
+                    mem_rel.save()
     ## Handle the case when some or all vlans has been deleted from device but remained in DB
     ## Remove all vlans which are in DB but not on device.
     for vlan_in_db in get_vlan_obj_from_db(device.mgt_ip):
         if vlan_in_db not in vlans_obj_vs_mem:
             del_vlan_from_db(device.mgt_ip, vlan_in_db.name)
```

### Comparing `orca_nw_lib-1.3.8/orca_nw_lib/vlan_gnmi.py` & `orca_nw_lib-1.3.9/orca_nw_lib/vlan_gnmi.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     create_gnmi_update,
     create_req_for_update,
     get_gnmi_del_req,
     send_gnmi_get,
     send_gnmi_set,
     get_gnmi_path,
 )
-from orca_nw_lib.interface_gnmi import get_if_mode_req
+from orca_nw_lib.interface_gnmi import get_if_vlan_gnmi_update_req
+from orca_nw_lib.port_chnl_gnmi import get_port_channel_vlan_gnmi_update_req
 from .utils import validate_and_get_ip_prefix
 
 
 def get_sonic_vlan_base_path() -> Path:
     """
     Generates a `Path` object for the sonic-vlan base path.
 
@@ -329,15 +330,18 @@
         mem_ifs (dict[str:IFMode]): A dictionary mapping interface names to their mode.
 
     Returns:
         list: A list of GNMI updates for adding VLAN member interfaces.
     """
     req = []
     for if_name, if_mode in mem_ifs.items():
-        req.append(get_if_mode_req(vlan_id, if_name, if_mode))
+        if "portchannel" in if_name.lower():
+            req.append(get_port_channel_vlan_gnmi_update_req(vlan_id, if_name, if_mode))
+        else:
+            req.append(get_if_vlan_gnmi_update_req(vlan_id, if_name, if_mode))
     return req
 
 
 def add_vlan_mem_interface_on_device(
     device_ip: str, vlan_id: int, mem_ifs: dict[str:IFMode]
 ):
     """
@@ -357,31 +361,37 @@
     )
 
 
 def del_vlan_mem_interface_on_device(
     device_ip: str, vlan_id: int, if_name: str, if_mode: IFMode
 ):
     """
-    Deletes a VLAN member interface on a device using the specified device IP, VLAN ID, and interface name.
+    Deletes a VLAN member interface on a device using the specified device IP, VLAN ID, interface name, and interface mode.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_id (int): The ID of the VLAN.
         if_name (str): The name of the interface to be removed from the VLAN.
         if_mode (IFMode): The mode of the interface to be removed from the VLAN.
 
     Returns:
         Result of sending a GNMI set request to delete the VLAN member interface.
     """
+    
     return send_gnmi_set(
         get_gnmi_del_req(
             get_gnmi_path(
                 f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/trunk-vlans[trunk-vlans={vlan_id}]"
                 if if_mode == IFMode.TRUNK
                 else f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/access-vlan"
+            ) if "ethernet" in if_name.lower() else ## Its a port channel
+            get_gnmi_path(
+                f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-aggregate:aggregation/openconfig-vlan:switched-vlan/config/trunk-vlans[trunk-vlans={vlan_id}]"
+                if if_mode == IFMode.TRUNK
+                else f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-aggregate:aggregation/openconfig-vlan:switched-vlan/config/access-vlan"
             )
         ),
         device_ip,
     )
 
 
 def vlan_ip_addr_oc_path(vlan_name, ip_addr=None):
```

### Comparing `orca_nw_lib-1.3.8/readme.md` & `orca_nw_lib-1.3.9/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         --env NEO4J_AUTH=neo4j/password \
         neo4j:latest
 Then open https://localhost:7474 with credentials neo4j/password to browse the database.
 
 
 ### orca_nw_lib configuration
 In the application where orca_nw_lib is used, `load_orca_config` function in [utils.py](orca_nw_lib/utils.py) must be called before using any APIs of orca_nw_lib. This function loads device and neo4j access information also the logging configuration by default from 
-[orca.yml](orca_nw_lib/orca.yml) and [logging.yml](orca_nw_lib/logging.yml) files.
+[orca_nw_lib.yml](orca_nw_lib/orca_nw_lib.yml) and [orca_nw_lib_logging.yml](orca_nw_lib/orca_nw_lib_logging.yml) files.
 Although user can call load_orca_config with custom config files.
 The parameter information is documented in orca.yml file and logging.yml is standard python logging configuration file.
 
 ## Build and Install orca_nw_lib from source
 Optionally if user want to build and install orca_nw_lib from source, ORCA Network Library uses poetry to build the orca_nw_lib package. As a pre-requisite poetry must be installed in this case. Poetry can be easily installed using the following command :
         
     pip install poetry
```

### Comparing `orca_nw_lib-1.3.8/PKG-INFO` & `orca_nw_lib-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orca_nw_lib
-Version: 1.3.8
+Version: 1.3.9
 Summary: APIs to interact with SONiC NW
 Author: Kamal Krishna Bhatt
 Author-email: kamal.bhatt@stordis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -60,15 +60,15 @@
         --env NEO4J_AUTH=neo4j/password \
         neo4j:latest
 Then open https://localhost:7474 with credentials neo4j/password to browse the database.
 
 
 ### orca_nw_lib configuration
 In the application where orca_nw_lib is used, `load_orca_config` function in [utils.py](orca_nw_lib/utils.py) must be called before using any APIs of orca_nw_lib. This function loads device and neo4j access information also the logging configuration by default from 
-[orca.yml](orca_nw_lib/orca.yml) and [logging.yml](orca_nw_lib/logging.yml) files.
+[orca_nw_lib.yml](orca_nw_lib/orca_nw_lib.yml) and [orca_nw_lib_logging.yml](orca_nw_lib/orca_nw_lib_logging.yml) files.
 Although user can call load_orca_config with custom config files.
 The parameter information is documented in orca.yml file and logging.yml is standard python logging configuration file.
 
 ## Build and Install orca_nw_lib from source
 Optionally if user want to build and install orca_nw_lib from source, ORCA Network Library uses poetry to build the orca_nw_lib package. As a pre-requisite poetry must be installed in this case. Poetry can be easily installed using the following command :
         
     pip install poetry
```

