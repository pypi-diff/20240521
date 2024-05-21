# Comparing `tmp/caluma-9.3.2.tar.gz` & `tmp/caluma-9.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma-9.3.2.tar", max compression
+gzip compressed data, was "caluma-9.3.3.tar", max compression
```

## Comparing `caluma-9.3.2.tar` & `caluma-9.3.3.tar`

### file list

```diff
@@ -1,213 +1,213 @@
--rw-r--r--   0        0        0    59003 2023-12-21 12:15:38.098933 caluma-9.3.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-12-21 12:15:38.098933 caluma-9.3.2/LICENSE
-drwxr-xr-x   0        0        0        0 2023-12-21 12:15:38.098933 caluma-9.3.2/LICENSES/
--rw-r--r--   0        0        0     1957 2023-12-21 12:15:38.098933 caluma-9.3.2/README.md
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/__init__.py
--rw-r--r--   0        0        0     5442 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/caluma_analytics/README.md
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/caluma_analytics/__init__.py
--rw-r--r--   0        0        0      105 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/caluma_analytics/apps.py
--rw-r--r--   0        0        0     3898 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/caluma_analytics/conftest.py
--rw-r--r--   0        0        0      797 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/caluma_analytics/factories.py
--rw-r--r--   0        0        0     1543 2023-12-21 12:15:38.098933 caluma-9.3.2/caluma/caluma_analytics/filters.py
--rw-r--r--   0        0        0     3842 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/management/commands/run_analytics.py
--rw-r--r--   0        0        0    11085 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/0001_initial.py
--rw-r--r--   0        0        0     2007 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py
--rw-r--r--   0        0        0     1025 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/0003_starting_objects.py
--rw-r--r--   0        0        0     1382 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/0004_simple_history.py
--rw-r--r--   0        0        0      781 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/0005_analytics_field_ordering.py
--rw-r--r--   0        0        0      631 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/0006_rename_form_slug_fields.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/migrations/__init__.py
--rw-r--r--   0        0        0     3593 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/models.py
--rw-r--r--   0        0        0     4082 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/pivot_table.py
--rw-r--r--   0        0        0     7235 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/schema.py
--rw-r--r--   0        0        0     4269 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/serializers.py
--rw-r--r--   0        0        0    44853 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/simple_table.py
--rw-r--r--   0        0        0    17612 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/sql.py
--rw-r--r--   0        0        0     1401 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_analytics/visibility.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/__init__.py
--rw-r--r--   0        0        0      975 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/apps.py
--rw-r--r--   0        0        0      195 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/collections.py
--rw-r--r--   0        0        0    11331 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/conftest.py
--rw-r--r--   0        0        0     2877 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/events.py
--rw-r--r--   0        0        0      325 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/factories.py
--rw-r--r--   0        0        0      485 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/faker.py
--rw-r--r--   0        0        0    19274 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/filters.py
--rw-r--r--   0        0        0      642 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/forms.py
--rw-r--r--   0        0        0     4176 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/health_checks.py
--rw-r--r--   0        0        0     8071 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/jexl.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/management/commands/__init__.py
--rw-r--r--   0        0        0     1824 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/management/commands/cleanup_history.py
--rw-r--r--   0        0        0     3803 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/management/commands/dump_caluma_config.py
--rw-r--r--   0        0        0      794 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/management/commands/migrate.py
--rw-r--r--   0        0        0     4934 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py
--rw-r--r--   0        0        0     3078 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/models.py
--rw-r--r--   0        0        0    11674 2023-12-21 12:15:38.102933 caluma-9.3.2/caluma/caluma_core/mutation.py
--rw-r--r--   0        0        0     3216 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/ordering.py
--rw-r--r--   0        0        0     3195 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/pagination.py
--rw-r--r--   0        0        0     4485 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/permissions.py
--rw-r--r--   0        0        0     1253 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/relay.py
--rw-r--r--   0        0        0     4764 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/serializers.py
--rw-r--r--   0        0        0     7577 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/types.py
--rw-r--r--   0        0        0      387 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/urls.py
--rw-r--r--   0        0        0     2430 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/validations.py
--rw-r--r--   0        0        0     1607 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/views.py
--rw-r--r--   0        0        0     2937 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_core/visibilities.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_data_source/__init__.py
--rw-r--r--   0        0        0      107 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_data_source/apps.py
--rw-r--r--   0        0        0     2066 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_data_source/data_source_handlers.py
--rw-r--r--   0        0        0     3231 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_data_source/data_sources.py
--rw-r--r--   0        0        0     1427 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_data_source/schema.py
--rw-r--r--   0        0        0      508 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_data_source/utils.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/__init__.py
--rw-r--r--   0        0        0     2472 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/api.py
--rw-r--r--   0        0        0      100 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/apps.py
--rw-r--r--   0        0        0    10172 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/domain_logic.py
--rw-r--r--   0        0        0     6287 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/factories.py
--rw-r--r--   0        0        0    19812 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/filters.py
--rw-r--r--   0        0        0     3283 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/format_validators.py
--rw-r--r--   0        0        0     7830 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/historical_schema.py
--rw-r--r--   0        0        0     7528 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/jexl.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/management/commands/__init__.py
--rw-r--r--   0        0        0     1880 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/management/commands/copy_form.py
--rw-r--r--   0        0        0      631 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/management/commands/create_bucket.py
--rw-r--r--   0        0        0     1194 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/management/commands/recalculate_calc_answers.py
--rw-r--r--   0        0        0    10983 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0001_initial.py
--rw-r--r--   0        0        0     2829 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0002_auto_20181221_1517.py
--rw-r--r--   0        0        0     3862 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0003_auto_20190130_0920.py
--rw-r--r--   0        0        0     1565 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0004_auto_20190207_1405.py
--rw-r--r--   0        0        0      825 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0005_auto_20190208_1016.py
--rw-r--r--   0        0        0      800 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0006_choice_type_conversion.py
--rw-r--r--   0        0        0      629 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0007_auto_20190208_1232.py
--rw-r--r--   0        0        0     1179 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0008_auto_20190319_1720.py
--rw-r--r--   0        0        0     2133 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0009_auto_20190321_1722.py
--rw-r--r--   0        0        0     2302 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0010_auto_20190404_0652.py
--rw-r--r--   0        0        0      604 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0011_auto_20190411_0607.py
--rw-r--r--   0        0        0      788 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0012_auto_20190416_1835.py
--rw-r--r--   0        0        0     1256 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0013_auto_20190418_0733.py
--rw-r--r--   0        0        0     1407 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0014_auto_20190429_0910.py
--rw-r--r--   0        0        0      659 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0015_question_format_validators.py
--rw-r--r--   0        0        0      530 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0016_auto_20190510_0843.py
--rw-r--r--   0        0        0      605 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0017_auto_20190619_1320.py
--rw-r--r--   0        0        0     1859 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py
--rw-r--r--   0        0        0      365 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0019_remove_answer_value_document.py
--rw-r--r--   0        0        0    27839 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py
--rw-r--r--   0        0        0     2470 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0021_auto_20190708_0905.py
--rw-r--r--   0        0        0     1453 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py
--rw-r--r--   0        0        0      558 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0023_auto_20190729_1448.py
--rw-r--r--   0        0        0     1087 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0024_auto_20190919_1244.py
--rw-r--r--   0        0        0     4834 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py
--rw-r--r--   0        0        0      828 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0026_auto_20191031_0834.py
--rw-r--r--   0        0        0     2087 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0027_auto_20200113_0727.py
--rw-r--r--   0        0        0    12675 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0028_auto_20200210_0929.py
--rw-r--r--   0        0        0     1570 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py
--rw-r--r--   0        0        0     1281 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0030_auto_20200219_1359.py
--rw-r--r--   0        0        0     1701 2023-12-21 12:15:38.106933 caluma-9.3.2/caluma/caluma_form/migrations/0031_auto_20200220_0910.py
--rw-r--r--   0        0        0     1153 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0032_auto_20200220_1311.py
--rw-r--r--   0        0        0     1269 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0033_slugfield_length.py
--rw-r--r--   0        0        0      518 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0034_fix_fk_lengths.py
--rw-r--r--   0        0        0     1687 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py
--rw-r--r--   0        0        0     1386 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0036_default_answers.py
--rw-r--r--   0        0        0      610 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0037_default_answer_one2one.py
--rw-r--r--   0        0        0     3050 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0038_auto_20201224_0920.py
--rw-r--r--   0        0        0      461 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0038_remove_table_answer_value.py
--rw-r--r--   0        0        0      283 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0039_merge_20210114_0956.py
--rw-r--r--   0        0        0    10393 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py
--rw-r--r--   0        0        0     2149 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0041_action_button_question.py
--rw-r--r--   0        0        0      750 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0042_auto_20220110_1051.py
--rw-r--r--   0        0        0     1209 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py
--rw-r--r--   0        0        0      991 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0044_migrate_format_validators.py
--rw-r--r--   0        0        0     5738 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0045_simple_history.py
--rw-r--r--   0        0        0     5998 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/0046_file_answer_reverse_keys.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/migrations/__init__.py
--rw-r--r--   0        0        0    23193 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/models.py
--rw-r--r--   0        0        0     2213 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/ordering.py
--rw-r--r--   0        0        0    38001 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/schema.py
--rw-r--r--   0        0        0    23084 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/serializers.py
--rw-r--r--   0        0        0     7471 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/signals.py
--rw-r--r--   0        0        0     3883 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/storage_clients.py
--rw-r--r--   0        0        0     8044 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/structure.py
--rw-r--r--   0        0        0    18456 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_form/validators.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_logging/__init__.py
--rw-r--r--   0        0        0      103 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_logging/apps.py
--rw-r--r--   0        0        0      365 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_logging/factories.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_logging/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.110933 caluma-9.3.2/caluma/caluma_logging/management/commands/__init__.py
--rw-r--r--   0        0        0     1087 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_logging/management/commands/cleanup_access_log.py
--rw-r--r--   0        0        0     1777 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_logging/middleware.py
--rw-r--r--   0        0        0     1559 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_logging/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_logging/migrations/__init__.py
--rw-r--r--   0        0        0      657 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_logging/models.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_user/__init__.py
--rw-r--r--   0        0        0      100 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_user/apps.py
--rw-r--r--   0        0        0      986 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_user/models.py
--rw-r--r--   0        0        0      667 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_user/permissions.py
--rw-r--r--   0        0        0     3355 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_user/views.py
--rw-r--r--   0        0        0      711 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_user/visibilities.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/__init__.py
--rw-r--r--   0        0        0     7821 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/api.py
--rw-r--r--   0        0        0      618 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/apps.py
--rw-r--r--   0        0        0    21249 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/domain_logic.py
--rw-r--r--   0        0        0     1606 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/dynamic_groups.py
--rw-r--r--   0        0        0     1941 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/dynamic_tasks.py
--rw-r--r--   0        0        0      533 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/events.py
--rw-r--r--   0        0        0     2674 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/factories.py
--rw-r--r--   0        0        0     6851 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/filters.py
--rw-r--r--   0        0        0     6485 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/jexl.py
--rw-r--r--   0        0        0    11029 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0001_initial.py
--rw-r--r--   0        0        0      665 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py
--rw-r--r--   0        0        0      755 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py
--rw-r--r--   0        0        0     1631 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py
--rw-r--r--   0        0        0     4268 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py
--rw-r--r--   0        0        0      993 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py
--rw-r--r--   0        0        0     1034 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py
--rw-r--r--   0        0        0      686 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py
--rw-r--r--   0        0        0     1620 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py
--rw-r--r--   0        0        0      752 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py
--rw-r--r--   0        0        0     1234 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py
--rw-r--r--   0        0        0    21984 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py
--rw-r--r--   0        0        0     3458 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py
--rw-r--r--   0        0        0     1120 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py
--rw-r--r--   0        0        0     1298 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py
--rw-r--r--   0        0        0     2219 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py
--rw-r--r--   0        0        0     7593 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py
--rw-r--r--   0        0        0      924 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py
--rw-r--r--   0        0        0      924 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0019_slugfield_length.py
--rw-r--r--   0        0        0     2849 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0020_case_families.py
--rw-r--r--   0        0        0     1741 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py
--rw-r--r--   0        0        0     2503 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0022_workitem_name_description.py
--rw-r--r--   0        0        0     1063 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py
--rw-r--r--   0        0        0     2490 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py
--rw-r--r--   0        0        0     1452 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py
--rw-r--r--   0        0        0     1336 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py
--rw-r--r--   0        0        0     6415 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py
--rw-r--r--   0        0        0     2618 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0028_redoable_field.py
--rw-r--r--   0        0        0      853 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0029_task_continue_async.py
--rw-r--r--   0        0        0     3680 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py
--rw-r--r--   0        0        0     3474 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/0031_simple_history.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/migrations/__init__.py
--rw-r--r--   0        0        0     9946 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/models.py
--rw-r--r--   0        0        0    12709 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/schema.py
--rw-r--r--   0        0        0    19994 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/serializers.py
--rw-r--r--   0        0        0     4914 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/utils.py
--rw-r--r--   0        0        0     1892 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/validators.py
--rw-r--r--   0        0        0     2120 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/caluma_workflow/visibilities.py
--rw-r--r--   0        0        0    13211 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/conftest.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/extensions/__init__.py
--rw-r--r--   0        0        0       53 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/extensions/data_sources.py
--rw-r--r--   0        0        0       39 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/extensions/dynamic_groups.py
--rw-r--r--   0        0        0       40 2023-12-21 12:15:38.114933 caluma-9.3.2/caluma/extensions/events.py
--rw-r--r--   0        0        0       58 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/extensions/format_validators.py
--rw-r--r--   0        0        0       52 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/extensions/permissions.py
--rw-r--r--   0        0        0       52 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/extensions/validations.py
--rw-r--r--   0        0        0       52 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/extensions/visibilities.py
--rw-r--r--   0        0        0     2785 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/schema.py
--rw-r--r--   0        0        0        0 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/settings/__init__.py
--rw-r--r--   0        0        0     3520 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/settings/caluma.py
--rw-r--r--   0        0        0     6014 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/settings/django.py
--rw-r--r--   0        0        0      100 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/urls.py
--rw-r--r--   0        0        0     3416 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/utils.py
--rw-r--r--   0        0        0      403 2023-12-21 12:15:38.118933 caluma-9.3.2/caluma/wsgi.py
--rw-r--r--   0        0        0     4013 2023-12-21 12:15:38.118933 caluma-9.3.2/pyproject.toml
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 caluma-9.3.2/PKG-INFO
+-rw-r--r--   0        0        0    59196 2024-01-05 13:19:39.576043 caluma-9.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-01-05 13:19:39.576043 caluma-9.3.3/LICENSE
+drwxr-xr-x   0        0        0        0 2024-01-05 13:19:39.576043 caluma-9.3.3/LICENSES/
+-rw-r--r--   0        0        0     1957 2024-01-05 13:19:39.576043 caluma-9.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/__init__.py
+-rw-r--r--   0        0        0     5442 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/README.md
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/__init__.py
+-rw-r--r--   0        0        0      105 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/apps.py
+-rw-r--r--   0        0        0     3898 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/conftest.py
+-rw-r--r--   0        0        0      797 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/factories.py
+-rw-r--r--   0        0        0     1543 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/filters.py
+-rw-r--r--   0        0        0     3842 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/management/commands/run_analytics.py
+-rw-r--r--   0        0        0    11085 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2007 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py
+-rw-r--r--   0        0        0     1025 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/0003_starting_objects.py
+-rw-r--r--   0        0        0     1382 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/0004_simple_history.py
+-rw-r--r--   0        0        0      781 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/0005_analytics_field_ordering.py
+-rw-r--r--   0        0        0      631 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/0006_rename_form_slug_fields.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/migrations/__init__.py
+-rw-r--r--   0        0        0     3593 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/models.py
+-rw-r--r--   0        0        0     4082 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/pivot_table.py
+-rw-r--r--   0        0        0     7235 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/schema.py
+-rw-r--r--   0        0        0     4269 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/serializers.py
+-rw-r--r--   0        0        0    44853 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/simple_table.py
+-rw-r--r--   0        0        0    17612 2024-01-05 13:19:39.576043 caluma-9.3.3/caluma/caluma_analytics/sql.py
+-rw-r--r--   0        0        0     1401 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_analytics/visibility.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/__init__.py
+-rw-r--r--   0        0        0      975 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/apps.py
+-rw-r--r--   0        0        0      195 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/collections.py
+-rw-r--r--   0        0        0    11331 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/conftest.py
+-rw-r--r--   0        0        0     2877 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/events.py
+-rw-r--r--   0        0        0      325 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/factories.py
+-rw-r--r--   0        0        0      485 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/faker.py
+-rw-r--r--   0        0        0    19274 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/filters.py
+-rw-r--r--   0        0        0      642 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/forms.py
+-rw-r--r--   0        0        0     4176 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/health_checks.py
+-rw-r--r--   0        0        0     8071 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/jexl.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1824 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/management/commands/cleanup_history.py
+-rw-r--r--   0        0        0     3803 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/management/commands/dump_caluma_config.py
+-rw-r--r--   0        0        0      794 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/management/commands/migrate.py
+-rw-r--r--   0        0        0     4934 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py
+-rw-r--r--   0        0        0     3078 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/models.py
+-rw-r--r--   0        0        0    11674 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/mutation.py
+-rw-r--r--   0        0        0     3216 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/ordering.py
+-rw-r--r--   0        0        0     3195 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/pagination.py
+-rw-r--r--   0        0        0     4485 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/permissions.py
+-rw-r--r--   0        0        0     1253 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/relay.py
+-rw-r--r--   0        0        0     4764 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/serializers.py
+-rw-r--r--   0        0        0     7577 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/types.py
+-rw-r--r--   0        0        0      387 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/urls.py
+-rw-r--r--   0        0        0     2430 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/validations.py
+-rw-r--r--   0        0        0     1607 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/views.py
+-rw-r--r--   0        0        0     2937 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_core/visibilities.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_data_source/__init__.py
+-rw-r--r--   0        0        0      107 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_data_source/apps.py
+-rw-r--r--   0        0        0     2066 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_data_source/data_source_handlers.py
+-rw-r--r--   0        0        0     3231 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_data_source/data_sources.py
+-rw-r--r--   0        0        0     1427 2024-01-05 13:19:39.580043 caluma-9.3.3/caluma/caluma_data_source/schema.py
+-rw-r--r--   0        0        0      508 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_data_source/utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/__init__.py
+-rw-r--r--   0        0        0     2472 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/api.py
+-rw-r--r--   0        0        0      100 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/apps.py
+-rw-r--r--   0        0        0    10172 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/domain_logic.py
+-rw-r--r--   0        0        0     6287 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/factories.py
+-rw-r--r--   0        0        0    19812 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/filters.py
+-rw-r--r--   0        0        0     3283 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/format_validators.py
+-rw-r--r--   0        0        0     7830 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/historical_schema.py
+-rw-r--r--   0        0        0     7528 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/jexl.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/management/commands/__init__.py
+-rw-r--r--   0        0        0     1880 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/management/commands/copy_form.py
+-rw-r--r--   0        0        0      631 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/management/commands/create_bucket.py
+-rw-r--r--   0        0        0     1194 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/management/commands/recalculate_calc_answers.py
+-rw-r--r--   0        0        0    10983 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2829 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0002_auto_20181221_1517.py
+-rw-r--r--   0        0        0     3862 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0003_auto_20190130_0920.py
+-rw-r--r--   0        0        0     1565 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0004_auto_20190207_1405.py
+-rw-r--r--   0        0        0      825 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0005_auto_20190208_1016.py
+-rw-r--r--   0        0        0      800 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0006_choice_type_conversion.py
+-rw-r--r--   0        0        0      629 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0007_auto_20190208_1232.py
+-rw-r--r--   0        0        0     1179 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0008_auto_20190319_1720.py
+-rw-r--r--   0        0        0     2133 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0009_auto_20190321_1722.py
+-rw-r--r--   0        0        0     2302 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0010_auto_20190404_0652.py
+-rw-r--r--   0        0        0      604 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0011_auto_20190411_0607.py
+-rw-r--r--   0        0        0      788 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0012_auto_20190416_1835.py
+-rw-r--r--   0        0        0     1256 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0013_auto_20190418_0733.py
+-rw-r--r--   0        0        0     1407 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0014_auto_20190429_0910.py
+-rw-r--r--   0        0        0      659 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0015_question_format_validators.py
+-rw-r--r--   0        0        0      530 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0016_auto_20190510_0843.py
+-rw-r--r--   0        0        0      605 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0017_auto_20190619_1320.py
+-rw-r--r--   0        0        0     1859 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py
+-rw-r--r--   0        0        0      365 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0019_remove_answer_value_document.py
+-rw-r--r--   0        0        0    27839 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py
+-rw-r--r--   0        0        0     2470 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0021_auto_20190708_0905.py
+-rw-r--r--   0        0        0     1453 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py
+-rw-r--r--   0        0        0      558 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0023_auto_20190729_1448.py
+-rw-r--r--   0        0        0     1087 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0024_auto_20190919_1244.py
+-rw-r--r--   0        0        0     4834 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py
+-rw-r--r--   0        0        0      828 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0026_auto_20191031_0834.py
+-rw-r--r--   0        0        0     2087 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0027_auto_20200113_0727.py
+-rw-r--r--   0        0        0    12675 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0028_auto_20200210_0929.py
+-rw-r--r--   0        0        0     1570 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py
+-rw-r--r--   0        0        0     1281 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0030_auto_20200219_1359.py
+-rw-r--r--   0        0        0     1701 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0031_auto_20200220_0910.py
+-rw-r--r--   0        0        0     1153 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0032_auto_20200220_1311.py
+-rw-r--r--   0        0        0     1269 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0033_slugfield_length.py
+-rw-r--r--   0        0        0      518 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0034_fix_fk_lengths.py
+-rw-r--r--   0        0        0     1687 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py
+-rw-r--r--   0        0        0     1386 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0036_default_answers.py
+-rw-r--r--   0        0        0      610 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0037_default_answer_one2one.py
+-rw-r--r--   0        0        0     3050 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0038_auto_20201224_0920.py
+-rw-r--r--   0        0        0      461 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0038_remove_table_answer_value.py
+-rw-r--r--   0        0        0      283 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0039_merge_20210114_0956.py
+-rw-r--r--   0        0        0    10393 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py
+-rw-r--r--   0        0        0     2149 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0041_action_button_question.py
+-rw-r--r--   0        0        0      750 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0042_auto_20220110_1051.py
+-rw-r--r--   0        0        0     1209 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py
+-rw-r--r--   0        0        0      991 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0044_migrate_format_validators.py
+-rw-r--r--   0        0        0     5738 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0045_simple_history.py
+-rw-r--r--   0        0        0     5998 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/0046_file_answer_reverse_keys.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/migrations/__init__.py
+-rw-r--r--   0        0        0    23193 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/models.py
+-rw-r--r--   0        0        0     2213 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/ordering.py
+-rw-r--r--   0        0        0    38001 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/schema.py
+-rw-r--r--   0        0        0    23084 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/serializers.py
+-rw-r--r--   0        0        0     7471 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/signals.py
+-rw-r--r--   0        0        0     3883 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/storage_clients.py
+-rw-r--r--   0        0        0     8044 2024-01-05 13:19:39.584043 caluma-9.3.3/caluma/caluma_form/structure.py
+-rw-r--r--   0        0        0    18456 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_form/validators.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/__init__.py
+-rw-r--r--   0        0        0      103 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/apps.py
+-rw-r--r--   0        0        0      365 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/factories.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/management/commands/__init__.py
+-rw-r--r--   0        0        0     1087 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/management/commands/cleanup_access_log.py
+-rw-r--r--   0        0        0     1777 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/middleware.py
+-rw-r--r--   0        0        0     1559 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/migrations/__init__.py
+-rw-r--r--   0        0        0      657 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_logging/models.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_user/__init__.py
+-rw-r--r--   0        0        0      100 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_user/apps.py
+-rw-r--r--   0        0        0      986 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_user/models.py
+-rw-r--r--   0        0        0      667 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_user/permissions.py
+-rw-r--r--   0        0        0     3355 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_user/views.py
+-rw-r--r--   0        0        0      711 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_user/visibilities.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/__init__.py
+-rw-r--r--   0        0        0     7821 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/api.py
+-rw-r--r--   0        0        0      618 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/apps.py
+-rw-r--r--   0        0        0    21452 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/domain_logic.py
+-rw-r--r--   0        0        0     1606 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/dynamic_groups.py
+-rw-r--r--   0        0        0     1941 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/dynamic_tasks.py
+-rw-r--r--   0        0        0      533 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/events.py
+-rw-r--r--   0        0        0     2674 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/factories.py
+-rw-r--r--   0        0        0     6851 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/filters.py
+-rw-r--r--   0        0        0     6485 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/jexl.py
+-rw-r--r--   0        0        0    11029 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0001_initial.py
+-rw-r--r--   0        0        0      665 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py
+-rw-r--r--   0        0        0      755 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py
+-rw-r--r--   0        0        0     1631 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py
+-rw-r--r--   0        0        0     4268 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py
+-rw-r--r--   0        0        0      993 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py
+-rw-r--r--   0        0        0     1034 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py
+-rw-r--r--   0        0        0      686 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py
+-rw-r--r--   0        0        0     1620 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py
+-rw-r--r--   0        0        0      752 2024-01-05 13:19:39.588043 caluma-9.3.3/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py
+-rw-r--r--   0        0        0     1234 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py
+-rw-r--r--   0        0        0    21984 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py
+-rw-r--r--   0        0        0     3458 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py
+-rw-r--r--   0        0        0     1120 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py
+-rw-r--r--   0        0        0     1298 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py
+-rw-r--r--   0        0        0     2219 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py
+-rw-r--r--   0        0        0     7593 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py
+-rw-r--r--   0        0        0      924 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py
+-rw-r--r--   0        0        0      924 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0019_slugfield_length.py
+-rw-r--r--   0        0        0     2849 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0020_case_families.py
+-rw-r--r--   0        0        0     1741 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py
+-rw-r--r--   0        0        0     2503 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0022_workitem_name_description.py
+-rw-r--r--   0        0        0     1063 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py
+-rw-r--r--   0        0        0     2490 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py
+-rw-r--r--   0        0        0     1452 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py
+-rw-r--r--   0        0        0     1336 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py
+-rw-r--r--   0        0        0     6415 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py
+-rw-r--r--   0        0        0     2618 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0028_redoable_field.py
+-rw-r--r--   0        0        0      853 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0029_task_continue_async.py
+-rw-r--r--   0        0        0     3680 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py
+-rw-r--r--   0        0        0     3474 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/0031_simple_history.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/migrations/__init__.py
+-rw-r--r--   0        0        0     9946 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/models.py
+-rw-r--r--   0        0        0    12709 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/schema.py
+-rw-r--r--   0        0        0    19994 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/serializers.py
+-rw-r--r--   0        0        0     4914 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/utils.py
+-rw-r--r--   0        0        0     1892 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/validators.py
+-rw-r--r--   0        0        0     2120 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/caluma_workflow/visibilities.py
+-rw-r--r--   0        0        0    13211 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/conftest.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/__init__.py
+-rw-r--r--   0        0        0       53 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/data_sources.py
+-rw-r--r--   0        0        0       39 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/dynamic_groups.py
+-rw-r--r--   0        0        0       40 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/events.py
+-rw-r--r--   0        0        0       58 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/format_validators.py
+-rw-r--r--   0        0        0       52 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/validations.py
+-rw-r--r--   0        0        0       52 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/extensions/visibilities.py
+-rw-r--r--   0        0        0     2785 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/schema.py
+-rw-r--r--   0        0        0        0 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/settings/__init__.py
+-rw-r--r--   0        0        0     3520 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/settings/caluma.py
+-rw-r--r--   0        0        0     6014 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/settings/django.py
+-rw-r--r--   0        0        0      100 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/urls.py
+-rw-r--r--   0        0        0     3416 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/utils.py
+-rw-r--r--   0        0        0      403 2024-01-05 13:19:39.592043 caluma-9.3.3/caluma/wsgi.py
+-rw-r--r--   0        0        0     4013 2024-01-05 13:19:39.596043 caluma-9.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 caluma-9.3.3/PKG-INFO
```

### Comparing `caluma-9.3.2/CHANGELOG.md` & `caluma-9.3.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# v9.3.3 (5 January 2024)
+### Fix
+* Only save updated fields in post_complete case logic ([`eeabb02`](https://github.com/projectcaluma/caluma/commit/eeabb02b2812e50b1f279cf04bd13518f5f9872d))
+
 # v9.3.2 (21 December 2023)
 ### Fix
 * New keycloak versions omit groups in claims if no groups are set ([`d88affa`](https://github.com/projectcaluma/caluma/commit/d88affaee5129164bc034a4897b8c40bb2e1cc10))
 
 # v9.3.1 (1 September 2023)
 ### Fix
 * **migrations:** Make app prefix migration language independent ([`2f3a5d3`](https://github.com/projectcaluma/caluma/commit/2f3a5d3a86c133da531cc0204adb9d7094ff1e15))
```

### Comparing `caluma-9.3.2/LICENSE` & `caluma-9.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/README.md` & `caluma-9.3.3/README.md`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/README.md` & `caluma-9.3.3/caluma/caluma_analytics/README.md`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/conftest.py` & `caluma-9.3.3/caluma/caluma_analytics/conftest.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/factories.py` & `caluma-9.3.3/caluma/caluma_analytics/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/filters.py` & `caluma-9.3.3/caluma/caluma_analytics/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/management/commands/run_analytics.py` & `caluma-9.3.3/caluma/caluma_analytics/management/commands/run_analytics.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/migrations/0001_initial.py` & `caluma-9.3.3/caluma/caluma_analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py` & `caluma-9.3.3/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/migrations/0003_starting_objects.py` & `caluma-9.3.3/caluma/caluma_analytics/migrations/0003_starting_objects.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/migrations/0004_simple_history.py` & `caluma-9.3.3/caluma/caluma_analytics/migrations/0004_simple_history.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/migrations/0005_analytics_field_ordering.py` & `caluma-9.3.3/caluma/caluma_analytics/migrations/0005_analytics_field_ordering.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/migrations/0006_rename_form_slug_fields.py` & `caluma-9.3.3/caluma/caluma_analytics/migrations/0006_rename_form_slug_fields.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/models.py` & `caluma-9.3.3/caluma/caluma_analytics/models.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/pivot_table.py` & `caluma-9.3.3/caluma/caluma_analytics/pivot_table.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/schema.py` & `caluma-9.3.3/caluma/caluma_analytics/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/serializers.py` & `caluma-9.3.3/caluma/caluma_analytics/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/simple_table.py` & `caluma-9.3.3/caluma/caluma_analytics/simple_table.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/sql.py` & `caluma-9.3.3/caluma/caluma_analytics/sql.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_analytics/visibility.py` & `caluma-9.3.3/caluma/caluma_analytics/visibility.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/apps.py` & `caluma-9.3.3/caluma/caluma_core/apps.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/conftest.py` & `caluma-9.3.3/caluma/caluma_core/conftest.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/events.py` & `caluma-9.3.3/caluma/caluma_core/events.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/filters.py` & `caluma-9.3.3/caluma/caluma_core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/forms.py` & `caluma-9.3.3/caluma/caluma_core/forms.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/health_checks.py` & `caluma-9.3.3/caluma/caluma_core/health_checks.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/jexl.py` & `caluma-9.3.3/caluma/caluma_core/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/management/commands/cleanup_history.py` & `caluma-9.3.3/caluma/caluma_core/management/commands/cleanup_history.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/management/commands/dump_caluma_config.py` & `caluma-9.3.3/caluma/caluma_core/management/commands/dump_caluma_config.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/management/commands/migrate.py` & `caluma-9.3.3/caluma/caluma_core/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py` & `caluma-9.3.3/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/models.py` & `caluma-9.3.3/caluma/caluma_core/models.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/mutation.py` & `caluma-9.3.3/caluma/caluma_core/mutation.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/ordering.py` & `caluma-9.3.3/caluma/caluma_core/ordering.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/pagination.py` & `caluma-9.3.3/caluma/caluma_core/pagination.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/permissions.py` & `caluma-9.3.3/caluma/caluma_core/permissions.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/relay.py` & `caluma-9.3.3/caluma/caluma_core/relay.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/serializers.py` & `caluma-9.3.3/caluma/caluma_core/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/types.py` & `caluma-9.3.3/caluma/caluma_core/types.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/validations.py` & `caluma-9.3.3/caluma/caluma_core/validations.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/views.py` & `caluma-9.3.3/caluma/caluma_core/views.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_core/visibilities.py` & `caluma-9.3.3/caluma/caluma_core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_data_source/data_source_handlers.py` & `caluma-9.3.3/caluma/caluma_data_source/data_source_handlers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_data_source/data_sources.py` & `caluma-9.3.3/caluma/caluma_data_source/data_sources.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_data_source/schema.py` & `caluma-9.3.3/caluma/caluma_data_source/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/api.py` & `caluma-9.3.3/caluma/caluma_form/api.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/domain_logic.py` & `caluma-9.3.3/caluma/caluma_form/domain_logic.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/factories.py` & `caluma-9.3.3/caluma/caluma_form/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/filters.py` & `caluma-9.3.3/caluma/caluma_form/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/format_validators.py` & `caluma-9.3.3/caluma/caluma_form/format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/historical_schema.py` & `caluma-9.3.3/caluma/caluma_form/historical_schema.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/jexl.py` & `caluma-9.3.3/caluma/caluma_form/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/management/commands/copy_form.py` & `caluma-9.3.3/caluma/caluma_form/management/commands/copy_form.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/management/commands/create_bucket.py` & `caluma-9.3.3/caluma/caluma_form/management/commands/create_bucket.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/management/commands/recalculate_calc_answers.py` & `caluma-9.3.3/caluma/caluma_form/management/commands/recalculate_calc_answers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0001_initial.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0002_auto_20181221_1517.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0002_auto_20181221_1517.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0003_auto_20190130_0920.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0003_auto_20190130_0920.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0004_auto_20190207_1405.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0004_auto_20190207_1405.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0005_auto_20190208_1016.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0005_auto_20190208_1016.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0006_choice_type_conversion.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0006_choice_type_conversion.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0007_auto_20190208_1232.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0007_auto_20190208_1232.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0008_auto_20190319_1720.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0008_auto_20190319_1720.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0009_auto_20190321_1722.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0009_auto_20190321_1722.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0010_auto_20190404_0652.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0010_auto_20190404_0652.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0011_auto_20190411_0607.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0011_auto_20190411_0607.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0012_auto_20190416_1835.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0012_auto_20190416_1835.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0013_auto_20190418_0733.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0013_auto_20190418_0733.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0014_auto_20190429_0910.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0014_auto_20190429_0910.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0015_question_format_validators.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0015_question_format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0016_auto_20190510_0843.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0016_auto_20190510_0843.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0017_auto_20190619_1320.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0017_auto_20190619_1320.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0021_auto_20190708_0905.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0021_auto_20190708_0905.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0023_auto_20190729_1448.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0023_auto_20190729_1448.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0024_auto_20190919_1244.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0024_auto_20190919_1244.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0026_auto_20191031_0834.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0026_auto_20191031_0834.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0027_auto_20200113_0727.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0027_auto_20200113_0727.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0028_auto_20200210_0929.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0028_auto_20200210_0929.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0030_auto_20200219_1359.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0030_auto_20200219_1359.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0031_auto_20200220_0910.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0031_auto_20200220_0910.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0032_auto_20200220_1311.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0032_auto_20200220_1311.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0033_slugfield_length.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0033_slugfield_length.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0034_fix_fk_lengths.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0034_fix_fk_lengths.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0036_default_answers.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0036_default_answers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0037_default_answer_one2one.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0037_default_answer_one2one.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0038_auto_20201224_0920.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0038_auto_20201224_0920.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0041_action_button_question.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0041_action_button_question.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0042_auto_20220110_1051.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0042_auto_20220110_1051.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0044_migrate_format_validators.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0044_migrate_format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0045_simple_history.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0045_simple_history.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/migrations/0046_file_answer_reverse_keys.py` & `caluma-9.3.3/caluma/caluma_form/migrations/0046_file_answer_reverse_keys.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/models.py` & `caluma-9.3.3/caluma/caluma_form/models.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/ordering.py` & `caluma-9.3.3/caluma/caluma_form/ordering.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/schema.py` & `caluma-9.3.3/caluma/caluma_form/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/serializers.py` & `caluma-9.3.3/caluma/caluma_form/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/signals.py` & `caluma-9.3.3/caluma/caluma_form/signals.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/storage_clients.py` & `caluma-9.3.3/caluma/caluma_form/storage_clients.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/structure.py` & `caluma-9.3.3/caluma/caluma_form/structure.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_form/validators.py` & `caluma-9.3.3/caluma/caluma_form/validators.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_logging/management/commands/cleanup_access_log.py` & `caluma-9.3.3/caluma/caluma_logging/management/commands/cleanup_access_log.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_logging/middleware.py` & `caluma-9.3.3/caluma/caluma_logging/middleware.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_logging/migrations/0001_initial.py` & `caluma-9.3.3/caluma/caluma_logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_logging/models.py` & `caluma-9.3.3/caluma/caluma_logging/models.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_user/models.py` & `caluma-9.3.3/caluma/caluma_user/models.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_user/permissions.py` & `caluma-9.3.3/caluma/caluma_user/permissions.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_user/views.py` & `caluma-9.3.3/caluma/caluma_user/views.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_user/visibilities.py` & `caluma-9.3.3/caluma/caluma_user/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/api.py` & `caluma-9.3.3/caluma/caluma_workflow/api.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/apps.py` & `caluma-9.3.3/caluma/caluma_workflow/apps.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/domain_logic.py` & `caluma-9.3.3/caluma/caluma_workflow/domain_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,22 @@
             ).exists()
         ):
             # no more tasks, mark case as complete
             case.status = models.Case.STATUS_COMPLETED
             case.closed_at = timezone.now()
             case.closed_by_user = user.username
             case.closed_by_group = user.group
-            case.save()
+            case.save(
+                update_fields=[
+                    "status",
+                    "closed_at",
+                    "closed_by_user",
+                    "closed_by_group",
+                ]
+            )
 
             send_event(
                 events.post_complete_case,
                 sender=sender,
                 case=case,
                 user=user,
                 context=context,
```

### Comparing `caluma-9.3.2/caluma/caluma_workflow/dynamic_groups.py` & `caluma-9.3.3/caluma/caluma_workflow/dynamic_groups.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/dynamic_tasks.py` & `caluma-9.3.3/caluma/caluma_workflow/dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/events.py` & `caluma-9.3.3/caluma/caluma_workflow/events.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/factories.py` & `caluma-9.3.3/caluma/caluma_workflow/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/filters.py` & `caluma-9.3.3/caluma/caluma_workflow/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/jexl.py` & `caluma-9.3.3/caluma/caluma_workflow/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0001_initial.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0019_slugfield_length.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0019_slugfield_length.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0020_case_families.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0020_case_families.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0022_workitem_name_description.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0022_workitem_name_description.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0028_redoable_field.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0028_redoable_field.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0029_task_continue_async.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0029_task_continue_async.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/migrations/0031_simple_history.py` & `caluma-9.3.3/caluma/caluma_workflow/migrations/0031_simple_history.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/models.py` & `caluma-9.3.3/caluma/caluma_workflow/models.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/schema.py` & `caluma-9.3.3/caluma/caluma_workflow/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/serializers.py` & `caluma-9.3.3/caluma/caluma_workflow/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/utils.py` & `caluma-9.3.3/caluma/caluma_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/validators.py` & `caluma-9.3.3/caluma/caluma_workflow/validators.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/caluma_workflow/visibilities.py` & `caluma-9.3.3/caluma/caluma_workflow/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/conftest.py` & `caluma-9.3.3/caluma/conftest.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/schema.py` & `caluma-9.3.3/caluma/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/settings/caluma.py` & `caluma-9.3.3/caluma/settings/caluma.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/settings/django.py` & `caluma-9.3.3/caluma/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/caluma/utils.py` & `caluma-9.3.3/caluma/utils.py`

 * *Files identical despite different names*

### Comparing `caluma-9.3.2/pyproject.toml` & `caluma-9.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma"
-version = "9.3.2"
+version = "9.3.3"
 description = "Caluma Service providing GraphQL API"
 homepage = "https://caluma.io"
 repository = "https://github.com/projectcaluma/caluma"
 documentation = "https://caluma.gitbook.io/"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
```

### Comparing `caluma-9.3.2/PKG-INFO` & `caluma-9.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma
-Version: 9.3.2
+Version: 9.3.3
 Summary: Caluma Service providing GraphQL API
 Home-page: https://caluma.io
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

