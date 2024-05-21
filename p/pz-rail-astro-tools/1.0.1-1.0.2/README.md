# Comparing `tmp/pz_rail_astro_tools-1.0.1.tar.gz` & `tmp/pz_rail_astro_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_astro_tools-1.0.1.tar", last modified: Fri May 17 18:43:56 2024, max compression
+gzip compressed data, was "pz_rail_astro_tools-1.0.2.tar", last modified: Tue May 21 17:31:20 2024, max compression
```

## Comparing `pz_rail_astro_tools-1.0.1.tar` & `pz_rail_astro_tools-1.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 18:43:56.000000 pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/astro_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 18:43:55.000000 pz_rail_astro_tools-1.0.1/src/rail/astro_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/grid_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/observing_condition_degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/photometric_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_selections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/creation/engines/gcr_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.268702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.292702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    25884 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/examples_data/testdata/rubin_dm_dc2_example2.pq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/src/rail/tools/photometry_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.264702 pz_rail_astro_tools-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/tests/astro_tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:43:56.296702 pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-17 18:43:50.000000 pz_rail_astro_tools-1.0.1/tests/astro_tools/test_gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.288578 pz_rail_astro_tools-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.256578 pz_rail_astro_tools-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.256578 pz_rail_astro_tools-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-21 17:31:20.288578 pz_rail_astro_tools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:31:20.288578 pz_rail_astro_tools-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.284578 pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-21 17:31:20.000000 pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-21 17:31:20.000000 pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:31:20.000000 pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-21 17:31:20.000000 pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 17:31:20.000000 pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.256578 pz_rail_astro_tools-1.0.2/src/rail/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/astro_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 17:31:19.000000 pz_rail_astro_tools-1.0.2/src/rail/astro_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.256578 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/grid_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/observing_condition_degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/photometric_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/spectroscopic_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/spectroscopic_selections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.256578 pz_rail_astro_tools-1.0.2/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/creation/engines/gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.260578 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.280578 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.284578 pz_rail_astro_tools-1.0.2/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    25884 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/examples_data/testdata/rubin_dm_dc2_example2.pq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.284578 pz_rail_astro_tools-1.0.2/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    19216 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/src/rail/tools/photometry_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.252578 pz_rail_astro_tools-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.284578 pz_rail_astro_tools-1.0.2/tests/astro_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:20.284578 pz_rail_astro_tools-1.0.2/tests/astro_tools/gcr_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/tests/astro_tools/gcr_test_data/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/tests/astro_tools/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/tests/astro_tools/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-21 17:31:14.000000 pz_rail_astro_tools-1.0.2/tests/astro_tools/test_gcr_engine.py
```

### Comparing `pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_astro_tools-1.0.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_astro_tools-1.0.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.github/pull_request_template.md` & `pz_rail_astro_tools-1.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.github/workflows/linting.yml` & `pz_rail_astro_tools-1.0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.github/workflows/publish-to-pypi.yml` & `pz_rail_astro_tools-1.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.github/workflows/smoke-test.yml` & `pz_rail_astro_tools-1.0.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.github/workflows/testing-and-coverage.yml` & `pz_rail_astro_tools-1.0.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.gitignore` & `pz_rail_astro_tools-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/.pre-commit-config.yaml` & `pz_rail_astro_tools-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/LICENSE` & `pz_rail_astro_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/PKG-INFO` & `pz_rail_astro_tools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 1.0.1
+Version: 1.0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_astro_tools-1.0.1/README.md` & `pz_rail_astro_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/pyproject.toml` & `pz_rail_astro_tools-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/PKG-INFO` & `pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 1.0.1
+Version: 1.0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_astro_tools-1.0.1/src/pz_rail_astro_tools.egg-info/SOURCES.txt` & `pz_rail_astro_tools-1.0.2/src/pz_rail_astro_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/grid_selection.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/grid_selection.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/lsst_error_model.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/observing_condition_degrader.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/observing_condition_degrader.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/photometric_errors.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/photometric_errors.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_degraders.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/spectroscopic_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/degraders/spectroscopic_selections.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/degraders/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/creation/engines/gcr_engine.py` & `pz_rail_astro_tools-1.0.2/src/rail/creation/engines/gcr_engine.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5` & `pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits` & `pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits` & `pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-1.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/examples_data/testdata/rubin_dm_dc2_example2.pq` & `pz_rail_astro_tools-1.0.2/src/rail/examples_data/testdata/rubin_dm_dc2_example2.pq`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/src/rail/tools/photometry_tools.py` & `pz_rail_astro_tools-1.0.2/src/rail/tools/photometry_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import tables_io
 from astropy.coordinates import SkyCoord
 
 from ceci.config import StageParameter as Param
 from rail.core.data import PqHandle
 from rail.core.stage import RailStage
 from rail.core.data import PqHandle, Hdf5Handle
+from rail.core.common_params import SHARED_PARAMS
 
 import hyperbolic  # https://github.com/jlvdb/hyperbolic
 
 dustmaps_config = tables_io.lazy_modules.lazyImport('dustmaps.config')
 dustmaps_sfd = tables_io.lazy_modules.lazyImport('dustmaps.sfd')
 
 
@@ -327,15 +328,15 @@
 
         Parameters
         ----------
         data : `PqHandle`
             Input table with photometry (magnitudes or flux columns and their respective
             uncertainties) as defined by the configuration.
         parameters : `PqHandle`
-            Table with smoothing parameters per photometric band, determined by
+            Table witdh smoothing parameters per photometric band, determined by
             `HyperbolicSmoothing`.
 
         Returns
         -------
         output: `PqHandle`
             Output table containting hyperbolic magnitudes and their uncertainties. If the columns
             in the input table contain a prefix `mag_`, this output tabel will replace the prefix
@@ -416,14 +417,16 @@
     Note: set copy_all_cols=True to copy all 
     columns in data, copy_cols will be ignored
     """
     name = 'DustMapBase'
 
     config_options = RailStage.config_options.copy()
     config_options.update(bands='ugrizy')
+    config_options.update(ra_name='ra')
+    config_options.update(dec_name='dec')
     config_options.update(mag_name="mag_{band}_lsst")
     config_options.update(band_a_env=[4.81,3.64,2.70,2.06,1.58,1.31])
     config_options.update(dustmap_name='sfd')
     config_options.update(dustmap_dir=str)
     config_options.update(copy_cols=[])
     config_options.update(copy_all_cols=False)
 
@@ -452,15 +455,15 @@
             
     def __init__(self, args, comm=None):
         RailStage.__init__(self, args, comm=comm)
 
     def run(self):
         data = self.get_data('input', allow_missing=True)
         out_data = {}
-        coords = SkyCoord(data['ra'], data['dec'], unit = 'deg',frame='fk5')
+        coords = SkyCoord(data[self.config.ra_name], data[self.config.dec_name], unit = 'deg',frame='fk5')
         dust_map_dict = dict(sfd=dustmaps_sfd.SFDQuery)
         try:
             dust_map_class = dust_map_dict[self.config.dustmap_name]
             dust_map_config = dustmaps_config.config
             dust_map_config['data_dir'] = self.config.dustmap_dir
             dust_map = dust_map_class()
         except KeyError as msg:  # pragma: no cover
```

### Comparing `pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/schema.yaml` & `pz_rail_astro_tools-1.0.2/tests/astro_tools/gcr_test_data/schema.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5` & `pz_rail_astro_tools-1.0.2/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/tests/astro_tools/test_core.py` & `pz_rail_astro_tools-1.0.2/tests/astro_tools/test_core.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/tests/astro_tools/test_degraders.py` & `pz_rail_astro_tools-1.0.2/tests/astro_tools/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-1.0.1/tests/astro_tools/test_gcr_engine.py` & `pz_rail_astro_tools-1.0.2/tests/astro_tools/test_gcr_engine.py`

 * *Files identical despite different names*

