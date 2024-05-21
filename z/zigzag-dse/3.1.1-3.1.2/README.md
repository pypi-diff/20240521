# Comparing `tmp/zigzag_dse-3.1.1.tar.gz` & `tmp/zigzag_dse-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag_dse-3.1.1.tar", last modified: Fri May 17 09:36:18 2024, max compression
+gzip compressed data, was "zigzag_dse-3.1.2.tar", last modified: Tue May 21 12:13:06 2024, max compression
```

## Comparing `zigzag_dse-3.1.1.tar` & `zigzag_dse-3.1.2.tar`

### file list

```diff
@@ -1,167 +1,160 @@
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:18.010040 zigzag_dse-3.1.1/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1074 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/LICENSE
--rw-r--r--   0 asymons  (27005) micas     (3600)       88 2024-01-03 17:20:40.000000 zigzag_dse-3.1.1/MANIFEST.in
--rw-r--r--   0 asymons  (27005) micas     (3600)    10698 2024-05-17 09:36:18.008040 zigzag_dse-3.1.1/PKG-INFO
--rw-r--r--   0 asymons  (27005) micas     (3600)     8519 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/README.md
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.673026 zigzag_dse-3.1.1/lab1/
--rw-r--r--   0 asymons  (27005) micas     (3600)     3577 2024-05-17 09:24:49.000000 zigzag_dse-3.1.1/lab1/main.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.602023 zigzag_dse-3.1.1/lab2/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.675026 zigzag_dse-3.1.1/lab2/solutions/
--rw-r--r--   0 asymons  (27005) micas     (3600)     3509 2024-05-17 09:24:49.000000 zigzag_dse-3.1.1/lab2/solutions/main.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.678026 zigzag_dse-3.1.1/lab3/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1484 2024-05-17 09:24:49.000000 zigzag_dse-3.1.1/lab3/main.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1577 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/pyproject.toml
--rw-r--r--   0 asymons  (27005) micas     (3600)       38 2024-05-17 09:36:18.010040 zigzag_dse-3.1.1/setup.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.605023 zigzag_dse-3.1.1/tests/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.609023 zigzag_dse-3.1.1/tests/main/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.685027 zigzag_dse-3.1.1/tests/main/test_imc/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_imc/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1598 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_imc/test_aimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1571 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_imc/test_dimc.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.698027 zigzag_dse-3.1.1/tests/main/test_origin/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1159 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1159 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1172 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1158 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1144 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.713028 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2070 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2716 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2144 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2113 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2281 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.726028 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1310 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1329 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1341 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1335 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1320 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.738029 zigzag_dse-3.1.1/zigzag/
--rw-r--r--   0 asymons  (27005) micas     (3600)       22 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3175 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/__main__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    20951 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/api.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.740029 zigzag_dse-3.1.1/zigzag/cacti/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.745029 zigzag_dse-3.1.1/zigzag/cacti/cacti_master/
--rw-r--r--   0 asymons  (27005) micas     (3600)    19996 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4266 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7388 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cacti/cacti_parser.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.751029 zigzag_dse-3.1.1/zigzag/cost_model/
--rw-r--r--   0 asymons  (27005) micas     (3600)    19531 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cost_model/CostModelEvaluationForIMC.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    58803 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cost_model/cost_model.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3460 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cost_model/port_activity.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3417 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/datatypes.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.615023 zigzag_dse-3.1.1/zigzag/hardware/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.816032 zigzag_dse-3.1.1/zigzag/hardware/architecture/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1164 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/Accelerator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      912 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/Adder.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    22786 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/AimcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5441 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/Core.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    41212 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/DimcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1881 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/ImcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     8583 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryHierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3730 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryInstance.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    27401 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/get_cacti_cost.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    10950 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/imc_unit.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7046 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/memory_level.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2680 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/memory_port.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2830 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_array.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1728 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_unit.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.618023 zigzag_dse-3.1.1/zigzag/inputs/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.619024 zigzag_dse-3.1.1/zigzag/inputs/validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.620024 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.648025 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.647025 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.834033 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7533 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    10670 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     8317 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1557 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     5101 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    12528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.651025 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.850033 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    12528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     5094 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1433 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    15946 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     8348 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     3649 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.865034 zigzag_dse-3.1.1/zigzag/mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)    31830 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/Mapping.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     8281 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/SpatialMappingInternal.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6848 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/TemporalMapping.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     8031 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/data_movement.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     8296 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/mapping_assist_funcs.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14492 2024-05-16 14:37:13.000000 zigzag_dse-3.1.1/zigzag/mapping/spatial_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.656025 zigzag_dse-3.1.1/zigzag/opt/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.874034 zigzag_dse-3.1.1/zigzag/opt/loma/
--rw-r--r--   0 asymons  (27005) micas     (3600)    11960 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/LomaEngine.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      532 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/Loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    17039 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/MemoryAllocator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2444 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/multipermute.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.878034 zigzag_dse-3.1.1/zigzag/opt/salsa/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8189 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaEngine.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaState.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.893035 zigzag_dse-3.1.1/zigzag/parser/
--rw-r--r--   0 asymons  (27005) micas     (3600)     9155 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/AcceleratorValidator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4035 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/MappingValidator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3405 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/UpgradedValidator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5314 2024-05-16 09:09:31.000000 zigzag_dse-3.1.1/zigzag/parser/WorkloadValidator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7711 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/accelerator_factory.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.909036 zigzag_dse-3.1.1/zigzag/parser/onnx/
--rw-r--r--   0 asymons  (27005) micas     (3600)     5399 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/ConvParser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1029 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/DefaultNodeParser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4987 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/GemmParser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3435 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/MatMulParser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4209 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/ONNXModelParser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1931 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/ONNXOperatorParser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7891 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/utils.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    11778 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/workload_factory.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.959038 zigzag_dse-3.1.1/zigzag/stages/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1515 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/AcceleratorParserStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2721 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/CostModelStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1542 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/DumpStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2556 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1831 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/LomaStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      731 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/MainStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      862 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/ONNXModelParserStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6002 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/PEArrayScalingStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1630 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9273 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/RemoveUnusedMemoryStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6024 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/SalsaStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    28132 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/SearchUnusedMemoryStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14263 2024-05-16 15:04:44.000000 zigzag_dse-3.1.1/zigzag/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    33280 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1980 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/Stage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3034 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2427 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/WorkloadParserStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1908 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/WorkloadStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5236 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/reduce_stages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6322 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/run_opt_stages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6348 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/save_stages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2146 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/utils.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.663025 zigzag_dse-3.1.1/zigzag/visualization/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.964038 zigzag_dse-3.1.1/zigzag/visualization/graph/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1626 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      963 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.969038 zigzag_dse-3.1.1/zigzag/visualization/results/
--rw-r--r--   0 asymons  (27005) micas     (3600)     9369 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5532 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.989039 zigzag_dse-3.1.1/zigzag/workload/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1130 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/DNNWorkload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2260 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/DummyNode.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      890 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/LayerAttribute.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      611 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/LayerNodeABC.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1083 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/ONNXWorkload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1063 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/Workload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6904 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/workload/layer_attributes.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14891 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/layer_node.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:18.005040 zigzag_dse-3.1.1/zigzag_dse.egg-info/
--rw-r--r--   0 asymons  (27005) micas     (3600)    10698 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 asymons  (27005) micas     (3600)     5368 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)        1 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)       52 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)      116 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)       39 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.290553 zigzag_dse-3.1.2/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1074 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/LICENSE
+-rw-r--r--   0 asymons  (27005) micas     (3600)       88 2024-01-03 17:20:40.000000 zigzag_dse-3.1.2/MANIFEST.in
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10698 2024-05-21 12:13:06.288553 zigzag_dse-3.1.2/PKG-INFO
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8519 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/README.md
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1577 2024-05-21 12:12:56.000000 zigzag_dse-3.1.2/pyproject.toml
+-rw-r--r--   0 asymons  (27005) micas     (3600)       38 2024-05-21 12:13:06.291553 zigzag_dse-3.1.2/setup.cfg
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.009541 zigzag_dse-3.1.2/tests/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.023542 zigzag_dse-3.1.2/tests/main/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.068544 zigzag_dse-3.1.2/tests/main/test_imc/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_imc/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1598 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_imc/test_aimc.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1571 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_imc/test_dimc.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.076544 zigzag_dse-3.1.2/tests/main/test_origin/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1159 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_origin/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1159 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_origin/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1172 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_origin/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1158 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_origin/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1144 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_origin/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.085545 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:38.000000 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2070 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2716 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2144 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2113 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2281 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.095545 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1310 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1329 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1341 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1335 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1320 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.103545 zigzag_dse-3.1.2/zigzag/
+-rw-r--r--   0 asymons  (27005) micas     (3600)       22 2024-05-21 12:12:56.000000 zigzag_dse-3.1.2/zigzag/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3175 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/__main__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    20951 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/api.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.104545 zigzag_dse-3.1.2/zigzag/cacti/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.108546 zigzag_dse-3.1.2/zigzag/cacti/cacti_master/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19996 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4266 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7388 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/cacti/cacti_parser.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.114546 zigzag_dse-3.1.2/zigzag/cost_model/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19531 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/cost_model/CostModelEvaluationForIMC.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    58803 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/cost_model/cost_model.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3460 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/cost_model/port_activity.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3417 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/datatypes.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.030542 zigzag_dse-3.1.2/zigzag/hardware/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.142547 zigzag_dse-3.1.2/zigzag/hardware/architecture/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1164 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/Accelerator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      912 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/Adder.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    22786 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/AimcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5441 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/Core.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    41212 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/DimcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1881 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/ImcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8583 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/MemoryHierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3730 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/MemoryInstance.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    27401 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/get_cacti_cost.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10950 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/imc_unit.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7046 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/memory_level.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2680 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/memory_port.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2830 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/operational_array.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1728 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.032542 zigzag_dse-3.1.2/zigzag/inputs/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.033542 zigzag_dse-3.1.2/zigzag/inputs/validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.034542 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.037542 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.036543 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.153547 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     7533 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    10670 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     8317 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1557 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     5101 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    12528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.038543 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.166548 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    12528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     5094 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1433 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    15946 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     8348 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     3649 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.177549 zigzag_dse-3.1.2/zigzag/mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    31830 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/mapping/Mapping.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8281 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/mapping/SpatialMappingInternal.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6848 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/mapping/TemporalMapping.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8031 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/mapping/data_movement.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8296 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/mapping/mapping_assist_funcs.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14492 2024-05-16 14:37:13.000000 zigzag_dse-3.1.2/zigzag/mapping/spatial_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.048543 zigzag_dse-3.1.2/zigzag/opt/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.184549 zigzag_dse-3.1.2/zigzag/opt/loma/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11960 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/opt/loma/LomaEngine.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      532 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/opt/loma/Loop.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    17039 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/opt/loma/MemoryAllocator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2444 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/opt/loma/multipermute.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.188549 zigzag_dse-3.1.2/zigzag/opt/salsa/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8189 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/opt/salsa/SalsaEngine.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/opt/salsa/SalsaState.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.199549 zigzag_dse-3.1.2/zigzag/parser/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9155 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/parser/AcceleratorValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4110 2024-05-21 11:54:56.000000 zigzag_dse-3.1.2/zigzag/parser/MappingValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3405 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/parser/UpgradedValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5314 2024-05-16 09:09:31.000000 zigzag_dse-3.1.2/zigzag/parser/WorkloadValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7711 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/parser/accelerator_factory.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.210550 zigzag_dse-3.1.2/zigzag/parser/onnx/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5399 2024-05-16 12:47:21.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/ConvParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1029 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/DefaultNodeParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4987 2024-05-16 12:47:21.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/GemmParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3435 2024-05-16 12:47:21.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/MatMulParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4209 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/ONNXModelParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1931 2024-05-16 12:47:21.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/ONNXOperatorParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7891 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/parser/onnx/utils.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    12037 2024-05-21 12:09:36.000000 zigzag_dse-3.1.2/zigzag/parser/workload_factory.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.248551 zigzag_dse-3.1.2/zigzag/stages/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1515 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/AcceleratorParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2721 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/CostModelStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1542 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/DumpStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2556 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1831 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/LomaStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      731 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/MainStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      862 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/ONNXModelParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6002 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/PEArrayScalingStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1630 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9273 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/RemoveUnusedMemoryStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6024 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/SalsaStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    28132 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/SearchUnusedMemoryStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14263 2024-05-16 15:04:44.000000 zigzag_dse-3.1.2/zigzag/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    33280 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1980 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/Stage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3034 2024-05-16 12:47:21.000000 zigzag_dse-3.1.2/zigzag/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2427 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/WorkloadParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1908 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/WorkloadStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5236 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/reduce_stages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6322 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/run_opt_stages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6348 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/stages/save_stages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2146 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/utils.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.054543 zigzag_dse-3.1.2/zigzag/visualization/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.252552 zigzag_dse-3.1.2/zigzag/visualization/graph/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1626 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      963 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.255552 zigzag_dse-3.1.2/zigzag/visualization/results/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9369 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5532 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.269552 zigzag_dse-3.1.2/zigzag/workload/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1130 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/workload/DNNWorkload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2260 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/workload/DummyNode.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      890 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/workload/LayerAttribute.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      611 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/workload/LayerNodeABC.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1083 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/workload/ONNXWorkload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1063 2024-05-15 14:16:39.000000 zigzag_dse-3.1.2/zigzag/workload/Workload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6904 2024-05-16 12:47:21.000000 zigzag_dse-3.1.2/zigzag/workload/layer_attributes.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    15144 2024-05-21 12:11:09.000000 zigzag_dse-3.1.2/zigzag/workload/layer_node.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-21 12:13:06.285553 zigzag_dse-3.1.2/zigzag_dse.egg-info/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10698 2024-05-21 12:13:05.000000 zigzag_dse-3.1.2/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5319 2024-05-21 12:13:06.000000 zigzag_dse-3.1.2/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)        1 2024-05-21 12:13:05.000000 zigzag_dse-3.1.2/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)       52 2024-05-21 12:13:05.000000 zigzag_dse-3.1.2/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)      116 2024-05-21 12:13:05.000000 zigzag_dse-3.1.2/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)       39 2024-05-21 12:13:05.000000 zigzag_dse-3.1.2/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag_dse-3.1.1/LICENSE` & `zigzag_dse-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/PKG-INFO` & `zigzag_dse-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 3.1.1
+Version: 3.1.2
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2021 MICAS (KU Leuven)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zigzag_dse-3.1.1/README.md` & `zigzag_dse-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/pyproject.toml` & `zigzag_dse-3.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "3.1.1"
+version = "3.1.2"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "3.1.1"
+current_version = "3.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag_dse-3.1.1/tests/main/test_imc/test_aimc.py` & `zigzag_dse-3.1.2/tests/main/test_imc/test_aimc.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_imc/test_dimc.py` & `zigzag_dse-3.1.2/tests/main/test_imc/test_dimc.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_origin/test_ascend_like.py` & `zigzag_dse-3.1.2/tests/main/test_origin/test_ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_origin/test_edge_tpu_like.py` & `zigzag_dse-3.1.2/tests/main/test_origin/test_edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_origin/test_meta_prototype_like.py` & `zigzag_dse-3.1.2/tests/main/test_origin/test_meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_origin/test_tesla_npu_like.py` & `zigzag_dse-3.1.2/tests/main/test_origin/test_tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_origin/test_tpu_like.py` & `zigzag_dse-3.1.2/tests/main/test_origin/test_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py` & `zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py` & `zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py` & `zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py` & `zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py` & `zigzag_dse-3.1.2/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_ascend_like.py` & `zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_edge_tpu_like.py` & `zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_meta_prototype_like.py` & `zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tesla_npu_like.py` & `zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tpu_like.py` & `zigzag_dse-3.1.2/tests/main/test_without_unused_memory/test_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/__main__.py` & `zigzag_dse-3.1.2/zigzag/__main__.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/api.py` & `zigzag_dse-3.1.2/zigzag/api.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_config_creator.py` & `zigzag_dse-3.1.2/zigzag/cacti/cacti_master/cacti_config_creator.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_top.py` & `zigzag_dse-3.1.2/zigzag/cacti/cacti_master/cacti_top.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/cacti/cacti_parser.py` & `zigzag_dse-3.1.2/zigzag/cacti/cacti_parser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/cost_model/CostModelEvaluationForIMC.py` & `zigzag_dse-3.1.2/zigzag/cost_model/CostModelEvaluationForIMC.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/cost_model/cost_model.py` & `zigzag_dse-3.1.2/zigzag/cost_model/cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/cost_model/port_activity.py` & `zigzag_dse-3.1.2/zigzag/cost_model/port_activity.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/datatypes.py` & `zigzag_dse-3.1.2/zigzag/datatypes.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/Accelerator.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/Accelerator.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/Adder.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/Adder.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/AimcArray.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/AimcArray.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/Core.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/Core.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/DimcArray.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/DimcArray.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/ImcArray.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/ImcArray.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryHierarchy.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/MemoryHierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryInstance.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/MemoryInstance.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/get_cacti_cost.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/get_cacti_cost.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/imc_unit.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/imc_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/memory_level.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/memory_level.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/memory_port.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/memory_port.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_array.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/operational_array.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_unit.py` & `zigzag_dse-3.1.2/zigzag/hardware/architecture/operational_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py` & `zigzag_dse-3.1.2/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/mapping/Mapping.py` & `zigzag_dse-3.1.2/zigzag/mapping/Mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/mapping/SpatialMappingInternal.py` & `zigzag_dse-3.1.2/zigzag/mapping/SpatialMappingInternal.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/mapping/TemporalMapping.py` & `zigzag_dse-3.1.2/zigzag/mapping/TemporalMapping.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/mapping/data_movement.py` & `zigzag_dse-3.1.2/zigzag/mapping/data_movement.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/mapping/mapping_assist_funcs.py` & `zigzag_dse-3.1.2/zigzag/mapping/mapping_assist_funcs.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/mapping/spatial_mapping.py` & `zigzag_dse-3.1.2/zigzag/mapping/spatial_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/opt/loma/LomaEngine.py` & `zigzag_dse-3.1.2/zigzag/opt/loma/LomaEngine.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/opt/loma/Loop.py` & `zigzag_dse-3.1.2/zigzag/opt/loma/Loop.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/opt/loma/MemoryAllocator.py` & `zigzag_dse-3.1.2/zigzag/opt/loma/MemoryAllocator.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/opt/loma/multipermute.py` & `zigzag_dse-3.1.2/zigzag/opt/loma/multipermute.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaEngine.py` & `zigzag_dse-3.1.2/zigzag/opt/salsa/SalsaEngine.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaState.py` & `zigzag_dse-3.1.2/zigzag/opt/salsa/SalsaState.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/AcceleratorValidator.py` & `zigzag_dse-3.1.2/zigzag/parser/AcceleratorValidator.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/MappingValidator.py` & `zigzag_dse-3.1.2/zigzag/parser/MappingValidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     # Schema for a single operation, UpgradeValidator extrapolates to list of operations
     SCHEMA_SINGLE = {
         "name": {
             "type": "string",
             "required": True,
         },
         "core_allocation": {"type": "list", "schema": {"type": "integer"}, "default": [0]},
+        "core_allocation_is_fixed": {"type": "boolean", "default": False},
         "spatial_mapping": {
             "type": "dict",
             "schema": {
                 "D1": {"type": "list", "schema": {"type": "string", "regex": r"^[A-Z]+, [0-9]+$"}, "required": False},
                 "D2": {"type": "list", "schema": {"type": "string", "regex": r"^[A-Z]+, [0-9]+$"}, "required": False},
                 "D3": {"type": "list", "schema": {"type": "string", "regex": r"^[A-Z]+, [0-9]+$"}, "required": False},
                 "D4": {"type": "list", "schema": {"type": "string", "regex": r"^[A-Z]+, [0-9]+$"}, "required": False},
```

### Comparing `zigzag_dse-3.1.1/zigzag/parser/UpgradedValidator.py` & `zigzag_dse-3.1.2/zigzag/parser/UpgradedValidator.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/WorkloadValidator.py` & `zigzag_dse-3.1.2/zigzag/parser/WorkloadValidator.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/accelerator_factory.py` & `zigzag_dse-3.1.2/zigzag/parser/accelerator_factory.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/ConvParser.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/ConvParser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/DefaultNodeParser.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/DefaultNodeParser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/GemmParser.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/GemmParser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/MatMulParser.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/MatMulParser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/ONNXModelParser.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/ONNXModelParser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/ONNXOperatorParser.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/ONNXOperatorParser.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/onnx/utils.py` & `zigzag_dse-3.1.2/zigzag/parser/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/parser/workload_factory.py` & `zigzag_dse-3.1.2/zigzag/parser/workload_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,28 +72,30 @@
         pr_layer_dim_sizes = self.create_pr_layer_dim_sizes()
 
         # From mapping data
         mapping_factory = MappingFactory(self.node_name, layer_type, self.mapping_data)
         spatial_mapping = mapping_factory.create_spatial_mapping()
         spatial_mapping_hint = mapping_factory.create_spatial_mapping_hint()
         core_allocation = mapping_factory.get_core_allocation()
+        core_allocation_is_fixed = mapping_factory.get_core_allocation_is_fixed()
         memory_operand_links = mapping_factory.create_memory_operand_links()
         temporal_ordering = mapping_factory.create_temporal_ordering()
 
         return LayerNodeAttributes(
             layer_type=layer_type,
             equation=equation,
             layer_dim_sizes=layer_dim_sizes,
             operand_precision=operand_precision,
             dimension_relations=dimension_relations,
             constant_operands=constant_operands,
             input_operand_source=input_operand_source,
             spatial_mapping=spatial_mapping,
             spatial_mapping_hint=spatial_mapping_hint,
             core_allocation=core_allocation,
+            core_allocation_is_fixed=core_allocation_is_fixed,
             memory_operand_links=memory_operand_links,
             temporal_ordering=temporal_ordering,
             padding=padding,
             pr_layer_dim_sizes=pr_layer_dim_sizes,
         )
 
     def create_equation(self) -> LayerEquation:
@@ -194,14 +196,17 @@
         else:
             self.mapping_data = next(filter(lambda x: x["name"] == "default", mapping_data))
             logger.warning("Operator %s not defined in mapping. Using default mapping instead.", operation_type)
 
     def get_core_allocation(self) -> list[int]:
         return self.mapping_data["core_allocation"]
 
+    def get_core_allocation_is_fixed(self) -> bool:
+        return self.mapping_data["core_allocation_is_fixed"]
+
     def create_spatial_mapping(self) -> SpatialMapping:
         if self.mapping_data["spatial_mapping"] is None:
             return SpatialMapping.empty()
 
         user_data: dict[str, list[str]] = self.mapping_data["spatial_mapping"]
         spatial_mapping_dict: dict[OADimension, MappingSingleOADim] = {}
```

### Comparing `zigzag_dse-3.1.1/zigzag/stages/AcceleratorParserStage.py` & `zigzag_dse-3.1.2/zigzag/stages/AcceleratorParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/CostModelStage.py` & `zigzag_dse-3.1.2/zigzag/stages/CostModelStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/DumpStage.py` & `zigzag_dse-3.1.2/zigzag/stages/DumpStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/GeneralParameterIteratorStage.py` & `zigzag_dse-3.1.2/zigzag/stages/GeneralParameterIteratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/LomaStage.py` & `zigzag_dse-3.1.2/zigzag/stages/LomaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/MainStage.py` & `zigzag_dse-3.1.2/zigzag/stages/MainStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/ONNXModelParserStage.py` & `zigzag_dse-3.1.2/zigzag/stages/ONNXModelParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/PEArrayScalingStage.py` & `zigzag_dse-3.1.2/zigzag/stages/PEArrayScalingStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/PlotTemporalMappingsStage.py` & `zigzag_dse-3.1.2/zigzag/stages/PlotTemporalMappingsStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/RemoveUnusedMemoryStage.py` & `zigzag_dse-3.1.2/zigzag/stages/RemoveUnusedMemoryStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/SalsaStage.py` & `zigzag_dse-3.1.2/zigzag/stages/SalsaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/SearchUnusedMemoryStage.py` & `zigzag_dse-3.1.2/zigzag/stages/SearchUnusedMemoryStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/SpatialMappingConversionStage.py` & `zigzag_dse-3.1.2/zigzag/stages/SpatialMappingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/SpatialMappingGeneratorStage.py` & `zigzag_dse-3.1.2/zigzag/stages/SpatialMappingGeneratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/Stage.py` & `zigzag_dse-3.1.2/zigzag/stages/Stage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/TemporalOrderingConversionStage.py` & `zigzag_dse-3.1.2/zigzag/stages/TemporalOrderingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/WorkloadParserStage.py` & `zigzag_dse-3.1.2/zigzag/stages/WorkloadParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/WorkloadStage.py` & `zigzag_dse-3.1.2/zigzag/stages/WorkloadStage.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/reduce_stages.py` & `zigzag_dse-3.1.2/zigzag/stages/reduce_stages.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/run_opt_stages.py` & `zigzag_dse-3.1.2/zigzag/stages/run_opt_stages.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/stages/save_stages.py` & `zigzag_dse-3.1.2/zigzag/stages/save_stages.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/utils.py` & `zigzag_dse-3.1.2/zigzag/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag_dse-3.1.2/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/visualization/graph/workload.py` & `zigzag_dse-3.1.2/zigzag/visualization/graph/workload.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/visualization/results/plot_cme.py` & `zigzag_dse-3.1.2/zigzag/visualization/results/plot_cme.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/visualization/results/print_mapping.py` & `zigzag_dse-3.1.2/zigzag/visualization/results/print_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/DNNWorkload.py` & `zigzag_dse-3.1.2/zigzag/workload/DNNWorkload.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/DummyNode.py` & `zigzag_dse-3.1.2/zigzag/workload/DummyNode.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/LayerAttribute.py` & `zigzag_dse-3.1.2/zigzag/workload/LayerAttribute.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/LayerNodeABC.py` & `zigzag_dse-3.1.2/zigzag/workload/LayerNodeABC.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/ONNXWorkload.py` & `zigzag_dse-3.1.2/zigzag/workload/ONNXWorkload.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/Workload.py` & `zigzag_dse-3.1.2/zigzag/workload/Workload.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/layer_attributes.py` & `zigzag_dse-3.1.2/zigzag/workload/layer_attributes.py`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.1/zigzag/workload/layer_node.py` & `zigzag_dse-3.1.2/zigzag/workload/layer_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     equation: LayerEquation
     layer_dim_sizes: LayerDimSizes
     operand_precision: LayerOperandPrecision
     dimension_relations: list[LayerDimRelation]
     spatial_mapping: SpatialMapping
     spatial_mapping_hint: SpatialMappingHint
     core_allocation: list[int]
+    core_allocation_is_fixed: bool
     memory_operand_links: MemoryOperandLinks
     temporal_ordering: LayerTemporalOrdering
     padding: LayerPadding
     constant_operands: list[LayerOperand]
     input_operand_source: InputOperandSource
     pr_layer_dim_sizes: LayerDimSizes | None
 
@@ -134,14 +135,15 @@
         self.equation = node_attr.equation
         self.layer_dim_sizes = node_attr.layer_dim_sizes
         self.operand_precision = node_attr.operand_precision
         self.dimension_relations = node_attr.dimension_relations
         self.spatial_mapping = node_attr.spatial_mapping
         self.spatial_mapping_hint = node_attr.spatial_mapping_hint
         self.core_allocation = node_attr.core_allocation
+        self.core_allocation_is_fixed = node_attr.core_allocation_is_fixed
         self.memory_operand_links = node_attr.memory_operand_links
         self.temporal_ordering = node_attr.temporal_ordering
         self.padding = node_attr.padding
         self.constant_operands = node_attr.constant_operands
         self.input_operand_source = node_attr.input_operand_source
         pr_layer_dim_sizes = node_attr.pr_layer_dim_sizes
 
@@ -185,14 +187,15 @@
         return json_repr_handler(
             {
                 "equation": self.equation,
                 "equation_relations": self.dimension_relations,
                 "loop_dimensions": self.layer_dim_sizes,
                 "operand_precision": self.operand_precision,
                 "core_allocation": self.core_allocation,
+                "core_allocation_is_fixed": self.core_allocation_is_fixed,
                 "user_spatial_mapping": self.spatial_mapping,
                 "memory_operand_links": self.memory_operand_links,
                 # "source_storage_level": self.source_storage_level, # NOTE not used?
             }
         )
 
     def calc_tensor_size(self, layer_op: LayerOperand, layer_dim_sizes: LayerDimSizes):
@@ -300,14 +303,15 @@
             equation=self.equation,
             layer_dim_sizes=self.layer_dim_sizes,
             operand_precision=self.operand_precision,
             dimension_relations=self.dimension_relations,
             spatial_mapping=self.spatial_mapping,
             spatial_mapping_hint=self.spatial_mapping_hint,
             core_allocation=self.core_allocation,
+            core_allocation_is_fixed=self.core_allocation_is_fixed,
             memory_operand_links=self.memory_operand_links,
             temporal_ordering=self.temporal_ordering,
             padding=self.padding,
             constant_operands=self.constant_operands,
             input_operand_source=self.input_operand_source,
             pr_layer_dim_sizes=self.pr_layer_dim_sizes,
         )
```

### Comparing `zigzag_dse-3.1.1/zigzag_dse.egg-info/PKG-INFO` & `zigzag_dse-3.1.2/zigzag_dse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 3.1.1
+Version: 3.1.2
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2021 MICAS (KU Leuven)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zigzag_dse-3.1.1/zigzag_dse.egg-info/SOURCES.txt` & `zigzag_dse-3.1.2/zigzag_dse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-lab1/main.py
-lab2/solutions/main.py
-lab3/main.py
 tests/main/test_imc/__init__.py
 tests/main/test_imc/test_aimc.py
 tests/main/test_imc/test_dimc.py
 tests/main/test_origin/test_ascend_like.py
 tests/main/test_origin/test_edge_tpu_like.py
 tests/main/test_origin/test_meta_prototype_like.py
 tests/main/test_origin/test_tesla_npu_like.py
```

