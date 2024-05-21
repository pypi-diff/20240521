# Comparing `tmp/pye2-0.7.9.tar.gz` & `tmp/pye2-0.8.0.tar.gz`

## Comparing `pye2-0.7.9.tar` & `pye2-0.8.0.tar`

### file list

```diff
@@ -1,90 +1,97 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.7.9/.gitattributes
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.7.9/TODOs.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.7.9/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.7.9/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.7.9/winrun.bat
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.7.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/_ver.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base_decentra_object.py
--rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/plugins_manager_mixin.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/__init__.py
--rw-r--r--   0        0        0    40906 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/instance.py
--rw-r--r--   0        0        0    29508 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/pipeline.py
--rw-r--r--   0        0        0    62467 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/plugin_template.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/bc/__init__.py
--rw-r--r--   0        0        0    26813 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/bc/base.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/bc/ec.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/code_cheker/__init__.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/code_cheker/base.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/README.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/base.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/comms.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/environment.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/formatter.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/misc.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/default/__init__.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/aixp1.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/io_formatter/default/default.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/__init__.py
--rw-r--r--   0        0        0    58743 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/base_logger.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/small_logger.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/class_instance_mixin.py
--rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/computer_vision_mixin.py
--rw-r--r--   0        0        0    11305 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/datetime_mixin.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/download_mixin.py
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/general_serialization_mixin.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/json_serialization_mixin.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/process_mixin.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/resource_size_mixin.py
--rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/timers_mixin.py
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/upload_mixin.py
--rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/logger_mixins/utils_mixin.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/__init__.py
--rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/unix.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/utils.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/win32.py
--rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/logging/tzlocal/windows_tz.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/.example_env
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/1. hello_world.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/2. first_deploy.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/tutorials/3. simple_real_time_custom_code.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/code.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/comm_utils.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.7.9/PyE2/utils/dotenv.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/.example_env
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/attach_example.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/ex1.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/hello.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/remote_exec.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/decentralized/chain_dist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/decentralized/chain_dist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.7.9/xperimental/decentralized/chain_dist_example_worker.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.7.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.7.9/LICENSE
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 pye2-0.7.9/README.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pye2-0.7.9/pyproject.toml
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 pye2-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.8.0/.gitattributes
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.8.0/TODOs.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.8.0/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.8.0/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.8.0/winrun.bat
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/_ver.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base_decentra_object.py
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/plugins_manager_mixin.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    49968 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/instance.py
+-rw-r--r--   0        0        0    49602 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0    62467 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/plugin_template.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/responses.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/transaction.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/bc/__init__.py
+-rw-r--r--   0        0        0    27458 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/bc/base.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/bc/ec.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/code_cheker/__init__.py
+-rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/code_cheker/base.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    13817 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/README.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/base.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/comms.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/environment.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/formatter.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/misc.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/aixp1.py
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/default.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/__init__.py
+-rw-r--r--   0        0        0    59434 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/base_logger.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/small_logger.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/class_instance_mixin.py
+-rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/computer_vision_mixin.py
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/datetime_mixin.py
+-rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/download_mixin.py
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/general_serialization_mixin.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/json_serialization_mixin.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/process_mixin.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/resource_size_mixin.py
+-rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/timers_mixin.py
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/upload_mixin.py
+-rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/utils_mixin.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/__init__.py
+-rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/unix.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/utils.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/win32.py
+-rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/windows_tz.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/.example_env
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/1. hello_world.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/2. first_deploy.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/3. simple_real_time_custom_code.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/4. real_time_custom_code_2.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/5. real_time_custom_code_multithreading.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/7. real_time_custom_code_multithreading.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/8. chatbot.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/comm_utils.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/dotenv.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/.example_env
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/attach_example.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/ex1.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/hello.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/decentralized/chain_dist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/decentralized/chain_dist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/decentralized/chain_dist_example_worker.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.8.0/LICENSE
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 pye2-0.8.0/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pye2-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 pye2-0.8.0/PKG-INFO
```

### Comparing `pye2-0.7.9/.github/workflows/python-publish.yml` & `pye2-0.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/base_decentra_object.py` & `pye2-0.8.0/PyE2/base_decentra_object.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/plugins_manager_mixin.py` & `pye2-0.8.0/PyE2/plugins_manager_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,24 @@
       modules += [plugins_location + '.' + x for x in files]
       names += [x.replace('_', '').lower() for x in files]
 
     return names, modules
 
   def _get_plugin_by_name(self, lst_plugins_locations, name, safe=False):
     name = self.log.camel_to_snake(name)
-    # the root location is supposed to be the first position in the list
-    root_location = lst_plugins_locations[0].replace('.', '/')
-    sub_locations = self.log.get_all_subfolders(root_location, as_package=True)
-    lst_plugins_locations = sub_locations + lst_plugins_locations
+    total_sub_locations = []
+    # First we extract all the sublocations
+    for location in lst_plugins_locations:
+      root_location = location.replace('.', '/')
+      sub_locations = self.log.get_all_subfolders(root_location, as_package=True)
+      total_sub_locations += sub_locations
+    # endfor
+    # we remove duplicates
+    total_sub_locations = list(set(total_sub_locations))
+    lst_plugins_locations = lst_plugins_locations + total_sub_locations
     for loc in lst_plugins_locations:
       if loc.endswith('__pycache__'):
         continue
       candidate = loc + '.' + name
       try:
         found = importlib.util.find_spec(candidate)
         if found is not None:
```

### Comparing `pye2-0.7.9/PyE2/base/generic_session.py` & `pye2-0.8.0/PyE2/base/generic_session.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 from ..base_decentra_object import BaseDecentrAIObject
 from ..io_formatter import IOFormatterWrapper
 from ..logging import Logger
 from ..utils import load_dotenv
 from ..utils.code import CodeUtils
 from .payload import Payload
 from .pipeline import Pipeline
+from .transaction import Transaction
 
 # TODO: add support for remaining commands from EE
 
 
 class GenericSession(BaseDecentrAIObject):
   """
-  A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
+  A Session is a connection to a communication server which provides the channel to interact with nodes from the DecentrAI network.
   A Session manages `Pipelines` and handles all messages received from the communication server.
-  The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
+  The Session handles all callbacks that are user-defined and passed as arguments in the API calls.
   """
   default_config = {
       "CONFIG_CHANNEL": {
           "TOPIC": "lummetry/{}/config"
       },
       "CTRL_CHANNEL": {
           "TOPIC": "lummetry/ctrl"
@@ -54,67 +55,71 @@
                port=None,
                user=None,
                pwd=None,
                name='pySDK',
                encrypt_comms=False,
                config={},
                filter_workers=None,
-               log : Logger =None,
+               log: Logger = None,
                on_payload=None,
                on_notification=None,
                on_heartbeat=None,
                silent=True,
                verbosity=1,
                dotenv_path=None,
+               show_commands=False,
                blockchain_config=BLOCKCHAIN_CONFIG,
                bc_engine=None,
                formatter_plugins_locations=['plugins.io_formatters'],
                **kwargs) -> None:
     """
-    A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
+    A Session is a connection to a communication server which provides the channel to interact with nodes from the DecentrAI network.
     A Session manages `Pipelines` and handles all messages received from the communication server.
-    The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
+    The Session handles all callbacks that are user-defined and passed as arguments in the API calls.
 
     Parameters
     ----------
     host : str, optional
         The hostname of the server. If None, it will be retrieved from the environment variable AIXP_HOSTNAME
     port : int, optional
         The port. If None, it will be retrieved from the environment variable AIXP_PORT
     user : str, optional
         The user name. If None, it will be retrieved from the environment variable AIXP_USERNAME
     pwd : str, optional
         The password. If None, it will be retrieved from the environment variable AIXP_PASSWORD
     name : str, optional
-        The name of this connection, used to identify owned pipelines on a specific AiXpand node.
-        The name will be used as `INITIATOR_ID` and `SESSION_ID` when communicating with AiXp nodes, by default 'pySDK'
+        The name of this connection, used to identify owned pipelines on a specific DecentrAI node.
+        The name will be used as `INITIATOR_ID` and `SESSION_ID` when communicating with DecentrAI nodes, by default 'pySDK'
     config : dict, optional
         Configures the names of the channels this session will connect to.
         If using a Mqtt server, these channels are in fact topics.
         Modify this if you are absolutely certain of what you are doing.
         By default {}
     filter_workers: list, optional
-        If set, process the messages that come only from the nodes from this list. 
+        If set, process the messages that come only from the nodes from this list.
         Defaults to None
+    show_commands : bool
+        If True, will print the commands that are being sent to the DecentrAI nodes.
+        Defaults to False
     log : Logger, optional
         A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
         In the future, the documentation for the Logger base class will be available and developers will be able to use
-        custom-made Loggers. 
+        custom-made Loggers.
     on_payload : Callable[[Session, str, str, str, str, dict], None], optional
         Callback that handles all payloads received from this network.
-        As arguments, it has a reference to this Session object, the node name, the pipeline, signature and instance, and the payload. 
+        As arguments, it has a reference to this Session object, the node name, the pipeline, signature and instance, and the payload.
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
     on_notification : Callable[[Session, str, dict], None], optional
-        Callback that handles notifications received from this network. 
-        As arguments, it has a reference to this Session object, the node name and the notification payload. 
+        Callback that handles notifications received from this network.
+        As arguments, it has a reference to this Session object, the node name and the notification payload.
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
         This callback will be called when there are notifications related to the node itself, e.g. when the node runs
-        low on memory. 
+        low on memory.
         Defaults to None.
     on_heartbeat : Callable[[Session, str, dict], None], optional
         Callback that handles heartbeats received from this network.
         As arguments, it has a reference to this Session object, the node name and the heartbeat payload.
         Defaults to None.
     silent : bool, optional
         This flag will disable debug logs, set to 'False` for a more verbose log, by default True
@@ -127,19 +132,20 @@
 
     self.log = log
     self.name = name
 
     self._verbosity = verbosity
     self.encrypt_comms = encrypt_comms
 
-    self._online_boxes = {}
+    self._online_boxes: dict[str, Pipeline] = {}
     self._last_seen_boxes = {}
     self._box_addr = {}
     self.online_timeout = 60
     self.filter_workers = filter_workers
+    self.__show_commands = show_commands
 
     pwd = pwd or kwargs.get('password', kwargs.get('pass', None))
     user = user or kwargs.get('username', None)
     host = host or kwargs.get('hostname', None)
     self.__fill_config(host, port, user, pwd, dotenv_path)
 
     self.custom_on_payload = on_payload
@@ -148,22 +154,22 @@
 
     self.own_pipelines = []
 
     self.__running_callback_threads = False
     self.__running_main_loop_thread = False
     self.__closed_everything = False
 
-    self.__close_pipelines = False
-
     self.sdk_main_loop_thread = Thread(target=self.__main_loop, daemon=True)
     self.__formatter_plugins_locations = formatter_plugins_locations
 
     self.__bc_engine = bc_engine
     self.__blockchain_config = blockchain_config
 
+    self.__open_transactions: list[Transaction] = []
+
     self.__create_user_callback_threads()
     super(GenericSession, self).__init__(log=log, DEBUG=not silent, create_logger=True)
     return
 
   def startup(self):
     self.__start_blockchain(self.__bc_engine, self.__blockchain_config)
     self.formatter_wrapper = IOFormatterWrapper(self.log, plugin_search_locations=self.__formatter_plugins_locations)
@@ -260,15 +266,15 @@
         return
 
       message_callback(dict_msg_parsed, msg_eeid, msg_pipeline, msg_signature, msg_instance)
       return
 
     def __handle_messages(self, message_queue, message_callback):
       """
-      Handle messages from the communication server. 
+      Handle messages from the communication server.
       This method is called in a separate thread.
 
       Parameters
       ----------
       message_queue : deque
           The queue of messages received from the communication server
       message_callback : Callable[[dict, str, str, str, str], None]
@@ -292,15 +298,15 @@
       """
       Check if the message should be ignored.
       A message should be ignored if the `filter_workers` attribute is set and the message comes from a node that is not in the list.
 
       Parameters
       ----------
       e2id : str
-          The name of the AiXpand node that sent the message.
+          The name of the DecentrAI node that sent the message.
 
       Returns
       -------
       bool
           True if the message should be ignored, False otherwise.
       """
       return self.filter_workers is not None and e2id not in self.filter_workers
@@ -308,30 +314,30 @@
     def __track_online_node(self, e2id, ee_address):
       """
       Track the last time a node was seen online.
 
       Parameters
       ----------
       e2id : str
-          The name of the AiXpand node that sent the message.
+          The name of the DecentrAI node that sent the message.
       """
       self._last_seen_boxes[e2id] = tm()
       self._box_addr[e2id] = ee_address
       return
 
     def __on_heartbeat(self, dict_msg: dict, msg_eeid, msg_pipeline, msg_signature, msg_instance):
       """
       Handle a heartbeat message received from the communication server.
 
       Parameters
       ----------
       dict_msg : dict
           The message received from the communication server
       msg_eeid : str
-          The name of the AiXpand node that sent the message.
+          The name of the DecentrAI node that sent the message.
       msg_pipeline : str
           The name of the pipeline that sent the message.
       msg_signature : str
           The signature of the plugin that sent the message.
       msg_instance : str
           The name of the instance that sent the message.
       """
@@ -343,23 +349,36 @@
         dict_msg = {**dict_msg, **data}
 
       msg_active_configs = dict_msg.get(HB.CONFIG_STREAMS)
       if msg_active_configs is None:
         return
 
       # default action
-      self._online_boxes[msg_eeid] = {config[PAYLOAD_DATA.NAME]: config for config in msg_active_configs}
+      if msg_eeid not in self._online_boxes:
+        self._online_boxes[msg_eeid] = {}
+      for config in msg_active_configs:
+        pipeline_name = config[PAYLOAD_DATA.NAME]
+        pipeline: Pipeline = self._online_boxes[msg_eeid].get(pipeline_name, None)
+        if pipeline is not None:
+          pipeline.update_full_configuration(config)
+        else:
+          self._online_boxes[msg_eeid][pipeline_name] = self.__create_pipeline_from_config(msg_eeid, config)
 
       ee_address = dict_msg[HB.EE_ADDR]
       self.__track_online_node(msg_eeid, ee_address)
 
       # TODO: move this call in `__on_message_default_callback`
       if self.__maybe_ignore_message(msg_eeid):
         return
 
+      # pass the heartbeat message to open transactions
+      no_transactions = len(self.__open_transactions)
+      for idx in range(no_transactions):
+        self.__open_transactions[idx].handle_heartbeat(dict_msg)
+
       self.D("Received hb from: {}".format(msg_eeid), verbosity=2)
 
       # call the custom callback, if defined
       if self.custom_on_heartbeat is not None:
         self.custom_on_heartbeat(self, msg_eeid, dict_msg)
 
       return
@@ -369,15 +388,15 @@
       Handle a notification message received from the communication server.
 
       Parameters
       ----------
       dict_msg : dict
           The message received from the communication server
       msg_eeid : str
-          The name of the AiXpand node that sent the message.
+          The name of the DecentrAI node that sent the message.
       msg_pipeline : str
           The name of the pipeline that sent the message.
       msg_signature : str
           The signature of the plugin that sent the message.
       msg_instance : str
           The name of the instance that sent the message.
       """
@@ -405,14 +424,19 @@
       for pipeline in self.own_pipelines:
         if msg_eeid == pipeline.e2id and msg_pipeline == pipeline.name:
           pipeline._on_notification(msg_signature, msg_instance, Payload(dict_msg))
           # since we found the pipeline, we can stop searching
           # because the pipelines have unique names
           break
 
+      # pass the notification message to open transactions
+      no_transactions = len(self.__open_transactions)
+      for idx in range(no_transactions):
+        self.__open_transactions[idx].handle_notification(dict_msg)
+
       # call the custom callback, if defined
       if self.custom_on_notification is not None:
         self.custom_on_notification(self, msg_eeid, Payload(dict_msg))
 
       return
 
     # TODO: maybe convert dict_msg to Payload object
@@ -423,15 +447,15 @@
       Handle a payload message received from the communication server.
 
       Parameters
       ----------
       dict_msg : dict
           The message received from the communication server
       msg_eeid : str
-          The name of the AiXpand node that sent the message.
+          The name of the DecentrAI node that sent the message.
       msg_pipeline : str
           The name of the pipeline that sent the message.
       msg_signature : str
           The signature of the plugin that sent the message.
       msg_instance : str
           The name of the instance that sent the message.
       """
@@ -445,14 +469,19 @@
       for pipeline in self.own_pipelines:
         if msg_eeid == pipeline.e2id and msg_pipeline == pipeline.name:
           pipeline._on_data(msg_signature, msg_instance, Payload(dict_msg))
           # since we found the pipeline, we can stop searching
           # because the pipelines have unique names
           break
 
+      # pass the payload message to open transactions
+      no_transactions = len(self.__open_transactions)
+      for idx in range(no_transactions):
+        self.__open_transactions[idx].handle_payload(dict_msg)
+
       if self.custom_on_payload is not None:
         self.custom_on_payload(self, msg_eeid, msg_pipeline, msg_signature, msg_instance, Payload(msg_data))
 
       return
 
   # Main loop
   if True:
@@ -475,14 +504,24 @@
     def __start_main_loop_thread(self):
       self._main_loop_thread = Thread(target=self.__main_loop, daemon=True)
 
       self.__running_main_loop_thread = True
       self._main_loop_thread.start()
       return
 
+    def __handle_open_transactions(self):
+      no_transactions = len(self.__open_transactions)
+
+      solved_transactions = [i for i in range(no_transactions) if self.__open_transactions[i].is_solved()]
+      solved_transactions.reverse()
+      for idx in solved_transactions:
+        self.__open_transactions[idx].callback()
+        self.__open_transactions.pop(idx)
+      return
+
     @property
     def _connected(self):
       """
       Check if the session is connected to the communication server.
       """
       raise NotImplementedError
 
@@ -494,22 +533,34 @@
       This method should be called in a user-defined main loop.
       This method is called in `run` method, in the main loop.
       """
       if self._connected == False:
         self._connect()
       return
 
-    def __close_own_pipelines(self):
+    def __close_own_pipelines(self, wait=True):
       """
       Close all pipelines that were created by or attached to this session.
+
+      Parameters
+      ----------
+      wait : bool, optional
+          If `True`, will wait for the transactions to finish. Defaults to `True`
       """
-      self.P("Closing own pipelines...", verbosity=2)
       # iterate through all CREATED pipelines from this session and close them
+      transactions = []
+
       for pipeline in self.own_pipelines:
-        pipeline.close()
+        transactions.extend(pipeline._close())
+
+      self.P("Closing own pipelines: {}".format([p.name for p in self.own_pipelines]))
+
+      if wait:
+        self.wait_for_transactions(transactions)
+        self.P("Closed own pipelines.")
       return
 
     def _communication_close(self):
       """
       Close the communication server connection.
       """
       raise NotImplementedError
@@ -524,16 +575,18 @@
       ----------
       close_pipelines : bool, optional
           close all the pipelines created by or attached to this session (basically calling `.close_own_pipelines()` for you), by default False
       wait_close : bool, optional
           If `True`, will wait for the main loop thread to exit. Defaults to `False`
       """
 
+      if close_pipelines:
+        self.__close_own_pipelines(wait=wait_close)
+
       self.__running_main_loop_thread = False
-      self.__close_pipelines = close_pipelines
 
       # wait for the main loop thread to exit
       while not self.__closed_everything and wait_close:
         sleep(0.1)
 
       return
 
@@ -546,15 +599,15 @@
     def _send_payload(self, to, payload):
       """
       Send a payload to a node.
 
       Parameters
       ----------
       to : str
-          The name of the AiXpand node that will receive the payload.
+          The name of the DecentrAI node that will receive the payload.
       payload : dict
           The payload to send.
       """
       raise NotImplementedError
 
     def __release_callback_threads(self):
       """
@@ -571,23 +624,21 @@
       """
       The main loop of this session. This method is called in a separate thread.
       This method runs on a separate thread from the main thread, and it is responsible for handling all messages received from the communication server.
       We use it like this to avoid blocking the main thread, which is used by the user.
       """
       while self.__running_main_loop_thread:
         self.__maybe_reconnect()
+        self.__handle_open_transactions()
         sleep(0.1)
       # end while self.running
 
       self.P("Main loop thread exiting...", verbosity=2)
       self.__release_callback_threads()
 
-      if self.__close_pipelines:
-        self.__close_own_pipelines()
-
       self.P("Comms closing...", verbosity=2)
       self._communication_close()
       self.__closed_everything = True
       return
 
     def run(self, wait=True, close_session=True, close_pipelines=False):
       """
@@ -607,15 +658,15 @@
       close_pipelines : bool, optional
           If `True` will close all pipelines initiated by this session when the loop is exited.
           This flag is ignored if `close_session` is `False`.
           Defaults to `False`
       """
       _start_timer = tm()
       try:
-        while ((isinstance(wait, bool) and wait) or (wait == 0) or (tm() - _start_timer) < wait) and not self.__closed_everything:
+        while ((isinstance(wait, bool) and wait) or ((not isinstance(wait, bool) and wait == 0)) or (tm() - _start_timer) < wait) and not self.__closed_everything:
           sleep(0.1)
       except KeyboardInterrupt:
         self.P("CTRL+C detected. Stopping loop.", color='r', verbosity=1)
 
       if close_session:
         self.close(close_pipelines, wait_close=True)
 
@@ -628,15 +679,15 @@
       Fill the configuration dictionary with the credentials provided when creating this instance.
 
 
       Parameters
       ----------
       host : str
           The hostname of the server.
-          Can be retrieved from the environment variables AIXP_HOSTNAME, AIXP_HOST 
+          Can be retrieved from the environment variables AIXP_HOSTNAME, AIXP_HOST
       port : int
           The port.
           Can be retrieved from the environment variable AIXP_PORT
       user : str
           The user name.
           Can be retrieved from the environment variables AIXP_USERNAME, AIXP_USER
       pwd : str
@@ -655,64 +706,67 @@
       # the path to env file, if not specified, will be search in the following order:
       #  1. current working directory
       #  2-N. directories of the files from the call stack
       load_dotenv(dotenv_path=dotenv_path, verbose=False)
 
       user = user or os.getenv(ENVIRONMENT.AIXP_USERNAME) or os.getenv(ENVIRONMENT.AIXP_USER)
       if user is None:
-        raise ValueError("Error: No user specified for AiXpand network connection")
+        raise ValueError("Error: No user specified for DecentrAI network connection")
       if self._config.get(comm_ct.USER, None) is None:
         self._config[comm_ct.USER] = user
 
       pwd = pwd or os.getenv(ENVIRONMENT.AIXP_PASSWORD) or os.getenv(
         ENVIRONMENT.AIXP_PASS) or os.getenv(ENVIRONMENT.AIXP_PWD)
       if pwd is None:
-        raise ValueError("Error: No password specified for AiXpand network connection")
+        raise ValueError("Error: No password specified for DecentrAI network connection")
       if self._config.get(comm_ct.PASS, None) is None:
         self._config[comm_ct.PASS] = pwd
 
       host = host or os.getenv(ENVIRONMENT.AIXP_HOSTNAME) or os.getenv(ENVIRONMENT.AIXP_HOST)
       if host is None:
-        raise ValueError("Error: No host specified for AiXpand network connection")
+        raise ValueError("Error: No host specified for DecentrAI network connection")
       if self._config.get(comm_ct.HOST, None) is None:
         self._config[comm_ct.HOST] = host
 
       port = port or os.getenv(ENVIRONMENT.AIXP_PORT)
       if port is None:
-        raise ValueError("Error: No port specified for AiXpand network connection")
+        raise ValueError("Error: No port specified for DecentrAI network connection")
       if self._config.get(comm_ct.PORT, None) is None:
         self._config[comm_ct.PORT] = int(port)
       return
 
-    def _send_command_to_box(self, command, worker, payload, show_command=False, worker_address=None, **kwargs):
+    def _send_command_to_box(self, command, worker, payload, show_command=False, session_id=None, **kwargs):
       """
       Send a command to a node.
 
       Parameters
       ----------
       command : str
           The command to send.
       worker : str
-          The name of the AiXpand node that will receive the command.
+          The name of the DecentrAI node that will receive the command.
       payload : dict
           The payload to send.
       show_command : bool, optional
           If True, will print the complete command that is being sent, by default False
       """
 
+      show_command = show_command or self.__show_commands
+
       if len(kwargs) > 0:
         self.D("Ignoring extra kwargs: {}".format(kwargs), verbosity=2)
 
       critical_data = {
         comm_ct.COMM_SEND_MESSAGE.K_ACTION: command,
         comm_ct.COMM_SEND_MESSAGE.K_PAYLOAD: payload,
       }
 
       # This part is duplicated with the creation of payloads
       encrypt_payload = self.encrypt_comms
+      worker_address = self._get_worker_address(worker)
       if encrypt_payload and worker_address is not None:
         # TODO: use safe_json_dumps
         str_data = json.dumps(critical_data)
         str_enc_data = self.bc_engine.encrypt(str_data, worker_address)
         critical_data = {
           comm_ct.COMM_SEND_MESSAGE.K_EE_IS_ENCRYPTED: True,
           comm_ct.COMM_SEND_MESSAGE.K_EE_ENCRYPTED_DATA: str_enc_data,
@@ -722,14 +776,15 @@
         if encrypt_payload:
           critical_data[comm_ct.COMM_SEND_MESSAGE.K_EE_ENCRYPTED_DATA] = "Error! No receiver address found!"
 
       # endif
       msg_to_send = {
           **critical_data,
           comm_ct.COMM_SEND_MESSAGE.K_EE_ID: worker,
+          comm_ct.COMM_SEND_MESSAGE.K_SESSION_ID: session_id or self.name,
           comm_ct.COMM_SEND_MESSAGE.K_INITIATOR_ID: self.name,
           comm_ct.COMM_SEND_MESSAGE.K_SENDER_ADDR: self.bc_engine.address,
           comm_ct.COMM_SEND_MESSAGE.K_TIME: dt.now().strftime("%Y-%m-%d %H:%M:%S.%f"),
       }
       self.bc_engine.sign(msg_to_send, use_digest=True)
       if show_command:
         self.P("Sending command '{}' to '{}':\n{}".format(command, worker, json.dumps(msg_to_send, indent=2)),
@@ -757,47 +812,47 @@
       return
 
     def _send_command_update_instance_config(self, worker, pipeline_name, signature, instance_id, instance_config, **kwargs):
       payload = {
         PAYLOAD_DATA.NAME: pipeline_name,
         PAYLOAD_DATA.SIGNATURE: signature,
         PAYLOAD_DATA.INSTANCE_ID: instance_id,
-        PAYLOAD_DATA.INSTANCE_CONFIG: instance_config
+        PAYLOAD_DATA.INSTANCE_CONFIG: {k.upper(): v for k, v in instance_config.items()}
       }
       self._send_command_to_box(COMMANDS.UPDATE_PIPELINE_INSTANCE, worker, payload, **kwargs)
       return
 
     def _send_command_batch_update_instance_config(self, worker, lst_updates, **kwargs):
       for update in lst_updates:
         assert isinstance(update, dict), "All updates must be dicts"
         assert PAYLOAD_DATA.NAME in update, "All updates must have a pipeline name"
         assert PAYLOAD_DATA.SIGNATURE in update, "All updates must have a plugin signature"
         assert PAYLOAD_DATA.INSTANCE_ID in update, "All updates must have a plugin instance id"
         assert PAYLOAD_DATA.INSTANCE_CONFIG in update, "All updates must have a plugin instance config"
         assert isinstance(update[PAYLOAD_DATA.INSTANCE_CONFIG], dict), \
             "All updates must have a plugin instance config as dict"
-      self._send_command_to_box(COMMANDS.BATCH_UPDATE_PIPELINE_INSTANCES, worker, lst_updates, **kwargs)
+      self._send_command_to_box(COMMANDS.BATCH_UPDATE_PIPELINE_INSTANCE, worker, lst_updates, **kwargs)
 
     def _send_command_pipeline_command(self, worker, pipeline_name, command, payload={}, command_params={}, **kwargs):
       payload = {
         PAYLOAD_DATA.NAME: pipeline_name,
         COMMANDS.PIPELINE_COMMAND: command,
-        # 'COMMAND_PARAMS': command_params, # TODO: check if this is oke
+        COMMANDS.COMMAND_PARAMS: command_params,
         **payload,
       }
       self._send_command_to_box(COMMANDS.PIPELINE_COMMAND, worker, payload, **kwargs)
       return
 
     def _send_command_instance_command(self, worker, pipeline_name, signature, instance_id, command, payload={}, command_params={}, **kwargs):
       payload = {
         COMMANDS.INSTANCE_COMMAND: command,
         **payload,
         COMMANDS.COMMAND_PARAMS: command_params,
       }
-      self._send_command_update_instance_config(worker, pipeline_name, signature, instance_id, payload)
+      self._send_command_update_instance_config(worker, pipeline_name, signature, instance_id, payload, **kwargs)
       return
 
     def _send_command_stop_node(self, worker, **kwargs):
       self._send_command_to_box(COMMANDS.STOP, worker, None, **kwargs)
       return
 
     def _send_command_restart_node(self, worker, **kwargs):
@@ -819,17 +874,67 @@
     def _send_command_delete_all(self, worker, **kwargs):
       self._send_command_to_box(COMMANDS.DELETE_CONFIG_ALL, worker, None, **kwargs)
       return
 
     def _get_worker_address(self, worker):
       return self._box_addr.get(worker)
 
+    def _register_transaction(self, session_id: str, lst_required_responses: list = None, timeout=0, on_success_callback: callable = None, on_failure_callback: callable = None) -> Transaction:
+      """
+      Register a new transaction.
+
+      Parameters
+      ----------
+      session_id : str
+          The session id.
+      lst_required_responses : list[Response], optional
+          The list of required responses, by default None
+      timeout : int, optional
+          The timeout, by default 0
+      on_success_callback : _type_, optional
+          The on success callback, by default None
+      on_failure_callback : _type_, optional
+          The on failure callback, by default None
+      Returns
+      -------
+      Transaction
+          The transaction object
+      """
+      transaction = Transaction(
+        log=self.log,
+        session_id=session_id,
+        lst_required_responses=lst_required_responses or [],
+        timeout=timeout,
+        on_success_callback=on_success_callback,
+        on_failure_callback=on_failure_callback,
+      )
+
+      self.__open_transactions.append(transaction)
+      return transaction
+
+    def __create_pipeline_from_config(self, node, config):
+      pipeline_config = {k.lower(): v for k, v in config.items()}
+      name = pipeline_config.pop('name', None)
+      plugins = pipeline_config.pop('plugins', None)
+
+      pipeline = Pipeline(
+        is_attached=True,
+        session=self,
+        log=self.log,
+        e2id=node,
+        name=name,
+        plugins=plugins,
+        existing_config=pipeline_config,
+      )
+
+      return pipeline
+
   # API
   if True:
-    @property
+    @ property
     def server(self):
       """
       The hostname of the server.
       """
       return self._config[comm_ct.HOST]
 
     def create_pipeline(self, *,
@@ -844,52 +949,52 @@
                         **kwargs) -> Pipeline:
       """
       Create a new pipeline on a node. A pipeline is the equivalent of the "config file" used by the Hyperfy dev team internally.
 
       A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
       A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
-      processing units, usually named `Plugins`. 
+      processing units, usually named `Plugins`.
 
       An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
 
       As such, one will work with `Instances`, by referring to them with the unique identifier (Pipeline, Plugin, Instance).
 
       In the documentation, the following refer to the same thing:
         `Pipeline` == `Stream`
 
         `Plugin` == `Signature`
 
-      This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an AiXpand node is online or not.
+      This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an DecentrAI node is online or not.
       If the node does not appear online, a warning will be displayed at the stdout, telling the user that the message that handles the
       creation of the pipeline will be sent, but it is not guaranteed that the specific node will receive it.
 
       Parameters
       ----------
       e2id : str
-          Name of the AiXpand node that will handle this pipeline.
+          Name of the DecentrAI node that will handle this pipeline.
       name : str
           Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
       data_source : str
           This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
       config : dict, optional
           This is the dictionary that contains the configuration of the acquisition source, by default {}
       plugins : list
-          List of dictionaries which contain the configurations of each plugin instance that is desired to run on the box. 
+          List of dictionaries which contain the configurations of each plugin instance that is desired to run on the box.
           Defaults to []. Should be left [], and instances should be created with the api.
       on_data : Callable[[Pipeline, str, str, dict], None], optional
-          Callback that handles messages received from any plugin instance. 
+          Callback that handles messages received from any plugin instance.
           As arguments, it has a reference to this Pipeline object, the signature and the instance of the plugin
           that sent the message and the payload itself.
           This callback acts as a default payload processor and will be called even if for a given instance
           the user has defined a specific callback.
           Defaults to None.
       on_notification : Callable[[Pipeline, dict], None], optional
-          Callback that handles notifications received from any plugin instance. 
-          As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+          Callback that handles notifications received from any plugin instance.
+          As arguments, it has a reference to this Pipeline object, along with the payload itself.
           This callback acts as a default payload processor and will be called even if for a given instance
           the user has defined a specific callback.
           Defaults to None.
       max_wait_time : int, optional
           The maximum time to busy-wait, allowing the Session object to listen to node heartbeats
           and to check if the desired node is online in the network, by default 0.
       **kwargs :
@@ -914,123 +1019,118 @@
             e2id, tm() - _start
         ), color='r', verbosity=1)
       pipeline = Pipeline(
           self,
           self.log,
           e2id=e2id,
           name=name,
-          data_source=data_source,
+          type=data_source,
           config=config,
           plugins=plugins,
           on_data=on_data,
           on_notification=on_notification,
+          is_attached=False,
           **kwargs
       )
       self.own_pipelines.append(pipeline)
       return pipeline
 
     def get_active_nodes(self):
       """
-      Get the list of all AiXp nodes that sent a message since this session was created, and that are considered online
-
-      Parameters
-      ----------
+      Get the list of all DecentrAI nodes that sent a message since this session was created, and that are considered online
 
       Returns
       -------
       list
-          List of names of all the AiXp nodes that are considered online
+          List of names of all the DecentrAI nodes that are considered online
 
       """
       return [k for k, v in self._last_seen_boxes.items() if tm() - v < self.online_timeout]
 
     def get_active_pipelines(self, e2id):
       """
-      Get a dictionary with all the pipelines that are active on this AiXp node
+      Get a dictionary with all the pipelines that are active on this DecentrAI node
 
       Parameters
       ----------
       e2id : str
-          name of the AiXp node
+          name of the DecentrAI node
 
       Returns
       -------
       dict
           The key is the name of the pipeline, and the value is the entire config dictionary of that pipeline.
 
       """
       return self._online_boxes.get(e2id, None) if e2id in self.get_active_nodes() else None
 
     def attach_to_pipeline(self, *,
                            e2id,
                            name,
                            on_data=None,
                            on_notification=None,
-                           max_wait_time=0,
-                           **kwargs) -> Pipeline:
+                           max_wait_time=0) -> Pipeline:
       """
-      Create a Pipeline object and attach to an existing pipeline on an AiXpand node.
+      Create a Pipeline object and attach to an existing pipeline on an DecentrAI node.
       Useful when one wants to treat an existing pipeline as one of his own,
       or when one wants to attach callbacks to various events (on_data, on_notification).
 
       A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
       A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
-      processing units, usually named `Plugins`. 
+      processing units, usually named `Plugins`.
 
       An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
 
       As such, one will work with `Instances`, by reffering to them with the unique identifier (Pipeline, Plugin, Instance).
 
       In the documentation, the following reffer to the same thing:
         `Pipeline` == `Stream`
 
         `Plugin` == `Signature`
 
-      This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an AiXpand node is online or not.
+      This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an DecentrAI node is online or not.
       If the node does not appear online, a warning will be displayed at the stdout, telling the user that the message that handles the
       creation of the pipeline will be sent, but it is not guaranteed that the specific node will receive it.
 
 
       Parameters
       ----------
       e2id : str
-          Name of the AiXpand node that handles this pipeline.  
+          Name of the DecentrAI node that handles this pipeline.
       name : str
           Name of the existing pipeline.
       on_data : Callable[[Pipeline, str, str, dict], None], optional
-          Callback that handles messages received from any plugin instance. 
+          Callback that handles messages received from any plugin instance.
           As arguments, it has a reference to this Pipeline object, the signature and the instance of the plugin
           that sent the message and the payload itself.
           This callback acts as a default payload processor and will be called even if for a given instance
           the user has defined a specific callback.
           Defaults to None.
       on_notification : Callable[[Pipeline, dict], None], optional
-          Callback that handles notifications received from any plugin instance. 
-          As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+          Callback that handles notifications received from any plugin instance.
+          As arguments, it has a reference to this Pipeline object, along with the payload itself.
           This callback acts as a default payload processor and will be called even if for a given instance
           the user has defined a specific callback.
           Defaults to None.
       max_wait_time : int, optional
           The maximum time to busy-wait, allowing the Session object to listen to node heartbeats
           and to check if the desired node is online in the network, by default 0.
-      **kwargs :
-          The user can provide the configuration of the acquisition source directly as kwargs.
 
       Returns
       -------
       Pipeline
           A `Pipeline` object.
 
       Raises
       ------
       Exception
           Node does not exist (it is considered offline because the session did not receive any heartbeat)
       Exception
-          Node does not host the desired pipeline 
+          Node does not host the desired pipeline
       """
 
       _start = tm()
       found = e2id in self.get_active_nodes()
       while (tm() - _start) < max_wait_time and not found:
         sleep(0.1)
         avail_workers = self.get_active_nodes()
@@ -1039,26 +1139,172 @@
 
       if not found:
         raise Exception("Unable to attach to pipeline. Node does not exist")
 
       if name not in self._online_boxes[e2id]:
         raise Exception("Unable to attach to pipeline. Pipeline does not exist")
 
-      pipeline_config = {
-          k.lower(): v for k, v in self._online_boxes[e2id][name].items()}
-      data_source = pipeline_config['type']
-
-      pipeline = Pipeline(
-        session=self,
-        log=self.log,
-        e2id=e2id,
-        data_source=data_source,
-        create_pipeline=False,
-        on_data=on_data,
-        on_notification=on_notification,
-        **pipeline_config,
-        **kwargs
-      )
+      pipeline = self._online_boxes[e2id][name]
 
       self.own_pipelines.append(pipeline)
 
       return pipeline
+
+    def create_or_attach_to_pipeline(self, *,
+                                     e2id,
+                                     name,
+                                     data_source,
+                                     config={},
+                                     plugins=[],
+                                     on_data=None,
+                                     on_notification=None,
+                                     max_wait_time=0,
+                                     **kwargs) -> Pipeline:
+      """
+      Create a new pipeline on a node, or attach to an existing pipeline on an DecentrAI node.
+
+      Parameters
+      ----------
+      e2id : str
+          Name of the DecentrAI node that will handle this pipeline.
+      name : str
+          Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
+      data_source : str
+          This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
+      config : dict, optional
+          This is the dictionary that contains the configuration of the acquisition source, by default {}
+      plugins : list
+          List of dictionaries which contain the configurations of each plugin instance that is desired to run on the box. 
+          Defaults to []. Should be left [], and instances should be created with the api.
+      on_data : Callable[[Pipeline, str, str, dict], None], optional
+          Callback that handles messages received from any plugin instance. 
+          As arguments, it has a reference to this Pipeline object, the signature and the instance of the plugin
+          that sent the message and the payload itself.
+          This callback acts as a default payload processor and will be called even if for a given instance
+          the user has defined a specific callback.
+          Defaults to None.
+      on_notification : Callable[[Pipeline, dict], None], optional
+          Callback that handles notifications received from any plugin instance. 
+          As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+          This callback acts as a default payload processor and will be called even if for a given instance
+          the user has defined a specific callback.
+          Defaults to None.
+      max_wait_time : int, optional
+          The maximum time to busy-wait, allowing the Session object to listen to node heartbeats
+          and to check if the desired node is online in the network, by default 0.
+      **kwargs :
+          The user can provide the configuration of the acquisition source directly as kwargs.
+
+      Returns
+      -------
+      Pipeline
+          A `Pipeline` object.
+      """
+
+      pipeline = None
+      try:
+        pipeline = self.attach_to_pipeline(
+          e2id=e2id,
+          name=name,
+          on_data=on_data,
+          on_notification=on_notification,
+          max_wait_time=max_wait_time,
+          **kwargs
+        )
+
+        possible_new_configuration = {
+          **config,
+          **kwargs
+        }
+
+        if len(plugins) > 0:
+          possible_new_configuration['PLUGINS'] = plugins
+
+        if len(possible_new_configuration) > 0:
+          pipeline.update_full_configuration(config=possible_new_configuration)
+      except Exception as e:
+        self.D("Failed to attach to pipeline: {}".format(e))
+        pipeline = self.create_pipeline(
+          e2id=e2id,
+          name=name,
+          data_source=data_source,
+          config=config,
+          plugins=plugins,
+          on_data=on_data,
+          on_notification=on_notification,
+          **kwargs
+        )
+
+      return pipeline
+
+    def wait_for_transactions(self, transactions):
+      """
+      Wait for the transactions to be solved.
+
+      Parameters
+      ----------
+      transactions : list[Transaction]
+          The transactions to wait for.
+      """
+      while any([not transaction.is_finished() for transaction in transactions]):
+        sleep(0.1)
+      return
+
+    def wait_for_any_node(self, timeout=15):
+      """
+      Wait for any node to appear online.
+
+      Parameters
+      ----------
+      timeout : int, optional
+          The timeout, by default 15
+
+      Returns
+      -------
+      bool
+          True if any node is online, False otherwise.
+      """
+      self.P("Waiting for any node to appear online...")
+      _start = tm()
+      found = len(self.get_active_nodes()) > 0
+      while (tm() - _start) < timeout and not found:
+        sleep(0.1)
+        found = len(self.get_active_nodes()) > 0
+      # end while
+
+      if found:
+        self.P("Found nodes {} online.".format(self.get_active_nodes()))
+      else:
+        self.P("No nodes found online in {:.1f}s.".format(tm() - _start), color='r')
+      return found
+
+    def wait_for_node(self, e2id, timeout=15):
+      """
+      Wait for a node to appear online.
+
+      Parameters
+      ----------
+      e2id : str
+          The name of the DecentrAI node.
+      timeout : int, optional
+          The timeout, by default 15
+
+      Returns
+      -------
+      bool
+          True if the node is online, False otherwise.
+      """
+
+      self.P("Waiting for node '{}' to appear online...".format(e2id))
+      _start = tm()
+      found = e2id in self.get_active_nodes()
+      while (tm() - _start) < timeout and not found:
+        sleep(0.1)
+        avail_workers = self.get_active_nodes()
+        found = e2id in avail_workers
+      # end while
+
+      if found:
+        self.P("Node '{}' is online.".format(e2id))
+      else:
+        self.P("Node '{}' did not appear online in {:.1f}s.".format(e2id, tm() - _start), color='r')
+      return found
```

### Comparing `pye2-0.7.9/PyE2/base/pipeline.py` & `pye2-0.8.0/PyE2/base/pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # TODO: for custom plugin, do the plugin verification locally too
 
 import os
 
+from ..const import PAYLOAD_DATA
 from ..utils.code import CodeUtils
 from .instance import Instance
-
-WAIT_FOR_WORKER = 15
+from .responses import PipelineArchiveResponse, PipelineOKResponse
+from .transaction import Transaction
 
 
 class Pipeline(object):
   """
   A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
   A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
@@ -21,15 +22,15 @@
 
   In the documentation, the following reffer to the same thing:
     `Pipeline` == `Stream`
 
     `Plugin` == `Signature`
   """
 
-  def __init__(self, session, log, *, e2id, name, data_source, config={}, plugins=[], on_data=None, on_notification=None, create_pipeline=True, **kwargs) -> None:
+  def __init__(self, session, log, *, e2id, name, config={}, plugins=[], on_data=None, on_notification=None, is_attached=False, existing_config=None, **kwargs) -> None:
     """
     A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
     A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
     processing units, usually named `Plugins`. 
 
     An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
@@ -47,15 +48,15 @@
         The Session object which owns this pipeline. A pipeline must be attached to a Session because that is the only
         way the `on_X` callbacks are called
     log : Logger
         A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
         In the future, the documentation for the Logger base class will be available and developers will be able to use
         custom-made Loggers. 
     e2id : str
-        Name of the AiXpand node that will handle this pipeline.  
+        Name of the DecentrAI node that will handle this pipeline.  
     name : str
         The name of this pipeline.
     data_source : str
         This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
     config : dict, optional
         This is the dictionary that contains the configuration of the acquisition source, by default {}
     plugins : List | None, optional
@@ -69,105 +70,232 @@
         Defaults to None.
     on_notification : Callable[[Pipeline, dict], None], optional
         Callback that handles notifications received from this instance. 
         As arguments, it has a reference to this Pipeline object, along with the payload itself. 
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
         Defaults to None.
-    create_pipeline : bool
+    is_attached : bool
         This is used internally to allow the user to create or attach to a pipeline, and then use the same
         objects in the same way, by default True
     **kwargs : dict
         The user can provide the configuration of the acquisition source directly as kwargs.
     """
     self.log = log
     self.session = session
     self.e2id = e2id
     self.name = name
-    self.data_source = data_source
 
-    self.config = {**config, **kwargs}
-    self.config = {k.upper(): v for k, v in self.config.items()}
+    self.config = {}
+    plugins = config.pop('PLUGINS', plugins)
+
+    if is_attached:
+      assert existing_config is not None, "When attaching to a pipeline, the existing configuration should be found in the heartbeat of the DecentrAI node."
+      assert config == {}, "Cannot provide a configuration when attaching to a pipeline."
+      assert len(kwargs) == 0, "Cannot provide a configuration when attaching to a pipeline."
+      self.config = {k.upper(): v for k, v in existing_config.items()}
+      self.config = self.__pop_ignored_keys_from_config(self.config)
+      self.proposed_config = None
+    else:
+      self.proposed_config = {**config, **kwargs}
+      self.proposed_config = {k.upper(): v for k, v in self.proposed_config.items()}
+      self.proposed_config = self.__pop_ignored_keys_from_config(self.proposed_config)
+    self.__staged_config = None
+
+    self.__was_last_operation_successful = None
+
+    self.proposed_remove_instances = []
+    self.__staged_remove_instances = []
 
     self.on_data_callbacks = []
     self.on_notification_callbacks = []
 
     if on_data is not None:
       self.on_data_callbacks.append(on_data)
     if on_notification is not None:
       self.on_notification_callbacks.append(on_notification)
 
-    self.lst_plugin_instances = []
+    self.lst_plugin_instances: list[Instance] = []
 
-    self.__init_plugins(plugins)
-    self.__maybe_create_new_pipeline_on_box(create_pipeline=create_pipeline)
+    self.__init_plugins(plugins, is_attached)
     return
 
   # Utils
   if True:
-    def __init_plugins(self, plugins):
+    def __init_plugins(self, plugins, is_attached):
       """
       Initialize the plugins list. This method is called at the creation of the pipeline and is used to create the instances of the plugins that are part of the pipeline.
 
       Parameters
       ----------
       plugins : List | None
+        The list of plugins, as they are found in the pipeline configuration dictionary in the heartbeat.
+      is_attached : bool
+        This is used internally to allow the user to create or attach to a pipeline, and then use the same objects in the same way.
 
       """
       if plugins is None:
         return
 
       for dct_signature_instances in plugins:
         signature = dct_signature_instances['SIGNATURE']
         instances = dct_signature_instances['INSTANCES']
         for dct_instance in instances:
-          params = {k: v for k, v in dct_instance.items()}
-          instance_id = params.pop('INSTANCE_ID')
-          instance = Instance(self, instance_id, signature, params=params)
+          config = {k.upper(): v for k, v in dct_instance.items()}
+          instance_id = config.pop('INSTANCE_ID')
+          instance = Instance(self.log, self, instance_id, signature, config=config, is_attached=is_attached)
           self.lst_plugin_instances.append(instance)
         # end for dct_instance
       # end for dct_signature_instances
       return
 
-    def __maybe_create_new_pipeline_on_box(self, *, create_pipeline=True):
+    def __get_proposed_pipeline_config(self):
+      """
+      Construct the proposed pipeline configuration dictionary.
+
+      Returns
+      -------
+      dict
+          The proposed pipeline configuration dictionary.
+      """
+
+      pipeline_config = self.proposed_config if self.proposed_config else self.config
+
+      plugin_dict = self.__construct_plugins_dictionary(skip_instances=self.proposed_remove_instances)
+
+      plugins_list = []
+      for signature, instances in plugin_dict.items():
+        plugins_list.append({
+          'SIGNATURE': signature,
+          'INSTANCES': [instance._get_proposed_config_dictionary() for instance in instances]
+        })
+
+      proposed_pipeline_config = {
+        'NAME': self.name,
+        'DEFAULT_PLUGIN': False,
+        'PLUGINS': plugins_list,
+        **pipeline_config,
+      }
+      return proposed_pipeline_config
+
+    def __register_transactions_for_update(self, session_id: str = None, timeout: float = 0) -> list[Transaction]:
       """
-      Create a new pipeline on the AiXpand node. 
-      This method is called at the creation of the pipeline and is used to create the pipeline on the AiXpand node.
+      Register transactions for updating the pipeline and instances configuration. 
+      This method is called before sending an update pipeline configuration command to the DecentrAI node.
 
       Parameters
       ----------
-      create_pipeline : bool, optional
-          If True, will send a message to the AiXpand node to create this pipeline, by default True
+      session_id : str, optional
+          The session id. A unique id for the session. Defaults to None.
+
+      timeout : int, optional
+          The timeout for the transaction. Defaults to 0.
+
+      Returns
+      -------
+      transactions : list[Transaction]
+          The list of transactions generated.
       """
-      if create_pipeline:
-        self.session._send_command_create_pipeline(
-          worker=self.e2id,
-          pipeline_config=self.__get_pipeline_config(),
-          worker_address=self._get_worker_address(),
+      transactions = []
 
-        )
-      return
+      # TODO: add different responses for different states of the plugin
+      # TODO: maybe this should be introduced as "pre-defined" business plugins, based on a schema
+      #       and the suer can specify them when creating the pipeline
+
+      for instance in self.lst_plugin_instances:
+        if instance._is_tainted():
+          transactions.append(self.session._register_transaction(
+            session_id=session_id,
+            lst_required_responses=instance._get_instance_update_required_responses(),
+            timeout=timeout,
+            on_success_callback=instance._apply_staged_config,
+            on_failure_callback=instance._discard_staged_config,
+          ))
+      # end for register to update instances
+
+      for instance in self.proposed_remove_instances:
+        transactions.append(self.session._register_transaction(
+          session_id=session_id,
+          lst_required_responses=instance._get_instance_remove_required_responses(),
+          timeout=timeout,
+          on_success_callback=lambda: self.__apply_staged_remove_instance(instance),
+          on_failure_callback=lambda fail_reason: self.__discard_staged_remove_instance(instance, fail_reason),
+        ))
+      # end for register to remove instances
+
+      if self.proposed_config is not None:
+        required_responses = [
+          PipelineOKResponse(self.e2id, self.name),
+        ]
+        transactions.append(self.session._register_transaction(
+          session_id=session_id,
+          lst_required_responses=required_responses,
+          timeout=timeout,
+          on_success_callback=self.__apply_staged_config,
+          on_failure_callback=self.__discard_staged_config,
+        ))
+
+      return transactions
 
-    def __get_pipeline_config(self):
+    def __register_transactions_for_delete(self, session_id: str = None, timeout: float = 0) -> list[Transaction]:
       """
-      Construct the pipeline configuration dictionary.
+      Register transactions for deleting the pipeline. 
+      This method is called before sending a delete pipeline command to the DecentrAI node.
+
+      Parameters
+      ----------
+      session_id : str, optional
+          The session id. A unique id for the session. Defaults to None.
+
+      timeout : int, optional
+          The timeout for the transaction. Defaults to 0.
 
       Returns
       -------
-      dict
-          The pipeline configuration dictionary.
+      transactions : list[Transaction]
+          The list of transactions generated.
       """
-      pipeline_config = {
-        'NAME': self.name,
-        'DEFAULT_PLUGIN': False,
-        'PLUGINS': self.__construct_plugins_list(),
-        'TYPE': self.data_source,
-        **self.config,
-      }
-      return pipeline_config
+      transactions = []
+
+      required_responses = [
+        PipelineArchiveResponse(self.e2id, self.name),
+      ]
+      transactions.append(self.session._register_transaction(
+        session_id=session_id,
+        lst_required_responses=required_responses,
+        timeout=timeout,
+        on_success_callback=None,
+        on_failure_callback=None,
+      ))
+
+      return transactions
+
+    def __register_transaction_for_pipeline_command(self, session_id: str = None, timeout: float = 0) -> list[Transaction]:
+      """
+      Register a transaction for a pipeline command. 
+      This method is called before sending a pipeline command to the DecentrAI node.
+
+      Parameters
+      ----------
+      session_id : str, optional
+          The session id. A unique id for the session. Defaults to None.
+
+      timeout : int, optional
+          The timeout for the transaction. Defaults to 0.
+
+      Returns
+      -------
+      transactions : list[Transaction]
+          The list of transactions generated.
+      """
+      transactions = []
+
+      # TODO: implement
+
+      return transactions
 
     def __construct_plugins_list(self):
       """
       Construct the plugins list that will be in the pipeline configuration dictionary.
 
       Returns
       -------
@@ -187,25 +315,111 @@
         plugins.append({
           'SIGNATURE': signature,
           'INSTANCES': [instance._get_config_dictionary() for instance in instances]
         })
       # end for construct plugins list
       return plugins
 
-    def __send_update_config_to_box(self):
+    def __construct_plugins_dictionary(self, skip_instances=None):
       """
-      Send an update pipeline configuration command to the AiXpand node.
+      Construct the plugins dictionary that will be in the pipeline configuration dictionary.
+
+      Returns
+      -------
+      dict
+          The plugins dictionary that will be in the pipeline configuration dictionary.
+      """
+      # plugins = []
+      skip_instances = skip_instances or []
+      dct_signature_instances = {}
+      for instance in self.lst_plugin_instances:
+        if instance in skip_instances:
+          continue
+        if instance.signature not in dct_signature_instances:
+          dct_signature_instances[instance.signature] = []
+        dct_signature_instances[instance.signature].append(instance)
+      # end for construct dct_signature_instances
+
+      return dct_signature_instances
+
+    def __send_update_config_to_box(self, session_id=None):
+      """
+      Send an update pipeline configuration command to the DecentrAI node.
       """
       self.session._send_command_update_pipeline_config(
           worker=self.e2id,
-          pipeline_config=self.__get_pipeline_config(),
-          worker_address=self._get_worker_address(),
+          pipeline_config=self.__get_proposed_pipeline_config(),
+          session_id=session_id
       )
       return
 
+    def __batch_update_instances(self, lst_instances, session_id=None):
+      """
+      Update the configuration of multiple instances at once.
+      ```
+
+      Parameters
+      ----------
+      lst_updates : List[Instance]
+          A list of instances.
+      """
+      lst_updates = []
+
+      for instance in lst_instances:
+        lst_updates.append({
+          PAYLOAD_DATA.NAME: self.name,
+          PAYLOAD_DATA.SIGNATURE: instance.signature,
+          PAYLOAD_DATA.INSTANCE_ID: instance.instance_id,
+          PAYLOAD_DATA.INSTANCE_CONFIG: instance._get_proposed_config_dictionary()
+        })
+
+      self.session._send_command_batch_update_instance_config(
+        worker=self.e2id,
+        lst_updates=lst_updates,
+        session_id=session_id
+      )
+
+    def __pop_ignored_keys_from_config(self, config):
+      """
+      Pop the ignored keys from the configuration.
+
+      Parameters
+      ----------
+      config : dict
+          The configuration dictionary.
+
+      Returns
+      -------
+      dict
+          The configuration dictionary without the ignored keys.
+      """
+      ignored_keys = ["INITIATOR_ADDR", "INITIATOR_ID", "LAST_UPDATE_TIME", "MODIFIED_BY_ADDR", "MODIFIED_BY_ID"]
+      return {k: v for k, v in config.items() if k not in ignored_keys}
+
+    def __get_instance_object(self, signature, instance_id):
+      """
+      Get the instance object by signature and instance id.
+
+      Parameters
+      ----------
+      signature : str
+          The signature of the plugin.
+      instance_id : str
+          The name of the instance.
+
+      Returns
+      -------
+      Instance
+          The instance object.
+      """
+      for instance in self.lst_plugin_instances:
+        if instance.signature == signature and instance.instance_id == instance_id:
+          return instance
+      return None
+
     @staticmethod
     def __custom_exec_on_data(self, instance_id, on_data_callback, data):
       """
       Handle the data received from a custom execution instance. This method is called by the Session object when a message is received from a custom execution instance.
 
       Parameters
       ----------
@@ -225,22 +439,150 @@
 
       if exec_error is not None:
         self.P("Error received from <CUSTOM_EXEC_01:{}>: {}".format(instance_id, exec_error), color="r", verbosity=1)
       if exec_data is not None:
         on_data_callback(self, exec_data, data)
       return
 
-    def _get_worker_address(self):
-      return self.session._get_worker_address(self.e2id)
+    def __apply_staged_remove_instance(self, instance: Instance):
+      """
+      Remove an instance from the pipeline.
+
+      Parameters
+      ----------
+      instance : Instance
+          The instance to be removed.
+      """
+      instance.config = None
+      self.__staged_remove_instances.remove(instance)
+      return
+
+    def __discard_staged_remove_instance(self, instance: Instance, fail_reason: str):
+      """
+      Discard the removal of an instance from the pipeline.
+
+      Parameters
+      ----------
+      instance : Instance
+          The instance to be removed.
+      """
+
+      self.P(
+        f"Discarding staged removal of instance <{instance.signature}:{instance.instance_id}>. Reason: {fail_reason}", color="r")
+
+      self.__staged_remove_instances.remove(instance)
+      self.lst_plugin_instances.append(instance)
+      return
+
+    def __apply_staged_config(self):
+      """
+      Apply the staged configuration to the pipeline.
+      """
+      if self.__staged_config is None:
+        return
+
+      self.P("Deployed pipeline <{}> on <{}>".format(self.name, self.e2id), color="g")
+      self.__was_last_operation_successful = True
+
+      self.config = {**self.config, **self.__staged_config}
+      self.__staged_config = None
+
+      return
+
+    def __apply_staged_instances_config(self):
+      """
+      Apply the staged configuration to the instances.
+      """
+      for instance in self.lst_plugin_instances:
+        instance._apply_staged_config()
+
+      for instance in self.__staged_remove_instances:
+        instance.config = None
+        self.lst_plugin_instances.remove(instance)
+
+      self.__staged_remove_instances = []
+      return
+
+    def __discard_staged_config(self, fail_reason: str):
+      """
+      Discard the staged configuration for the pipeline.
+      """
+
+      self.P(f'Discarding staged configuration for pipeline <{self.name}>. Reason: {fail_reason}', color="r")
+      self.__was_last_operation_successful = False
+
+      self.__staged_config = None
+      self.__staged_remove_instances = []
+      return
+
+    def __stage_proposed_config(self):
+      """
+      Stage the proposed configuration.
+      """
+      if self.proposed_config is not None:
+        if self.__staged_config is not None:
+          raise ValueError(
+            "Pipeline configuration has already been staged, waiting for confirmation from Execution Engine")
+
+        self.__staged_config = self.proposed_config
+        self.proposed_config = None
+
+      for instance in self.lst_plugin_instances:
+        instance._stage_proposed_config()
+
+      self.__staged_remove_instances.extend(self.proposed_remove_instances)
+      self.proposed_remove_instances = []
+
+      self.__was_last_operation_successful = None
+      return
+
+    def __print_proposed_changes(self):
+      """
+      Print the proposed changes to the pipeline.
+      """
+
+      if self.proposed_config is not None:
+        self.P("Proposed changes to pipeline <{}>:".format(self.name), verbosity=1)
+        self.P("  - Current config: {}".format(self.config), verbosity=1)
+        self.P("  - New pipeline config: {}".format(self.proposed_config), verbosity=1)
+
+      if len(self.proposed_remove_instances) > 0:
+        self.P(
+          "  - Remove instances: {}".format([instance.instance_id for instance in self.proposed_remove_instances]), verbosity=1)
+
+      for instance in self.lst_plugin_instances:
+        if instance._is_tainted():
+          self.P("  - Plugin <{}:{}>:".format(instance.signature, instance.instance_id), verbosity=1)
+          self.P("    - Current config: {}".format(instance.config), verbosity=1)
+          self.P("    - Proposed config: {}".format(instance.proposed_config), verbosity=1)
+      return
+
+    def _close(self):
+      """
+      Close the pipeline.
+
+      Returns
+      -------
+      list[Transaction]
+          The list of transactions generated.
+      """
+      transactions = self.__register_transactions_for_delete(timeout=10)
+
+      self.session._send_command_archive_pipeline(
+        worker=self.e2id,
+        pipeline_name=self.name,
+      )
+
+      return transactions
 
   # Message handling
   if True:
     def _on_data(self, signature, instance_id, data):
       """
-      Handle the data received from the AiXpand node. This method is called by the Session object when a message is received from the AiXpand node.
+      Handle the data received from the DecentrAI node. This method is called by the Session object when a message is received from the DecentrAI node.
       This method will call all the `on_data` callbacks of the pipeline and the instance that received the message.
 
       Parameters
       ----------
       signature : str
           The signature of the plugin that sent the message.
       instance_id : str
@@ -254,15 +596,15 @@
 
       # call all instance callbacks
       self.__call_instance_on_data_callbacks(signature, instance_id, data)
       return
 
     def _on_notification(self, signature, instance_id, data):
       """
-      Handle the notification received from the AiXpand node. This method is called by the Session object when a notification is received from the AiXpand node.
+      Handle the notification received from the DecentrAI node. This method is called by the Session object when a notification is received from the DecentrAI node.
 
       Parameters
       ----------
       signature : str
           The signature of the plugin that sent the notification.
       instance_id : str
           The name of the instance that sent the notification.
@@ -311,26 +653,38 @@
       for instance in self.lst_plugin_instances:
         if instance.signature == signature and instance.instance_id == instance_id:
           instance._on_notification(self, data)
       return
 
   # API
   if True:
-    def start_plugin_instance(self, *, signature, instance_id, params={}, on_data=None, on_notification=None, **kwargs) -> Instance:
+    @property
+    def was_last_operation_successful(self):
+      """
+      Return whether the last operation was successful.
+
+      Returns
+      -------
+      bool
+          True if the last operation was successful, False if it failed, None if the ACK has not been received yet
+      """
+      return self.__was_last_operation_successful
+
+    def create_plugin_instance(self, *, signature, instance_id, config={}, on_data=None, on_notification=None, **kwargs) -> Instance:
       """
       Create a new instance of a desired plugin, with a given configuration. This instance is attached to this pipeline, 
-      meaning it processes data from this pipelines data source. Parameters can be passed either in the `params` dict, or as `kwargs`.
+      meaning it processes data from this pipelines data source. Parameters can be passed either in the `config` dict, or as `kwargs`.
 
       Parameters
       ----------
       signature : str
           The name of the plugin signature. This is the name of the desired overall functionality.
       instance_id : str
           The name of the instance. There can be multiple instances of the same plugin, mostly with different parameters
-      params : dict, optional
+      config : dict, optional
           parameters used to customize the functionality. One can change the AI engine used for object detection, 
           or finetune alerter parameters to better fit a camera located in a low light environment.
           Defaults to {}
       on_data : Callable[[Pipeline, dict], None], optional
           Callback that handles messages received from this instance. 
           As arguments, it has a reference to this Pipeline object, along with the payload itself.
           Defaults to None
@@ -346,76 +700,67 @@
 
       Raises
       ------
       Exception
           Plugin instance already exists. 
       """
 
-      # TODO: maybe wait for a confirmation?
       for instance in self.lst_plugin_instances:
         if instance.instance_id == instance_id and instance.signature == signature:
           raise Exception("plugin {} with instance {} already exists".format(signature, instance_id))
 
       # create the new instance and add it to the list
-      instance = Instance(self, instance_id, signature, on_data, on_notification, params, **kwargs)
-      self.lst_plugin_instances.append(instance)
-
-      # send an update config command to the box to create the instance there
-      self.__send_update_config_to_box()
-
-      self.P("Starting plugin {}:{} on {}:{}".format(signature, instance_id, self.e2id, self.name), verbosity=1)
-      self.D("with params {}".format(params), verbosity=2)
+      config = {**config, **kwargs}
+      instance = Instance(self.log, self, instance_id, signature, on_data, on_notification, config, is_attached=False)
 
+      self.lst_plugin_instances.append(instance)
       return instance
 
-    def stop_plugin_instance(self, instance):
+    def remove_plugin_instance(self, instance):
       """
       Stop a plugin instance from this pipeline. 
 
 
       Parameters
       ----------
       instance : Instance
           The instance to be stopped.
 
       """
 
       if instance is None:
-        raise Exception("instance is None")
+        raise Exception("The provided instance is None. Please provide a valid instance")
 
       if instance not in self.lst_plugin_instances:
         raise Exception("plugin  <{}/{}> does not exist on this pipeline".format(instance.signature, instance.instance_id))
 
       # remove the instance from the list
       self.lst_plugin_instances.remove(instance)
-
-      # send an update config command to the box to remove the instance there
-      self.__send_update_config_to_box()
-
+      self.proposed_remove_instances.append(instance)
       return
 
-    def start_custom_plugin(self, *, instance_id, plain_code: str = None, plain_code_path: str = None, custom_code: str = None, params={}, on_data=None, on_notification=None, **kwargs) -> Instance:
+    def create_custom_plugin_instance(self, *, instance_id, plain_code: str = None, plain_code_path: str = None, custom_code: str = None, config={}, on_data=None, on_notification=None, **kwargs) -> Instance:
       """
       Create a new custom execution instance, with a given configuration. This instance is attached to this pipeline, 
       meaning it processes data from this pipelines data source. The code used for the custom instance must be provided
-      either as a string, or as a path to a file. Parameters can be passed either in the params dict, or as kwargs.
+      either as a string, or as a path to a file. Parameters can be passed either in the `config` dict, or as kwargs.
       The custom plugin instance will run periodically. If one desires to execute a custom code only once, use `wait_exec`.
 
       Parameters
       ----------
       instance_id : str
           The name of the instance. There can be multiple instances of the same plugin, mostly with different parameters
       plain_code : str, optional
-          A string containing the entire code that is to be executed remotely on an AiXp node. Defaults to None.
+          A string containing the entire code that is to be executed remotely on an DecentrAI node. Defaults to None.
       plain_code_path : str, optional
-          A string containing the path to the code that is to be executed remotely on an AiXp node. Defaults to None.
+          A string containing the path to the code that is to be executed remotely on an DecentrAI node. Defaults to None.
       custom_code : str | Callable[[CustomPluginTemplate], Any], optional
           A string containing the entire code, a path to a file containing the code as a string or a function with the code.
-          This code will be executed remotely on an AiXp node. Defaults to None.
-      params : dict, optional
+          This code will be executed remotely on an DecentrAI node. Defaults to None.
+      config : dict, optional
           parameters used to customize the functionality. One can change the AI engine used for object detection, 
           or finetune alerter parameters to better fit a camera located in a low light environment.
           Defaults to {}
       on_data : Callable[[Pipeline, dict], None], optional
           Callback that handles messages received from this instance. 
           As arguments, it has a reference to this Pipeline object, along with the payload itself.
           Defaults to None
@@ -470,52 +815,87 @@
           raise Exception("custom_code is not a string or a callable")
         # endif get plain code
 
       b64code = CodeUtils().code_to_base64(plain_code)
 
       def callback(pipeline, data): return self.__custom_exec_on_data(pipeline, instance_id, on_data, data)
 
-      return self.start_plugin_instance(
+      return self.create_plugin_instance(
           signature='CUSTOM_EXEC_01',
           instance_id=instance_id,
-          params={
+          config={
               'CODE': b64code,
-              **params
+              **config
           },
           on_data=callback,
           on_notification=on_notification,
           **kwargs
       )
 
-    def stop_custom_instance(self, instance):
+    def deploy(self, with_confirmation=True, wait_confirmation=True, timeout=10):
       """
-      Stop a custom execution instance from this pipeline.
-      This method is an alias for `stop_plugin_instance`.
+      This method is used to deploy the pipeline on the DecentrAI node. 
+      Here we collect all the proposed configurations and send them to the DecentrAI node.
+      All proposed configs become staged configs.
+      After all responses, apply the staged configs to finish the transaction. 
+      """
+      # generate a unique session id for this deploy operation
+      # this session id will be used to track the transactions
+
+      # step 0: print the proposed changes
+      self.__print_proposed_changes()
+
+      # step 1: register transactions for updates
+      transactions = []
+
+      if with_confirmation:
+        transactions: list[Transaction] = self.__register_transactions_for_update(timeout=timeout)
+
+      # step 1: send the proposed config to the box
+      pipeline_config_changed = self.proposed_config is not None
+      have_to_remove_instances = len(self.proposed_remove_instances) > 0
+      have_new_instances = any([instance._is_tainted() and len(instance.config) == 0
+                                for instance in self.lst_plugin_instances])
+      if pipeline_config_changed or have_to_remove_instances or have_new_instances:
+        # updated pipeline config or deleted instances
+        self.__send_update_config_to_box()
+      elif any([instance._is_tainted() for instance in self.lst_plugin_instances]):
+        # updated instances only
+        tainted_instances = [instance for instance in self.lst_plugin_instances if instance._is_tainted()]
+        self.__batch_update_instances(tainted_instances)
+      else:
+        return
 
-      Parameters
-      ----------
-      instance : Instance
-          The instance to be stopped.
+      # step 3: stage the proposed config
+      self.__stage_proposed_config()
 
-      """
-      self.stop_plugin_instance(instance)
+      # step 3: wait for the box to respond
+      if with_confirmation and wait_confirmation:
+        self.session.wait_for_transactions(transactions)
+
+      # step 4: apply the staged config
+      if not with_confirmation:
+        self.__apply_staged_config()
+        self.__apply_staged_instances_config()
+
+      return
 
-    def wait_exec(self, *, plain_code: str = None, plain_code_path: str = None, params={}):
+    def wait_exec(self, *, plain_code: str = None, plain_code_path: str = None, config={}):
       """
       Create a new REST-like custom execution instance, with a given configuration. This instance is attached to this pipeline, 
-      meaning it processes data from this pipelines data source. The code used for the custom instance must be provided either as a string, or as a path to a file. Parameters can be passed either in the params dict, or as kwargs.
+      meaning it processes data from this pipelines data source. The code used for the custom instance must be provided either as a string, or as a path to a file. Parameters can be passed either in the config dict, or as kwargs.
       The REST-like custom plugin instance will execute only once. If one desires to execute a custom code periodically, use `start_custom_plugin`.
 
       Parameters
       ----------
       plain_code : str, optional
-          A string containing the entire code that is to be executed remotely on an AiXp node, by default None
+          A string containing the entire code that is to be executed remotely on an DecentrAI node, by default None
       plain_code_path : str, optional
-          A string containing the path to the code that is to be executed remotely on an AiXp node, by default None
-      params : dict, optional
+          A string containing the path to the code that is to be executed remotely on an DecentrAI node, by default None
+      config : dict, optional
           parameters used to customize the functionality, by default {}
 
       Returns
       -------
       Tuple[Any, Any]
           a tuple containing the result of the execution and the error, if any. 
           If the execution completed successfully, the `error` is None, and the `result` is the returned value of the custom code.
@@ -549,49 +929,48 @@
           result = data['specificValue']['rest_execution_result']
           error = data['specificValue']['rest_execution_error']
           finished = True
         return
 
       b64code = CodeUtils().code_to_base64(plain_code)
       instance_id = self.name + "_rest_custom_exec_synchronous_0"
-      params = {
+      config = {
           'REQUEST': {
               'DATA': {
                   'CODE': b64code,
               },
               'TIMESTAMP': self.log.time_to_str()
           },
           'RESULT_KEY': 'REST_EXECUTION_RESULT',
           'ERROR_KEY': 'REST_EXECUTION_ERROR',
-          **params
+          **config
       }
 
-      instance = self.start_plugin_instance(
+      instance = self.create_plugin_instance(
           signature='REST_CUSTOM_EXEC_01',
           instance_id=instance_id,
-          params=params,
+          config=config,
           on_data=on_data
       )
       while not finished:
         pass
 
       # stop the stream
       instance.close()
 
       return result, error
 
     def close(self):
       """
       Close the pipeline, stopping all the instances associated with it.
       """
-      # remove callbacks
-      self.session._send_command_archive_pipeline(
-        worker=self.e2id,
-        pipeline_name=self.name,
-      )
+
+      transactions = self._close()
+
+      self.session.wait_for_transactions(transactions)
       return
 
     def P(self, *args, **kwargs):
       """
       Print info to stdout.
       """
       return self.log.P(*args, **kwargs)
@@ -599,17 +978,17 @@
     def D(self, *args, **kwargs):
       """
       Call the `Logger.D` method.
       If using the default Logger, this call will print debug info to stdout if `silent` is set to `False`.
       The logger object is passed from the Session object to the Pipeline object when creating
       it with `create_pipeline` or `attach_to_pipeline`.
       """
-      return self.log.D(*args, **kwargs)
+      return self.session.D(*args, **kwargs)
 
-    def attach_to_instance(self, signature, instance_id, on_data=None, on_notification=None) -> Instance:
+    def attach_to_plugin_instance(self, signature, instance_id, on_data=None, on_notification=None) -> Instance:
       """
       Attach to an existing instance on this pipeline. 
       This method is useful when one wishes to attach an 
       `on_data` and `on_notification` callbacks to said instance.
 
       Parameters
       ----------
@@ -652,15 +1031,15 @@
         instance._add_on_data_callback(on_data)
 
       if on_notification is not None:
         instance._add_on_notification_callback(on_notification)
 
       return found_instance
 
-    def attach_to_custom_instance(self, instance_id, on_data=None, on_notification=None) -> Instance:
+    def attach_to_custom_plugin_instance(self, instance_id, on_data=None, on_notification=None) -> Instance:
       """
       Attach to an existing custom execution instance on this pipeline. 
       This method is useful when one wishes to attach an 
       `on_data` and `on_notification` callbacks to said instance.
 
       Parameters
       ----------
@@ -684,20 +1063,20 @@
           the pipeline does not contain any custom plugin.
       Exception
           The pipeline does not contain the desired instance.
       """
 
       def callback(pipeline, data): return self.__custom_exec_on_data(pipeline, instance_id, on_data, data)
 
-      return self.attach_to_instance("CUSTOM_EXEC_01", instance_id, callback, on_notification)
+      return self.attach_to_plugin_instance("CUSTOM_EXEC_01", instance_id, callback, on_notification)
 
     def detach_from_instance(self, instance: Instance):
       # search for the instance in the list
       if instance is None:
-        raise Exception("instance is None")
+        raise Exception("The provided instance is None. Please provide a valid instance")
 
       instance._reset_on_data_callback()
       instance._reset_on_notification_callback()
       return
 
     def update_acquisition_parameters(self, config={}, **kwargs):
       """
@@ -705,71 +1084,207 @@
       Parameters can be passed either in the `config` dict, or as `kwargs`.
 
       Parameters
       ----------
       config : dict, optional
           The new configuration of the acquisition source, by default {}
       """
-      self.config = {
-          **self.config,
-          **config,
-          **kwargs
-      }
-      self.__send_update_config_to_box()
-
-      return
+      if self.__staged_config is not None:
+        raise ValueError("Pipeline configuration has already been staged, waiting for confirmation from Execution Engine")
 
-    def batch_update_instances(self, lst_updates):
-      """
-      Update the configuration of multiple instances at once.
-      This method is useful when one wants to update the configuration of multiple instances at once, 
-        while only sending one message to the AiXpand node.
+      if self.proposed_config is None:
+        self.proposed_config = {}
 
-      Example:
-      ```
-      instance1 : Instance
-      instance2 : Instance
+      self.proposed_config = {**self.proposed_config, **config, **{k.upper(): v for k, v in kwargs.items()}}
+      self.proposed_config = self.__pop_ignored_keys_from_config(self.proposed_config)
 
-      config1 : dict
-      config2 : dict
+      for k, v in self.config.items():
+        if k in self.proposed_config:
+          if self.proposed_config[k] == v:
+            del self.proposed_config[k]
 
-      update1 = instance1.update_instance_config(config1)
-      update2 = instance2.update_instance_config(config2)
+      if len(self.proposed_config) == 0:
+        self.proposed_config = None
 
-      lst_updates = [update1, update2]
-      pipeline.batch_update_instances(lst_updates)
-      ```
+      return
 
-      Parameters
-      ----------
-      lst_updates : List[dict]
-          A list of dictionaries containing the updates for each instance.
+    def send_pipeline_command(self, command, payload={}, command_params={}, wait_for_confirmation=True, timeout=10) -> list[Transaction]:
+      # TODO: test if pipeline command works okay
       """
-      self.session._send_command_batch_update_instance_config(
-        worker=self.e2id,
-        lst_updates=lst_updates,
-        worker_address=self._get_worker_address(),
-      )
+      Send a pipeline command to the DecentrAI node.
+      This command can block until the command is confirmed by the DecentrAI node.
 
-    def send_pipeline_command(self, command, payload={}, command_params={}):
-      # TODO: test if this is oke like this
-      """
-      Send a pipeline command to the AiXpand node.
+      Example:
+      --------
+      ```python
+      pipeline.send_pipeline_command('START', wait_for_confirmation=True)
+
+      transactions_p1 = pipeline1.send_pipeline_command('START', wait_for_confirmation=False)
+      transactions_p2 = pipeline2.send_pipeline_command('START', wait_for_confirmation=False)
+      # wait for both commands to be confirmed, but after both commands are sent
+      session.wait_for_transactions(transactions_p1 + transactions_p2)
+      ```
 
       Parameters
       ----------
       command : str
           The name of the command.
       payload : dict, optional
           The payload of the command, by default {}
       command_params : dict, optional
           The parameters of the command, by default {}
+      wait_for_confirmation : bool, optional
+          Whether to wait for the confirmation of the command, by default False
+      timeout : int, optional
+          The timeout for the transaction, by default 10    
+
+      Returns
+      -------
+      list[Transaction] | None
+          The list of transactions generated, or None if `wait_for_confirmation` is False.
       """
+      transactions = self.__register_transaction_for_pipeline_command(timeout=timeout)
+
       self.session._send_command_pipeline_command(
         worker=self.e2id,
         pipeline_name=self.name,
         command=command,
         payload=payload,
         command_params=command_params,
-        worker_address=self._get_worker_address(),
       )
+
+      if wait_for_confirmation:
+        self.session.wait_for_transactions(transactions)
+      else:
+        return transactions
+      return
+
+    def create_or_attach_to_plugin_instance(self, *, signature, instance_id, config={}, on_data=None, on_notification=None, **kwargs) -> Instance:
+      """
+      Create a new instance of a desired plugin, with a given configuration, or attach to an existing instance.
+
+      Parameters
+      ----------
+      signature : str
+          The name of the plugin signature. This is the name of the desired overall functionality.
+      instance_id : str
+          The name of the instance. There can be multiple instances of the same plugin, mostly with different parameters
+      config : dict, optional
+          parameters used to customize the functionality. One can change the AI engine used for object detection, 
+          or finetune alerter parameters to better fit a camera located in a low light environment.
+          Defaults to {}
+      on_data : Callable[[Pipeline, dict], None], optional
+          Callback that handles messages received from this instance. 
+          As arguments, it has a reference to this Pipeline object, along with the payload itself.
+          Defaults to None
+      on_notification : Callable[[Pipeline, dict], None], optional
+          Callback that handles notifications received from this instance. 
+          As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+          Defaults to None
+
+      Returns
+      -------
+      instance : Instance
+          An `Instance` object.
+      """
+      try:
+        instance = self.attach_to_plugin_instance(signature, instance_id, on_data, on_notification)
+        instance.update_instance_config(config, kwargs)
+      except Exception:
+        instance = self.create_plugin_instance(
+          signature=signature,
+          instance_id=instance_id,
+          config=config,
+          on_data=on_data,
+          on_notification=on_notification,
+          **kwargs
+        )
+      return instance
+
+    def create_or_attach_to_custom_plugin_instance(self, *, instance_id, plain_code: str = None, plain_code_path: str = None, custom_code: str = None, config={}, on_data=None, on_notification=None, **kwargs) -> Instance:
+      """
+      Create a new instance of a desired plugin, with a given configuration, or attach to an existing instance. 
+
+      Parameters
+      ----------
+      signature : str
+          The name of the plugin signature. This is the name of the desired overall functionality.
+      instance_id : str
+          The name of the instance. There can be multiple instances of the same plugin, mostly with different parameters
+      config : dict, optional
+          parameters used to customize the functionality. One can change the AI engine used for object detection, 
+          or finetune alerter parameters to better fit a camera located in a low light environment.
+          Defaults to {}
+      on_data : Callable[[Pipeline, dict], None], optional
+          Callback that handles messages received from this instance. 
+          As arguments, it has a reference to this Pipeline object, along with the payload itself.
+          Defaults to None
+      on_notification : Callable[[Pipeline, dict], None], optional
+          Callback that handles notifications received from this instance. 
+          As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+          Defaults to None
+
+      Returns
+      -------
+      instance : Instance
+          An `Instance` object.
+      """
+
+      try:
+        instance = self.attach_to_custom_plugin_instance(instance_id, on_data, on_notification)
+        instance.update_instance_config(config, **kwargs)
+      except:
+        instance = self.create_custom_plugin_instance(
+          instance_id=instance_id,
+          plain_code=plain_code,
+          plain_code_path=plain_code_path,
+          custom_code=custom_code,
+          config=config,
+          on_data=on_data,
+          on_notification=on_notification,
+          **kwargs
+        )
+      return instance
+
+    def update_full_configuration(self, config={}):
+      """
+      Update the full configuration of this pipeline.
+      Parameters are passed in the `config` dict.
+      We do not support kwargs yet because it makes it difficult to check priority of dictionary, merging values, etc.
+
+      Parameters
+      ----------
+      config : dict, optional
+          The new configuration of the pipeline, by default {}
+      """
+      if self.__staged_config is not None:
+        raise ValueError("Pipeline configuration has already been staged, waiting for confirmation from Execution Engine")
+
+      # pop the illegal to modify keys
+      config.pop('NAME', None)
+      config.pop('TYPE', None)
+      plugins = config.pop('PLUGINS', {})
+
+      self.update_acquisition_parameters(config)
+
+      new_plugins = []
+      for dct_signature_instances in plugins:
+        signature = dct_signature_instances['SIGNATURE']
+        instances = dct_signature_instances['INSTANCES']
+        for dct_instance in instances:
+          instance_id = dct_instance['INSTANCE_ID']
+          new_plugins.append((signature, instance_id))
+          instance_object = self.__get_instance_object(signature, instance_id)
+
+          if instance_object is None:
+            self.create_plugin_instance(signature=signature, instance_id=instance_id, config=dct_instance)
+          else:
+            instance_object.update_instance_config(dct_instance)
+        # end for dct_instance
+      # end for dct_signature_instances
+
+      # now check if we have to remove any instances
+      for instance in self.lst_plugin_instances:
+        if (instance.signature, instance.instance_id) not in new_plugins:
+          self.remove_plugin_instance(instance)
+      # end for instance
       return
```

### Comparing `pye2-0.7.9/PyE2/base/plugin_template.py` & `pye2-0.8.0/PyE2/base/plugin_template.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/base/payload/payload.py` & `pye2-0.8.0/PyE2/base/payload/payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import numpy as np
 
 
 class Payload(UserDict):
   """
   This class enriches the default python dict, providing
-  helpful methods to process the payloads received from AiXp nodes.
+  helpful methods to process the payloads received from DecentrAI nodes.
   """
 
-  def get_image_as_np(self, key='IMG'):
+  def get_images_as_np(self, key='IMG') -> list:
     """
     Extract the image from the payload.
     The image is returned as a numpy array.
 
     Parameters
     ----------
     key : str, optional
@@ -23,20 +23,20 @@
         Can be modified if the user wants to extract an image from a different key
 
     Returns
     -------
     NDArray[Any] | None
         The image if it was found or None otherwise.
     """
-    image = self.get_image_as_PIL(key)
-    if image is not None:
-      image = np.array(image)
-    return image
+    images = self.get_images_as_PIL(key)
+    if images is not None:
+      images = [np.array(image) for image in images]
+    return images
 
-  def get_image_as_PIL(self, key='IMG'):
+  def get_images_as_PIL(self, key='IMG') -> list:
     """
     Extract the image from the payload.
     The image is returned as a PIL image.
 
     Parameters
     ----------
     key : str, optional
```

### Comparing `pye2-0.7.9/PyE2/bc/base.py` & `pye2-0.8.0/PyE2/bc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 class BCct:
   SIGN      = 'EE_SIGN'
   SENDER    = 'EE_SENDER'
   HASH      = 'EE_HASH'
   
-  ADDR_PREFIX   = "aixp_"
+  ADDR_PREFIX_OLD = "aixp_"
+  ADDR_PREFIX   = "0xai_"
   
   K_PEM_FILE = 'PEM_FILE'
   K_PASSWORD = 'PASSWORD'
   K_PEM_LOCATION = 'PEM_LOCATION'
   
   ERR_UNAVL_MSG = "Missing signature/sender data"
   ERR_UNAVL = 1
@@ -31,15 +32,15 @@
   ERR_UNAVL = 1000
 
   ERR_SIGN_MSG = "Bad signature"
   ERR_UNAVL = 1001
   
   AUTHORISED_ADDRS = 'authorized_addrs'
   
-  DEFAULT_INFO = 'AiXp handshake data'
+  DEFAULT_INFO = '0xai handshake data'
   
   
 class _DotDict(dict):
   __getattr__ = dict.__getitem__
   __setattr__ = dict.__setitem__
   __delattr__ = dict.__delitem__
   
@@ -485,17 +486,36 @@
         lst_allowed = fh.readlines()
     else:
       full_path = os.path.abspath(fn)
       self.P("WARNING: no `{}` file found. Creating empty one.".format(full_path), verbosity=1)
       with open(fn, 'wt') as fh:
         fh.write('\n')
     lst_allowed = [x.strip().split(' ')[0] for x in lst_allowed]
+    lst_allowed = [self._remove_prefix(x) for x in lst_allowed if x != '']
     return lst_allowed
       
-  
+  def _remove_prefix(self, address):
+    """
+    Removes the prefix from the address
+
+    Parameters
+    ----------
+    address : str
+      the text address.
+
+    Returns
+    -------
+    address : str
+      the address without the prefix.
+    """
+    if address.startswith(BCct.ADDR_PREFIX):
+      address = address[len(BCct.ADDR_PREFIX):]
+    elif address.startswith(BCct.ADDR_PREFIX_OLD):
+      address = address[len(BCct.ADDR_PREFIX_OLD):]
+    return address
   
   def _pk_to_address(self, public_key):
     """
     Given a pk object will return the simple text address.
     
     OBS: Should be overwritten in particular implementations using X962
 
@@ -533,15 +553,15 @@
 
     Returns
     -------
     pk : pk
       the pk object.
 
     """
-    simple_address = address.replace(BCct.ADDR_PREFIX, '')
+    simple_address = self._remove_prefix(address)
     bpublic_key = self._text_to_binary(simple_address)
     # below works for DER / SubjectPublicKeyInfo
     public_key = serialization.load_der_public_key(bpublic_key)
     return public_key
   
   
   def _text_to_sk(self, source, from_file=False, password=None):
@@ -944,16 +964,17 @@
     if return_full_info:
       result = verify_msg
     else:
       result = verify_msg.ok
     return result
   
   
-  def is_allowed(self, sender_address):
-    is_allowed = sender_address in self.allowed_list or sender_address == self.address
+  def is_allowed(self, sender_address: str):
+    to_search_address = self._remove_prefix(sender_address)
+    is_allowed = to_search_address in self.allowed_list or to_search_address == self._remove_prefix(self.address)
     return is_allowed
   
   
   def encrypt(self, data, destination):
     """
     Encrypts the data for a given destination
```

### Comparing `pye2-0.7.9/PyE2/bc/ec.py` & `pye2-0.8.0/PyE2/bc/ec.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
     Returns
     -------
     pk : EllipticCurvePublicKey
       the pk object.
 
     """
-    simple_address = address.replace(BCct.ADDR_PREFIX, '')
+    simple_address = self._remove_prefix(address)
     bpublic_key = self._text_to_binary(simple_address)
     public_key = ec.EllipticCurvePublicKey.from_encoded_point(
       curve=ec.SECP256K1(), 
       data=bpublic_key
     )
     return public_key
```

### Comparing `pye2-0.7.9/PyE2/comm/amqp_wrapper.py` & `pye2-0.8.0/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/comm/mqtt_wrapper.py` & `pye2-0.8.0/PyE2/comm/mqtt_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # PAHO
-#TODO: implement config validation and base config format
+# TODO: implement config validation and base config format
+# TODO: add queue for to_send messages
 
-import paho.mqtt.client as mqtt
-import traceback
-
-from paho.mqtt import __version__ as mqtt_version
-
-from collections import OrderedDict, deque
+# TODO: adding a lock for accessing self._mqttc should solve some of the bugs, but it introduces a new one
+# basically, when a user thread calls send, they should acquire the lock for the self._mqttc object
+# and use it to send messages. However, if the mqttc has loop started but did not connect, the lock will
+# prevent the client from ever connecting.
 
-from select import select
+import traceback
+from collections import deque
+from threading import Lock
 from time import sleep
 
+import paho.mqtt.client as mqtt
+from paho.mqtt import __version__ as mqtt_version
 
-from ..const import COLORS, COMMS, BASE_CT, PAYLOAD_CT
+from ..const import BASE_CT, COLORS, COMMS, PAYLOAD_CT
 from ..utils import resolve_domain_or_ip
 
 
 class MQTTWrapper(object):
   def __init__(self,
                log,
                config,
@@ -163,41 +166,82 @@
     cfg[COMMS.TOPIC] = topic
     return cfg
 
   @property
   def connection(self):
     return self._mqttc
 
+  def __get_client_id(self):
+    mqttc = self._mqttc
+    client_id = str(mqttc._client_id) if mqttc is not None else 'None'
+    return client_id
+
+  def __create_mqttc_object(self, comtype, client_uid):
+    client_id = self._connection_name + '_' + comtype + '_' + client_uid
+    if mqtt_version.startswith('2'):
+      mqttc = mqtt.Client(
+        callback_api_version=mqtt.CallbackAPIVersion.VERSION2,
+        client_id=client_id,
+        clean_session=True,
+      )
+    else:
+      mqttc = mqtt.Client(
+        client_id=client_id,
+        clean_session=True
+      )
+
+    mqttc.username_pw_set(
+      username=self.cfg_user,
+      password=self.cfg_pass
+    )
+
+    mqttc.on_connect = self._callback_on_connect
+    mqttc.on_disconnect = self._callback_on_disconnect
+    mqttc.on_message = self._callback_on_message
+    mqttc.on_publish = self._callback_on_publish
+
+    return mqttc
+
+  def __sleep_until_connected(self, max_sleep, sleep_time):
+    for sleep_iter in range(1, int(max_sleep / sleep_time) + 1):
+      sleep(sleep_time)
+      if self.connected:
+        break
+    # endfor
+    return sleep_iter
+
   def _callback_on_connect(self, client, userdata, flags, rc, *args, **kwargs):
     self.connected = False
     if rc == 0:
       self.connected = True
-      mqttc = self._mqttc
-      client_id = str(mqttc._client_id) if mqttc is not None else 'None'
-      self.P("Conn ok clntid '{}' with code: {}".format(client_id, rc), color='g', verbosity=1)
+      self.P("Conn ok clntid '{}' with code: {}".format(
+        self.__get_client_id(), rc), color='g', verbosity=1)
     return
 
   def _callback_on_disconnect(self, client, userdata, rc, *args, **kwargs):
     """
     Tricky callback
 
     we can piggy-back ride the client with flags:
-      client.connected_flag = False 
+      client.connected_flag = False
       client.disconnect_flag = True
     """
+
+    if mqtt_version.startswith('2'):
+      # In version 2, on_disconnect has a different order of parameters, and rc is passed as the 4th parameter
+      # check https://eclipse.dev/paho/files/paho.mqtt.python/html/migrations.html for more info
+      rc = args[0]
     if rc == 0:
-      self.P('Gracefull disconn (reason_code={})'.format(rc), color='m', verbosity=1)
-      str_error = "Gracefull disconn."
+      self.P('Graceful disconnect (reason_code={})'.format(rc), color='m', verbosity=1)
+      str_error = "Graceful disconnect."
     else:
       str_error = mqtt.error_string(rc) + ' (reason_code={})'.format(rc)
-      mqttc = self._mqttc
-      client_id = str(mqttc._client_id) if mqttc is not None else 'None'
-      self.P("Unexpected disconn for client id '{}': {}".format(
-        client_id, str_error), color='r', verbosity=1,
-      )
+      self.P("Unexpected disconnect for client id '{}': {}".format(
+        self.__get_client_id(), str_error), color='r', verbosity=1)
+
     if self._disconnected_counter > 0:
       self.P("Trying to determine IP of target server...", verbosity=1)
       ok, str_ip, str_domain = resolve_domain_or_ip(self.cfg_host)
       msg = '  Multiple conn loss ({} disconnects so far), showing previous 10:\n{}'.format(
         self._disconnected_counter, self.last_disconnect_log
       )
       server_port = "*****  Please check server connection: {}:{} {} *****".format(
@@ -207,17 +251,18 @@
       msg += "\n\n{}\n{}\n{}".format("*" * len(server_port), server_port, "*" * len(server_port))
       self.P(msg, color='r', verbosity=1)
     # endif multiple disconnects
     self.connected = False
     self.disconnected = True
     self._disconnected_log.append((self.log.time_to_str(), str_error))
     self._disconnected_counter += 1
-    self.last_disconnect_log = '\n'.join([f"* Comm error '{x2}' occured at {x1}" for x1, x2 in self._disconnected_log])
+    self.last_disconnect_log = '\n'.join([f"* Comm error '{x2}' occurred at {x1}" for x1, x2 in self._disconnected_log])
     # we need to stop the loop otherwise the client thread will keep working
     # so we call release->loop_stop
+
     self.release()
     return
 
   def _callback_on_publish(self, client, userdata, mid, *args, **kwargs):
     return
 
   def _callback_on_message(self, client, userdata, message, *args, **kwargs):
@@ -237,103 +282,101 @@
       self._post_default_on_message()
     return
 
   def get_connection_issues(self):
     return {x1: x2 for x1, x2 in self._disconnected_log}
 
   def server_connect(self, max_retries=5):
+    max_sleep = 2
+    sleep_time = 0.01
     nr_retry = 1
     has_connection = False
     exception = None
     sleep_iter = None
     comtype = self._comm_type[:7] if self._comm_type is not None else 'CUSTOM'
 
     while nr_retry <= max_retries:
       try:
+        # 1. create a unique client id
         client_uid = self.log.get_unique_id()
-        client_id = self._connection_name + '_' + comtype + '_' + client_uid
-        if mqtt_version.startswith('2'):
-          self._mqttc = mqtt.Client(
-            callback_api_version=mqtt.CallbackAPIVersion.VERSION2,
-            client_id=client_id,
-            clean_session=True
-          )
-        else:
-          self._mqttc = mqtt.Client(
-            client_id=client_id,
-            clean_session=True
-          )
 
-        self._mqttc.username_pw_set(
-          username=self.cfg_user,
-          password=self.cfg_pass
-        )
-
-        self._mqttc.on_connect = self._callback_on_connect
-        self._mqttc.on_disconnect = self._callback_on_disconnect
-        self._mqttc.on_message = self._callback_on_message
-        self._mqttc.on_publish = self._callback_on_publish
+        # 2. create the mqtt client object (with callbacks set)
+        self._mqttc = self.__create_mqttc_object(comtype, client_uid)
+
         # TODO: more verbose logging including when there is no actual exception
+        # 3. connect to the server
         self._mqttc.connect(host=self.cfg_host, port=self.cfg_port)
 
+        # 4. start the loop in another thread
         if self._mqttc is not None:
           self._mqttc.loop_start()  # start loop in another thread
 
-        sleep_time = 0.01
-        max_sleep = 2
-        for sleep_iter in range(1, int(max_sleep / sleep_time) + 1):
-          sleep(sleep_time)
-          if self.connected:
-            break
-        # endfor
+        # 5. wait until connected
+        sleep_iter = self.__sleep_until_connected(max_sleep=max_sleep, sleep_time=sleep_time)
 
         has_connection = self.connected
       except Exception as e:
         exception = e
         if self.debug_errors:
-          self.P(e, color='r', verbosity=1)
+          self.P(exception, color='r', verbosity=1)
           self.P(traceback.format_exc(), color='r', verbosity=1)
 
       # end try-except
 
       if has_connection:
         break
 
       nr_retry += 1
     # endwhile
-    if self._mqttc is not None and hasattr(self._mqttc, '_thread') and self._mqttc._thread is not None:
-      self._mqttc._thread.name = self._connection_name + '_' + comtype + '_' + client_uid
-      self._thread_name = self._mqttc._thread.name
+
+    # set thread name ; useful for debugging
+    mqttc = self._mqttc
+    if mqttc is not None and hasattr(mqttc, '_thread') and mqttc._thread is not None:
+      mqttc._thread.name = self._connection_name + '_' + comtype + '_' + client_uid
+      self._thread_name = mqttc._thread.name
 
     if has_connection:
       msg = "MQTT conn ok by '{}' in {:.1f}s - {}:{}".format(
-        self._thread_name, sleep_iter * sleep_time, self.cfg_host, self.cfg_port
+        self._thread_name,
+        sleep_iter * sleep_time,
+        self.cfg_host,
+        self.cfg_port
       )
       msg_type = PAYLOAD_CT.STATUS_TYPE.STATUS_NORMAL
       self._nr_full_retries = 0
-      self.P(msg, color='g', verbosity=1)
+
+      self.P(msg)
+
     else:
       reason = exception
       if reason is None:
         reason = " max retries in {:.1f}s".format(sleep_iter * sleep_time)
+
       self._nr_full_retries += 1
       msg = 'MQTT (Paho) conn to {}:{} failed after {} retr ({} trials) (reason:{})'.format(
-        self.cfg_host, self.cfg_port, nr_retry, self._nr_full_retries, reason
+        self.cfg_host,
+        self.cfg_port,
+        nr_retry,
+        self._nr_full_retries,
+        reason
       )
       msg_type = PAYLOAD_CT.STATUS_TYPE.STATUS_EXCEPTION
       self.P(msg, color='r', verbosity=1)
-      # now register failure
+
     # endif
 
     dct_ret = {
       'has_connection': has_connection,
       'msg': msg,
       'msg_type': msg_type
     }
 
+    # if release was not called from on_disconnect, basically
+    # this method of checking self._mqttc is not None is not
+    # very reliable, as race conditions can occur
     if self._mqttc is not None and not has_connection:
       self.release()
 
     return dct_ret
 
   def get_thread_name(self):
     return self._thread_name
@@ -346,19 +389,20 @@
     nr_retry = 1
     has_connection = False
     exception = None
     topic = self.recv_channel_def[COMMS.TOPIC]
 
     while nr_retry <= max_retries:
       try:
-        self._mqttc.subscribe(
-          topic=topic,
-          qos=self.cfg_qos
-        )
-        has_connection = True
+        if self._mqttc is not None:
+          self._mqttc.subscribe(
+            topic=topic,
+            qos=self.cfg_qos
+          )
+          has_connection = True
       except Exception as e:
         exception = e
 
       if has_connection:
         break
 
       sleep(1)
@@ -381,18 +425,19 @@
 
     return dct_ret
 
   def receive(self):
     return
 
   def send(self, message):
-    if self._mqttc is None:
+    mqttc = self._mqttc
+    if mqttc is None:
       return
 
-    result = self._mqttc.publish(
+    result = mqttc.publish(
       topic=self.send_channel_def[COMMS.TOPIC],
       payload=message,
       qos=self.cfg_qos
     )
 
     ####
     self.D("Sent message '{}'".format(message))
@@ -401,18 +446,24 @@
     if result.rc == mqtt.MQTT_ERR_QUEUE_SIZE:
       raise ValueError('Message is not queued due to ERR_QUEUE_SIZE')
 
     return
 
   def release(self):
     try:
-      self._mqttc.disconnect()
-      self._mqttc.loop_stop()  # stop the loop thread
-      self.connected = False
-      del self._mqttc
+      mqttc = self._mqttc
+
+      if mqttc is not None:
+        self._mqttc.disconnect()
+        self._mqttc.loop_stop()  # stop the loop thread
       self._mqttc = None
+      self.connected = False
       msg = 'MQTT (Paho) connection released.'
     except Exception as e:
       msg = 'MQTT (Paho) exception while releasing connection: `{}`'.format(str(e))
 
+    self.P(msg)
+
+    # TODO: method should return None; update code in core to reflect this
     dct_ret = {'msgs': [msg]}
+
     return dct_ret
```

### Comparing `pye2-0.7.9/PyE2/const/base.py` & `pye2-0.8.0/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/const/comms.py` & `pye2-0.8.0/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/const/heartbeat.py` & `pye2-0.8.0/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/const/payload.py` & `pye2-0.8.0/PyE2/const/payload.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,17 @@
   PIPELINE_ARCHIVE_OK = PIPELINE_DCT_CONFIG_OK + 1  # archiving is ok
   PIPELINE_ARCHIVE_FAILED = -PIPELINE_ARCHIVE_OK
 
   # plugins from 100 to 999
   PLUGIN_CONFIG_OK = 100
   PLUGIN_CONFIG_FAILED = -PLUGIN_CONFIG_OK
 
+  PLUGIN_INSTANCE_COMMAND_OK = 101
+  PLUGIN_INSTANCE_COMMAND_FAILED = -PLUGIN_INSTANCE_COMMAND_OK
+
   PLUGIN_PAUSE_OK = 110
   PLUGIN_PAUSE_FAILED = -PLUGIN_PAUSE_OK
 
   PLUGIN_RESUME_OK = 111
   PLUGIN_RESUME_FAILED = -PLUGIN_RESUME_OK
 
   PLUGIN_WORKING_HOURS_SHIFT_START = 112
@@ -78,14 +81,16 @@
     PIPELINE_DCT_CONFIG_OK: "PIPELINE_DCT_CONFIG_OK",
     PIPELINE_DCT_CONFIG_FAILED: "PIPELINE_DCT_CONFIG_FAILED",
     PIPELINE_ARCHIVE_OK: "PIPELINE_ARCHIVE_OK",
     PIPELINE_ARCHIVE_FAILED: "PIPELINE_ARCHIVE_FAILED",
 
     PLUGIN_CONFIG_OK: "PLUGIN_CONFIG_OK",
     PLUGIN_CONFIG_FAILED: "PLUGIN_CONFIG_FAILED",
+    PLUGIN_INSTANCE_COMMAND_OK: "PLUGIN_INSTANCE_COMMAND_OK",
+    PLUGIN_INSTANCE_COMMAND_FAILED: "PLUGIN_INSTANCE_COMMAND_FAILED",
     PLUGIN_PAUSE_OK: "PLUGIN_PAUSE_OK",
     PLUGIN_PAUSE_FAILED: "PLUGIN_PAUSE_FAILED",
     PLUGIN_RESUME_OK: "PLUGIN_RESUME_OK",
     PLUGIN_RESUME_FAILED: "PLUGIN_RESUME_FAILED",
     PLUGIN_DELAYED: "PLUGIN_DELAYED",
     PLUGIN_WORKING_HOURS_SHIFT_START: "PLUGIN_WORKING_HOURS_SHIFT_START",
     PLUGIN_WORKING_HOURS_SHIFT_START_FAILED: "PLUGIN_WORKING_HOURS_SHIFT_START_FAILED",
```

### Comparing `pye2-0.7.9/PyE2/default/mqtt_session.py` & `pye2-0.8.0/PyE2/default/mqtt_session.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,23 +44,22 @@
     """
     Check if the session is connected to the communication server.
     """
     return self._default_communicator.connected and self._heartbeats_communicator.connected and self._notifications_communicator.connected
 
   def _connect(self) -> None:
     if self._default_communicator.connection is None:
-      self._default_comm_con_res = self._default_communicator.server_connect()
-      self._default_comm_sub_res = self._default_communicator.subscribe()
+      self._default_communicator.server_connect()
+      self._default_communicator.subscribe()
     if self._heartbeats_communicator.connection is None:
-      self._hb_comm_con_res = self._heartbeats_communicator.server_connect()
-      self._hb_comm_sub_res = self._heartbeats_communicator.subscribe()
+      self._heartbeats_communicator.server_connect()
+      self._heartbeats_communicator.subscribe()
     if self._notifications_communicator.connection is None:
-      self._notif_comm_con_res = self._notifications_communicator.server_connect()
-      self._notif_comm_sub_res = self._notifications_communicator.subscribe()
-
+      self._notifications_communicator.server_connect()
+      self._notifications_communicator.subscribe()
     return
 
   def _communication_close(self, **kwargs):
     self._default_communicator.release()
     self._heartbeats_communicator.release()
     self._notifications_communicator.release()
     return
```

### Comparing `pye2-0.7.9/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.8.0/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.8.0/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.8.0/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/io_formatter/default/aixp1.py` & `pye2-0.8.0/PyE2/io_formatter/default/aixp1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/io_formatter/default/cavi2.py` & `pye2-0.8.0/PyE2/io_formatter/default/cavi2.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,16 @@
     }
     time = {
         'deviceTime': '',
         'hostTime': output.pop('EE_TIMESTAMP'),
         'internetTime': '',
     }
     sender = {
-        'id': "AiXp-ExecutionEngine",
-        'instanceId': "AiXp-EE-v" + ee_version,
+        'id': "DecentrAI-ExecutionEngine",
+        'instanceId': "DecentrAI-EE-v" + ee_version,
         "hostId": output.pop('EE_ID')
     }
 
     if ee_event_type == 'payload':
       self.log.start_timer(
           '_encode_payload', section='Formatter_' + str(self.signature))
       ee_event_type = output.pop('SIGNATURE').lower()
```

### Comparing `pye2-0.7.9/PyE2/logging/base_logger.py` & `pye2-0.8.0/PyE2/logging/base_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import threading
 import re
 
 from time import time as tm
 from time import strftime, localtime, strptime, mktime
 from collections import OrderedDict
 from datetime import datetime as dt
-from datetime import timedelta, timezone
+from datetime import timedelta, timezone, tzinfo
 from dateutil import tz
 from pathlib import Path
 
 from .tzlocal import get_localzone_name
 
 
 
@@ -437,21 +437,39 @@
     return
   
   def get_processor_platform(self):
     return self.processor_platform
     
   
   def lock_resource(self, str_res):
+    """
+    Possible critical failure:
+    
+    1. base plugin runs try stuff etc
+    2. plugin runs lock
+    3. threading.Lock() fails
+    4. base plugin runs except
+    5. except locks in log (no output) due to _lock_table_mutex.acquire(blocking=True)
+    6. any thread running lock_reource will hang with NO LOG OUTPUT
+    """
+    result = None
     self._lock_table_mutex.acquire(blocking=True)
-    if str_res not in self._lock_table:      
-      self._lock_table[str_res] = threading.Lock()
-    self._lock_table_mutex.release()
-
-    self._lock_table[str_res].acquire(blocking=True)
-    return self._lock_table[str_res]
+    try:
+      if str_res not in self._lock_table:      
+        self._lock_table[str_res] = threading.Lock()
+    except:
+      print("**************************************************************\nPANIC: Failed to create lock for resource '{}'\n**************************************************************".format(str_res))
+    finally:
+      self._lock_table_mutex.release()
+
+    if str_res in self._lock_table:      
+      self._lock_table[str_res].acquire(blocking=True)
+      result = self._lock_table[str_res]
+      
+    return result
   
   def unlock_resource(self, str_res):
     if str_res in self._lock_table:
       self._lock_table[str_res].release()
     return
   
   def lock_logger(self):
@@ -1427,45 +1445,44 @@
   def utc_to_local(remote_datetime, remote_utc, fmt='%Y-%m-%d %H:%M:%S', as_string=False):
     """
     Given a "remote" datetime (in datetime or str format) and a string or int denoting an offset 
     will return local datetime as a datetime object.
 
     Parameters
     ----------
-    remote_datetime: datetime or str
+    remote_datetime: datetime or str or tzinfo
       The remote datetime
       
     remote_utc: int or str
       The UTC offset of the remote datetime as int or as string - i.e. "UTC+3" or even "+3"
 
     Returns
     -------
       datetime      
     """
     if remote_utc is None:
       remote_utc = 'UTC+3'
     if isinstance(remote_utc, str):
-      utc_offset = int(remote_utc.replace('UTC', ''))
+      remote_utc = tz.gettz(remote_utc)
     elif isinstance(remote_utc, int):
       utc_offset = remote_utc
-    else:
-      raise ValueError("Uknown remote_utc type: {}".format(type(remote_utc)))
-      
+      remote_utc = tz.tzoffset(None, timedelta(hours=utc_offset))
+    elif not isinstance(remote_utc, tzinfo):
+      raise ValueError("Unknown remote_utc type: {}".format(type(remote_utc)))
+
     if isinstance(remote_datetime, str):
       remote_datetime = dt.strptime(remote_datetime, fmt)
-      
-    offset_timezone = timezone(timedelta(hours=utc_offset))
-    remote_datetime = remote_datetime.replace(tzinfo=offset_timezone)
+
+    remote_datetime = remote_datetime.replace(tzinfo=remote_utc)
     local_timezone = tz.tzlocal()
     local_datetime = remote_datetime.astimezone(local_timezone)
     local_datetime = local_datetime.replace(tzinfo=None)
     if as_string:
       local_datetime = local_datetime.strftime(fmt)
     return local_datetime
-    
   
   @staticmethod
   def str_to_sec(s):
     res = None
     try:
       import time
       x = time.strptime(s,'%H:%M:%S')
```

### Comparing `pye2-0.7.9/PyE2/logging/small_logger.py` & `pye2-0.8.0/PyE2/logging/small_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/__init__.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/class_instance_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/class_instance_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/computer_vision_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/computer_vision_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/datetime_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/datetime_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 from datetime import datetime as dt, timedelta
 from dateutil.relativedelta import relativedelta
+from ...const import WEEKDAYS_SHORT
 
 
-WEEKDAYS_SHORT = [
-  'MON',
-  'TUE',
-  'WED',
-  'THU',
-  'FRI',
-  'SAT',
-  'SUN'
-]
 class _DateTimeMixin(object):
   """
   Mixin for date and time functionalities that are attached to `pye2.Logger`.
 
   This mixin cannot be instantiated because it is built just to provide some additional
   functionalities for `pye2.Logger`
```

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/download_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/download_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
       _append_to_download_dir, _fn = os.path.split(_fn)
       _crt_download_dir = os.path.join(download_dir, _append_to_download_dir)
       save_path = os.path.join(_crt_download_dir, _fn)
 
       # Check if the file already exists, otherwise we need to download it now.
       has_file = os.path.exists(save_path)
       if not has_file or force_download:
+        file_path = None
         # handle http standard download
         # automatically add .zip in this corner case
         if unzip and not save_path.endswith('.zip'):
           save_path += '.zip'
 
         # Check if the download directory exists, otherwise create it.
         if not os.path.exists(_crt_download_dir):
@@ -239,29 +240,30 @@
           file_path = save_path
 
           if verbose:
             self.P("Copied file from given location to {}".format(save_path))
         else:
           self.P("ERROR: unknown url type: {}".format(_url), color='error')
 
-        if unzip:
-          _directory_to_extract_to = os.path.splitext(save_path)[0]
-          if verbose:
-            self.P("Unzipping '...{}' ...".format(file_path[-40:]))
-          if not os.path.exists(_directory_to_extract_to):
-            os.makedirs(_directory_to_extract_to)
-
-          with zipfile.ZipFile(file_path, 'r') as zip_ref:
-            zip_ref.extractall(_directory_to_extract_to)
-
-          # remove the downloaded zip file as it was already extracted, so it occupies space without any use
-          os.remove(file_path)
-          saved_files.append(_directory_to_extract_to)
-        else:
-          saved_files.append(file_path)
+        if file_path is not None:
+          if unzip:
+            _directory_to_extract_to = os.path.splitext(save_path)[0]
+            if verbose:
+              self.P("Unzipping '...{}' ...".format(file_path[-40:]))
+            if not os.path.exists(_directory_to_extract_to):
+              os.makedirs(_directory_to_extract_to)
+
+            with zipfile.ZipFile(file_path, 'r') as zip_ref:
+              zip_ref.extractall(_directory_to_extract_to)
+
+            # remove the downloaded zip file as it was already extracted, so it occupies space without any use
+            os.remove(file_path)
+            saved_files.append(_directory_to_extract_to)
+          else:
+            saved_files.append(file_path)
 
       else:
         if verbose:
           self.P("File {} found. Skipping.".format(_fn))
         saved_files.append(save_path)
         msgs.append("'{}' already downloaded.".format(save_path))
     # endfor
```

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/general_serialization_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/general_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/json_serialization_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/json_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/pickle_serialization_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/pickle_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/process_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/process_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/resource_size_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/resource_size_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/timers_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/timers_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/upload_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/upload_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/logger_mixins/utils_mixin.py` & `pye2-0.8.0/PyE2/logging/logger_mixins/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/tzlocal/unix.py` & `pye2-0.8.0/PyE2/logging/tzlocal/unix.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/tzlocal/utils.py` & `pye2-0.8.0/PyE2/logging/tzlocal/utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/tzlocal/win32.py` & `pye2-0.8.0/PyE2/logging/tzlocal/win32.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/logging/tzlocal/windows_tz.py` & `pye2-0.8.0/PyE2/logging/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/tutorials/1. hello_world.py` & `pye2-0.8.0/PyE2/tutorials/1. hello_world.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This is a simple example of how to use the PyE2 library.
 
 In this example, we connect to the network, listen for heartbeats from 
-  AiXpand nodes and print the CPU of each node.
+  DecentrAI nodes and print the CPU of each node.
 """
 
 from PyE2 import Session
 
 
 def on_hb(session: Session, e2id: str, data: dict):
   session.P("{} has a {}".format(e2id, data['CPU']))
```

### Comparing `pye2-0.7.9/PyE2/tutorials/2. first_deploy.py` & `pye2-0.8.0/PyE2/tutorials/2. first_deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from time import sleep
 
 
 def instance_on_data(pipeline: Pipeline, data: Payload):
   # the images can be extracted from the Payload object
   # PIL needs to be installed for this to work
-  images = data.get_image_as_PIL()
+  images = data.get_images_as_PIL()
   if images is not None:
     images[0].save('frame.jpg')
 
 
 if __name__ == '__main__':
   # create a session
   # the network credentials are read from the .env file automatically
@@ -41,21 +41,23 @@
       'URL': "https://www.dropbox.com/scl/fi/8z2wpeelhav3k2dv8bb5p/Cars_3.mp4?rlkey=imv415rr3j1tx3zstpurlxkqb&dl=1"
     }
   )
 
   # next, we deploy a plugin instance
   # we will use the view scene plugin, which essentially generates payloads with frames from the video
   # to consume the payloads generated by the plugin, we need to specify a callback function
-  instance: Instance = pipeline.start_plugin_instance(
+  instance: Instance = pipeline.create_plugin_instance(
     signature='VIEW_SCENE_01',
     instance_id='inst01',
     on_data=instance_on_data,
     # we can specify the configuration for the plugin instance as kwargs
     process_delay=3,
     # we can also specify if the payloads should be encrypted
     # if so, only the creator of this pipeline, in our case us, will be able to decrypt the payloads
     encrypt_payload=True,
   )
 
+  pipeline.deploy()
+
   # run the program for 30 seconds, then close the session
   session.run(wait=30, close_session=True, close_pipelines=True)
   session.P("Main thread exiting...")
```

### Comparing `pye2-0.7.9/PyE2/tutorials/3. simple_real_time_custom_code.py` & `pye2-0.8.0/PyE2/tutorials/3. simple_real_time_custom_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,29 +27,28 @@
 
   return
 
 
 def custom_instance_on_data(pipeline: Pipeline, custom_code_data: dict, data: Payload):
   # the images can be extracted from the Payload object
   # PIL needs to be installed for this to work
-  data.get_image_as_PIL().save('frame.jpg')
+  data.get_images_as_PIL()[0].save('frame.jpg')
   pipeline.P("Persons in frame: {}".format(custom_code_data['PERSONS_COUNT']))
 
 
 if __name__ == '__main__':
   # create a session
   # the network credentials are read from the .env file automatically
   session: Session = Session()
 
-  while session.get_active_nodes() == []:
-    session.P("Waiting for nodes to send heartbeats...")
-    sleep(1)
+  # wait for any node to be available
+  session.wait_for_any_node(timeout=10)
 
+  # get the first available node
   chosen_node = session.get_active_nodes()[0]
-  chosen_node = 'stefan-box'
 
   # we have our node, let's deploy a plugin
 
   # first, we create a pipeline
   # we will use the video file data source, since we want to extract frames from a video
   pipeline: Pipeline = session.create_pipeline(
     e2id=chosen_node,
@@ -57,24 +56,27 @@
     data_source='VideoFile',
     config={
       'URL': "https://www.dropbox.com/scl/fi/8z2wpeelhav3k2dv8bb5p/Cars_3.mp4?rlkey=imv415rr3j1tx3zstpurlxkqb&dl=1"
     }
   )
 
   # next, we deploy a custom code plugin instance
-  instance: Instance = pipeline.start_custom_plugin(
+  instance: Instance = pipeline.create_custom_plugin_instance(
     instance_id='inst01',
     custom_code=real_time_code,
     on_data=custom_instance_on_data,
     # we can specify the configuration for the plugin instance as kwargs
     process_delay=3,
     allow_empty_inputs=False,
     ai_engine="lowres_general_detector",
     object_type=["person"],
     # we can also specify if the payloads should be encrypted
     # if so, only the creator of this pipeline, in our case us, will be able to decrypt the payloads
     encrypt_payload=True,
   )
 
+  # we increase the timeout because the AI engine has to start and warm up, which can take a while
+  pipeline.deploy(timeout=60)
+
   # run the program for 120 seconds, then close the session
   session.run(wait=120, close_session=True, close_pipelines=True)
   session.P("Main thread exiting...")
```

### Comparing `pye2-0.7.9/PyE2/utils/code.py` & `pye2-0.8.0/PyE2/utils/code.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,18 @@
     str_encoded = b_encoded.decode('utf-8')
     l_b64 = len(str_encoded)
     self.__msg("Code checking and serialization suceeded. Initial/Compress/B64: {}/{}/{}".format(
         l_i, l_c, l_b64), color='g'
     )
     return str_encoded
 
+  def method_to_base64(self, func):
+    code = self.get_function_source_code(func)
+    return self.code_to_base64(code)
+
   def compress_bytes(self, data):
     if not isinstance(data, bytes):
       data = bytes(str(data), 'utf-8')
     zip_data = zlib.compress(data)
     return zip_data
 
   def decompress_bytes(self, zip_data):
```

### Comparing `pye2-0.7.9/PyE2/utils/code_exec.py` & `pye2-0.8.0/PyE2/utils/code_exec.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import zlib
 import sys
 import base64
 
 
 def code_to_base64(plain_code, verbose=False, compress=True, code_checker_callback=None):
   if verbose:
@@ -22,7 +23,20 @@
   str_encoded = b_encoded.decode('utf-8')
   l_b64 = len(str_encoded)
   if verbose:
     print("Code checking and serialization suceeded. Initial/Compress/B64: {}/{}/{}".format(
         l_i, l_c, l_b64), color='g'
     )
   return str_encoded
+
+
+def _get_function_source_code(func):
+  plain_code = inspect.getsourcelines(func)[0]
+  plain_code = plain_code[1:]
+  indent = len(plain_code[0]) - len(plain_code[0].lstrip())
+  plain_code = '\n'.join([line.rstrip()[indent:] for line in plain_code])
+  return plain_code
+
+
+def method_to_base64(func, verbose=False, compress=True, code_checker_callback=None):
+  code = _get_function_source_code(func)
+  return code_to_base64(code, verbose=verbose, compress=compress, code_checker_callback=code_checker_callback)
```

### Comparing `pye2-0.7.9/PyE2/utils/comm_utils.py` & `pye2-0.8.0/PyE2/utils/comm_utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/PyE2/utils/dotenv.py` & `pye2-0.8.0/PyE2/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/xperimental/attach_example.py` & `pye2-0.8.0/xperimental/attach_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   e2id=e2id,
   name='test_mqtt',
   on_notification=pipeline_on_notification,
   max_wait_time=60
 )
 
 # now start a cyclic process
-inst = pipeline.attach_to_custom_instance('inst01', on_data=instance_on_data)
+inst = pipeline.attach_to_custom_plugin_instance('inst01', on_data=instance_on_data)
 
 
 def generate_net_map():
   global boxes
   net_map_msgs = ["Printing network map"]
   for box, (instances, last_time) in boxes.items():
     if last_time - time() > 30:
```

### Comparing `pye2-0.7.9/xperimental/ex1.py` & `pye2-0.8.0/xperimental/ex1.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,40 +37,46 @@
           'URL': 0
       },
       on_data=pipeline_on_data
   )
 
   # now we start a perimeter intrusion functionality for low-res cameras with all
   # the other params default
-  perimeter_violation_instance: Instance = pipeline.start_plugin_instance(  # should return an id
+  perimeter_violation_instance: Instance = pipeline.create_plugin_instance(  # should return an id
       signature='PERIMETER_VIOLATION_01',
       instance_id='inst01',
       on_data=instance_on_data,
       ai_engine='lowres_general_detector'
   )
 
   plain_code = """
 result="Data on node"
   """
 
   # now start a cyclic process
-  custom_instance: Instance = pipeline.start_custom_plugin(
+  custom_instance: Instance = pipeline.create_custom_plugin_instance(
       instance_id='inst01',
       plain_code=plain_code,
       on_data=another_instance_on_data
   )
 
+  # now deploy the pipeline
+  pipeline.deploy()
+
   # we wait for 30 seconds
   sess.run(30, close_session=False)
 
   # we can stop an instance like this
-  pipeline.stop_plugin_instance(perimeter_violation_instance)
+  pipeline.remove_plugin_instance(perimeter_violation_instance)
 
   # or like this
   custom_instance.stop()
 
+  # we still need to deploy the changes
+  pipeline.deploy()
+
   # we wait until the user presses `Ctrl+C`
   sess.run(0, close_session=False)
 
   # now close conn to comm server
   pipeline.close()
   sess.close()
```

### Comparing `pye2-0.7.9/xperimental/remote_exec.py` & `pye2-0.8.0/xperimental/remote_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,24 @@
         "RECONNECTABLE": True,
     },
     plugins=None,
     on_notification=pipeline_on_notification
 )
 
 # now start a ciclic process
-pipeline.start_custom_plugin(
+pipeline.create_custom_plugin_instance(
     instance_id='inst01',
     # plain_code_path="./custom_exec_scripts/custom_exec_tutorial.txt", # you can provide it as a file
     plain_code=custom_worker_code,
     on_data=instance_on_data,
     process_delay=2
 )
 
+pipeline.deploy()
+
 
 def generate_net_map():
   global boxes
   net_map_msgs = ["Printing network map"]
   for box, (instances, last_time) in boxes.items():
     if last_time - time() > 30:
       continue
```

### Comparing `pye2-0.7.9/xperimental/save_images.py` & `pye2-0.8.0/xperimental/save_images.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,18 +23,20 @@
     data_source="VideoFile",
     config={
       "URL": "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4",
       "LIVE": False,
     },
   )
 
-  instance = pipeline.start_plugin_instance(
+  instance = pipeline.create_plugin_instance(
     signature="OBJECT_TRACKING_01",
     instance_id="Demo1",
-    params={
+    config={
       "OBJECT_TYPE": ["person"]
     },
     on_data=instance_on_data,
   )
 
+  pipeline.deploy()
+
   sess.run(wait=120, close_pipelines=True)
   sess.P("Main thread exiting...")
```

### Comparing `pye2-0.7.9/xperimental/decentralized/chain_dist_example.py` & `pye2-0.8.0/xperimental/decentralized/chain_dist_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,23 +34,25 @@
       data_source='IotQueueListener',  # this DCT allows data acquisition from MQTT brokers
       config={
           'STREAM_CONFIG_METADATA': listener_params,
           "RECONNECTABLE": True,
       },
   )
 
-  pipeline.start_custom_plugin(
+  pipeline.create_custom_plugin_instance(
       instance_id='inst02',
       plain_code_path=INITIATOR_CODE_PATH,
-      params={
+      config={
           'MAX_TRIES': 10,  # this will be used within plugin as `plugin.cfg_max_tries`
           'MAX_RUN_TIME': 60,  # this will be used within plugin as `plugin.cfg_max_run_time`
           'N_WORKERS': 3,  # this will be used within plugin as `plugin.cfg_n_workers`
 
           # this will be used within plugin as `plugin.cfg_worker_code`
           'WORKER_CODE': code_to_base64(worker_code)
       },
       on_data=instance_on_data,
       process_delay=0.2
   )
 
+  pipeline.deploy()
+
   sess.run(wait=True, close_session=True, close_pipelines=True)
```

### Comparing `pye2-0.7.9/xperimental/decentralized/chain_dist_example_initiator.py` & `pye2-0.8.0/xperimental/decentralized/chain_dist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/.gitignore` & `pye2-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/LICENSE` & `pye2-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.7.9/README.md` & `pye2-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PyE2 SDK
 
-This is the Python SDK package that allows interactions, development and deployment of jobs in AiXpand network. The SDK enables low-code development and deployment of end-to-end AI (and not only) cooperative application pipelines within the AiXpand Execution Engine processing nodes ecosystem. For further information please see "AiXpand - Decentralized ubiquitous computing MLOps execution engine".
+This is the Python SDK package that allows interactions, development and deployment of jobs in DecentrAI network. The SDK enables low-code development and deployment of end-to-end AI (and not only) cooperative application pipelines within the DecentrAI Execution Engine processing nodes ecosystem. For further information please see "DecentrAI - Decentralized ubiquitous computing MLOps execution engine".
 
 ## Dependencies
 
 This packet depends on the following packets: [`pika`, `paho-mqtt`, `numpy`, `cryptography`].
 
 ## Installation
```

### Comparing `pye2-0.7.9/pyproject.toml` & `pye2-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.7.9"
+version = "0.8.0"
 authors = [
-  { name="Stefan Saraev", email="stefan.saraev@hyperfy.tech" },
-  { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
-  { name="Cristan Bleotiu", email="cristan.bleotiu@hyperfy.tech" },
+  { name="Stefan Saraev", email="saraevstefan@gmail.com" },
+  { name="Andrei Ionut Damian", email="andrei.damian@me.com" },
+  { name="Cristan Bleotiu", email="cristibleotiu@gmail.com" },
 ]
-description = "PyE2 is the Python SDK required for client app development in the AiXpand network"
+description = "PyE2 is the Python SDK required for client app development in the DecentrAI network"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -25,9 +25,9 @@
   "pyopenssl>=23.0.0",
   "cryptography>=39.0.0",
   "python-dateutil",
   "pyaml"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/AiXpand/PyE2"
-"Bug Tracker" = "https://github.com/AiXpand/PyE2/issues"
+"Homepage" = "https://github.com/DecentrAI/PyE2"
+"Bug Tracker" = "https://github.com/DecentrAI/PyE2/issues"
```

### Comparing `pye2-0.7.9/PKG-INFO` & `pye2-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: PyE2
-Version: 0.7.9
-Summary: PyE2 is the Python SDK required for client app development in the AiXpand network
-Project-URL: Homepage, https://github.com/AiXpand/PyE2
-Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
-Author-email: Stefan Saraev <stefan.saraev@hyperfy.tech>, Andrei Ionut Damian <andrei.damian@lummetry.ai>, Cristan Bleotiu <cristan.bleotiu@hyperfy.tech>
+Version: 0.8.0
+Summary: PyE2 is the Python SDK required for client app development in the DecentrAI network
+Project-URL: Homepage, https://github.com/DecentrAI/PyE2
+Project-URL: Bug Tracker, https://github.com/DecentrAI/PyE2/issues
+Author-email: Stefan Saraev <saraevstefan@gmail.com>, Andrei Ionut Damian <andrei.damian@me.com>, Cristan Bleotiu <cristibleotiu@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: cryptography>=39.0.0
 Requires-Dist: numpy
@@ -17,15 +17,15 @@
 Requires-Dist: pyaml
 Requires-Dist: pyopenssl>=23.0.0
 Requires-Dist: python-dateutil
 Description-Content-Type: text/markdown
 
 # PyE2 SDK
 
-This is the Python SDK package that allows interactions, development and deployment of jobs in AiXpand network. The SDK enables low-code development and deployment of end-to-end AI (and not only) cooperative application pipelines within the AiXpand Execution Engine processing nodes ecosystem. For further information please see "AiXpand - Decentralized ubiquitous computing MLOps execution engine".
+This is the Python SDK package that allows interactions, development and deployment of jobs in DecentrAI network. The SDK enables low-code development and deployment of end-to-end AI (and not only) cooperative application pipelines within the DecentrAI Execution Engine processing nodes ecosystem. For further information please see "DecentrAI - Decentralized ubiquitous computing MLOps execution engine".
 
 ## Dependencies
 
 This packet depends on the following packets: [`pika`, `paho-mqtt`, `numpy`, `cryptography`].
 
 ## Installation
```

