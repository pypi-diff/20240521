# Comparing `tmp/dsf-python-3.5.0rc2.tar.gz` & `tmp/dsf_python-3.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsf-python-3.5.0rc2.tar", last modified: Mon Jan 15 18:24:29 2024, max compression
+gzip compressed data, was "dsf_python-3.5.1rc1.tar", last modified: Mon May  6 17:55:42 2024, max compression
```

## Comparing `dsf-python-3.5.0rc2.tar` & `dsf_python-3.5.1rc1.tar`

### file list

```diff
@@ -1,224 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.688521 dsf-python-3.5.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-01-15 18:24:29.688521 dsf-python-3.5.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-15 18:24:29.688521 dsf-python-3.5.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.652520 dsf-python-3.5.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.652520 dsf-python-3.5.0rc2/src/dsf/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.656520 dsf-python-3.5.0rc2/src/dsf/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/base_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/code_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/code_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/code_interception.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/code_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/http_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/model_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/object_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/commands/user_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.656520 dsf-python-3.5.0rc2/src/dsf/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/base_command_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/command_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.660520 dsf-python-3.5.0rc2/src/dsf/connections/init_messages/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/init_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/init_messages/client_init_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/init_messages/server_init_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/intercept_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/connections/subscribe_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.660520 dsf-python-3.5.0rc2/src/dsf/object_model/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.660520 dsf-python-3.5.0rc2/src/dsf/object_model/boards/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/accelerometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/board_closed_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/boards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.660520 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_screen_st7567.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/driver_closed_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/boards/min_max_current.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.660520 dsf-python-3.5.0rc2/src/dsf/object_model/directories/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/directories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/directories/directories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.664520 dsf-python-3.5.0rc2/src/dsf/object_model/fans/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/fans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/fans/fan_thermostatic_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/fans/fans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.664520 dsf-python-3.5.0rc2/src/dsf/object_model/heat/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/heat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/heat/heat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater_model_pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.664520 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/input_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/input_channel_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/inputs/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.668520 dsf-python-3.5.0rc2/src/dsf/object_model/job/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/build_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/gcode_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/thumbnail_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/job/times_left.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.668520 dsf-python-3.5.0rc2/src/dsf/object_model/led_strips/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/led_strips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/led_strips/led_strip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.668520 dsf-python-3.5.0rc2/src/dsf/object_model/limits/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/limits/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.668520 dsf-python-3.5.0rc2/src/dsf/object_model/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/messages/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/model_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/model_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/model_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.672520 dsf-python-3.5.0rc2/src/dsf/object_model/move/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/current_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/driver_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/extruder.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/extruder_non_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/input_shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/keepout_zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.672520 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/core_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/delta_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/delta_tower.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/hangprinter_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/kinematics_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/polar_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/scara_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/tilt_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/zleadscrew_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/microstepping.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/motors_idle_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move_compensation.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move_deviations.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move_queue_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/move_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/probe_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/move/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.676520 dsf-python-3.5.0rc2/src/dsf/object_model/network/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/network/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/network/network_interface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/network/network_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/network/network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/object_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.676520 dsf-python-3.5.0rc2/src/dsf/object_model/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/plugins/plugin_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/plugins/sbc_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.676520 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.676520 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/dsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/http_endpoint_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.676520 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/user_sessions/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/user_sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/user_sessions/access_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/user_sessions/session_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/user_sessions/user_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sbc/sbc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.680520 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/analog_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/analog_sensor_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/endstop.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/endstop_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.680520 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/Duet3DFilamentMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/filament_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/filament_monitor_enable_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/filament_monitor_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/filament_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/laser_filament_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/pulsed_filament_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/rotating_magnet_filament_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/gp_input_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/probe_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/sensors/temperature_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.680520 dsf-python-3.5.0rc2/src/dsf/object_model/spindles/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/spindles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/spindles/spindle_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/spindles/spindles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.684520 dsf-python-3.5.0rc2/src/dsf/object_model/state/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/beep_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/gp_output_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/log_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/machine_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/machine_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/message_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/restore_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/startup_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.684520 dsf-python-3.5.0rc2/src/dsf/object_model/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/tools/tool_retraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/tools/tool_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.684520 dsf-python-3.5.0rc2/src/dsf/object_model/volumes/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/object_model/volumes/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.684520 dsf-python-3.5.0rc2/src/dsf/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/src/dsf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.688521 dsf-python-3.5.0rc2/src/dsf_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-01-15 18:24:29.000000 dsf-python-3.5.0rc2/src/dsf_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-01-15 18:24:29.000000 dsf-python-3.5.0rc2/src/dsf_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 18:24:29.000000 dsf-python-3.5.0rc2/src/dsf_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-15 18:24:29.000000 dsf-python-3.5.0rc2/src/dsf_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-15 18:24:29.000000 dsf-python-3.5.0rc2/src/dsf_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:24:29.688521 dsf-python-3.5.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/tests/test_custom_http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/tests/test_custom_m_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17482 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/tests/test_send_simple_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-15 18:24:22.000000 dsf-python-3.5.0rc2/tests/test_subscribe_object_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.612588 dsf_python-3.5.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-06 17:55:42.612588 dsf_python-3.5.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 17:55:42.612588 dsf_python-3.5.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.580587 dsf_python-3.5.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.584588 dsf_python-3.5.1rc1/src/dsf/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.588588 dsf_python-3.5.1rc1/src/dsf/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/code_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/code_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/code_interception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/code_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/http_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/model_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/object_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/commands/user_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.588588 dsf_python-3.5.1rc1/src/dsf/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/base_command_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/command_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.588588 dsf_python-3.5.1rc1/src/dsf/connections/init_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/init_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/init_messages/client_init_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/init_messages/server_init_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/intercept_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/connections/subscribe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.588588 dsf_python-3.5.1rc1/src/dsf/object_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.592588 dsf_python-3.5.1rc1/src/dsf/object_model/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/accelerometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/board_closed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/boards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.592588 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_screen_st7567.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/driver_closed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/inductive_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/boards/min_max_current.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.592588 dsf_python-3.5.1rc1/src/dsf/object_model/directories/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/directories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/directories/directories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.592588 dsf_python-3.5.1rc1/src/dsf/object_model/fans/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/fans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/fans/fan_thermostatic_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/fans/fans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.592588 dsf_python-3.5.1rc1/src/dsf/object_model/heat/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/heat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/heat/heat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater_model_pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.592588 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/input_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/input_channel_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/inputs/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.596588 dsf_python-3.5.1rc1/src/dsf/object_model/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/build_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/gcode_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/thumbnail_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/job/times_left.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.596588 dsf_python-3.5.1rc1/src/dsf/object_model/led_strips/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/led_strips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/led_strips/led_strip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.596588 dsf_python-3.5.1rc1/src/dsf/object_model/limits/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/limits/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.596588 dsf_python-3.5.1rc1/src/dsf/object_model/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/messages/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/model_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/model_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/model_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.600587 dsf_python-3.5.1rc1/src/dsf/object_model/move/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/current_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/driver_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/extruder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/extruder_non_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/input_shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/keepout_zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.600587 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/core_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/delta_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/delta_tower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/hangprinter_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/kinematics_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/polar_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/scara_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/tilt_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/zleadscrew_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/microstepping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/motors_idle_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move_compensation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move_deviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move_queue_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/move_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/probe_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/move/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.600587 dsf_python-3.5.1rc1/src/dsf/object_model/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/network/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/network/network_interface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/network/network_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/network/network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/object_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.600587 dsf_python-3.5.1rc1/src/dsf/object_model/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/plugins/plugin_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/plugins/sbc_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.604587 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.604587 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/dsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/http_endpoint_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.604587 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/user_sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/user_sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/user_sessions/access_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/user_sessions/session_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/user_sessions/user_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sbc/sbc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.604587 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/analog_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/analog_sensor_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/endstop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/endstop_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.608588 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/Duet3DFilamentMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/filament_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/filament_monitor_enable_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/filament_monitor_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/filament_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/laser_filament_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/pulsed_filament_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/rotating_magnet_filament_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/gp_input_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/probe_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/sensors/temperature_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.608588 dsf_python-3.5.1rc1/src/dsf/object_model/spindles/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/spindles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/spindles/spindle_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/spindles/spindles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.608588 dsf_python-3.5.1rc1/src/dsf/object_model/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/beep_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/gp_output_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/log_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/machine_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/machine_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/message_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/restore_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/startup_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.608588 dsf_python-3.5.1rc1/src/dsf/object_model/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/tools/tool_retraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/tools/tool_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.608588 dsf_python-3.5.1rc1/src/dsf/object_model/volumes/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/object_model/volumes/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.608588 dsf_python-3.5.1rc1/src/dsf/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/src/dsf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.612588 dsf_python-3.5.1rc1/src/dsf_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-06 17:55:42.000000 dsf_python-3.5.1rc1/src/dsf_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-06 17:55:42.000000 dsf_python-3.5.1rc1/src/dsf_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:55:42.000000 dsf_python-3.5.1rc1/src/dsf_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 17:55:42.000000 dsf_python-3.5.1rc1/src/dsf_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 17:55:42.000000 dsf_python-3.5.1rc1/src/dsf_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:55:42.612588 dsf_python-3.5.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/tests/test_custom_http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/tests/test_custom_m_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/tests/test_send_simple_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 17:55:38.000000 dsf_python-3.5.1rc1/tests/test_subscribe_object_model.py
```

### Comparing `dsf-python-3.5.0rc2/LICENSE` & `dsf_python-3.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/PKG-INFO` & `dsf_python-3.5.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: dsf-python
-Version: 3.5.0rc2
+Version: 3.5.1rc1
 Summary: Python interface to access DuetSoftwareFramework
 Home-page: https://github.com/Duet3D/dsf-python
 Author: Duet3D Ltd.
 Author-email: pkg@duet3d.com
 Project-URL: Duet3D Support, https://forum.duet3d.com/
 Project-URL: Bug Reports, https://github.com/Duet3D/dsf-python/issues
 Project-URL: Source, https://github.com/Duet3D/dsf-python/
 Keywords: Duet3D,DuetSoftwareFramework,DSF,dsf-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Provides-Extra: dev
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: tox; extra == "dev"
```

### Comparing `dsf-python-3.5.0rc2/README.md` & `dsf_python-3.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/setup.py` & `dsf_python-3.5.1rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 
 import setuptools
 
 long_description = open("README.md", encoding="utf-8").read()
 
 setuptools.setup(
     name="dsf-python",
-    version="3.5.0rc2",
+    version="3.5.1rc1",
     description="Python interface to access DuetSoftwareFramework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Duet3D/dsf-python",
     author="Duet3D Ltd.",
     author_email="pkg@duet3d.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
     ],
     install_requires=[
         'python-dateutil'
     ],
     keywords="Duet3D, DuetSoftwareFramework, DSF, dsf-python",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.9, <4",
+    python_requires=">=3.7, <4",
     extras_require={
         "dev": [
             "sphinx",
             "tox",
         ],
     },
     project_urls={
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/code.py` & `dsf_python-3.5.1rc1/src/dsf/commands/code.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/code_channel.py` & `dsf_python-3.5.1rc1/src/dsf/commands/code_channel.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/code_flags.py` & `dsf_python-3.5.1rc1/src/dsf/commands/code_flags.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/code_interception.py` & `dsf_python-3.5.1rc1/src/dsf/commands/code_interception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Optional
 
 from .base_command import BaseCommand
 from ..object_model.messages import MessageType
 
 
 def cancel():
     """Cancel a code in Connection.InterceptionMode."""
@@ -13,15 +13,15 @@
     """
     Ignore the code to intercept and allow it to be processed without any modifications.
     This command is only permitted in ConnectionMode.Intercept mode.
     """
     return BaseCommand("Ignore")
 
 
-def resolve_code(rtype: MessageType, content: str | None = None):
+def resolve_code(rtype: MessageType, content: Optional[str]):
     """
     Resolve the code to intercept and return the given message details for its completion.
     This command is only permitted in ConnectionMode.Intercept mode.
     :param rtype: Type of the resolving message
     :param content: Content of the resolving message
     """
     if not isinstance(rtype, MessageType):
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/code_parameter.py` & `dsf_python-3.5.1rc1/src/dsf/commands/code_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 codeparameter contains all classes and methods dealing with deserialized code parameters.
 """
-from __future__ import annotations
 import json
 
 from ..exceptions import CodeParserException
 from ..object_model.move.driver_id import DriverId
 
 
 class CodeParameter(json.JSONEncoder):
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/condition_type.py` & `dsf_python-3.5.1rc1/src/dsf/commands/condition_type.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/files.py` & `dsf_python-3.5.1rc1/src/dsf/commands/files.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/generic.py` & `dsf_python-3.5.1rc1/src/dsf/commands/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Optional
 
 from .base_command import BaseCommand
 from .code_channel import CodeChannel
 from ..object_model.state.log_level import LogLevel
 from ..object_model.messages import MessageType
 
 
@@ -104,15 +104,15 @@
     return BaseCommand("SimpleCode", **{"Code": code, "Channel": channel, "ExecuteAsynchronously": async_exec})
 
 
 def write_message(
     message_type: MessageType,
     content: str,
     output_message: bool = True,
-    log_level: LogLevel | None = None,
+    log_level: Optional[LogLevel] = None,
 ):
     """
     Write an arbitrary generic message
 
     :param message_type: Type of the message to write
     :param content: Content of the message to write
     :param output_message: Output the message on the console and via the object model
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/http_endpoints.py` & `dsf_python-3.5.1rc1/src/dsf/commands/http_endpoints.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/object_model.py` & `dsf_python-3.5.1rc1/src/dsf/commands/object_model.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/packages.py` & `dsf_python-3.5.1rc1/src/dsf/commands/packages.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/plugins.py` & `dsf_python-3.5.1rc1/src/dsf/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/responses.py` & `dsf_python-3.5.1rc1/src/dsf/commands/responses.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/commands/user_sessions.py` & `dsf_python-3.5.1rc1/src/dsf/commands/user_sessions.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/connections/__init__.py` & `dsf_python-3.5.1rc1/src/dsf/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/connections/base_command_connection.py` & `dsf_python-3.5.1rc1/src/dsf/connections/base_command_connection.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/connections/base_connection.py` & `dsf_python-3.5.1rc1/src/dsf/connections/base_connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-from __future__ import annotations
 import json
 import socket
+from typing import Optional
 
-from .exceptions import (IncompatibleVersionException, InternalServerException, IPCSocketBrokenException,
-                         TaskCanceledException)
+from .exceptions import IncompatibleVersionException, InternalServerException, TaskCanceledException
 from .init_messages import client_init_messages, server_init_message
 from ..commands import responses
 
 
 class BaseConnection:
     """
     Base class for connections that access the control server via the Duet API
     using a UNIX socket
-
-    Constructor arguments:
-    :param debug: Whether to print debug information or not
-    :param timeout: Set a timeout value on blocking socket operations or None to set the socket in non-blocking mode
     """
 
-    def __init__(self, debug: bool = False, timeout: int = None):
+    def __init__(self, debug: bool = False, timeout: int = 3):
         self.debug = debug
         self.timeout = timeout
-        self.socket: socket.socket | None = None
+        self.socket: Optional[socket.socket] = None
         self.id = None
         self.input = ""
 
     def connect(self, init_message: client_init_messages.ClientInitMessage, socket_file: str):
         """Establishes a connection to the given UNIX socket file"""
 
         self.socket = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         self.socket.connect(socket_file)
-        self.socket.settimeout(self.timeout)
+        self.socket.setblocking(True)
         server_init_msg = server_init_message.ServerInitMessage.from_json(
             json.loads(self.socket.recv(50).decode("utf8"))
         )
         if not server_init_msg.is_compatible():
             raise IncompatibleVersionException(
                 f"Incompatible API version (need {server_init_msg.PROTOCOL_VERSION}, got {server_init_msg.version})"
             )
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/connections/init_messages/client_init_messages.py` & `dsf_python-3.5.1rc1/src/dsf/connections/init_messages/client_init_messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-from __future__ import annotations
+from typing import List
 from .server_init_message import ServerInitMessage
 from .. import ConnectionMode, InterceptionMode, SubscriptionMode
 from ...commands.code_channel import CodeChannel
 
 
 class ClientInitMessage:
     """
@@ -34,18 +34,19 @@
         self.version = ServerInitMessage.PROTOCOL_VERSION
         for key, value in kwargs.items():
             self.__dict__[key] = value
 
 
 def intercept_init_message(
         intercept_mode: InterceptionMode,
-        channels: list[CodeChannel],
-        filters: list[str],
+        channels: List[CodeChannel],
+        filters: List[str],
         priority_codes: bool,
-        auto_flush: bool = True):
+        auto_flush: bool = True,
+        auto_evaluate_expression: bool = True):
     """
     Enter interception mode
     Whenever a code is received, the connection must respond with one of
     - `Cancel` to cancel the code
     - `Ignore` to pass through the code without modifications
     - `Resolve` to resolve the current code and to return a message
     In addition the interceptor may issue custom commands once a code has been received
@@ -58,23 +59,27 @@
     Alternatively keyword types may be specified (e.g. if or elif).
     Asterisks are supported, too (e.g. T*)
     :param priority_codes: Defines if either regular or priority codes are supposed to be intercepted
     :param auto_flush: Automatically flush the code channel before notifying the client in case a code filter
     is specified.
     This option makes extra Flush calls in the interceptor implementation obsolete.
     It is highly recommended to enable this in order to avoid potential deadlocks when dealing with macros!
+    :param auto_evaluate_expression: Automatically evaluate expression parameters to their final values
+    before sending it over to the client.
+    This requires auto_flush to be True and happens when the remaining codes have been processed.
     """
     return ClientInitMessage(
         ConnectionMode.INTERCEPT,
         **{
             "InterceptionMode": intercept_mode,
             "Channels": channels,
             "AutoFlush": auto_flush,
+            "AutoEvaluateExpressions": auto_evaluate_expression,
             "Filters": filters,
-            "PriortyCodes": priority_codes,
+            "PriorityCodes": priority_codes,
         },
     )
 
 
 def command_init_message():
     """Enter command-based connection mode"""
     return ClientInitMessage(ConnectionMode.COMMAND)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/connections/init_messages/server_init_message.py` & `dsf_python-3.5.1rc1/src/dsf/connections/init_messages/server_init_message.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/connections/subscribe_connection.py` & `dsf_python-3.5.1rc1/src/dsf/connections/subscribe_connection.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/http.py` & `dsf_python-3.5.1rc1/src/dsf/http.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/__init__.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/__init__.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/__init__.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/board_closed_loop.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/board_closed_loop.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/boards.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/boards.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import annotations
 from enum import Enum
-from typing import List, Union
+from typing import List, Optional
 
 from .accelerometer import Accelerometer
 from .board_closed_loop import BoardClosedLoop
 from .direct_display import DirectDisplay
 from .driver import Driver
+from .inductive_sensor import InductiveSensor
 from .min_max_current import MinMaxCurrent
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 from ..utils import wrap_model_property
 from ...utils import deprecated
 
 
@@ -39,14 +39,16 @@
 
     # Accelerometer of this board or None if unknown
     accelerometer = wrap_model_property('accelerometer', Accelerometer)
     # Closed loop data of this board or None if unknown
     closed_loop = wrap_model_property('closed_loop', BoardClosedLoop)
     # Details about a connected display or None if none is connected
     direct_display = wrap_model_property('direct_display', DirectDisplay)
+    # Information about an inductive sensor or None if not present
+    inductive_sensor = wrap_model_property('inductive_sensor', InductiveSensor)
     # Minimum, maximum, and current temperatures of the MCU or None if unknown
     mcu_temp = wrap_model_property('mcu_temp', MinMaxCurrent)
     # Minimum, maximum, and current voltages on the 12V rail or None if unknown
     v_12 = wrap_model_property('v_12', MinMaxCurrent)
     # Minimum, maximum, and current voltages on the input rail or None if unknown
     v_in = wrap_model_property('v_in', MinMaxCurrent)
 
@@ -69,19 +71,23 @@
         self._firmware_date = ""
         # Filename of the firmware binary
         self._firmware_file_name = ""
         # Name of the firmware build
         self._firmware_name = ""
         # Version of the firmware build
         self._firmware_version = ""
+        # Amount of free RAM on this board (in bytes or null if unknown)
+        self._free_ram = None
         # Filename of the IAP binary that is used for updates from the SBC or None if unsupported
         self._iap_file_name_SBC = None
         # Filename of the IAP binary that is used for updates from the SD card or None if unsupported
         # This is only available for the mainboard (first board item)
         self._iap_file_name_SD = None
+        # Information about an inductive sensor or None if not present
+        self._inductive_sensor = None
         # Maximum number of heaters this board can control
         self._max_heaters = 0
         # Maximum number of motors this board can drive
         self._max_motors = 0
         # Minimum, maximum, and current temperatures of the MCU or None if unknown
         self._mcu_temp = None
         # Full name of the board
@@ -101,33 +107,33 @@
         self._v_12 = None
         # Minimum, maximum, and current voltages on the input rail or None if unknown
         self._v_in = None
         # Filename of the on-board WiFi chip or None if not present
         self._wifi_firmware_file_name = None
 
     @property
-    def bootloader_file_name(self) -> Union[str, None]:
+    def bootloader_file_name(self) -> Optional[str]:
         """Filename of the bootloader binary or None if unknown"""
         return self._bootloader_file_name
 
     @bootloader_file_name.setter
-    def bootloader_file_name(self, value: str | None = None):
+    def bootloader_file_name(self, value):
         self._bootloader_file_name = str(value) if value is not None else None
 
     @property
-    def can_address(self) -> Union[int, None]:
+    def can_address(self) -> Optional[int]:
         """CAN address of this board or None if not applicable"""
         return self._can_address
 
     @can_address.setter
-    def can_address(self, value: int | None = None):
+    def can_address(self, value):
         self._can_address = int(value) if value is not None else None
 
     @property
-    def drivers(self) -> Union[List[Driver], None]:
+    def drivers(self) -> Optional[List[Driver]]:
         """Drivers of this board"""
         return self._drivers
 
     @drivers.setter
     def drivers(self, value):
         self._drivers = None if value is None else ModelCollection(Driver, value)
 
@@ -164,30 +170,39 @@
         return self._firmware_version
 
     @firmware_version.setter
     def firmware_version(self, value):
         self._firmware_version = str(value)
 
     @property
-    def iap_file_name_SBC(self) -> Union[str, None]:
+    def free_ram(self) -> Optional[int]:
+        """Amount of free RAM on this board (in bytes or null if unknown)"""
+        return self._free_ram
+
+    @free_ram.setter
+    def free_ram(self, value):
+        self._free_ram = None if value is None else int(value)
+
+    @property
+    def iap_file_name_SBC(self) -> Optional[str]:
         """Filename of the IAP binary that is used for updates from the SBC or None if unsupported"""
         return self._iap_file_name_SBC
 
     @iap_file_name_SBC.setter
-    def iap_file_name_SBC(self, value: str | None = None):
+    def iap_file_name_SBC(self, value):
         self._iap_file_name_SBC = str(value) if value is not None else None
 
     @property
-    def iap_file_name_SD(self) -> Union[str, None]:
+    def iap_file_name_SD(self) -> Optional[str]:
         """Filename of the IAP binary that is used for updates from the SD card or None if unsupported
         This is only available for the mainboard (first board item)"""
         return self._iap_file_name_SD
 
     @iap_file_name_SD.setter
-    def iap_file_name_SD(self, value: str | None = None):
+    def iap_file_name_SD(self, value):
         self._iap_file_name_SD = str(value) if value is not None else None
 
     @property
     def max_heaters(self) -> int:
         """Maximum number of heaters this board can drive"""
         return self._max_heaters
 
@@ -224,50 +239,49 @@
 
     @property
     def state(self) -> BoardState:
         """State of this board"""
         return self._state
 
     @state.setter
-    def state(self, value: BoardState):
-        if isinstance(value, BoardState):
+    def state(self, value):
+        if value is None or isinstance(value, BoardState):
             self._state = value
         elif isinstance(value, str):
             self._state = BoardState(value)
         else:
-            raise TypeError(f"{__name__}.state must be of type BoardState."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.state must be of type BoardState or None. Got {type(value)}: {value}")
 
     @property
     @deprecated(f"Use {__name__}.supports_direct_display instead")
     def supports_12864(self) -> bool:
         """Indicates if this board supports external 12864 displays
         Deprecated: Use supports_direct_display instead"""
         return self._supports_12864
 
     @supports_12864.setter
-    def supports_12864(self, value: bool):
+    def supports_12864(self, value):
         self._supports_12864 = bool(value)
 
     @property
     def supports_direct_display(self) -> bool:
         """Indicates if this board supports external displays"""
         return self._supports_direct_display
 
     @supports_direct_display.setter
-    def supports_direct_display(self, value: bool):
+    def supports_direct_display(self, value):
         self._supports_direct_display = bool(value)
 
     @property
-    def unique_id(self) -> Union[str, None]:
+    def unique_id(self) -> Optional[str]:
         """Unique identifier of the board or None if unknown"""
         return self._unique_id
 
     @unique_id.setter
-    def unique_id(self, value: str | None = None):
+    def unique_id(self, value):
         self._unique_id = str(value) if value is not None else None
 
     @property
     def wifi_firmware_file_name(self):
         """Filename of the on-board WiFi chip or None if not present"""
         return self._wifi_firmware_file_name
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_encoder.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_encoder.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_screen.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_screen.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/direct_display/direct_display_screen_st7567.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/direct_display/direct_display_screen_st7567.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/driver.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/driver.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/driver_closed_loop.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/driver_closed_loop.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/boards/min_max_current.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/boards/min_max_current.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/directories/directories.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/directories/directories.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,64 +23,64 @@
 
     @property
     def filaments(self) -> str:
         """Path to the filaments directory"""
         return self._filaments
 
     @filaments.setter
-    def filaments(self, value: str):
+    def filaments(self, value):
         self._filaments = str(value)
 
     @property
     def firmware(self) -> str:
         """Path to the firmware directory"""
         return self._firmware
 
     @firmware.setter
-    def firmware(self, value: str):
+    def firmware(self, value):
         self._firmware = str(value)
 
     @property
     def g_codes(self) -> str:
         """Path to the G-Codes directory"""
         return self._g_codes
 
     @g_codes.setter
-    def g_codes(self, value: str):
+    def g_codes(self, value):
         self._g_codes = str(value)
 
     @property
     def macros(self) -> str:
         """Path to the macros directory"""
         return self._macros
 
     @macros.setter
-    def macros(self, value: str):
+    def macros(self, value):
         self._macros = str(value)
 
     @property
     def menu(self) -> str:
         """Path to the menu directory
         Intended for 12864 displays but currently unused in DSF. It is only needed for the Duet Maestro > DWC"""
         return self._menu
 
     @menu.setter
-    def menu(self, value: str):
+    def menu(self, value):
         self._menu = str(value)
 
     @property
     def system(self) -> str:
         """Path to the system directory"""
         return self._system
 
     @system.setter
-    def system(self, value: str):
+    def system(self, value):
         self._system = str(value)
 
     @property
     def web(self) -> str:
         """Path to the web directory"""
         return self._web
 
     @web.setter
-    def web(self, value: str):
+    def web(self, value):
         self._web = str(value)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/fans/fan_thermostatic_control.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/cpu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-from __future__ import annotations
+from typing import Union
+
 from ..model_object import ModelObject
-from ...utils import deprecated
 
 
-class FanThermostaticControl(ModelObject):
-    """Thermostatic parameters of a fan"""
+class CPU(ModelObject):
+    """Information about the SBC's CPU"""
+
     def __init__(self):
         super().__init__()
-        # List of the heaters to monitor (indices)
-        self._heaters = []
-        # Upper temperature range required to turn on the fan (in C)
-        self._high_temperature = None
-        # Lower temperature range required to turn on the fan (in C)
-        self._low_temperature = None
-        # List of sensors to monitor (indices)
-        self._sensors = []
+        self._avg_load = None
+        self._hardware = None
+        self._num_cores = 1
+        self._temperature = None
 
     @property
-    @deprecated(f"Use {__name__}.sensors instead")
-    def heaters(self) -> List[int]:
-        """List of the heaters to monitor (indices)
-        Deprecated: Use sensors instead"""
-        return self._heaters
+    def avg_load(self) -> Union[float, None]:
+        """Average CPU load (0..100%) or None if unknown"""
+        return self._avg_load
+
+    @avg_load.setter
+    def avg_load(self, value):
+        self._avg_load = float(value) if value is not None else None
 
     @property
-    def high_temperature(self) -> float | None:
-        """Upper temperature range required to turn on the fan (in C)"""
-        return self._high_temperature
-
-    @high_temperature.setter
-    def high_temperature(self, value: float | None = None):
-        self._high_temperature = float(value) if value is not None else None
+    def hardware(self) -> Union[str, None]:
+        """CPU hardware as reported by /proc/cpuinfo"""
+        return self._hardware
+
+    @hardware.setter
+    def hardware(self, value):
+        self._hardware = str(value) if value is not None else None
 
     @property
-    def low_temperature(self) -> float | None:
-        """Lower temperature range required to turn on the fan (in C)"""
-        return self._low_temperature
-
-    @low_temperature.setter
-    def low_temperature(self, value: float | None = None):
-        self._low_temperature = float(value) if value is not None else None
+    def num_cores(self) -> int:
+        """Number of CPU cores/threads (defaults to 1)"""
+        return self._num_cores
+
+    @num_cores.setter
+    def num_cores(self, value):
+        self._num_cores = int(value)
 
     @property
-    def sensors(self) -> List[int]:
-        """List of sensors to monitor (indices)"""
-        return self._sensors
+    def temperature(self) -> Union[float, None]:
+        """Current CPU temperature (in degC) or None if unknown"""
+        return self._temperature
+
+    @temperature.setter
+    def temperature(self, value):
+        self._temperature = float(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/fans/fans.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/fans/fans.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         self._min = 0
         # Name of the fan
         self._name = ""
         # Requested value for this fan on a scale between 0 and 1
         self._requested_value = 0
         # Current RPM of this fan or -1 if unknown/unset
         self._rpm = -1
+        # Pulses per tacho revolution
+        self._tacho_ppr = 2.0
         # Thermostatic control parameters
         self._thermostatic = FanThermostaticControl()
 
     @property
     def actual_value(self) -> float:
         """Value of this fan (0..1 or -1 if unknown)"""
         return self._actual_value
@@ -74,15 +76,15 @@
 
     @property
     def name(self) -> str:
         """Name of the fan"""
         return self._name
 
     @name.setter
-    def name(self, value: str):
+    def name(self, value):
         self._name = str(value)
 
     @property
     def requested_value(self) -> float:
         """Requested value for this fan on a scale between 0 and 1"""
         return self._requested_value
 
@@ -96,10 +98,19 @@
         return self._rpm
 
     @rpm.setter
     def rpm(self, value):
         self._rpm = int(value)
 
     @property
+    def tacho_ppr(self) -> float:
+        """Pulses per tacho revolution"""
+        return self._tacho_ppr
+
+    @tacho_ppr.setter
+    def tacho_ppr(self, value):
+        self._tacho_ppr = float(value)
+
+    @property
     def thermostatic(self) -> FanThermostaticControl:
         """Thermostatic control parameters"""
         return self._thermostatic
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/heat/heat.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/heat/heat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .heater import Heater
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 
 
 class Heat(ModelObject):
@@ -18,21 +18,21 @@
         self._cold_extrude_temperature = 160
         # Minimum required temperature for retraction moves (in C)
         self._cold_retract_temperature = 90
         # List of configured heaters
         self._heaters = ModelCollection(Heater)
 
     @property
-    def bed_heaters(self) -> list[int]:
+    def bed_heaters(self) -> List[int]:
         """List of configured bed heaters (indices)
         Items may be -1 if unconfigured"""
         return self._bed_heaters
 
     @property
-    def chamber_heaters(self) -> list[int]:
+    def chamber_heaters(self) -> List[int]:
         """List of configured chamber heaters (indices)
         Items may be -1 if unconfigured"""
         return self._chamber_heaters
 
     @property
     def cold_extrude_temperature(self) -> float:
         """Minimum required temperature for extrusion moves (in C)"""
@@ -48,10 +48,10 @@
         return self._cold_retract_temperature
 
     @cold_retract_temperature.setter
     def cold_retract_temperature(self, value: float = 90):
         self._cold_retract_temperature = float(value)
 
     @property
-    def heaters(self) -> list[Heater]:
+    def heaters(self) -> List[Heater]:
         """List of configured heaters"""
         return self._heaters
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from enum import Enum
+from typing import List
 
 from .heater_model import HeaterModel
 from .heater_monitor import HeaterMonitor
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 
 
@@ -138,15 +138,15 @@
 
     @property
     def model(self) -> HeaterModel:
         """Information about the heater model"""
         return self._model
 
     @property
-    def monitors(self) -> list[HeaterMonitor]:
+    def monitors(self) -> List[HeaterMonitor]:
         """Monitors of this heater"""
         return self._monitors
 
     @property
     def sensor(self) -> int:
         """Sensor number of this heater or -1 if not configured"""
         return self._sensor
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater_model.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from ..model_object import ModelObject
 from .heater_model_pid import HeaterModelPID
 
 
 class HeaterModel(ModelObject):
     """Information about the way the heater heats up"""
 
@@ -104,14 +102,14 @@
 
     @property
     def pid(self) -> HeaterModelPID:
         """Details about the PID controller"""
         return self._pid
 
     @property
-    def standard_voltage(self) -> float | None:
+    def standard_voltage(self) -> float:
         """Standard voltage or null if unknown"""
         return self._standard_voltage
 
     @standard_voltage.setter
     def standard_voltage(self, value):
         self._standard_voltage = float(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater_model_pid.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater_model_pid.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     @property
     def overridden(self) -> bool:
         """Indicates if custom PID values are used"""
         return self._overridden
 
     @overridden.setter
-    def overridden(self, value: bool):
+    def overridden(self, value):
         self._overridden = bool(value)
 
     @property
     def p(self) -> float:
         """Proportional value of the PID regulator"""
         return self._p
 
@@ -55,9 +55,9 @@
 
     @property
     def used(self) -> bool:
         """Indicates if PID control is being used"""
         return self._used
 
     @used.setter
-    def used(self, value: bool):
+    def used(self, value):
         self._used = bool(value)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/heat/heater_monitor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/heat/heater_monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations
 from enum import Enum, IntEnum
 from typing import Union
 
 from ..model_object import ModelObject
 
 
 class HeaterMonitorAction(IntEnum):
@@ -57,33 +56,33 @@
     def action(self, value: Union[HeaterMonitorAction, None] = None):
         if value is None or isinstance(value, HeaterMonitorAction):
             self._action = value
         elif isinstance(value, int):
             self._action = HeaterMonitorAction(value)
         else:
             raise TypeError(f"{__name__}.action must be of type HeaterMonitorAction or None."
-                            f" Got {type(value)}: {value}")
+                            f"Got {type(value)}: {value}")
 
     @property
     def condition(self):
         """Condition to meet to perform an action"""
         return self._condition
 
     @condition.setter
     def condition(self, value: HeaterMonitorCondition = HeaterMonitorCondition.disabled):
-        if isinstance(value, HeaterMonitorCondition):
+        if value is None or isinstance(value, HeaterMonitorCondition):
             self._condition = value
         elif isinstance(value, str):
             self._condition = HeaterMonitorCondition(value)
         else:
             raise TypeError(f"{__name__}.condition must be of type HeaterMonitorCondition or None."
-                            f" Got {type(value)}: {value}")
+                            f"Got {type(value)}: {value}")
 
     @property
-    def limit(self) -> float | None:
+    def limit(self) -> float:
         """Limit threshold for this heater monitor"""
         return self._limit
 
     @limit.setter
     def limit(self, value: Union[float, None]):
         self._limit = float(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/inputs/input_channel.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/inputs/input_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,54 +58,52 @@
 
     @property
     def axes_relative(self) -> bool:
         """Whether relative positioning is being used"""
         return self._axes_relative
 
     @axes_relative.setter
-    def axes_relative(self, value: bool):
+    def axes_relative(self, value):
         self._axes_relative = bool(value)
 
     @property
     def compatibility(self) -> Compatibility:
         """Emulation used on this channel"""
         return self._compatibility
 
     @compatibility.setter
-    def compatibility(self, value: Compatibility):
+    def compatibility(self, value):
         if isinstance(value, Compatibility):
             self._compatibility = value
         elif isinstance(value, str):
             self._compatibility = Compatibility(value)
         else:
-            raise TypeError(f"{__name__}.compatibility must be of type Compatibility."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.compatibility must be of type Compatibility. Got {type(value)}: {value}")
 
     @property
     def distance_unit(self) -> DistanceUnit:
         """Whether inches are being used instead of mm"""
         return self._distance_unit
 
     @distance_unit.setter
-    def distance_unit(self, value: DistanceUnit):
+    def distance_unit(self, value):
         if isinstance(value, DistanceUnit):
             self._distance_unit = value
         elif isinstance(value, str):
             self._distance_unit = DistanceUnit(value)
         else:
-            raise TypeError(f"{__name__}.distance_unit must be of type DistanceUnit."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.distance_unit must be of type DistanceUnit. Got {type(value)}: {value}")
 
     @property
     def drives_relative(self) -> bool:
         """Whether relative extrusion is being used"""
         return self._drives_relative
 
     @drives_relative.setter
-    def drives_relative(self, value: bool):
+    def drives_relative(self, value):
         self._drives_relative = bool(value)
 
     @property
     def feed_rate(self) -> float:
         """Current feedrate in mm/s"""
         return self._feed_rate
 
@@ -115,15 +113,15 @@
 
     @property
     def in_macro(self) -> bool:
         """Whether a macro file is being processed"""
         return self._in_macro
 
     @in_macro.setter
-    def in_macro(self, value: bool):
+    def in_macro(self, value):
         self._in_macro = bool(value)
 
     @property
     def inverse_time_mode(self) -> bool:
         """Indicates if inverse time mode (G73) is active"""
         return self._inverse_time_mode
 
@@ -142,15 +140,15 @@
 
     @property
     def macro_restartable(self) -> bool:
         """Indicates if the current macro file can be restarted after a pause"""
         return self._macro_restartable
 
     @macro_restartable.setter
-    def macro_restartable(self, value: bool):
+    def macro_restartable(self, value):
         self._macro_restartable = bool(value)
 
     @property
     def motion_system(self) -> int:
         """Active motion system index"""
         return self._motion_system
 
@@ -160,22 +158,21 @@
 
     @property
     def name(self) -> CodeChannel:
         """Name of this channel"""
         return self._name
 
     @name.setter
-    def name(self, value: CodeChannel):
+    def name(self, value):
         if isinstance(value, CodeChannel):
             self._name = value
         elif isinstance(value, str):
             self._name = CodeChannel(value)
         else:
-            raise TypeError(f"{__name__}.name must be of type CodeChannel. "
-                            f"Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.name must be of type CodeChannel. Got {type(value)}: {value}")
 
     @property
     def selected_plane(self) -> int:
         """Index of the selected plane"""
         return self._selected_plane
 
     @selected_plane.setter
@@ -193,24 +190,23 @@
 
     @property
     def state(self) -> InputChannelState:
         """State of this input channel"""
         return self._state
 
     @state.setter
-    def state(self, value: InputChannelState):
+    def state(self, value):
         if isinstance(value, InputChannelState):
             self._state = value
         elif isinstance(value, str):
             self._state = InputChannelState(value)
         else:
-            raise TypeError(f"{__name__}.state must be of type InputChannelState. "
-                            f"Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.state must be of type InputChannelState. Got {type(value)}: {value}")
 
     @property
     def volumetric(self) -> bool:
         """Whether volumetric extrusion is being used"""
         return self._volumetric
 
     @volumetric.setter
-    def volumetric(self, value: bool):
+    def volumetric(self, value):
         self._volumetric = bool(value)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/inputs/inputs.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/inputs/inputs.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/build.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .build_object import BuildObject
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 
 
 class Build(ModelObject):
@@ -33,23 +33,23 @@
 
     @property
     def m486_names(self) -> bool:
         """Whether M486 names are being used"""
         return self._m486_names
 
     @m486_names.setter
-    def m486_names(self, value: bool):
+    def m486_names(self, value):
         self._m486_names = bool(value)
 
     @property
     def m486_numbers(self) -> bool:
         """Whether M486 numbers are being used"""
         return self._m486_numbers
 
     @m486_numbers.setter
-    def m486_numbers(self, value: bool):
+    def m486_numbers(self, value):
         self._m486_numbers = bool(value)
 
     @property
-    def objects(self) -> list[BuildObject]:
+    def objects(self) -> List[BuildObject]:
         """List of detected build objects"""
         return self._objects
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/build_object.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/build_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from __future__ import annotations
+from typing import List, Union
 
 from ..model_object import ModelObject
 
 
 class BuildObject(ModelObject):
     """Information about a detected build object"""
 
     def __init__(self):
         super().__init__()
         # Indicates if this build object is cancelled
         self._canceled = False
         # Name of the build object (if any)
         self._name = None
-        # X coordinates of the build object (in mm or None if not found)
+        # X coordinates of the build object (in mm or null if not found)
         self._x = None
-        # Y coordinates of the build object (in mm or None if not found)
+        # Y coordinates of the build object (in mm or null if not found)
         self._y = None
 
     @property
     def canceled(self) -> bool:
         """Indicates if this build object is cancelled"""
         return self._canceled
 
     @canceled.setter
-    def canceled(self, value: bool):
+    def canceled(self, value):
         self._canceled = bool(value)
 
     @property
-    def name(self) -> str | None:
+    def name(self) -> Union[str, None]:
         """Name of the build object (if any)"""
         return self._name
 
     @name.setter
-    def name(self, value: str | None = None):
+    def name(self, value):
         self._name = str(value) if value is not None else None
 
     @property
-    def x(self) -> list[float | None] | None:
-        """X coordinates of the build object (in mm or None if not found)"""
+    def x(self) -> Union[List[float], None]:
+        """X coordinates of the build object (in mm or null if not found)"""
         return self._x
 
     @property
-    def y(self) -> list[float | None] | None:
-        """Y coordinates of the build object (in mm or None if not found)"""
+    def y(self) -> Union[List[float], None]:
+        """Y coordinates of the build object (in mm or null if not found)"""
         return self._y
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/gcode_fileinfo.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/gcode_fileinfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from datetime import datetime
+from typing import List, Union
 
 from .thumbnail_info import ThumbnailInfo
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 
 
 class GCodeFileInfo(ModelObject):
@@ -20,59 +20,58 @@
         self._num_layers = 0
         self._print_time = None
         self._simulated_time = None
         self._size = 0
         self._thumbnails = ModelCollection(ThumbnailInfo)
 
     @property
-    def filament(self) -> list[float]:
+    def filament(self) -> List[float]:
         """Filament consumption per extruder drive (in mm)"""
         return self._filament
 
     @property
-    def file_name(self) -> str | None:
+    def file_name(self) -> Union[str, None]:
         """The filename of the G-code file"""
         return self._file_name
 
     @file_name.setter
-    def file_name(self, value : str | None = None):
+    def file_name(self, value):
         self._file_name = str(value) if value is not None else None
 
     @property
-    def generated_by(self) -> str | None:
+    def generated_by(self) -> Union[str, None]:
         """Name of the application that generated this file"""
         return self._generated_by
 
     @generated_by.setter
-    def generated_by(self, value: str | None = None):
+    def generated_by(self, value):
         self._generated_by = str(value) if value is not None else None
 
     @property
     def height(self) -> float:
         """Build height of the G-code job or 0 if not found (in mm)"""
         return self._height
 
     @height.setter
     def height(self, value):
         self._height = float(value)
 
     @property
-    def last_modified(self) -> datetime | None:
+    def last_modified(self) -> Union[datetime, None]:
         """Value indicating when the file was last modified or null if unknown"""
         return self._last_modified
 
     @last_modified.setter
-    def last_modified(self, value: datetime | None = None):
+    def last_modified(self, value):
         if isinstance(value, datetime) or value is None:
             self._last_modified = value
         elif isinstance(value, str):
             self._last_modified = datetime.fromisoformat(value)
         else:
-            raise TypeError(f"{__name__}.last_modified must be of type datetime or None. "
-                            f"Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.last_modified must be of type datetime or None. Got {type(value)}: {value}")
 
     @property
     def layer_height(self) -> float:
         """Height of each other layer or 0 if not found (in mm)"""
         return self._layer_height
 
     @layer_height.setter
@@ -85,37 +84,37 @@
         return self._num_layers
 
     @num_layers.setter
     def num_layers(self, value):
         self._num_layers = int(value)
 
     @property
-    def print_time(self) -> int | None:
+    def print_time(self) -> Union[int, None]:
         """Estimated print time (in s)"""
         return self._print_time
 
     @print_time.setter
-    def print_time(self, value: int | None = None):
+    def print_time(self, value):
         self._print_time = int(value) if value is not None else None
 
     @property
-    def simulated_time(self) -> int | None:
+    def simulated_time(self) -> Union[int, None]:
         """Estimated print time from G-code simulation (in s)"""
         return self._simulated_time
 
     @simulated_time.setter
-    def simulated_time(self, value: int | None = None):
+    def simulated_time(self, value):
         self._simulated_time = int(value) if value is not None else None
 
     @property
     def size(self) -> int:
         """Size of the file"""
         return self._size
 
     @size.setter
-    def size(self, value: int):
-        self._size = int(value)
+    def size(self, value):
+        self._size = int(value) if value is not None else None
 
     @property
-    def thumbnails(self) -> list[ThumbnailInfo]:
+    def thumbnails(self) -> List[ThumbnailInfo]:
         """Collection of thumbnails parsed from Gcode"""
         return self._thumbnails
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/job.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/job.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List, Union
 
 from .build import Build
 from .gcode_fileinfo import GCodeFileInfo
 from .layer import Layer
 from .times_left import TimesLeft
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
@@ -56,70 +56,70 @@
 
     @property
     def duration(self) -> Union[int, None]:
         """Total active duration of the current job file (in s or None)"""
         return self._duration
 
     @duration.setter
-    def duration(self, value: int | None = None):
+    def duration(self, value):
         self._duration = int(value) if value is not None else None
 
     @property
     def file_position(self) -> Union[int, None]:
         """Current position in the file being processed (in bytes or None)"""
         return self._file_position
 
     @file_position.setter
-    def file_position(self, value: int | None = None):
+    def file_position(self, value):
         self._file_position = int(value) if value is not None else None
 
     @property
     def last_duration(self) -> Union[int, None]:
         """Total duration of the last job (in s or None)"""
         return self._last_duration
 
     @last_duration.setter
-    def last_duration(self, value: int | None = None):
+    def last_duration(self, value):
         self._last_duration = int(value) if value is not None else None
 
     @property
     def last_file_aborted(self) -> bool:
         """Indicates if the last file was aborted (unexpected cancellation)"""
         return self._last_file_aborted
 
     @last_file_aborted.setter
-    def last_file_aborted(self, value: bool):
+    def last_file_aborted(self, value):
         self._last_file_aborted = bool(value)
 
     @property
     def last_file_cancelled(self) -> bool:
         """Indicates if the last file was cancelled (user cancelled)"""
         return self._last_file_cancelled
 
     @last_file_cancelled.setter
-    def last_file_cancelled(self, value: bool):
+    def last_file_cancelled(self, value):
         self._last_file_cancelled = bool(value)
 
     @property
     def last_file_name(self) -> Union[str, None]:
         """Name of the last file processed or None"""
         return self._last_file_name
 
     @last_file_name.setter
-    def last_file_name(self, value: str | None = None):
+    def last_file_name(self, value):
         self._last_file_name = str(value) if value is not None else None
 
     @property
     def last_file_simulated(self) -> bool:
         """Indicates if the last file processed was simulated
         This is not set if the file was aborted or cancelled"""
         return self._last_file_simulated
 
     @last_file_simulated.setter
-    def last_file_simulated(self, value: bool):
+    def last_file_simulated(self, value):
         self._last_file_simulated = bool(value)
 
     @property
     def last_warm_up_duration(self) -> Union[int, None]:
         """Warm-up duration of the last print or None if not available (in s)"""
         return self._last_warm_up_duration
 
@@ -129,56 +129,60 @@
 
     @property
     def layer(self) -> Union[int, None]:
         """Number of the current layer or None if not available"""
         return self._layer
 
     @layer.setter
-    def layer(self, value: int | None = None):
+    def layer(self, value):
         self._layer = int(value) if value is not None else None
 
     @property
-    def layers(self) -> list[Layer]:
+    def layers(self) -> List[Layer]:
         """Information about the past layers
+        In previous API versions this was a ModelGrowingCollection{T} but it has been changed to ModelCollection{T} to
+        allow past layers to be modified again when needed.
+        Note that previous plugins subscribing to this property will not receive any more updates about this property
+        to avoid memory leaks.
         See also Layer"""
         return self._layers
 
     @property
     def layer_time(self) -> Union[float, None]:
         """Time elapsed since the last layer change (in s or None)"""
         return self._layer_time
 
     @layer_time.setter
-    def layer_time(self, value: float | None = None):
+    def layer_time(self, value):
         self._layer_time = float(value) if value is not None else None
 
     @property
-    def pause_duration(self) -> int | None:
+    def pause_duration(self) -> Union[int, None]:
         """Total pause time since the job started"""
         return self._pause_duration
 
     @pause_duration.setter
-    def pause_duration(self, value: int | None = None):
+    def pause_duration(self, value):
         self._pause_duration = int(value) if value is not None else None
 
     @property
-    def raw_extrusion(self) -> float | None:
+    def raw_extrusion(self) -> Union[float, None]:
         """Total extrusion amount without extrusion factors applied (in mm)"""
         return self._raw_extrusion
 
     @raw_extrusion.setter
-    def raw_extrusion(self, value: float | None = None):
+    def raw_extrusion(self, value):
         self._raw_extrusion = float(value) if value is not None else None
 
     @property
     def times_left(self) -> TimesLeft:
         """Estimated times left"""
         return self._times_left
 
     @property
     def warm_up_duration(self) -> Union[int, None]:
         """Time needed to heat up the heaters (in s or None)"""
         return self._warm_up_duration
 
     @warm_up_duration.setter
-    def warm_up_duration(self, value: int | None = None):
+    def warm_up_duration(self, value):
         self._warm_up_duration = int(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/layer.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from ..model_object import ModelObject
 
 
 class Layer(ModelObject):
     """Information about a layer from a file being printed"""
 
@@ -25,15 +25,15 @@
         return self._duration
 
     @duration.setter
     def duration(self, value):
         self._duration = float(value)
 
     @property
-    def filament(self) -> list[float]:
+    def filament(self) -> List[float]:
         """Actual amount of filament extruded during this layer (in mm)"""
         return self._filament
 
     @property
     def fraction_printed(self) -> float:
         """Fraction of the file printed during this layer (0..1)"""
         return self._fraction_printed
@@ -48,10 +48,10 @@
         return self._height
 
     @height.setter
     def height(self, value):
         self._height = int(value)
 
     @property
-    def temperatures(self) -> list[float]:
+    def temperatures(self) -> List[float]:
         """Last heater temperatures (in C or null if unknown)"""
         return self._temperatures
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/thumbnail_info.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/thumbnail_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from enum import Enum
+from typing import Union
 
 from ..model_object import ModelObject
 
 
 class ThumbnailInfoFormat(str, Enum):
     """Image formats for parsed thumbnails"""
 
@@ -31,38 +31,37 @@
         self._offset = 0
         # Size of this thumbnail
         self._size = 0
         # Width of this thumbnail
         self._width = 0
 
     @property
-    def data(self) -> str | None:
+    def data(self) -> Union[str, None]:
         """Base64-encoded thumbnail or null if invalid or not requested
         This property is not provided by RepRapFirmware fileinfo results,
         and it may be null if no thumbnail content is requested"""
         return self._data
 
     @data.setter
-    def data(self, value: str | None = None):
+    def data(self, value):
         self._data = str(value) if value is not None else None
 
     @property
     def format(self) -> ThumbnailInfoFormat:
         """Format of this thumbnail"""
         return self._format
 
     @format.setter
-    def format(self, value: ThumbnailInfoFormat):
+    def format(self, value):
         if isinstance(value, ThumbnailInfoFormat):
             self._format = value
         elif isinstance(value, str):
             self._format = ThumbnailInfoFormat(value)
         else:
-            raise TypeError(f"{__name__}.format must be of type ThumbnailInfoFormat."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.format must be of type ThumbnailInfoFormat. Got {type(value)}: {value}")
 
     @property
     def height(self) -> int:
         """Height of this thumbnail"""
         return self._height
 
     @height.setter
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/job/times_left.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/job/times_left.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from ..model_object import ModelObject
 
 
 class TimesLeft(ModelObject):
     """Estimations about the times left"""
 
@@ -12,32 +12,32 @@
         self._filament = None
         # Time left based on file progress (in s or null)
         self._file = None
         # Time left based on the slicer reports (see M73, in s or null)
         self._slicer = None
 
     @property
-    def filament(self) -> int | None:
+    def filament(self) -> Union[int, None]:
         """Time left based on filament consumption (in s or null)"""
         return self._filament
 
     @filament.setter
-    def filament(self, value: int | None = None):
+    def filament(self, value):
         self._filament = int(value) if value is not None else None
 
     @property
-    def file(self) -> int | None:
+    def file(self) -> Union[int, None]:
         """Time left based on file progress (in s or null)"""
         return self._file
 
     @file.setter
-    def file(self, value: int | None = None):
+    def file(self, value):
         self._file = int(value) if value is not None else None
 
     @property
-    def slicer(self) -> int | None:
+    def slicer(self) -> Union[int, None]:
         """Time left based on the slicer reports (see M73, in s or null)"""
         return self._slicer
 
     @slicer.setter
-    def slicer(self, value: int | None = None):
+    def slicer(self, value):
         self._slicer = int(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/led_strips/led_strip.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/led_strips/led_strip.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/limits/limits.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/limits/limits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from ..model_object import ModelObject
 
 
 class Limits(ModelObject):
     """Machine configuration limits"""
 
@@ -60,137 +60,137 @@
         self._workplaces = None
         # Maximum number of Z-probe programming bytes or null if unknown
         self._z_probe_program_bytes = None
         # Maximum number of Z-probes or null if unknown
         self._z_probes = None
 
     @property
-    def axes(self) -> int | None:
+    def axes(self) -> Union[int, None]:
         """Maximum number of axes or null if unknown"""
         return self._axes
 
     @axes.setter
-    def axes(self, value: int | None = None):
+    def axes(self, value):
         self._axes = int(value) if value is not None else None
 
     @property
-    def axes_plus_extruders(self) -> int | None:
+    def axes_plus_extruders(self) -> Union[int, None]:
         """Maximum number of axes + extruders or null if unknown"""
         return self._axes_plus_extruders
 
     @axes_plus_extruders.setter
-    def axes_plus_extruders(self, value: int | None = None):
+    def axes_plus_extruders(self, value):
         self._axes_plus_extruders = int(value) if value is not None else None
 
     @property
-    def bed_heaters(self) -> int | None:
+    def bed_heaters(self) -> Union[int, None]:
         """Maximum number of bed heaters or null if unknown"""
         return self._bed_heaters
 
     @bed_heaters.setter
-    def bed_heaters(self, value: int | None = None):
+    def bed_heaters(self, value):
         self._bed_heaters = int(value) if value is not None else None
 
     @property
-    def boards(self) -> int | None:
+    def boards(self) -> Union[int, None]:
         """Maximum number of boards or null if unknown"""
         return self._boards
 
     @boards.setter
-    def boards(self, value: int | None = None):
+    def boards(self, value):
         self._boards = int(value) if value is not None else None
 
     @property
-    def chamber_heaters(self) -> int | None:
+    def chamber_heaters(self) -> Union[int, None]:
         """Maximum number of chamber heaters or null if unknown"""
         return self._chamber_heaters
 
     @chamber_heaters.setter
-    def chamber_heaters(self, value: int | None = None):
+    def chamber_heaters(self, value):
         self._chamber_heaters = int(value) if value is not None else None
 
     @property
-    def drivers(self) -> int | None:
+    def drivers(self) -> Union[int, None]:
         """Maximum number of drivers or null if unknown"""
         return self._drivers
 
     @drivers.setter
-    def drivers(self, value: int | None = None):
+    def drivers(self, value):
         self._drivers = int(value) if value is not None else None
 
     @property
-    def drivers_per_axis(self) -> int | None:
+    def drivers_per_axis(self) -> Union[int, None]:
         """Maximum number of drivers per axis or null if unknown"""
         return self._drivers_per_axis
 
     @drivers_per_axis.setter
-    def drivers_per_axis(self, value: int | None = None):
+    def drivers_per_axis(self, value):
         self._drivers_per_axis = int(value) if value is not None else None
 
     @property
-    def extruders(self) -> int | None:
+    def extruders(self) -> Union[int, None]:
         """Maximum number of extruders or null if unknown"""
         return self._extruders
 
     @extruders.setter
-    def extruders(self, value: int | None = None):
+    def extruders(self, value):
         self._extruders = int(value) if value is not None else None
 
     @property
-    def extruders_per_tool(self) -> int | None:
+    def extruders_per_tool(self) -> Union[int, None]:
         """Maximum number of extruders per tool or null if unknown"""
         return self._extruders_per_tool
 
     @extruders_per_tool.setter
-    def extruders_per_tool(self, value: int | None = None):
+    def extruders_per_tool(self, value):
         self._extruders_per_tool = int(value) if value is not None else None
 
     @property
-    def fans(self) -> int | None:
+    def fans(self) -> Union[int, None]:
         """Maximum number of fans or null if unknown"""
         return self._fans
 
     @fans.setter
-    def fans(self, value: int | None = None):
+    def fans(self, value):
         self._fans = int(value) if value is not None else None
 
     @property
-    def gp_in_ports(self) -> int | None:
+    def gp_in_ports(self) -> Union[int, None]:
         """Maximum number of general-purpose input ports or null if unknown"""
         return self._gp_in_ports
 
     @gp_in_ports.setter
-    def gp_in_ports(self, value: int | None = None):
+    def gp_in_ports(self, value):
         self._gp_in_ports = int(value) if value is not None else None
 
     @property
-    def gp_out_ports(self) -> int | None:
+    def gp_out_ports(self) -> Union[int, None]:
         """Maximum number of general-purpose output ports or null if unknown"""
         return self._gp_out_ports
 
     @gp_out_ports.setter
-    def gp_out_ports(self, value: int | None = None):
+    def gp_out_ports(self, value):
         self._gp_out_ports = int(value) if value is not None else None
 
     @property
-    def heaters(self) -> int | None:
+    def heaters(self) -> Union[int, None]:
         """Maximum number of heaters or null if unknown"""
         return self._heaters
 
     @heaters.setter
-    def heaters(self, value: int | None = None):
+    def heaters(self, value):
         self._heaters = int(value) if value is not None else None
 
     @property
-    def heaters_per_tool(self) -> int | None:
+    def heaters_per_tool(self) -> Union[int, None]:
         """Maximum number of heaters per tool or null if unknown"""
         return self._heaters_per_tool
 
     @heaters_per_tool.setter
-    def heaters_per_tool(self, value: int | None = None):
+    def heaters_per_tool(self, value):
         self._heaters_per_tool = int(value) if value is not None else None
 
     @property
     def led_strips(self) -> Union[int, None]:
         """Maximum number of configured LED strips or null if unknown"""
         return self._led_strips
 
@@ -200,15 +200,15 @@
 
     @property
     def monitors_per_heater(self) -> Union[int, None]:
         """Maximum number of monitors per heater or null if unknown"""
         return self._monitors_per_heater
 
     @monitors_per_heater.setter
-    def monitors_per_heater(self, value: int | None = None):
+    def monitors_per_heater(self, value):
         self._monitors_per_heater = int(value) if value is not None else None
 
     @property
     def ports_per_heater(self) -> Union[int, None]:
         """Maximum number of output ports per heater or null if unknown"""
         return self._ports_per_heater
 
@@ -218,90 +218,90 @@
 
     @property
     def restore_points(self) -> Union[int, None]:
         """Maximum number of restore points or null if unknown"""
         return self._restore_points
 
     @restore_points.setter
-    def restore_points(self, value: int | None = None):
+    def restore_points(self, value):
         self._restore_points = int(value) if value is not None else None
 
     @property
-    def sensors(self) -> int | None:
+    def sensors(self) -> Union[int, None]:
         """Maximum number of sensors or null if unknown"""
         return self._sensors
 
     @sensors.setter
-    def sensors(self, value: int | None = None):
+    def sensors(self, value):
         self._sensors = int(value) if value is not None else None
 
     @property
-    def spindles(self) -> int | None:
+    def spindles(self) -> Union[int, None]:
         """Maximum number of spindles or null if unknown"""
         return self._spindles
 
     @spindles.setter
-    def spindles(self, value: int | None = None):
+    def spindles(self, value):
         self._spindles = int(value) if value is not None else None
 
     @property
-    def tools(self) -> int | None:
+    def tools(self) -> Union[int, None]:
         """Maximum number of tools or null if unknown"""
         return self._tools
 
     @tools.setter
-    def tools(self, value: int | None = None):
+    def tools(self, value):
         self._tools = int(value) if value is not None else None
 
     @property
-    def tracked_objects(self) -> int | None:
+    def tracked_objects(self) -> Union[int, None]:
         """Maximum number of tracked objects or null if unknown"""
         return self._tracked_objects
 
     @tracked_objects.setter
-    def tracked_objects(self, value: int | None = None):
+    def tracked_objects(self, value):
         self._tracked_objects = int(value) if value is not None else None
 
     @property
-    def triggers(self) -> int | None:
+    def triggers(self) -> Union[int, None]:
         """Maximum number of triggers or null if unknown"""
         return self._triggers
 
     @triggers.setter
-    def triggers(self, value: int | None = None):
+    def triggers(self, value):
         self._triggers = int(value) if value is not None else None
 
     @property
-    def volumes(self) -> int | None:
+    def volumes(self) -> Union[int, None]:
         """Maximum number of triggers or null if unknown"""
         return self._volumes
 
     @volumes.setter
-    def volumes(self, value: int | None = None):
+    def volumes(self, value):
         self._volumes = int(value) if value is not None else None
 
     @property
-    def workplaces(self) -> int | None:
+    def workplaces(self) -> Union[int, None]:
         """Maximum number of workplaces or null if unknown"""
         return self._workplaces
 
     @workplaces.setter
-    def workplaces(self, value: int | None = None):
+    def workplaces(self, value):
         self._workplaces = int(value) if value is not None else None
 
     @property
-    def z_probe_program_bytes(self) -> int | None:
+    def z_probe_program_bytes(self) -> Union[int, None]:
         """Maximum number of Z-probe programming bytes or null if unknown"""
         return self._z_probe_program_bytes
 
     @z_probe_program_bytes.setter
-    def z_probe_program_bytes(self, value: int | None = None):
+    def z_probe_program_bytes(self, value):
         self._z_probe_program_bytes = int(value) if value is not None else None
 
     @property
-    def z_probes(self) -> int | None:
+    def z_probes(self) -> Union[int, None]:
         """Maximum number of Z-probes or null if unknown"""
         return self._z_probes
 
     @z_probes.setter
-    def z_probes(self, value: int | None = None):
+    def z_probes(self, value):
         self._z_probes = int(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/messages/messages.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/messages/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations
 import dateutil.parser as dp
 from datetime import datetime
 from enum import IntEnum
 
 from ..model_object import ModelObject
 
 
@@ -24,15 +23,15 @@
     Generic container for messages
     :param content: Content of this message
     :param time: Time at which the message was generated
     :param msg_type: Type of this message
     """
 
     @classmethod
-    def from_json(cls, data: dict[any]) -> 'Message':
+    def from_json(cls, data):
         """Deserialize an instance of this class from JSON deserialized dictionary"""
         data['msg_type'] = data.pop('type')  # Replace 'type' to not shadow the built-in keyword name
         return cls(**data)
 
     def __init__(self, msg_type: MessageType = MessageType.Success, content: str = "", time: datetime = datetime.now()):
         super().__init__()
         self._content = content
@@ -49,39 +48,37 @@
 
     @property
     def content(self) -> str:
         """Content of this message"""
         return self._content
 
     @content.setter
-    def content(self, value: str):
+    def content(self, value):
         self._content = str(value)
 
     @property
     def time(self) -> datetime:
         """Time at which the message was generated"""
         return self._time
 
     @time.setter
-    def time(self, value: datetime):
+    def time(self, value):
         if isinstance(value, datetime):
             self._time = value
         elif isinstance(value, str):  # Update from JSON
             self._time = dp.isoparse(value)
         else:
-            raise TypeError(f"{__name__}.time must be of type datetime."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.time must be of type datetime. Got {type(value)}: {value}")
 
     @property
     def type(self) -> MessageType:
         """Type of this message"""
         return self._type
 
     @type.setter
-    def type(self, value: MessageType):
+    def type(self, value):
         if isinstance(value, MessageType):
             self._type = value
         elif isinstance(value, int):
             self._type = MessageType(value)
         else:
-            raise TypeError(f"{__name__}.type must be of type MessageType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.type must be of type MessageType. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/model_collection.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/model_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from .utils import is_model_object
 
 
 class ModelCollection(list):
     """
     Class for storing model object items in a list
     Useful for updating model object items from JSON data (patches)
@@ -17,15 +15,15 @@
         """
         super().__init__()
         self._item_constructor = item_constructor
 
         if value is not None:
             self[:] = value
 
-    def update_from_json(self, json_element: dict[any]):
+    def update_from_json(self, json_element):
         """
         Update this instance from the given data
         :param json_element: JSON data to upgrade this instance from
         :return: Updated instance
         """
         if not isinstance(json_element, list):
             raise Exception(f"Invalid JSON element type for model collection {type(json_element)}.")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/model_dictionary.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/model_dictionary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import annotations
-
 from .utils import is_model_object
 
 
 class ModelDictionary(dict):
     """
     Class for storing model object items in a dictionary
     Useful for updating model object items from JSON data (patches)
     """
 
-    def __init__(self, null_deletes_keys: bool, item_constructor=None, value=None):
+    def __init__(self, null_deletes_keys, item_constructor=None, value=None):
         """
         :param null_deletes_keys: Whether setting null to items effectively deletes them
         :param item_constructor: Item constructor type to use for type-checking
         :param value: Value used to initialize the dictionary from
         """
         super().__init__()
         self._item_constructor = item_constructor
@@ -44,14 +42,14 @@
                 return super().__setitem__(key, new_item)
         elif is_model_object(current_item):
             new_item = current_item.update_from_json(value)
             return super().__setitem__(key, new_item)
 
         return super().__setitem__(key, value)
 
-    def update_from_json(self, json_element: dict[any]):
+    def update_from_json(self, json_element):
         if json_element is None:
             super().clear()
         else:
             for k, v in json_element.items():
                 self[k] = v
         return self
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/model_object.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/model_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import annotations
 import json
 from datetime import datetime
+from typing import Union
 
 
 from .utils import is_model_object
 from ..utils import preserve_builtin, camel_to_snake, snake_to_camel
 
 
 class FloatJSON(float):
@@ -75,22 +75,22 @@
                 if is_model_object(attr):
                     setattr(self, attr_name, attr.update_from_json(json_value))
                 elif isinstance(attr, list):
                     setattr(self, attr_name, json_value)
         return self
 
     @classmethod
-    def from_json(cls, data: dict[any] | str) -> 'ModelObject':
+    def from_json(cls, data: Union[dict, str]) -> 'ModelObject':
         """Deserialize a new instance of this class from JSON deserialized dictionary"""
         # Deserialize a string object into a JSON (dict) object
         if isinstance(data, str):
             data = json.loads(data)
         return cls()._update_from_json(**preserve_builtin(data))
 
-    def update_from_json(self, data: dict[any] | str):
+    def update_from_json(self, data: Union[dict, str]):
         """Update the current instance of this class from JSON deserialized dictionary"""
         if isinstance(data, str):
             data = json.loads(data)
         return self._update_from_json(**preserve_builtin(data))
 
     def to_json(self) -> str:
         """Serialize this instance of this class into a JSON dictionary"""
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/__init__.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/__init__.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/axis.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from enum import Enum
+from typing import List, Union
 
 from .driver_id import DriverId
 from .microstepping import MicroStepping
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 
 
@@ -22,14 +22,34 @@
     D = 'D'
     a = 'a'
     b = 'b'
     c = 'c'
     d = 'd'
     e = 'e'
     f = 'f'
+    g = 'g'
+    h = 'h'
+    i = 'i'
+    j = 'j'
+    k = 'k'
+    l = 'l'
+    m = 'm'
+    n = 'n'
+    o = 'o'
+    p = 'p'
+    q = 'q'
+    r = 'r'
+    s = 's'
+    t = 't'
+    u = 'u'
+    v = 'v'
+    w = 'w'
+    x = 'x'
+    y = 'y'
+    z = 'z'
     none = ''
 
 
 class Axis(ModelObject):
     """Information about a configured axis"""
 
     def __init__(self):
@@ -112,25 +132,25 @@
         return self._current
 
     @current.setter
     def current(self, value):
         self._current = int(value)
 
     @property
-    def drivers(self) -> list[DriverId]:
+    def drivers(self) -> List[DriverId]:
         """List of the assigned drivers"""
         return self._drivers
 
     @property
     def homed(self) -> bool:
         """Whether the axis is homed"""
         return self._homed
 
     @homed.setter
-    def homed(self, value: bool):
+    def homed(self, value):
         self._homed = bool(value)
 
     @property
     def jerk(self) -> float:
         """Motor jerk (in mm/min)"""
         return self._jerk
 
@@ -140,32 +160,31 @@
 
     @property
     def letter(self) -> AxisLetter:
         """Letter of this axis"""
         return self._letter
 
     @letter.setter
-    def letter(self, value: AxisLetter):
+    def letter(self, value):
         if isinstance(value, AxisLetter):
             self._letter = value
         elif isinstance(value, str):
             self._letter = AxisLetter(value)
         else:
-            raise TypeError(f"{__name__}.letter must be of type AxisLetter."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.letter must be of type AxisLetter. Got {type(value)}: {value}")
 
     @property
     def machine_position(self) -> Union[float, None]:
         """Current machine position (in mm) or None if unknown/unset
         This value reflects the machine position of the move being performed
         or of the last one if the machine is not moving"""
         return self._machine_position
 
     @machine_position.setter
-    def machine_position(self, value: float | None = None):
+    def machine_position(self, value):
         self._machine_position = float(value) if value is not None else None
 
     @property
     def max(self) -> float:
         """Maximum travel of this axis (in mm)"""
         return self._max
 
@@ -175,15 +194,15 @@
 
     @property
     def max_probed(self) -> bool:
         """Whether the axis maximum was probed"""
         return self._max_probed
 
     @max_probed.setter
-    def max_probed(self, value: bool):
+    def max_probed(self, value):
         self._max_probed = bool(value)
 
     @property
     def microstepping(self) -> MicroStepping:
         """Microstepping configuration"""
         return self._microstepping
 
@@ -198,15 +217,15 @@
 
     @property
     def min_probed(self) -> bool:
         """Whether the axis minimum was probed"""
         return self._min_probed
 
     @min_probed.setter
-    def min_probed(self, value: bool):
+    def min_probed(self, value):
         self._min_probed = bool(value)
 
     @property
     def percent_current(self) -> int:
         """Percentage applied to the motor current (0..100)"""
         return self._percent_current
 
@@ -216,15 +235,15 @@
 
     @property
     def percent_stst_current(self) -> Union[int, None]:
         """Percentage applied to the motor current during standstill (0..100 or None if not supported)"""
         return self._percent_stst_current
 
     @percent_stst_current.setter
-    def percent_stst_current(self, value: int | None = None):
+    def percent_stst_current(self, value):
         self._percent_stst_current = int(value) if value is not None else None
 
     @property
     def reduced_acceleration(self) -> float:
         """Reduced accelerations used by Z probing and stall homing moves (in mm/s^2)"""
         return self._reduced_acceleration
 
@@ -253,23 +272,23 @@
     @property
     def user_position(self) -> Union[float, None]:
         """Current user position (in mm) or None if unknown
         This value reflects the target position of the last move fed into the look-ahead buffer"""
         return self._user_position
 
     @user_position.setter
-    def user_position(self, value: float | None = None):
+    def user_position(self, value):
         self._user_position = float(value) if value is not None else None
 
     @property
     def visible(self) -> bool:
         """Whether the axis is visible"""
         return self._visible
 
     @visible.setter
     def visible(self, value):
         self._visible = bool(value)
 
     @property
-    def workplace_offsets(self) -> list[float]:
+    def workplace_offsets(self) -> List[float]:
         """Offsets of this axis for each workplace (in mm)"""
         return self._workplace_offsets
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/current_move.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/current_move.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from ..model_object import ModelObject
 
 
 class CurrentMove(ModelObject):
     """Information about the current move"""
     def __init__(self):
@@ -31,15 +31,15 @@
 
     @property
     def deceleration(self) -> float:
         """Deceleration of the current move (in mm/s^2)"""
         return self._deceleration
 
     @deceleration.setter
-    def deceleration(self, value: float):
+    def deceleration(self, value):
         self._deceleration = float(value)
 
     @property
     def extrusion_rate(self) -> float:
         """Current extrusion rate (in mm/s)"""
         return self._extrusion_rate
 
@@ -49,27 +49,27 @@
 
     @property
     def laser_pwm(self) -> Union[float, None]:
         """Laser PWM of the current move (0..1) or null if not applicable"""
         return self._laser_pwm
 
     @laser_pwm.setter
-    def laser_pwm(self, value: float | None = None):
+    def laser_pwm(self, value):
         self._laser_pwm = float(value) if value is not None else None
 
     @property
     def requested_speed(self) -> float:
         """Requested speed of the current move (in mm/s)"""
         return self._requested_speed
 
     @requested_speed.setter
-    def requested_speed(self, value: float):
+    def requested_speed(self, value):
         self._requested_speed = float(value)
 
     @property
     def top_speed(self) -> float:
         """Top speed of the current move (in mm/s)"""
         return self._top_speed
 
     @top_speed.setter
-    def top_speed(self, value: float):
+    def top_speed(self, value):
         self._top_speed = float(value)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/driver_id.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/driver_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import annotations
 import re
 
 from ..model_object import ModelObject
 from ...exceptions import CodeParserException
 
 
-def is_driverId(value: any):
+def is_driverId(value):
     return isinstance(value, DriverId)
 
 
 class DriverId(ModelObject):
     """
     Class representing a driver identifier
     :param board: Board of this driver identifier
@@ -55,15 +54,15 @@
         if self is None:
             return o is None
         return isinstance(o, DriverId) and self.board == o.board and self.port == o.port
 
     def __ne__(self, o):
         return not self == o
 
-    def update_from_json(self, data: dict[any]) -> DriverId | None:
+    def update_from_json(self, data):
         if isinstance(data, str):
             matches = re.search(r'(\d+)\.(\d+)', data)
             if matches:
                 self.board = int(matches.group(1))
                 self.port = int(matches.group(2))
             else:
                 self.board = None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/extruder.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/extruder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from .driver_id import DriverId
 from .extruder_non_linear import ExtruderNonlinear
 from .microstepping import MicroStepping
 from ..model_object import ModelObject
 from ..utils import wrap_model_property
 
@@ -31,15 +31,15 @@
         self._jerk = 15
         # Microstepping configuration
         self._microstepping = MicroStepping()
         # Nonlinear extrusion parameters (see M592)
         self._nonlinear = ExtruderNonlinear()
         # Percentage applied to the motor current (0..100)
         self._percent_current = 100
-        # Percentage applied to the motor current during standstill (0..100 or None if not supported)
+        # Percentage applied to the motor current during standstill (0..100 or null if not supported)
         self._percent_stst_current = None
         # Extruder position (in mm)
         self._position = 0
         # Pressure advance
         self._pressure_advance = 0
         # Raw extruder position as commanded by the slicer without extrusion factor applied (in mm)
         self._raw_position = 0
@@ -77,15 +77,15 @@
 
     @property
     def filament(self) -> str:
         """Name of the currently loaded filament"""
         return self._filament
 
     @filament.setter
-    def filament(self, value: str):
+    def filament(self, value):
         self._filament = str(value)
 
     @property
     def filament_diameter(self) -> float:
         """Diameter of the corresponding filament (in mm)"""
         return self._filament_diameter
 
@@ -118,20 +118,20 @@
         return self._percent_current
 
     @percent_current.setter
     def percent_current(self, value):
         self._percent_current = int(value)
 
     @property
-    def percent_stst_current(self) -> int | None:
-        """Percentage applied to the motor current during standstill (0..100 or None if not supported)"""
+    def percent_stst_current(self) -> Union[int, None]:
+        """Percentage applied to the motor current during standstill (0..100 or null if not supported)"""
         return self._percent_stst_current
 
     @percent_stst_current.setter
-    def percent_stst_current(self, value: int | None = None):
+    def percent_stst_current(self, value):
         self._percent_stst_current = int(value) if value is not None else None
 
     @property
     def position(self) -> float:
         """Extruder position (in mm)"""
         return self._position
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/extruder_non_linear.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/extruder_non_linear.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/input_shaping.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/input_shaping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from enum import Enum
+from typing import List
 
 from ..model_object import ModelObject
 
 
 class InputShapingType(str, Enum):
     """Enumeration of possible input shaping methods"""
 
@@ -47,29 +47,29 @@
         # Minimum fraction of the original acceleration or feed rate to which the acceleration or
         # feed rate may be reduced in order to apply input shaping
         self._reduction_limit = 0.25
         # Configured input shaping type
         self._type = InputShapingType.none
 
     @property
-    def amplitudes(self) -> list[float]:
+    def amplitudes(self) -> List[float]:
         """Amplitudes of the input shaper"""
         return self._amplitudes
 
     @property
     def damping(self) -> float:
         """Damping factor"""
         return self._damping
 
     @damping.setter
     def damping(self, value):
         self._damping = float(value)
 
     @property
-    def durations(self) -> list[float]:
+    def durations(self) -> List[float]:
         """Input shaper durations (in s)"""
         return self._durations
 
     @property
     def frequency(self) -> float:
         """Frequency (in Hz)"""
         return self._frequency
@@ -90,15 +90,14 @@
 
     @property
     def type(self) -> InputShapingType:
         """Configured input shaping type"""
         return self._type
 
     @type.setter
-    def type(self, value: InputShapingType):
+    def type(self, value):
         if isinstance(value, InputShapingType):
             self._type = value
         elif isinstance(value, str):
             self._type = InputShapingType(value)
         else:
-            raise TypeError(f"{__name__}.type must be of type InputShapingType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.type must be of type InputShapingType. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/keepout_zone.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/keepout_zone.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/__init__.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/__init__.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/core_kinematics.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/core_kinematics.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/delta_kinematics.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/delta_kinematics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .delta_tower import DeltaTower
 from .kinematics import Kinematics
 from .kinematics_name import KinematicsName
 from ...model_collection import ModelCollection
 
 
@@ -47,15 +47,15 @@
         return self._print_radius
     
     @print_radius.setter
     def print_radius(self, value):
         self._print_radius = float(value)
 
     @property
-    def towers(self) -> list[DeltaTower]:
+    def towers(self) -> List[DeltaTower]:
         """Delta tower properties"""
         return self._towers
     
     @property
     def x_tilt(self) -> float:
         """How much Z needs to be raised for each unit of movement in the +X direction"""
         return self._x_tilt
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/delta_tower.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/delta_tower.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/hangprinter_kinematics.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/hangprinter_kinematics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .kinematics import Kinematics
 from .kinematics_name import KinematicsName
 
 
 class HangprinterKinematics(Kinematics):
     """Information about hangprinter kinematics"""
@@ -15,15 +15,15 @@
             [2000,   1000, -100],
             [-2000,  1000, -100],
             [0,      0,    3000]
         ]
         self._print_radius = 1500
 
     @property
-    def anchors(self) -> list[list[float]]:
+    def anchors(self) -> List[List[float]]:
         """Anchor configurations for A, B, C, Dz"""
         return self._anchors
     
     @property
     def print_radius(self) -> float:
         """Print radius (in mm)"""
         return self._print_radius
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/kinematics.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/kinematics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from .kinematics_name import KinematicsName
 from ..move_segmentation import MoveSegmentation
 from ...model_object import ModelObject
 
 
 class Kinematics(ModelObject):
@@ -53,32 +53,32 @@
 
     @property
     def name(self) -> KinematicsName:
         """Name of the configured kinematics"""
         return self._name
 
     @property
-    def segmentation(self) -> MoveSegmentation | None:
+    def segmentation(self) -> Union[MoveSegmentation, None]:
         """Segmentation parameters or null if not configured"""
         return self._segmentation
 
     @segmentation.setter
-    def segmentation(self, value: MoveSegmentation | None = None):
+    def segmentation(self, value):
         if value is None or isinstance(value, MoveSegmentation):
             self._segmentation = value
         elif isinstance(value, dict):  # Update from JSON
             if self._segmentation is None:
                 self._segmentation = MoveSegmentation.from_json(value)
             else:
                 self._segmentation.update_from_json(value)
         else:
             raise TypeError(f"{__name__}.segmentation must be None or of type MoveSegmentation."
                             f"Got {type(value)}: {value}")
 
-    def _update_from_json(self, **kwargs) -> Kinematics:
+    def _update_from_json(self, **kwargs):
         """Override ObjectModel._update_from_json to return the Kinematics type matching the given name"""
         if 'name' in kwargs and self.name != KinematicsName(kwargs.get('name')):
             kinematic_type = self.get_kinematics_type(kwargs.get('name'))
             new_kinematic = kinematic_type.update_from_json(kwargs)
             return new_kinematic
 
         super(Kinematics, self)._update_from_json(**kwargs)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/tilt_correction.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/tilt_correction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from ...model_object import ModelObject
 
 
 class TiltCorrection(ModelObject):
     """Tilt correction parameters for Z leadscrew compensation"""
     def __init__(self):
@@ -26,15 +26,15 @@
         return self._correction_factor
     
     @correction_factor.setter
     def correction_factor(self, value):
         self._correction_factor = float(value)
         
     @property
-    def last_corrections(self) -> list[float]:
+    def last_corrections(self) -> List[float]:
         """Last corrections (in mm)"""
         return self._last_corrections
 
     @property
     def max_correction(self) -> float:
         """Maximum Z correction (in mm)"""
         return self._max_correction
@@ -49,15 +49,15 @@
         return self._screw_pitch
 
     @screw_pitch.setter
     def screw_pitch(self, value):
         self._screw_pitch = float(value)
         
     @property
-    def screw_x(self) -> list[float]:
+    def screw_x(self) -> List[float]:
         """X positions of the leadscrews (in mm)"""
         return self._screw_x
     
     @property
-    def screw_y(self) -> list[float]:
+    def screw_y(self) -> List[float]:
         """Y positions of the leadscrews (in mm)"""
         return self._screw_y
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/kinematics/zleadscrew_kinematics.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/kinematics/zleadscrew_kinematics.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/microstepping.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/microstepping.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     @property
     def interpolated(self) -> bool:
         """"Indicates if the stepper driver uses interpolation"""
         return self._interpolated
 
     @interpolated.setter
-    def interpolated(self, value: bool):
+    def interpolated(self, value):
         self._interpolated = bool(value)
 
     @property
     def value(self) -> int:
         """Microsteps per full step"""
         return self._value
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/motors_idle_control.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/motors_idle_control.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .axis import Axis
 from .current_move import CurrentMove
 from .extruder import Extruder
 from .keepout_zone import KeepoutZone
 from .kinematics import Kinematics
 from .input_shaping import InputShaping
@@ -55,15 +55,15 @@
         self._travel_acceleration = 0
         # Virtual total extruder position
         self._virtual_e_pos = 0
         # Index of the currently selected workplace
         self._workplace_number = 0
 
     @property
-    def axes(self) -> list[Axis]:
+    def axes(self) -> List[Axis]:
         """List of the configured axes
         See Axis()"""
         return self._axes
 
     @property
     def backlash_factor(self) -> int:
         """Backlash distance multiplier"""
@@ -85,15 +85,15 @@
 
     @property
     def current_move(self) -> CurrentMove:
         """Information about the current move"""
         return self._current_move
 
     @property
-    def extruders(self) -> list[Extruder]:
+    def extruders(self) -> List[Extruder]:
         """List of configured extruders
         See Extruder()"""
         return self._extruders
 
     @property
     def idle(self) -> MotorsIdleControl:
         """Idle current reduction parameters"""
@@ -111,37 +111,37 @@
 
     @property
     def limit_axes(self) -> bool:
         """Limit axis positions by their minima and maxima"""
         return self._limit_axes
 
     @limit_axes.setter
-    def limit_axes(self, value: bool):
+    def limit_axes(self, value):
         self._limit_axes = bool(value)
 
     @property
     def no_moves_before_homing(self) -> bool:
         """Indicates if standard moves are forbidden if the corresponding axis is not homed"""
         return self._no_moves_before_homing
 
     @no_moves_before_homing.setter
-    def no_moves_before_homing(self, value: bool):
+    def no_moves_before_homing(self, value):
         self._no_moves_before_homing = bool(value)
 
     @property
     def printing_acceleration(self) -> float:
         """Maximum acceleration allowed while printing (in mm/s^2)"""
         return self._printing_acceleration
 
     @printing_acceleration.setter
     def printing_acceleration(self, value):
         self._printing_acceleration = float(value)
 
     @property
-    def queue(self) -> list[MoveQueueItem]:
+    def queue(self) -> List[MoveQueueItem]:
         """List of move queue items (DDA rings)"""
         return self._queue
 
     @property
     def rotation(self) -> MoveRotation:
         """Parameters for centre rotation"""
         return self._rotation
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move_calibration.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move_calibration.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move_compensation.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move_compensation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from enum import Enum
+from typing import Union
 
 from .move_calibration import MoveDeviations
 from .probe_grid import ProbeGrid
 from .skew import Skew
 from ..model_object import ModelObject
 from ..utils import wrap_model_property
 
@@ -40,29 +40,29 @@
         self._probe_grid = ProbeGrid()
         # Information about the configured orthogonal axis parameters
         self._skew = Skew()
         # Type of the compensation in use
         self._type = MoveCompensationType.none
 
     @property
-    def fade_height(self) -> float | None:
+    def fade_height(self) -> Union[float, None]:
         """Effective height before the bed compensation is turned off (in mm) or null if not configured"""
         return self._fade_height
 
     @fade_height.setter
-    def fade_height(self, value: float | None = None):
+    def fade_height(self, value):
         self._fade_height = float(value) if value is not None else None
 
     @property
-    def file(self) -> str | None:
+    def file(self) -> Union[str, None]:
         """Full path to the currently used height map file or null if none is in use"""
         return self._file
 
     @file.setter
-    def file(self, value: str | None = None):
+    def file(self, value):
         self._file = str(value) if value is not None else None
 
     @property
     def probe_grid(self) -> ProbeGrid:
         """Probe grid settings as defined by M557"""
         return self._probe_grid
 
@@ -73,15 +73,16 @@
 
     @property
     def type(self) -> MoveCompensationType:
         """Type of the compensation in use"""
         return self._type
 
     @type.setter
-    def type(self, value: MoveCompensationType = MoveCompensationType.none):
-        if isinstance(value, MoveCompensationType):
+    def type(self, value):
+        if value is None or value == "":
+            self._type = MoveCompensationType.none
+        elif isinstance(value, MoveCompensationType):
             self._type = value
         elif isinstance(value, str):
             self._type = MoveCompensationType(value)
         else:
-            raise TypeError(f"{__name__}.type must be of type MoveCompensationType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.type must be of type MoveCompensationType. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move_deviations.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move_deviations.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move_queue_item.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move_queue_item.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move_rotation.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move_rotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from ..model_object import ModelObject
 
 
 class MoveRotation(ModelObject):
     """Information about centre rotation as defined by G68"""
     def __init__(self):
@@ -18,10 +18,10 @@
         return self._angle
 
     @angle.setter
     def angle(self, value):
         self._angle = float(value)
 
     @property
-    def centre(self) -> list[float]:
+    def centre(self) -> List[float]:
         """XY coordinates of the centre rotation"""
         return self._centre
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/move_segmentation.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/move_segmentation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from ..model_object import ModelObject
 
 
 class MoveSegmentation(ModelObject):
     """Move segmentation parameters"""
     def __init__(self):
         super().__init__()
-        self._segments_per_sec = 0
-        self._min_segment_length = 0
+        self._segments_per_sec = 0.0
+        self._min_segment_length = 0.0
         
     @property
-    def segments_per_sec(self) -> int:
+    def segments_per_sec(self) -> float:
         """Number of segments per second"""
         return self._segments_per_sec
     
     @segments_per_sec.setter
     def segments_per_sec(self, value):
-        self._segments_per_sec = int(value)
+        self._segments_per_sec = float(value)
         
     @property
     def min_segment_length(self) -> float:
         """Minimum length of a segment (in mm)"""
         return self._min_segment_length
     
     @min_segment_length.setter
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/probe_grid.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/probe_grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from ..model_object import ModelObject
 
 
 class ProbeGrid(ModelObject):
     """Information about the configured probe grid (see M557)"""
     def __init__(self):
@@ -15,34 +15,34 @@
         self._mins = [0, 0]
         # Probing radius for delta kinematics
         self._radius = 0
         # Spacings between the coordinates
         self._spacings = [0, 0]
 
     @property
-    def axes(self) -> list[str]:
+    def axes(self) -> List[str]:
         """Axis letters of this heightmap"""
         return self._axes
 
     @property
-    def maxs(self) -> list[float]:
+    def maxs(self) -> List[float]:
         """End coordinates of the heightmap"""
         return self._maxs
 
     @property
-    def mins(self) -> list[float]:
+    def mins(self) -> List[float]:
         """Start coordinates of the heightmap"""
         return self._mins
 
     @property
     def radius(self) -> float:
         """Probing radius for delta kinematics"""
         return self._radius
 
     @radius.setter
     def radius(self, value):
         self._radius = float(value)
 
     @property
-    def spacings(self) -> list[float]:
+    def spacings(self) -> List[float]:
         """Spacings between the coordinates"""
         return self._spacings
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/move/skew.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/move/skew.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     @property
     def compensate_XY(self) -> bool:
         """Indicates if the TanXY value is used to compensate X when Y moves (else Y when X moves)"""
         return self._compensate_XY
 
     @compensate_XY.setter
-    def compensate_XY(self, value: bool):
+    def compensate_XY(self, value):
         self._compensate_XY = bool(value)
 
     @property
     def tan_XY(self) -> float:
         """Tangent of the skew angle for the XY or YX axes"""
         return self._tan_XY
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/network/network.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/network/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List, Union
 
 from .network_interface import NetworkInterface
 from ..model_collection import ModelCollection
 from ..model_object import ModelObject
 
 
 class Network(ModelObject):
@@ -23,37 +23,37 @@
         self._hostname = Network.DEFAULT_HOSTNAME
         # List of available network interfaces
         self._interfaces = ModelCollection(NetworkInterface)
         # Name of the machine
         self._name = Network.DEFAULT_NAME
 
     @property
-    def cors_site(self) -> str | None:
+    def cors_site(self) -> Union[str, None]:
         """If this is set, the web server will allow cross-origin requests via the Access-Control-Allow-Origin header"""
         return self._cors_site
 
     @cors_site.setter
-    def cors_site(self, value: str | None = None):
+    def cors_site(self, value):
         self._cors_site = str(value) if value is not None else None
 
     @property
-    def hostname(self) -> str | None:
+    def hostname(self) -> Union[str, None]:
         """Hostname of the machine"""
         return self._hostname
 
     @hostname.setter
-    def hostname(self, value: str | None = None):
+    def hostname(self, value):
         self._hostname = str(value) if value is not None else None
 
     @property
-    def interfaces(self) -> list[NetworkInterface]:
+    def interfaces(self) -> List[NetworkInterface]:
         """List of available network interfaces"""
         return self._interfaces
 
     @property
-    def name(self) -> str | None:
+    def name(self) -> Union[str, None]:
         """Name of the machine"""
         return self._name
 
     @name.setter
-    def name(self, value: str | None = None):
+    def name(self, value):
         self._name = str(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/network/network_interface.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/network/network_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List, Union
 
 from .network_interface_type import NetworkInterfaceType
 from .network_protocol import NetworkProtocol
 from .network_state import NetworkState
 from ..model_object import ModelObject
 
 
@@ -15,121 +15,122 @@
         self._active_protocols = []
         # Actual IPv4 address of the network adapter or null if unknown
         self._actual_IP = ""
         # Configured IPv4 address of the network adapter or null if unknown
         self._configured_IP = ""
         # Configured IPv4 DNS server fo the network adapter or null if unknown
         self._dns_server = ""
-        # Version of the network interface or None if unknown.
+        # Version of the network interface or null if unknown.
         self._firmware_version = ""
         # IPv4 gateway of the network adapter or null if unknown
         self._gateway = ""
         # Physical address of the network adapter or null if unknown
         self._mac = ""
-        # Number of reconnect attempts or None if unknown
+        # Number of reconnect attempts or null if unknown
         self._num_reconnects = None
-        # Signal of the Wi-Fi adapter (only Wi-Fi, in dBm, or None if unknown)
+        # Signal of the Wi-Fi adapter (only Wi-Fi, in dBm, or null if unknown)
         self._signal = None
-        # Speed of the network interface (in MBit, None if unknown, 0 if not connected)
+        # Speed of the network interface (in MBit, null if unknown, 0 if not connected)
         self._speed = None
         # SSID of the Wi-Fi network or null if not applicable
         self._ssid = None
         # State of this network interface or null if unknown
         self._state = None
         # Subnet of the network adapter or null if unknown
         self._subnet = None
         # Type of this network interface
         self._type = NetworkInterfaceType.wifi
         # WiFi country code if this is a WiFi adapter and if the country code can be determined
         self._wifi_country = None
 
     @property
-    def active_protocols(self) -> list[NetworkProtocol]:
+    def active_protocols(self) -> List[NetworkProtocol]:
         """List of active protocols"""
         return self._active_protocols
 
     @property
     def actual_IP(self) -> Union[str, None]:
         """Actual IPv4 address of the network adapter or null if unknown"""
         return self._actual_IP
     
     @actual_IP.setter
-    def actual_IP(self, value: str | None = None):
+    def actual_IP(self, value):
         self._actual_IP = str(value) if value is not None else None
         
     @property
     def configured_IP(self) -> Union[str, None]:
         """Configured IPv4 address of the network adapter or null if unknown"""
         return self._configured_IP
     
     @configured_IP.setter
-    def configured_IP(self, value: str | None = None):
+    def configured_IP(self, value):
         self._configured_IP = str(value) if value is not None else None
         
     @property
     def dns_server(self) -> Union[str, None]:
         """Configured IPv4 DNS server fo the network adapter or null if unknown"""
         return self._dns_server
     
     @dns_server.setter
-    def dns_server(self, value: str | None = None):
+    def dns_server(self, value):
         self._dns_server = str(value) if value is not None else None
         
     @property
-    def firmware_version(self) -> str | None:
-        """Version of the network interface or None if unknown."""
+    def firmware_version(self) -> Union[str, None]:
+        """Version of the network interface or null if unknown.
+        This is primarily intended for the ESP8266-based network interfaces as used on the Duet WiFi"""
         return self._firmware_version
     
     @firmware_version.setter
-    def firmware_version(self, value: str | None = None):
+    def firmware_version(self, value):
         self._firmware_version = str(value) if value is not None else None
         
     @property
     def gateway(self) -> Union[str, None]:
         """IPv4 gateway of the network adapter or null if unknown"""
         return self._gateway
     
     @gateway.setter
-    def gateway(self, value: str | None = None):
+    def gateway(self, value):
         self._gateway = str(value) if value is not None else None
     
     @property
     def mac(self) -> Union[str, None]:
         """Physical address of the network adapter or null if unknown"""
         return self._mac
     
     @mac.setter
-    def mac(self, value: str | None = None):
+    def mac(self, value):
         self._mac = str(value) if value is not None else None
         
     @property
-    def num_reconnects(self) -> int | None:
-        """Number of reconnect attempts or None if unknown"""
+    def num_reconnects(self) -> Union[int, None]:
+        """Number of reconnect attempts or null if unknown"""
         return self._num_reconnects
     
     @num_reconnects.setter
-    def num_reconnects(self, value: int | None = None):
+    def num_reconnects(self, value):
         self._num_reconnects = int(value) if value is not None else None
         
     @property
-    def signal(self) -> int | None:
-        """Signal of the Wi-Fi adapter (only Wi-Fi, in dBm, or None if unknown)"""
+    def signal(self) -> Union[int, None]:
+        """Signal of the Wi-Fi adapter (only Wi-Fi, in dBm, or null if unknown)"""
         return self._signal
     
     @signal.setter
-    def signal(self, value: int | None = None):
+    def signal(self, value):
         self._signal = int(value) if value is not None else None
 
     @property
-    def speed(self) -> int | None:
-        """Speed of the network interface (in MBit, None if unknown, 0 if not connected)"""
+    def speed(self) -> Union[int, None]:
+        """Speed of the network interface (in MBit, null if unknown, 0 if not connected)"""
         return self._speed
 
     @speed.setter
-    def speed(self, value: int | None = None):
+    def speed(self, value):
         self._speed = int(value) if value is not None else None
 
     @property
     def ssid(self) -> Union[str, None]:
         """SSID of the Wi-Fi network or null if not applicable"""
         return self._ssid
 
@@ -139,40 +140,41 @@
     
     @property
     def state(self) -> Union[NetworkState, None]:
         """State of this network interface or null if unknown"""
         return self._state
     
     @state.setter
-    def state(self, value: NetworkState | None = None):
+    def state(self, value):
         if value is None or isinstance(value, NetworkState):
             self._state = value
         elif isinstance(value, str):
             self._state = NetworkState(value)
         else:
-            raise TypeError(f"{__name__}.state must be of type NetworkState or None."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.state must be of type NetworkState. Got {type(value)}: {value}")
         
     @property
     def subnet(self) -> Union[str, None]:
         """Subnet of the network adapter or null if unknown"""
         return self._subnet
     
     @subnet.setter
-    def subnet(self, value: str | None = None):
+    def subnet(self, value):
         self._subnet = str(value) if value is not None else None
         
     @property
     def type(self) -> NetworkInterfaceType:
         """Type of this network interface"""
         return self._type
     
     @type.setter
-    def type(self, value: NetworkInterfaceType = NetworkInterfaceType.wifi):
-        if isinstance(value, NetworkInterfaceType):
+    def type(self, value):
+        if value is None or value == "":
+            self._type = NetworkInterfaceType.wifi
+        elif isinstance(value, NetworkInterfaceType):
             self._type = value
         elif isinstance(value, str):
             self._type = NetworkInterfaceType(value)
         else:
             raise TypeError(f"{__name__}.type must be of type NetworkInterfaceType. Got {type(value)}: {value}")
 
     @property
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/network/network_state.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/network/network_state.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/object_model.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/object_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .model_collection import ModelCollection
 from .model_dictionary import ModelDictionary
 from .model_object import ModelObject
 from .boards import Board
 from .directories import Directories
 from .fans import Fan
@@ -50,27 +50,27 @@
         self._sensors = Sensors()
         self._spindles = ModelCollection(Spindle)
         self._state = State()
         self._tools = ModelCollection(Tool)
         self._volumes = ModelCollection(Volume)
 
     @property
-    def boards(self) -> list[Board]:
+    def boards(self) -> List[Board]:
         """List of connected boards
         The first item represents the main board"""
         return self._boards
 
     @property
     def directories(self) -> Directories:
         """Information about the individual directories
         This may not be available in RepRapFirmware if no mass storages are available"""
         return self._directories
 
     @property
-    def fans(self) -> list[Fan]:
+    def fans(self) -> List[Fan]:
         """List of configured fans
         See also Fan()"""
         return self._fans
 
     @property
     def globals(self) -> dict:
         """Dictionary of global variables vs JSON values
@@ -100,15 +100,15 @@
 
     @property
     def limits(self) -> Limits:
         """Machine configuration limits"""
         return self._limits
 
     @property
-    def messages(self) -> list[Message]:
+    def messages(self) -> List[Message]:
         """Generic messages that do not belong explicitly to codes being executed.
         This includes status messages, generic errors and outputs generated by M118
         See also Message()"""
         return self._messages
 
     @property
     def move(self) -> Move:
@@ -130,26 +130,26 @@
 
     @property
     def sensors(self) -> Sensors:
         """Information about connected sensors including Z-probes and endstops"""
         return self._sensors
 
     @property
-    def spindles(self) -> list[Spindle]:
+    def spindles(self) -> List[Spindle]:
         """List of configured CNC spindles
         See also Spindle()"""
         return self._spindles
 
     @property
     def state(self) -> State:
         """Information about the machine state"""
         return self._state
 
     @property
-    def tools(self) -> list[Tool]:
+    def tools(self) -> List[Tool]:
         """List of configured tools
         See also Tool()"""
         return self._tools
 
     @property
     def volumes(self) -> List[Volume]:
         """List of available mass storages
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/plugins/plugin_manifest.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/plugins/plugin_manifest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 import re
+from typing import List
 
 from .sbc_permissions import SbcPermissions
 from ..model_object import ModelObject
 
 
 class PluginManifest(ModelObject):
     """Information about a third-party plugin"""
@@ -16,17 +16,18 @@
         self._dwc_version = None
         self._homepage = None
         self._id = None
         self._license = "LGPL-3.0-or-later"
         self._name = None
         self._rrf_version = None
         self._sbc_auto_restart = False
+        self._sbc_config_files = []
         self._sbc_dsf_version = None
         self._sbc_executable = None
-        self._sbc_executable_arguments = None
+        self._sbc_executable_arguments = []
         self._sbc_extra_executables = []
         self._sbc_output_redirected = None
         self._sbc_package_dependencies = []
         self._sbc_permissions = []  # Use a list instead of a set to keep insertion order (useful for json serialising)
         self._sbc_plugin_dependencies = []
         self._sbc_python_dependencies = []
         self._sbc_required = None
@@ -46,44 +47,44 @@
     def data(self):
         """Custom plugin data to be populated in the object model (DSF/DWC in SBC mode - or - DWC in standalone mode).
         Before Commands.SetPluginData can be used, corresponding properties must be registered via this property first!
         """
         return self._data
 
     @property
-    def dwc_dependencies(self) -> list[str]:
+    def dwc_dependencies(self) -> List[str]:
         """List of DWC plugins this plugin depends on. Circular dependencies are not supported"""
         return self._dwc_dependencies
 
     @property
-    def dwc_version(self) -> str | None:
+    def dwc_version(self) -> str:
         """Major/minor compatible DWC version"""
         return self._dwc_version
 
     @dwc_version.setter
-    def dwc_version(self, value: str | None = None):
+    def dwc_version(self, value):
         self._dwc_version = str(value) if value is not None else None
         
     @property
-    def homepage(self) -> str | None:
+    def homepage(self) -> str:
         """Link to the plugin homepage or source code repository"""
         return self._homepage
     
     @homepage.setter
-    def homepage(self, value: str | None = None):
+    def homepage(self, value):
         self._homepage = str(value) if value is not None else None
 
     @property
     def id(self) -> str:
         """Identifier of this plugin. May consist of letters and digits only (max length 32 chars)
         For plugins with DWC components, this is the Webpack chunk name too"""
         return self._id
 
     @id.setter
-    def id(self, value: str):
+    def id(self, value):
         if not value:
             raise Exception(f"Invalid plugin identifier: {value}")
 
         value = str(value)
         if value.isspace() or len(value) > 32:
             raise Exception(f"Invalid plugin identifier: {value}")
         for c in value:
@@ -103,154 +104,161 @@
 
     @property
     def name(self) -> str:
         """Name of the plugin. May consist of letters, digits, dashes, and underscores only (max length 64 chars)"""
         return self._name
 
     @name.setter
-    def name(self, value: str):
+    def name(self, value):
         if not value:
             raise Exception(f"Invalid plugin name: {value}")
 
         value = str(value)
         if value.isspace() or len(value) > 64:
             raise Exception(f"Invalid plugin name: {value}")
         for c in value:
             if not c.isalnum() and c != ' ' and c != '-' and c != '_':
                 raise Exception(f"Illegal plugin name: {value}")
 
         self._name = value
 
     @property
-    def rrf_version(self) -> str | None:
+    def rrf_version(self) -> str:
         """Major/minor supported RRF version (optional)"""
         return self._rrf_version
 
     @rrf_version.setter
-    def rrf_version(self, value: str | None = None):
+    def rrf_version(self, value):
         self._rrf_version = str(value) if value is not None else None
 
     @property
     def sbc_auto_restart(self) -> bool:
         """Automatically restart the SBC process when terminated"""
         return self._sbc_auto_restart
 
     @sbc_auto_restart.setter
     def sbc_auto_restart(self, value):
         self._sbc_auto_restart = bool(value)
+        
+    @property
+    def sbc_config_files(self) -> List[str]:
+        """List of files in the sys or virtual SD directory that should not be overwritten on upgrade
+        The file may be specified either relative to 0:/sys directory (e.g. motion.conf) or relative to the
+        virtual SD directory (e.g. sys/motion.conf). Drive indices as in 0:/sys/motion.conf are not allowed!"""
+        return self._sbc_config_files
 
     @property
     def sbc_dsf_version(self) -> str:
         """Required DSF version for the plugin running on the SBC (ignored if there is no SBC executable)"""
         return self._sbc_dsf_version
 
     @sbc_dsf_version.setter
-    def sbc_dsf_version(self, value: str | None = None):
+    def sbc_dsf_version(self, value):
         self._sbc_dsf_version = str(value) if value is not None else None
 
     @property
     def sbc_executable(self) -> str:
         """Filename in the dsf directory used to start the plugin
         A plugin may provide different binaries in subdirectories per architecture.
         Supported architectures are: arm, arm64, x86, x86_64"""
         return self._sbc_executable
 
     @sbc_executable.setter
-    def sbc_executable(self, value: str):
+    def sbc_executable(self, value):
         if value is not None:
             value = str(value)
             if '..' in value:
                 raise Exception(f"Executable must not contain relative file paths: {value}")
         self._sbc_executable = value
 
     @property
-    def sbc_executable_arguments(self) -> str | None:
+    def sbc_executable_arguments(self) -> List[str]:
         """Command-line arguments for the executable"""
         return self._sbc_executable_arguments
 
     @sbc_executable_arguments.setter
-    def sbc_executable_arguments(self, value: str | None = None):
+    def sbc_executable_arguments(self, value):
         self._sbc_executable_arguments = str(value) if value is not None else None
         
     @property
-    def sbc_extra_executables(self) -> list[str]:
+    def sbc_extra_executables(self) -> List[str]:
         """List of other filenames in the dsf directory that should be executable"""
         return self._sbc_extra_executables
 
     @property
     def sbc_output_redirected(self) -> bool:
         """Defines if messages from stdout/stderr are output as generic messages"""
         return self._sbc_output_redirected
     
     @sbc_output_redirected.setter
-    def sbc_output_redirected(self, value: bool):
+    def sbc_output_redirected(self, value):
         self._sbc_output_redirected = bool(value)
 
     @property
-    def sbc_package_dependencies(self) -> list[str]:
+    def sbc_package_dependencies(self) -> List[str]:
         """List of packages this plugin depends on (apt packages in the case of DuetPi)"""
         return self._sbc_package_dependencies
         
     @property
-    def sbc_permissions(self) -> list[SbcPermissions]:
+    def sbc_permissions(self) -> List[SbcPermissions]:
         """List of permissions required by the plugin executable running on the SBC"""
         return self._sbc_permissions
     
     @sbc_permissions.setter
-    def sbc_permissions(self, values: list[SbcPermissions]):
+    def sbc_permissions(self, values):
         permissions = []
         for value in values:
             if isinstance(value, SbcPermissions):
                 permissions.append(value)
             elif isinstance(value, str):
                 permissions.append(SbcPermissions(value))
             else:
                 raise TypeError(f"{__name__}.sbc_permissions must be of type SbcPermissions."
                                 f" Got {type(value)}: {value}")
         self._sbc_permissions = permissions
         
     @property
-    def sbc_plugin_dependencies(self) -> list[str]:
+    def sbc_plugin_dependencies(self) -> List[str]:
         """List of SBC plugins this plugin depends on. Circular dependencies are not supported"""
         return self._sbc_plugin_dependencies
         
     @property
-    def sbc_python_dependencies(self) -> list[str]:
+    def sbc_python_dependencies(self) -> List[str]:
         """List of Python packages this plugin depends on"""
         return self._sbc_python_dependencies
 
     @property
     def sbc_required(self) -> bool:
         """Set to true if an SBC is absolutely required for this plugin"""
         return self._sbc_required
 
     @sbc_required.setter
-    def sbc_required(self, value: bool):
+    def sbc_required(self, value):
         self._sbc_required = bool(value)
         
     @property
-    def tags(self) -> list[str]:
+    def tags(self) -> List[str]:
         """List of general tags for search"""
         return self._tags
 
     @property
     def version(self) -> str:
         """Version of the plugin"""
         return self._version
 
     @version.setter
     def version(self, value):
         self._version = str(value)
 
     @staticmethod
-    def check_version(actual: str, required: str) -> bool:
+    def check_version(actual: str, required: str):
         """Check if the given version satisfies a required version
         :param actual: Actual version
         :param required: Required version
-        :returns: Whether the actual version fulfills the requirement"""
+        :returns: Whether the actual version fulfills teh requirement"""
         split_chars = r'\.|-|\+'
         actual_items = re.split(split_chars, actual)
         required_items = re.split(split_chars, required)
         for actual_idx, required_idx in zip(actual_items, required_items):
             if actual_idx != required_idx:
                 return False
         return True
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/plugins/plugins.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/plugins/plugins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .plugin_manifest import PluginManifest
 
 
 class Plugin(PluginManifest):
     """Class representing a loaded plugin"""
 
@@ -10,25 +10,25 @@
         super(Plugin, self).__init__()
         self._dsf_files = []
         self._dwc_files = []
         self._sd_files = []
         self._pid = -1
 
     @property
-    def dsf_files(self) -> list[str]:
+    def dsf_files(self) -> List[str]:
         """List of files for the DSF plugin"""
         return self._dsf_files
 
     @property
-    def dwc_files(self) -> list[str]:
+    def dwc_files(self) -> List[str]:
         """List of files for the DWC plugin"""
         return self._dwc_files
 
     @property
-    def sd_files(self) -> list[str]:
+    def sd_files(self) -> List[str]:
         """List of files to be installed to the (virtual) SD excluding web files"""
         return self._sd_files
 
     @property
     def pid(self) -> int:
         """Process ID of the plugin or -1 if not started. It is set to 0 while the plugin is being shut down"""
         return self._pid
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/plugins/sbc_permissions.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/plugins/sbc_permissions.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/dsf.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/dsf.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class DSF(ModelObject):
     """Information about Duet Software Framework"""
 
     def __init__(self):
         super().__init__()
         self._build_date_time = ""
         self._http_endpoints = ModelCollection(HttpEndpoint)
+        self._is64bit = False
         self._plugin_support = False
         self._root_plugin_support = False
         self._user_sessions = ModelCollection(UserSession)
         self._version = ""
 
     @property
     def build_date_time(self) -> str:
@@ -24,14 +25,23 @@
         return self._build_date_time
 
     @build_date_time.setter
     def build_date_time(self, value):
         self._build_date_time = str(value)
 
     @property
+    def is64bit(self) -> bool:
+        """Indicates if the process is 64-bit"""
+        return self._is64bit
+
+    @is64bit.setter
+    def is64bit(self, value):
+        self._is64bit = bool(value)
+
+    @property
     def http_endpoints(self) -> List[HttpEndpoint]:
         """List of registered third-party HTTP endpoints"""
         return self._http_endpoints
 
     @property
     def plugin_support(self) -> bool:
         """Indicates if DSF allows the installation and usage of third-party plugins"""
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/http_endpoint.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/http_endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,32 +22,31 @@
 
     @property
     def endpoint_type(self) -> HttpEndpointType:
         """HTTP type of this endpoint"""
         return self._endpoint_type
 
     @endpoint_type.setter
-    def endpoint_type(self, value: HttpEndpointType):
+    def endpoint_type(self, value):
         if isinstance(value, HttpEndpointType):
             self._endpoint_type = value
         elif isinstance(value, str):
             self._endpoint_type = HttpEndpointType(value)
         else:
-            raise TypeError(f"{__name__}.endpoint_type must be of type HttpEndpointType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.endpoint_type must be of type HttpEndpointType. Got {type(value)}: {value}")
 
     @property
     def is_upload_request(self) -> bool:
         """Whether this is an upload request
         If set to true, the whole body payload is written to a temporary file
         and the file path is passed via the Commands.ReceivedHttpRequest.Body property"""
         return self._is_upload_request
 
     @is_upload_request.setter
-    def is_upload_request(self, value: bool):
+    def is_upload_request(self, value):
         self._is_upload_request = bool(value)
 
     @property
     def namespace(self) -> str:
         """Namespace of the endpoint"""
         return self._namespace
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/http_endpoint_type.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/http_endpoint_type.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sbc/dsf/user_sessions/user_sessions.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/dsf/user_sessions/user_sessions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from .access_level import AccessLevel
 from .session_type import SessionType
 from ....model_object import ModelObject
 
 
 class UserSession(ModelObject):
@@ -22,39 +22,33 @@
         
     @property
     def access_level(self) -> AccessLevel:
         """Access level of this session"""
         return self._access_level
     
     @access_level.setter
-    def access_level(self, value: AccessLevel):
-        if isinstance(value, AccessLevel):
-            self._access_level = value
-        elif isinstance(value, str):
-            self._access_level = AccessLevel(value)
-        else:
-            raise TypeError(f"{__name__}.access_level must be of type AccessLevel."
-                            f" Got {type(value)}: {value}")
+    def access_level(self, value):
+        self._access_level = value
         
     @property
     def id(self) -> int:
         """Identifier of this session"""
         return self._id
     
     @id.setter
     def id(self, value):
         self._id = int(value)
         
     @property
-    def origin(self) -> str | None:
+    def origin(self) -> Union[str, None]:
         """Origin of this session. For remote sessions, this equals the remote IP address"""
         return self._origin
     
     @origin.setter
-    def origin(self, value: str | None = None):
+    def origin(self, value):
         self._origin = str(value) if value is not None else None
         
     @property
     def origin_id(self) -> int:
         """Corresponding identifier of the origin.
         If it is a remote session, it is the remote port, else it defaults to the PID of the current process"""
         return self._origin_id
@@ -65,15 +59,16 @@
         
     @property
     def session_type(self) -> SessionType:
         """Type of this session"""
         return self._session_type
     
     @session_type.setter
-    def session_type(self, value: SessionType):
-        if isinstance(value, SessionType):
+    def session_type(self, value):
+        if value is None or value == "":
+            self._session_type = SessionType.local
+        elif isinstance(value, SessionType):
             self._session_type = value
         elif isinstance(value, str):
             self._session_type = SessionType(value)
         else:
-            raise TypeError(f"{__name__}.session_type must be of type SessionType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.session_type must be of type SessionType. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sbc/memory.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/memory.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sbc/sbc.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sbc/sbc.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/analog_sensor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/analog_sensor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from .analog_sensor_type import AnalogSensorType
 from .temperature_error import TemperatureError
 from ..model_object import ModelObject
 
 
 class AnalogSensor(ModelObject):
@@ -10,17 +10,19 @@
 
     def __init__(self):
         super(AnalogSensor, self).__init__()
         self._beta = None
         self._c = None
         self._last_reading = None
         self._name = None
+        self._offset_adj = 0.0
         self._port = None
         self._r_25 = None
         self._r_ref = None
+        self._slope_adj = 0.0
         self._state = TemperatureError.ok
         self._type = AnalogSensorType.Unknown
 
     @property
     def beta(self) -> Union[float, None]:
         """Beta value of this sensor (if applicable)"""
         return self._beta
@@ -40,25 +42,35 @@
 
     @property
     def last_reading(self) -> Union[float, None]:
         """Last sensor reading (in C) or null if invalid"""
         return self._last_reading
     
     @last_reading.setter
-    def last_reading(self, value: float | None = None):
+    def last_reading(self, value):
         self._last_reading = float(value) if value is not None else None
         
     @property
-    def name(self) -> str | None:
+    def name(self) -> Union[str, None]:
         """Name of this sensor or null if not configured"""
         return self._name
     
     @name.setter
-    def name(self, value: str | None = None):
+    def name(self, value):
         self._name = str(value) if value is not None else None
+        
+    @property
+    def offset_adj(self) -> float:
+        """Offset adjustment (in K)
+        See also M308 U"""
+        return self._offset_adj
+    
+    @offset_adj.setter
+    def offset_adj(self, value):
+        self._offset_adj = float(value)
 
     @property
     def port(self) -> Union[str, None]:
         """Port of this sensor or None if not applicable"""
         return self._port
 
     @port.setter
@@ -80,14 +92,24 @@
         return self._r_ref
 
     @r_ref.setter
     def r_ref(self, value):
         self._r_ref = float(value) if value is not None else None
 
     @property
+    def slope_adj(self) -> float:
+        """Slope adjustment factor
+        See also M308 V"""
+        return self._slope_adj
+
+    @slope_adj.setter
+    def slope_adj(self, value):
+        self._slope_adj = float(value)
+
+    @property
     def state(self) -> TemperatureError:
         """State of this sensor"""
         return self._state
 
     @state.setter
     def state(self, value):
         if isinstance(value, TemperatureError):
@@ -105,9 +127,8 @@
         if value is None:
             self._type = AnalogSensorType.Unknown
         elif isinstance(value, AnalogSensorType):
             self._type = value
         elif isinstance(value, str):
             self._type = AnalogSensorType(value)
         else:
-            raise TypeError(f"{__name__}.type must be of type AnalogSensorType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.type must be of type AnalogSensorType or None. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/analog_sensor_type.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/analog_sensor_type.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/endstop.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/endstop.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     @property
     def high_end(self) -> bool:
         """Whether this endstop is at the high end of the axis"""
         return self._high_end
 
     @high_end.setter
-    def high_end(self, value: bool):
+    def high_end(self, value):
         self._high_end = bool(value)
 
     @property
     def probe(self) -> Union[int, None]:
         """Number of the referenced probe if type is ZProbeAsEndstop, else None"""
         return self._probe
 
@@ -34,24 +34,23 @@
 
     @property
     def triggered(self) -> bool:
         """Whether the endstop is hit"""
         return self._triggered
 
     @triggered.setter
-    def triggered(self, value: bool):
+    def triggered(self, value):
         self._triggered = bool(value)
 
     @property
     def type(self) -> EndstopType:
         """Type of the endstop"""
         return self._type
 
     @type.setter
-    def type(self, value: EndstopType):
-        if isinstance(value, EndstopType):
+    def type(self, value):
+        if value is None or isinstance(value, EndstopType):
             self._type = value
         elif isinstance(value, str):
             self._type = EndstopType(value)
         else:
-            raise TypeError(f"{__name__}.type must be of type EndstopType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.type must be of type EndstopType or None. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/Duet3DFilamentMonitor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/Duet3DFilamentMonitor.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/__init__.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/__init__.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/filament_monitor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/filament_monitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,28 +36,27 @@
     @deprecated(f"Use {__name__}.enable_mode instead")
     def enabled(self) -> bool:
         """Indicates if this filament monitor is enabled
         Deprecated: Use enable_mode instead"""
         return self._enabled
 
     @enabled.setter
-    def enabled(self, value: bool):
+    def enabled(self, value):
         self._enabled = bool(value)
 
     @staticmethod
-    def get_filament_monitor(type_: FilamentMonitorType) -> 'FilamentMonitor':
+    def get_filament_monitor(type_: FilamentMonitorType):
         from .laser_filament_monitor import LaserFilamentMonitor
         from .pulsed_filament_monitor import PulsedFilamentMonitor
         from .rotating_magnet_filament_monitor import RotatingMagnetFilamentMonitor
 
         if isinstance(type_, str):
             type_ = FilamentMonitorType(type_)
         elif not isinstance(type_, FilamentMonitorType):
-            raise TypeError(f"type must be of type FilamentMonitorType."
-                            f" Got {type(type_)}: {type_}")
+            raise TypeError(f"type must be of type FilamentMonitorType. Got {type(type_)}: {type_}")
 
         if type_ == FilamentMonitorType.Laser:
             return LaserFilamentMonitor()
         elif type_ == FilamentMonitorType.Pulsed:
             return PulsedFilamentMonitor()
         elif type_ == FilamentMonitorType.RotatingMagnet:
             return RotatingMagnetFilamentMonitor()
@@ -66,29 +65,30 @@
 
     @property
     def status(self) -> FilamentMonitorStatus:
         """Last reported status of this filament monitor"""
         return self._status
 
     @status.setter
-    def status(self, value: FilamentMonitorStatus = FilamentMonitorStatus.NoDataReceived):
-        if isinstance(value, FilamentMonitorStatus):
+    def status(self, value):
+        if value is None:
+            self._status = FilamentMonitorStatus.NoDataReceived
+        elif isinstance(value, FilamentMonitorStatus):
             self._status = value
         elif isinstance(value, str):
             self._status = FilamentMonitorStatus(value)
         else:
-            raise TypeError(f"{__name__}.status must be of type FilamentMonitorStatus."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.status must be of type FilamentMonitorStatus. Got {type(value)}: {value}")
 
     @property
     def type(self) -> FilamentMonitorType:
         """Type of this filament monitor"""
         return self._type
 
-    def _update_from_json(self, **kwargs) -> 'FilamentMonitor':
+    def _update_from_json(self, **kwargs):
         """Override ObjectModel._update_from_json to return the FilamentMonitorType type matching the given type"""
         if 'type_' in kwargs and self.type != FilamentMonitorType(kwargs.get('type_')):
             required_type = self.get_filament_monitor(kwargs.get('type_'))
             new_filament_monitor = required_type.update_from_json(kwargs)
             return new_filament_monitor
 
         super(FilamentMonitor, self)._update_from_json(**kwargs)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/filament_monitor_status.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/filament_monitor_status.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/laser_filament_monitor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/laser_filament_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Union
 
 from .Duet3DFilamentMonitor import Duet3DFilamentMonitor
 from .filament_monitor_type import FilamentMonitorType
 from ...model_object import ModelObject
 from ...utils import wrap_model_property
 
 
@@ -75,15 +75,15 @@
 
     @property
     def all_moves(self) -> bool:
         """Whether all moves and not only printing moves are supposed to be checked"""
         return self._all_moves
 
     @all_moves.setter
-    def all_moves(self, value: bool):
+    def all_moves(self, value):
         self._all_moves = bool(value)
 
     @property
     def percent_max(self) -> float:
         """Maximum percentage (0..1 or greater)"""
         return self._percent_max
 
@@ -125,14 +125,14 @@
 
     @property
     def configured(self) -> LaserFilamentMonitorConfigured:
         """Configured properties of this filament monitor"""
         return self._configured
 
     @property
-    def filament_present(self) -> bool | None:
+    def filament_present(self) -> Union[bool, None]:
         """Indicates if a filament is present"""
         return self._filament_present
 
     @filament_present.setter
-    def filament_present(self, value: bool | None = None):
+    def filament_present(self, value):
         self._filament_present = bool(value) if value is not None else None
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/pulsed_filament_monitor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/pulsed_filament_monitor.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/filament_monitors/rotating_magnet_filament_monitor.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/filament_monitors/rotating_magnet_filament_monitor.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/probe.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/probe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Optional
 
 from .probe_type import ProbeType
 from ..model_object import ModelObject
 from ...utils import deprecated
 
 
 class Probe(ModelObject):
@@ -16,37 +16,38 @@
         self._deployed_by_user = False
         self._disables_heaters = False
         self._dive_height = 5
         self._dive_heights = [0, 0]
         self._is_calibrated = None
         self._last_stop_height = 0
         self._max_probe_count = 1
+        self._measured_height = None
         self._offsets = [0, 0]
         self._recovery_time = 0
         self._scan_coefficients = None
         self._speeds = [2, 2]
         self._temperature_coefficients = [0, 0]
         self._threshold = 500
         self._tolerance = 0.03
         self._travel_speed = 6000
         self._trigger_height = 0.7
         self._type = ProbeType.NoProbe
         self._value = []
 
     @property
-    def calib_a(self) -> Union[float, None]:
+    def calib_a(self) -> Optional[float]:
         """Linear coefficient for scanning probes"""
         return self._calib_a
 
     @calib_a.setter
     def calib_a(self, value):
         self._calib_a = float(value) if value is not None else None
 
     @property
-    def calib_b(self) -> Union[float, None]:
+    def calib_b(self) -> Optional[float]:
         """Quadratic coefficient for scanning probes"""
         return self._calib_b
 
     @calib_b.setter
     def calib_b(self, value):
         self._calib_b = float(value) if value is not None else None
 
@@ -61,24 +62,24 @@
         
     @property
     def deployed_by_user(self) -> bool:
         """Indicates if the user has deployed the probe"""
         return self._deployed_by_user
     
     @deployed_by_user.setter
-    def deployed_by_user(self, value: bool):
+    def deployed_by_user(self, value):
         self._deployed_by_user = bool(value)
         
     @property
     def disables_heaters(self) -> bool:
         """Whether probing disables the heater(s)"""
         return self._disables_heaters
     
     @disables_heaters.setter
-    def disables_heaters(self, value: bool):
+    def disables_heaters(self, value):
         self._disables_heaters = bool(value)
         
     @property
     @deprecated(f"Use {__name__}.dive_heights[0] instead")
     def dive_height(self) -> float:
         """Dive height (in mm)
         Deprecated: Use dive_heights[0] instead
@@ -93,15 +94,15 @@
     def dive_heights(self) -> List[float]:
         """Dive heights of the probe.
         The first element is the regular dive height, the second element may be used by scanning Z-probes
         """
         return self._dive_heights
 
     @property
-    def is_calibrated(self) -> Union[bool, None]:
+    def is_calibrated(self) -> Optional[bool]:
         """Indicates if the scanning probe is calibrated"""
         return self._is_calibrated
 
     @is_calibrated.setter
     def is_calibrated(self, value):
         self._is_calibrated = bool(value) if value is not None else None
         
@@ -120,15 +121,24 @@
         return self._max_probe_count
     
     @max_probe_count.setter
     def max_probe_count(self, value):
         self._max_probe_count = int(value)
         
     @property
-    def offsets(self) -> list[float]:
+    def measured_height(self) -> Optional[float]:
+        """Measured height (only applicable for scanning probes, in mm or null)"""
+        return self._measured_height
+    
+    @measured_height.setter
+    def measured_height(self, value):
+        self._measured_height = None if value is None else float(value)
+        
+    @property
+    def offsets(self) -> List[float]:
         """X+Y offsets (in mm)"""
         return self._offsets
     
     @property
     def recovery_time(self) -> float:
         """Recovery time (in s)"""
         return self._recovery_time
@@ -140,33 +150,34 @@
     @property
     def speed(self) -> float:
         """Probe speed (in mm/s)
         Obsolete: Use Speeds[0] instead"""
         return self._speeds[0]
 
     @property
-    def scan_coefficients(self) -> Union[List[float], None]:
+    def scan_coefficients(self) -> Optional[List[float]]:
         """Coefficients for the scanning Z-probe (4 elements, if applicable)"""
         return self._scan_coefficients
 
     @scan_coefficients.setter
     def scan_coefficients(self, value):
         self._scan_coefficients = None if value is None else [float(v) for v in value]
         
     @property
-    def speeds(self) -> list[float]:
-        """Fast and slow probing speeds (in mm/s)"""
+    def speeds(self) -> List[float]:
+        """Fast and slow probing speeds (in mm/s)
+        Scanning probes may have three speeds where the last one is the movement speed while probing heightmaps"""
         return self._speeds
     
     @speeds.setter
     def speeds(self, values):
         self._speeds = [float(value) for value in values]
         
     @property
-    def temperature_coefficients(self) -> list[float]:
+    def temperature_coefficients(self) -> List[float]:
         """List of temperature coefficients"""
         return self._temperature_coefficients
         
     @property
     def threshold(self) -> int:
         """Configured trigger threshold (0..1023)"""
         return self._threshold
@@ -205,20 +216,19 @@
     @property
     def type(self) -> ProbeType:
         """Type of the configured probe
         See also ProbeType"""
         return self._type
     
     @type.setter
-    def type(self, value: ProbeType):
-        if isinstance(value, ProbeType):
+    def type(self, value):
+        if value is None or isinstance(value, ProbeType):
             self._type = value
         elif isinstance(value, int):
             self._type = ProbeType(value)
         else:
-            raise TypeError(f"{__name__}.type must be of type ProbeType."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.type must be of type ProbeType or None. Got {type(value)}: {value}")
         
     @property
     def value(self) -> List[int]:
         """Current analog values of the probe"""
         return self._value
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/probe_type.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/probe_type.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/sensors.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/sensors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .analog_sensor import AnalogSensor
 from .endstop import Endstop
 from .filament_monitors import FilamentMonitor
 from .gp_input_port import GpInputPort
 from .probe import Probe
 from ..model_collection import ModelCollection
@@ -17,30 +17,30 @@
         self._analog = ModelCollection(AnalogSensor)
         self._endstops = ModelCollection(Endstop)
         self._filament_monitors = ModelCollection(FilamentMonitor)
         self._gp_in = ModelCollection(GpInputPort)
         self._probes = ModelCollection(Probe)
 
     @property
-    def analog(self) -> list[AnalogSensor]:
+    def analog(self) -> List[AnalogSensor]:
         """List of analog sensors"""
         return self._analog
 
     @property
-    def endstops(self) -> list[Endstop]:
+    def endstops(self) -> List[Endstop]:
         """List of configured endstops"""
         return self._endstops
 
     @property
-    def filament_monitors(self) -> list[FilamentMonitor]:
+    def filament_monitors(self) -> List[FilamentMonitor]:
         """List of configured filament monitors"""
         return self._filament_monitors
 
     @property
-    def gp_in(self) -> list[GpInputPort]:
+    def gp_in(self) -> List[GpInputPort]:
         """List of general-purpose input ports"""
         return self._gp_in
 
     @property
-    def probes(self) -> list[Probe]:
+    def probes(self) -> List[Probe]:
         """"""
         return self._probes
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/sensors/temperature_error.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/sensors/temperature_error.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/spindles/spindles.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/spindles/spindles.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         
     @property
     def state(self) -> SpindleState:
         """Current state"""
         return self._state
     
     @state.setter
-    def state(self, value: SpindleState = SpindleState.unconfigured):
-        if isinstance(value, SpindleState):
-            self._state = value
+    def state(self, value):
+        if value is None or value == "":
+            self._state = SpindleState.unconfigured
         elif isinstance(value, str):
             self._state = SpindleState(value)
+        elif isinstance(value, SpindleState):
+            self._state = value
         else:
-            raise TypeError(f"{__name__}.state must be of type SpindleState."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.state must be of type SpindleState. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/beep_request.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/beep_request.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/gp_output_port.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/gp_output_port.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/machine_status.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/machine_status.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/message_box.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/message_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         
     @property
     def message(self) -> str:
         """Content of the message box"""
         return self._message
     
     @message.setter
-    def message(self, value: str):
+    def message(self, value):
         self._message = str(value)
 
     @property
     def min(self) -> float:
         """Minimum input value (only for modes >= 5)"""
         return self._min
 
@@ -123,24 +123,25 @@
         
     @property
     def mode(self) -> MessageBoxMode:
         """Mode of the message box to display"""
         return self._mode
     
     @mode.setter
-    def mode(self, value: MessageBoxMode):
-        if isinstance(value, MessageBoxMode):
+    def mode(self, value):
+        if value is None:
+            self._mode = MessageBoxMode.OkOnly
+        elif isinstance(value, MessageBoxMode):
             self._mode = value
         elif isinstance(value, int):
             self._mode = MessageBoxMode(value)
         elif isinstance(value, str):
             self._mode = MessageBoxMode[value]
         else:
-            raise TypeError(f"{__name__}.mode must be of type MessageBoxMode."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.mode must be of type MessageBoxMode. Got {type(value)}: {value}")
         
     @property
     def seq(self) -> int:
         """Sequence number of the message box
         This is increased whenever a new message box is supposed to be displayed"""
         return self._seq
     
@@ -159,9 +160,9 @@
         
     @property
     def title(self) -> str:
         """Title of the message box"""
         return self._title
     
     @title.setter
-    def title(self, value: str):
+    def title(self, value):
         self._title = str(value)
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/restore_point.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/restore_point.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List, Union
 
 from ..model_object import ModelObject
 
 
 class RestorePoint(ModelObject):
     """
     Class holding information about a restore point
@@ -22,15 +22,15 @@
         self._io_bits = None
         # Laser PWM value (0..1) or null if not applicable
         self._laser_pwm = None
         # The tool number that was active
         self._tool_number = -1
         
     @property
-    def coords(self) -> list[float]:
+    def coords(self) -> List[float]:
         """Axis coordinates of the restore point (in mm)"""
         return self._coords
     
     @property
     def extruder_pos(self) -> float:
         """The virtual extruder position at the start of this move"""
         return self._extruder_pos
@@ -54,29 +54,29 @@
         return self._feed_rate
     
     @feed_rate.setter
     def feed_rate(self, value):
         self._feed_rate = float(value)
         
     @property
-    def io_bits(self) -> int | None:
+    def io_bits(self) -> Union[int, None]:
         """The output port bits setting for this move or null if not applicable"""
         return self._io_bits
     
     @io_bits.setter
-    def io_bits(self, value: int | None = None):
+    def io_bits(self, value):
         self._io_bits = int(value) if value is not None else None
         
     @property
-    def laser_pwm(self) -> float | None:
+    def laser_pwm(self) -> Union[float, None]:
         """Laser PWM value (0..1) or null if not applicable"""
         return self._laser_pwm
     
     @laser_pwm.setter
-    def laser_pwm(self, value: float | None = None):
+    def laser_pwm(self, value):
         self._laser_pwm = float(value) if value is not None else None
     
     @property
     def tool_number(self) -> int:
         """The tool number that was active"""
         return self._tool_number
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/startup_error.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/startup_error.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/state/state.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/state/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from __future__ import annotations
 from datetime import datetime
+from typing import List, Union
 
 from .beep_request import BeepRequest
 from .gp_output_port import GpOutputPort
 from .log_level import LogLevel
 from .machine_mode import MachineMode
 from .machine_status import MachineStatus
 from .message_box import MessageBox
@@ -49,119 +49,117 @@
         self._status = MachineStatus.starting
         self._this_active = True
         self._this_input = None
         self._time = None
         self._up_time = 0
 
     @property
-    def atx_power(self) -> bool | None:
+    def atx_power(self) -> Union[bool, None]:
         """State of the ATX power pin (if controlled)"""
         return self._atx_power
 
     @atx_power.setter
-    def atx_power(self, value: bool | None = None):
+    def atx_power(self, value):
         self._atx_power = bool(value) if value is not None else None
 
     @property
-    def atx_power_port(self) -> str | None:
+    def atx_power_port(self) -> Union[str, None]:
         """Port of the ATX power pin or null if not assigned"""
         return self._atx_power_port
 
     @atx_power_port.setter
-    def atx_power_port(self, value: str | None = None):
+    def atx_power_port(self, value):
         self._atx_power_port = str(value) if value is not None else None
 
     @property
     def current_tool(self) -> int:
         """Number of the currently selected tool or -1 if none is selected"""
         return self._current_tool
 
     @current_tool.setter
     def current_tool(self, value):
         self._current_tool = int(value)
 
     @property
-    def deferred_power_down(self) -> bool | None:
+    def deferred_power_down(self) -> Union[bool, None]:
         """When provided it normally has value 0 normally and 1 when a deferred power down is pending
         It is only available after power switching has been enabled by M80 or M81"""
         return self._deferred_power_down
 
     @deferred_power_down.setter
-    def deferred_power_down(self, value: bool | None = None):
+    def deferred_power_down(self, value):
         self._deferred_power_down = bool(value) if value is not None else None
 
     @property
     def display_message(self) -> str:
         """Persistent message to display (see M117)"""
         return self._display_message
 
     @display_message.setter
     def display_message(self, value):
         self._display_message = str(value)
 
     @property
-    def gp_out(self) -> list[GpOutputPort]:
+    def gp_out(self) -> List[GpOutputPort]:
         """List of general-purpose output ports"""
         return self._gp_out
 
     @property
-    def laser_pwm(self) -> float | None:
+    def laser_pwm(self) -> Union[float, None]:
         """Laser PWM of the next commanded move (0..1) or null if not applicable"""
         return self._laser_pwm
 
     @laser_pwm.setter
-    def laser_pwm(self, value: float | None = None):
+    def laser_pwm(self, value):
         self._laser_pwm = float(value) if value is not None else None
 
     @property
-    def log_file(self) -> str | None:
+    def log_file(self) -> Union[str, None]:
         """Log file being written to or null if logging is disabled"""
         return self._log_file
 
     @log_file.setter
-    def log_file(self, value: str | None = None):
+    def log_file(self, value):
         self._log_file = str(value) if value is not None else None
 
     @property
-    def log_level(self) -> LogLevel:
+    def log_level(self) -> Union[LogLevel, None]:
         """Current log level"""
         return self._log_level
 
     @log_level.setter
-    def log_level(self, value: LogLevel):
-        if isinstance(value, LogLevel):
+    def log_level(self, value):
+        if value is None or isinstance(value, LogLevel):
             self._log_level = value
         elif isinstance(value, str):
             self._log_level = LogLevel(value)
         else:
-            raise TypeError(f"{__name__}.log_level must be of type LogLevel."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.log_level must be of type LogLevel or None. Got {type(value)}: {value}")
 
     @property
-    def machine_mode(self) -> MachineMode:
+    def machine_mode(self) -> Union[MachineMode, None]:
         """Current mode of operation"""
         return self._machine_mode
 
     @machine_mode.setter
-    def machine_mode(self, value: MachineMode):
-        if isinstance(value, MachineMode):
+    def machine_mode(self, value):
+        if value is None or isinstance(value, MachineMode):
             self._machine_mode = value
         elif isinstance(value, str):
             self._machine_mode = MachineMode(value)
         else:
-            raise TypeError(f"{__name__}.machine_mode must be of type MachineMode."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.machine_mode must be of type MachineMode or None. Got {type(value)}: {value}")
 
     @property
     def macro_restarted(self) -> bool:
         """Indicates if the current macro file was restarted after a pause"""
         return self._macro_restarted
 
     @macro_restarted.setter
-    def macro_restarted(self, value: bool):
+    def macro_restarted(self, value):
         self._macro_restarted = bool(value)
 
     @property
     def ms_up_time(self) -> int:
         """Millisecond fraction of `uptime`"""
         return self._ms_up_time
 
@@ -180,54 +178,53 @@
 
     @property
     def plugins_started(self) -> bool:
         """Indicates if at least one plugin has been started"""
         return self._plugins_started
 
     @plugins_started.setter
-    def plugins_started(self, value: bool):
+    def plugins_started(self, value):
         self._plugins_started = bool(value)
 
     @property
     def power_fail_script(self) -> str:
         """Script to execute when the power fails"""
         return self._power_fail_script
 
     @power_fail_script.setter
-    def power_fail_script(self, value: str):
+    def power_fail_script(self, value):
         self._power_fail_script = str(value)
 
     @property
     def previous_tool(self) -> int:
         """Number of the previous tool"""
         return self._previous_tool
 
     @previous_tool.setter
     def previous_tool(self, value):
         self._previous_tool = int(value)
 
     @property
-    def restore_points(self) -> list[RestorePoint]:
+    def restore_points(self) -> List[RestorePoint]:
         """List of restore points"""
         return self._restore_points
 
     @property
-    def status(self) -> MachineStatus:
+    def status(self) -> Union[MachineStatus, None]:
         """Current state of the machine"""
         return self._status
 
     @status.setter
-    def status(self, value: MachineStatus):
-        if isinstance(value, MachineStatus):
+    def status(self, value):
+        if value is None or isinstance(value, MachineStatus):
             self._status = value
         elif isinstance(value, str):
             self._status = MachineStatus(value)
         else:
-            raise TypeError(f"{__name__}.status must be of type MachineStatus."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.status must be of type MachineStatus or None. Got {type(value)}: {value}")
 
     @property
     def this_active(self) -> bool:
         """Shorthand for inputs[state.thisInput].active"""
         return self._this_active
 
     @this_active.setter
@@ -238,24 +235,24 @@
     def this_input(self) -> Union[int, None]:
         """Index of the current G-code input channel (see ObjectModel.Inputs)
         This is primarily intended for macro files to determine on which G-code channel it is running.
         The value of this property is always null in object model queries"""
         return self._this_input
 
     @this_input.setter
-    def this_input(self, value: int | None = None):
+    def this_input(self, value):
         self._this_input = int(value) if value is not None else None
 
     @property
-    def time(self) -> datetime | None:
+    def time(self) -> Union[datetime, None]:
         """Internal date and time in RepRapFirmware or null if unknown"""
         return self._time
 
     @time.setter
-    def time(self, value: str | None = None):
+    def time(self, value):
         self._time = datetime.fromisoformat(value) if value is not None else None
 
     @property
     def up_time(self) -> int:
         """How long the machine has been running (in s)"""
         return self._up_time
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/tools/tool_retraction.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/tools/tool_retraction.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/tools/tools.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import List
 
 from .tool_state import ToolState
 from .tool_retraction import ToolRetraction
 from ..model_object import ModelObject
 
 
 class Tool(ModelObject):
@@ -44,36 +44,36 @@
         self._spindle_rpm = 0
         # Standby temperatures of the associated heaters (in C)
         self._standby = []
         # Current state of this tool
         self._state = ToolState.off
         
     @property
-    def active(self) -> list[float]:
+    def active(self) -> List[float]:
         """Active temperatures of the associated heaters (in C)"""
         return self._active
 
     @property
-    def axes(self) -> list[int]:
+    def axes(self) -> List[int]:
         """Associated axes. At present only X and Y can be mapped per tool.
         The order is the same as the visual axes, so by default the layout is
         [
             [0],    // X
             [1]     // Y
         ]
         Make sure to set each item individually so the change events are called"""
         return self._axes
 
     @property
-    def extruders(self) -> list[int]:
+    def extruders(self) -> List[int]:
         """Extruder drives of this tool"""
         return self._extruders
 
     @property
-    def fans(self) -> list[int]:
+    def fans(self) -> List[int]:
         """List of associated fans (indices)"""
         return self._fans
     
     @property
     def feed_forward(self) -> List[float]:
         """Feedforward coefficients to apply to the mapped heaters during extrusions"""
         return self._feed_forward
@@ -84,29 +84,29 @@
         return self._filament_extruder
     
     @filament_extruder.setter
     def filament_extruder(self, value):
         self._filament_extruder = int(value)
         
     @property
-    def heaters(self) -> list[int]:
+    def heaters(self) -> List[int]:
         """List of associated heaters (indices)"""
         return self._heaters
     
     @property
     def is_retracted(self) -> bool:
         """True if the filament has been firmware-retracted"""
         return self._is_retracted
     
     @is_retracted.setter
-    def is_retracted(self, value: bool):
+    def is_retracted(self, value):
         self._is_retracted = bool(value)
         
     @property
-    def mix(self) -> list[float]:
+    def mix(self) -> List[float]:
         """Mix ratios of the associated extruder drives"""
         return self._mix
     
     @property
     def name(self) -> str:
         """Name of this tool"""
         return self._name
@@ -121,15 +121,15 @@
         return self._number
     
     @number.setter
     def number(self, value):
         self._number = int(value)
         
     @property
-    def offsets(self) -> list[float]:
+    def offsets(self) -> List[float]:
         """Axis offsets (in mm)
         This list is in the same order as Move.Axes"""
         return self._offsets
     
     @property
     def offsets_probed(self) -> int:
         """Bitmap of the probed axis offsets"""
@@ -159,25 +159,26 @@
         return self._spindle_rpm
     
     @spindle_rpm.setter
     def spindle_rpm(self, value):
         self._spindle_rpm = int(value)
         
     @property
-    def standby(self) -> list[float]:
+    def standby(self) -> List[float]:
         """Standby temperatures of the associated heaters (in C)"""
         return self._standby
     
     @property
     def state(self) -> ToolState:
         """Current state of this tool"""
         return self._state
     
     @state.setter
-    def state(self, value: ToolState):
-        if isinstance(value, ToolState):
+    def state(self, value):
+        if value is None or value == "":
+            self._state = ToolState.off
+        elif isinstance(value, ToolState):
             self._state = value
         elif isinstance(value, str):
             self._state = ToolState(value)
         else:
-            raise TypeError(f"{__name__}.state must be of type ToolState."
-                            f" Got {type(value)}: {value}")
+            raise TypeError(f"{__name__}.state must be of type ToolState. Got {type(value)}: {value}")
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/object_model/utils.py` & `dsf_python-3.5.1rc1/src/dsf/object_model/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
-def is_model_object(o) -> bool:
+def is_model_object(o):
     from .model_object import ModelObject
     from .model_collection import ModelCollection
     from .model_dictionary import ModelDictionary
 
     return isinstance(o, ModelObject) or isinstance(o, ModelCollection) or isinstance(o, ModelDictionary)
 
 
-def wrap_model_property(name: str, model_type):
+def wrap_model_property(name, model_type):
     """
     Wrap a nullable model object property so that type checks can be performed during update
     :param name: Property of the derived class
     :param model_type: Constructor for creating new elements
     :return:
     """
```

### Comparing `dsf-python-3.5.0rc2/src/dsf/utils.py` & `dsf_python-3.5.1rc1/src/dsf/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import re
 import warnings
 
 
 # We don't want our deprecations to be ignored by default, so create our own type.
 class DeprecatedWarning(UserWarning):
     pass
@@ -21,16 +22,18 @@
     """Flags a function/method as deprecated.
     :param instructions: A human-friendly string of instructions
     """
     def decorator(func):
         """This is a decorator which can be used to mark functions as deprecated.
         It will result in a warning being emitted when the function is used."""
         def deprecated_func(*args, **kwargs):
-            warnings.warn(f"Call to deprecated function {func.__name__}(). {instructions}",
-                          DeprecatedWarning, stacklevel=2)
+            # Do not show DeprecatedWarning on ObjectModel update (function called by update_from_json)
+            if inspect.currentframe().f_back.f_code.co_name not in ['_update_from_json', 'update_from_json']:
+                warnings.warn(f"Call to deprecated function {func.__name__}(). {instructions}",
+                              DeprecatedWarning, stacklevel=2)
             return func(*args, **kwargs)
         return deprecated_func
     return decorator
 
 
 def preserve_builtin(data: dict) -> dict:
     """Add a trailing underscore to parameters using built-in name
```

### Comparing `dsf-python-3.5.0rc2/src/dsf_python.egg-info/PKG-INFO` & `dsf_python-3.5.1rc1/src/dsf_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: dsf-python
-Version: 3.5.0rc2
+Version: 3.5.1rc1
 Summary: Python interface to access DuetSoftwareFramework
 Home-page: https://github.com/Duet3D/dsf-python
 Author: Duet3D Ltd.
 Author-email: pkg@duet3d.com
 Project-URL: Duet3D Support, https://forum.duet3d.com/
 Project-URL: Bug Reports, https://github.com/Duet3D/dsf-python/issues
 Project-URL: Source, https://github.com/Duet3D/dsf-python/
 Keywords: Duet3D,DuetSoftwareFramework,DSF,dsf-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dateutil
 Provides-Extra: dev
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: tox; extra == "dev"
```

### Comparing `dsf-python-3.5.0rc2/src/dsf_python.egg-info/SOURCES.txt` & `dsf_python-3.5.1rc1/src/dsf_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 src/dsf/object_model/utils.py
 src/dsf/object_model/boards/__init__.py
 src/dsf/object_model/boards/accelerometer.py
 src/dsf/object_model/boards/board_closed_loop.py
 src/dsf/object_model/boards/boards.py
 src/dsf/object_model/boards/driver.py
 src/dsf/object_model/boards/driver_closed_loop.py
+src/dsf/object_model/boards/inductive_sensor.py
 src/dsf/object_model/boards/min_max_current.py
 src/dsf/object_model/boards/direct_display/__init__.py
 src/dsf/object_model/boards/direct_display/direct_display.py
 src/dsf/object_model/boards/direct_display/direct_display_controller.py
 src/dsf/object_model/boards/direct_display/direct_display_encoder.py
 src/dsf/object_model/boards/direct_display/direct_display_screen.py
 src/dsf/object_model/boards/direct_display/direct_display_screen_st7567.py
```

### Comparing `dsf-python-3.5.0rc2/tests/test_code.py` & `dsf_python-3.5.1rc1/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/tests/test_custom_http_endpoint.py` & `dsf_python-3.5.1rc1/tests/test_custom_http_endpoint.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/tests/test_custom_m_codes.py` & `dsf_python-3.5.1rc1/tests/test_custom_m_codes.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/tests/test_object_model.py` & `dsf_python-3.5.1rc1/tests/test_object_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         self.assertEqual(model.sbc.dsf.http_endpoints[0].endpoint_type, HttpEndpointType.GET)
 
         json_patch = '{"sbc":{"dsf":{"httpEndpoints":[{},{"endpointType":"POST","namespace":"ExecOnMcode","path":"saveCmdList","isUploadRequest":false,"unixSocket":"/run/dsf/ExecOnMcode/saveCmdList-POST.sock"}]}}}'
         model.update_from_json(json_patch)
         self.assertEqual(len(model.sbc.dsf.http_endpoints), 2)
         self.assertEqual(model.sbc.dsf.http_endpoints[1].endpoint_type, HttpEndpointType.POST)
 
-    def test_job(self):
+    @staticmethod
+    def test_job():
         model = ObjectModel()
-
         json_patch = '{"job":{"file":{"filament":[496.4],"fileName":"0:/gcodes/Veil_Token.gcode","generatedBy":"ideaMaker 4.2.1.5321, 2022-10-01 17:45:38 UTC\u002B0200","height":1.04,"lastModified":"2022-10-01T16:45:39+01:00","layerHeight":0.12,"numLayers":9,"printTime":798,"size":594195,"thumbnails":[{"data":"iVBORw0KGgoAAAANSUhEUgAAAMgAAADICAYAAACtWK6eAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAUnklEQVR4nO3cfYwcZ30H8O/zzMy\u002B3d77nl\u002BuztmOA7bjGIOdBBJioDSEJkBLStOWCERTaKS2alWkqqioqpD6BxSVSlUFaktVggRUjdomBVIaikrA4Y9AYkhsY5vEdnz2\u002Bezz3u3e3b7OzPP8\u002BsfM7O5dfMmdb\u002B9s1O9HWu3u3e7s8/xmnmeefZ7fLEBERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERET0/5261gXoljuA7N5cbuADw8PDU8bc6Isa3eJ5W3MaY/NWxiyQ6Xy9o1D0gCPnguBwv8jzvzY5\u002BTMAZq3L\u002BdG\u002BvqFfHRjYXDVmm0Dv2p72bimFZswCfZ2vc4GL/a5TnPTDM0UTHBtynBe/cv78\u002BOPALABZyzI\u002BAKTev2XL1poxb96bzR4oGbPLCAqdr3GgZvIaxZrF\u002BIwJpozIsY1aTz5Vr8/86/R08SWguZZlXC8/bw1E/3ImM3ZTOl24v39ot6OlcNmYnSOOuzWj9Zhv7UBW62FHqfRKNhpYWw1FXihZ84ILPPfVmZmnD1UqZ14GGqsp7Ad7e3ftdDOFd/f37r0Qhrs3uu4tWmGbo9RmT6nMa2\u002Bho4wijcDKBJRMzBjzk4xS4yfqwZGvz5dOfKdeH19NObcBmXv7\u002B/f81tDQnlIY3j7ierc5Su1MKdW/ku0YEb8pMuMpVZwJzZmGmHP9jvPSdBiePV71L/1naer0c8AlAHY15V1P13MDcf9\u002B4\u002BgDe3PpA3PW7negtg05zphWylmPDw9FmpNheOT5pvmdv7h0/shy3vO5jRt/6U2Z7IMN4NYRx9ntKOWtdTkBwIgEZWtOOMDh5xuNRz5\u002B8eJTy3nfp0dGbtqTyf3TJs99i7vCTuVqWREzY8y4hfxUizo6EQTHHpqc\u002BBcA4Xp8/kq517oAS9kDFLbkMl/2Fby840IjGv9YCBwAapVtOxRBAKAR39cB1CBoCDAnghIkXYXcOuXhLQCW1UC2ZHMPV5X6jawCqgBcicqqASgV3etVlltE0ABQhyAQYD6qg1cS7J2B7J1PpXIAnlrOtvqy2V9sOM7bp0TgQpCOy\u002BcAXS\u002B3FUETQAA4Ruvt88D2WbHvuZzyghHgfy4DF1f1AWvkum0gBghqgPgAVDzkFgAi0c1CoBGdq6ObwALQEj03AHwAAQQmfh5K1BCa8d8CAUIIfCzdffnG9Cy3zGVryspxkZQ5OaQ6yy1xXRTaDd7Gz61Erw0A\u002BB3lDgD4EjWKMC53gKihLB6rNMKwvNzyVq3NDTiCGhS0ADXVjvXiciOJL64Q87jsFlHM/bicSYxriMrrx/FuoP1lTwA0oipel67bBnICmC4a89NhR7/RU\u002B3zhQPAU4AjUeG1UlFPF/d8RgFGJD4jALMiKCNuICra2dHWXv17btPaSSvybDkMv7ncMp8Kgie3KvX\u002BYa03uAAcpRZ8SudjF0AWQEopaChoCBwV1TIQgYFCFdFZbTbufTu3caX\u002BvGnMuZLvf3e55X252XxCtL4rB/XOfkcPZSQq81LnCgFajdbGdeiBQkZF\u002B8WN94UPgZXoW3pNAVURVACUICjLwjiE1k7NA9PLLfN6u\u002B6\u002BgxwAvAO5XOGegYH\u002BqtXbJ8Tcf3M285sbtO7zgNZBtFwighqAM2LxsrG1sshpUWjOh\u002BHlukgttPYylJpztJ4GcPbM/Pz4nO9PHWs2X7rKKqjtmczYrb29u/dlMjdWwvCmPq1vvzGVunVIqXQvFFIA1FXUowzBRSu4LNJ80fefvWzN0XwqdWSiWj014ftnj1YqJ3CVM1w3AKP7h4dvvjGdLvRovdUDsr6VMc/RhR7AS2t3REFcLbJjm\u002BPkB5RCdoV1AKLGXxZBSezseL35RI\u002BSxzamUse/MzNz\u002BUeVSum56\u002Bxsci0biP5gPr97fyY/ckdv9pZJP9zd7zqb\u002Bx29o2mlkFaq39N62cOb5QhFalVrjzTF/qDkm6c/O3n\u002B6R8Dl7u1/T1A6s6BgZvv7\u002B3fXxO7f4Pr7nCV2hHPWuW79TkA0BSpiMhkzdpTc8YeySh14ofV\u002Bol/n5k6fgQodetzHsrnR27v7d0/6qbuGXKdNztK7ct0uS6\u002BSCMUuewoTJVDe6Eu5uQG1z17rF4/81i5fOxMozF9Mvq6te7WvIE8DHj3jI7uKAP7tzjeLqtx0IXaup4zUktJZn\u002BKYfiZD54//7WVvv/RTZtGqlq/64ZU6h4ruKPguq9fi3KuVDEMT3gK3zvj\u002B9/7WbX635\u002BZnV1xg3l0dOxdQ57\u002BqyHXfdNalHElRMRMxzNfrqijE37wbI\u002BWo1\u002B\u002BcGH8G9FIes2sdQNRj90w9s\u002BjrvtAt88G3VASi6IITlv52Z\u002BdfXnnSt//lRtu\u002BPwOL/X76asYaqyHkrX2ULPx\u002BU9duPBHK33vf2y/8eSgUq/PAfCuw/oF1laPBsG3P3r\u002B3Aewhguna/4lfUphq6fQkxULr2MKUcU3Hb9OYeXj8oQVac2sJF8gQ8QzVALMQ1AXoBLfz8Tj\u002BdYMkFxdfC8DPSkRpOIp0lRcNzeup1rqdpX1FJFW/Vozc4jG9fMQ1AQoQ6L6Rd\u002B99LzIihb7EnPxdLKLaLo6paLHHgBn8VRw/J5u7c/F9UxmxxoiKMV1nRDpOWvtwFV9wAqsdQMRALUmgM7p2k4qntWIpjmjg9aJ3yhoTylK6z4Kni/tqcQQ0RRugKhRROsb0XRuGP9/LZZujbVVdGy/vey\u002BqJ6CBfNmItFkb3IwJfVLpj7b94IgXqdpN4aongGima1mXM8A3c2T6ayBRTQjFe3Dxf9d\u002BKYF84PS7oSS6WHE5Wzvz/Z0cT1\u002BfYB2Pf14Gr7WXkdpl0ut7fAKWIcziAAXjAhcqFZXI0vcTMe7kgCGglZDMPF/Og96A8BIcgBJ6\u002BzRebAsdX4wIjURGZ8Ngr\u002B5mrqVQ3my37W/3qvVBhfRYlpnp7m4fp0HSNLYk78paZfZR3JQLjwzBvFaQ4D2gfRqDd\u002BKzDZEnrqauh2u1z51UyrzibxWO3NaZVyJG/SiaWDpuL9SfTsbQVK/UBY3wPY\u002B9RGt\u002BST1TOp9pX3oiExi6d3bFWs\u002BuPxQobD59ZnM72aBd/c6zu6s1oMpAJl4ujM6dSt4aJ\u002Buk1tnkGvxesa0CBrxAZIsogFR0P24B/I7/t9asLK20rD2rIgUNXBo1pgTPY5z\u002BKnJyfFL0cL3Vflwf//2kVzu7hHPO\u002BiJ7MxovTOndX8a7d4nOVskS4QeoszJlFJIoz1USSR1DhD1qqV4LaQs7UXCEO0GlBxcgbWzDWvHHeCFWWO\u002BB2O\u002B//Vi8eTV1u2tQO8bN20aE\u002BC2Ta672wH2aqV29yldSDs676E9rExGAUl9BQpGBKJUqzNQAHoB5KGQUapV784GZeI61xEN8yoQXBDBXDxi8K2drxlzGMCTl\u002Br1r/1vuXz2auu3HGvaQA4A3tuGhzfcmU5vnbdq37Z06kBTyX0j2tmsV/F9Y0IEzwT\u002BibKVFw2AmjWXrUgQaF33gGLW8y7XwnDuzPz8eN3a2ulqdXwOmOlu7ZakCsCmsZ6ekd3Z7NimVHZsg6vu3KjUfdscd7AHK1/LSRgRXBLBuNj5s2H4jUlrf1D0/fGLtdrkbK127hQw1d2qLK0PGBpNpws78vmxbel0YcB1\u002B\u002BrGjAiQs9YOp5TyUsoZCWGRh9ryhpS3b1RpvZq6F62dTAv\u002BayoMn3PEPH\u002B60Rh/dGbm0lqunXS1gbwZ6Hvn0NCet\u002Bfzt9dE7dvkOfuMYDSr1Ei3p3RDkYuTgf/Xf3Du3BfORxkk14178/mRB3sHDuRd9Z4R1zvoKbWj2\u002BsgRqTZsPbEnLGHG7CP/\u002BW5c9//CbDsNJP18NG\u002BvqEHh4b\u002BNK/1RzylN3Vz21bENEWKSmFiJgyPOMDhI43Gc1\u002Bemnr\u002BGFDp1uesuIE8APQf3LCh8LpMZvOFwNxycyZ1c9nYPVmtd/U5zmi3CrZcgUhlKgwe88PwH57x/Rc\u002BWyyu64LSA\u002Bgbeu8v9Baswb4tae\u002BOQHDXJs\u002B9bT3LAAC\u002BtbU5Y486GofP\u002B/5TvSIvfHFycuJbwNx6luPhwcH\u002Bd\u002BRyB4Zc9z2DjvtwtzuG12JFTMmYs0m28LgfHO918OKpqpn8t/LFqedWuG7yqg3kvp6eTQezvbsOxivdoylvL4DNAApZrdd8im0lrIgJIadKoXlyyg8f\u002B8jFiaewBl/gfhvI3DC44cBbezNv9ZRzMK2wx9G6kFaqt9uftRqBtTUDTNStnAzEHDru\u002Bz/8\u002BMWLT2ON0sq/uGHLG0Yy\u002BmMbXfdeD2qrXqdU/\u002BUwIsa3tqyUnhJIsRSaIwOuPn6k0XjxC5OTP3y1zINWA3konx95b3//Dqv1XQPafbuI7Cx47uvWpwrd93LT/9svnh//xLe6cGXbh4Ge\u002BzZvuWc45dzf67j3p9e5V\u002ByWpkilFAZP1EJ8db42d\u002BihcnnVQ7J7gfTHbhj7zPZU6o\u002B7UcZroWzMORE8M2PDZ7S1T39zdvbUlyqVywCgPjcy8qa9ufwnc1rdntF6VF/HGb4rMWNt7dH5uYP/WCweXs12HkT/4MPbhh7vc5y3dats14M5a559ZGrqfY9Uq6u6DuOThcL\u002Bu3v7Dg1onetW2a4lC4QNay8YkR\u002BfrQefdm/L5w/ltXPdpYGsVF0ENQguWMEZsThvrb4osurGXs36\u002BWlgVzpeTV7thVrXmolTz58xduxH1qZWu72667qnxerh\u002BKL6rIqn7H9OY6UBN6f1GICxjVm5zT0vUtssticLhdR1mHNzJbMirfWBmTj9IE6taC\u002B8AalCOn1VaRaLzYlARJABkIUgHa/huD8n8ZqL4zMpFhPx44rtTm7B9lSqzwFSNURjWUcEHqKUlBQEXrzu4\u002BHnK15nrMXzYQi3Ya1f0hplCLREOUUu4guToOLLLV\u002BZO3W16xiJzvyp5JYs6vkiqMbpE1WJFglnEDWKOazDT49cqbyI0lf8jqvudHxJbZSf1M7BWpxr1o08rFY5pL0IKuiIGQRVARoQVASYE4uyANMdK9hrISlHolUmAZoq\u002BksrV0ukdWxpxBe8IYrb4uOs8wZ073hLshiCuJxVEdQRdRpFEUyLtFaNayJww45pL4v2gkK0uinxFXgLSVxZwcK8KWBhwDp3TAhBKFF\u002BUeelpBbR6rBBx6Ww8TaSlISw4z3LnZZqWnvyTLl8dJkvX1Idr0znaOWOoR1sif8TX526YGUZ6MhR6sg3S7aBjm0lj9sxlDjPbGH2QCjty4o7L3E1EqVu\u002BGgfDFeigBBa\u002BysIxRUdKhaP3VUYOTekZasDAK9yIAuSPLL28\u002Bg\u002Bjl5HLldnAuSrxa0zRakzncfGcVucVeHHcWtdvowkVenKl1477\u002Brr\u002B5VerW9cnGOzWGdOUCu1IU6YawCt\u002B7q0n1fjvzUQZdI247/XEe3YprRbchgXOAlIZ6Ozi54vWUaRWihyrBaGj5wulf7wB/X6hdd4y2s6FYZz\u002B3pytZyjb3cVeqIfMlje6LozVWZh3NrXlCex6oxbDVGMGgCqiIaOPhbGLdlOiKXz2paKmRWplcLwT75fKj298ogsdDwIKi/Ozn5pIJud11oPWaUKWsFpHeDLjBXwyv19pbglyYtJrJqS/M4AWpdZNxBdqpwM\u002BxqIGkYD7QZqlviszng1rP2u\u002BvPR0Z0DjvN3Gxz37nzHeaydebpwQ7Joo0nCXfL6zkS0zvV/v9XHtndq8trkBwCS1pskIobSfu\u002BVKiAiUjXmuKfU8Wnff8JT6vCpqamXXlhFbtVSPjQyctP2dPrBLPT9w67e3a9U2ot3vY6vdRcAUO2YXSl5r93LyYKzhpH24yQ\u002B0eOOJD8sjFv7\u002BvCFP0wh8fB0cRZzzZijxtqv1YPg248Xi891KzYdUr\u002B3efNeR\u002BQNo573bgXsH3Scm3Iq\u002BhEwpyOZU2FRzLAwbsArz6jJ8QZ0nDWk3evbjr8nI5XW8SYLE1zDeEvJGSTJb0u2VTfmmZlK5cFWg3jf8PBtr0ulDg647jt6tN6RgRrJajWgAc/rGGZ17ujWc5WcBheePtunK1mQeRpIu0EIol/ESM4incMvI9IIrZ0VpSqi1GQ1DMcNMO4AP51oNE6fKZWOn1\u002B/HKuWXmD4/Rs33jnqeXvSSr1lUDtbNWTAgxpOK/Q4SmkH0S\u002BsJGnenb15q9GoOCayuFG0h2wL47ZwqGkk6Q0lGffbhtiyAWpa62IlDE8KcHKm2Tx0qlY78VK9fn6tY7PYENC3t69v596enp2eUnuyWu/q17rgKFXwgMG0UjkPqtdRHUmbi\u002BKW/OrLgs4mPiCtLGwUUawUgrgBSEeMWo2j43hrAIFv7awAMzVrf\u002BIAh8/U6986VCq9ACy9kp69e3Bw5I09PQPlMNziAje6WhcKrru5bm1BATkLFFwRV5Te4Kjkug6B0npQK5WNfpoH4lsz2dm7ATIXiFQCEau0vqSUqqS1nq8bU5kNw/HAmFoITA6m00VrzPzp2dnZS/V65eXrLM9oEWdXb\u002B/A7nR6eGsqlZ81ZhTWjmQ9b6zfcQoudM634YhA9SlBj1LoVUr1JuNpA1Epx9mcNBYLII6btNL5xV4KAWOVqgowl9b6cihSK/n\u002BeN3asmg9vcF1X56oVksXwrB2tFot4trMZyzLRqBnWzY7ONrTk9ueTg8Vw7Cggc09WhdcIDfoeRsq1m50RWkL2egoaCXIi1J9UVJf1IV4UdxU0tEG1l60EBsPo5rW2ul4pbgIpWppxynONJvjVWOmoFR5IJ0\u002Beb5SmZ0ol2eu1XXvRERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERERNe3/wOxabcDNmswcQAAAABJRU5ErkJggg==","format":"png","height":200,"offset":483,"size":7144,"width":200}]},"build":{"currentObject":-1,"m486Names":false,"m486Numbers":false,"objects":[]},"duration":0,"pauseDuration":0,"rawExtrusion":0,"warmUpDuration":0,"layers":[],"lastDuration":null}}'
         model.update_from_json(json_patch)
 
     def test_json_serialization(self):
         # Hint: To get the object model, execute the command get_object_model() from any connection in debug mode
         # and take the JSON returned from debug (after "recv:")
         with open('object_model/model_geminiv2.json') as fp:
```

### Comparing `dsf-python-3.5.0rc2/tests/test_send_simple_code.py` & `dsf_python-3.5.1rc1/tests/test_send_simple_code.py`

 * *Files identical despite different names*

### Comparing `dsf-python-3.5.0rc2/tests/test_subscribe_object_model.py` & `dsf_python-3.5.1rc1/tests/test_subscribe_object_model.py`

 * *Files identical despite different names*

