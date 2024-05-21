# Comparing `tmp/kohlrahbi-1.1.1.tar.gz` & `tmp/kohlrahbi-1.1.2.tar.gz`

## Comparing `kohlrahbi-1.1.1.tar` & `kohlrahbi-1.1.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.gitattributes
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/README.md
--rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/kohlrahbi-image.png
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/requirements.txt
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/tox.ini
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/wip.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxfilefinder.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/table_header.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/version.py
--rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahb/command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/__init__.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbcondtions.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbpackagetable.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbsubtable.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtable.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtablerow.py
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/changehistory/__init__.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/changehistory/changehistorytable.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/changehistory/command.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/conditions/__init__.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/conditions/command.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/ahbexportfileformat.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
--rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
--rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
--rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
--rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/LICENSE
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.gitattributes
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/README.md
+-rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/kohlrahbi-image.png
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/requirements.txt
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/tox.ini
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/wip.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/docxfilefinder.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/table_header.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/version.py
+-rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahb/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/__init__.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbcondtions.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbpackagetable.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbsubtable.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbtable.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbtablerow.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/changehistory/__init__.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/changehistory/changehistorytable.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/changehistory/command.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/conditions/__init__.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/conditions/command.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/enums/ahbexportfileformat.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
+-rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
+-rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
+-rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
+-rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 kohlrahbi-1.1.2/PKG-INFO
```

### Comparing `kohlrahbi-1.1.1/.pre-commit-config.yaml` & `kohlrahbi-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/README.md` & `kohlrahbi-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/kohlrahbi-image.png` & `kohlrahbi-1.1.2/kohlrahbi-image.png`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/requirements.txt` & `kohlrahbi-1.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/tox.ini` & `kohlrahbi-1.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/wip.md` & `kohlrahbi-1.1.2/wip.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/dependabot.yml` & `kohlrahbi-1.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/coverage.yml` & `kohlrahbi-1.1.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/dependabot_automerge.yml` & `kohlrahbi-1.1.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/formatting.yml` & `kohlrahbi-1.1.2/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/packaging_test.yml` & `kohlrahbi-1.1.2/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/python-publish.yml` & `kohlrahbi-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/pythonlint.yml` & `kohlrahbi-1.1.2/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.github/workflows/unittests.yml` & `kohlrahbi-1.1.2/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/dev_requirements/requirements-test_packaging.txt` & `kohlrahbi-1.1.2/dev_requirements/requirements-test_packaging.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/dev_requirements/requirements-tests.txt` & `kohlrahbi-1.1.2/dev_requirements/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/dev_requirements/requirements-type_check.txt` & `kohlrahbi-1.1.2/dev_requirements/requirements-type_check.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/__init__.py` & `kohlrahbi-1.1.2/src/kohlrahbi/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/docxfilefinder.py` & `kohlrahbi-1.1.2/src/kohlrahbi/docxfilefinder.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/read_functions.py` & `kohlrahbi-1.1.2/src/kohlrahbi/read_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     searched_pruefi_is_found: bool,
     ahb_table: AhbTable | None,
     seed: Seed | None = None,
 ) -> tuple[bool, AhbTable]:
     """Processes tables to find and build the AHB table."""
     if is_item_table_with_pruefidentifikatoren(item):
         seed = Seed.from_table(docx_table=item)
-
+        # pylint:disable=unsupported-membership-test
         if pruefi in seed.pruefidentifikatoren and not searched_pruefi_is_found:
             log_found_pruefi(pruefi)
             ahb_sub_table = AhbSubTable.from_table_with_header(docx_table=item)
             ahb_table = AhbTable.from_ahb_sub_table(ahb_sub_table=ahb_sub_table)
             searched_pruefi_is_found = True
 
     elif is_item_headless_table((item, ahb_table)):
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-1.1.2/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/seed.py` & `kohlrahbi-1.1.2/src/kohlrahbi/seed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 This module provides a class to collect information which of need for all parsing functions
 """
 
 from docx.table import Table
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from kohlrahbi.enums import RowType
 from kohlrahbi.table_header import PruefiMetaData, TableHeader, get_tabstop_positions
 
 
 # pylint: disable=too-few-public-methods
 class Seed(BaseModel):
     """
     helper class to store all values to extract the AHB and the final AHB as dataframe
     """
 
-    pruefidentifikatoren: list[str] = []
-    column_headers: list[str] = []
+    pruefidentifikatoren: list[str] = Field(default_factory=list)
+    column_headers: list[str] = Field(default_factory=list)
     edifact_struktur_left_indent_position: int = 0
     middle_cell_left_indent_position: int = 0
-    tabstop_positions: list[int] = []
-    last_two_row_types: list[RowType] = []
-    metadata: list[PruefiMetaData] = []
+    tabstop_positions: list[int] = Field(default_factory=list)
+    last_two_row_types: list[RowType] = Field(default_factory=list)
+    metadata: list[PruefiMetaData] = Field(default_factory=list)
 
     # why this classmethod?
     # to decouple the data structure of Elixir from the input data
     # more information can be found on https://www.attrs.org/en/stable/init.html#initialization
     @classmethod
     def from_table(cls, docx_table: Table) -> "Seed":
         """Prepare DataFrame for a new table with new Prüfidentifikatoren
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/table_header.py` & `kohlrahbi-1.1.2/src/kohlrahbi/table_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from enum import StrEnum
 from typing import Dict, List, Mapping, cast
 
 from docx.table import _Cell
 from docx.text.paragraph import Paragraph
 from more_itertools import first, last
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class HeaderSection(StrEnum):
     """
     Enum for the different sections of the table header
     """
 
@@ -89,15 +89,15 @@
 
 class TableHeader(BaseModel):
     """
     Class for the table header.
     It contains the information about the Prüfidentifikatoren.
     """
 
-    pruefi_meta_data: List[PruefiMetaData] = []
+    pruefi_meta_data: List[PruefiMetaData] = Field(default_factory=list)
 
     @classmethod
     def from_header_cell(cls, row_cell: _Cell) -> "TableHeader":
         """
         Create a TableHeader instance from a list of strings.
         """
 
@@ -184,8 +184,9 @@
 
     def get_pruefidentifikatoren(self) -> List[str]:
         """
         Get all Prüfidentifikatoren from the table header.
         The order of the Prüfidentifikatoren is the same as in the docx table headers.
         So there should be no duplicates.
         """
+        # pylint:disable=not-an-iterable
         return [pruefi.pruefidentifikator for pruefi in self.pruefi_meta_data]
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahb/__init__.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains the functions to scrape the AHBs for Pruefidentifikatoren.
 """
 
 import fnmatch
+import gc
 import re
 from datetime import date
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import click
 import docx
@@ -43,27 +44,28 @@
     return pruefi_docx_file_map
 
 
 def process_ahb_table(
     ahb_table: AhbTable,
     pruefi: str,
     output_path: Path,
-    file_type: str,
+    file_type: tuple[AhbExportFileFormat, ...],
 ) -> None:
     """
     Process the ahb table.
     """
     unfolded_ahb = UnfoldedAhb.from_ahb_table(ahb_table=ahb_table, pruefi=pruefi)
 
-    if "xlsx" in file_type:
+    if AhbExportFileFormat.XLSX in file_type:
         unfolded_ahb.dump_xlsx(output_path)
-    if "flatahb" in file_type:
+    if AhbExportFileFormat.FLATAHB in file_type:
         unfolded_ahb.dump_flatahb_json(output_path)
-    if "csv" in file_type:
+    if AhbExportFileFormat.CSV in file_type:
         unfolded_ahb.dump_csv(output_path)
+    del unfolded_ahb
 
 
 # pylint:disable=anomalous-backslash-in-string
 def get_valid_pruefis(list_of_pruefis: list[str], all_known_pruefis: Optional[list[str]] = None) -> list[str]:
     """
     This function returns a list with only those pruefis which match the pruefi_pattern "^[1-9]\\d{4}$".
     It also supports unix wildcards like '*' and '?' if a list of known pruefis is given.
@@ -88,20 +90,19 @@
     valid_pruefis = get_valid_pruefis(pruefis)
     if not valid_pruefis:
         click.secho("⚠️ There are no valid pruefidentifkatoren.", fg="red")
         raise click.Abort()
     return valid_pruefis
 
 
-# pylint: disable=too-many-arguments
 def process_pruefi(
     pruefi: str,
     path_to_ahb_docx_file: Path,
     output_path: Path,
-    file_type: str,
+    file_type: tuple[AhbExportFileFormat, ...],
 ) -> None:
     """
     Process one pruefi.
     If the input path ends with .docx, we assume that the file containing the pruefi is given.
     Therefore we only access that file.
     """
 
@@ -112,14 +113,18 @@
         return
 
     ahb_table = get_ahb_table(document=doc, pruefi=pruefi)
     if not ahb_table:
         return
 
     process_ahb_table(ahb_table, pruefi, output_path, file_type)
+    del ahb_table.table
+    del ahb_table
+    del doc
+    gc.collect()
 
 
 def get_ahb_documents_path(base_path: Path, version: str) -> Path:
     """Returns the path to the AHB documents for the specified format version."""
     path = base_path / f"edi_energy_de/{version}"
     if not path.exists():
         raise FileNotFoundError(f"The specified path {path.absolute()} does not exist.")
@@ -144,14 +149,15 @@
     pruefis: dict[str, str] = {}
     for item in get_all_paragraphs_and_tables(doc):
         if (
             isinstance(item, Table)
             and table_header_starts_with_text_edifact_struktur(item)
             and table_header_contains_text_pruefidentifikator(item)
         ):
+            # pylint:disable=not-an-iterable
             pruefis.update({pruefi: docx_path.name for pruefi in extract_pruefis_from_table(item)})
     return pruefis
 
 
 def save_pruefi_map_to_toml(pruefis: Dict[str, str], version: str) -> None:
     """Saves the pruefis to file mapping to a toml file."""
     output_filename = f"{version}_pruefi_docx_filename_map.toml"
@@ -210,15 +216,15 @@
     return {pruefi: filename for pruefi, filename in pruefi_to_file_mapping.items() if pruefi in pruefis}
 
 
 def scrape_pruefis(
     pruefis: list[str],
     basic_input_path: Path,
     output_path: Path,
-    file_type: AhbExportFileFormat,
+    file_type: tuple[AhbExportFileFormat, ...],
     format_version: EdifactFormatVersion,
 ) -> None:
     """
     starts the scraping process for provided pruefi_to_file_mappings
     """
     pruefi_to_file_mapping = get_pruefi_to_file_mapping(
         basic_input_path=basic_input_path, format_version=format_version
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahb/command.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahb/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     help="Confirm all prompts automatically.",
 )
 # pylint: disable=too-many-arguments
 def ahb(
     pruefis: list[str],
     edi_energy_mirror_path: Path,
     output_path: Path,
-    file_type: AhbExportFileFormat,
+    file_type: tuple[AhbExportFileFormat, ...],
     format_version: EdifactFormatVersion | str,
     assume_yes: bool,  # pylint: disable=unused-argument
     # it is used by the callback function of the output-path
 ) -> None:
     """
     Scrape AHB documents for pruefidentifikatoren.
     This is a command line interface for the pruefis module.
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbcondtions.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbcondtions.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import json
 import re
 from pathlib import Path
 
 from docx.table import Table as DocxTable
 from maus.edifact import EdifactFormat
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 
 from kohlrahbi.logger import logger
 
 
 class AhbConditions(BaseModel):
     """
     Class which contains a dict of conditions for each edifact format
     """
 
-    conditions_dict: dict[EdifactFormat, dict[str, str]] = {}
+    conditions_dict: dict[EdifactFormat, dict[str, str]] = Field(default_factory=dict)
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     @classmethod
     def from_docx_table(cls, docx_tables: list[DocxTable], edifact_format: EdifactFormat) -> "AhbConditions":
         """
         Create an AhbPackageTable object from a docx table.
@@ -56,32 +56,37 @@
     def include_condition_dict(self, to_add: dict[EdifactFormat, dict[str, str]] | None) -> None:
         """ " Include a dict of conditions to the conditions_dict"""
         if to_add is None:
             logger.info("Conditions dict to be added is empty.")
             return
         for edifact_format, edi_cond_dict in to_add.items():
             for condition_key, condition_text in edi_cond_dict.items():
-                if edifact_format in self.conditions_dict:
+                if edifact_format in self.conditions_dict:  # pylint:disable=unsupported-membership-test
                     if (
+                        # pylint:disable=unsubscriptable-object
                         condition_key in self.conditions_dict[edifact_format]
                         and len(condition_text) > len(self.conditions_dict[edifact_format][condition_key])
+                        # pylint:disable=unsubscriptable-object
                         or condition_key not in self.conditions_dict[edifact_format]
                     ):
                         self.conditions_dict[edifact_format][condition_key] = condition_text
                 else:
-                    self.conditions_dict[edifact_format] = {condition_key: condition_text}
+                    self.conditions_dict[edifact_format] = {  # pylint:disable=unsupported-assignment-operation
+                        condition_key: condition_text
+                    }
 
         logger.info("Conditions were updated.")
 
     def dump_as_json(self, output_directory_path: Path) -> None:
         """
         Writes all collected conditions to a json file.
         The file will be stored in the directory:
             'output_directory_path/<edifact_format>/conditions.json'
         """
+        # pylint:disable=no-member
         for edifact_format, format_cond_dict in self.conditions_dict.items():
             condition_json_output_directory_path = output_directory_path / str(edifact_format)
             condition_json_output_directory_path.mkdir(parents=True, exist_ok=True)
             file_path = condition_json_output_directory_path / "conditions.json"
             # resort ConditionKeyConditionTextMappings for output
             sorted_condition_dict = {k: format_cond_dict[k] for k in sorted(format_cond_dict, key=int)}
             array = [
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbpackagetable.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbpackagetable.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 import json
 import re
 from pathlib import Path
 
 import pandas as pd
 from docx.table import Table as DocxTable
 from maus.edifact import EdifactFormat
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 
 from kohlrahbi.ahbtable.ahbcondtions import parse_conditions_from_string
 from kohlrahbi.logger import logger
 
 
 class AhbPackageTable(BaseModel):
     """
     This class contains the AHB Package table as you see it in the beginning AHB documents,
     but in a machine readable format.
     Caution: if two PackageTables objects are combined so far only the package_dict field is updated.
     """
 
     table: pd.DataFrame = pd.DataFrame()
-    package_dict: dict[EdifactFormat, dict[str, str]] = {}
+    package_dict: dict[EdifactFormat, dict[str, str]] = Field(default_factory=dict)
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     @classmethod
     def from_docx_table(cls, docx_tables: list[DocxTable]) -> "AhbPackageTable":
         """
         Create an AhbPackageTable object from a docx table.
         """
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbsubtable.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtable.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbtable.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pathlib import Path
 from typing import Union
 
 import pandas as pd
 from maus.edifact import get_format_of_pruefidentifikator
 from more_itertools import peekable
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 
 from kohlrahbi.ahbtable.ahbsubtable import AhbSubTable
 from kohlrahbi.logger import logger
 from kohlrahbi.table_header import PruefiMetaData
 
 _column_letter_width_mapping: dict[str, Union[float, int]] = {
     "A": 3.5,
@@ -28,15 +28,15 @@
 
 class AhbTable(BaseModel):
     """
     This class contains the AHB table as you see it in the AHB documents, but in a machine readable format.
     """
 
     table: pd.DataFrame
-    metadata: list[PruefiMetaData] = []
+    metadata: list[PruefiMetaData] = Field(default_factory=list)
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def fill_segment_gruppe_segment_dataelement(self) -> None:
         """
         For easier readability this functions adds the segment
```

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtablerow.py` & `kohlrahbi-1.1.2/src/kohlrahbi/ahbtable/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/changehistory/__init__.py` & `kohlrahbi-1.1.2/src/kohlrahbi/changehistory/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/changehistory/changehistorytable.py` & `kohlrahbi-1.1.2/src/kohlrahbi/changehistory/changehistorytable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/changehistory/command.py` & `kohlrahbi-1.1.2/src/kohlrahbi/changehistory/command.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/conditions/__init__.py` & `kohlrahbi-1.1.2/src/kohlrahbi/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/conditions/command.py` & `kohlrahbi-1.1.2/src/kohlrahbi/conditions/command.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-1.1.2/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-1.1.2/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml` & `kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml` & `kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml` & `kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml` & `kohlrahbi-1.1.2/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-1.1.2/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-1.1.2/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/.gitignore` & `kohlrahbi-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/LICENSE` & `kohlrahbi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/pyproject.toml` & `kohlrahbi-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.1/PKG-INFO` & `kohlrahbi-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kohlrahbi
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
```

