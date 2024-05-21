# Comparing `tmp/datajunction_query-0.0.1a47.tar.gz` & `tmp/datajunction_query-0.0.1a48.tar.gz`

## Comparing `datajunction_query-0.0.1a47.tar` & `datajunction_query-0.0.1a48.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.coveragerc
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.isort.cfg
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.pylintrc
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.readthedocs.yml
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/Dockerfile
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/Makefile
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/alembic.ini
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/config.djqs.yml
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/config.jsonschema
--rw-r--r--   0        0        0    34516 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/openapi.json
--rw-r--r--   0        0        0   159833 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/pdm.lock
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/setup.cfg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tox.ini
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/alembic/README
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/alembic/env.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/alembic/script.py.mako
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/alembic/versions/2023_02_28_0541-a7e11a2438b4_initial_migration.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/alembic/versions/2023_10_09_1858-f3407a1ec625_add_type_and_extra_para_ms_field_for_.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/__about__.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/__init__.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/config.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/constants.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/engine.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/enum.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/exceptions.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/fixes.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/typing.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/catalogs.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/engines.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/helpers.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/main.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/queries.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/api/tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/models/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/models/catalog.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/models/engine.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/models/query.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/djqs/models/table.py
--rw-r--r--   0        0        0  1323008 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/default.duckdb
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/druid_environment
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/druid_init.sh
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/druid_spec.json
--rw-r--r--   0        0        0    30612 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/duckdb.sql
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/duckdb_load.py
--rw-r--r--   0        0        0    18765 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/postgres_init.roads.sql
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/postgres_init.sql
--rw-r--r--   0        0        0    12877 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/spark.roads.sql
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/spark_load_roads.py
--rwxr-xr-x   0        0        0     4051 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/wait-for
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/cockroachdb/cockroachdb_examples_init.sql
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/cockroachdb/cockroachdb_metadata_init.sql
--rw-r--r--   0        0        0    62052 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/cockroachdb/steam-games.csv
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/docker/cockroachdb/steam-hours-played.csv
--rwxr-xr-x   0        0        0      622 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/scripts/generate-openapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/config.djqs.yml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/conftest.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/exceptions_test.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/api/__init__.py
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/api/catalogs_test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/api/engines_test.py
--rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/api/queries_test.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/api/table_test.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/databases/druid.yaml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/databases/gsheets.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/databases/postgres.yaml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/nodes/core/comments.yaml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/nodes/core/dim_users.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/nodes/core/num_comments.yaml
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/configs/nodes/core/users.yaml
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/contractors.parquet
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/dispatchers.parquet
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/hard_hat_state.parquet
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/hard_hats.parquet
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/municipality.parquet
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/municipality_municipality_type.parquet
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/municipality_type.parquet
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/repair_order_details.parquet
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/repair_orders.parquet
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/repair_type.parquet
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/us_region.parquet
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/tests/resources/us_states.parquet
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/.gitignore
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/AUTHORS.rst
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/LICENSE.txt
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/README.rst
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/pyproject.toml
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a47/PKG-INFO
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.coveragerc
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.flake8
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.isort.cfg
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.pylintrc
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.readthedocs.yml
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/Dockerfile
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/Makefile
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/alembic.ini
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/config.djqs.yml
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/config.jsonschema
+-rw-r--r--   0        0        0    34516 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/openapi.json
+-rw-r--r--   0        0        0   159833 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/pdm.lock
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/setup.cfg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tox.ini
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/alembic/README
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/alembic/env.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/alembic/script.py.mako
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/alembic/versions/2023_02_28_0541-a7e11a2438b4_initial_migration.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/alembic/versions/2023_10_09_1858-f3407a1ec625_add_type_and_extra_para_ms_field_for_.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/__about__.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/__init__.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/config.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/constants.py
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/engine.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/enum.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/exceptions.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/fixes.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/typing.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/catalogs.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/engines.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/helpers.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/main.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/queries.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/api/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/models/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/models/catalog.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/models/engine.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/models/query.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/djqs/models/table.py
+-rw-r--r--   0        0        0  1323008 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/default.duckdb
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/druid_environment
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/druid_init.sh
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/druid_spec.json
+-rw-r--r--   0        0        0    30612 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/duckdb.sql
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/duckdb_load.py
+-rw-r--r--   0        0        0    18765 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/postgres_init.roads.sql
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/postgres_init.sql
+-rw-r--r--   0        0        0    12877 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/spark.roads.sql
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/spark_load_roads.py
+-rwxr-xr-x   0        0        0     4051 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/wait-for
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/cockroachdb/cockroachdb_examples_init.sql
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/cockroachdb/cockroachdb_metadata_init.sql
+-rw-r--r--   0        0        0    62052 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/cockroachdb/steam-games.csv
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/docker/cockroachdb/steam-hours-played.csv
+-rwxr-xr-x   0        0        0      622 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/scripts/generate-openapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/config.djqs.yml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/conftest.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/exceptions_test.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/api/__init__.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/api/catalogs_test.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/api/engines_test.py
+-rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/api/queries_test.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/api/table_test.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/databases/druid.yaml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/databases/gsheets.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/databases/postgres.yaml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/nodes/core/comments.yaml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/nodes/core/dim_users.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/nodes/core/num_comments.yaml
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/configs/nodes/core/users.yaml
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/contractors.parquet
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/dispatchers.parquet
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/hard_hat_state.parquet
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/hard_hats.parquet
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/municipality.parquet
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/municipality_municipality_type.parquet
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/municipality_type.parquet
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/repair_order_details.parquet
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/repair_orders.parquet
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/repair_type.parquet
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/us_region.parquet
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/tests/resources/us_states.parquet
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/.gitignore
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/AUTHORS.rst
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/LICENSE.txt
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/README.rst
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/pyproject.toml
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 datajunction_query-0.0.1a48/PKG-INFO
```

### Comparing `datajunction_query-0.0.1a47/.coveragerc` & `datajunction_query-0.0.1a48/.coveragerc`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/.pre-commit-config.yaml` & `datajunction_query-0.0.1a48/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/CODE_OF_CONDUCT.md` & `datajunction_query-0.0.1a48/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/Makefile` & `datajunction_query-0.0.1a48/Makefile`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/alembic.ini` & `datajunction_query-0.0.1a48/alembic.ini`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/config.jsonschema` & `datajunction_query-0.0.1a48/config.jsonschema`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/openapi.json` & `datajunction_query-0.0.1a48/openapi.json`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/pdm.lock` & `datajunction_query-0.0.1a48/pdm.lock`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/setup.cfg` & `datajunction_query-0.0.1a48/setup.cfg`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/alembic/env.py` & `datajunction_query-0.0.1a48/alembic/env.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/alembic/script.py.mako` & `datajunction_query-0.0.1a48/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/alembic/versions/2023_02_28_0541-a7e11a2438b4_initial_migration.py` & `datajunction_query-0.0.1a48/alembic/versions/2023_02_28_0541-a7e11a2438b4_initial_migration.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/alembic/versions/2023_10_09_1858-f3407a1ec625_add_type_and_extra_para_ms_field_for_.py` & `datajunction_query-0.0.1a48/alembic/versions/2023_10_09_1858-f3407a1ec625_add_type_and_extra_para_ms_field_for_.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/config.py` & `datajunction_query-0.0.1a48/djqs/config.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/engine.py` & `datajunction_query-0.0.1a48/djqs/engine.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/enum.py` & `datajunction_query-0.0.1a48/djqs/enum.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/exceptions.py` & `datajunction_query-0.0.1a48/djqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/typing.py` & `datajunction_query-0.0.1a48/djqs/typing.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/utils.py` & `datajunction_query-0.0.1a48/djqs/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/api/catalogs.py` & `datajunction_query-0.0.1a48/djqs/api/catalogs.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/api/engines.py` & `datajunction_query-0.0.1a48/djqs/api/engines.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/api/helpers.py` & `datajunction_query-0.0.1a48/djqs/api/helpers.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/api/main.py` & `datajunction_query-0.0.1a48/djqs/api/main.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/api/queries.py` & `datajunction_query-0.0.1a48/djqs/api/queries.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/api/tables.py` & `datajunction_query-0.0.1a48/djqs/api/tables.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/models/catalog.py` & `datajunction_query-0.0.1a48/djqs/models/catalog.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/models/engine.py` & `datajunction_query-0.0.1a48/djqs/models/engine.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/djqs/models/query.py` & `datajunction_query-0.0.1a48/djqs/models/query.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/default.duckdb` & `datajunction_query-0.0.1a48/docker/default.duckdb`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/druid_environment` & `datajunction_query-0.0.1a48/docker/druid_environment`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/druid_spec.json` & `datajunction_query-0.0.1a48/docker/druid_spec.json`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/duckdb.sql` & `datajunction_query-0.0.1a48/docker/duckdb.sql`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/postgres_init.roads.sql` & `datajunction_query-0.0.1a48/docker/postgres_init.roads.sql`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/postgres_init.sql` & `datajunction_query-0.0.1a48/docker/postgres_init.sql`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/spark.roads.sql` & `datajunction_query-0.0.1a48/docker/spark.roads.sql`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/spark_load_roads.py` & `datajunction_query-0.0.1a48/docker/spark_load_roads.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/wait-for` & `datajunction_query-0.0.1a48/docker/wait-for`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/cockroachdb/cockroachdb_examples_init.sql` & `datajunction_query-0.0.1a48/docker/cockroachdb/cockroachdb_examples_init.sql`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/cockroachdb/steam-games.csv` & `datajunction_query-0.0.1a48/docker/cockroachdb/steam-games.csv`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/docker/cockroachdb/steam-hours-played.csv` & `datajunction_query-0.0.1a48/docker/cockroachdb/steam-hours-played.csv`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/scripts/generate-openapi.py` & `datajunction_query-0.0.1a48/scripts/generate-openapi.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/conftest.py` & `datajunction_query-0.0.1a48/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/exceptions_test.py` & `datajunction_query-0.0.1a48/tests/exceptions_test.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/utils_test.py` & `datajunction_query-0.0.1a48/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/api/catalogs_test.py` & `datajunction_query-0.0.1a48/tests/api/catalogs_test.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/api/engines_test.py` & `datajunction_query-0.0.1a48/tests/api/engines_test.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/api/queries_test.py` & `datajunction_query-0.0.1a48/tests/api/queries_test.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/api/table_test.py` & `datajunction_query-0.0.1a48/tests/api/table_test.py`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/contractors.parquet` & `datajunction_query-0.0.1a48/tests/resources/contractors.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/dispatchers.parquet` & `datajunction_query-0.0.1a48/tests/resources/dispatchers.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/hard_hats.parquet` & `datajunction_query-0.0.1a48/tests/resources/hard_hats.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/municipality.parquet` & `datajunction_query-0.0.1a48/tests/resources/municipality.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/repair_order_details.parquet` & `datajunction_query-0.0.1a48/tests/resources/repair_order_details.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/repair_orders.parquet` & `datajunction_query-0.0.1a48/tests/resources/repair_orders.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/repair_type.parquet` & `datajunction_query-0.0.1a48/tests/resources/repair_type.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/tests/resources/us_states.parquet` & `datajunction_query-0.0.1a48/tests/resources/us_states.parquet`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/.gitignore` & `datajunction_query-0.0.1a48/.gitignore`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/LICENSE.txt` & `datajunction_query-0.0.1a48/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/README.rst` & `datajunction_query-0.0.1a48/README.rst`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/pyproject.toml` & `datajunction_query-0.0.1a48/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datajunction_query-0.0.1a47/PKG-INFO` & `datajunction_query-0.0.1a48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: datajunction-query
-Version: 0.0.1a47
+Version: 0.0.1a48
 Summary: OSS Implementation of a DataJunction Query Service
 Project-URL: repository, https://github.com/DataJunction/dj
 Author-email: DataJunction Authors <roberto@dealmeida.net>
 License: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
```

