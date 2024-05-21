# Comparing `tmp/pye2-0.8.0.tar.gz` & `tmp/pye2-0.8.1.tar.gz`

## Comparing `pye2-0.8.0.tar` & `pye2-0.8.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.8.0/.gitattributes
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.8.0/TODOs.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.8.0/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.8.0/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.8.0/winrun.bat
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/_ver.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base_decentra_object.py
--rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/plugins_manager_mixin.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/__init__.py
--rw-r--r--   0        0        0    49968 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/generic_session.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/instance.py
--rw-r--r--   0        0        0    49602 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/pipeline.py
--rw-r--r--   0        0        0    62467 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/plugin_template.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/responses.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/transaction.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/bc/__init__.py
--rw-r--r--   0        0        0    27458 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/bc/base.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/bc/ec.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/code_cheker/__init__.py
--rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/code_cheker/base.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    13817 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/README.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/base.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/comms.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/environment.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/formatter.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/misc.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/default/__init__.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/aixp1.py
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/io_formatter/default/default.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/__init__.py
--rw-r--r--   0        0        0    59434 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/base_logger.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/small_logger.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/class_instance_mixin.py
--rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/computer_vision_mixin.py
--rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/datetime_mixin.py
--rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/download_mixin.py
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/general_serialization_mixin.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/json_serialization_mixin.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/process_mixin.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/resource_size_mixin.py
--rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/timers_mixin.py
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/upload_mixin.py
--rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/logger_mixins/utils_mixin.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/__init__.py
--rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/unix.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/utils.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/win32.py
--rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/logging/tzlocal/windows_tz.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/.example_env
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/1. hello_world.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/2. first_deploy.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/3. simple_real_time_custom_code.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/4. real_time_custom_code_2.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/5. real_time_custom_code_multithreading.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/7. real_time_custom_code_multithreading.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/tutorials/8. chatbot.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/code.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/comm_utils.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.8.0/PyE2/utils/dotenv.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/.example_env
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/attach_example.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/ex1.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/hello.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/remote_exec.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/decentralized/chain_dist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/decentralized/chain_dist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.8.0/xperimental/decentralized/chain_dist_example_worker.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.8.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.8.0/LICENSE
--rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 pye2-0.8.0/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pye2-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 pye2-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.8.1/.gitattributes
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.8.1/TODOs.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.8.1/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.8.1/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.8.1/winrun.bat
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/_ver.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base_decentra_object.py
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/plugins_manager_mixin.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    50160 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/instance.py
+-rw-r--r--   0        0        0    49635 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0    62467 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/plugin_template.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/responses.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/transaction.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/bc/__init__.py
+-rw-r--r--   0        0        0    27458 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/bc/base.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/bc/ec.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/code_cheker/__init__.py
+-rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/code_cheker/base.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/README.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/base.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/comms.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/environment.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/formatter.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/misc.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/default/aixp1.py
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/io_formatter/default/default.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/__init__.py
+-rw-r--r--   0        0        0    59434 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/base_logger.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/small_logger.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/class_instance_mixin.py
+-rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/computer_vision_mixin.py
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/datetime_mixin.py
+-rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/download_mixin.py
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/general_serialization_mixin.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/json_serialization_mixin.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/process_mixin.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/resource_size_mixin.py
+-rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/timers_mixin.py
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/upload_mixin.py
+-rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/logger_mixins/utils_mixin.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/tzlocal/__init__.py
+-rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/tzlocal/unix.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/tzlocal/utils.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/tzlocal/win32.py
+-rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/logging/tzlocal/windows_tz.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/.example_env
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/1. hello_world.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/2. first_deploy.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/3. simple_real_time_custom_code.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/4. real_time_custom_code_2.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/5. real_time_custom_code_multithreading.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/7. real_time_custom_code_multithreading.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/tutorials/8. chatbot.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/utils/comm_utils.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.8.1/PyE2/utils/dotenv.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/.example_env
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/attach_example.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/ex1.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/hello.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/decentralized/chain_dist_example.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/decentralized/chain_dist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.8.1/xperimental/decentralized/chain_dist_example_worker.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.8.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.8.1/LICENSE
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pye2-0.8.1/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pye2-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 pye2-0.8.1/PKG-INFO
```

### Comparing `pye2-0.8.0/.github/workflows/python-publish.yml` & `pye2-0.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/base_decentra_object.py` & `pye2-0.8.1/PyE2/base_decentra_object.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/plugins_manager_mixin.py` & `pye2-0.8.1/PyE2/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/base/generic_session.py` & `pye2-0.8.1/PyE2/base/generic_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,20 +256,20 @@
       # parse the message
       dict_msg_parsed = self.__parse_message(dict_msg)
       if dict_msg_parsed is None:
         return
 
       try:
         msg_path = dict_msg.get(PAYLOAD_DATA.EE_PAYLOAD_PATH, [None] * 4)
-        msg_eeid, msg_pipeline, msg_signature, msg_instance = msg_path
+        msg_node_id, msg_pipeline, msg_signature, msg_instance = msg_path
       except:
         self.D("Message does not respect standard: {}".format(dict_msg), verbosity=2)
         return
 
-      message_callback(dict_msg_parsed, msg_eeid, msg_pipeline, msg_signature, msg_instance)
+      message_callback(dict_msg_parsed, msg_node_id, msg_pipeline, msg_signature, msg_instance)
       return
 
     def __handle_messages(self, message_queue, message_callback):
       """
       Handle messages from the communication server.
       This method is called in a separate thread.
 
@@ -290,53 +290,53 @@
 
       # process the remaining messages before exiting
       while len(message_queue) > 0:
         current_msg = message_queue.popleft()
         self.__on_message_default_callback(current_msg, message_callback)
       return
 
-    def __maybe_ignore_message(self, e2id):
+    def __maybe_ignore_message(self, node_id):
       """
       Check if the message should be ignored.
       A message should be ignored if the `filter_workers` attribute is set and the message comes from a node that is not in the list.
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           The name of the DecentrAI node that sent the message.
 
       Returns
       -------
       bool
           True if the message should be ignored, False otherwise.
       """
-      return self.filter_workers is not None and e2id not in self.filter_workers
+      return self.filter_workers is not None and node_id not in self.filter_workers
 
-    def __track_online_node(self, e2id, ee_address):
+    def __track_online_node(self, node_id, ee_address):
       """
       Track the last time a node was seen online.
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           The name of the DecentrAI node that sent the message.
       """
-      self._last_seen_boxes[e2id] = tm()
-      self._box_addr[e2id] = ee_address
+      self._last_seen_boxes[node_id] = tm()
+      self._box_addr[node_id] = ee_address
       return
 
-    def __on_heartbeat(self, dict_msg: dict, msg_eeid, msg_pipeline, msg_signature, msg_instance):
+    def __on_heartbeat(self, dict_msg: dict, msg_node_id, msg_pipeline, msg_signature, msg_instance):
       """
       Handle a heartbeat message received from the communication server.
 
       Parameters
       ----------
       dict_msg : dict
           The message received from the communication server
-      msg_eeid : str
+      msg_node_id : str
           The name of the DecentrAI node that sent the message.
       msg_pipeline : str
           The name of the pipeline that sent the message.
       msg_signature : str
           The signature of the plugin that sent the message.
       msg_instance : str
           The name of the instance that sent the message.
@@ -349,141 +349,141 @@
         dict_msg = {**dict_msg, **data}
 
       msg_active_configs = dict_msg.get(HB.CONFIG_STREAMS)
       if msg_active_configs is None:
         return
 
       # default action
-      if msg_eeid not in self._online_boxes:
-        self._online_boxes[msg_eeid] = {}
+      if msg_node_id not in self._online_boxes:
+        self._online_boxes[msg_node_id] = {}
       for config in msg_active_configs:
         pipeline_name = config[PAYLOAD_DATA.NAME]
-        pipeline: Pipeline = self._online_boxes[msg_eeid].get(pipeline_name, None)
+        pipeline: Pipeline = self._online_boxes[msg_node_id].get(pipeline_name, None)
         if pipeline is not None:
           pipeline.update_full_configuration(config)
         else:
-          self._online_boxes[msg_eeid][pipeline_name] = self.__create_pipeline_from_config(msg_eeid, config)
+          self._online_boxes[msg_node_id][pipeline_name] = self.__create_pipeline_from_config(msg_node_id, config)
 
       ee_address = dict_msg[HB.EE_ADDR]
-      self.__track_online_node(msg_eeid, ee_address)
+      self.__track_online_node(msg_node_id, ee_address)
 
       # TODO: move this call in `__on_message_default_callback`
-      if self.__maybe_ignore_message(msg_eeid):
+      if self.__maybe_ignore_message(msg_node_id):
         return
 
       # pass the heartbeat message to open transactions
       no_transactions = len(self.__open_transactions)
       for idx in range(no_transactions):
         self.__open_transactions[idx].handle_heartbeat(dict_msg)
 
-      self.D("Received hb from: {}".format(msg_eeid), verbosity=2)
+      self.D("Received hb from: {}".format(msg_node_id), verbosity=2)
 
       # call the custom callback, if defined
       if self.custom_on_heartbeat is not None:
-        self.custom_on_heartbeat(self, msg_eeid, dict_msg)
+        self.custom_on_heartbeat(self, msg_node_id, dict_msg)
 
       return
 
-    def __on_notification(self, dict_msg: dict, msg_eeid, msg_pipeline, msg_signature, msg_instance):
+    def __on_notification(self, dict_msg: dict, msg_node_id, msg_pipeline, msg_signature, msg_instance):
       """
       Handle a notification message received from the communication server.
 
       Parameters
       ----------
       dict_msg : dict
           The message received from the communication server
-      msg_eeid : str
+      msg_node_id : str
           The name of the DecentrAI node that sent the message.
       msg_pipeline : str
           The name of the pipeline that sent the message.
       msg_signature : str
           The signature of the plugin that sent the message.
       msg_instance : str
           The name of the instance that sent the message.
       """
       # extract relevant data from the message
       notification_type = dict_msg.get(STATUS_TYPE.NOTIFICATION_TYPE)
       notification = dict_msg.get(PAYLOAD_DATA.NOTIFICATION)
 
-      if self.__maybe_ignore_message(msg_eeid):
+      if self.__maybe_ignore_message(msg_node_id):
         return
 
       color = None
       if notification_type != STATUS_TYPE.STATUS_NORMAL:
         color = 'r'
       self.D("Received notification {} from <{}/{}>: {}"
              .format(
                 notification_type,
-                msg_eeid,
+                msg_node_id,
                 msg_pipeline,
                 notification),
              color=color,
              verbosity=2,
              )
 
       # call the pipeline and instance defined callbacks
       for pipeline in self.own_pipelines:
-        if msg_eeid == pipeline.e2id and msg_pipeline == pipeline.name:
+        if msg_node_id == pipeline.node_id and msg_pipeline == pipeline.name:
           pipeline._on_notification(msg_signature, msg_instance, Payload(dict_msg))
           # since we found the pipeline, we can stop searching
           # because the pipelines have unique names
           break
 
       # pass the notification message to open transactions
       no_transactions = len(self.__open_transactions)
       for idx in range(no_transactions):
         self.__open_transactions[idx].handle_notification(dict_msg)
 
       # call the custom callback, if defined
       if self.custom_on_notification is not None:
-        self.custom_on_notification(self, msg_eeid, Payload(dict_msg))
+        self.custom_on_notification(self, msg_node_id, Payload(dict_msg))
 
       return
 
     # TODO: maybe convert dict_msg to Payload object
     #       also maybe strip the dict from useless info for the user of the sdk
     #       Add try-except + sleep
-    def __on_payload(self, dict_msg: dict, msg_eeid, msg_pipeline, msg_signature, msg_instance) -> None:
+    def __on_payload(self, dict_msg: dict, msg_node_id, msg_pipeline, msg_signature, msg_instance) -> None:
       """
       Handle a payload message received from the communication server.
 
       Parameters
       ----------
       dict_msg : dict
           The message received from the communication server
-      msg_eeid : str
+      msg_node_id : str
           The name of the DecentrAI node that sent the message.
       msg_pipeline : str
           The name of the pipeline that sent the message.
       msg_signature : str
           The signature of the plugin that sent the message.
       msg_instance : str
           The name of the instance that sent the message.
       """
       # extract relevant data from the message
       msg_data = dict_msg
 
-      if self.__maybe_ignore_message(msg_eeid):
+      if self.__maybe_ignore_message(msg_node_id):
         return
 
       # call the pipeline and instance defined callbacks
       for pipeline in self.own_pipelines:
-        if msg_eeid == pipeline.e2id and msg_pipeline == pipeline.name:
+        if msg_node_id == pipeline.node_id and msg_pipeline == pipeline.name:
           pipeline._on_data(msg_signature, msg_instance, Payload(dict_msg))
           # since we found the pipeline, we can stop searching
           # because the pipelines have unique names
           break
 
       # pass the payload message to open transactions
       no_transactions = len(self.__open_transactions)
       for idx in range(no_transactions):
         self.__open_transactions[idx].handle_payload(dict_msg)
 
       if self.custom_on_payload is not None:
-        self.custom_on_payload(self, msg_eeid, msg_pipeline, msg_signature, msg_instance, Payload(msg_data))
+        self.custom_on_payload(self, msg_node_id, msg_pipeline, msg_signature, msg_instance, Payload(msg_data))
 
       return
 
   # Main loop
   if True:
     def __start_blockchain(self, bc_engine, blockchain_config):
       if bc_engine is not None:
@@ -916,15 +916,15 @@
       name = pipeline_config.pop('name', None)
       plugins = pipeline_config.pop('plugins', None)
 
       pipeline = Pipeline(
         is_attached=True,
         session=self,
         log=self.log,
-        e2id=node,
+        node_id=node,
         name=name,
         plugins=plugins,
         existing_config=pipeline_config,
       )
 
       return pipeline
 
@@ -934,15 +934,15 @@
     def server(self):
       """
       The hostname of the server.
       """
       return self._config[comm_ct.HOST]
 
     def create_pipeline(self, *,
-                        e2id,
+                        node_id,
                         name,
                         data_source,
                         config={},
                         plugins=[],
                         on_data=None,
                         on_notification=None,
                         max_wait_time=0,
@@ -966,15 +966,15 @@
 
       This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an DecentrAI node is online or not.
       If the node does not appear online, a warning will be displayed at the stdout, telling the user that the message that handles the
       creation of the pipeline will be sent, but it is not guaranteed that the specific node will receive it.
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           Name of the DecentrAI node that will handle this pipeline.
       name : str
           Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
       data_source : str
           This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
       config : dict, optional
           This is the dictionary that contains the configuration of the acquisition source, by default {}
@@ -1003,29 +1003,29 @@
       Returns
       -------
       Pipeline
           A `Pipeline` object.
 
       """
       _start = tm()
-      found = e2id in self.get_active_nodes()
+      found = node_id in self.get_active_nodes()
       while (tm() - _start) < max_wait_time and not found:
         sleep(0.1)
         avail_workers = self.get_active_nodes()
-        found = e2id in avail_workers
+        found = node_id in avail_workers
       # end while
 
       if not found:
         self.P("WARNING: could not find worker '{}' in {:.1f}s. The job may not have a valid active worker.".format(
-            e2id, tm() - _start
+            node_id, tm() - _start
         ), color='r', verbosity=1)
       pipeline = Pipeline(
           self,
           self.log,
-          e2id=e2id,
+          node_id=node_id,
           name=name,
           type=data_source,
           config=config,
           plugins=plugins,
           on_data=on_data,
           on_notification=on_notification,
           is_attached=False,
@@ -1042,33 +1042,33 @@
       -------
       list
           List of names of all the DecentrAI nodes that are considered online
 
       """
       return [k for k, v in self._last_seen_boxes.items() if tm() - v < self.online_timeout]
 
-    def get_active_pipelines(self, e2id):
+    def get_active_pipelines(self, node_id):
       """
       Get a dictionary with all the pipelines that are active on this DecentrAI node
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           name of the DecentrAI node
 
       Returns
       -------
       dict
           The key is the name of the pipeline, and the value is the entire config dictionary of that pipeline.
 
       """
-      return self._online_boxes.get(e2id, None) if e2id in self.get_active_nodes() else None
+      return self._online_boxes.get(node_id, None) if node_id in self.get_active_nodes() else None
 
     def attach_to_pipeline(self, *,
-                           e2id,
+                           node_id,
                            name,
                            on_data=None,
                            on_notification=None,
                            max_wait_time=0) -> Pipeline:
       """
       Create a Pipeline object and attach to an existing pipeline on an DecentrAI node.
       Useful when one wants to treat an existing pipeline as one of his own,
@@ -1091,15 +1091,15 @@
       This call can busy-wait for a number of seconds to listen to heartbeats, in order to check if an DecentrAI node is online or not.
       If the node does not appear online, a warning will be displayed at the stdout, telling the user that the message that handles the
       creation of the pipeline will be sent, but it is not guaranteed that the specific node will receive it.
 
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           Name of the DecentrAI node that handles this pipeline.
       name : str
           Name of the existing pipeline.
       on_data : Callable[[Pipeline, str, str, dict], None], optional
           Callback that handles messages received from any plugin instance.
           As arguments, it has a reference to this Pipeline object, the signature and the instance of the plugin
           that sent the message and the payload itself.
@@ -1126,49 +1126,49 @@
       Exception
           Node does not exist (it is considered offline because the session did not receive any heartbeat)
       Exception
           Node does not host the desired pipeline
       """
 
       _start = tm()
-      found = e2id in self.get_active_nodes()
+      found = node_id in self.get_active_nodes()
       while (tm() - _start) < max_wait_time and not found:
         sleep(0.1)
         avail_workers = self.get_active_nodes()
-        found = e2id in avail_workers
+        found = node_id in avail_workers
       # end while
 
       if not found:
         raise Exception("Unable to attach to pipeline. Node does not exist")
 
-      if name not in self._online_boxes[e2id]:
+      if name not in self._online_boxes[node_id]:
         raise Exception("Unable to attach to pipeline. Pipeline does not exist")
 
-      pipeline = self._online_boxes[e2id][name]
+      pipeline = self._online_boxes[node_id][name]
 
       self.own_pipelines.append(pipeline)
 
       return pipeline
 
     def create_or_attach_to_pipeline(self, *,
-                                     e2id,
+                                     node_id,
                                      name,
                                      data_source,
                                      config={},
                                      plugins=[],
                                      on_data=None,
                                      on_notification=None,
                                      max_wait_time=0,
                                      **kwargs) -> Pipeline:
       """
       Create a new pipeline on a node, or attach to an existing pipeline on an DecentrAI node.
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           Name of the DecentrAI node that will handle this pipeline.
       name : str
           Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
       data_source : str
           This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
       config : dict, optional
           This is the dictionary that contains the configuration of the acquisition source, by default {}
@@ -1199,15 +1199,15 @@
       Pipeline
           A `Pipeline` object.
       """
 
       pipeline = None
       try:
         pipeline = self.attach_to_pipeline(
-          e2id=e2id,
+          node_id=node_id,
           name=name,
           on_data=on_data,
           on_notification=on_notification,
           max_wait_time=max_wait_time,
           **kwargs
         )
 
@@ -1220,15 +1220,15 @@
           possible_new_configuration['PLUGINS'] = plugins
 
         if len(possible_new_configuration) > 0:
           pipeline.update_full_configuration(config=possible_new_configuration)
       except Exception as e:
         self.D("Failed to attach to pipeline: {}".format(e))
         pipeline = self.create_pipeline(
-          e2id=e2id,
+          node_id=node_id,
           name=name,
           data_source=data_source,
           config=config,
           plugins=plugins,
           on_data=on_data,
           on_notification=on_notification,
           **kwargs
@@ -1273,38 +1273,38 @@
 
       if found:
         self.P("Found nodes {} online.".format(self.get_active_nodes()))
       else:
         self.P("No nodes found online in {:.1f}s.".format(tm() - _start), color='r')
       return found
 
-    def wait_for_node(self, e2id, timeout=15):
+    def wait_for_node(self, node_id, timeout=15):
       """
       Wait for a node to appear online.
 
       Parameters
       ----------
-      e2id : str
+      node_id : str
           The name of the DecentrAI node.
       timeout : int, optional
           The timeout, by default 15
 
       Returns
       -------
       bool
           True if the node is online, False otherwise.
       """
 
-      self.P("Waiting for node '{}' to appear online...".format(e2id))
+      self.P("Waiting for node '{}' to appear online...".format(node_id))
       _start = tm()
-      found = e2id in self.get_active_nodes()
+      found = node_id in self.get_active_nodes()
       while (tm() - _start) < timeout and not found:
         sleep(0.1)
         avail_workers = self.get_active_nodes()
-        found = e2id in avail_workers
+        found = node_id in avail_workers
       # end while
 
       if found:
-        self.P("Node '{}' is online.".format(e2id))
+        self.P("Node '{}' is online.".format(node_id))
       else:
-        self.P("Node '{}' did not appear online in {:.1f}s.".format(e2id, tm() - _start), color='r')
+        self.P("Node '{}' did not appear online in {:.1f}s.".format(node_id, tm() - _start), color='r')
       return found
```

### Comparing `pye2-0.8.0/PyE2/base/instance.py` & `pye2-0.8.1/PyE2/base/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,20 +128,20 @@
       """
       self.on_notification_callbacks = []
       return
 
   # Utils
   if True:
     def __repr__(self) -> str:
-      e2id = self.pipeline.e2id
+      node_id = self.pipeline.node_id
       pipeline_name = self.pipeline.name
       signature = self.signature
       instance_id = self.instance_id
 
-      return f"<Instance: {e2id}/{pipeline_name}/{signature}/{instance_id}>"
+      return f"<Instance: {node_id}/{pipeline_name}/{signature}/{instance_id}>"
 
     def _is_tainted(self):
       """
       Check if the instance has a proposed configuration.
 
       Returns
       -------
@@ -256,17 +256,17 @@
 
       Returns
       -------
       list[Transaction]
           The list of transactions generated
       """
       required_responses = [
-        PipelineOKResponse(self.pipeline.e2id, self.pipeline.name),
-        PluginInstanceCommandOKResponse(self.pipeline.e2id, self.pipeline.name, self.signature, self.instance_id),
-        # PluginConfigOKResponse(self.pipeline.e2id, self.pipeline.name, self.signature, self.instance_id),
+        PipelineOKResponse(self.pipeline.node_id, self.pipeline.name),
+        PluginInstanceCommandOKResponse(self.pipeline.node_id, self.pipeline.name, self.signature, self.instance_id),
+        # PluginConfigOKResponse(self.pipeline.node_id, self.pipeline.name, self.signature, self.instance_id),
       ]
 
       transactions = [self.pipeline.session._register_transaction(
           session_id=session_id,
           lst_required_responses=required_responses,
           timeout=timeout,
           on_success_callback=self._handle_instance_command_success,
@@ -281,31 +281,31 @@
 
       Returns
       -------
       list[str]
           The list of responses required to update the instance
       """
       responses = [
-        PipelineOKResponse(self.pipeline.e2id, self.pipeline.name),
-        PluginConfigOKResponse(self.pipeline.e2id, self.pipeline.name, self.signature, self.instance_id),
+        PipelineOKResponse(self.pipeline.node_id, self.pipeline.name),
+        PluginConfigOKResponse(self.pipeline.node_id, self.pipeline.name, self.signature, self.instance_id),
       ]
 
       return responses
 
     def _get_instance_remove_required_responses(self):
       """
       Get the responses required to delete the instance.
 
       Returns
       -------
       list[str]
           The list of responses required to delete the instance
       """
       responses = [
-        PipelineOKResponse(self.pipeline.e2id, self.pipeline.name),
+        PipelineOKResponse(self.pipeline.node_id, self.pipeline.name),
       ]
 
       return responses
 
   # API
   if True:
     @property
@@ -406,15 +406,15 @@
       self.P(f'Sending command <{command}> to instance <{self.__repr__()}>', color="b")
 
       self.__was_last_operation_successful = None
 
       transactions = self.__register_transaction_for_instance_command(timeout=timeout)
 
       self.pipeline.session._send_command_instance_command(
-        worker=self.pipeline.e2id,
+        worker=self.pipeline.node_id,
         pipeline_name=self.pipeline.name,
         signature=self.signature,
         instance_id=self.instance_id,
         command=command,
         payload=payload,
         command_params=command_params,
       )
```

### Comparing `pye2-0.8.0/PyE2/base/pipeline.py` & `pye2-0.8.1/PyE2/base/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
   In the documentation, the following reffer to the same thing:
     `Pipeline` == `Stream`
 
     `Plugin` == `Signature`
   """
 
-  def __init__(self, session, log, *, e2id, name, config={}, plugins=[], on_data=None, on_notification=None, is_attached=False, existing_config=None, **kwargs) -> None:
+  def __init__(self, session, log, *, node_id, name, config={}, plugins=[], on_data=None, on_notification=None, is_attached=False, existing_config=None, **kwargs) -> None:
     """
     A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
     A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
     processing units, usually named `Plugins`. 
 
     An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
@@ -47,15 +47,15 @@
     session : Session
         The Session object which owns this pipeline. A pipeline must be attached to a Session because that is the only
         way the `on_X` callbacks are called
     log : Logger
         A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
         In the future, the documentation for the Logger base class will be available and developers will be able to use
         custom-made Loggers. 
-    e2id : str
+    node_id : str
         Name of the DecentrAI node that will handle this pipeline.  
     name : str
         The name of this pipeline.
     data_source : str
         This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
     config : dict, optional
         This is the dictionary that contains the configuration of the acquisition source, by default {}
@@ -78,15 +78,15 @@
         This is used internally to allow the user to create or attach to a pipeline, and then use the same
         objects in the same way, by default True
     **kwargs : dict
         The user can provide the configuration of the acquisition source directly as kwargs.
     """
     self.log = log
     self.session = session
-    self.e2id = e2id
+    self.node_id = node_id
     self.name = name
 
     self.config = {}
     plugins = config.pop('PLUGINS', plugins)
 
     if is_attached:
       assert existing_config is not None, "When attaching to a pipeline, the existing configuration should be found in the heartbeat of the DecentrAI node."
@@ -220,15 +220,15 @@
           on_success_callback=lambda: self.__apply_staged_remove_instance(instance),
           on_failure_callback=lambda fail_reason: self.__discard_staged_remove_instance(instance, fail_reason),
         ))
       # end for register to remove instances
 
       if self.proposed_config is not None:
         required_responses = [
-          PipelineOKResponse(self.e2id, self.name),
+          PipelineOKResponse(self.node_id, self.name),
         ]
         transactions.append(self.session._register_transaction(
           session_id=session_id,
           lst_required_responses=required_responses,
           timeout=timeout,
           on_success_callback=self.__apply_staged_config,
           on_failure_callback=self.__discard_staged_config,
@@ -253,15 +253,15 @@
       -------
       transactions : list[Transaction]
           The list of transactions generated.
       """
       transactions = []
 
       required_responses = [
-        PipelineArchiveResponse(self.e2id, self.name),
+        PipelineArchiveResponse(self.node_id, self.name),
       ]
       transactions.append(self.session._register_transaction(
         session_id=session_id,
         lst_required_responses=required_responses,
         timeout=timeout,
         on_success_callback=None,
         on_failure_callback=None,
@@ -342,15 +342,15 @@
       return dct_signature_instances
 
     def __send_update_config_to_box(self, session_id=None):
       """
       Send an update pipeline configuration command to the DecentrAI node.
       """
       self.session._send_command_update_pipeline_config(
-          worker=self.e2id,
+          worker=self.node_id,
           pipeline_config=self.__get_proposed_pipeline_config(),
           session_id=session_id
       )
       return
 
     def __batch_update_instances(self, lst_instances, session_id=None):
       """
@@ -369,15 +369,15 @@
           PAYLOAD_DATA.NAME: self.name,
           PAYLOAD_DATA.SIGNATURE: instance.signature,
           PAYLOAD_DATA.INSTANCE_ID: instance.instance_id,
           PAYLOAD_DATA.INSTANCE_CONFIG: instance._get_proposed_config_dictionary()
         })
 
       self.session._send_command_batch_update_instance_config(
-        worker=self.e2id,
+        worker=self.node_id,
         lst_updates=lst_updates,
         session_id=session_id
       )
 
     def __pop_ignored_keys_from_config(self, config):
       """
       Pop the ignored keys from the configuration.
@@ -476,15 +476,15 @@
     def __apply_staged_config(self):
       """
       Apply the staged configuration to the pipeline.
       """
       if self.__staged_config is None:
         return
 
-      self.P("Deployed pipeline <{}> on <{}>".format(self.name, self.e2id), color="g")
+      self.P("Deployed pipeline <{}> on <{}>".format(self.name, self.node_id), color="g")
       self.__was_last_operation_successful = True
 
       self.config = {**self.config, **self.__staged_config}
       self.__staged_config = None
 
       return
 
@@ -564,15 +564,15 @@
       -------
       list[Transaction]
           The list of transactions generated.
       """
       transactions = self.__register_transactions_for_delete(timeout=10)
 
       self.session._send_command_archive_pipeline(
-        worker=self.e2id,
+        worker=self.node_id,
         pipeline_name=self.name,
       )
 
       return transactions
 
   # Message handling
   if True:
@@ -1141,15 +1141,15 @@
       -------
       list[Transaction] | None
           The list of transactions generated, or None if `wait_for_confirmation` is False.
       """
       transactions = self.__register_transaction_for_pipeline_command(timeout=timeout)
 
       self.session._send_command_pipeline_command(
-        worker=self.e2id,
+        worker=self.node_id,
         pipeline_name=self.name,
         command=command,
         payload=payload,
         command_params=command_params,
       )
 
       if wait_for_confirmation:
```

### Comparing `pye2-0.8.0/PyE2/base/plugin_template.py` & `pye2-0.8.1/PyE2/base/plugin_template.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/base/responses.py` & `pye2-0.8.1/PyE2/base/responses.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/base/transaction.py` & `pye2-0.8.1/PyE2/base/transaction.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/base/payload/payload.py` & `pye2-0.8.1/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/bc/base.py` & `pye2-0.8.1/PyE2/bc/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/bc/ec.py` & `pye2-0.8.1/PyE2/bc/ec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/code_cheker/base.py` & `pye2-0.8.1/PyE2/code_cheker/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/comm/amqp_wrapper.py` & `pye2-0.8.1/PyE2/comm/amqp_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 
 from ..const import COLORS, COMMS, BASE_CT, PAYLOAD_CT
 
 
 class AMQPWrapper(object):
   def __init__(
-    self, 
-    log, 
-    config, 
-    recv_buff=None, 
-    send_channel_name=None, 
-    recv_channel_name=None, 
+    self,
+    log,
+    config,
+    recv_buff=None,
+    send_channel_name=None,
+    recv_channel_name=None,
     comm_type=None,
-    verbosity=1, 
+    verbosity=1,
     **kwargs
   ):
     self._config = config
     self._recv_buff = recv_buff
     self._send_to = None
     self._comm_type = comm_type
     self.__verbosity = verbosity
@@ -92,15 +92,15 @@
     return self._config[COMMS.PORT]
 
   @property
   def cfg_routing_key(self):
     return self._config.get(COMMS.ROUTING_KEY, "")
 
   @property
-  def cfg_eeid(self):
+  def cfg_node_id(self):
     return self._config.get(COMMS.EE_ID, self._config.get(COMMS.SB_ID, None))
 
   @property
   def send_channel_def(self):
     if self.send_channel_name is None:
       return
 
@@ -120,15 +120,15 @@
       return
 
     cfg = self._config[self.recv_channel_name].copy()
     queue = cfg.get(COMMS.QUEUE, cfg[COMMS.EXCHANGE])
     cfg[COMMS.QUEUE] = queue
     _queue_device_specific = cfg.pop(COMMS.QUEUE_DEVICE_SPECIFIC, True)
     if _queue_device_specific:
-      cfg[COMMS.QUEUE] += '/{}'.format(self.cfg_eeid)
+      cfg[COMMS.QUEUE] += '/{}'.format(self.cfg_node_id)
     cfg[COMMS.QUEUE] += '/{}'.format(str(uuid.uuid4())[:8])
     return cfg
 
   @property
   def connection(self):
     return self._connection
```

### Comparing `pye2-0.8.0/PyE2/comm/mqtt_wrapper.py` & `pye2-0.8.1/PyE2/comm/mqtt_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
   @recv_channel_name.setter
   def recv_channel_name(self, x):
     self._recv_channel_name = x
     return
 
   @property
-  def cfg_eeid(self):
+  def cfg_node_id(self):
     return self._config.get(COMMS.EE_ID, self._config.get(COMMS.SB_ID, None))
 
   @property
   def cfg_user(self):
     return self._config[COMMS.USER]
 
   @property
@@ -142,15 +142,15 @@
   def recv_channel_def(self):
     if self.recv_channel_name is None:
       return
 
     cfg = self._config[self.recv_channel_name].copy()
     topic = cfg[COMMS.TOPIC]
     if "{}" in topic:
-      topic = topic.format(self.cfg_eeid)
+      topic = topic.format(self.cfg_node_id)
 
     cfg[COMMS.TOPIC] = topic
     return cfg
 
   @property
   def send_channel_def(self):
     if self.send_channel_name is None:
```

### Comparing `pye2-0.8.0/PyE2/const/base.py` & `pye2-0.8.1/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/const/comms.py` & `pye2-0.8.1/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/const/heartbeat.py` & `pye2-0.8.1/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/const/payload.py` & `pye2-0.8.1/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/default/mqtt_session.py` & `pye2-0.8.1/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.8.1/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.8.1/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.8.1/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/io_formatter/default/aixp1.py` & `pye2-0.8.1/PyE2/io_formatter/default/aixp1.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 
     return lvl_0_dct
 
   def _decode_output(self, encoded_output):
     # Pop the unimportant stuff
     encoded_output.get('EE_FORMATTER', None)
 
-    ee_id, pipeline, signature, instance_id = encoded_output.get('EE_PAYLOAD_PATH', [None, None, None, None])
+    node_id, pipeline, signature, instance_id = encoded_output.get('EE_PAYLOAD_PATH', [None, None, None, None])
 
-    encoded_output['EE_ID'] = ee_id
+    encoded_output['EE_ID'] = node_id
 
     if encoded_output['EE_EVENT_TYPE'] != 'HEARTBEAT':
       encoded_output['STREAM_NAME'] = pipeline
 
     if pipeline is not None:
       encoded_output['SIGNATURE'] = signature
```

### Comparing `pye2-0.8.0/PyE2/io_formatter/default/cavi2.py` & `pye2-0.8.1/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/base_logger.py` & `pye2-0.8.1/PyE2/logging/base_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/small_logger.py` & `pye2-0.8.1/PyE2/logging/small_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/__init__.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/class_instance_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/class_instance_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/computer_vision_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/computer_vision_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/datetime_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/datetime_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/download_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/download_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/general_serialization_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/general_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/json_serialization_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/json_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/pickle_serialization_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/pickle_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/process_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/process_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/resource_size_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/resource_size_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/timers_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/timers_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/upload_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/upload_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/logger_mixins/utils_mixin.py` & `pye2-0.8.1/PyE2/logging/logger_mixins/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/tzlocal/unix.py` & `pye2-0.8.1/PyE2/logging/tzlocal/unix.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/tzlocal/utils.py` & `pye2-0.8.1/PyE2/logging/tzlocal/utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/tzlocal/win32.py` & `pye2-0.8.1/PyE2/logging/tzlocal/win32.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/logging/tzlocal/windows_tz.py` & `pye2-0.8.1/PyE2/logging/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/tutorials/1. hello_world.py` & `pye2-0.8.1/PyE2/tutorials/1. hello_world.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 In this example, we connect to the network, listen for heartbeats from 
   DecentrAI nodes and print the CPU of each node.
 """
 
 from PyE2 import Session
 
 
-def on_hb(session: Session, e2id: str, data: dict):
-  session.P("{} has a {}".format(e2id, data['CPU']))
+def on_hb(session: Session, node_id: str, data: dict):
+  session.P("{} has a {}".format(node_id, data['CPU']))
   return
 
 
 if __name__ == '__main__':
   # create a session
   # the network credentials are read from the .env file automatically
   session = Session(
```

### Comparing `pye2-0.8.0/PyE2/tutorials/2. first_deploy.py` & `pye2-0.8.1/PyE2/tutorials/2. first_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   chosen_node = session.get_active_nodes()[0]
 
   # we have our node, let's deploy a plugin
 
   # first, we create a pipeline
   # we will use the video file data source, since we want to extract frames from a video
   pipeline: Pipeline = session.create_pipeline(
-    e2id=chosen_node,
+    node_id=chosen_node,
     name='first_deploy',
     data_source='VideoFile',
     config={
       'URL': "https://www.dropbox.com/scl/fi/8z2wpeelhav3k2dv8bb5p/Cars_3.mp4?rlkey=imv415rr3j1tx3zstpurlxkqb&dl=1"
     }
   )
```

### Comparing `pye2-0.8.0/PyE2/tutorials/3. simple_real_time_custom_code.py` & `pye2-0.8.1/PyE2/tutorials/3. simple_real_time_custom_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
   chosen_node = session.get_active_nodes()[0]
 
   # we have our node, let's deploy a plugin
 
   # first, we create a pipeline
   # we will use the video file data source, since we want to extract frames from a video
   pipeline: Pipeline = session.create_pipeline(
-    e2id=chosen_node,
+    node_id=chosen_node,
     name='real_time_custom_code_deploy',
     data_source='VideoFile',
     config={
       'URL': "https://www.dropbox.com/scl/fi/8z2wpeelhav3k2dv8bb5p/Cars_3.mp4?rlkey=imv415rr3j1tx3zstpurlxkqb&dl=1"
     }
   )
```

### Comparing `pye2-0.8.0/PyE2/tutorials/4. real_time_custom_code_2.py` & `pye2-0.8.1/PyE2/tutorials/4. real_time_custom_code_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   chosen_node = session.get_active_nodes()[0]
 
   # we have our node, let's deploy a plugin
 
   # first, we create a pipeline
   # we will use the video file data source, since we want to extract frames from a video
   pipeline: Pipeline = session.create_pipeline(
-    e2id=chosen_node,
+    node_id=chosen_node,
     name='real_time_custom_code_deploy',
     data_source='VideoFile',
     cap_resolution=5,
     config={
       'URL': "https://www.dropbox.com/scl/fi/8z2wpeelhav3k2dv8bb5p/Cars_3.mp4?rlkey=imv415rr3j1tx3zstpurlxkqb&dl=1"
     }
   )
```

### Comparing `pye2-0.8.0/PyE2/tutorials/5. real_time_custom_code_multithreading.py` & `pye2-0.8.1/PyE2/tutorials/5. real_time_custom_code_multithreading.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
   s = Session()
 
   s.wait_for_any_node()
 
   node = s.get_active_nodes()[0]
 
   p = s.create_or_attach_to_pipeline(
-    e2id=node,
+    node_id=node,
     name="run_threading_api",
     data_source="Void"
   )
 
   p.create_or_attach_to_custom_plugin_instance(
     instance_id="run_threading_api_01",
     custom_code=plugin_custom_code,
```

### Comparing `pye2-0.8.0/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py` & `pye2-0.8.1/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
   s = Session()
 
   s.wait_for_any_node()
 
   node = s.get_active_nodes()[0]
 
   p = s.create_or_attach_to_pipeline(
-    e2id=node,
+    node_id=node,
     name="run_threading_api",
     data_source="Void"
   )
 
   p.create_or_attach_to_custom_plugin_instance(
     instance_id="run_threading_api_01",
     custom_code=plugin_custom_code,
```

### Comparing `pye2-0.8.0/PyE2/tutorials/7. real_time_custom_code_multithreading.py` & `pye2-0.8.1/PyE2/tutorials/7. real_time_custom_code_multithreading.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
   s = Session()
 
   s.wait_for_any_node()
 
   node = s.get_active_nodes()[0]
 
   p = s.create_or_attach_to_pipeline(
-    e2id=node,
+    node_id=node,
     name="run_threading_api",
     data_source="Void"
   )
 
   p.create_or_attach_to_custom_plugin_instance(
     instance_id="run_threading_api_01",
     custom_code=plugin_custom_code_map,
```

### Comparing `pye2-0.8.0/PyE2/tutorials/8. chatbot.py` & `pye2-0.8.1/PyE2/tutorials/8. chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import sleep
 from PyE2 import Session
 
 
 class LLMChat():
-  def __init__(self, e2id, pipeline_name) -> None:
-    self.e2id = e2id
+  def __init__(self, node_id, pipeline_name) -> None:
+    self.node_id = node_id
     self.pipeline_name = pipeline_name
     self.default_context = {
       "STRUCT_DATA": [{
         "request": "",
         "history": [],
         "system_info":
           "You are a python programmer assistant. Be as concise and correct as possible. Write only the code without explanations."
@@ -55,18 +55,18 @@
     self.pipeline.send_pipeline_command(to_send)
     return
 
   def main(self):
     self.sess = Session()
 
     self.sess.P("Please wait until the Execution Engine sends a heartbeat in order to attach to the desired plugin instance.")
-    self.sess.wait_for_node(self.e2id)
+    self.sess.wait_for_node(self.node_id)
 
     self.pipeline = self.sess.create_or_attach_to_pipeline(
-      e2id=self.e2id,
+      node_id=self.node_id,
       name=self.pipeline_name,
       data_source='OnDemandTextInput',
     )
 
     self.pipeline.create_or_attach_to_plugin_instance(
       instance_id="default",
       signature="code_assist_01",
```

### Comparing `pye2-0.8.0/PyE2/utils/code.py` & `pye2-0.8.1/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/utils/code_exec.py` & `pye2-0.8.1/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/utils/comm_utils.py` & `pye2-0.8.1/PyE2/utils/comm_utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/PyE2/utils/dotenv.py` & `pye2-0.8.1/PyE2/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/xperimental/attach_example.py` & `pye2-0.8.1/xperimental/attach_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,19 +23,19 @@
   'HOST': env_variables['AIXP_HOSTNAME'],
   'PORT': int(env_variables['AIXP_PORT']),
   'USER': env_variables['AIXP_USERNAME'],
   'PASS': env_variables['AIXP_PASSWORD'],
   'TOPIC': 'lummetry/ctrl',
 }
 
-e2id = 'e2id'
+node_id = 'node_id'
 sess = Session()
 
 pipeline = sess.attach_to_pipeline(
-  e2id=e2id,
+  node_id=node_id,
   name='test_mqtt',
   on_notification=pipeline_on_notification,
   max_wait_time=60
 )
 
 # now start a cyclic process
 inst = pipeline.attach_to_custom_plugin_instance('inst01', on_data=instance_on_data)
```

### Comparing `pye2-0.8.0/xperimental/ex1.py` & `pye2-0.8.1/xperimental/ex1.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
   # this could refresh a UI
   pipeline.P('Receive specific message from CUSTOM_EXEC_01:inst01 (hardcoded)')
 
 
 def pipeline_on_data(pipeline: Pipeline, signature, instance, data: Payload):
   # this could refresh a UI
   pipeline.P('Received data from box {} by server {}, stream:{}, plugin: {}, instance:{}, the following data:{}'.format(
-      pipeline.e2id,
+      pipeline.node_id,
       pipeline.session.server,
       pipeline.name,
       signature,
       instance,
       data
   ))
 
 
 if __name__ == '__main__':
 
-  e2id = 'stefan-box'
+  node_id = 'stefan-box'
 
   sess = Session()
 
   pipeline: Pipeline = sess.create_pipeline(
-      e2id=e2id,
+      node_id=node_id,
       name='test_normal',
       data_source='VideoStream',
       config={
           'URL': 0
       },
       on_data=pipeline_on_data
   )
```

### Comparing `pye2-0.8.0/xperimental/remote_exec.py` & `pye2-0.8.1/xperimental/remote_exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,37 +44,37 @@
 
 def pipeline_on_notification(pipeline, notification: dict):
   pipeline.P(
       "Received specific notification for pipeline {}".format(pipeline.name))
   return
 
 
-def sess_on_hb(sess, e2id, hb):
+def sess_on_hb(sess, node_id, hb):
   act_plug = hb['ACTIVE_PLUGINS']
   for plug in act_plug:
-    sess.P((e2id, plug['STREAM_ID'], plug['SIGNATURE'], plug['INSTANCE_ID']))
+    sess.P((node_id, plug['STREAM_ID'], plug['SIGNATURE'], plug['INSTANCE_ID']))
 
 
 load_dotenv()
 
 listener_params = {
   'HOST': os.getenv('AIXP_HOSTNAME'),
   'PORT': int(os.getenv('AIXP_PORT')),
   'USER': os.getenv('AIXP_USERNAME'),
   'PASS': os.getenv('AIXP_PASSWORD'),
   'TOPIC': 'lummetry/ctrl',
 }
 
-e2id = 'e2id'
+node_id = 'node_id'
 sess = Session(
   on_heartbeat=sess_on_hb
 )
 
 pipeline = sess.create_pipeline(
-    e2id=e2id,
+    node_id=node_id,
     name='test_mqtt',
     data_source='IotQueueListener',
     config={
         'STREAM_CONFIG_METADATA': listener_params,
         "RECONNECTABLE": True,
     },
     plugins=None,
```

### Comparing `pye2-0.8.0/xperimental/save_images.py` & `pye2-0.8.1/xperimental/save_images.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,21 +8,21 @@
   global val
   payload.get_image_as_PIL().save("images/img_{}.jpeg".format(val))
   val += 1
 
 
 if __name__ == '__main__':
   sess = Session(
-      filter_workers=['e2id']
+      filter_workers=['node_id']
   )
 
   sess.connect()
 
   pipeline = sess.create_pipeline(
-    e2id="e2id",
+    node_id="node_id",
     name="test",
     data_source="VideoFile",
     config={
       "URL": "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4",
       "LIVE": False,
     },
   )
```

### Comparing `pye2-0.8.0/xperimental/decentralized/chain_dist_example.py` & `pye2-0.8.1/xperimental/decentralized/chain_dist_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
   folder = os.path.split(__file__)[0]
   WORKER_CODE_PATH = os.path.join(folder, 'chain_dist_example_worker.py')
   INITIATOR_CODE_PATH = os.path.join(folder, 'chain_dist_example_initiator.py')
 
   with open(WORKER_CODE_PATH, 'rt') as fh:
     worker_code = fh.read()
 
-  e2id = 'stefan-box'  # provide a known EE id
-  sess = Session(filter_workers=[e2id])
+  node_id = 'stefan-box'  # provide a known EE id
+  sess = Session(filter_workers=[node_id])
 
   listener_params = {
     'HOST': os.getenv('AIXP_HOSTNAME'),
     'PORT': int(os.getenv('AIXP_PORT')),
     'USER': os.getenv('AIXP_USERNAME'),
     'PASS': os.getenv('AIXP_PASSWORD'),
     'TOPIC': 'lummetry/ctrl',
   }
 
   pipeline = sess.create_pipeline(
-      e2id=e2id,
+      node_id=node_id,
       name='test_dist_jobs',
       data_source='IotQueueListener',  # this DCT allows data acquisition from MQTT brokers
       config={
           'STREAM_CONFIG_METADATA': listener_params,
           "RECONNECTABLE": True,
       },
   )
```

### Comparing `pye2-0.8.0/xperimental/decentralized/chain_dist_example_initiator.py` & `pye2-0.8.1/xperimental/decentralized/chain_dist_example_initiator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-result=None
+result = None
 if plugin.int_cache['run_first_time'] == 0:
   # this is the first run, consider this the setup
-  
+
   plugin.int_cache['run_first_time'] = 1
 
   worker_code = plugin.cfg_worker_code
   n_workers = plugin.cfg_n_workers
   # we use DeAPI `plugin.deapi_get_wokers` call to get the needed workers
   plugin.obj_cache['lst_workers'] = plugin.deapi_get_wokers(n_workers)
   plugin.obj_cache['dct_workers'] = {}
   plugin.obj_cache['dct_worker_progress'] = {}
   plugin.P(plugin.obj_cache['lst_workers'])
-  
+
   # for each worker we symetrically launch the same job
   for worker in plugin.obj_cache['lst_workers']:
     plugin.obj_cache['dct_worker_progress'][worker] = []
     pipeline_name = plugin.cmdapi_start_simple_custom_pipeline(
-      base64code=worker_code, 
+      base64code=worker_code,
       dest=worker,
       instance_config={
-        'MAX_TRIES': plugin.cfg_max_tries, 
+        'MAX_TRIES': plugin.cfg_max_tries,
       }
     )
-    plugin.obj_cache['dct_workers'][worker] = pipeline_name 
+    plugin.obj_cache['dct_workers'][worker] = pipeline_name
   # endfor
-  
+
   plugin.obj_cache["start_time"] = plugin.datetime.now()
   # endfor
 elif (plugin.datetime.now() - plugin.obj_cache["start_time"]).seconds > plugin.cfg_max_run_time:
-  # if the configured time has elapsed we stop all the worker pipelines 
+  # if the configured time has elapsed we stop all the worker pipelines
   # as well as stop this pipeline itself
-  
-  for ee_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
-    plugin.cmdapi_archive_pipeline(dest=ee_id, name=pipeline_name)
+
+  for node_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
+    plugin.cmdapi_archive_pipeline(dest=node_id, name=pipeline_name)
   # now archive own pipeline
   plugin.cmdapi_archive_pipeline()
   result = {
-    'STATUS'  : 'DONE',
-    'RESULTS' : plugin.obj_cache['dct_worker_progress']
+    'STATUS': 'DONE',
+    'RESULTS': plugin.obj_cache['dct_worker_progress']
   }
 else:
   # here are the operations we are running periodically
-  payload = plugin.dataapi_struct_data() # we use the DataAPI to get upstream data
+  payload = plugin.dataapi_struct_data()  # we use the DataAPI to get upstream data
   if payload is not None:
-    
-    ee_id = payload.get('EE_ID', payload.get('SB_ID'))
+
+    node_id = payload.get('EE_ID', payload.get('SB_ID'))
     pipeline_name = payload.get('STREAM_NAME')
-    
-    if (ee_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
+
+    if (node_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
       # now we extract result from the result key of the payload JSON
       # this also can be configured to another name
       num = payload.get('EXEC_RESULT', payload.get('EXEC_INFO'))
       if num is not None:
-        plugin.obj_cache['dct_worker_progress'][ee_id].append(num)
+        plugin.obj_cache['dct_worker_progress'][node_id].append(num)
         result = {
-          'STATUS'  : 'IN_PROGRESS',
-          'RESULTS' : plugin.obj_cache['dct_worker_progress']
+          'STATUS': 'IN_PROGRESS',
+          'RESULTS': plugin.obj_cache['dct_worker_progress']
         }
   # endif
-# endif
+# endif
```

### Comparing `pye2-0.8.0/.gitignore` & `pye2-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/LICENSE` & `pye2-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.8.0/README.md` & `pye2-0.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 ```python
 from PyE2 import Session
 ```
 
 #### Preparing callbacks
 
 ```python
-def on_hb(session : Session, e2id : str, data : dict):
-  print(e2id, " has a ", data['CPU'])
+def on_hb(session : Session, node_id : str, data : dict):
+  print(node_id, " has a ", data['CPU'])
   return
 ```
 
 #### Running a simple main loop
 
 ```python
 if __name__ == '__main__':
@@ -136,36 +136,36 @@
 
   plugin.obj_cache["start_time"] = plugin.datetime.now()
   # endfor
 elif (plugin.datetime.now() - plugin.obj_cache["start_time"]).seconds > plugin.cfg_max_run_time:
   # if the configured time has elapsed we stop all the worker pipelines
   # as well as stop this pipeline itself
 
-  for ee_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
-    plugin.cmdapi_archive_pipeline(dest=ee_id, name=pipeline_name)
+  for node_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
+    plugin.cmdapi_archive_pipeline(dest=node_id, name=pipeline_name)
   # now archive own pipeline
   plugin.cmdapi_archive_pipeline()
   result = {
     'STATUS'  : 'DONE',
     'RESULTS' : plugin.obj_cache['dct_worker_progress']
   }
 else:
   # here are the operations we are running periodically
   payload = plugin.dataapi_struct_data() # we use the DataAPI to get upstream data
   if payload is not None:
 
-    ee_id = payload.get('EE_ID', payload.get('SB_ID'))
+    node_id = payload.get('EE_ID', payload.get('SB_ID'))
     pipeline_name = payload.get('STREAM_NAME')
 
-    if (ee_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
+    if (node_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
       # now we extract result from the result key of the payload JSON
       # this also can be configured to another name
       num = payload.get('EXEC_RESULT', payload.get('EXEC_INFO'))
       if num is not None:
-        plugin.obj_cache['dct_worker_progress'][ee_id].append(num)
+        plugin.obj_cache['dct_worker_progress'][node_id].append(num)
         result = {
           'STATUS'  : 'IN_PROGRESS',
           'RESULTS' : plugin.obj_cache['dct_worker_progress']
         }
   # endif
 # endif
 ```
@@ -197,24 +197,24 @@
 
   WORKER_CODE_PATH = 'chain_dist_example_worker.py'
   INITIATOR_CODE_PATH = 'chain_dist_example_initiator.py'
 
   with open(WORKER_CODE_PATH, 'rt') as fh:
     worker_code = fh.read()
 
-  e2id = 'e2id' # provide a known EE id
+  node_id = 'node_id' # provide a known EE id
   sess = Session(**SERVER_CONFIG, silent=True)
   sess.connect()
 
   listener_params = {k.upper(): v for k, v in SERVER_CONFIG.items()}
   listener_params["PASS"] = listener_params["PWD"]
   listener_params["TOPIC"] = "lummetry/payloads"
 
   pipeline = sess.create_pipeline(
-      e2id=e2id,
+      node_id=node_id,
       name='test_dist_jobs',
       data_source='IotQueueListener', # this DCT allows data acquisition from MQTT brokers
       config={
           'STREAM_CONFIG_METADATA': listener_params,
           "RECONNECTABLE": True,
       },
   )
@@ -306,15 +306,15 @@
   # Notice that we call `sess.connect()` before `sess.run()`. That is because in order
   # to create pipelines and to start plugin instances, we need to be connected to the session
   sess.connect()
 
   # Create a pipeline that will acquire data from a Video File located at the given URL
   # The URL can be a path to a local file or a link to a downloadable file
   pipeline = sess.create_pipeline(
-    e2id="e2id",
+    node_id="node_id",
     name="RealTimePersonTracking",
     data_source="VideoFile",
     config={
       "URL": "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4"
     },
   )
 
@@ -361,23 +361,23 @@
 
 - Feat(session): added `filter_workers` to Session, process only messages from specific workers
 - Feat(session): track online nodes and keep a list of them;
   consider a node offline if it did not send any message for more than 60 seconds
 
 BREAKING CHANGE:
 
-- Refactor(on_heartbeat): added `e2id` as parameter, now the signature of the method looks like this
+- Refactor(on_heartbeat): added `node_id` as parameter, now the signature of the method looks like this
 
   ```python
-  on_heartbeat(sess: Session, e2id: str, heartbeat: dict)
+  on_heartbeat(sess: Session, node_id: str, heartbeat: dict)
   ```
 
 ### v0.3.5
 
-- Hotfix(session): changed self.e2id to e2id
+- Hotfix(session): changed self.node_id to node_id
 
 ### v0.3.4
 
 - Added docstrings
 - Included examples with credentials from environment variables
 
 ### v0.3.2
```

### Comparing `pye2-0.8.0/pyproject.toml` & `pye2-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="Stefan Saraev", email="saraevstefan@gmail.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@me.com" },
   { name="Cristan Bleotiu", email="cristibleotiu@gmail.com" },
 ]
 description = "PyE2 is the Python SDK required for client app development in the DecentrAI network"
 readme = "README.md"
```

### Comparing `pye2-0.8.0/PKG-INFO` & `pye2-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyE2
-Version: 0.8.0
+Version: 0.8.1
 Summary: PyE2 is the Python SDK required for client app development in the DecentrAI network
 Project-URL: Homepage, https://github.com/DecentrAI/PyE2
 Project-URL: Bug Tracker, https://github.com/DecentrAI/PyE2/issues
 Author-email: Stefan Saraev <saraevstefan@gmail.com>, Andrei Ionut Damian <andrei.damian@me.com>, Cristan Bleotiu <cristibleotiu@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -66,16 +66,16 @@
 ```python
 from PyE2 import Session
 ```
 
 #### Preparing callbacks
 
 ```python
-def on_hb(session : Session, e2id : str, data : dict):
-  print(e2id, " has a ", data['CPU'])
+def on_hb(session : Session, node_id : str, data : dict):
+  print(node_id, " has a ", data['CPU'])
   return
 ```
 
 #### Running a simple main loop
 
 ```python
 if __name__ == '__main__':
@@ -157,36 +157,36 @@
 
   plugin.obj_cache["start_time"] = plugin.datetime.now()
   # endfor
 elif (plugin.datetime.now() - plugin.obj_cache["start_time"]).seconds > plugin.cfg_max_run_time:
   # if the configured time has elapsed we stop all the worker pipelines
   # as well as stop this pipeline itself
 
-  for ee_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
-    plugin.cmdapi_archive_pipeline(dest=ee_id, name=pipeline_name)
+  for node_id, pipeline_name in plugin.obj_cache['dct_workers'].items():
+    plugin.cmdapi_archive_pipeline(dest=node_id, name=pipeline_name)
   # now archive own pipeline
   plugin.cmdapi_archive_pipeline()
   result = {
     'STATUS'  : 'DONE',
     'RESULTS' : plugin.obj_cache['dct_worker_progress']
   }
 else:
   # here are the operations we are running periodically
   payload = plugin.dataapi_struct_data() # we use the DataAPI to get upstream data
   if payload is not None:
 
-    ee_id = payload.get('EE_ID', payload.get('SB_ID'))
+    node_id = payload.get('EE_ID', payload.get('SB_ID'))
     pipeline_name = payload.get('STREAM_NAME')
 
-    if (ee_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
+    if (node_id, pipeline_name) in plugin.obj_cache['dct_workers'].items():
       # now we extract result from the result key of the payload JSON
       # this also can be configured to another name
       num = payload.get('EXEC_RESULT', payload.get('EXEC_INFO'))
       if num is not None:
-        plugin.obj_cache['dct_worker_progress'][ee_id].append(num)
+        plugin.obj_cache['dct_worker_progress'][node_id].append(num)
         result = {
           'STATUS'  : 'IN_PROGRESS',
           'RESULTS' : plugin.obj_cache['dct_worker_progress']
         }
   # endif
 # endif
 ```
@@ -218,24 +218,24 @@
 
   WORKER_CODE_PATH = 'chain_dist_example_worker.py'
   INITIATOR_CODE_PATH = 'chain_dist_example_initiator.py'
 
   with open(WORKER_CODE_PATH, 'rt') as fh:
     worker_code = fh.read()
 
-  e2id = 'e2id' # provide a known EE id
+  node_id = 'node_id' # provide a known EE id
   sess = Session(**SERVER_CONFIG, silent=True)
   sess.connect()
 
   listener_params = {k.upper(): v for k, v in SERVER_CONFIG.items()}
   listener_params["PASS"] = listener_params["PWD"]
   listener_params["TOPIC"] = "lummetry/payloads"
 
   pipeline = sess.create_pipeline(
-      e2id=e2id,
+      node_id=node_id,
       name='test_dist_jobs',
       data_source='IotQueueListener', # this DCT allows data acquisition from MQTT brokers
       config={
           'STREAM_CONFIG_METADATA': listener_params,
           "RECONNECTABLE": True,
       },
   )
@@ -327,15 +327,15 @@
   # Notice that we call `sess.connect()` before `sess.run()`. That is because in order
   # to create pipelines and to start plugin instances, we need to be connected to the session
   sess.connect()
 
   # Create a pipeline that will acquire data from a Video File located at the given URL
   # The URL can be a path to a local file or a link to a downloadable file
   pipeline = sess.create_pipeline(
-    e2id="e2id",
+    node_id="node_id",
     name="RealTimePersonTracking",
     data_source="VideoFile",
     config={
       "URL": "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4"
     },
   )
 
@@ -382,23 +382,23 @@
 
 - Feat(session): added `filter_workers` to Session, process only messages from specific workers
 - Feat(session): track online nodes and keep a list of them;
   consider a node offline if it did not send any message for more than 60 seconds
 
 BREAKING CHANGE:
 
-- Refactor(on_heartbeat): added `e2id` as parameter, now the signature of the method looks like this
+- Refactor(on_heartbeat): added `node_id` as parameter, now the signature of the method looks like this
 
   ```python
-  on_heartbeat(sess: Session, e2id: str, heartbeat: dict)
+  on_heartbeat(sess: Session, node_id: str, heartbeat: dict)
   ```
 
 ### v0.3.5
 
-- Hotfix(session): changed self.e2id to e2id
+- Hotfix(session): changed self.node_id to node_id
 
 ### v0.3.4
 
 - Added docstrings
 - Included examples with credentials from environment variables
 
 ### v0.3.2
```

