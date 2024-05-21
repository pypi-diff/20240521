# Comparing `tmp/codecarbon-2.4.1.tar.gz` & `tmp/codecarbon-2.4.2.tar.gz`

## Comparing `codecarbon-2.4.1.tar` & `codecarbon-2.4.2.tar`

### file list

```diff
@@ -1,60 +1,68 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/_version.py
--rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/emissions_tracker.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/input.py
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/cli/__init__.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/cli/cli_utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/__init__.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/api_client.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/cloud.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/co2_signal.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/config.py
--rw-r--r--   0        0        0    13483 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/cpu.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/emissions.py
--rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/gpu.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/measure.py
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/powermetrics.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/rapl.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/schemas.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/units.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/core/util.py
--rw-r--r--   0        0        0   409749 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/canada_provinces.geojson
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/cloud/impact.csv
--rw-r--r--   0        0        0    92710 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/hardware/cpu_power.csv
--rw-r--r--   0        0        0    49131 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2023-07-07-22-40-48.png
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0        0        0    49591 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb
--rw-r--r--   0        0        0   420635 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/world_energy_mix.csv
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0        0        0    48072 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2016/global_energy_mix-old.json
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0        0        0    42145 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb
--rw-r--r--   0        0        0    29597 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb
--rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/__init__.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/geography.py
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/hardware.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/logger.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/scheduler.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/external/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/prometheus/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/prometheus/metric_definitions.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/prometheus/prometheus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/__init__.py
--rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/carbonboard.py
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0        0        0    28035 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/components.py
--rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/__init__.py
--rw-r--r--   0        0        0    25442 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 codecarbon-2.4.1/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codecarbon-2.4.1/.gitignore
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 codecarbon-2.4.1/LICENSE
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 codecarbon-2.4.1/README.md
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 codecarbon-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 codecarbon-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/_version.py
+-rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/emissions_tracker.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/input.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/cli/__init__.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/cli/cli_utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/__init__.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/api_client.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/cloud.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/co2_signal.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/config.py
+-rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/cpu.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/emissions.py
+-rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/gpu.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/measure.py
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/powermetrics.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/rapl.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/schemas.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/units.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/core/util.py
+-rw-r--r--   0        0        0   409749 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/canada_provinces.geojson
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/cloud/impact.csv
+-rw-r--r--   0        0        0    92734 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/hardware/cpu_power.csv
+-rw-r--r--   0        0        0    49131 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2023-07-07-22-40-48.png
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0        0        0    49591 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb
+-rw-r--r--   0        0        0   420635 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/world_energy_mix.csv
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0        0        0    48072 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2016/global_energy_mix-old.json
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0        0        0    42145 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb
+-rw-r--r--   0        0        0    29597 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb
+-rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/external/__init__.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/external/geography.py
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/external/hardware.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/external/logger.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/external/scheduler.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/external/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/base_output.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/emissions_data.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/file.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/http.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/metrics/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/metrics/metric_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/metrics/prometheus/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/metrics/prometheus/metrics.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/output_methods/metrics/prometheus/prometheus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/__init__.py
+-rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/carbonboard.py
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0        0        0    28035 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/components.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0        0        0    25442 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 codecarbon-2.4.2/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codecarbon-2.4.2/.gitignore
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 codecarbon-2.4.2/LICENSE
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 codecarbon-2.4.2/README.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 codecarbon-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 codecarbon-2.4.2/PKG-INFO
```

### Comparing `codecarbon-2.4.1/codecarbon/emissions_tracker.py` & `codecarbon-2.4.2/codecarbon/emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/input.py` & `codecarbon-2.4.2/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/cli/cli_utils.py` & `codecarbon-2.4.2/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/cli/main.py` & `codecarbon-2.4.2/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/api_client.py` & `codecarbon-2.4.2/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/cloud.py` & `codecarbon-2.4.2/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/co2_signal.py` & `codecarbon-2.4.2/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/config.py` & `codecarbon-2.4.2/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/cpu.py` & `codecarbon-2.4.2/codecarbon/core/cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,18 @@
             scorer=fuzz.ratio,
             score_cutoff=THRESHOLD_DIRECT,
         )
 
         if direct_match:
             return direct_match[0]
 
+        model_raw = model_raw.replace("(R)", "")
+        start_cpu = model_raw.find(" CPU @ ")
+        if start_cpu > 0:
+            model_raw = model_raw[0:start_cpu]
         indirect_matches = process.extract(
             model_raw,
             cpu_df["Name"],
             processor=utils.default_process,
             scorer=fuzz.token_set_ratio,
             score_cutoff=THRESHOLD_TOKEN_SET,
         )
```

### Comparing `codecarbon-2.4.1/codecarbon/core/emissions.py` & `codecarbon-2.4.2/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/gpu.py` & `codecarbon-2.4.2/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/measure.py` & `codecarbon-2.4.2/codecarbon/core/measure.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/powermetrics.py` & `codecarbon-2.4.2/codecarbon/core/powermetrics.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/rapl.py` & `codecarbon-2.4.2/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/schemas.py` & `codecarbon-2.4.2/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/units.py` & `codecarbon-2.4.2/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/core/util.py` & `codecarbon-2.4.2/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/canada_provinces.geojson` & `codecarbon-2.4.2/codecarbon/data/canada_provinces.geojson`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/cloud/impact.csv` & `codecarbon-2.4.2/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.4.2/codecarbon/data/hardware/cpu_power.csv`

 * *Files 0% similar despite different names*

```diff
@@ -2383,14 +2383,15 @@
 Intel Core i7-6650U,15
 Intel Core i7-6660U,15
 Intel Core i7-6700,65
 Intel Core i7-6700HQ,45
 Intel Core i7-6700K,95
 Intel Core i7-6700T,35
 Intel Core i7-6700TE,35
+Intel Core i7-6700HQ,45
 Intel Core i7-6770HQ,45
 Intel Core i7-6785R,65
 Intel Core i7-6800K,140
 Intel Core i7-680UM,18
 Intel Core i7-6820EQ,45
 Intel Core i7-6820HK,45
 Intel Core i7-6820HQ,45
```

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2023-07-07-22-40-48.png` & `codecarbon-2.4.2/codecarbon/data/private_infra/2023-07-07-22-40-48.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.4.2/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.4.2/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb` & `codecarbon-2.4.2/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/world_energy_mix.csv` & `codecarbon-2.4.2/codecarbon/data/private_infra/world_energy_mix.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.4.2/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2016/global_energy_mix-old.json` & `codecarbon-2.4.2/codecarbon/data/private_infra/2016/global_energy_mix-old.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.4.2/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb` & `codecarbon-2.4.2/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb` & `codecarbon-2.4.2/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb` & `codecarbon-2.4.2/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv` & `codecarbon-2.4.2/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/external/geography.py` & `codecarbon-2.4.2/codecarbon/external/geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/external/hardware.py` & `codecarbon-2.4.2/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/external/logger.py` & `codecarbon-2.4.2/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/external/scheduler.py` & `codecarbon-2.4.2/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/external/task.py` & `codecarbon-2.4.2/codecarbon/external/task.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/prometheus/prometheus.py` & `codecarbon-2.4.2/codecarbon/output_methods/metrics/prometheus/prometheus.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,45 @@
+import dataclasses
 import os
 
 from prometheus_client import push_to_gateway
 from prometheus_client.exposition import basic_auth_handler
 
-from codecarbon.prometheus.metric_definitions import (
+from codecarbon.external.logger import logger
+from codecarbon.output_methods.base_output import BaseOutput
+from codecarbon.output_methods.emissions_data import EmissionsData
+from codecarbon.output_methods.metrics.prometheus.metrics import (
     cpu_energy_gauge,
     cpu_power_gauge,
     duration_gauge,
     emissions_gauge,
     emissions_rate_gauge,
     energy_consumed_gauge,
     gpu_energy_gauge,
     gpu_power_gauge,
     ram_energy_gauge,
     ram_power_gauge,
     registry,
 )
 
 
-class Prometheus:
-    def __init__(self, prometheus_url):
+class PrometheusOutput(BaseOutput):
+    """
+    Send emissions data to prometheus pushgateway
+    """
+
+    def __init__(self, prometheus_url: str):
         self.prometheus_url = prometheus_url
 
+    def out(self, data: EmissionsData):
+        try:
+            self.add_emission(dataclasses.asdict(data))
+        except Exception as e:
+            logger.error(e, exc_info=True)
+
     def _auth_handler(self, url, method, timeout, headers, data):
         username = os.getenv("PROMETHEUS_USERNAME")
         password = os.getenv("PROMETHEUS_PASSWORD")
         return basic_auth_handler(
             url, method, timeout, headers, data, username, password
         )
```

### Comparing `codecarbon-2.4.1/codecarbon/viz/carbonboard.py` & `codecarbon-2.4.2/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.4.2/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/viz/components.py` & `codecarbon-2.4.2/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/viz/data.py` & `codecarbon-2.4.2/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.4.2/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.4.2/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.4.2/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/.gitignore` & `codecarbon-2.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/LICENSE` & `codecarbon-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/README.md` & `codecarbon-2.4.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 - [Quickstart 🚀](#quickstart-)
     - [Installation 🔧](#installation-)
     - [Start to estimate your impact 📏](#start-to-estimate-your-impact-)
       - [Monitoring your whole machine](#monitoring-your-machine-)
       - [In your python code](#in-your-python-code-)
       - [Visualize](#visualize-)
 - [Contributing 🤝](#contributing-)
+- [How To Cite 📝](#how-to-cite-)
 - [Contact 📝](#contact-)
 
 # About CodeCarbon 💡
 
 **CodeCarbon** started with a quite simple question: 
 
 **What is the carbon emission impact of my computer program? :shrug:**
@@ -116,11 +117,57 @@
 
 In order to contribute a change to our code base, please submit a pull request (PR) via GitHub and someone from our team will go over it and accept it.
 
 Check out our [contribution guidelines :arrow_upper_right:](https://github.com/mlco2/codecarbon/blob/master/CONTRIBUTING.md)
 
 Contact [@vict0rsch](https://github.com/vict0rsch) to be added to our slack workspace if you want to contribute regularly!
 
+# How To Cite 📝
+
+If you find CodeCarbon useful for your research, you can find a citation under a variety of formats on [Zenodo](https://zenodo.org/records/11171501).
+
+Here is a sample for BibTeX: 
+```tex 
+@software{benoit_courty_2024_11171501,
+  author       = {Benoit Courty and
+                  Victor Schmidt and
+                  Sasha Luccioni and
+                  Goyal-Kamal and
+                  MarionCoutarel and
+                  Boris Feld and
+                  Jérémy Lecourt and
+                  LiamConnell and
+                  Amine Saboni and
+                  Inimaz and
+                  supatomic and
+                  Mathilde Léval and
+                  Luis Blanche and
+                  Alexis Cruveiller and
+                  ouminasara and
+                  Franklin Zhao and
+                  Aditya Joshi and
+                  Alexis Bogroff and
+                  Hugues de Lavoreille and
+                  Niko Laskaris and
+                  Edoardo Abati and
+                  Douglas Blank and
+                  Ziyao Wang and
+                  Armin Catovic and
+                  Marc Alencon and
+                  Michał Stęchły and
+                  Christian Bauer and
+                  Lucas-Otavio and
+                  JPW and
+                  MinervaBooks},
+  title        = {mlco2/codecarbon: v2.4.1},
+  month        = may,
+  year         = 2024,
+  publisher    = {Zenodo},
+  version      = {v2.4.1},
+  doi          = {10.5281/zenodo.11171501},
+  url          = {https://doi.org/10.5281/zenodo.11171501}
+}
+```
 
 # Contact 📝
 
 Maintainers are [@vict0rsch](https://github.com/vict0rsch) [@benoit-cty](https://github.com/benoit-cty) and [@SaboniAmine](https://github.com/saboniamine). Codecarbon is developed by volunteers from [**Mila**](http://mila.quebec) and the [**DataForGoodFR**](https://twitter.com/dataforgood_fr) community alongside donated professional time of engineers at [**Comet.ml**](https://comet.ml) and [**BCG GAMMA**](https://www.bcg.com/en-nl/beyond-consulting/bcg-gamma/default).
```

### Comparing `codecarbon-2.4.1/pyproject.toml` & `codecarbon-2.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codecarbon-2.4.1/PKG-INFO` & `codecarbon-2.4.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: codecarbon
-Version: 2.4.1
+Version: 2.4.2
 Project-URL: Homepage, https://codecarbon.io/
 Project-URL: Repository, https://github.com/mlco2/codecarbon
 Project-URL: Dashboard, http://dashboard.codecarbon.io/
 Project-URL: Documentation, https://mlco2.github.io/codecarbon/
 Project-URL: Issues, https://github.com/mlco2/codecarbon/issues
 Project-URL: Changelog, https://github.com/mlco2/codecarbon/releases
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
@@ -51,14 +51,15 @@
 - [Quickstart 🚀](#quickstart-)
     - [Installation 🔧](#installation-)
     - [Start to estimate your impact 📏](#start-to-estimate-your-impact-)
       - [Monitoring your whole machine](#monitoring-your-machine-)
       - [In your python code](#in-your-python-code-)
       - [Visualize](#visualize-)
 - [Contributing 🤝](#contributing-)
+- [How To Cite 📝](#how-to-cite-)
 - [Contact 📝](#contact-)
 
 # About CodeCarbon 💡
 
 **CodeCarbon** started with a quite simple question: 
 
 **What is the carbon emission impact of my computer program? :shrug:**
@@ -151,11 +152,57 @@
 
 In order to contribute a change to our code base, please submit a pull request (PR) via GitHub and someone from our team will go over it and accept it.
 
 Check out our [contribution guidelines :arrow_upper_right:](https://github.com/mlco2/codecarbon/blob/master/CONTRIBUTING.md)
 
 Contact [@vict0rsch](https://github.com/vict0rsch) to be added to our slack workspace if you want to contribute regularly!
 
+# How To Cite 📝
+
+If you find CodeCarbon useful for your research, you can find a citation under a variety of formats on [Zenodo](https://zenodo.org/records/11171501).
+
+Here is a sample for BibTeX: 
+```tex 
+@software{benoit_courty_2024_11171501,
+  author       = {Benoit Courty and
+                  Victor Schmidt and
+                  Sasha Luccioni and
+                  Goyal-Kamal and
+                  MarionCoutarel and
+                  Boris Feld and
+                  Jérémy Lecourt and
+                  LiamConnell and
+                  Amine Saboni and
+                  Inimaz and
+                  supatomic and
+                  Mathilde Léval and
+                  Luis Blanche and
+                  Alexis Cruveiller and
+                  ouminasara and
+                  Franklin Zhao and
+                  Aditya Joshi and
+                  Alexis Bogroff and
+                  Hugues de Lavoreille and
+                  Niko Laskaris and
+                  Edoardo Abati and
+                  Douglas Blank and
+                  Ziyao Wang and
+                  Armin Catovic and
+                  Marc Alencon and
+                  Michał Stęchły and
+                  Christian Bauer and
+                  Lucas-Otavio and
+                  JPW and
+                  MinervaBooks},
+  title        = {mlco2/codecarbon: v2.4.1},
+  month        = may,
+  year         = 2024,
+  publisher    = {Zenodo},
+  version      = {v2.4.1},
+  doi          = {10.5281/zenodo.11171501},
+  url          = {https://doi.org/10.5281/zenodo.11171501}
+}
+```
 
 # Contact 📝
 
 Maintainers are [@vict0rsch](https://github.com/vict0rsch) [@benoit-cty](https://github.com/benoit-cty) and [@SaboniAmine](https://github.com/saboniamine). Codecarbon is developed by volunteers from [**Mila**](http://mila.quebec) and the [**DataForGoodFR**](https://twitter.com/dataforgood_fr) community alongside donated professional time of engineers at [**Comet.ml**](https://comet.ml) and [**BCG GAMMA**](https://www.bcg.com/en-nl/beyond-consulting/bcg-gamma/default).
```

