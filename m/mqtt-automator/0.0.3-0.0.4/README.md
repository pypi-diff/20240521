# Comparing `tmp/mqtt_automator-0.0.3.tar.gz` & `tmp/mqtt_automator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_automator-0.0.3.tar", last modified: Mon May 20 12:59:49 2024, max compression
+gzip compressed data, was "mqtt_automator-0.0.4.tar", last modified: Tue May 21 16:25:50 2024, max compression
```

## Comparing `mqtt_automator-0.0.3.tar` & `mqtt_automator-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1068 2024-05-01 11:55:42.000000 mqtt_automator-0.0.3/LICENSE
--rw-r--r--   0 oleg      (1000) oleg      (1000)     7256 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5371 2024-05-16 19:47:21.000000 mqtt_automator-0.0.3/README.md
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.3/mqtt_automator/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3629 2024-05-20 12:53:26.000000 mqtt_automator-0.0.3/mqtt_automator/automator.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      226 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/broker.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator/config/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.3/mqtt_automator/config/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6339 2024-05-20 12:56:20.000000 mqtt_automator-0.0.3/mqtt_automator/config/parser.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1308 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/config/time_parser.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator/devices/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       29 2024-05-16 19:36:52.000000 mqtt_automator-0.0.3/mqtt_automator/devices/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2860 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/base.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1411 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/lytko.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1344 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/vakio.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1927 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/yeelink.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator.egg-info/
--rw-r--r--   0 oleg      (1000) oleg      (1000)     7256 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      637 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       69 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/entry_points.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       95 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/requires.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       15 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/top_level.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1258 2024-05-20 12:59:36.000000 mqtt_automator-0.0.3/pyproject.toml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/setup.cfg
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/tests/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2552 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/tests/test_config_parser.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-21 16:25:50.453487 mqtt_automator-0.0.4/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1068 2024-05-01 11:55:42.000000 mqtt_automator-0.0.4/LICENSE
+-rw-r--r--   0 oleg      (1000) oleg      (1000)     7256 2024-05-21 16:25:50.453487 mqtt_automator-0.0.4/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5371 2024-05-16 19:47:21.000000 mqtt_automator-0.0.4/README.md
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-21 16:25:50.449487 mqtt_automator-0.0.4/mqtt_automator/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.4/mqtt_automator/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3730 2024-05-21 16:24:49.000000 mqtt_automator-0.0.4/mqtt_automator/automator.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      226 2024-05-20 11:48:34.000000 mqtt_automator-0.0.4/mqtt_automator/broker.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-21 16:25:50.449487 mqtt_automator-0.0.4/mqtt_automator/config/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.4/mqtt_automator/config/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6527 2024-05-21 16:24:49.000000 mqtt_automator-0.0.4/mqtt_automator/config/parser.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1308 2024-05-20 11:48:34.000000 mqtt_automator-0.0.4/mqtt_automator/config/time_parser.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-21 16:25:50.449487 mqtt_automator-0.0.4/mqtt_automator/devices/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       29 2024-05-16 19:36:52.000000 mqtt_automator-0.0.4/mqtt_automator/devices/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2925 2024-05-21 16:24:49.000000 mqtt_automator-0.0.4/mqtt_automator/devices/base.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1411 2024-05-20 11:48:34.000000 mqtt_automator-0.0.4/mqtt_automator/devices/lytko.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1344 2024-05-20 11:48:34.000000 mqtt_automator-0.0.4/mqtt_automator/devices/vakio.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2687 2024-05-21 16:24:49.000000 mqtt_automator-0.0.4/mqtt_automator/devices/yeelink.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-21 16:25:50.449487 mqtt_automator-0.0.4/mqtt_automator.egg-info/
+-rw-r--r--   0 oleg      (1000) oleg      (1000)     7256 2024-05-21 16:25:50.000000 mqtt_automator-0.0.4/mqtt_automator.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      637 2024-05-21 16:25:50.000000 mqtt_automator-0.0.4/mqtt_automator.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2024-05-21 16:25:50.000000 mqtt_automator-0.0.4/mqtt_automator.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       69 2024-05-21 16:25:50.000000 mqtt_automator-0.0.4/mqtt_automator.egg-info/entry_points.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       95 2024-05-21 16:25:50.000000 mqtt_automator-0.0.4/mqtt_automator.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       15 2024-05-21 16:25:50.000000 mqtt_automator-0.0.4/mqtt_automator.egg-info/top_level.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1258 2024-05-21 16:24:49.000000 mqtt_automator-0.0.4/pyproject.toml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2024-05-21 16:25:50.453487 mqtt_automator-0.0.4/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-21 16:25:50.449487 mqtt_automator-0.0.4/tests/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2523 2024-05-21 16:24:49.000000 mqtt_automator-0.0.4/tests/test_config_parser.py
```

### Comparing `mqtt_automator-0.0.3/LICENSE` & `mqtt_automator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.3/PKG-INFO` & `mqtt_automator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-automator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple smart-home automation system. Self-hosted, LAN only. Supports Vakio Lytko and Yeelink.
 Author-email: Oleg Strizhechenko <oleg.strizhechenko@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mqtt_automator-0.0.3/README.md` & `mqtt_automator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.3/mqtt_automator/automator.py` & `mqtt_automator-0.0.4/mqtt_automator/automator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             for device, name, rule in self.config.get_active_rules():
                 client: base.BaseClient = self.devices[device]
                 await self.apply_actions(client, device, name, rule.get('action', noop))
                 for sub_name, sub_rule in self.config.get_active_sub_rules(rule.get('sub_rules', noop)):
                     await self.apply_actions(client, device, sub_name, sub_rule['action'])
 
             until_start_of_next_minute = 60 - datetime.now().time().second
+            log.debug("Sleep for %d seconds until start of next minute", until_start_of_next_minute)
             await asyncio.sleep(until_start_of_next_minute)
 
     @staticmethod
     async def apply_actions(client, device, name, actions: dict):
         for sub_topic, payload in actions.items():
             log.debug('Applying %s %s %s %s', device, name, sub_topic, payload)
             await client.publish(sub_topic, payload)
```

### Comparing `mqtt_automator-0.0.3/mqtt_automator/config/parser.py` & `mqtt_automator-0.0.4/mqtt_automator/config/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         """
         for vendor, devices in self.config.items():
             if vendor in self.system_keys:
                 continue
             for device_name, device in devices.items():
                 if device_name == 'common':
                     continue
-                yield Device(vendor=vendor, name=device_name, id=device.get('device', device_name))
+                device_id = device.pop('device', device_name)
+                yield Device(vendor=vendor, name=device_name, id=device_id, **device)
 
     def get_active_rules(self):
         """For rule structure see class Rule"""
         now = datetime.now()
         is_workday, now_time = now.isoweekday() <= 5, now.time()
         for vendor, devices in self.config.items():
             if vendor in self.system_keys:
@@ -121,16 +122,18 @@
 
             for device, rules in devices.items():
                 if device == 'common':
                     continue
 
                 log.debug('Looking for device %s', device)
                 for name, rule_ in (rules | common).items():
-                    if name == 'device':
+                    if name in ('device', 'parent'):
                         continue
+                    if not isinstance(rule_, dict):
+                        log.error("Bad rule %s %s %s", device, name, rule_)
                     rule = Rule(**rule_)
                     schedule = (rule.workday if is_workday else rule.weekend) or rule.time
                     log.debug('Checking rule %s schedule %s', name, schedule)
                     if schedule and match_time_range(schedule, now_time):
                         log.debug('rule %s schedule %s matched! yielding %s', name, schedule, rule)
                         yield device, name, rule.model_dump(exclude_unset=True)
```

### Comparing `mqtt_automator-0.0.3/mqtt_automator/config/time_parser.py` & `mqtt_automator-0.0.4/mqtt_automator/config/time_parser.py`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.3/mqtt_automator/devices/base.py` & `mqtt_automator-0.0.4/mqtt_automator/devices/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import abc
 import logging
 from datetime import datetime, timedelta
-from typing import Generator
+from typing import Generator, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from mqtt_automator.broker import Broker
 
 CLIENT_BLOCK_SECONDS = timedelta(hours=4).seconds
 
 log = logging.getLogger(__name__)
 
 
 class Device(BaseModel):
     vendor: str
     id: str
     name: str
+    parent: Optional[str] = Field(default=None)
 
 
 class BaseClient(abc.ABC):
     topic_template: str
 
     def __init__(self, device: Device, broker: Broker = None):
         self.broker = broker
```

### Comparing `mqtt_automator-0.0.3/mqtt_automator/devices/lytko.py` & `mqtt_automator-0.0.4/mqtt_automator/devices/lytko.py`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.3/mqtt_automator/devices/vakio.py` & `mqtt_automator-0.0.4/mqtt_automator/devices/vakio.py`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.3/mqtt_automator.egg-info/PKG-INFO` & `mqtt_automator-0.0.4/mqtt_automator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-automator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple smart-home automation system. Self-hosted, LAN only. Supports Vakio Lytko and Yeelink.
 Author-email: Oleg Strizhechenko <oleg.strizhechenko@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mqtt_automator-0.0.3/mqtt_automator.egg-info/SOURCES.txt` & `mqtt_automator-0.0.4/mqtt_automator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.3/pyproject.toml` & `mqtt_automator-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = 'mqtt-automator'
 authors = [
     {name = 'Oleg Strizhechenko', email = 'oleg.strizhechenko@gmail.com'},
 ]
-version = 'v0.0.3'
+version = 'v0.0.4'
 readme = 'README.md'
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 keywords = ["mqtt", "aiomqtt", "vakio", "lytko", "yeelink", "self-hosted"]
 description = 'Simple smart-home automation system. Self-hosted, LAN only. Supports Vakio Lytko and Yeelink.'
 dependencies = [
     'PyYAML ~= 6.0.1',
```

### Comparing `mqtt_automator-0.0.3/tests/test_config_parser.py` & `mqtt_automator-0.0.4/tests/test_config_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,40 +22,40 @@
 def test_config_example(config):
     assert config.broker.ip == '192.168.1.120'
     assert config.broker.protocol == 5
     assert list(config.get_devices()) == [
         Device(vendor='vakio', id='cabinet', name='cabinet'),
         Device(vendor='vakio', id='restroom', name='restroom'),
         Device(vendor='lytko', id='12345', name='floor'),
-        Device(vendor='yeelink', id='192.168.1.121', name='light1'),
+        Device(vendor='yeelink', id='192.168.1.121', name='light1', parent='192.168.1.123'),
         Device(vendor='yeelink', id='192.168.1.122', name='light2'),
     ]
 
 
 @pytest.mark.parametrize('time_to_freeze', ('2024-05-17 20:00', '2024-05-18 20:15'))
 def test_get_active_rules_evening(config, time_to_freeze):
     """ Difference between workday and weekday is located at sub-rules level"""
     with freezegun.freeze_time(time_to_freeze):
         assert list(config.get_active_rules()) == [
             ('cabinet', 'day', {'workday': '18:00-22:29', 'weekend': '09:30-22:29', 'action': {'speed': 3}}),
             ('restroom', 'before_sleep', {'time': '20:00-21:59', 'action': {'state': True, 'speed': 3}}),
             ('floor', 'day', {'time': '12:00-20:29', 'action': {'mode': True, 'temperature': 18}}),
-            ('light1', 'evening', {'time': '19:00-22:59', 'action': {'set_power': True}}),
-            ('light2', 'evening', {'time': '19:00-22:59', 'action': {'set_power': True}})
+            ('light1', 'evening', {'time': '19:00-22:59', 'action': {'set_power': 'icmp'}}),
+            ('light2', 'evening', {'time': '19:00-22:59', 'action': {'set_power': 'icmp'}})
         ]
 
 
+@freezegun.freeze_time('2024-05-17 14:58')
 def test_get_active_sub_rules_at_work(config):
     """ Difference between workday and weekday is located at sub-rules level"""
-    with freezegun.freeze_time('2024-05-17 14:58'):
-        cabinet = next(config.get_active_rules())
-        assert cabinet == ('cabinet', 'at_work', {
-                'workday': '09:15-18:00',
-                'sub_rules': {
-                    'before_meetings': {'hours': '11-15', 'minutes': '55-59', 'action': {'speed': 7}},
-                    'meetings': {'hours': '12-15', 'minutes': '0-15', 'action': {'speed': 1}},
-                    'fallback': {'action': {'speed': 3}}
-                }
-        })
-        assert list(config.get_active_sub_rules(cabinet[2]['sub_rules'])) == [
-            ('before_meetings', {'hours': '11-15', 'minutes': '55-59', 'action': {'speed': 7}})
-        ]
+    cabinet = next(config.get_active_rules())
+    assert cabinet == ('cabinet', 'at_work', {
+            'workday': '09:15-18:00',
+            'sub_rules': {
+                'before_meetings': {'hours': '11-15', 'minutes': '55-59', 'action': {'speed': 7}},
+                'meetings': {'hours': '12-15', 'minutes': '0-15', 'action': {'speed': 1}},
+                'fallback': {'action': {'speed': 3}}
+            }
+    })
+    assert list(config.get_active_sub_rules(cabinet[2]['sub_rules'])) == [
+        ('before_meetings', {'hours': '11-15', 'minutes': '55-59', 'action': {'speed': 7}})
+    ]
```

