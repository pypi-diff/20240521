# Comparing `tmp/asusrouter-1.8.0.tar.gz` & `tmp/asusrouter-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asusrouter-1.8.0.tar", last modified: Wed Mar 20 21:12:06 2024, max compression
+gzip compressed data, was "asusrouter-1.9.0.tar", last modified: Wed May  1 08:38:20 2024, max compression
```

## Comparing `asusrouter-1.8.0.tar` & `asusrouter-1.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.944893 asusrouter-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-20 21:11:52.000000 asusrouter-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-20 21:11:52.000000 asusrouter-1.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-03-20 21:12:06.944893 asusrouter-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-03-20 21:11:52.000000 asusrouter-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.936893 asusrouter-1.8.0/asusrouter/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30935 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/asusrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.940893 asusrouter-1.8.0/asusrouter/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/access_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/aimesh.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/data_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/data_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.944893 asusrouter-1.8.0/asusrouter/modules/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/devicemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/devicemap_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/ethernet_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/firmware_note.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/firmware_note_aimesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/hook_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/networkmapd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/port_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/update_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/vpn_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/endpoint/wan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/homeassistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/led.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/openvpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/parental_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/port_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/vpnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/wireguard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/modules/wlan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.944893 asusrouter-1.8.0/asusrouter/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-20 21:11:52.000000 asusrouter-1.8.0/asusrouter/tools/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.944893 asusrouter-1.8.0/asusrouter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-03-20 21:12:06.000000 asusrouter-1.8.0/asusrouter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-20 21:12:06.000000 asusrouter-1.8.0/asusrouter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 21:12:06.000000 asusrouter-1.8.0/asusrouter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 21:12:06.000000 asusrouter-1.8.0/asusrouter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 21:12:06.000000 asusrouter-1.8.0/asusrouter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-20 21:11:52.000000 asusrouter-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-20 21:12:06.944893 asusrouter-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:12:06.944893 asusrouter-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-03-20 21:11:52.000000 asusrouter-1.8.0/tests/test_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.095998 asusrouter-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 08:38:08.000000 asusrouter-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 08:38:08.000000 asusrouter-1.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-01 08:38:20.095998 asusrouter-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-05-01 08:38:08.000000 asusrouter-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.083998 asusrouter-1.9.0/asusrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30935 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/asusrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.087998 asusrouter-1.9.0/asusrouter/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/access_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/aimesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/data_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/data_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.091998 asusrouter-1.9.0/asusrouter/modules/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/devicemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/devicemap_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/ethernet_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/firmware_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/firmware_note_aimesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/hook_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/networkmapd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/port_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/update_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/vpn_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/endpoint/wan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/homeassistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/openvpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/parental_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/port_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/vpnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/wireguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/modules/wlan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.095998 asusrouter-1.9.0/asusrouter/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-01 08:38:08.000000 asusrouter-1.9.0/asusrouter/tools/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.095998 asusrouter-1.9.0/asusrouter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-01 08:38:20.000000 asusrouter-1.9.0/asusrouter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-01 08:38:20.000000 asusrouter-1.9.0/asusrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:38:20.000000 asusrouter-1.9.0/asusrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 08:38:20.000000 asusrouter-1.9.0/asusrouter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 08:38:20.000000 asusrouter-1.9.0/asusrouter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 08:38:08.000000 asusrouter-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 08:38:20.095998 asusrouter-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:38:20.095998 asusrouter-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-01 08:38:08.000000 asusrouter-1.9.0/tests/test_devices.py
```

### Comparing `asusrouter-1.8.0/LICENSE` & `asusrouter-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/PKG-INFO` & `asusrouter-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asusrouter
-Version: 1.8.0
+Version: 1.9.0
 Summary: API wrapper for communication with ASUSWRT-powered routers using HTTP protocol
 Home-page: https://github.com/Vaskivskyi/asusrouter
 Author-email: Yevhenii Vaskivskyi <yevhenii@vaskivskyi.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/Vaskivskyi/asusrouter
 Project-URL: Bug Reports, https://github.com/Vaskivskyi/asusrouter/issues
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asusrouter Version: 1.8.0 Summary: API wrapper for
+Metadata-Version: 2.1 Name: asusrouter Version: 1.9.0 Summary: API wrapper for
 communication with ASUSWRT-powered routers using HTTP protocol Home-page:
 https://github.com/Vaskivskyi/asusrouter Author-email: Yevhenii Vaskivskyi
 vaskivskyi.com> License: Apache-2.0 Project-URL: Source Code, https://
 github.com/Vaskivskyi/asusrouter Project-URL: Bug Reports, https://github.com/
 Vaskivskyi/asusrouter/issues Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
```

### Comparing `asusrouter-1.8.0/README.md` & `asusrouter-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/__main__.py` & `asusrouter-1.9.0/asusrouter/__main__.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/asusrouter.py` & `asusrouter-1.9.0/asusrouter/asusrouter.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/connection.py` & `asusrouter-1.9.0/asusrouter/connection.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/const.py` & `asusrouter-1.9.0/asusrouter/const.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/error.py` & `asusrouter-1.9.0/asusrouter/error.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/aimesh.py` & `asusrouter-1.9.0/asusrouter/modules/aimesh.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/client.py` & `asusrouter-1.9.0/asusrouter/modules/client.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/connection.py` & `asusrouter-1.9.0/asusrouter/modules/connection.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/data.py` & `asusrouter-1.9.0/asusrouter/modules/data.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/data_finder.py` & `asusrouter-1.9.0/asusrouter/modules/data_finder.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/data_transform.py` & `asusrouter-1.9.0/asusrouter/modules/data_transform.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/__init__.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/devicemap.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/devicemap.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/devicemap_const.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/devicemap_const.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/error.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/error.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/ethernet_ports.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/ethernet_ports.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/firmware.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/firmware.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/firmware_note.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/firmware_note.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/hook.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/hook.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/hook_const.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/hook_const.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/onboarding.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/onboarding.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/port_status.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/port_status.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/sysinfo.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/sysinfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,28 +54,39 @@
         }
     sysinfo["connections"] = connections_info
 
     # Memory info
     memory_info = {}
     memory_data = data.get("mem_stats_arr")
     if memory_data:
+        # Before 388.7
         # JFFS data is presented as a string of `XX.xx / YY.yy MB`
         # where `XX.xx` is the used space (float) and `YY.yy` is the total space (float)
-        jffs_data = memory_data[7][:-3].split(" / ")
-        jffs_used = safe_float(jffs_data[0])
-        jffs_total = safe_float(jffs_data[1])
+        jffs = memory_data[7]
+        if "/" in jffs:
+            jffs_data = jffs[:-3].split(" / ")
+            jffs_used = safe_float(jffs_data[0])
+            jffs_total = safe_float(jffs_data[1])
+            jffs_free = jffs_total - jffs_used if jffs_used and jffs_total else None
+        # From 388.7
+        # JFFS is just a `free` single float
+        else:
+            jffs_free = safe_float(jffs)
+            jffs_used = None
+            jffs_total = None
 
         memory_info = {
             "total": safe_float(memory_data[0]),
             "free": safe_float(memory_data[1]),
             "buffers": safe_float(memory_data[2]),
             "cache": safe_float(memory_data[3]),
             "swap_1": safe_float(memory_data[4]),
             "swap_2": safe_float(memory_data[5]),
             "nvram": safe_int(memory_data[6]),
+            "jffs_free": jffs_free,
             "jffs_used": jffs_used,
             "jffs_total": jffs_total,
         }
     sysinfo["memory"] = memory_info
 
     # Load average info
     load_avg_info = {}
```

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/temperature.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/temperature.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/update_clients.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/update_clients.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/vpn.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/vpn.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/endpoint/vpn_const.py` & `asusrouter-1.9.0/asusrouter/modules/endpoint/vpn_const.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/firmware.py` & `asusrouter-1.9.0/asusrouter/modules/firmware.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/homeassistant.py` & `asusrouter-1.9.0/asusrouter/modules/homeassistant.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/identity.py` & `asusrouter-1.9.0/asusrouter/modules/identity.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/ip_address.py` & `asusrouter-1.9.0/asusrouter/modules/ip_address.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/led.py` & `asusrouter-1.9.0/asusrouter/modules/led.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/openvpn.py` & `asusrouter-1.9.0/asusrouter/modules/openvpn.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/parental_control.py` & `asusrouter-1.9.0/asusrouter/modules/parental_control.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/port_forwarding.py` & `asusrouter-1.9.0/asusrouter/modules/port_forwarding.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/ports.py` & `asusrouter-1.9.0/asusrouter/modules/ports.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/service.py` & `asusrouter-1.9.0/asusrouter/modules/service.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/state.py` & `asusrouter-1.9.0/asusrouter/modules/state.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/system.py` & `asusrouter-1.9.0/asusrouter/modules/system.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/vpnc.py` & `asusrouter-1.9.0/asusrouter/modules/vpnc.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/wireguard.py` & `asusrouter-1.9.0/asusrouter/modules/wireguard.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/modules/wlan.py` & `asusrouter-1.9.0/asusrouter/modules/wlan.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/tools/cleaners.py` & `asusrouter-1.9.0/asusrouter/tools/cleaners.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/tools/converters.py` & `asusrouter-1.9.0/asusrouter/tools/converters.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/tools/dump.py` & `asusrouter-1.9.0/asusrouter/tools/dump.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/tools/legacy.py` & `asusrouter-1.9.0/asusrouter/tools/legacy.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/tools/readers.py` & `asusrouter-1.9.0/asusrouter/tools/readers.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter/tools/writers.py` & `asusrouter-1.9.0/asusrouter/tools/writers.py`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/asusrouter.egg-info/PKG-INFO` & `asusrouter-1.9.0/asusrouter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asusrouter
-Version: 1.8.0
+Version: 1.9.0
 Summary: API wrapper for communication with ASUSWRT-powered routers using HTTP protocol
 Home-page: https://github.com/Vaskivskyi/asusrouter
 Author-email: Yevhenii Vaskivskyi <yevhenii@vaskivskyi.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/Vaskivskyi/asusrouter
 Project-URL: Bug Reports, https://github.com/Vaskivskyi/asusrouter/issues
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asusrouter Version: 1.8.0 Summary: API wrapper for
+Metadata-Version: 2.1 Name: asusrouter Version: 1.9.0 Summary: API wrapper for
 communication with ASUSWRT-powered routers using HTTP protocol Home-page:
 https://github.com/Vaskivskyi/asusrouter Author-email: Yevhenii Vaskivskyi
 vaskivskyi.com> License: Apache-2.0 Project-URL: Source Code, https://
 github.com/Vaskivskyi/asusrouter Project-URL: Bug Reports, https://github.com/
 Vaskivskyi/asusrouter/issues Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
```

### Comparing `asusrouter-1.8.0/asusrouter.egg-info/SOURCES.txt` & `asusrouter-1.9.0/asusrouter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asusrouter-1.8.0/pyproject.toml` & `asusrouter-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name            = "asusrouter"
-version         = "1.8.0"
+version         = "1.9.0"
 license         = {text = "Apache-2.0"}
 requires-python = ">=3.11.0"
 readme          = "README.md"
 description     = "API wrapper for communication with ASUSWRT-powered routers using HTTP protocol"
 authors         = [
     { name="Yevhenii Vaskivskyi", email="yevhenii@vaskivskyi.com" },
 ]
```

### Comparing `asusrouter-1.8.0/tests/test_devices.py` & `asusrouter-1.9.0/tests/test_devices.py`

 * *Files identical despite different names*

