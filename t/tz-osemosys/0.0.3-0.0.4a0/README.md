# Comparing `tmp/tz_osemosys-0.0.3.tar.gz` & `tmp/tz_osemosys-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tz_osemosys-0.0.3.tar", last modified: Fri May 10 11:19:12 2024, max compression
+gzip compressed data, was "tz_osemosys-0.0.4a0.tar", last modified: Tue May 21 10:06:32 2024, max compression
```

## Comparing `tz_osemosys-0.0.3.tar` & `tz_osemosys-0.0.4a0.tar`

### file list

```diff
@@ -1,133 +1,630 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.438459 tz_osemosys-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/bin/memory_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:19:12.438459 tz_osemosys-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/fixtures/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/fixtures/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/test_compatability/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_runspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_timedef.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/test_composition/
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_composition/test_compose_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_composition/test_compose_runspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tests/test_construction/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_load_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_runspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_timedefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_integration/test_linopy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tests/test_solve/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_solve/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_solve/test_to_xr_ds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.414459 tz_osemosys-0.0.3/tz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tz/osemosys/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tz/osemosys/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/io/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/io/simpleeval.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tz/osemosys/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.426459 tz_osemosys-0.0.3/tz/osemosys/model/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/accounting_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/annual_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/capital_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/new_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/operating_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/re_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/reserve_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/salvage_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    19117 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_discounted_costs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.426459 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/financials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/reserve_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.430459 tz_osemosys-0.0.3/tz/osemosys/model/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.430459 tz_osemosys-0.0.3/tz/osemosys/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/commodity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.430459 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/impact.py
--rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/time_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/impact.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/time_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/commodity_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/impact_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_presolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/region_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/storage_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/technology_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/timedefinition_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/validation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/tz/osemosys/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/utils/cfg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/tz_osemosys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.150021 tz_osemosys-0.0.4a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.042021 tz_osemosys-0.0.4a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.042021 tz_osemosys-0.0.4a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.042021 tz_osemosys-0.0.4a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/workflows/ci-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.github/workflows/test_pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-21 10:06:32.150021 tz_osemosys-0.0.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.042021 tz_osemosys-0.0.4a0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/bin/memory_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.046021 tz_osemosys-0.0.4a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/commodity.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/impact.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/operating_mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/region.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/storage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/technology.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/time_definition.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.046021 tz_osemosys-0.0.4a0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.046021 tz_osemosys-0.0.4a0/examples/CAISO-ERCOT-IC/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/CAISO-ERCOT-IC/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/CAISO-ERCOT-IC/technologies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.038021 tz_osemosys-0.0.4a0/examples/otoole_compat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.046021 tz_osemosys-0.0.4a0/examples/otoole_compat/config_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/config_files/otoole-full-electricity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/config_files/otoole-simple-hydro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.038021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.058021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30527 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.070021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    55323 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53273 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   122456 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    51815 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   127042 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   203338 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19511 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    82323 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-complete/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.082021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   117964 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.094021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.106021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    71503 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.118021 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/input_csv/otoole-simple-hydro/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.038021 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.126021 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/AccumulatedNewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualEmissions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualFixedOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmissionByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualVariableOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/CapitalInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/Demand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedSalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedTechnologyEmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/NewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   209150 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26252 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnologyAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   172779 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   205093 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   213389 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   113730 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   118340 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/SalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21669 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/TotalAnnualTechnologyActivityByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20347 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/TotalCapacityAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/TotalDiscountedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyAnnualActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   115801 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-full-electricity/UseByTechnology.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/AccumulatedNewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualEmissions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualFixedOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualTechnologyEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualTechnologyEmissionByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualVariableOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/CapitalInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/Demand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedSalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedTechnologyEmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/NewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    48446 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnologyAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42760 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    48459 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    50925 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33426 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/SalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalAnnualTechnologyActivityByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalCapacityAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalDiscountedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyAnnualActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31767 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/otoole_compat/results_csv/otoole-simple-hydro/UseByTechnology.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/examples/quickstart/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/quickstart/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/examples/utopia/
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/examples/utopia/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:06:32.150021 tz_osemosys-0.0.4a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/fixtures/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/fixtures/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/tests/test_compatability/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_runspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_timedef.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.130021 tz_osemosys-0.0.4a0/tests/test_composition/
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_composition/test_compose_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_composition/test_compose_runspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.134021 tz_osemosys-0.0.4a0/tests/test_construction/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_load_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_runspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_construction/test_timedefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.134021 tz_osemosys-0.0.4a0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_integration/test_linopy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.134021 tz_osemosys-0.0.4a0/tests/test_solve/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_solve/test_salvage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_solve/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tests/test_solve/test_to_xr_ds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.038021 tz_osemosys-0.0.4a0/tz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.134021 tz_osemosys-0.0.4a0/tz/osemosys/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.134021 tz_osemosys-0.0.4a0/tz/osemosys/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/io/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/io/simpleeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.138021 tz_osemosys-0.0.4a0/tz/osemosys/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.138021 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_accounting_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_capital_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_operating_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_salvage_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_total_discounted_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/annual_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/capacity_adequacy_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/capacity_adequacy_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/energy_balance_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/energy_balance_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/new_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/re_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/reserve_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/total_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/total_capacity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.142022 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/discounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/financials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/reserve_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.142022 tz_osemosys-0.0.4a0/tz/osemosys/model/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/variables/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/variables/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/model/variables/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.142022 tz_osemosys-0.0.4a0/tz/osemosys/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/commodity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.146021 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/time_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15398 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/time_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.146021 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/commodity_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/impact_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/model_presolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/region_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/storage_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/technology_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12528 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/timedefinition_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.146021 tz_osemosys-0.0.4a0/tz/osemosys/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/utils/cfg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-21 10:06:28.000000 tz_osemosys-0.0.4a0/tz/osemosys/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:06:32.150021 tz_osemosys-0.0.4a0/tz_osemosys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-21 10:06:31.000000 tz_osemosys-0.0.4a0/tz_osemosys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43183 2024-05-21 10:06:32.000000 tz_osemosys-0.0.4a0/tz_osemosys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:06:31.000000 tz_osemosys-0.0.4a0/tz_osemosys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 10:06:31.000000 tz_osemosys-0.0.4a0/tz_osemosys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 10:06:31.000000 tz_osemosys-0.0.4a0/tz_osemosys.egg-info/top_level.txt
```

### Comparing `tz_osemosys-0.0.3/LICENSE` & `tz_osemosys-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/PKG-INFO` & `tz_osemosys-0.0.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tz-osemosys
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero
 Author-email: Lucas Kruitwagen <lucas.kruitwagen@gmail.com>, Ed Gill <edwardxtg@gmail.com>, Abhishek Shivakumar <abhishek0208@gmail.com>
 Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org
 Project-URL: Source, https://github.com/transitionzero/tz-osemosys
 Keywords: energy,milp,climate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.3 Summary: An OSeMOSYS
+Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.4a0 Summary: An OSeMOSYS
 implementation for the Future Energy Outlook by TransitionZero Author-email:
 Lucas Kruitwagen
 gmail.com>, Ed Gill
 gmail.com>, Abhishek Shivakumar
 gmail.com> Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org Project-URL: Source, https://
```

### Comparing `tz_osemosys-0.0.3/README.md` & `tz_osemosys-0.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/bin/memory_profile.py` & `tz_osemosys-0.0.4a0/bin/memory_profile.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/pyproject.toml` & `tz_osemosys-0.0.4a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [project]
 name = "tz-osemosys"  # Required
-version = "0.0.3"  # Required
+dynamic = ["version"]
 description = "An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.11"
 license = {file = "LICENSE.txt"}
 keywords = ["energy", "milp", "climate"]  # Optional
 authors = [
   {name = "Lucas Kruitwagen", email = "lucas.kruitwagen@gmail.com" },
   {name = "Ed Gill", email = "edwardxtg@gmail.com" },
   {name = "Abhishek Shivakumar", email = "abhishek0208@gmail.com" },
 ]
 
-#maintainers = [
-#  {name = "A. Great Maintainer", email = "maintainer@example.com" } # Optional
-#]
 
-# For a list of valid classifiers, see https://pypi.org/classifiers/
 classifiers = [  # Optional
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
@@ -35,14 +31,22 @@
   "pydantic-settings",
   "xarray",
   "orjson",
   "linopy",
 
 ]
 
+
+#maintainers = [
+#  {name = "A. Great Maintainer", email = "maintainer@example.com" } # Optional
+#]
+
+# For a list of valid classifiers, see https://pypi.org/classifiers/
+
+
 [project.optional-dependencies] # Optional
 dev = [
   "pre-commit",
   "black",
   "pytest",
   "pytest-order",
   "pytest-cov",
@@ -75,9 +79,10 @@
 
 [tool.setuptools.packages]
 find = {}
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
-requires = ["setuptools>=43.0.0", "wheel"]
+requires = ["setuptools>=43.0.0","setuptools_scm>=8", "wheel"]
 build-backend = "setuptools.build_meta"
+[tool.setuptools_scm]
```

### Comparing `tz_osemosys-0.0.3/tests/fixtures/misc.py` & `tz_osemosys-0.0.4a0/tests/fixtures/misc.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_commodity.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_commodity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_impact.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_region.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_roundtrip.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_roundtrip.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_runspec.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_runspec.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_storage.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_technology.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_technology.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_timedef.py` & `tz_osemosys-0.0.4a0/tests/test_compatability/test_otoole_timedef.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_composition/test_compose_base.py` & `tz_osemosys-0.0.4a0/tests/test_composition/test_compose_base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_composition/test_compose_runspec.py` & `tz_osemosys-0.0.4a0/tests/test_composition/test_compose_runspec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import json
+from tempfile import NamedTemporaryFile
+
+from tz.osemosys import Model
 from tz.osemosys.schemas.model import RunSpec
 from tz.osemosys.utils import recursive_keys
 
 PASSING_RUNSPEC_DEFINITIONS = dict(
     most_basic=dict(
         time_definition=dict(
             id="yearpart-daypart",
@@ -101,7 +105,17 @@
         input_activity_ratio = [k for k in recursive_keys(op_mode_1.input_activity_ratio.data)]
         for region in spec.regions:
             assert region.id in [k[0] for k in input_activity_ratio]
         for commodity in spec.commodities:
             assert commodity.id in [k[1] for k in input_activity_ratio]
         for year in spec.time_definition.years:
             assert str(year) in [k[2] for k in input_activity_ratio]
+
+
+def test_model_roundtrip():
+    tmp = NamedTemporaryFile()
+    for name, params in PASSING_RUNSPEC_DEFINITIONS.items():
+        model = Model(id=name, **params)
+        json.dump(model.model_dump(), open(tmp.name, "w"))
+        model_recovered = Model(**json.load(open(tmp.name)))
+
+        assert model == model_recovered
```

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_base.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_commodity.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_commodity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_data.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_data.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_impact.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_load_from_yaml.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_load_from_yaml.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_model.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_region.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_runspec.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_runspec.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_storage.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tests/test_construction/test_technology.py` & `tz_osemosys-0.0.4a0/tests/test_construction/test_technology.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+from tempfile import NamedTemporaryFile
+
 import pytest
 
 from tz.osemosys.schemas.technology import Technology
 
 PASSING_TECH_DEFINITIONS = dict(
     most_basic=dict(
         id="most_basic",
@@ -69,7 +72,16 @@
 
 
 @pytest.mark.skip(reason="Should only be tested for greater than / less than after composition")
 def test_tech_construction_failcases():
     for _name, params in FAILING_TECH_DEFINITIONS.items():
         with pytest.raises(ValueError) as e:  # noqa: F841
             Technology(**params)
+
+
+def test_technology_roundtrip():
+    tmp = NamedTemporaryFile()
+    for _name, params in PASSING_TECH_DEFINITIONS.items():
+        tech = Technology(**params)
+        json.dump(tech.model_dump(), open(tmp.name, "w"))
+        tech_recovered = Technology(**json.load(open(tmp.name)))
+        assert tech == tech_recovered
```

### Comparing `tz_osemosys-0.0.3/tests/test_integration/test_linopy_model.py` & `tz_osemosys-0.0.4a0/tests/test_integration/test_linopy_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,11 +25,11 @@
             model = Model.from_otoole_csv(sample_path)
 
             model.solve()
 
             ref_results_df = pd.read_csv(Path(results_path) / "TotalDiscountedCost.csv")
 
         assert np.isclose(
-            model._m.solution.TotalDiscountedCost.sum().values,
+            model.objective,
             ref_results_df["VALUE"].sum(),
             rtol=TOL,
         )
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/__init__.py` & `tz_osemosys-0.0.4a0/tz/osemosys/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from tz.osemosys.io.load_model import load_model
 from tz.osemosys.model.model import Model
 from tz.osemosys.schemas.commodity import Commodity
 from tz.osemosys.schemas.impact import Impact
 from tz.osemosys.schemas.region import Region
+from tz.osemosys.schemas.storage import Storage
 from tz.osemosys.schemas.technology import OperatingMode, Technology
 from tz.osemosys.schemas.time_definition import TimeDefinition
 
 __all__ = [
     "Model",
     "Commodity",
     "Technology",
+    "Storage",
     "Impact",
     "Region",
     "TimeDefinition",
     "OperatingMode",
     "load_model",
 ]
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/defaults.py` & `tz_osemosys-0.0.4a0/tz/osemosys/defaults.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/io/load_model.py` & `tz_osemosys-0.0.4a0/tz/osemosys/io/load_model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/io/simpleeval.py` & `tz_osemosys-0.0.4a0/tz/osemosys/io/simpleeval.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/__init__.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from typing import Dict
 
 import xarray as xr
 from linopy import LinearExpression, Model
 
-from .accounting_technology import add_accounting_technology_constraints
 from .annual_activity import add_annual_activity_constraints
 from .capacity_adequacy_a import add_capacity_adequacy_a_constraints
 from .capacity_adequacy_b import add_capacity_adequacy_b_constraints
-from .capital_costs import add_capital_costs_constraints
 from .emissions import add_emissions_constraints
 from .energy_balance_a import add_energy_balance_a_constraints
 from .energy_balance_b import add_energy_balance_b_constraints
 from .new_capacity import add_new_capacity_constraints
-from .operating_costs import add_operating_costs_constraints
 from .re_targets import add_re_targets_constraints
 from .reserve_margin import add_reserve_margin_constraints
-from .salvage_value import add_salvage_value_constraints
 from .storage import add_storage_constraints
 from .total_activity import add_total_activity_constraints
 from .total_capacity import add_total_capacity_constraints
-from .total_discounted_costs import add_total_discounted_costs_constraints
 
 
 def add_constraints(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]) -> Model:
     """Add all constraints to the model
 
     Arguments
     ---------
@@ -38,22 +33,17 @@
     """
 
     # restore one at a time
     m = add_capacity_adequacy_a_constraints(ds, m, lex)
     m = add_capacity_adequacy_b_constraints(ds, m, lex)
     m = add_energy_balance_a_constraints(ds, m, lex)
     m = add_energy_balance_b_constraints(ds, m, lex)
-    m = add_capital_costs_constraints(ds, m, lex)
     m = add_emissions_constraints(ds, m, lex)
     m = add_annual_activity_constraints(ds, m, lex)
-    m = add_accounting_technology_constraints(ds, m, lex)
     m = add_new_capacity_constraints(ds, m, lex)
-    m = add_operating_costs_constraints(ds, m, lex)
     m = add_re_targets_constraints(ds, m, lex)
     m = add_reserve_margin_constraints(ds, m, lex)
-    m = add_salvage_value_constraints(ds, m, lex)
     m = add_storage_constraints(ds, m, lex)
     m = add_total_activity_constraints(ds, m, lex)
     m = add_total_capacity_constraints(ds, m, lex)
-    m = add_total_discounted_costs_constraints(ds, m, lex)
 
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/accounting_technology.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_accounting_technology.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/annual_activity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/annual_activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_a.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/capacity_adequacy_a.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,31 +53,30 @@
         r in REGION, t in TECHNOLOGY, y in YEAR: CapacityOfOneTechnologyUnit[r,t,y]<>0}:
         CapacityOfOneTechnologyUnit[r,t,y] * NumberOfNewTechnologyUnits[r,t,y]
         =
         NewCapacity[r,t,y];
     ```
     """
 
-    mask = (ds.YEAR - lex["NewCapacity"].data.BUILDYEAR >= 0) & (
-        ds.YEAR - lex["NewCapacity"].data.BUILDYEAR < ds.OperationalLife
-    )
-    con = m["AccumulatedNewCapacity"] - lex["NewCapacity"].where(mask).sum("BUILDYEAR") == 0
-    m.add_constraints(con, name="CAa1_TotalNewCapacity")
-
-    con = m["TotalCapacityAnnual"] - m["AccumulatedNewCapacity"] == ds["ResidualCapacity"].fillna(0)
-    m.add_constraints(con, name="CAa2_TotalAnnualCapacity")
-
+    # gross capacity sufficiency
     con = (
         lex["RateOfTotalActivity"]
-        - (m["TotalCapacityAnnual"] * ds["CapacityFactor"] * ds["CapacityToActivityUnit"])
+        - (
+            lex["GrossCapacity"].assign_coords(
+                {"TIMESLICE": ds["CapacityFactor"].coords["TIMESLICE"]}
+            )
+            * ds["CapacityFactor"]
+            * ds["CapacityToActivityUnit"]
+        )
         <= 0
     )
     mask = ~ds["CapacityFactor"].isnull()
     m.add_constraints(con, name="CAa4_Constraint_Capacity", mask=mask)
 
+    # unit-of-one-technology
     con = (
         ds["CapacityOfOneTechnologyUnit"] * m["NumberOfNewTechnologyUnits"] - m["NewCapacity"] == 0
     )
     mask = ds["CapacityOfOneTechnologyUnit"].notnull()
     m.add_constraints(con, name="CAa5_TotalNewCapacity", mask=mask)
 
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_b.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/capacity_adequacy_b.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,20 @@
         sum{l in TIMESLICE} (TotalCapacityAnnual[r,t,y] * CapacityFactor[r,t,l,y] *
         YearSplit[l,y]) * AvailabilityFactor[r,t,y] * CapacityToActivityUnit[r,t];
     ```
     """
 
     mask = ds["AvailabilityFactor"] < 1
     con = (lex["RateOfTotalActivity"] * ds["YearSplit"]).sum(dims="TIMESLICE") - (
-        (m["TotalCapacityAnnual"] * ds["CapacityFactor"] * ds["YearSplit"]).sum(dims="TIMESLICE")
+        (
+            lex["GrossCapacity"].assign_coords(
+                {"TIMESLICE": ds["CapacityFactor"].coords["TIMESLICE"]}
+            )
+            * ds["CapacityFactor"]
+            * ds["YearSplit"]
+        ).sum(dims="TIMESLICE")
         * ds["AvailabilityFactor"]
         * ds["CapacityToActivityUnit"]
     ) <= 0
     m.add_constraints(con, name="CAb1_PlannedMaintenance", mask=mask)
 
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/capital_costs.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_capital_costs.py`

 * *Files 22% similar despite different names*

```diff
@@ -42,10 +42,11 @@
 
     s.t. CC2_DiscountingCapitalInvestment{
         r in REGION, t in TECHNOLOGY, y in YEAR}:
         CapitalInvestment[r,t,y]  / DiscountFactor[r,y] = DiscountedCapitalInvestment[r,t,y];
     ```
     """
 
-    con = (lex["CapitalInvestment"] / lex["DiscountFactor"]) - m["DiscountedCapitalInvestment"] == 0
-    m.add_constraints(con, name="CC2_DiscountingCapitalInvestment")
+    # NOTE: These constraints have all been replaced by linear expressions in other constraints
+    #       This file remains just for reference
+
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/emissions.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/emissions.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,21 +84,14 @@
         <=
         ModelPeriodEmissionLimit[r,e];
         ```
     """
 
     if ds["EMISSION"].size > 0:
 
-        con = (
-            lex["AnnualTechnologyEmissionsPenalty"] / lex["DiscountFactorMid"]
-            - m["DiscountedTechnologyEmissionsPenalty"]
-            == 0
-        )
-        m.add_constraints(con, name="E5_DiscountedEmissionsPenaltyByTechnology")
-
         con = lex["AnnualEmissions"].fillna(0) <= ds["AnnualEmissionLimit"] - ds[
             "AnnualExogenousEmission"
         ].fillna(0)
         mask = (ds["AnnualEmissionLimit"] != -1) & (ds["AnnualEmissionLimit"].notnull())
 
         m.add_constraints(con, name="E8_AnnualEmissionsLimit", mask=mask)
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_a.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/energy_balance_a.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_b.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/energy_balance_b.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/new_capacity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/new_capacity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/operating_costs.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/_operating_costs.py`

 * *Files 21% similar despite different names*

```diff
@@ -51,10 +51,11 @@
         r in REGION, t in TECHNOLOGY, y in YEAR}:
         OperatingCost[r,t,y] / DiscountFactorMid[r, y]
         =
         DiscountedOperatingCost[r,t,y];
     ```
     """
 
-    con = (lex["OperatingCost"] / lex["DiscountFactorMid"]) - m["DiscountedOperatingCost"] == 0
-    m.add_constraints(con, name="OC4_DiscountedOperatingCostsTotalAnnual")
+    # NOTE: These constraints have all been replaced by linear expressions in other constraints
+    #       This file remains just for reference
+
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/re_targets.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/re_targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,10 @@
     s.t. RE5_FuelUseByTechnologyAnnual{
         r in REGION, t in TECHNOLOGY, f in FUEL, y in YEAR}:
         sum{l in TIMESLICE} RateOfUseByTechnology[r,l,t,f,y] * YearSplit[l,y] =
         UseByTechnologyAnnual[r,t,f,y];
     ```
     """
 
+    # TODO
+
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/reserve_margin.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/reserve_margin.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/storage.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/storage.py`

 * *Files 25% similar despite different names*

```diff
@@ -251,204 +251,31 @@
         DiscountedCapitalInvestmentStorage[r,s,y]
         - DiscountedSalvageValueStorage[r,s,y]
         = TotalDiscountedStorageCost[r,s,y];
     ```
     """
     if ds["STORAGE"].size > 0:
 
-        m.add_constraints(
-            m["StorageLevelYearStart"] == lex["StorageLevelYearStart"],
-            name="S5_and_S6_StorageLevelYearStart",
-        )
-        m.add_constraints(
-            m["StorageLevelYearFinish"] == lex["StorageLevelYearFinish"],
-            name="S7_and_S8_StorageLevelYearFinish",
-        )
-        m.add_constraints(
-            m["StorageLevelSeasonStart"] == lex["StorageLevelSeasonStart"],
-            name="S9_and_S10_StorageLevelSeasonStart",
-        )
-        m.add_constraints(
-            m["StorageLevelDayTypeStart"] == lex["StorageLevelDayTypeStart"],
-            name="S11_and_S12_StorageLevelDayTypeStart",
-        )
-        m.add_constraints(
-            m["StorageLevelDayTypeFinish"] == lex["StorageLevelDayTypeFinish"],
-            name="S13_and_S14_and_S15_StorageLevelDayTypeFinish",
-        )
-
-        # STORAGE INVESTMENTS
-
-        discount_factor_storage = (1 + ds["DiscountRate"]) ** (
-            ds.coords["YEAR"] - ds.coords["YEAR"][0]
-        )
-
-        new_storage_cap = m["NewStorageCapacity"].rename(YEAR="BUILDYEAR")
-        mask = (ds.YEAR - new_storage_cap.data.BUILDYEAR >= 0) & (
-            ds.YEAR - new_storage_cap.data.BUILDYEAR < ds.OperationalLifeStorage
-        )
-        con = m["AccumulatedNewStorageCapacity"] - new_storage_cap.where(mask).sum("BUILDYEAR") == 0
-        m.add_constraints(con, name="SI3_TotalNewStorage")
-
-        discount_factor_storage = (1 + ds["DiscountRate"]) ** (
-            ds.coords["YEAR"] - ds.coords["YEAR"][0]
-        )
-        CapitalInvestmentStorage = ds["CapitalCostStorage"] * m["NewStorageCapacity"]
-        con = (CapitalInvestmentStorage / discount_factor_storage) - m[
-            "DiscountedCapitalInvestmentStorage"
-        ] == 0
-        m.add_constraints(con, name="SI5_DiscountingCapitalInvestmentStorage")
-
-        def numerator_sv1(y: int):
-            return (1 + ds["DiscountRateStorage"]) ** (ds.coords["YEAR"][-1] - y + 1) - 1
-
-        def denominator_sv1():
-            return (1 + ds["DiscountRateStorage"]) ** ds["OperationalLifeStorage"] - 1
-
-        def salvage_cost_sv1(ds):
-            return ds["CapitalCostStorage"].fillna(0) * (
-                1 - (numerator_sv1(ds.coords["YEAR"]) / denominator_sv1())
-            )
-
-        con = m["SalvageValueStorage"] - (m["NewStorageCapacity"] * salvage_cost_sv1(ds)) == 0
-        mask = (
-            (ds["DepreciationMethod"] == 1)
-            & ((ds.coords["YEAR"] + ds["OperationalLifeStorage"] - 1) > ds.coords["YEAR"][-1])
-            & (ds["DiscountRateStorage"] > 0)
-        )
-        m.add_constraints(con, name="SI6_SalvageValueStorageAtEndOfPeriod1", mask=mask)
-
-        def numerator_sv2(y: int):
-            return ds.coords["YEAR"][-1] - y + 1
-
-        def denominator_sv2():
-            return ds["OperationalLifeStorage"]
-
-        def salvage_cost_sv2(ds):
-            return ds["CapitalCostStorage"].fillna(0) * (
-                1 - (numerator_sv2(ds.coords["YEAR"]) / denominator_sv2())
-            )
-
-        con = m["SalvageValueStorage"] - (m["NewStorageCapacity"] * salvage_cost_sv2(ds)) == 0
-        mask = (
-            (ds["DepreciationMethod"] == 1)
-            & ((ds.coords["YEAR"] + ds["OperationalLifeStorage"] - 1) > ds.coords["YEAR"][-1])
-            & (ds["DiscountRateStorage"] == 0)
-        ) | (
-            (ds["DepreciationMethod"] == 2)
-            & ((ds.coords["YEAR"] + ds["OperationalLifeStorage"] - 1) > ds.coords["YEAR"][-1])
-        )
-        m.add_constraints(con, name="SI7_SalvageValueStorageAtEndOfPeriod2", mask=mask)
-
-        con = m["SalvageValueStorage"] == 0
-        mask = (ds.coords["YEAR"] + ds["OperationalLifeStorage"] - 1) <= ds.coords["YEAR"][-1]
-        m.add_constraints(con, name="SI8_SalvageValueStorageAtEndOfPeriod3", mask=mask)
-
-        def discounting(ds):
-            return (1 + ds["DiscountRateStorage"]) ** (
-                1 + ds.coords["YEAR"][-1] - ds.coords["YEAR"][0]
-            )
-
-        con = m["DiscountedSalvageValueStorage"] - m["SalvageValueStorage"] / discounting(ds) == 0
-        m.add_constraints(con, name="SI9_SalvageValueStorageDiscountedToStartYear")
-
-        con = (
-            m["DiscountedCapitalInvestmentStorage"] - m["DiscountedSalvageValueStorage"]
-            == m["TotalDiscountedStorageCost"]
-        )
-        m.add_constraints(con, name="SI10_TotalDiscountedCostByStorage")
-
-        # CAPACITY CONSTRAINTS
-
-        con = (
-            lex["StorageLevelDayTypeStart"]
-            + lex["NetChargeWithinDay"].shift(DAILYTIMEBRACKET=1).cumsum("DAILYTIMEBRACKET")
-            - lex["StorageLowerLimit"]
-            >= 0
-        )
-        m.add_constraints(con, name="SC1_LowerLimit_BeginningOfFirstWeek")
-
-        con = (
-            lex["StorageLevelDayTypeStart"]
-            + lex["NetChargeWithinDay"].shift(DAILYTIMEBRACKET=1).cumsum("DAILYTIMEBRACKET")
-            - lex["StorageUpperLimit"]
-            <= 0
-        )
-        m.add_constraints(con, name="SC1_UpperLimit_BeginningOfFirstWeek")
-
-        con = (
-            lex["StorageLevelDayTypeStart"]
-            # sum minus cumsum gives the sum of DAILYTIMEBRACKET for all future timebrackets
-            - (
-                lex["NetChargeWithinDay"].shift(DAYTYPE=1).sum("DAILYTIMEBRACKET")
-                - lex["NetChargeWithinDay"].shift(DAYTYPE=1).cumsum("DAILYTIMEBRACKET")
-            )
-            - lex["StorageLowerLimit"]
-            >= 0
-        )
-        mask = ds["DAYTYPE"] != ds["DAYTYPE"][0]
-        m.add_constraints(con, name="SC2_LowerLimit_EndOfFirstWeek", mask=mask)
-
-        con = (
-            lex["StorageLevelDayTypeStart"]
-            # sum minus cumsum gives the sum of DAILYTIMEBRACKET for all future timebrackets
-            - (
-                lex["NetChargeWithinDay"].shift(DAYTYPE=1).sum("DAILYTIMEBRACKET")
-                - lex["NetChargeWithinDay"].shift(DAYTYPE=1).cumsum("DAILYTIMEBRACKET")
-            )
-            - lex["StorageUpperLimit"]
-            <= 0
-        )
-        mask = ds["DAYTYPE"] != ds["DAYTYPE"][0]
-        m.add_constraints(con, name="SC2_UpperLimit_EndOfFirstWeek", mask=mask)
-
-        con = (
-            lex["StorageLevelDayTypeFinish"]
-            # sum minus cumsum gives the sum of DAILYTIMEBRACKET for all future timebrackets
-            - (
-                lex["NetChargeWithinDay"].sum("DAILYTIMEBRACKET")
-                - lex["NetChargeWithinDay"].cumsum("DAILYTIMEBRACKET")
-            )
-            - lex["StorageLowerLimit"]
-            >= 0
-        )
-        m.add_constraints(con, name="SC3_LowerLimit_EndOfLastWeek")
-
-        con = (
-            lex["StorageLevelDayTypeFinish"]
-            # sum minus cumsum gives the sum of DAILYTIMEBRACKET for all future timebrackets
-            - (
-                lex["NetChargeWithinDay"].sum("DAILYTIMEBRACKET")
-                - lex["NetChargeWithinDay"].cumsum("DAILYTIMEBRACKET")
-            )
-            - lex["StorageUpperLimit"]
-            <= 0
-        )
-        m.add_constraints(con, name="SC3_UpperLimit_EndOfLastWeek")
-
-        con = (
-            lex["StorageLevelDayTypeFinish"].shift(DAYTYPE=1)
-            + lex["NetChargeWithinDay"].shift(DAILYTIMEBRACKET=1).cumsum("DAILYTIMEBRACKET")
-            - lex["StorageLowerLimit"]
-            >= 0
-        )
-        mask = ds["DAYTYPE"] != ds["DAYTYPE"][0]
-        m.add_constraints(con, name="SC4_LowerLimit_BeginningOfLastWeek", mask=mask)
-
-        con = (
-            lex["StorageLevelDayTypeFinish"].shift(DAYTYPE=1)
-            + lex["NetChargeWithinDay"].shift(DAILYTIMEBRACKET=1).cumsum("DAILYTIMEBRACKET")
-            - lex["StorageUpperLimit"]
-            <= 0
-        )
-        mask = ds["DAYTYPE"] != ds["DAYTYPE"][0]
-        m.add_constraints(con, name="SC4_UpperLimit_BeginningOfLastWeek", mask=mask)
+        # storage level may not exceed gross capacity
+        con = lex["StorageLevel"] <= lex["GrossStorageCapacity"].expand_dims(
+            {"TIMESLICE": ds["TIMESLICE"]}
+        ).stack(YRTS=["YEAR", "TIMESLICE"])
+        m.add_constraints(con, name="StorageGrossCapacitySufficiency")
+
+        # storage level may not be less than minimum charge
+        if "MinStorageCharge" in ds.data_vars:
+            con = lex["StorageLevel"].fillna(0) >= ds["MinStorageCharge"].expand_dims(
+                {"TIMESLICE": ds["TIMESLICE"]}
+            ).stack(YRTS=["YEAR", "TIMESLICE"])
+            m.add_constraints(con, name="StorageMinimumCharge")
 
+        # storage charge rate may not exceed max charge rate
         if "StorageMaxChargeRate" in ds.data_vars:
             con = lex["RateOfStorageCharge"] <= ds["StorageMaxChargeRate"]
             m.add_constraints(con, name="SC5_MaxChargeConstraint")
 
+        # # storage discharge rate may not exceed max discharge rate
         if "StorageMaxDischargeRate" in ds.data_vars:
             con = lex["RateOfStorageDischarge"] <= ds["StorageMaxDischargeRate"]
             m.add_constraints(con, name="SC6_MaxDischargeConstraint")
 
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_activity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/total_activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_capacity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/constraints/total_capacity.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     s.t. TCC2_TotalAnnualMinCapacityConstraint{
         r in REGION, t in TECHNOLOGY, y in YEAR:
         TotalAnnualMinCapacity[r,t,y]>0}:
         TotalCapacityAnnual[r,t,y] >= TotalAnnualMinCapacity[r,t,y];
     ```
     """
 
-    con = m["TotalCapacityAnnual"] <= ds["TotalAnnualMaxCapacity"]
+    con = lex["GrossCapacity"] <= ds["TotalAnnualMaxCapacity"]
     mask = ds["TotalAnnualMaxCapacity"] >= 0
     m.add_constraints(con, name="TCC1_TotalAnnualMaxCapacityConstraint", mask=mask)
 
-    con = m["TotalCapacityAnnual"] >= ds["TotalAnnualMinCapacity"]
+    con = lex["GrossCapacity"] >= ds["TotalAnnualMinCapacity"]
     mask = ds["TotalAnnualMinCapacity"] > 0
     m.add_constraints(con, name="TCC2_TotalAnnualMinCapacityConstraint", mask=mask)
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_discounted_costs.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/financials.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,89 @@
 from typing import Dict
 
 import xarray as xr
 from linopy import LinearExpression, Model
 
 
-def add_total_discounted_costs_constraints(
-    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
-) -> Model:
-    """Add Total Discounted Costs constraints to the model.
-    Calculates the total discounted costs of the entire system across the entire model period.
-
-    Arguments
-    ---------
-    ds: xarray.Dataset
-        The parameters dataset
-    m: linopy.Model
-        A linopy model
-    lex: Dict[str, LinearExpression]
-
-
-    Returns
-    -------
-    linopy.Model
-
-
-    Notes
-    -----
-    ```ampl
-    s.t. TDC1_TotalDiscountedCostByTechnology{
-        r in REGION, t in TECHNOLOGY, y in YEAR}:
-        DiscountedOperatingCost[r,t,y] +
-        DiscountedCapitalInvestment[r,t,y]
-        + DiscountedTechnologyEmissionsPenalty[r,t,y] -
-        DiscountedSalvageValue[r,t,y] = TotalDiscountedCostByTechnology[r,t,y];
-
-    s.t. TDC2_TotalDiscountedCost{
-        r in REGION, y in YEAR}:
-        sum{t in TECHNOLOGY} TotalDiscountedCostByTechnology[r,t,y] +
-        sum{s in STORAGE} TotalDiscountedStorageCost[r,s,y]
-        = TotalDiscountedCost[r,y];
-    ```
-    """
-    con = (
-        m["DiscountedOperatingCost"]
-        + m["DiscountedCapitalInvestment"]
-        + m["DiscountedTechnologyEmissionsPenalty"]
-        - m["DiscountedSalvageValue"]
-        - m["TotalDiscountedCostByTechnology"]
-        == 0
+def add_lex_financials(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]):
+
+    CapitalInvestment = (
+        ds["CapitalCost"].fillna(0)
+        * m["NewCapacity"]
+        * lex["CapitalRecoveryFactor"]
+        * lex["PVAnnuity"]
+    )
+
+    # costs
+    AnnualVariableOperatingCost = (
+        (lex["TotalAnnualTechnologyActivityByMode"] * ds["VariableCost"].fillna(0))
+        .sum(dims="MODE_OF_OPERATION")
+        .where(
+            (ds["VariableCost"].sum(dim="MODE_OF_OPERATION") != 0)
+            & (~ds["VariableCost"].sum(dim="MODE_OF_OPERATION").isnull())
+        )
+    )
+    AnnualFixedOperatingCost = lex["GrossCapacity"] * ds["FixedCost"].fillna(0)
+    OperatingCost = AnnualVariableOperatingCost + AnnualFixedOperatingCost
+
+    SV1Cost = ds["CapitalCost"].fillna(0) * (1 - (lex["SV1Numerator"] / lex["SV1Denominator"]))
+
+    SV2Cost = ds["CapitalCost"].fillna(0) * (1 - (lex["SV2Numerator"] / lex["SV2Denominator"]))
+
+    # costs
+    DiscountedOperatingCost = OperatingCost / lex["DiscountFactorMid"]
+
+    DiscountedCapitalInvestment = CapitalInvestment / lex["DiscountFactor"]
+
+    SalvageValue = (
+        m["NewCapacity"] * SV1Cost.where(lex["sv1_mask"])
+        + m["NewCapacity"] * SV2Cost.where(lex["sv2_mask"])
+    ).fillna(0)
+
+    DiscountedSalvageValue = SalvageValue / lex["DiscountFactorSalvage"]
+
+    TotalDiscountedCostByTechnology = (
+        DiscountedCapitalInvestment + DiscountedOperatingCost - DiscountedSalvageValue
     )
-    m.add_constraints(con, name="TDC1_TotalDiscountedCostByTechnology")
 
-    try:
-        con = (
-            m["TotalDiscountedCostByTechnology"].sum("TECHNOLOGY")
-            + m["TotalDiscountedStorageCost"].sum("STORAGE")
-            - m["TotalDiscountedCost"]
-            == 0
+    if ds["EMISSION"].size > 0:
+        DiscountedTechnologyEmissionsPenalty = (
+            lex["AnnualTechnologyEmissionsPenalty"] / lex["DiscountFactorMid"]
+        )
+
+        TotalDiscountedCostByTechnology = (
+            TotalDiscountedCostByTechnology + DiscountedTechnologyEmissionsPenalty
         )
-    except KeyError:
-        con = m["TotalDiscountedCostByTechnology"].sum("TECHNOLOGY") - m["TotalDiscountedCost"] == 0
-    finally:
-        m.add_constraints(con, name="TDC2_TotalDiscountedCost")
 
-    return m
+        lex.update(
+            {
+                "DiscountedTechnologyEmissionsPenalty": DiscountedTechnologyEmissionsPenalty,
+            }
+        )
+
+    if ds["STORAGE"].size > 0:
+
+        # total costs with storage
+        TotalDiscountedCost = TotalDiscountedCostByTechnology.sum("TECHNOLOGY") + lex[
+            "TotalDiscountedStorageCost"
+        ].sum(["STORAGE", "TECHNOLOGY"])
+
+    else:
+        # total costs without storage
+        TotalDiscountedCost = TotalDiscountedCostByTechnology.sum("TECHNOLOGY")
+
+    lex.update(
+        {
+            "CapitalInvestment": CapitalInvestment,
+            "AnnualVariableOperatingCost": AnnualVariableOperatingCost,
+            "AnnualFixedOperatingCost": AnnualFixedOperatingCost,
+            "OperatingCost": OperatingCost,
+            "DiscountedOperatingCost": DiscountedOperatingCost,
+            "DiscountedCapitalInvestment": DiscountedCapitalInvestment,
+            "DiscountedSalvageValue": DiscountedSalvageValue,
+            "TotalDiscountedCostByTechnology": TotalDiscountedCostByTechnology,
+            "TotalDiscountedCost": TotalDiscountedCost,
+            "SV1Cost": SV1Cost,
+            "SV2Cost": SV2Cost,
+            "SalvageValue": SalvageValue,
+        }
+    )
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/__init__.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from typing import Dict
 
 import xarray as xr
 from linopy import LinearExpression, Model
 
 from tz.osemosys.model.linear_expressions.activity import add_lex_activity
 from tz.osemosys.model.linear_expressions.capacity import add_lex_capacity
+from tz.osemosys.model.linear_expressions.discounting import add_lex_discounting
 from tz.osemosys.model.linear_expressions.emissions import add_lex_emissions
 from tz.osemosys.model.linear_expressions.financials import add_lex_financials
 from tz.osemosys.model.linear_expressions.production import add_lex_quantities
 from tz.osemosys.model.linear_expressions.reserve_margin import add_lex_reserve_margin
 from tz.osemosys.model.linear_expressions.storage import add_lex_storage
 
 
 def add_linear_expressions(ds: xr.Dataset, m: Model) -> Dict[str, LinearExpression]:
     lex = {}
 
+    add_lex_discounting(ds, m, lex)
     add_lex_activity(ds, m, lex)
     add_lex_capacity(ds, m, lex)
     if ds["EMISSION"].size > 0:
         add_lex_emissions(ds, m, lex)
+    if ds["STORAGE"].size > 0:
+        add_lex_storage(ds, m, lex)
     add_lex_financials(ds, m, lex)
     add_lex_quantities(ds, m, lex)
     add_lex_reserve_margin(ds, m, lex)
-    if ds["STORAGE"].size > 0:
-        add_lex_storage(ds, m, lex)
 
     return lex
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/activity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/emissions.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/emissions.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/production.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/production.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     RateOfProductionByTechnologyByMode = m["RateOfActivity"] * ds["OutputActivityRatio"].where(
         ds["OutputActivityRatio"].notnull()
     )
     RateOfProductionByTechnology = RateOfProductionByTechnologyByMode.where(
         ds["OutputActivityRatio"].sum("MODE_OF_OPERATION") != 0
     ).sum(dims="MODE_OF_OPERATION")
     RateOfProduction = RateOfProductionByTechnology.sum(dims="TECHNOLOGY")
+    ProductionByTechnology = RateOfProductionByTechnology * ds["YearSplit"]
     Production = RateOfProduction * ds["YearSplit"]
     ProductionAnnual = Production.sum(dims="TIMESLICE")
 
     RateOfUseByTechnologyByMode = m["RateOfActivity"] * ds["InputActivityRatio"].where(
         ds["InputActivityRatio"].notnull()
     )
     RateOfUseByTechnology = RateOfUseByTechnologyByMode.where(
@@ -28,14 +29,15 @@
 
     lex.update(
         {
             "RateOfProductionByTechnologyByMode": RateOfProductionByTechnologyByMode,
             "RateOfProductionByTechnology": RateOfProductionByTechnology,
             "RateOfProduction": RateOfProduction,
             "Production": Production,
+            "ProductionByTechnology": ProductionByTechnology,
             "ProductionAnnual": ProductionAnnual,
             "RateOfUseByTechnologyByMode": RateOfUseByTechnologyByMode,
             "RateOfUseByTechnology": RateOfUseByTechnology,
             "RateOfUse": RateOfUse,
             "Use": Use,
             "UseAnnual": UseAnnual,
         }
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/reserve_margin.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/linear_expressions/reserve_margin.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import xarray as xr
 from linopy import LinearExpression, Model
 
 
 def add_lex_reserve_margin(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]):
     TotalCapacityInReserveMargin = (
         (
-            ds["ReserveMarginTagTechnology"]
-            * ds["CapacityToActivityUnit"]
-            * m["TotalCapacityAnnual"]
+            ds["ReserveMarginTagTechnology"] * ds["CapacityToActivityUnit"] * lex["GrossCapacity"]
         ).where(
             (ds["ReserveMargin"] > 0)
             & (ds["ReserveMarginTagTechnology"] == 1)
             & (ds["ReserveMarginTagTechnology"] * ds["CapacityToActivityUnit"]).notnull()
         )
     ).sum("TECHNOLOGY")
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/variables/capacity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/variables/activity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import xarray as xr
 from linopy import Model
 from numpy import inf
 
 
-def add_capacity_variables(ds: xr.Dataset, m: Model) -> Model:
-    """Add capacity variables to the model
+def add_activity_variables(ds: xr.Dataset, m: Model) -> Model:
+    """Add activity variables to the model
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
 
     Returns
     -------
     linopy.Model
     """
-    # Create the required index
-    RTeY = [ds.coords["REGION"], ds.coords["TECHNOLOGY"], ds.coords["YEAR"]]
+    # Add indices
+    RRTiFY = [
+        ds.coords["REGION"],
+        ds.coords["_REGION"],
+        ds.coords["TIMESLICE"],
+        ds.coords["FUEL"],
+        ds.coords["YEAR"],
+    ]
+    RTeMYTi = [
+        ds.coords["REGION"],
+        ds.coords["TECHNOLOGY"],
+        ds.coords["MODE_OF_OPERATION"],
+        ds.coords["YEAR"],
+        ds.coords["TIMESLICE"],
+    ]
 
-    # masks
-    mask = ds["CapacityOfOneTechnologyUnit"].notnull()
+    m.add_variables(lower=0, upper=inf, coords=RTeMYTi, name="RateOfActivity", integer=False)
+
+    m.add_variables(lower=-inf, upper=inf, coords=RRTiFY, name="Trade", integer=False)
 
-    m.add_variables(
-        lower=0, upper=inf, coords=RTeY, name="NumberOfNewTechnologyUnits", integer=True, mask=mask
-    )
-    m.add_variables(lower=0, upper=inf, coords=RTeY, name="NewCapacity", integer=False)
-    m.add_variables(lower=0, upper=inf, coords=RTeY, name="AccumulatedNewCapacity", integer=False)
-    m.add_variables(lower=0, upper=inf, coords=RTeY, name="TotalCapacityAnnual", integer=False)
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/model/variables/emissions.py` & `tz_osemosys-0.0.4a0/tz/osemosys/model/variables/storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import xarray as xr
 from linopy import Model
 from numpy import inf
 
 
-def add_emission_variables(ds: xr.Dataset, m: Model) -> Model:
-    """Add emisison variables to the model
+def add_storage_variables(ds: xr.Dataset, m: Model) -> Model:
+    """Add storage variables to the model
 
-    Arguments
+        Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
 
     Returns
     -------
     linopy.Model
     """
-    # Create the required indexes
-    RTeY = [ds.coords["REGION"], ds.coords["TECHNOLOGY"], ds.coords["YEAR"]]
-
-    m.add_variables(
-        lower=0, upper=inf, coords=RTeY, name="DiscountedTechnologyEmissionsPenalty", integer=False
-    )
+    RSY = [ds.coords["REGION"], ds.coords["STORAGE"], ds.coords["YEAR"]]
 
+    m.add_variables(lower=0, upper=inf, coords=RSY, name="NewStorageCapacity", integer=False)
     return m
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/base.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,28 +285,40 @@
                 super().__init__(data=args[0])
         else:
             if "data" in data.keys() and len(data.keys()) > 1:
                 raise ValueError(
                     "If initialising via a dict keyed by 'data', 'data' must be the only key."
                 )
             elif "data" in data.keys():
-                super().__init__(data=data["data"])
+                if isinstance(data["data"], dict):
+                    if "data" in data["data"].keys():
+                        super().__init__(**data["data"])
+                    else:
+                        super().__init__(**data)
+                else:
+                    super().__init__(**data)
             else:
                 super().__init__(data=data)
 
     is_composed: bool = False
     data: Union[
         DataVar,  # {data: 6.}
         Dict[IdxVar, DataVar],
         Dict[IdxVar, Dict[IdxVar, DataVar]],
         Dict[IdxVar, Dict[IdxVar, Dict[IdxVar, DataVar]]],
         Dict[IdxVar, Dict[IdxVar, Dict[IdxVar, Dict[IdxVar, DataVar]]]],
         Dict[IdxVar, Dict[IdxVar, Dict[IdxVar, Dict[IdxVar, Dict[IdxVar, DataVar]]]]],
     ]
 
+    def __getitem__(self, key: Any):
+        return self.data[key]
+
+    def __setitem__(self, key: Any, value: Any):
+        self.data[key] = value
+
 
 class DepreciationMethod(str, Enum):
     sinking_fund = "sinking-fund"
     straight_line = "straight-line"
 
 
 def _check_nesting_depth(obj_id: str, data: Any, max_depth: int):
@@ -514,22 +526,27 @@
         _compose_RCY,
         _compose_RIY,
         _compose_RO,
         _null,
     ],
 ):
     # add a new OSEMOSYSData class for each data cooridinate key
-    setattr(OSeMOSYSData, key, create_model("OSeMOSYSData" + f"_{key}", __base__=OSeMOSYSData))
+    setattr(
+        OSeMOSYSData,
+        key,
+        create_model("OSeMOSYSData" + f"_{key}", __base__=OSeMOSYSData),
+    )
 
     # add the compose method to each new class
     getattr(OSeMOSYSData, key).compose = func
 
     # add the datatype constructors
     for _type, validator in zip(
-        ["Int", "Bool", "SumOne"], [check_or_cast_int, check_or_cast_bool, nested_sum_one]
+        ["Int", "Bool", "SumOne"],
+        [check_or_cast_int, check_or_cast_bool, nested_sum_one],
     ):
         setattr(
             getattr(OSeMOSYSData, key),
             _type,
             create_model(
                 f"OSeMOSYSData_{key}_{_type}",
                 __base__=getattr(OSeMOSYSData, key),
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/commodity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/commodity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/base.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/commodity.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/commodity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/impact.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/model.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/region.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/storage.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/technology.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/technology.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/time_definition.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/compat/time_definition.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/impact.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/model.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/region.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/storage.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/technology.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/technology.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from pydantic import ConfigDict, Field, conlist, model_validator
+from pydantic import ConfigDict, Field, conlist, field_serializer, model_validator
 
 from tz.osemosys.defaults import defaults
 from tz.osemosys.schemas.base import OSeMOSYSBase, OSeMOSYSData, cast_osemosysdata_value
 from tz.osemosys.schemas.compat.technology import OtooleTechnology
 from tz.osemosys.schemas.validation.validation_utils import check_min_vals_lower_max
 
 
@@ -64,20 +64,29 @@
         },
     )
 
     OperatingMode(**basic_operating_mode)
     ```
     """
 
+    @field_serializer
+    def osemosysdata_serializer(cls, value: Any, serializer_field):
+        if isinstance(value, serializer_field.type_):
+            return value.data
+        else:
+            return value
+
     model_config = ConfigDict(extra="forbid")
 
     opex_variable: OSeMOSYSData.RY | None = Field(
         OSeMOSYSData.RY(defaults.technology_opex_variable_cost)
     )
-    emission_activity_ratio: OSeMOSYSData.RIY | None = Field(None)
+    emission_activity_ratio: OSeMOSYSData.RIY | None = Field(
+        None, serializer=osemosysdata_serializer
+    )
     input_activity_ratio: OSeMOSYSData.RCY | None = Field(None)
     output_activity_ratio: OSeMOSYSData.RCY | None = Field(None)
     to_storage: OSeMOSYSData.RO.Bool | None = Field(None)
     from_storage: OSeMOSYSData.RO.Bool | None = Field(None)
 
     def compose(self, **sets):
         # compose root OSeMOSYSData
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/time_definition.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/time_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,22 @@
     @classmethod
     def from_years(cls, years):
         return cls(years=dict(zip(sorted(years)[:-1], sorted(years)[1:])))
 
     def inv(self):
         return TimeAdjacency(
             years={v: k for k, v in self.years.items()},
-            seasons={v: k for k, v in self.seasons.items()} if self.seasons else None,
-            day_types=({v: k for k, v in self.day_types.items()} if self.day_types else None),
+            seasons={v: k for k, v in self.seasons.items()} if self.seasons is not None else None,
+            day_types=(
+                {v: k for k, v in self.day_types.items()} if self.day_types is not None else None
+            ),
             time_brackets=(
-                {v: k for k, v in self.time_brackets.items()} if self.time_brackets else None
+                {v: k for k, v in self.time_brackets.items()}
+                if self.time_brackets is not None
+                else None
             ),
             timeslices={v: k for k, v in self.timeslices.items()},
         )
 
 
 def construction_from_timeslices(values: Any):
     """pathway 3: years plus any of timeslices, timeslice_in_timebracket, timeslice_in_daytype,
@@ -143,14 +147,20 @@
       - option: if adjacency is specified:
         - use specified adjacency, validating keys
         - else:
           - if ordered yearparts, daytypes, and dayparts given, assume adjacency
           - else: raise error for required parameter
     """
 
+    def _first_part_in_timeslice(parts, timeslice):
+        for part in parts:
+            if part in timeslice:
+                return part
+        raise ValueError(f"None of {parts} are in {timeslices}")
+
     # Convert list of int to list of str
     for key in values.keys():
         if isinstance(values[key], list):
             values[key] = [str(item) if isinstance(item, int) else item for item in values[key]]
 
     years = values.get("years")
     seasons = values.get("seasons")
@@ -160,82 +170,99 @@
     # build timeslices from parts
     timeslices = build_timeslices_from_parts(seasons, day_types, time_brackets)
     values["timeslices"] = timeslices
 
     # build time_brackets/seasons/day_types and link to timeslice if necessary
     if time_brackets:
         values["timeslice_in_timebracket"] = {
-            timeslice: [time_bracket for time_bracket in time_brackets if time_bracket in timeslice]
+            timeslice: _first_part_in_timeslice(time_brackets, timeslice)
             for timeslice in timeslices
         }
     else:
-        values["daily_time_brackets"] = [1]
-        values["timeslice_in_timebracket"] = {timeslice: [1] for timeslice in timeslices}
+        values["daily_time_brackets"] = ["1"]
+        values["timeslice_in_timebracket"] = {timeslice: "1" for timeslice in timeslices}
     if seasons:
         values["timeslice_in_season"] = {
-            timeslice: [season for season in seasons if season in timeslice]
-            for timeslice in timeslices
+            timeslice: _first_part_in_timeslice(seasons, timeslice) for timeslice in timeslices
         }
     else:
-        values["seasons"] = [1]
-        values["timeslice_in_season"] = {timeslice: [1] for timeslice in timeslices}
+        values["seasons"] = ["1"]
+        values["timeslice_in_season"] = {timeslice: "1" for timeslice in timeslices}
     if day_types:
         values["timeslice_in_daytype"] = {
-            timeslice: [day_type for day_type in day_types if day_type in timeslice]
-            for timeslice in timeslices
+            timeslice: _first_part_in_timeslice(day_types, timeslice) for timeslice in timeslices
         }
     else:
-        values["day_types"] = [1]
-        values["timeslice_in_daytype"] = {timeslice: [1] for timeslice in timeslices}
+        values["day_types"] = ["1"]
+        values["timeslice_in_daytype"] = {timeslice: "1" for timeslice in timeslices}
 
     # validate keys on splits, if any, or maybe get parts
     year_split, days_in_day_type, day_split = validate_parts_from_splits(
-        timeslices, day_types, time_brackets, values
+        timeslices,
+        day_types or values["day_types"],
+        time_brackets or values["daily_time_brackets"],
+        values,
     )
     values["year_split"] = year_split
     values["day_split"] = day_split
     values["days_in_day_type"] = days_in_day_type
 
     # if adjacency is given, validate keys
     adj = values.get("adj")
     if adj is not None:
         validate_adjacency_keys(adj, timeslices, years, seasons, day_types, time_brackets)
     else:
-        adj = TimeAdjacency(
+        build_adj = dict(
             years=dict(zip(sorted(years)[:-1], sorted(years)[1:])),
             timeslices=dict(zip(timeslices[:-1], timeslices[1:])),
         )
+        if seasons is not None:
+            build_adj["seasons"] = (
+                dict(zip(seasons[:-1], seasons[1:])) if len(seasons) > 1 else None
+            )
+        if day_types is not None:
+            build_adj["day_types"] = (
+                dict(zip(day_types[:-1], day_types[1:])) if len(day_types) > 1 else None
+            )
+        if time_brackets is not None:
+            build_adj["time_brackets"] = (
+                dict(zip(time_brackets[:-1], time_brackets[1:])) if len(time_brackets) > 1 else None
+            )
+
+        adj = TimeAdjacency(**build_adj)
         values["adj"] = adj
 
     return values
 
 
 def construction_from_years_only(values: Any):
     """pathway 1: years only
     - build unitary yearparts, daytypes, and dayparts
     - build adjacency from ordered years
     """
     years = values.get("years")
 
-    values["yearparts"] = [1]
-    values["day_types"] = [1]
-    values["seasons"] = [1]
-    values["timeslices"] = [1]
-    values["daily_time_brackets"] = [1]
-    values["dayparts"] = [1]
-
-    values["year_split"] = {1: 1.0}
-    values["day_split"] = {1: 1.0}
-    values["days_in_day_type"] = {1: 1.0}
-
-    values["timeslice_in_timebracket"] = {1: 1}
-    values["timeslice_in_daytype"] = {1: 1}
-    values["timeslice_in_season"] = {1: 1}
-    values["adj"] = TimeAdjacency.from_years(years)
-    values["adj_inv"] = TimeAdjacency.from_years(years).inv()
+    values["yearparts"] = ["1"]
+    values["day_types"] = ["1"]
+    values["seasons"] = ["1"]
+    values["timeslices"] = ["1"]
+    values["daily_time_brackets"] = ["1"]
+    values["dayparts"] = ["1"]
+
+    values["year_split"] = {"1": 1.0}
+    values["day_split"] = {"1": 1.0}
+    values["days_in_day_type"] = {"1": 1.0}
+
+    values["timeslice_in_timebracket"] = {"1": "1"}
+    values["timeslice_in_daytype"] = {"1": "1"}
+    values["timeslice_in_season"] = {"1": "1"}
+    values["adj"] = TimeAdjacency(
+        years=dict(zip(sorted(years)[:-1], sorted(years)[1:])),
+    )
+    values["adj_inv"] = values["adj"].inv()
 
     return values
 
 
 def format_by_max_length(val: int, max):
     if max > 10:
         return f"{val:02}"
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/impact_validation.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/impact_validation.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_composition.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/model_composition.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_presolve.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/model_presolve.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/region_validation.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/region_validation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tz.osemosys.utils import json_dict_to_dataframe
+import pandas as pd
 
 
 def reserve_margin_fully_defined(values):
     """
     Check that reserve margin is fully defined
     """
     reserve_margin = values.get("reserve_margin")
@@ -24,17 +24,17 @@
     Check that discount rates are in decimals
     """
     discount_rate = values.get("discount_rate")
     discount_rate_idv = values.get("discount_rate_idv")
     discount_rate_storage = values.get("discount_rate_storage")
 
     if discount_rate is not None:
-        df = json_dict_to_dataframe(discount_rate.data).iloc[:, -1]
+        df = pd.json_normalize(discount_rate.data).iloc[:, -1]
         assert (df.abs() < 1).all(), "discount_rate should take decimal values"
     if discount_rate_idv is not None:
-        df = json_dict_to_dataframe(discount_rate_idv.data).iloc[:, -1]
+        df = pd.json_normalize(discount_rate_idv.data).iloc[:, -1]
         assert (df.abs() < 1).all(), "discount_rate_idv should take decimal values"
     if discount_rate_storage is not None:
-        df = json_dict_to_dataframe(discount_rate_storage.data).iloc[:, -1]
+        df = pd.json_normalize(discount_rate_storage.data).iloc[:, -1]
         assert (df.abs() < 1).all(), "discount_rate_storage should take decimal values"
 
     return values
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/technology_validation.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/technology_validation.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/timedefinition_validation.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/timedefinition_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,36 +147,60 @@
     adj: Mapping,
     timeslices: List[str],
     years: List[int],
     seasons: List[str] | None,
     day_types: List[str] | None,
     time_brackets: List[str] | None,
 ):
-    if set(list(adj["timeslices"].keys()) + list(adj["timeslices"].values())) != set(timeslices):
+    if len(timeslices) > 1 and (
+        set(list(adj["timeslices"].keys()) + list(adj["timeslices"].values())) != set(timeslices)
+    ):
         raise ValueError("provided 'timeslices' do not match keys or values of 'adj.timeslices'")
-    if set(list(adj["years"].keys()) + list(adj["years"].values())) != set(years):
+    if {int(yr) for yr in list(adj["years"].keys()) + list(adj["years"].values())} != set(years):
         raise ValueError("provided 'years' do not match keys or values of 'adj.years'")
     if seasons is not None and "seasons" in adj.keys():
-        if set(list(adj["seasons"].keys()) + list(adj["seasons"].values())) != set(seasons):
-            raise ValueError("provided 'seasons' do not match keys or values of 'adj.seasons'")
-    elif seasons is not None or "seasons" in adj.keys():
+        if len(seasons) > 1:
+            if set(list(adj["seasons"].keys()) + list(adj["seasons"].values())) != set(seasons):
+                raise ValueError("provided 'seasons' do not match keys or values of 'adj.seasons'")
+        else:
+            if adj["seasons"] != {}:
+                raise ValueError(
+                    f"Adjacency provided for seasons, but only one season {seasons} is defined."
+                )
+    elif seasons is not None or adj.get("seasons"):
         raise ValueError("seasons provided without adjacency.")
     if day_types is not None and "day_types" in adj.keys():
-        if set(list(adj["day_types"].keys()) + list(adj["day_types"].values())) != set(day_types):
-            raise ValueError("provided 'day_types' do not match keys or values of 'adj.day_types'")
-    elif day_types is not None or "day_types" in adj.keys():
+        if len(day_types) > 1:
+            if set(list(adj["day_types"].keys()) + list(adj["day_types"].values())) != set(
+                day_types
+            ):
+                raise ValueError(
+                    "provided 'day_types' do not match keys or values of 'adj.day_types'"
+                )
+        else:
+            if adj["day_types"] != {}:
+                raise ValueError(
+                    f"Adjacency provided for day_types, but only one day_type {day_types} is defined."  # NOQA E501
+                )
+    elif day_types is not None or adj.get("day_types"):
         raise ValueError("day_types provided without adjacency")
     if time_brackets is not None and "time_brackets" in adj.keys():
-        if set(list(adj["time_brackets"].keys()) + list(adj["time_brackets"].values())) != set(
-            time_brackets
-        ):
-            raise ValueError(
-                "provided 'time_brackets' do not match keys or values of 'adj.time_brackets'"
-            )
-    elif time_brackets is not None or "time_brackets" in adj.keys():
+        if len(time_brackets) > 1:
+            if set(list(adj["time_brackets"].keys()) + list(adj["time_brackets"].values())) != set(
+                time_brackets
+            ):
+                raise ValueError(
+                    "provided 'time_brackets' do not match keys or values of 'adj.time_brackets'"
+                )
+        else:
+            if adj["time_brackets"] != {}:
+                raise ValueError(
+                    f"Adjacency provided for time_brackets, but only one time_bracket {time_brackets} is defined."  # NOQA E501
+                )
+    elif time_brackets is not None or adj.get("time_brackets"):
         raise ValueError("time_brackets provided without adjacency")
 
 
 def validate_adjacency_fullyconstrained(
     timeslices: List[str | int],
     timeslice_in_season: List[str | int] | None,
     timeslice_in_daytype: List[str | int] | None,
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/validation_utils.py` & `tz_osemosys-0.0.4a0/tz/osemosys/schemas/validation/validation_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 
 from tz.osemosys.utils import json_dict_to_dataframe
 
 
 def check_sums_one(data, leniency, cols, cols_to_groupby):
-    data_df = json_dict_to_dataframe(data)
+    data_df = pd.json_normalize(data)
     data_df.columns = cols
     assert np.allclose(data_df.groupby(cols_to_groupby)["VALUE"].sum(), 1, atol=leniency), (
         f"demand_profile must sum to one (within {leniency}) for all REGION,"
         f" YEAR, and commodity; commodity {id} does not"
     )
```

### Comparing `tz_osemosys-0.0.3/tz/osemosys/utils/__init__.py` & `tz_osemosys-0.0.4a0/tz/osemosys/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/utils/cfg_parser.py` & `tz_osemosys-0.0.4a0/tz/osemosys/utils/cfg_parser.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.3/tz/osemosys/utils/utils.py` & `tz_osemosys-0.0.4a0/tz/osemosys/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,34 +278,36 @@
         prefix (str, optional): used to build a prefix for the column names when constructing the
         DataFrame. Defaults to "".
 
     Returns:
         DataFrame: data in pandas DataFrame format
     """
 
-    if isinstance(data, dict):
+    # Check if data is not empty
+    if isinstance(data, dict) and len(data) > 0:
         # If data is a dictionary, iterate through its items
         result = pd.DataFrame()
         for key, value in data.items():
             new_prefix = f"{prefix}-{key}" if prefix else key
             df = json_dict_to_dataframe(value, new_prefix)
             result = pd.concat([result, df], axis=1)
         if (
             prefix == ""
         ):  # Execute this step if all iterations complete and final result ready to be returned
             result = result.T
             result = result.reset_index()
+
             result = pd.concat([result["index"].str.split("-", expand=True), result[0]], axis=1)
             return result
         else:
             return result
     else:
         # If data is not a dictionary, create a single-column DataFrame
         # with empty column name, used in iteration
-        return pd.DataFrame({prefix: [data]})
+        return pd.json_normalize({prefix: [data]})
 
 
 def add_instance_data_to_output_dfs(instance, output_dfs, otoole_stems, root_column=None):
     """Add data from the given class instance to the given output dfs, returning the modified dfs
     If root_column is given, add root_column as a column to the instance data with values of self.id
     (to account for data from multiple instances, e.g. technology, being added to the same df)
 
@@ -325,15 +327,15 @@
         sub_attribute = otoole_stems[output_file]["attribute"]
 
         # Add data from this class instance to the output_dfs
         if getattr(instance, f"{sub_attribute}") is not None:
             if isinstance(getattr(instance, f"{sub_attribute}"), list):
                 data = pd.DataFrame({"VALUE": getattr(instance, f"{sub_attribute}")})
             else:
-                data = json_dict_to_dataframe(getattr(instance, f"{sub_attribute}").data)
+                data = pd.json_normalize(getattr(instance, f"{sub_attribute}").data)
 
             columns = otoole_stems[output_file]["columns"][:]
             if root_column is not None:
                 columns.remove(root_column)
             data.columns = columns
             if root_column is not None:
                 data[root_column] = instance.id
@@ -354,18 +356,30 @@
         self: An instance of the Runspec class
 
     Returns:
         output_dfs (dict{str:df}): a dict of output CSV name and associated df
     """
     # Attribute and root column names
     attributes = {
-        "time_definition": {"otoole_stems": self.time_definition.otoole_stems, "root_column": None},
-        "regions": {"otoole_stems": self.regions[0].otoole_stems, "root_column": "REGION"},
-        "commodities": {"otoole_stems": self.commodities[0].otoole_stems, "root_column": "FUEL"},
-        "impacts": {"otoole_stems": self.impacts[0].otoole_stems, "root_column": "EMISSION"},
+        "time_definition": {
+            "otoole_stems": self.time_definition.otoole_stems,
+            "root_column": None,
+        },
+        "regions": {
+            "otoole_stems": self.regions[0].otoole_stems,
+            "root_column": "REGION",
+        },
+        "commodities": {
+            "otoole_stems": self.commodities[0].otoole_stems,
+            "root_column": "FUEL",
+        },
+        "impacts": {
+            "otoole_stems": self.impacts[0].otoole_stems,
+            "root_column": "EMISSION",
+        },
         "technologies": {
             "otoole_stems": self.technologies[0].otoole_stems,
             "root_column": "TECHNOLOGY",
         },
     }
     # Add storage technologies to attributes dict if present
     if self.storage_technologies:
```

### Comparing `tz_osemosys-0.0.3/tz_osemosys.egg-info/PKG-INFO` & `tz_osemosys-0.0.4a0/tz_osemosys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tz-osemosys
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero
 Author-email: Lucas Kruitwagen <lucas.kruitwagen@gmail.com>, Ed Gill <edwardxtg@gmail.com>, Abhishek Shivakumar <abhishek0208@gmail.com>
 Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org
 Project-URL: Source, https://github.com/transitionzero/tz-osemosys
 Keywords: energy,milp,climate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.3 Summary: An OSeMOSYS
+Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.4a0 Summary: An OSeMOSYS
 implementation for the Future Energy Outlook by TransitionZero Author-email:
 Lucas Kruitwagen
 gmail.com>, Ed Gill
 gmail.com>, Abhishek Shivakumar
 gmail.com> Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org Project-URL: Source, https://
```

