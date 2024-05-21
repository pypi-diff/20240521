# Comparing `tmp/baybe-0.8.2.tar.gz` & `tmp/baybe-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baybe-0.8.2.tar", last modified: Wed Mar 27 11:28:11 2024, max compression
+gzip compressed data, was "baybe-0.9.0.tar", last modified: Tue May 21 18:54:37 2024, max compression
```

## Comparing `baybe-0.8.2.tar` & `baybe-0.9.0.tar`

### file list

```diff
@@ -1,273 +1,328 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.998840 baybe-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 11:27:50.000000 baybe-0.8.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.950840 baybe-0.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 11:27:50.000000 baybe-0.8.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.950840 baybe-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-03-27 11:27:50.000000 baybe-0.8.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-27 11:27:50.000000 baybe-0.8.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-03-27 11:27:50.000000 baybe-0.8.2/.github/workflows/regular.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-27 11:27:50.000000 baybe-0.8.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-27 11:27:50.000000 baybe-0.8.2/.github/workflows/reminders.yml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-27 11:27:50.000000 baybe-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-27 11:27:50.000000 baybe-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-03-27 11:27:50.000000 baybe-0.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-03-27 11:27:50.000000 baybe-0.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-27 11:27:50.000000 baybe-0.8.2/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-03-27 11:27:50.000000 baybe-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17196 2024-03-27 11:28:10.998840 baybe-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-03-27 11:27:50.000000 baybe-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.954840 baybe-0.8.2/baybe/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/campaign.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.954840 baybe-0.8.2/baybe/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/constraints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/constraints/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/constraints/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/constraints/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/constraints/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.958840 baybe-0.8.2/baybe/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/substance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/parameters/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.958840 baybe-0.8.2/baybe/recommenders/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.958840 baybe-0.8.2/baybe/recommenders/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/meta/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/meta/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/naive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.958840 baybe-0.8.2/baybe/recommenders/pure/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.958840 baybe-0.8.2/baybe/recommenders/pure/bayesian/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/bayesian/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/bayesian/sequential_greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.962840 baybe-0.8.2/baybe/recommenders/pure/nonpredictive/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/nonpredictive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/nonpredictive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/nonpredictive/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/recommenders/pure/nonpredictive/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.962840 baybe-0.8.2/baybe/searchspace/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/searchspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/searchspace/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/searchspace/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    28308 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/searchspace/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/searchspace/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.962840 baybe-0.8.2/baybe/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/serialization/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/serialization/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/serialization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30463 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.962840 baybe-0.8.2/baybe/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/strategies/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.962840 baybe-0.8.2/baybe/surrogates/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/ngboost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/surrogates/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.966840 baybe-0.8.2/baybe/targets/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/targets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/targets/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/targets/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/targets/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/targets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.966840 baybe-0.8.2/baybe/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/botorch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/chemistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-27 11:27:50.000000 baybe-0.8.2/baybe/utils/sampling_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.990840 baybe-0.8.2/baybe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17196 2024-03-27 11:28:10.000000 baybe-0.8.2/baybe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-03-27 11:28:10.000000 baybe-0.8.2/baybe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:28:10.000000 baybe-0.8.2/baybe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-27 11:28:10.000000 baybe-0.8.2/baybe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 11:28:10.000000 baybe-0.8.2/baybe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.966840 baybe-0.8.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.970840 baybe-0.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    23544 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/banner1.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23373 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/banner2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)   322341 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/logo1.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26901 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/logo2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38680 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/_static/target_transforms.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/known_issues.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.970840 baybe-0.8.2/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/misc/changelog_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/misc/contributing_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/misc/contributors_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/misc/license_link.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.970840 baybe-0.8.2/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/scripts/convert_code_to_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.970840 baybe-0.8.2/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/templates/custom-attribute-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/templates/custom-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.974840 baybe-0.8.2/docs/userguide/
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/campaigns.md
--rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/constraints.md
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/objective.md
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/parameters.md
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/recommenders.md
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/searchspace.md
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/simulation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/surrogates.md
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/targets.md
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/transfer_learning.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-27 11:27:50.000000 baybe-0.8.2/docs/userguide/userguide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.974840 baybe-0.8.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.974840 baybe-0.8.2/examples/Backtesting/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/Backtesting_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/botorch_analytical.py
--rw-r--r--   0 runner    (1001) docker     (127)    36414 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/botorch_analytical_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    36062 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/botorch_analytical_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/custom_analytical.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/full_initial_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/full_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    62466 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/full_lookup_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    61938 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/full_lookup_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/impute_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    88465 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/lookup.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    83199 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/lookup_withmissing.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Backtesting/multi_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.978840 baybe-0.8.2/examples/Basics/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Basics/Basics_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Basics/campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Basics/recommenders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.978840 baybe-0.8.2/examples/Constraints_Continuous/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Continuous/Constraints_Continuous_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Continuous/hybrid_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Continuous/linear_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.978840 baybe-0.8.2/examples/Constraints_Discrete/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Discrete/Constraints_Discrete_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Discrete/custom_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Discrete/dependency_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Discrete/exclusion_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Discrete/mixture_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Constraints_Discrete/prodsum_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.978840 baybe-0.8.2/examples/Custom_Surrogates/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Custom_Surrogates/Custom_Surrogates_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Custom_Surrogates/custom_architecture_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Custom_Surrogates/custom_architecture_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Custom_Surrogates/custom_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Custom_Surrogates/surrogate_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.978840 baybe-0.8.2/examples/Multi_Target/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Multi_Target/Multi_Target_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Multi_Target/desirability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.982840 baybe-0.8.2/examples/Searchspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Searchspaces/Searchspaces_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Searchspaces/continuous_space_botorch_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Searchspaces/continuous_space_custom_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Searchspaces/discrete_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Searchspaces/hybrid_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.982840 baybe-0.8.2/examples/Serialization/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Serialization/Serialization_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Serialization/basic_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Serialization/create_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Serialization/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.982840 baybe-0.8.2/examples/Transfer_Learning/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/Transfer_Learning_Header.md
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    46984 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/backtesting_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    46456 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/backtesting_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/basic_transfer_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    47629 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/basic_transfer_learning_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    47167 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/Transfer_Learning/basic_transfer_learning_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-27 11:27:50.000000 baybe-0.8.2/examples/plotting_themes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-27 11:27:50.000000 baybe-0.8.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-27 11:27:50.000000 baybe-0.8.2/pydoclint.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-27 11:27:50.000000 baybe-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-27 11:27:50.000000 baybe-0.8.2/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 11:28:10.998840 baybe-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.982840 baybe-0.8.2/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-27 11:27:50.000000 baybe-0.8.2/streamlit/initial_recommender.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-03-27 11:27:50.000000 baybe-0.8.2/streamlit/surrogate_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.986840 baybe-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28211 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.986840 baybe-0.8.2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/docs/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/docs/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/docs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.986840 baybe-0.8.2/tests/hypothesis_strategies/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.990840 baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_searchspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/hypothesis_strategies/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.990840 baybe-0.8.2/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_campaign_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_constraint_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_dataframe_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_meta_recommender_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_naive_hybrid_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_objective_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_parameter_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_searchspace_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_surrogate_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/serialization/test_target_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/simulate_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_constraints_continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_constraints_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_custom_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_custom_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_input_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_iterations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_meta_recommenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_searchspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/test_substance_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:28:10.990840 baybe-0.8.2/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/validation/test_interval_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/validation/test_parameter_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-27 11:27:50.000000 baybe-0.8.2/tests/validation/test_target_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-27 11:27:50.000000 baybe-0.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.269870 baybe-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 18:54:32.000000 baybe-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.217869 baybe-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 18:54:32.000000 baybe-0.9.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.221869 baybe-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-21 18:54:32.000000 baybe-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-21 18:54:32.000000 baybe-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-21 18:54:32.000000 baybe-0.9.0/.github/workflows/regular.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-21 18:54:32.000000 baybe-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 18:54:32.000000 baybe-0.9.0/.github/workflows/reminders.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 18:54:32.000000 baybe-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-21 18:54:32.000000 baybe-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    21712 2024-05-21 18:54:32.000000 baybe-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-21 18:54:32.000000 baybe-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-21 18:54:32.000000 baybe-0.9.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-21 18:54:32.000000 baybe-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18382 2024-05-21 18:54:37.269870 baybe-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-05-21 18:54:32.000000 baybe-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.221869 baybe-0.9.0/baybe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.221869 baybe-0.9.0/baybe/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/acquisition/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/acquisition/acqfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/acquisition/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/acquisition/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.225869 baybe-0.9.0/baybe/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/constraints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/constraints/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/constraints/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/constraints/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/constraints/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.225869 baybe-0.9.0/baybe/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/kernels/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/kernels/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/kernels/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.225869 baybe-0.9.0/baybe/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objectives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objectives/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objectives/desirability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objectives/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/objectives/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.225869 baybe-0.9.0/baybe/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/substance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/parameters/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.225869 baybe-0.9.0/baybe/priors/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/priors/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/recommenders/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/meta/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/meta/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/naive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/recommenders/pure/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/recommenders/pure/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/bayesian/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/bayesian/sequential_greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/recommenders/pure/nonpredictive/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/nonpredictive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/nonpredictive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/nonpredictive/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/recommenders/pure/nonpredictive/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/searchspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/searchspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9485 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/searchspace/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14236 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/searchspace/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31184 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/searchspace/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/searchspace/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.229869 baybe-0.9.0/baybe/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/serialization/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/serialization/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/serialization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.233869 baybe-0.9.0/baybe/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/simulation/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/simulation/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/simulation/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/simulation/transfer_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.233869 baybe-0.9.0/baybe/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/strategies/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.233869 baybe-0.9.0/baybe/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.233869 baybe-0.9.0/baybe/surrogates/gaussian_process/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/gaussian_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/gaussian_process/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/gaussian_process/kernel_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.233869 baybe-0.9.0/baybe/surrogates/gaussian_process/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/gaussian_process/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/gaussian_process/presets/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/gaussian_process/presets/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/ngboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/surrogates/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.233869 baybe-0.9.0/baybe/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/targets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/targets/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/targets/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/targets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.237869 baybe-0.9.0/baybe/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/botorch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17814 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/sampling_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-21 18:54:32.000000 baybe-0.9.0/baybe/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.261870 baybe-0.9.0/baybe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18382 2024-05-21 18:54:37.000000 baybe-0.9.0/baybe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-21 18:54:37.000000 baybe-0.9.0/baybe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:54:37.000000 baybe-0.9.0/baybe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-21 18:54:37.000000 baybe-0.9.0/baybe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 18:54:37.000000 baybe-0.9.0/baybe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.237869 baybe-0.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.237869 baybe-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    23544 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/banner1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23373 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/banner2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)   322341 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/logo1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26901 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/logo2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    38680 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/_static/target_transforms.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/known_issues.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.241870 baybe-0.9.0/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/misc/changelog_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/misc/contributing_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/misc/contributors_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/misc/license_link.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.241870 baybe-0.9.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/scripts/convert_code_to_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.241870 baybe-0.9.0/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/templates/custom-attribute-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/templates/custom-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.241870 baybe-0.9.0/docs/userguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/campaigns.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/constraints.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/envvars.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/objectives.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/parameters.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/recommenders.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/searchspace.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14954 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/serialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/simulation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/surrogates.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/targets.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 18:54:32.000000 baybe-0.9.0/docs/userguide/userguide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.241870 baybe-0.9.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.245869 baybe-0.9.0/examples/Backtesting/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/Backtesting_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/botorch_analytical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36414 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/botorch_analytical_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    36062 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/botorch_analytical_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/custom_analytical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/full_initial_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/full_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62466 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/full_lookup_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    61938 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/full_lookup_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/impute_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88465 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/lookup.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    83199 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/lookup_withmissing.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Backtesting/multi_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.245869 baybe-0.9.0/examples/Basics/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Basics/Basics_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Basics/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Basics/recommenders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.245869 baybe-0.9.0/examples/Constraints_Continuous/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Continuous/Constraints_Continuous_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Continuous/hybrid_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Continuous/linear_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.249869 baybe-0.9.0/examples/Constraints_Discrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Discrete/Constraints_Discrete_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Discrete/custom_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Discrete/dependency_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Discrete/exclusion_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Discrete/mixture_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Constraints_Discrete/prodsum_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.249869 baybe-0.9.0/examples/Custom_Surrogates/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Custom_Surrogates/Custom_Surrogates_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Custom_Surrogates/custom_architecture_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Custom_Surrogates/custom_architecture_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Custom_Surrogates/custom_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Custom_Surrogates/surrogate_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.249869 baybe-0.9.0/examples/Multi_Target/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Multi_Target/Multi_Target_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Multi_Target/desirability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.249869 baybe-0.9.0/examples/Searchspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Searchspaces/Searchspaces_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Searchspaces/continuous_space_botorch_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Searchspaces/continuous_space_custom_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Searchspaces/discrete_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Searchspaces/hybrid_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.249869 baybe-0.9.0/examples/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Serialization/Serialization_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Serialization/basic_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Serialization/create_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Serialization/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.249869 baybe-0.9.0/examples/Transfer_Learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/Transfer_Learning_Header.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46984 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/backtesting_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    46456 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/backtesting_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/basic_transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47629 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/basic_transfer_learning_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    47167 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/Transfer_Learning/basic_transfer_learning_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 18:54:32.000000 baybe-0.9.0/examples/plotting_themes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-21 18:54:32.000000 baybe-0.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-21 18:54:32.000000 baybe-0.9.0/pydoclint.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-21 18:54:32.000000 baybe-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-21 18:54:32.000000 baybe-0.9.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:54:37.269870 baybe-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.253869 baybe-0.9.0/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-21 18:54:32.000000 baybe-0.9.0/streamlit/initial_recommender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-21 18:54:32.000000 baybe-0.9.0/streamlit/surrogate_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.253869 baybe-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29120 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.257870 baybe-0.9.0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/docs/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/docs/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/docs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.257870 baybe-0.9.0/tests/hypothesis_strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.257870 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_searchspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/hypothesis_strategies/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.261870 baybe-0.9.0/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_acquisition_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_campaign_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_constraint_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_dataframe_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_kernel_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_meta_recommender_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_naive_hybrid_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_objective_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_parameter_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_prior_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_searchspace_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_surrogate_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/serialization/test_target_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/simulate_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_constraints_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_constraints_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_custom_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_custom_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_meta_recommenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_searchspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_substance_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:37.261870 baybe-0.9.0/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/validation/test_interval_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/validation/test_objective_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/validation/test_parameter_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-21 18:54:32.000000 baybe-0.9.0/tests/validation/test_target_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-21 18:54:32.000000 baybe-0.9.0/tox.ini
```

### Comparing `baybe-0.8.2/.github/workflows/ci.yml` & `baybe-0.9.0/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.py-version.semantic }}
       - name: Run linting
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e lint-${{ matrix.py-version.tox }}
 
   build-docs:
     name: "Build Docs"
     runs-on: ubuntu-latest
     needs: [lint]
     permissions:
@@ -77,15 +77,15 @@
       id-token: write
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with: {python-version: "3.12"}
       - name: Build Docs
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e docs-py312 -- -e
           
   typecheck:
     needs: [lint]
     strategy:
       matrix:
         py-version: [ {semantic: '3.12', tox: 'py312'} ]
@@ -95,15 +95,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.py-version.semantic }}
       - name: Run type check
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e mypy-${{ matrix.py-version.tox }}
 
   audit:
     needs: [lint]
     strategy:
       matrix:
         py-version: [ {semantic: '3.12', tox: 'py312'} ]
@@ -113,15 +113,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.py-version.semantic }}
       - name: Run pip-audit
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e audit-${{ matrix.py-version.tox }}
 
   coretest:
     needs: [typecheck, audit]
     strategy:
       matrix:
         py-version: [ {semantic: '3.9', tox: 'py39'} ]
@@ -135,15 +135,15 @@
           python-version: ${{ matrix.py-version.semantic }}
       - uses: actions/cache@v4
         with:
           path: .tox/coretest-${{ matrix.py-version.tox }}
           key: coretest-${{ matrix.py-version.tox }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('tox.ini') }}
       - name: Run core tests
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e coretest-${{ matrix.py-version.tox }}
 
   fulltest:
     needs: [typecheck, audit]
     strategy:
       matrix:
         py-version: [ {semantic: '3.9', tox: 'py39'}, {semantic: '3.12', tox: 'py312'} ]
@@ -157,15 +157,15 @@
           python-version: ${{ matrix.py-version.semantic }}
       - uses: actions/cache@v4
         with:
           path: .tox/fulltest-${{ matrix.py-version.tox }}
           key: fulltest-${{ matrix.py-version.tox }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('tox.ini') }}
       - name: Run full tests
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e fulltest-${{ matrix.py-version.tox }} -- --cov-report=xml
       - name: "Assert Overall Coverage"
         run: |
           pip install coverage
           coverage report --fail-under=${{ env.COVERAGE_OVERALL_THRESH }}
       - name: "Assert Individual Coverage"
         shell: bash
```

### Comparing `baybe-0.8.2/.github/workflows/docs.yml` & `baybe-0.9.0/.github/workflows/docs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 name: Documentation
 
 on:
   release:
     types:
       - published
   workflow_dispatch:
+    inputs:
+      force:
+        description: 'Force'
+        default: false
+        required: false
+        type: boolean
+      tag:
+        description: 'Specify tag (empty builds branch HEAD)'
+        required: false
+        default: ''
 
 concurrency:
   group: ${{ github.workflow }}
   cancel-in-progress: true
 
-env:
-  BAYBE_DOCS_LINKCHECK_IGNORE: true  # Ignore link checks to github.io (pages might not yet exist)
-
 jobs:
   build:
     runs-on: ubuntu-latest
     permissions:
       contents: read
       pages: write
       id-token: write
     steps:
       - uses: actions/checkout@v4
+        with:
+          ref: ${{ inputs.tag || github.ref }}
       - uses: actions/setup-python@v5
         with: {python-version: "3.9"}
-      - name: Build Docs
-        run: |
-          pip install tox
-          tox -e docs-py39
+      - name: Install tox
+        run: pip install tox-uv
+      - name: Build Docs ${{ inputs.force == true && '(Force)' || '' }}
+        run: tox -e docs-py39 ${{ inputs.force == true && '-- -f' || '' }}
       - name: Upload docs artifact
         uses: actions/upload-pages-artifact@v1
         with:
-          path: 'build/docs'
+          path: 'docs/build'
 
   deploy:
     needs: build
     runs-on: ubuntu-latest
     permissions:
       contents: read
       pages: write
       id-token: write
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - name: Deploy to GitHub Pages
         id: deployment
-        uses: actions/deploy-pages@v1
+        uses: actions/deploy-pages@v1
```

### Comparing `baybe-0.8.2/.github/workflows/regular.yml` & `baybe-0.9.0/.github/workflows/regular.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
       contents: read
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with: {python-version: "3.9"}
       - name: Build Docs
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e docs-py39
 
   lint:
     strategy:
       fail-fast: false
       matrix:
         py-version: [ {semantic: '3.9', tox: 'py39'},
@@ -60,15 +60,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.py-version.semantic }}
       - name: Run linting
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e lint-${{ matrix.py-version.tox }}
 
   typecheck:
     needs: [lint]
     strategy:
       fail-fast: false
       matrix:
@@ -82,15 +82,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.py-version.semantic }}
       - name: Run type check
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e mypy-${{ matrix.py-version.tox }}
 
   audit:
     needs: [lint]
     strategy:
       fail-fast: false
       matrix:
@@ -104,15 +104,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.py-version.semantic }}
       - name: Run pip-audit
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e audit-${{ matrix.py-version.tox }}
 
   coretest:
     needs: [typecheck, audit]
     strategy:
       fail-fast: false
       matrix:
@@ -130,15 +130,15 @@
           python-version: ${{ matrix.py-version.semantic }}
       - uses: actions/cache@v4
         with:
           path: .tox/coretest-${{ matrix.py-version.tox }}
           key: coretest-${{ matrix.py-version.tox }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('tox.ini') }}
       - name: Run core tests
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e coretest-${{ matrix.py-version.tox }}
 
   fulltest:
     needs: [typecheck, audit]
     strategy:
       fail-fast: false
       matrix:
@@ -156,15 +156,15 @@
           python-version: ${{ matrix.py-version.semantic }}
       - uses: actions/cache@v4
         with:
           path: .tox/fulltest-${{ matrix.py-version.tox }}
           key: fulltest-${{ matrix.py-version.tox }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('tox.ini') }}
       - name: Run full tests
         run: |
-          pip install tox
+          pip install tox-uv
           tox -e fulltest-${{ matrix.py-version.tox }} -- --cov-report=xml
       - name: "Assert Overall Coverage"
         run: |
           pip install coverage
           coverage report --fail-under=${{ env.COVERAGE_OVERALL_THRESH }}
       - name: "Assert Individual Coverage"
         shell: bash
```

### Comparing `baybe-0.8.2/.github/workflows/release.yml` & `baybe-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/.pre-commit-config.yaml` & `baybe-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/CHANGELOG.md` & `baybe-0.9.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,76 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.0] - 2024-05-21
+### Added
+- Class hierarchy for objectives
+- `AdditiveKernel`, `LinearKernel`, `MaternKernel`, `PeriodicKernel`, 
+  `PiecewisePolynomialKernel`, `PolynomialKernel`, `ProductKernel`, `RBFKernel`, 
+  `RFFKernel`, `RQKernel`, `ScaleKernel` classes
+- `KernelFactory` protocol enabling context-dependent construction of kernels
+- Preset mechanism for `GaussianProcessSurrogate`
+- `hypothesis` strategies and roundtrip test for kernels, constraints, objectives,
+  priors and acquisition functions
+- New acquisition functions: `qSR`, `qNEI`, `LogEI`, `qLogEI`, `qLogNEI`
+- `GammaPrior`, `HalfCauchyPrior`, `NormalPrior`, `HalfNormalPrior`, `LogNormalPrior`
+  and `SmoothedBoxPrior` classes
+- Possibility to deserialize classes from optional class name abbreviations
+- Basic deserialization tests using different class type specifiers
+- Serialization user guide
+- Environment variables user guide
+- Utility for estimating memory requirements of discrete product search space
+- `mypy` for search space and objectives
+
+### Changed
+- Reorganized acquisition.py into `acquisition` subpackage
+- Reorganized simulation.py into `simulation` subpackage
+- Reorganized gaussian_process.py into `gaussian_process` subpackage
+- Acquisition functions are now their own objects
+- `acquisition_function_cls` constructor parameter renamed to `acquisition_function`
+- User guide now explains the new objective classes
+- Telemetry deactivation warning is only shown to developers
+- `torch`, `gpytorch` and `botorch` are lazy-loaded for improved startup time
+- If an exception is encountered during simulation, incomplete results are returned 
+  with a warning instead of passing through the uncaught exception
+- Environment variables `BAYBE_NUMPY_USE_SINGLE_PRECISION` and
+  `BAYBE_TORCH_USE_SINGLE_PRECISION` to enforce single point precision usage
+
+### Removed
+- `model_params` attribute from `Surrogate` base class, `GaussianProcessSurrogate` and
+  `CustomONNXSurrogate`
+- Dependency on `requests` package
+  
+### Fixed
+- `n_task_params` now evaluates to 1 if `task_idx == 0`
+- Simulation no longer fails in `ignore` mode when lookup dataframe contains duplicate
+  parameter configurations
+- Simulation no longer fails for targets in `MATCH` mode
+- `closest_element` now works for array-like input of all kinds
+- Structuring concrete subclasses no longer requires providing an explicit `type` field
+- `_target(s)` attributes of `Objectives` are now de-/serialized without leading
+  underscore to support user-friendly serialization strings
+- Telemetry does not execute any code if it was disabled
+- Running simulations no longer alters the states of the global random number generators
+
+### Deprecations
+- The former `baybe.objective.Objective` class has been replaced with
+  `SingleTargetObjective` and `DesirabilityObjective`
+- `acquisition_function_cls` constructor parameter for `BayesianRecommender`
+- `VarUCB` and `qVarUCB` acquisition functions
+
+### Expired Deprecations (from 0.6.*)
+- `BayBE` class
+- `baybe.surrogate` module
+- `baybe.targets.Objective` class
+- `baybe.strategies.Strategy` class
+
 ## [0.8.2] - 2024-03-27
 ### Added
 - Simulation user guide
 - Example for transfer learning backtesting utility
 - `pyupgrade` pre-commit hook
 - Better human readable `__str__` representation of objective and targets
 - Alternative dataframe deserialization from `pd.DataFrame` constructors
@@ -15,29 +78,30 @@
 ### Changed
 - More detailed and sophisticated search space user guide
 - Support for Python 3.12
 - Upgraded syntax to Python 3.9
 - Bumped `onnx` version to fix vulnerability
 - Increased threshold for low-dimensional GP priors
 - Replaced `fit_gpytorch_mll_torch` with `fit_gpytorch_mll`
+- Use `tox-uv` in pipelines
 
 ### Fixed
 - `telemetry` dependency is no longer a group (enables Poetry installation)
 
 ## [0.8.1] - 2024-03-11
 ### Added
 - Better human readable `__str__` representation of campaign
 - README now contains an example on substance encoding results
 - Transfer learning user guide
 - `from_simplex` constructor now also takes and applies optional constraints
 
 ### Changed
 - Full lookup backtesting example now tests different substance encodings
 - Replaced unmaintained `mordred` dependency by `mordredcommunity`
-- `SearchSpace`s now use `ndarray` instead of `Tensor` 
+- `SearchSpace`s now use `ndarray` instead of `Tensor`
 
 ### Fixed
 - `from_simplex` now efficiently validated in `Campaign.validate_config`
 
 ## [0.8.0] - 2024-02-29
 ### Changed
 - BoTorch dependency bumped to `>=0.9.3`
@@ -76,17 +140,16 @@
 ### Fixed
 - Unhandled exception in telemetry when username could not be inferred on Windows
 - Metadata is now correctly updated for hybrid spaces
 - Unintended deactivation of telemetry due to import problem
 - Line wrapping in examples
 
 ### Deprecations
-- `TwoPhaseStrategy`
-- `SequentialStrategy`
-- `StreamingSequentialStrategy`
+- `TwoPhaseStrategy`, `SequentialStrategy` and `StreamingSequentialStrategy` have been
+  replaced with their new `MetaRecommender` versions
 
 ## [0.7.3] - 2024-02-09
 ### Added
 - Copy button for code blocks in documentation
 - `mypy` for campaign, constraints and telemetry
 - Top-level example summaries
 - `RecommenderProtocol` as common interface for `Strategy` and `Recommender`
@@ -142,15 +205,15 @@
 - `ignore_example` flag builds but does not execute examples when building documentation
 - New user guide versions for campaigns, targets and objectives
 - Binarization of dataframes now happens via pickling
 
 ### Fixed
 - Wrong use of `tolerance` argument in constraints user guide
 - Errors with generics and type aliases in documentation
-- Deduplication bug in substance_data hypothesis 
+- Deduplication bug in substance_data `hypothesis` strategy
 - Use pydoclint as flake8 plugin and not as a stand-alone linter
 - Margins in documentation for desktop and mobile version
 - `Interval`s can now also be deserialized from a bounds iterable
 - `SubspaceDiscrete` and `SubspaceContinuous` now have de-/serialization methods
 
 ### Removed
 - Conda install instructions and version badge
```

### Comparing `baybe-0.8.2/CONTRIBUTING.md` & `baybe-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/CONTRIBUTORS.md` & `baybe-0.9.0/CONTRIBUTORS.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Contributors
 
-## Authors
+## Maintainers
 - Martin Fitzner (Merck KGaA, Darmstadt, Germany), [Contact](mailto:martin.fitzner@merckgroup.com), [Github](https://github.com/Scienfitz)
 - Adrian Šošić (Merck Life Science KGaA, Darmstadt, Germany), [Contact](mailto:adrian.sosic@merckgroup.com), [Github](https://github.com/AdrianSosic)
 - Alexander Hopp (Merck KGaA, Darmstadt, Germany) [Contact](mailto:alexander.hopp@merckgroup.com), [Github](https://github.com/AVHopp)
-- Alex Lee (EMD Electronics, Tempe, Arizona, USA) [Contact](mailto:alex.lee@emdgroup.com), [Github](https://github.com/galaxee87)
 
 ## Contributors
+- Alex Lee (EMD Electronics, Tempe, Arizona, USA):  
+  Work on surrogate models
 - Daniel Weber (Merck KGaA, Darmstadt, Germany):  
   Telemetry prototype
 - Emeline Sola (during an internship at Merck KGaA, Darmstadt, Germany):  
   Auto-documentation of the examples
 - Sourabh Agrawal (Sigma-Aldrich Chemicals Private Limited):
   Initial implementation of additional surrogate models and clustering methods
 - Julie Fang (Merck Life Science KGaA, Darmstadt, Germany):
```

### Comparing `baybe-0.8.2/LICENSE` & `baybe-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/PKG-INFO` & `baybe-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baybe
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Bayesian Back End for Design of Experiments
 Author: Merck KGaA, Darmstadt, Germany
 License: Apache-2.0
 Project-URL: Homepage, https://emdgroup.github.io/baybe/
 Project-URL: Documentation, https://emdgroup.github.io/baybe/_autosummary/baybe.html
 Project-URL: Changelog, https://emdgroup.github.io/baybe/misc/changelog_link.html
 Project-URL: GitHub, https://github.com/emdgroup/baybe/
@@ -35,20 +35,19 @@
 Requires-Dist: pandas>=1.4.2
 Requires-Dist: protobuf<=3.20.3
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: scikit-learn-extra>=0.3.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: setuptools-scm>=7.1.0
 Requires-Dist: torch>=1.13.1
+Requires-Dist: typing_extensions>=4.7.0
 Requires-Dist: opentelemetry-sdk>=1.16.0
 Requires-Dist: opentelemetry-propagator-aws-xray>=1.0.0
 Requires-Dist: opentelemetry-exporter-otlp>=1.16.0
 Requires-Dist: opentelemetry-sdk-extension-aws>=2.0.0
-Requires-Dist: requests>=2.31.0
-Requires-Dist: urllib3>=2.0.7
 Provides-Extra: chem
 Requires-Dist: rdkit>=2022.3.4; extra == "chem"
 Requires-Dist: mordredcommunity>=1.2.0; extra == "chem"
 Provides-Extra: onnx
 Requires-Dist: onnx>=1.16.0; extra == "onnx"
 Requires-Dist: onnxruntime>=1.15.1; extra == "onnx"
 Requires-Dist: skl2onnx>=1.15.0; extra == "onnx"
@@ -58,15 +57,15 @@
 Requires-Dist: baybe[examples]; extra == "dev"
 Requires-Dist: baybe[lint]; extra == "dev"
 Requires-Dist: baybe[mypy]; extra == "dev"
 Requires-Dist: baybe[onnx]; extra == "dev"
 Requires-Dist: baybe[simulation]; extra == "dev"
 Requires-Dist: baybe[test]; extra == "dev"
 Requires-Dist: pip-audit>=2.5.5; extra == "dev"
-Requires-Dist: tox>=4.10.0; extra == "dev"
+Requires-Dist: tox-uv>=1.7.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: baybe[examples]; extra == "docs"
 Requires-Dist: furo>=2023.09.10; extra == "docs"
 Requires-Dist: jupyter>=1.0.0; extra == "docs"
 Requires-Dist: jupytext>=1.16.1; extra == "docs"
 Requires-Dist: myst-parser>=2.0.0; extra == "docs"
 Requires-Dist: sphinx>=7.1.1; extra == "docs"
@@ -89,15 +88,14 @@
 Requires-Dist: pydoclint==0.2.1; extra == "lint"
 Requires-Dist: ruff==0.1.6; extra == "lint"
 Requires-Dist: typos==1.16.23; extra == "lint"
 Provides-Extra: mypy
 Requires-Dist: mypy>=1.6.1; extra == "mypy"
 Requires-Dist: pandas-stubs>=2.0.3.230814; extra == "mypy"
 Requires-Dist: funcy-stubs>=0.1.1; extra == "mypy"
-Requires-Dist: types-requests>=2.31.0.20240106; extra == "mypy"
 Requires-Dist: types-seaborn>=0.12.2; extra == "mypy"
 Provides-Extra: simulation
 Requires-Dist: xyzpy>=1.2.1; extra == "simulation"
 Provides-Extra: test
 Requires-Dist: baybe[lint]; extra == "test"
 Requires-Dist: hypothesis[pandas]>=6.88.4; extra == "test"
 Requires-Dist: pytest>=7.2.0; extra == "test"
@@ -127,63 +125,62 @@
 &nbsp;•&nbsp;
 <a href="https://emdgroup.github.io/baybe/misc/contributing_link.html">Contribute<a/>
 &nbsp;
 </div>
 
 # BayBE — A Bayesian Back End for Design of Experiments
 
-The Bayesian Back End (**BayBE**) provides a general-purpose toolbox for Bayesian Design
+The Bayesian Back End (**BayBE**) is a general-purpose toolbox for Bayesian Design
 of Experiments, focusing on additions that enable real-world experimental campaigns.
 
 Besides functionality to perform a typical recommend-measure loop, BayBE's highlights are:
-- Custom parameter encodings: Improve your campaign with domain knowledge
-- Built-in chemical encodings: Improve your campaign with chemical knowledge
-- Single and multiple targets with min, max and match objectives
-- Custom surrogate models: For specialized problems or active learning
-- Hybrid (mixed continuous and discrete) spaces
-- Transfer learning: Mix data from multiple campaigns and accelerate optimization
-- Comprehensive backtest, simulation and imputation utilities: Benchmark and find your best settings
-- Fully typed and hypothesis-tested: Robust code base
-- All objects are fully de-/serializable: Useful for storing results in databases or use in wrappers like APIs
+- ✨ Custom parameter encodings: Improve your campaign with domain knowledge
+- 🧪 Built-in chemical encodings: Improve your campaign with chemical knowledge
+- 🎯 Single and multiple targets with min, max and match objectives
+- ⚙️ Custom surrogate models: For specialized problems or active learning
+- 🎭 Hybrid (mixed continuous and discrete) spaces
+- 🚀 Transfer learning: Mix data from multiple campaigns and accelerate optimization
+- 📈 Comprehensive backtest, simulation and imputation utilities: Benchmark and find your best settings
+- 📝 Fully typed and hypothesis-tested: Robust code base
+- 🔄 All objects are fully de-/serializable: Useful for storing results in databases or use in wrappers like APIs
 
 
-## Quick Start
+## ⚡ Quick Start
 
 Let us consider a simple experiment where we control three parameters and want to
 maximize a single target called `Yield`.
 
 First, install BayBE into your Python environment: 
 ```bash 
 pip install baybe 
 ``` 
 For more information on this step, see our
 [detailed installation instructions](#installation).
 
 ### Defining the Optimization Objective
 
 In BayBE's language, the `Yield` can be represented as a `NumericalTarget`,
-which we pass into an `Objective`.
+which we wrap into a `SingleTargetObjective`:
 
 ```python
 from baybe.targets import NumericalTarget
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 
 target = NumericalTarget(
     name="Yield",
     mode="MAX",
 )
-objective = Objective(mode="SINGLE", targets=[target])
+objective = SingleTargetObjective(target=target)
 ```
-
-In cases where we need to consider multiple (potentially competing) targets, the
-role of the `Objective` is to define additional settings, e.g. how these targets should
-be balanced.
-In `SINGLE` mode, however, there are no additional settings.
-For more details, see 
-[the objective section of the user guide](https://emdgroup.github.io/baybe/userguide/objective.html).
+In cases where we are confronted with multiple (potentially conflicting) targets,
+the `DesirabilityObjective` can be used instead. It allows to define additional
+settings, such as how these targets should be balanced.
+For more details, see the
+[objectives section](https://emdgroup.github.io/baybe/userguide/objectives.html)
+of the user guide.
 
 ### Defining the Search Space
 
 Next, we inform BayBE about the available "control knobs", that is, the underlying
 system parameters we can tune to optimize our targets. This also involves specifying 
 their values/ranges and other parameter-specific details.
 
@@ -226,23 +223,27 @@
 of the user guide.
 
 Additionally, we can define a set of constraints to further specify allowed ranges and
 relationships between our parameters. Details can be found in the
 [constraints section](https://emdgroup.github.io/baybe/userguide/constraints.html) of the user guide.
 In this example, we assume no further constraints.
 
-With the parameter and constraint definitions at hand, we can now create our
+With the parameter definitions at hand, we can now create our
 `SearchSpace` based on the Cartesian product of all possible parameter values:
 
 ```python
 from baybe.searchspace import SearchSpace
 
 searchspace = SearchSpace.from_product(parameters)
 ```
 
+See the [search spaces section](https://emdgroup.github.io/baybe/userguide/searchspace.html)
+of our user guide for more information on the structure of search spaces
+and alternative ways of construction. 
+
 ### Optional: Defining the Optimization Strategy
 
 As an optional step, we can specify details on how the optimization should be
 conducted. If omitted, BayBE will choose a default setting.
 
 For our example, we combine two recommenders via a so-called meta recommender named
 `TwoPhaseMetaRecommender`:
@@ -313,27 +314,27 @@
 campaign.add_measurements(df)
 ```
 
 With the newly arrived data, BayBE can produce a refined design for the next iteration.
 This loop would typically continue until a desired target value has been achieved in
 the experiment.
 
-### Advanced Example - Chemical Substances
+### Advanced Example: Chemical Substances
 BayBE has several modules to go beyond traditional approaches. One such example is the
 use of custom encodings for categorical parameters. Chemical encodings for substances
 are a special built-in case of this that comes with BayBE.
 
 In the following picture you can see
 the outcome for treating the solvent, base and ligand in a direct arylation reaction
 optimization (from [Shields, B.J. et al.](https://doi.org/10.1038/s41586-021-03213-y)) with
 chemical encodings compared to one-hot and a random baseline:
 ![Substance Encoding Example](./examples/Backtesting/full_lookup_light.svg)
 
 (installation)=
-## Installation
+## 💻 Installation
 ### From Package Index
 The easiest way to install BayBE is via PyPI:
 
 ```bash
 pip install baybe
 ```
 
@@ -394,28 +395,43 @@
 - `lint`: Required for linting and formatting.
 - `mypy`: Required for static type checking.
 - `onnx`: Required for using custom surrogate models in [ONNX format](https://onnx.ai).
 - `simulation`: Enabling the [simulation](https://emdgroup.github.io/baybe/_autosummary/baybe.simulation.html) module.
 - `test`: Required for running the tests.
 - `dev`: All of the above plus `tox` and `pip-audit`. For code contributors.
 
+## 📡 Telemetry
+BayBE collects anonymous usage statistics **only** for employees of Merck KGaA, 
+Darmstadt, Germany and/or its affiliates. The recording of metrics is turned off for
+all other users and is impossible due to a VPN block. In any case, the usage statistics
+do **not** involve logging of recorded measurements, targets/parameters or their names
+or any project information that would allow for reconstruction of details. The user and
+host machine names are anonymized with via truncated hashing.
+- You can verify the above statements by studying the open-source code in the
+  `telemetry` module.
+- You can always deactivate all telemetry by setting the environment variable 
+  `BAYBE_TELEMETRY_ENABLED` to `false` or `off`. For details please consult
+  [this page](https://emdgroup.github.io/baybe/userguide/envvars.html#telemetry).
+- If you want to be absolutely sure, you can uninstall internet related packages such
+  as `opentelemetry*` or its secondary dependencies from the environment. Due to the
+  inability of specifying opt-out dependencies, these are installed by default, but the
+  package works without them.
 
-## Authors
+## 👨🏻‍🔧 Maintainers
 
 - Martin Fitzner (Merck KGaA, Darmstadt, Germany), [Contact](mailto:martin.fitzner@merckgroup.com), [Github](https://github.com/Scienfitz)
 - Adrian Šošić (Merck Life Science KGaA, Darmstadt, Germany), [Contact](mailto:adrian.sosic@merckgroup.com), [Github](https://github.com/AdrianSosic)
 - Alexander Hopp (Merck KGaA, Darmstadt, Germany) [Contact](mailto:alexander.hopp@merckgroup.com), [Github](https://github.com/AVHopp)
-- Alex Lee (EMD Electronics, Tempe, Arizona, USA) [Contact](mailto:alex.lee@emdgroup.com), [Github](https://github.com/galaxee87)
 
 
-## Known Issues
+## 🛠️ Known Issues
 A list of know issues can be found [here](https://emdgroup.github.io/baybe/known_issues.html).
 
 
-## License
+## 📄 License
 
 Copyright 2022-2024 Merck KGaA, Darmstadt, Germany
 and/or its affiliates. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `baybe-0.8.2/README.md` & `baybe-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,63 +22,62 @@
 &nbsp;•&nbsp;
 <a href="https://emdgroup.github.io/baybe/misc/contributing_link.html">Contribute<a/>
 &nbsp;
 </div>
 
 # BayBE — A Bayesian Back End for Design of Experiments
 
-The Bayesian Back End (**BayBE**) provides a general-purpose toolbox for Bayesian Design
+The Bayesian Back End (**BayBE**) is a general-purpose toolbox for Bayesian Design
 of Experiments, focusing on additions that enable real-world experimental campaigns.
 
 Besides functionality to perform a typical recommend-measure loop, BayBE's highlights are:
-- Custom parameter encodings: Improve your campaign with domain knowledge
-- Built-in chemical encodings: Improve your campaign with chemical knowledge
-- Single and multiple targets with min, max and match objectives
-- Custom surrogate models: For specialized problems or active learning
-- Hybrid (mixed continuous and discrete) spaces
-- Transfer learning: Mix data from multiple campaigns and accelerate optimization
-- Comprehensive backtest, simulation and imputation utilities: Benchmark and find your best settings
-- Fully typed and hypothesis-tested: Robust code base
-- All objects are fully de-/serializable: Useful for storing results in databases or use in wrappers like APIs
+- ✨ Custom parameter encodings: Improve your campaign with domain knowledge
+- 🧪 Built-in chemical encodings: Improve your campaign with chemical knowledge
+- 🎯 Single and multiple targets with min, max and match objectives
+- ⚙️ Custom surrogate models: For specialized problems or active learning
+- 🎭 Hybrid (mixed continuous and discrete) spaces
+- 🚀 Transfer learning: Mix data from multiple campaigns and accelerate optimization
+- 📈 Comprehensive backtest, simulation and imputation utilities: Benchmark and find your best settings
+- 📝 Fully typed and hypothesis-tested: Robust code base
+- 🔄 All objects are fully de-/serializable: Useful for storing results in databases or use in wrappers like APIs
 
 
-## Quick Start
+## ⚡ Quick Start
 
 Let us consider a simple experiment where we control three parameters and want to
 maximize a single target called `Yield`.
 
 First, install BayBE into your Python environment: 
 ```bash 
 pip install baybe 
 ``` 
 For more information on this step, see our
 [detailed installation instructions](#installation).
 
 ### Defining the Optimization Objective
 
 In BayBE's language, the `Yield` can be represented as a `NumericalTarget`,
-which we pass into an `Objective`.
+which we wrap into a `SingleTargetObjective`:
 
 ```python
 from baybe.targets import NumericalTarget
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 
 target = NumericalTarget(
     name="Yield",
     mode="MAX",
 )
-objective = Objective(mode="SINGLE", targets=[target])
+objective = SingleTargetObjective(target=target)
 ```
-
-In cases where we need to consider multiple (potentially competing) targets, the
-role of the `Objective` is to define additional settings, e.g. how these targets should
-be balanced.
-In `SINGLE` mode, however, there are no additional settings.
-For more details, see 
-[the objective section of the user guide](https://emdgroup.github.io/baybe/userguide/objective.html).
+In cases where we are confronted with multiple (potentially conflicting) targets,
+the `DesirabilityObjective` can be used instead. It allows to define additional
+settings, such as how these targets should be balanced.
+For more details, see the
+[objectives section](https://emdgroup.github.io/baybe/userguide/objectives.html)
+of the user guide.
 
 ### Defining the Search Space
 
 Next, we inform BayBE about the available "control knobs", that is, the underlying
 system parameters we can tune to optimize our targets. This also involves specifying 
 their values/ranges and other parameter-specific details.
 
@@ -121,23 +120,27 @@
 of the user guide.
 
 Additionally, we can define a set of constraints to further specify allowed ranges and
 relationships between our parameters. Details can be found in the
 [constraints section](https://emdgroup.github.io/baybe/userguide/constraints.html) of the user guide.
 In this example, we assume no further constraints.
 
-With the parameter and constraint definitions at hand, we can now create our
+With the parameter definitions at hand, we can now create our
 `SearchSpace` based on the Cartesian product of all possible parameter values:
 
 ```python
 from baybe.searchspace import SearchSpace
 
 searchspace = SearchSpace.from_product(parameters)
 ```
 
+See the [search spaces section](https://emdgroup.github.io/baybe/userguide/searchspace.html)
+of our user guide for more information on the structure of search spaces
+and alternative ways of construction. 
+
 ### Optional: Defining the Optimization Strategy
 
 As an optional step, we can specify details on how the optimization should be
 conducted. If omitted, BayBE will choose a default setting.
 
 For our example, we combine two recommenders via a so-called meta recommender named
 `TwoPhaseMetaRecommender`:
@@ -208,27 +211,27 @@
 campaign.add_measurements(df)
 ```
 
 With the newly arrived data, BayBE can produce a refined design for the next iteration.
 This loop would typically continue until a desired target value has been achieved in
 the experiment.
 
-### Advanced Example - Chemical Substances
+### Advanced Example: Chemical Substances
 BayBE has several modules to go beyond traditional approaches. One such example is the
 use of custom encodings for categorical parameters. Chemical encodings for substances
 are a special built-in case of this that comes with BayBE.
 
 In the following picture you can see
 the outcome for treating the solvent, base and ligand in a direct arylation reaction
 optimization (from [Shields, B.J. et al.](https://doi.org/10.1038/s41586-021-03213-y)) with
 chemical encodings compared to one-hot and a random baseline:
 ![Substance Encoding Example](./examples/Backtesting/full_lookup_light.svg)
 
 (installation)=
-## Installation
+## 💻 Installation
 ### From Package Index
 The easiest way to install BayBE is via PyPI:
 
 ```bash
 pip install baybe
 ```
 
@@ -289,28 +292,43 @@
 - `lint`: Required for linting and formatting.
 - `mypy`: Required for static type checking.
 - `onnx`: Required for using custom surrogate models in [ONNX format](https://onnx.ai).
 - `simulation`: Enabling the [simulation](https://emdgroup.github.io/baybe/_autosummary/baybe.simulation.html) module.
 - `test`: Required for running the tests.
 - `dev`: All of the above plus `tox` and `pip-audit`. For code contributors.
 
+## 📡 Telemetry
+BayBE collects anonymous usage statistics **only** for employees of Merck KGaA, 
+Darmstadt, Germany and/or its affiliates. The recording of metrics is turned off for
+all other users and is impossible due to a VPN block. In any case, the usage statistics
+do **not** involve logging of recorded measurements, targets/parameters or their names
+or any project information that would allow for reconstruction of details. The user and
+host machine names are anonymized with via truncated hashing.
+- You can verify the above statements by studying the open-source code in the
+  `telemetry` module.
+- You can always deactivate all telemetry by setting the environment variable 
+  `BAYBE_TELEMETRY_ENABLED` to `false` or `off`. For details please consult
+  [this page](https://emdgroup.github.io/baybe/userguide/envvars.html#telemetry).
+- If you want to be absolutely sure, you can uninstall internet related packages such
+  as `opentelemetry*` or its secondary dependencies from the environment. Due to the
+  inability of specifying opt-out dependencies, these are installed by default, but the
+  package works without them.
 
-## Authors
+## 👨🏻‍🔧 Maintainers
 
 - Martin Fitzner (Merck KGaA, Darmstadt, Germany), [Contact](mailto:martin.fitzner@merckgroup.com), [Github](https://github.com/Scienfitz)
 - Adrian Šošić (Merck Life Science KGaA, Darmstadt, Germany), [Contact](mailto:adrian.sosic@merckgroup.com), [Github](https://github.com/AdrianSosic)
 - Alexander Hopp (Merck KGaA, Darmstadt, Germany) [Contact](mailto:alexander.hopp@merckgroup.com), [Github](https://github.com/AVHopp)
-- Alex Lee (EMD Electronics, Tempe, Arizona, USA) [Contact](mailto:alex.lee@emdgroup.com), [Github](https://github.com/galaxee87)
 
 
-## Known Issues
+## 🛠️ Known Issues
 A list of know issues can be found [here](https://emdgroup.github.io/baybe/known_issues.html).
 
 
-## License
+## 📄 License
 
 Copyright 2022-2024 Merck KGaA, Darmstadt, Germany
 and/or its affiliates. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

#### html2text {}

```diff
@@ -22,144 +22,159 @@
    baybe/pulls/) [![License](https://shields.io/badge/License-Apache%202.0-
      green.svg?style=flat-square&labelColor=96d7d2&color=ffdcb9)](http://
             www.apache.org/licenses/LICENSE-2.0) [![Logo](https://
 raw.githubusercontent.com/emdgroup/baybe/main/docs/_static/banner2.svg)](https:
  //github.com/emdgroup/baybe/)   _H_o_m_e_p_a_g_e_ _ _â__¢_ _ _U_s_e_r_ _G_u_i_d_e_ _ _â__¢_ _ _D_o_c_u_m_e_n_t_a_t_i_o_n
                               _ _â__¢_ _ _C_o_n_t_r_i_b_u_t_e_ _ 
 # BayBE â A Bayesian Back End for Design of Experiments The Bayesian Back End
-(**BayBE**) provides a general-purpose toolbox for Bayesian Design of
-Experiments, focusing on additions that enable real-world experimental
-campaigns. Besides functionality to perform a typical recommend-measure loop,
-BayBE's highlights are: - Custom parameter encodings: Improve your campaign
-with domain knowledge - Built-in chemical encodings: Improve your campaign with
-chemical knowledge - Single and multiple targets with min, max and match
-objectives - Custom surrogate models: For specialized problems or active
-learning - Hybrid (mixed continuous and discrete) spaces - Transfer learning:
-Mix data from multiple campaigns and accelerate optimization - Comprehensive
-backtest, simulation and imputation utilities: Benchmark and find your best
-settings - Fully typed and hypothesis-tested: Robust code base - All objects
-are fully de-/serializable: Useful for storing results in databases or use in
-wrappers like APIs ## Quick Start Let us consider a simple experiment where we
-control three parameters and want to maximize a single target called `Yield`.
-First, install BayBE into your Python environment: ```bash pip install baybe
-``` For more information on this step, see our [detailed installation
-instructions](#installation). ### Defining the Optimization Objective In
-BayBE's language, the `Yield` can be represented as a `NumericalTarget`, which
-we pass into an `Objective`. ```python from baybe.targets import
-NumericalTarget from baybe.objective import Objective target = NumericalTarget
-( name="Yield", mode="MAX", ) objective = Objective(mode="SINGLE", targets=
-[target]) ``` In cases where we need to consider multiple (potentially
-competing) targets, the role of the `Objective` is to define additional
-settings, e.g. how these targets should be balanced. In `SINGLE` mode, however,
-there are no additional settings. For more details, see [the objective section
-of the user guide](https://emdgroup.github.io/baybe/userguide/objective.html).
-### Defining the Search Space Next, we inform BayBE about the available
-"control knobs", that is, the underlying system parameters we can tune to
-optimize our targets. This also involves specifying their values/ranges and
-other parameter-specific details. For our example, we assume that we can
-control three parameters â `Granularity`, `Pressure[bar]`, and `Solvent` â
-as follows: ```python from baybe.parameters import ( CategoricalParameter,
-NumericalDiscreteParameter, SubstanceParameter, ) parameters =
-[ CategoricalParameter( name="Granularity", values=["coarse", "medium",
-"fine"], encoding="OHE", # one-hot encoding of categories ),
+(**BayBE**) is a general-purpose toolbox for Bayesian Design of Experiments,
+focusing on additions that enable real-world experimental campaigns. Besides
+functionality to perform a typical recommend-measure loop, BayBE's highlights
+are: - â¨ Custom parameter encodings: Improve your campaign with domain
+knowledge - ð§ª Built-in chemical encodings: Improve your campaign with
+chemical knowledge - ð¯ Single and multiple targets with min, max and match
+objectives - âï¸ Custom surrogate models: For specialized problems or active
+learning - ð­ Hybrid (mixed continuous and discrete) spaces - ð Transfer
+learning: Mix data from multiple campaigns and accelerate optimization - ð
+Comprehensive backtest, simulation and imputation utilities: Benchmark and find
+your best settings - ð Fully typed and hypothesis-tested: Robust code base -
+ð All objects are fully de-/serializable: Useful for storing results in
+databases or use in wrappers like APIs ## â¡ Quick Start Let us consider a
+simple experiment where we control three parameters and want to maximize a
+single target called `Yield`. First, install BayBE into your Python
+environment: ```bash pip install baybe ``` For more information on this step,
+see our [detailed installation instructions](#installation). ### Defining the
+Optimization Objective In BayBE's language, the `Yield` can be represented as a
+`NumericalTarget`, which we wrap into a `SingleTargetObjective`: ```python from
+baybe.targets import NumericalTarget from baybe.objectives import
+SingleTargetObjective target = NumericalTarget( name="Yield", mode="MAX", )
+objective = SingleTargetObjective(target=target) ``` In cases where we are
+confronted with multiple (potentially conflicting) targets, the
+`DesirabilityObjective` can be used instead. It allows to define additional
+settings, such as how these targets should be balanced. For more details, see
+the [objectives section](https://emdgroup.github.io/baybe/userguide/
+objectives.html) of the user guide. ### Defining the Search Space Next, we
+inform BayBE about the available "control knobs", that is, the underlying
+system parameters we can tune to optimize our targets. This also involves
+specifying their values/ranges and other parameter-specific details. For our
+example, we assume that we can control three parameters â `Granularity`,
+`Pressure[bar]`, and `Solvent` â as follows: ```python from baybe.parameters
+import ( CategoricalParameter, NumericalDiscreteParameter, SubstanceParameter,
+) parameters = [ CategoricalParameter( name="Granularity", values=["coarse",
+"medium", "fine"], encoding="OHE", # one-hot encoding of categories ),
 NumericalDiscreteParameter( name="Pressure[bar]", values=[1, 5, 10],
 tolerance=0.2, # allows experimental inaccuracies up to 0.2 when reading values
 ), SubstanceParameter( name="Solvent", data={ "Solvent A": "COC", "Solvent B":
 "CCC", # label-SMILES pairs "Solvent C": "O", "Solvent D": "CS(=O)C", },
 encoding="MORDRED", # chemical encoding via mordred package ), ] ``` For more
 parameter types and their details, see the [parameters section](https://
 emdgroup.github.io/baybe/userguide/parameters.html) of the user guide.
 Additionally, we can define a set of constraints to further specify allowed
 ranges and relationships between our parameters. Details can be found in the
 [constraints section](https://emdgroup.github.io/baybe/userguide/
 constraints.html) of the user guide. In this example, we assume no further
-constraints. With the parameter and constraint definitions at hand, we can now
-create our `SearchSpace` based on the Cartesian product of all possible
-parameter values: ```python from baybe.searchspace import SearchSpace
-searchspace = SearchSpace.from_product(parameters) ``` ### Optional: Defining
-the Optimization Strategy As an optional step, we can specify details on how
-the optimization should be conducted. If omitted, BayBE will choose a default
-setting. For our example, we combine two recommenders via a so-called meta
-recommender named `TwoPhaseMetaRecommender`: 1. In cases where no measurements
-have been made prior to the interaction with BayBE, a selection via
-`initial_recommender` is used. 2. As soon as the first measurements are
-available, we switch to `recommender`. For more details on the different
-recommenders, their underlying algorithmic details, and their configuration
-settings, see the [recommenders section](https://emdgroup.github.io/baybe/
-userguide/recommenders.html) of the user guide. ```python from
-baybe.recommenders import ( SequentialGreedyRecommender, FPSRecommender,
-TwoPhaseMetaRecommender, ) recommender = TwoPhaseMetaRecommender
-( initial_recommender=FPSRecommender(), # farthest point sampling
-recommender=SequentialGreedyRecommender(), # Bayesian model-based optimization
-) ``` ### The Optimization Loop We can now construct a campaign object that
-brings all pieces of the puzzle together: ```python from baybe import Campaign
-campaign = Campaign(searchspace, objective, recommender) ``` With this object
-at hand, we can start our experimentation cycle. In particular: * We can ask
-BayBE to `recommend` new experiments. * We can `add_measurements` for certain
-experimental settings to the campaign's database. Note that these two steps can
-be performed in any order. In particular, available measurements can be
-submitted at any time and also several times before querying the next
-recommendations. ```python df = campaign.recommend(batch_size=3) print(df) ```
-```none Granularity Pressure[bar] Solvent 15 medium 1.0 Solvent D 10 coarse
-10.0 Solvent C 29 fine 5.0 Solvent B ``` Note that the specific recommendations
-will depend on both the data already fed to the campaign and the random number
-generator seed that is used. After having conducted the corresponding
-experiments, we can add our measured targets to the table and feed it back to
-the campaign: ```python df["Yield"] = [79.8, 54.1, 59.4]
-campaign.add_measurements(df) ``` With the newly arrived data, BayBE can
-produce a refined design for the next iteration. This loop would typically
-continue until a desired target value has been achieved in the experiment. ###
-Advanced Example - Chemical Substances BayBE has several modules to go beyond
-traditional approaches. One such example is the use of custom encodings for
-categorical parameters. Chemical encodings for substances are a special built-
-in case of this that comes with BayBE. In the following picture you can see the
-outcome for treating the solvent, base and ligand in a direct arylation
-reaction optimization (from [Shields, B.J. et al.](https://doi.org/10.1038/
-s41586-021-03213-y)) with chemical encodings compared to one-hot and a random
-baseline: ![Substance Encoding Example](./examples/Backtesting/
-full_lookup_light.svg) (installation)= ## Installation ### From Package Index
-The easiest way to install BayBE is via PyPI: ```bash pip install baybe ``` A
-certain released version of the package can be installed by specifying the
-corresponding version tag in the form `baybe==x.y.z`. ### From GitHub If you
-need finer control and would like to install a specific commit that has not
-been released under a certain version tag, you can do so by installing BayBE
-directly from GitHub via git and specifying the corresponding [git ref](https:/
-/pip.pypa.io/en/stable/topics/vcs-support/#git). For instance, to install the
-latest commit of the main branch, run: ```bash pip install git+https://
-github.com/emdgroup/baybe.git@main ``` ### From Local Clone Alternatively, you
-can install the package from your own local copy. First, clone the repository,
-navigate to the repository root folder, check out the desired commit, and run:
-```bash pip install . ``` A developer would typically also install the package
-in editable mode ('-e'), which ensures that changes to the code do not require
-a reinstallation. ```bash pip install -e . ``` If you need to add additional
-dependencies, make sure to use the correct syntax including `''`: ```bash pip
-install -e '.[dev]' ``` ### Optional Dependencies There are several dependency
-groups that can be selected during pip installation, like ```bash pip install
-'baybe[test,lint]' # will install baybe with additional dependency groups
-`test` and `lint` ``` To get the most out of `baybe`, we recommend to install
-at least ```bash pip install 'baybe[chem,simulation]' ``` The available groups
-are: - `chem`: Cheminformatics utilities (e.g. for the `SubstanceParameter`). -
-`docs`: Required for creating the documentation. - `examples`: Required for
-running the examples/streamlit. - `lint`: Required for linting and formatting.
-- `mypy`: Required for static type checking. - `onnx`: Required for using
-custom surrogate models in [ONNX format](https://onnx.ai). - `simulation`:
-Enabling the [simulation](https://emdgroup.github.io/baybe/_autosummary/
-baybe.simulation.html) module. - `test`: Required for running the tests. -
-`dev`: All of the above plus `tox` and `pip-audit`. For code contributors. ##
-Authors - Martin Fitzner (Merck KGaA, Darmstadt, Germany), [Contact](mailto:
-martin.fitzner@merckgroup.com), [Github](https://github.com/Scienfitz) - Adrian
-Å oÅ¡iÄ (Merck Life Science KGaA, Darmstadt, Germany), [Contact](mailto:
-adrian.sosic@merckgroup.com), [Github](https://github.com/AdrianSosic) -
-Alexander Hopp (Merck KGaA, Darmstadt, Germany) [Contact](mailto:
-alexander.hopp@merckgroup.com), [Github](https://github.com/AVHopp) - Alex Lee
-(EMD Electronics, Tempe, Arizona, USA) [Contact](mailto:alex.lee@emdgroup.com),
-[Github](https://github.com/galaxee87) ## Known Issues A list of know issues
-can be found [here](https://emdgroup.github.io/baybe/known_issues.html). ##
-License Copyright 2022-2024 Merck KGaA, Darmstadt, Germany and/or its
-affiliates. All rights reserved. Licensed under the Apache License, Version 2.0
-(the "License"); you may not use this file except in compliance with the
-License. You may obtain a copy of the License at http://www.apache.org/
-licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
-software distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
-the License for the specific language governing permissions and limitations
-under the License.
+constraints. With the parameter definitions at hand, we can now create our
+`SearchSpace` based on the Cartesian product of all possible parameter values:
+```python from baybe.searchspace import SearchSpace searchspace =
+SearchSpace.from_product(parameters) ``` See the [search spaces section](https:
+//emdgroup.github.io/baybe/userguide/searchspace.html) of our user guide for
+more information on the structure of search spaces and alternative ways of
+construction. ### Optional: Defining the Optimization Strategy As an optional
+step, we can specify details on how the optimization should be conducted. If
+omitted, BayBE will choose a default setting. For our example, we combine two
+recommenders via a so-called meta recommender named `TwoPhaseMetaRecommender`:
+1. In cases where no measurements have been made prior to the interaction with
+BayBE, a selection via `initial_recommender` is used. 2. As soon as the first
+measurements are available, we switch to `recommender`. For more details on the
+different recommenders, their underlying algorithmic details, and their
+configuration settings, see the [recommenders section](https://
+emdgroup.github.io/baybe/userguide/recommenders.html) of the user guide.
+```python from baybe.recommenders import ( SequentialGreedyRecommender,
+FPSRecommender, TwoPhaseMetaRecommender, ) recommender =
+TwoPhaseMetaRecommender( initial_recommender=FPSRecommender(), # farthest point
+sampling recommender=SequentialGreedyRecommender(), # Bayesian model-based
+optimization ) ``` ### The Optimization Loop We can now construct a campaign
+object that brings all pieces of the puzzle together: ```python from baybe
+import Campaign campaign = Campaign(searchspace, objective, recommender) ```
+With this object at hand, we can start our experimentation cycle. In
+particular: * We can ask BayBE to `recommend` new experiments. * We can
+`add_measurements` for certain experimental settings to the campaign's
+database. Note that these two steps can be performed in any order. In
+particular, available measurements can be submitted at any time and also
+several times before querying the next recommendations. ```python df =
+campaign.recommend(batch_size=3) print(df) ``` ```none Granularity Pressure
+[bar] Solvent 15 medium 1.0 Solvent D 10 coarse 10.0 Solvent C 29 fine 5.0
+Solvent B ``` Note that the specific recommendations will depend on both the
+data already fed to the campaign and the random number generator seed that is
+used. After having conducted the corresponding experiments, we can add our
+measured targets to the table and feed it back to the campaign: ```python df
+["Yield"] = [79.8, 54.1, 59.4] campaign.add_measurements(df) ``` With the newly
+arrived data, BayBE can produce a refined design for the next iteration. This
+loop would typically continue until a desired target value has been achieved in
+the experiment. ### Advanced Example: Chemical Substances BayBE has several
+modules to go beyond traditional approaches. One such example is the use of
+custom encodings for categorical parameters. Chemical encodings for substances
+are a special built-in case of this that comes with BayBE. In the following
+picture you can see the outcome for treating the solvent, base and ligand in a
+direct arylation reaction optimization (from [Shields, B.J. et al.](https://
+doi.org/10.1038/s41586-021-03213-y)) with chemical encodings compared to one-
+hot and a random baseline: ![Substance Encoding Example](./examples/
+Backtesting/full_lookup_light.svg) (installation)= ## ð» Installation ###
+From Package Index The easiest way to install BayBE is via PyPI: ```bash pip
+install baybe ``` A certain released version of the package can be installed by
+specifying the corresponding version tag in the form `baybe==x.y.z`. ### From
+GitHub If you need finer control and would like to install a specific commit
+that has not been released under a certain version tag, you can do so by
+installing BayBE directly from GitHub via git and specifying the corresponding
+[git ref](https://pip.pypa.io/en/stable/topics/vcs-support/#git). For instance,
+to install the latest commit of the main branch, run: ```bash pip install
+git+https://github.com/emdgroup/baybe.git@main ``` ### From Local Clone
+Alternatively, you can install the package from your own local copy. First,
+clone the repository, navigate to the repository root folder, check out the
+desired commit, and run: ```bash pip install . ``` A developer would typically
+also install the package in editable mode ('-e'), which ensures that changes to
+the code do not require a reinstallation. ```bash pip install -e . ``` If you
+need to add additional dependencies, make sure to use the correct syntax
+including `''`: ```bash pip install -e '.[dev]' ``` ### Optional Dependencies
+There are several dependency groups that can be selected during pip
+installation, like ```bash pip install 'baybe[test,lint]' # will install baybe
+with additional dependency groups `test` and `lint` ``` To get the most out of
+`baybe`, we recommend to install at least ```bash pip install 'baybe
+[chem,simulation]' ``` The available groups are: - `chem`: Cheminformatics
+utilities (e.g. for the `SubstanceParameter`). - `docs`: Required for creating
+the documentation. - `examples`: Required for running the examples/streamlit. -
+`lint`: Required for linting and formatting. - `mypy`: Required for static type
+checking. - `onnx`: Required for using custom surrogate models in [ONNX format]
+(https://onnx.ai). - `simulation`: Enabling the [simulation](https://
+emdgroup.github.io/baybe/_autosummary/baybe.simulation.html) module. - `test`:
+Required for running the tests. - `dev`: All of the above plus `tox` and `pip-
+audit`. For code contributors. ## ð¡ Telemetry BayBE collects anonymous usage
+statistics **only** for employees of Merck KGaA, Darmstadt, Germany and/or its
+affiliates. The recording of metrics is turned off for all other users and is
+impossible due to a VPN block. In any case, the usage statistics do **not**
+involve logging of recorded measurements, targets/parameters or their names or
+any project information that would allow for reconstruction of details. The
+user and host machine names are anonymized with via truncated hashing. - You
+can verify the above statements by studying the open-source code in the
+`telemetry` module. - You can always deactivate all telemetry by setting the
+environment variable `BAYBE_TELEMETRY_ENABLED` to `false` or `off`. For details
+please consult [this page](https://emdgroup.github.io/baybe/userguide/
+envvars.html#telemetry). - If you want to be absolutely sure, you can uninstall
+internet related packages such as `opentelemetry*` or its secondary
+dependencies from the environment. Due to the inability of specifying opt-out
+dependencies, these are installed by default, but the package works without
+them. ## ð¨ð»âð§ Maintainers - Martin Fitzner (Merck KGaA, Darmstadt,
+Germany), [Contact](mailto:martin.fitzner@merckgroup.com), [Github](https://
+github.com/Scienfitz) - Adrian Å oÅ¡iÄ (Merck Life Science KGaA, Darmstadt,
+Germany), [Contact](mailto:adrian.sosic@merckgroup.com), [Github](https://
+github.com/AdrianSosic) - Alexander Hopp (Merck KGaA, Darmstadt, Germany)
+[Contact](mailto:alexander.hopp@merckgroup.com), [Github](https://github.com/
+AVHopp) ## ð ï¸ Known Issues A list of know issues can be found [here]
+(https://emdgroup.github.io/baybe/known_issues.html). ## ð License Copyright
+2022-2024 Merck KGaA, Darmstadt, Germany and/or its affiliates. All rights
+reserved. Licensed under the Apache License, Version 2.0 (the "License"); you
+may not use this file except in compliance with the License. You may obtain a
+copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
+required by applicable law or agreed to in writing, software distributed under
+the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
+CONDITIONS OF ANY KIND, either express or implied. See the License for the
+specific language governing permissions and limitations under the License.
```

### Comparing `baybe-0.8.2/baybe/__init__.py` & `baybe-0.9.0/baybe/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """BayBE — A Bayesian Back End for Design of Experiments."""
 
 import warnings
 
 from baybe.campaign import Campaign
-from baybe.deprecation import BayBE
 
 # Show deprecation warnings
 warnings.filterwarnings("default", category=DeprecationWarning, module="baybe")
 
 
 def infer_version() -> str:  # pragma: no cover
     """Determine the package version for the different ways the code can be invoked."""
@@ -48,12 +47,11 @@
     # there is no way to figure out the correct version.
     return "unknown"
 
 
 __version__ = infer_version()
 __all__ = [
     "__version__",
-    "BayBE",
     "Campaign",
 ]
 
 del infer_version
```

### Comparing `baybe-0.8.2/baybe/campaign.py` & `baybe-0.9.0/baybe/campaign.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import cattrs
 import numpy as np
 import pandas as pd
 from attrs import define, field
 
 from baybe.exceptions import DeprecationError
-from baybe.objective import Objective
+from baybe.objectives.base import Objective, to_objective
 from baybe.parameters.base import Parameter
 from baybe.recommenders.base import RecommenderProtocol
 from baybe.recommenders.meta.sequential import TwoPhaseMetaRecommender
 from baybe.searchspace.core import (
     SearchSpace,
     validate_searchspace_from_config,
 )
@@ -43,16 +43,18 @@
         * Records metadata about the progress of the experimentation process.
     """
 
     # DOE specifications
     searchspace: SearchSpace = field()
     """The search space in which the experiments are conducted."""
 
-    objective: Objective = field()
-    """The optimization objective."""
+    objective: Objective = field(converter=to_objective)
+    """The optimization objective.
+    When passing a single :class:`baybe.targets.base.Target`, it gets automatically
+    wrapped into a :class:`baybe.objectives.single.SingleTargetObjective`."""
 
     recommender: RecommenderProtocol = field(factory=TwoPhaseMetaRecommender)
     """The employed recommender"""
 
     # Metadata
     n_batches_done: int = field(default=0, init=False)
     """The number of already processed batches."""
@@ -114,20 +116,20 @@
 
     @property
     def measurements(self) -> pd.DataFrame:
         """The experimental data added to the Campaign."""
         return self._measurements_exp
 
     @property
-    def parameters(self) -> list[Parameter]:
+    def parameters(self) -> tuple[Parameter, ...]:
         """The parameters of the underlying search space."""
         return self.searchspace.parameters
 
     @property
-    def targets(self) -> list[Target]:
+    def targets(self) -> tuple[Target, ...]:
         """The targets of the underlying objective."""
         return self.objective.targets
 
     @property
     def _measurements_parameters_comp(self) -> pd.DataFrame:
         """The computational representation of the measured parameters."""
         if len(self._measurements_exp) < 1:
@@ -309,36 +311,44 @@
         telemetry_record_value(TELEM_LABELS["COUNT_RECOMMEND"], 1)
         telemetry_record_value(TELEM_LABELS["BATCH_SIZE"], batch_size)
 
         return rec
 
 
 def _add_version(dict_: dict) -> dict:
-    """Add the package version to the created dictionary."""
+    """Add the package version to the given dictionary."""
     from baybe import __version__
 
     return {**dict_, "version": __version__}
 
 
+def _drop_version(dict_: dict) -> dict:
+    """Drop the package version from the given dictionary."""
+    dict_.pop("version", None)
+    return dict_
+
+
 # Register de-/serialization hooks
 unstructure_hook = cattrs.gen.make_dict_unstructure_fn(
     Campaign,
     converter,
     _cattrs_include_init_false=True,
     # TODO: Remove once deprecation got expired:
     numerical_measurements_must_be_within_tolerance=cattrs.override(omit=True),
     strategy=cattrs.override(omit=True),
 )
 structure_hook = cattrs.gen.make_dict_structure_fn(
-    Campaign, converter, _cattrs_include_init_false=True
+    Campaign, converter, _cattrs_include_init_false=True, _cattrs_forbid_extra_keys=True
 )
 converter.register_unstructure_hook(
     Campaign, lambda x: _add_version(unstructure_hook(x))
 )
-converter.register_structure_hook(Campaign, structure_hook)
+converter.register_structure_hook(
+    Campaign, lambda d, cl: structure_hook(_drop_version(d), cl)
+)
 
 
 # Converter for config validation
 _validation_converter = converter.copy()
 _validation_converter.register_structure_hook(
     SearchSpace, validate_searchspace_from_config
 )
```

### Comparing `baybe-0.8.2/baybe/constraints/__init__.py` & `baybe-0.9.0/baybe/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/constraints/base.py` & `baybe-0.9.0/baybe/constraints/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Base classes for all constraints."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from collections.abc import Sequence
 from typing import TYPE_CHECKING, Any, ClassVar
 
 import pandas as pd
 from attr import define, field
 from attr.validators import min_len
 
 from baybe.constraints.conditions import Condition
 from baybe.parameters import NumericalContinuousParameter
 from baybe.serialization import (
     SerialMixin,
     converter,
     get_base_structure_hook,
     unstructure_base,
 )
-from baybe.utils.numerical import DTypeFloatTorch
 
 if TYPE_CHECKING:
     from torch import Tensor
 
 
 @define
 class Constraint(ABC, SerialMixin):
@@ -144,15 +144,15 @@
 
     @coefficients.default
     def _default_coefficients(self):
         """Return equal weight coefficients as default."""
         return [1.0] * len(self.parameters)
 
     def to_botorch(
-        self, parameters: list[NumericalContinuousParameter], idx_offset: int = 0
+        self, parameters: Sequence[NumericalContinuousParameter], idx_offset: int = 0
     ) -> tuple[Tensor, Tensor, float]:
         """Cast the constraint in a format required by botorch.
 
         Used in calling ``optimize_acqf_*`` functions, for details see
         https://botorch.org/api/optim.html#botorch.optim.optimize.optimize_acqf
 
         Args:
@@ -160,21 +160,24 @@
             idx_offset: Offset to the provided parameter indices.
 
         Returns:
             The tuple required by botorch.
         """
         import torch
 
+        from baybe.utils.torch import DTypeFloatTorch
+
         param_names = [p.name for p in parameters]
         param_indices = [
             param_names.index(p) + idx_offset
             for p in self.parameters
             if p in param_names
         ]
 
+        # TODO: Cast rhs to correct precision once BoTorch also supports single point.
         return (
             torch.tensor(param_indices),
             torch.tensor(self.coefficients, dtype=DTypeFloatTorch),
             self.rhs,
         )
```

### Comparing `baybe-0.8.2/baybe/constraints/conditions.py` & `baybe-0.9.0/baybe/constraints/conditions.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/constraints/continuous.py` & `baybe-0.9.0/baybe/constraints/continuous.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/constraints/discrete.py` & `baybe-0.9.0/baybe/constraints/discrete.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/constraints/validation.py` & `baybe-0.9.0/baybe/constraints/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Validation functionality for constraints."""
 
+from collections.abc import Collection
 
 from baybe.constraints.base import Constraint
 from baybe.constraints.discrete import DiscreteDependenciesConstraint
-from baybe.parameters.base import ContinuousParameter, DiscreteParameter, Parameter
+from baybe.parameters.base import Parameter
 
 
 def validate_constraints(  # noqa: DOC101, DOC103
-    constraints: list[Constraint], parameters: list[Parameter]
+    constraints: Collection[Constraint], parameters: Collection[Parameter]
 ) -> None:
     """Assert that a given collection of constraints is valid.
 
     Raises:
         ValueError: If there is more than one
             :class:`baybe.constraints.discrete.DiscreteDependenciesConstraint` declared.
         ValueError: If any constraint contains an invalid parameter name.
@@ -21,20 +22,16 @@
     if sum(isinstance(itm, DiscreteDependenciesConstraint) for itm in constraints) > 1:
         raise ValueError(
             f"There is only one {DiscreteDependenciesConstraint.__name__} allowed. "
             f"Please specify all dependencies in one single constraint."
         )
 
     param_names_all = [p.name for p in parameters]
-    param_names_discrete = [
-        p.name for p in parameters if isinstance(p, DiscreteParameter)
-    ]
-    param_names_continuous = [
-        p.name for p in parameters if isinstance(p, ContinuousParameter)
-    ]
+    param_names_discrete = [p.name for p in parameters if p.is_discrete]
+    param_names_continuous = [p.name for p in parameters if p.is_continuous]
     for constraint in constraints:
         if not all(p in param_names_all for p in constraint.parameters):
             raise ValueError(
                 f"You are trying to create a constraint with at least one parameter "
                 f"name that does not exist in the list of defined parameters. "
                 f"Parameter list of the affected constraint: {constraint.parameters}"
             )
```

### Comparing `baybe-0.8.2/baybe/deprecation.py` & `baybe-0.9.0/baybe/deprecation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,11 @@
 """Temporary name aliases for backward compatibility."""
 
 import warnings
 
-from attrs import define
-
-from baybe import Campaign
-
-
-@define
-class BayBE(Campaign):
-    """A :class:`baybe.campaign.Campaign` alias for backward compatibility."""
-
-    def __attrs_pre_init__(self):
-        warnings.warn(
-            "The 'BayBE' class is deprecated and will be removed in a future version. "
-            "Please use the 'Campaign' class instead.",
-            DeprecationWarning,
-        )
-
 
 def compatibilize_config(config: dict) -> dict:
     """Turn a legacy-format config into the new format."""
     if "parameters" not in config:
         return config
 
     if "searchspace" in config:
```

### Comparing `baybe-0.8.2/baybe/exceptions.py` & `baybe-0.9.0/baybe/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,14 @@
     """The created search space contains no parameters."""
 
 
 class NothingToSimulateError(Exception):
     """There is nothing to simulate because there are no testable configurations."""
 
 
-# TODO: This exception class is needed only temporarily in `CustomONNXSurrogate` until
-#   the use of `model_params` has be refactored.
-class ModelParamsNotSupportedError(Exception):
-    """The class does not support any model parameters."""
-
-
 class NoRecommendersLeftError(Exception):
     """A recommender is requested by a meta recommender but there are no recommenders
     left.
     """
 
 
 class NumericalUnderflowError(Exception):
@@ -48,7 +42,11 @@
 
 class OptionalImportError(Exception):
     """An attempt was made to import an optional but uninstalled dependency."""
 
 
 class DeprecationError(Exception):
     """Signals the use of a deprecated mechanism to the user, interrupting execution."""
+
+
+class UnidentifiedSubclassError(Exception):
+    """A specified subclass cannot be found in the given class hierarchy."""
```

### Comparing `baybe-0.8.2/baybe/parameters/__init__.py` & `baybe-0.9.0/baybe/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/parameters/base.py` & `baybe-0.9.0/baybe/parameters/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,24 @@
     @abstractmethod
     def summary(self) -> dict:
         """Return a custom summarization of the parameter."""
 
     def __str__(self) -> str:
         return str(self.summary())
 
+    @property
+    def is_continuous(self) -> bool:
+        """Boolean indicating if this is a continuous parameter."""
+        return isinstance(self, ContinuousParameter)
+
+    @property
+    def is_discrete(self) -> bool:
+        """Boolean indicating if this is a discrete parameter."""
+        return isinstance(self, DiscreteParameter)
+
 
 @define(frozen=True, slots=False)
 class DiscreteParameter(Parameter, ABC):
     """Abstract class for discrete parameters."""
 
     # TODO [15280]: needs to be refactored
```

### Comparing `baybe-0.8.2/baybe/parameters/categorical.py` & `baybe-0.9.0/baybe/parameters/categorical.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/parameters/custom.py` & `baybe-0.9.0/baybe/parameters/custom.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/parameters/enum.py` & `baybe-0.9.0/baybe/parameters/enum.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/parameters/numerical.py` & `baybe-0.9.0/baybe/parameters/numerical.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/parameters/substance.py` & `baybe-0.9.0/baybe/parameters/substance.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/parameters/utils.py` & `baybe-0.9.0/baybe/parameters/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 _TParameter = TypeVar("_TParameter", bound=Parameter)
 
 
 def get_parameters_from_dataframe(
     df: pd.DataFrame,
     factory: Callable[[str, Collection[Any]], _TParameter],
-    parameters: Optional[list[_TParameter]] = None,
+    parameters: Optional[Collection[_TParameter]] = None,
 ) -> list[_TParameter]:
     """Create a list of parameters from a dataframe.
 
     Returns one parameter for each column of the given dataframe. By default,
     the parameters are created using the provided factory, which takes the name
     of the column and its unique values as arguments. However, there is also
     the possibility to provide explicit parameter objects with names matching specific
```

### Comparing `baybe-0.8.2/baybe/parameters/validation.py` & `baybe-0.9.0/baybe/parameters/validation.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/recommenders/__init__.py` & `baybe-0.9.0/baybe/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/recommenders/base.py` & `baybe-0.9.0/baybe/recommenders/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,11 +39,12 @@
     RecommenderProtocol,
     lambda x: unstructure_base(
         x,
         # TODO: Remove once deprecation got expired:
         overrides=dict(
             allow_repeated_recommendations=cattrs.override(omit=True),
             allow_recommending_already_measured=cattrs.override(omit=True),
+            acquisition_function_cls=cattrs.override(omit=True),
         ),
     ),
 )
 converter.register_structure_hook(RecommenderProtocol, structure_recommender_protocol)
```

### Comparing `baybe-0.8.2/baybe/recommenders/deprecation.py` & `baybe-0.9.0/baybe/recommenders/deprecation.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 def structure_recommender_protocol(val: dict, _) -> RecommenderProtocol:
     """A structure hook using ``TwoPhaseMetaRecommender`` as fallback type."""  # noqa: D401 (imperative mood)
     from baybe.recommenders.base import RecommenderProtocol
     from baybe.recommenders.meta.sequential import TwoPhaseMetaRecommender
 
     try:
-        _type = val["type"]
+        val = val.copy()
+        _type = val.pop("type")
         cls = next(
             (cl for cl in get_subclasses(RecommenderProtocol) if cl.__name__ == _type),
             None,
         )
         if cls is None:
             raise ValueError(f"Unknown subclass '{_type}'.")
     except KeyError:
@@ -32,10 +33,10 @@
         warnings.warn(
             f"A recommender has been specified without a corresponding type. "
             f"As a fallback, '{TwoPhaseMetaRecommender.__name__}' is used. "
             f"However, this behavior is deprecated and will be disabled in "
             f"a future version.",
             DeprecationWarning,
         )
-    fun = make_dict_structure_fn(cls, converter)  # type: ignore
+    fun = make_dict_structure_fn(cls, converter, _cattrs_forbid_extra_keys=True)  # type: ignore
 
     return fun(val, cls)
```

### Comparing `baybe-0.8.2/baybe/recommenders/meta/base.py` & `baybe-0.9.0/baybe/recommenders/meta/base.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/recommenders/meta/sequential.py` & `baybe-0.9.0/baybe/recommenders/meta/sequential.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/recommenders/naive.py` & `baybe-0.9.0/baybe/recommenders/naive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Naive recommender for hybrid spaces."""
 
 import warnings
-from typing import ClassVar, Optional, cast
+from typing import ClassVar, Optional
 
 import pandas as pd
 from attrs import define, evolve, field, fields
-from torch import Tensor
 
-from baybe.acquisition import PartialAcquisitionFunction
 from baybe.recommenders.pure.base import PureRecommender
 from baybe.recommenders.pure.bayesian.base import BayesianRecommender
 from baybe.recommenders.pure.bayesian.sequential_greedy import (
     SequentialGreedyRecommender,
 )
 from baybe.recommenders.pure.nonpredictive.base import NonPredictiveRecommender
 from baybe.searchspace import SearchSpace, SearchSpaceType
@@ -82,14 +80,16 @@
         searchspace: SearchSpace,
         batch_size: int = 1,
         train_x: Optional[pd.DataFrame] = None,
         train_y: Optional[pd.DataFrame] = None,
     ) -> pd.DataFrame:
         # See base class.
 
+        from baybe.acquisition.partial import PartialAcquisitionFunction
+
         if (not isinstance(self.disc_recommender, BayesianRecommender)) and (
             not isinstance(self.disc_recommender, NonPredictiveRecommender)
         ):
             raise NotImplementedError(
                 """The discrete recommender should be either a Bayesian or a
                 NonPredictiveRecommender."""
             )
@@ -112,63 +112,61 @@
         # We are in a hybrid setting now
 
         # We will attach continuous parts to discrete parts and the other way round.
         # To make things simple, we sample a single point in the continuous space which
         # will then be attached to every discrete point when the acquisition function
         # is evaluated.
         cont_part = searchspace.continuous.samples_random(1)
-        cont_part_tensor = cast(Tensor, to_tensor(cont_part)).unsqueeze(-2)
+        cont_part_tensor = to_tensor(cont_part).unsqueeze(-2)
 
         # Get discrete candidates. The metadata flags are ignored since the search space
         # is hybrid
         # TODO Slight BOILERPLATE CODE, see recommender.py, ll. 47+
         _, candidates_comp = searchspace.discrete.get_candidates(
             allow_repeated_recommendations=True,
             allow_recommending_already_measured=True,
         )
 
         # We now check whether the discrete recommender is bayesian.
         if isinstance(self.disc_recommender, BayesianRecommender):
             # Get access to the recommenders acquisition function
-            self.disc_recommender.setup_acquisition_function(
-                searchspace, train_x, train_y
-            )
+            self.disc_recommender._setup_botorch_acqf(searchspace, train_x, train_y)
 
             # Construct the partial acquisition function that attaches cont_part
             # whenever evaluating the acquisition function
             disc_acqf_part = PartialAcquisitionFunction(
-                acqf=self.disc_recommender._acquisition_function,
+                botorch_acqf=self.disc_recommender._botorch_acqf,
                 pinned_part=cont_part_tensor,
                 pin_discrete=False,
             )
 
-            self.disc_recommender._acquisition_function = disc_acqf_part
+            self.disc_recommender._botorch_acqf = disc_acqf_part
 
         # Call the private function of the discrete recommender and get the indices
         disc_rec_idx = self.disc_recommender._recommend_discrete(
             subspace_discrete=searchspace.discrete,
             candidates_comp=candidates_comp,
             batch_size=batch_size,
         )
 
         # Get one random discrete point that will be attached when evaluating the
         # acquisition function in the discrete space.
         disc_part = searchspace.discrete.comp_rep.loc[disc_rec_idx].sample(1)
-        disc_part_tensor = cast(Tensor, to_tensor(disc_part)).unsqueeze(-2)
+        disc_part_tensor = to_tensor(disc_part).unsqueeze(-2)
 
         # Setup a fresh acquisition function for the continuous recommender
-        self.cont_recommender.setup_acquisition_function(searchspace, train_x, train_y)
+        self.cont_recommender._setup_botorch_acqf(searchspace, train_x, train_y)
 
         # Construct the continuous space as a standalone space
         cont_acqf_part = PartialAcquisitionFunction(
-            acqf=self.cont_recommender._acquisition_function,
+            botorch_acqf=self.cont_recommender._botorch_acqf,
             pinned_part=disc_part_tensor,
             pin_discrete=True,
         )
-        self.cont_recommender._acquisition_function = cont_acqf_part
+        self.cont_recommender._botorch_acqf = cont_acqf_part
 
         # Call the private function of the continuous recommender
         rec_cont = self.cont_recommender._recommend_continuous(
             searchspace.continuous, batch_size
         )
 
         # Glue the solutions together and return them
```

### Comparing `baybe-0.8.2/baybe/recommenders/pure/__init__.py` & `baybe-0.9.0/baybe/recommenders/pure/__init__.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/recommenders/pure/base.py` & `baybe-0.9.0/baybe/recommenders/pure/base.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/recommenders/pure/bayesian/base.py` & `baybe-0.9.0/baybe/recommenders/pure/bayesian/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 """Base class for all Bayesian recommenders."""
 
 from abc import ABC
-from functools import partial
-from typing import Callable, Literal, Optional
+from typing import Optional
 
 import pandas as pd
 from attrs import define, field
-from botorch.acquisition import (
-    AcquisitionFunction,
-    ExpectedImprovement,
-    PosteriorMean,
-    ProbabilityOfImprovement,
-    UpperConfidenceBound,
-    qExpectedImprovement,
-    qProbabilityOfImprovement,
-    qUpperConfidenceBound,
-)
 
-from baybe.acquisition import debotorchize
+from baybe.acquisition.acqfs import qExpectedImprovement
+from baybe.acquisition.base import AcquisitionFunction
+from baybe.acquisition.utils import convert_acqf
+from baybe.exceptions import DeprecationError
 from baybe.recommenders.pure.base import PureRecommender
 from baybe.searchspace import SearchSpace
 from baybe.surrogates import _ONNX_INSTALLED, GaussianProcessSurrogate
 from baybe.surrogates.base import Surrogate
 from baybe.utils.dataframe import to_tensor
 
 if _ONNX_INSTALLED:
@@ -31,47 +23,35 @@
 @define
 class BayesianRecommender(PureRecommender, ABC):
     """An abstract class for Bayesian Recommenders."""
 
     surrogate_model: Surrogate = field(factory=GaussianProcessSurrogate)
     """The used surrogate model."""
 
-    acquisition_function_cls: Literal[
-        "PM", "PI", "EI", "UCB", "qPI", "qEI", "qUCB", "VarUCB", "qVarUCB"
-    ] = field(default="qEI")
+    acquisition_function: AcquisitionFunction = field(
+        converter=convert_acqf, factory=qExpectedImprovement, kw_only=True
+    )
     """The used acquisition function class."""
 
-    _acquisition_function: Optional[AcquisitionFunction] = field(
-        default=None, init=False
-    )
+    _botorch_acqf = field(default=None, init=False)
     """The current acquisition function."""
 
-    def _get_acquisition_function_cls(
-        self,
-    ) -> Callable:
-        """Get the actual acquisition function class.
+    acquisition_function_cls: bool = field(default=None)
+    "Deprecated! Raises an error when used."
 
-        Returns:
-            The debotorchized acquisition function class.
-        """
-        mapping = {
-            "PM": PosteriorMean,
-            "PI": ProbabilityOfImprovement,
-            "EI": ExpectedImprovement,
-            "UCB": partial(UpperConfidenceBound, beta=1.0),
-            "qEI": qExpectedImprovement,
-            "qPI": qProbabilityOfImprovement,
-            "qUCB": partial(qUpperConfidenceBound, beta=1.0),
-            "VarUCB": partial(UpperConfidenceBound, beta=100.0),
-            "qVarUCB": partial(qUpperConfidenceBound, beta=100.0),
-        }
-        fun = debotorchize(mapping[self.acquisition_function_cls])
-        return fun
+    @acquisition_function_cls.validator
+    def _validate_deprecated_argument(self, _, value) -> None:
+        """Raise DeprecationError if old acquisition_function_cls parameter is used."""
+        if value is not None:
+            raise DeprecationError(
+                "Passing 'acquisition_function_cls' to the constructor is deprecated. "
+                "The parameter has been renamed to 'acquisition_function'."
+            )
 
-    def setup_acquisition_function(
+    def _setup_botorch_acqf(
         self,
         searchspace: SearchSpace,
         train_x: Optional[pd.DataFrame] = None,
         train_y: Optional[pd.DataFrame] = None,
     ) -> None:
         """Create the current acquisition function from provided training data.
 
@@ -87,19 +67,18 @@
             NotImplementedError: If the setup is attempted from empty training data
         """
         if train_x is None or train_y is None:
             raise NotImplementedError(
                 "Bayesian recommenders do not support empty training data yet."
             )
 
-        best_f = train_y.max().item()
         surrogate_model = self._fit(searchspace, train_x, train_y)
-        acquisition_function_cls = self._get_acquisition_function_cls()
-
-        self._acquisition_function = acquisition_function_cls(surrogate_model, best_f)
+        self._botorch_acqf = self.acquisition_function.to_botorch(
+            surrogate_model, train_x, train_y
+        )
 
     def _fit(
         self,
         searchspace: SearchSpace,
         train_x: pd.DataFrame,
         train_y: pd.DataFrame,
     ) -> Surrogate:
@@ -132,10 +111,10 @@
         train_y: Optional[pd.DataFrame] = None,
     ) -> pd.DataFrame:
         # See base class.
 
         if _ONNX_INSTALLED and isinstance(self.surrogate_model, CustomONNXSurrogate):
             CustomONNXSurrogate.validate_compatibility(searchspace)
 
-        self.setup_acquisition_function(searchspace, train_x, train_y)
+        self._setup_botorch_acqf(searchspace, train_x, train_y)
 
         return super().recommend(searchspace, batch_size, train_x, train_y)
```

### Comparing `baybe-0.8.2/baybe/recommenders/pure/bayesian/sequential_greedy.py` & `baybe-0.9.0/baybe/recommenders/pure/bayesian/sequential_greedy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Sequential greedy recommender."""
 
 from typing import Any, ClassVar
 
 import pandas as pd
 from attrs import define, field, validators
-from botorch.optim import optimize_acqf, optimize_acqf_discrete, optimize_acqf_mixed
 
 from baybe.exceptions import NoMCAcquisitionFunctionError
 from baybe.recommenders.pure.bayesian.base import BayesianRecommender
 from baybe.searchspace import (
     SearchSpace,
     SearchSpaceType,
     SubspaceContinuous,
@@ -63,27 +62,45 @@
 
     def _recommend_discrete(
         self,
         subspace_discrete: SubspaceDiscrete,
         candidates_comp: pd.DataFrame,
         batch_size: int,
     ) -> pd.Index:
-        # See base class.
+        """Generate recommendations from a discrete search space.
 
-        # determine the next set of points to be tested
-        candidates_tensor = to_tensor(candidates_comp)
-        try:
-            points, _ = optimize_acqf_discrete(
-                self._acquisition_function, batch_size, candidates_tensor
-            )
-        except AttributeError as ex:
+        Args:
+            subspace_discrete: The discrete subspace from which to generate
+                recommendations.
+            candidates_comp: The computational representation of all discrete candidate
+                points to be considered.
+            batch_size: The size of the recommendation batch.
+
+        Raises:
+            NoMCAcquisitionFunctionError: If a non-Monte Carlo acquisition function is
+                used with a batch size > 1.
+
+        Returns:
+            The dataframe indices of the recommended points in the provided
+            computational representation.
+        """
+        # For batch size > 1, this optimizer needs a MC acquisition function
+        if batch_size > 1 and not self.acquisition_function.is_mc:
             raise NoMCAcquisitionFunctionError(
                 f"The '{self.__class__.__name__}' only works with Monte Carlo "
-                f"acquisition functions."
-            ) from ex
+                f"acquisition functions for batch sizes > 1."
+            )
+
+        from botorch.optim import optimize_acqf_discrete
+
+        # determine the next set of points to be tested
+        candidates_tensor = to_tensor(candidates_comp)
+        points, _ = optimize_acqf_discrete(
+            self._botorch_acqf, batch_size, candidates_tensor
+        )
 
         # retrieve the index of the points from the input dataframe
         # IMPROVE: The merging procedure is conceptually similar to what
         #   `SearchSpace._match_measurement_with_searchspace_indices` does, though using
         #   a simpler matching logic. When refactoring the SearchSpace class to
         #   handle continuous parameters, a corresponding utility could be extracted.
         idxs = pd.Index(
@@ -97,40 +114,55 @@
         return idxs
 
     def _recommend_continuous(
         self,
         subspace_continuous: SubspaceContinuous,
         batch_size: int,
     ) -> pd.DataFrame:
-        # See base class.
-        import torch
+        """Generate recommendations from a continuous search space.
 
-        try:
-            points, _ = optimize_acqf(
-                acq_function=self._acquisition_function,
-                bounds=torch.from_numpy(subspace_continuous.param_bounds_comp),
-                q=batch_size,
-                num_restarts=5,  # TODO make choice for num_restarts
-                raw_samples=10,  # TODO make choice for raw_samples
-                equality_constraints=[
-                    c.to_botorch(subspace_continuous.parameters)
-                    for c in subspace_continuous.constraints_lin_eq
-                ]
-                or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
-                inequality_constraints=[
-                    c.to_botorch(subspace_continuous.parameters)
-                    for c in subspace_continuous.constraints_lin_ineq
-                ]
-                or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
-            )
-        except AttributeError as ex:
+        Args:
+            subspace_continuous: The continuous subspace from which to generate
+                recommendations.
+            batch_size: The size of the recommendation batch.
+
+        Raises:
+            NoMCAcquisitionFunctionError: If a non-Monte Carlo acquisition function is
+                used with a batch size > 1.
+
+        Returns:
+            A dataframe containing the recommendations as individual rows.
+        """
+        # For batch size > 1, this optimizer needs a MC acquisition function
+        if batch_size > 1 and not self.acquisition_function.is_mc:
             raise NoMCAcquisitionFunctionError(
                 f"The '{self.__class__.__name__}' only works with Monte Carlo "
-                f"acquisition functions."
-            ) from ex
+                f"acquisition functions for batch sizes > 1."
+            )
+
+        import torch
+        from botorch.optim import optimize_acqf
+
+        points, _ = optimize_acqf(
+            acq_function=self._botorch_acqf,
+            bounds=torch.from_numpy(subspace_continuous.param_bounds_comp),
+            q=batch_size,
+            num_restarts=5,  # TODO make choice for num_restarts
+            raw_samples=10,  # TODO make choice for raw_samples
+            equality_constraints=[
+                c.to_botorch(subspace_continuous.parameters)
+                for c in subspace_continuous.constraints_lin_eq
+            ]
+            or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
+            inequality_constraints=[
+                c.to_botorch(subspace_continuous.parameters)
+                for c in subspace_continuous.constraints_lin_ineq
+            ]
+            or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
+        )
 
         # Return optimized points as dataframe
         rec = pd.DataFrame(points, columns=subspace_continuous.param_names)
         return rec
 
     def _recommend_hybrid(
         self,
@@ -149,22 +181,30 @@
 
         Args:
             searchspace: The search space in which the recommendations should be made.
             candidates_comp: The computational representation of the candidates
                 of the discrete subspace.
             batch_size: The size of the calculated batch.
 
+        Raises:
+            NoMCAcquisitionFunctionError: If a non-Monte Carlo acquisition function is
+                used with a batch size > 1.
+
         Returns:
             The recommended points.
-
-        Raises:
-            NoMCAcquisitionFunctionError: If a non Monte Carlo acquisition function
-                is chosen.
         """
+        # For batch size > 1, this optimizer needs a MC acquisition function
+        if batch_size > 1 and not self.acquisition_function.is_mc:
+            raise NoMCAcquisitionFunctionError(
+                f"The '{self.__class__.__name__}' only works with Monte Carlo "
+                f"acquisition functions for batch sizes > 1."
+            )
+
         import torch
+        from botorch.optim import optimize_acqf_mixed
 
         if len(candidates_comp) > 0:
             # Calculate the number of samples from the given percentage
             n_candidates = int(self.sampling_percentage * len(candidates_comp.index))
 
             # Potential sampling of discrete candidates
             if self.hybrid_sampler == "Farthest":
@@ -181,44 +221,38 @@
             num_comp_columns = len(candidates_comp.columns)
             candidates_comp.columns = list(range(num_comp_columns))  # type: ignore
             fixed_features_list = candidates_comp.to_dict("records")
         else:
             fixed_features_list = None
 
         # Actual call of the BoTorch optimization routine
-        try:
-            points, _ = optimize_acqf_mixed(
-                acq_function=self._acquisition_function,
-                bounds=torch.from_numpy(searchspace.param_bounds_comp),
-                q=batch_size,
-                num_restarts=5,  # TODO make choice for num_restarts
-                raw_samples=10,  # TODO make choice for raw_samples
-                fixed_features_list=fixed_features_list,
-                equality_constraints=[
-                    c.to_botorch(
-                        searchspace.continuous.parameters,
-                        idx_offset=len(candidates_comp.columns),
-                    )
-                    for c in searchspace.continuous.constraints_lin_eq
-                ]
-                or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
-                inequality_constraints=[
-                    c.to_botorch(
-                        searchspace.continuous.parameters,
-                        idx_offset=num_comp_columns,
-                    )
-                    for c in searchspace.continuous.constraints_lin_ineq
-                ]
-                or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
-            )
-        except AttributeError as ex:
-            raise NoMCAcquisitionFunctionError(
-                f"The '{self.__class__.__name__}' only works with Monte Carlo "
-                f"acquisition functions."
-            ) from ex
+        points, _ = optimize_acqf_mixed(
+            acq_function=self._botorch_acqf,
+            bounds=torch.from_numpy(searchspace.param_bounds_comp),
+            q=batch_size,
+            num_restarts=5,  # TODO make choice for num_restarts
+            raw_samples=10,  # TODO make choice for raw_samples
+            fixed_features_list=fixed_features_list,
+            equality_constraints=[
+                c.to_botorch(
+                    searchspace.continuous.parameters,
+                    idx_offset=len(candidates_comp.columns),
+                )
+                for c in searchspace.continuous.constraints_lin_eq
+            ]
+            or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
+            inequality_constraints=[
+                c.to_botorch(
+                    searchspace.continuous.parameters,
+                    idx_offset=num_comp_columns,
+                )
+                for c in searchspace.continuous.constraints_lin_ineq
+            ]
+            or None,  # TODO: https://github.com/pytorch/botorch/issues/2042
+        )
 
         disc_points = points[:, :num_comp_columns]
         cont_points = points[:, num_comp_columns:]
 
         # Get selected candidate indices
         idxs = pd.Index(
             pd.merge(
```

### Comparing `baybe-0.8.2/baybe/recommenders/pure/nonpredictive/clustering.py` & `baybe-0.9.0/baybe/recommenders/pure/nonpredictive/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     """Class variable describing the name of the clustering parameter."""
 
     _use_custom_selector: ClassVar[bool] = False
     """Class variable flagging whether a custom selector is being used."""
 
     # Object variables
     model_params: dict = field(factory=dict)
-    """The parameters for the used model. This is initialized with reasonable default
-    values for the derived child classes."""
+    """Optional model parameter that will be passed to the surrogate constructor.
+    This is initialized with reasonable default values for the derived child classes."""
 
     def _make_selection_default(
         self,
         model: ClusterMixin,
         candidates_scaled: Union[pd.DataFrame, np.ndarray],
     ) -> list[int]:
         """Select one candidate from each cluster uniformly at random.
```

### Comparing `baybe-0.8.2/baybe/recommenders/pure/nonpredictive/sampling.py` & `baybe-0.9.0/baybe/recommenders/pure/nonpredictive/sampling.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/scaler.py` & `baybe-0.9.0/baybe/scaler.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/searchspace/continuous.py` & `baybe-0.9.0/baybe/searchspace/continuous.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 """Continuous subspaces."""
 
 from __future__ import annotations
 
-from collections.abc import Collection
-from typing import Any, Optional
+from collections.abc import Collection, Sequence
+from typing import Any, Optional, cast
 
 import numpy as np
 import pandas as pd
 from attr import define, field
 
 from baybe.constraints import (
     ContinuousLinearEqualityConstraint,
     ContinuousLinearInequalityConstraint,
 )
 from baybe.parameters import NumericalContinuousParameter
+from baybe.parameters.base import ContinuousParameter
 from baybe.parameters.utils import get_parameters_from_dataframe
 from baybe.searchspace.validation import validate_parameter_names
 from baybe.serialization import SerialMixin, converter, select_constructor_hook
+from baybe.utils.basic import to_tuple
 from baybe.utils.dataframe import pretty_print_df
 from baybe.utils.numerical import DTypeFloatNumpy
 
 
 @define
 class SubspaceContinuous(SerialMixin):
     """Class for managing continuous subspaces.
 
     Builds the subspace from parameter definitions, keeps
     track of search metadata, and provides access to candidate sets and different
     parameter views.
     """
 
-    parameters: list[NumericalContinuousParameter] = field(
-        validator=lambda _1, _2, x: validate_parameter_names(x)
+    parameters: tuple[NumericalContinuousParameter, ...] = field(
+        converter=to_tuple, validator=lambda _, __, x: validate_parameter_names(x)
     )
     """The list of parameters of the subspace."""
 
-    constraints_lin_eq: list[ContinuousLinearEqualityConstraint] = field(factory=list)
+    constraints_lin_eq: tuple[ContinuousLinearEqualityConstraint, ...] = field(
+        converter=to_tuple, factory=tuple
+    )
     """List of linear equality constraints."""
 
-    constraints_lin_ineq: list[ContinuousLinearInequalityConstraint] = field(
-        factory=list
+    constraints_lin_ineq: tuple[ContinuousLinearInequalityConstraint, ...] = field(
+        converter=to_tuple, factory=tuple
     )
     """List of linear inequality constraints."""
 
     def __str__(self) -> str:
         if self.is_empty:
             return ""
 
@@ -88,24 +92,24 @@
         # Assert that the input represents valid bounds
         assert bounds.shape[0] == 2
         assert (np.diff(bounds.values, axis=0) >= 0).all()
         assert bounds.apply(pd.api.types.is_numeric_dtype).all()
 
         # Create the corresponding parameters and from them the search space
         parameters = [
-            NumericalContinuousParameter(name, bound)
+            NumericalContinuousParameter(cast(str, name), bound)
             for (name, bound) in bounds.items()
         ]
         return SubspaceContinuous(parameters)
 
     @classmethod
     def from_dataframe(
         cls,
         df: pd.DataFrame,
-        parameters: Optional[list[NumericalContinuousParameter]] = None,
+        parameters: Optional[Sequence[ContinuousParameter]] = None,
     ) -> SubspaceContinuous:
         """Create a hyperrectangle-shaped continuous subspace from a dataframe.
 
         More precisely, create the smallest axis-aligned hyperrectangle-shaped
         continuous subspace that contains the points specified in the given dataframe.
 
         Args:
@@ -115,19 +119,32 @@
                 attributes. If a match between column name and parameter name is found,
                 the corresponding parameter object is used. If a column has no match in
                 the parameter list, a new
                 :class:`baybe.parameters.numerical.NumericalContinuousParameter`
                 is created with default optional arguments. For more details, see
                 :func:`baybe.parameters.utils.get_parameters_from_dataframe`.
 
+        Raises:
+            ValueError: If parameter types other than
+                :class:`baybe.parameters.numerical.NumericalContinuousParameter`
+                are provided.
+
         Returns:
             The created continuous subspace.
         """
         # TODO: Add option for convex hull once constraints are in place
 
+        if parameters and not all(
+            isinstance(p, NumericalContinuousParameter) for p in parameters
+        ):
+            raise ValueError(
+                "Currently, only parameters of type "
+                "'{NumericalContinuousParameter.__name__}' are supported."
+            )
+
         def continuous_parameter_factory(name: str, values: Collection[Any]):
             return NumericalContinuousParameter(name, (min(values), max(values)))
 
         # Get the full list of both explicitly and implicitly defined parameter
         parameters = get_parameters_from_dataframe(
             df, continuous_parameter_factory, parameters
         )
@@ -136,17 +153,17 @@
 
     @property
     def is_empty(self) -> bool:
         """Return whether this subspace is empty."""
         return len(self.parameters) == 0
 
     @property
-    def param_names(self) -> list[str]:
+    def param_names(self) -> tuple[str, ...]:
         """Return list of parameter names."""
-        return [p.name for p in self.parameters]
+        return tuple(p.name for p in self.parameters)
 
     @property
     def param_bounds_comp(self) -> np.ndarray:
         """Return bounds as numpy array."""
         if not self.parameters:
             return np.empty((2, 0), dtype=DTypeFloatNumpy)
         return np.stack([p.bounds.to_ndarray() for p in self.parameters]).T
```

### Comparing `baybe-0.8.2/baybe/searchspace/core.py` & `baybe-0.9.0/baybe/searchspace/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Functionality for managing search spaces."""
 
 from __future__ import annotations
 
+from collections.abc import Iterable, Sequence
 from enum import Enum
 from typing import Optional, cast
 
 import numpy as np
 import pandas as pd
 from attr import define, field
 
 from baybe.constraints import (
     ContinuousLinearEqualityConstraint,
     ContinuousLinearInequalityConstraint,
     validate_constraints,
 )
-from baybe.constraints.base import Constraint, DiscreteConstraint
+from baybe.constraints.base import Constraint
 from baybe.parameters import (
     SubstanceEncoding,
     TaskParameter,
 )
-from baybe.parameters.base import ContinuousParameter, DiscreteParameter, Parameter
+from baybe.parameters.base import Parameter
 from baybe.searchspace.continuous import SubspaceContinuous
 from baybe.searchspace.discrete import (
+    MemorySize,
     SubspaceDiscrete,
     validate_simplex_subspace_from_config,
 )
 from baybe.searchspace.validation import validate_parameters
 from baybe.serialization import SerialMixin, converter, select_constructor_hook
 from baybe.telemetry import TELEM_LABELS, telemetry_record_value
 
@@ -95,16 +97,16 @@
             TELEM_LABELS["NUM_CONSTRAINTS"],
             len(self.constraints) if self.constraints else 0,
         )
 
     @classmethod
     def from_product(
         cls,
-        parameters: list[Parameter],
-        constraints: Optional[list[Constraint]] = None,
+        parameters: Sequence[Parameter],
+        constraints: Optional[Sequence[Constraint]] = None,
         empty_encoding: bool = False,
     ) -> SearchSpace:
         """Create a search space from a cartesian product.
 
         In the search space, optional subsequent constraints are applied.
         That is, the discrete subspace becomes the (filtered) cartesian product
         containing all discrete parameter combinations while, analogously, the
@@ -131,41 +133,39 @@
         validate_parameters(parameters)
         if constraints:
             validate_constraints(constraints, parameters)
         else:
             constraints = []
 
         discrete: SubspaceDiscrete = SubspaceDiscrete.from_product(
-            parameters=[p for p in parameters if isinstance(p, DiscreteParameter)],
-            constraints=[
-                cast(DiscreteConstraint, c) for c in constraints if c.is_discrete
-            ],
+            parameters=[p for p in parameters if p.is_discrete],  # type:ignore[misc]
+            constraints=[c for c in constraints if c.is_discrete],  # type:ignore[misc]
             empty_encoding=empty_encoding,
         )
         continuous: SubspaceContinuous = SubspaceContinuous(
-            parameters=[p for p in parameters if isinstance(p, ContinuousParameter)],
-            constraints_lin_eq=[
-                cast(ContinuousLinearEqualityConstraint, c)
+            parameters=[p for p in parameters if p.is_continuous],  # type:ignore[misc]
+            constraints_lin_eq=[  # type:ignore[misc]
+                c
                 for c in constraints
                 if isinstance(c, ContinuousLinearEqualityConstraint)
             ],
-            constraints_lin_ineq=[
-                cast(ContinuousLinearInequalityConstraint, c)
+            constraints_lin_ineq=[  # type:ignore[misc]
+                c
                 for c in constraints
                 if isinstance(c, ContinuousLinearInequalityConstraint)
             ],
         )
 
         return SearchSpace(discrete=discrete, continuous=continuous)
 
     @classmethod
     def from_dataframe(
         cls,
         df: pd.DataFrame,
-        parameters: list[Parameter],
+        parameters: Sequence[Parameter],
     ) -> SearchSpace:
         """Create a search space from a specified set of parameter configurations.
 
         The way in which the contents of the columns are interpreted depends on the
         types of the corresponding parameter objects provided. For details, see
         :meth:`baybe.searchspace.discrete.SubspaceDiscrete.from_dataframe` and
         :meth:`baybe.searchspace.continuous.SubspaceContinuous.from_dataframe`.
@@ -184,38 +184,40 @@
         """
         if {p.name for p in parameters} != set(df.columns.values):
             raise ValueError(
                 "The provided dataframe columns must match exactly with the specified "
                 "parameter names."
             )
 
-        disc_params = [p for p in parameters if isinstance(p, DiscreteParameter)]
-        cont_params = [p for p in parameters if isinstance(p, ContinuousParameter)]
+        disc_params = [p for p in parameters if p.is_discrete]
+        cont_params = [p for p in parameters if p.is_continuous]
 
         return SearchSpace(
             discrete=SubspaceDiscrete.from_dataframe(
-                df[[p.name for p in disc_params]], disc_params
+                df[[p.name for p in disc_params]],
+                disc_params,  # type:ignore[arg-type]
             ),
             continuous=SubspaceContinuous.from_dataframe(
-                df[[p.name for p in cont_params]], cont_params
+                df[[p.name for p in cont_params]],
+                cont_params,  # type:ignore[arg-type]
             ),
         )
 
     @property
-    def parameters(self) -> list[Parameter]:
+    def parameters(self) -> tuple[Parameter, ...]:
         """Return the list of parameters of the search space."""
-        return self.discrete.parameters + self.continuous.parameters
+        return (*self.discrete.parameters, *self.continuous.parameters)
 
     @property
-    def constraints(self) -> list[Constraint]:
+    def constraints(self) -> tuple[Constraint, ...]:
         """Return the constraints of the search space."""
         return (
-            self.discrete.constraints
-            + self.continuous.constraints_lin_eq
-            + self.continuous.constraints_lin_ineq
+            *self.discrete.constraints,
+            *self.continuous.constraints_lin_eq,
+            *self.continuous.constraints_lin_ineq,
         )
 
     @property
     def type(self) -> SearchSpaceType:
         """Return the type of the search space."""
         if self.discrete.is_empty and not self.continuous.is_empty:
             return SearchSpaceType.CONTINUOUS
@@ -252,21 +254,22 @@
         try:
             # TODO [16932]: Redesign metadata handling
             task_param = next(
                 p for p in self.parameters if isinstance(p, TaskParameter)
             )
         except StopIteration:
             return None
-        # TODO[11611]: The current approach has two limitations:
+        # TODO[11611]: The current approach has three limitations:
         #   1.  It matches by column name and thus assumes that the parameter name
         #       is used as the column name.
         #   2.  It relies on the current implementation detail that discrete parameters
         #       appear first in the computational dataframe.
+        #   3.  It assumes there exists exactly one task parameter
         #   --> Fix this when refactoring the data
-        return self.discrete.comp_rep.columns.get_loc(task_param.name)
+        return cast(int, self.discrete.comp_rep.columns.get_loc(task_param.name))
 
     @property
     def n_tasks(self) -> int:
         """The number of tasks encoded in the search space."""
         # TODO [16932]: This approach only works for a single task parameter. For
         #  multiple task parameters, we need to align what the output should even
         #  represent (e.g. number of combinatorial task combinations, number of
@@ -277,14 +280,30 @@
             )
             return len(task_param.values)
 
         # When there are no task parameters, we effectively have a single task
         except StopIteration:
             return 1
 
+    @staticmethod
+    def estimate_product_space_size(parameters: Iterable[Parameter]) -> MemorySize:
+        """Estimate an upper bound for the memory size of a product space.
+
+        Continuous parameters are ignored because creating a continuous subspace has
+        no considerable memory footprint.
+
+        Args:
+            parameters: The parameters spanning the product space.
+
+        Returns:
+            The estimated memory size.
+        """
+        discrete_parameters = [p for p in parameters if p.is_discrete]
+        return SubspaceDiscrete.estimate_product_space_size(discrete_parameters)  # type: ignore[arg-type]
+
     def transform(
         self,
         data: pd.DataFrame,
     ) -> pd.DataFrame:
         """Transform data from experimental to computational representation.
 
         This function can e.g. be used to transform data obtained from measurements.
```

### Comparing `baybe-0.8.2/baybe/searchspace/discrete.py` & `baybe-0.9.0/baybe/searchspace/discrete.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Discrete subspaces."""
 
 from __future__ import annotations
 
-from collections.abc import Collection, Iterable
-from itertools import zip_longest
+from collections.abc import Collection, Iterable, Sequence
+from math import prod
 from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
 from attr import define, field
 from cattrs import IterableValidationError
 
@@ -18,48 +18,76 @@
     NumericalDiscreteParameter,
     TaskParameter,
 )
 from baybe.parameters.base import DiscreteParameter, Parameter
 from baybe.parameters.utils import get_parameters_from_dataframe
 from baybe.searchspace.validation import validate_parameter_names, validate_parameters
 from baybe.serialization import SerialMixin, converter, select_constructor_hook
+from baybe.utils.basic import to_tuple
 from baybe.utils.boolean import eq_dataframe
 from baybe.utils.dataframe import (
     df_drop_single_value_columns,
     fuzzy_row_match,
     pretty_print_df,
 )
+from baybe.utils.memory import bytes_to_human_readable
+from baybe.utils.numerical import DTypeFloatNumpy
 
 _METADATA_COLUMNS = ["was_recommended", "was_measured", "dont_recommend"]
 
 
+@define(kw_only=True)
+class MemorySize:
+    """Estimated memory size of a :class:`SubspaceDiscrete`."""
+
+    exp_rep_memory: float
+    """The memory size of the experimental representation dataframe."""
+
+    exp_rep_unit: str
+    """The unit ``exp_rep_size``."""
+
+    exp_rep_shape: tuple[int, int]
+    """The shape of the experimental representation dataframe."""
+
+    comp_rep_memory: float
+    """The memory size of the computational representation dataframe."""
+
+    comp_rep_unit: str
+    """The unit ``comp_rep_size``."""
+
+    comp_rep_shape: tuple[int, int]
+    """The shape of the computational representation dataframe."""
+
+
 @define
 class SubspaceDiscrete(SerialMixin):
     """Class for managing discrete subspaces.
 
     Builds the subspace from parameter definitions and optional constraints, keeps
     track of search metadata, and provides access to candidate sets and different
     parameter views.
     """
 
-    parameters: list[DiscreteParameter] = field(
-        validator=lambda _1, _2, x: validate_parameter_names(x)
+    parameters: tuple[DiscreteParameter, ...] = field(
+        converter=to_tuple, validator=lambda _, __, x: validate_parameter_names(x)
     )
     """The list of parameters of the subspace."""
 
     exp_rep: pd.DataFrame = field(eq=eq_dataframe)
     """The experimental representation of the subspace."""
 
     metadata: pd.DataFrame = field(eq=eq_dataframe)
     """The metadata."""
 
     empty_encoding: bool = field(default=False)
     """Flag encoding whether an empty encoding is used."""
 
-    constraints: list[DiscreteConstraint] = field(factory=list)
+    constraints: tuple[DiscreteConstraint, ...] = field(
+        converter=to_tuple, factory=tuple
+    )
     """A list of constraints for restricting the space."""
 
     comp_rep: pd.DataFrame = field(eq=eq_dataframe)
     """The computational representation of the space. Technically not required but added
     as an optional initializer argument to allow ingestion from e.g. serialized objects
     and thereby speed up construction. If not provided, the default hook will derive it
     from ``exp_rep``."""
@@ -124,15 +152,15 @@
         if self.is_empty:
             return pd.DataFrame(columns=_METADATA_COLUMNS)
 
         # TODO [16605]: Redesign metadata handling
         # Exclude inactive tasks from search
         df = pd.DataFrame(False, columns=_METADATA_COLUMNS, index=self.exp_rep.index)
         off_task_idxs = ~self._on_task_configurations()
-        df.loc[off_task_idxs.values, "dont_recommend"] = True
+        df.loc[off_task_idxs.values, "dont_recommend"] = True  # type: ignore
         return df
 
     @metadata.validator
     def _validate_metadata(  # noqa: DOC101, DOC103
         self, _: Any, metadata: pd.DataFrame
     ) -> None:
         """Validate the metadata.
@@ -142,15 +170,15 @@
                 for inactive tasks.
         """
         # We first check whether there are actually any parameters that need to be
         # checked.
         if self.is_empty:
             return
         off_task_idxs = ~self._on_task_configurations()
-        if not metadata.loc[off_task_idxs.values, "dont_recommend"].all():
+        if not metadata.loc[off_task_idxs.values, "dont_recommend"].all():  # type: ignore
             raise ValueError(
                 "Inconsistent instructions given: The provided metadata allows "
                 "testing parameter configurations for inactive tasks."
             )
 
     @comp_rep.default
     def _default_comp_rep(self) -> pd.DataFrame:
@@ -170,15 +198,15 @@
         return comp_rep
 
     def __attrs_post_init__(self) -> None:
         # TODO [16605]: Redesign metadata handling
         if self.is_empty:
             return
         off_task_idxs = ~self._on_task_configurations()
-        self.metadata.loc[off_task_idxs.values, "dont_recommend"] = True
+        self.metadata.loc[off_task_idxs.values, "dont_recommend"] = True  # type: ignore
 
     def _on_task_configurations(self) -> pd.Series:
         """Retrieve the parameter configurations for the active tasks."""
         # TODO [16932]: This only works for a single parameter
         try:
             task_param = next(
                 p for p in self.parameters if isinstance(p, TaskParameter)
@@ -195,16 +223,16 @@
             exp_rep=pd.DataFrame(),
             metadata=pd.DataFrame(columns=_METADATA_COLUMNS),
         )
 
     @classmethod
     def from_product(
         cls,
-        parameters: list[DiscreteParameter],
-        constraints: Optional[list[DiscreteConstraint]] = None,
+        parameters: Sequence[DiscreteParameter],
+        constraints: Optional[Sequence[DiscreteConstraint]] = None,
         empty_encoding: bool = False,
     ) -> SubspaceDiscrete:
         """See :class:`baybe.searchspace.core.SearchSpace`."""
         # Set defaults
         constraints = constraints or []
 
         # Create a dataframe representing the experimental search space
@@ -220,15 +248,15 @@
             empty_encoding=empty_encoding,
         )
 
     @classmethod
     def from_dataframe(
         cls,
         df: pd.DataFrame,
-        parameters: Optional[list[DiscreteParameter]] = None,
+        parameters: Optional[Sequence[DiscreteParameter]] = None,
         empty_encoding: bool = False,
     ) -> SubspaceDiscrete:
         """Create a discrete subspace with a specified set of configurations.
 
         Args:
             df: The experimental representation of the search space to be created.
             parameters: Optional parameter objects corresponding to the columns in the
@@ -264,17 +292,17 @@
 
         return cls(parameters=parameters, exp_rep=df, empty_encoding=empty_encoding)
 
     @classmethod
     def from_simplex(
         cls,
         max_sum: float,
-        simplex_parameters: list[NumericalDiscreteParameter],
-        product_parameters: Optional[list[DiscreteParameter]] = None,
-        constraints: Optional[list[DiscreteConstraint]] = None,
+        simplex_parameters: Sequence[NumericalDiscreteParameter],
+        product_parameters: Optional[Sequence[DiscreteParameter]] = None,
+        constraints: Optional[Sequence[DiscreteConstraint]] = None,
         min_nonzero: int = 0,
         max_nonzero: Optional[int] = None,
         boundary_only: bool = False,
         tolerance: float = 1e-6,
     ) -> SubspaceDiscrete:
         """Efficiently create discrete simplex subspaces.
 
@@ -321,25 +349,25 @@
             product_parameters = []
         if constraints is None:
             constraints = []
         if max_nonzero is None:
             max_nonzero = len(simplex_parameters)
 
         # Validate constraints
-        validate_constraints(constraints, simplex_parameters + product_parameters)
+        validate_constraints(constraints, [*simplex_parameters, *product_parameters])
 
         # Validate parameter types
         if not (
             all(isinstance(p, NumericalDiscreteParameter) for p in simplex_parameters)
         ):
             raise ValueError(
                 f"All parameters passed via 'simplex_parameters' "
                 f"must be of type '{NumericalDiscreteParameter.__name__}'."
             )
-        if not all(isinstance(p, DiscreteParameter) for p in product_parameters):
+        if not all(p.is_discrete for p in product_parameters):
             raise ValueError(
                 f"All parameters passed via 'product_parameters' "
                 f"must be of subclasses of '{DiscreteParameter.__name__}'."
             )
 
         # Construct the product part of the space
         product_space = parameter_cartesian_prod_to_df(product_parameters)
@@ -421,20 +449,19 @@
         #   desired number of nonzero after all joins.
         for i, (
             param,
             min_sum_to_go,
             min_nonzero_to_go,
             max_nonzero_to_go,
         ) in enumerate(
-            zip_longest(
+            zip(
                 simplex_parameters,
-                min_sum_upcoming,
-                min_nonzero_upcoming,
-                max_nonzero_upcoming,
-                fillvalue=0,
+                np.append(min_sum_upcoming, 0),
+                np.append(min_nonzero_upcoming, 0),
+                np.append(max_nonzero_upcoming, 0),
             )
         ):
             if i == 0:
                 exp_rep = pd.DataFrame({param.name: param.values})
             else:
                 exp_rep = pd.merge(
                     exp_rep, pd.DataFrame({param.name: param.values}), how="cross"
@@ -459,15 +486,15 @@
         if product_parameters:
             exp_rep = pd.merge(exp_rep, product_space, how="cross")
 
         # Remove entries that violate parameter constraints:
         _apply_constraint_filter(exp_rep, constraints)
 
         return cls(
-            parameters=simplex_parameters + product_parameters,
+            parameters=[*simplex_parameters, *product_parameters],
             exp_rep=exp_rep,
             constraints=constraints,
         )
 
     @property
     def is_empty(self) -> bool:
         """Return whether this subspace is empty."""
@@ -488,14 +515,60 @@
                 for p in self.parameters
                 for col in p.comp_df
                 if col in self.comp_rep.columns
             ]
         )
         return bounds
 
+    @staticmethod
+    def estimate_product_space_size(
+        parameters: Sequence[DiscreteParameter]
+    ) -> MemorySize:
+        """Estimate an upper bound for the memory size of a product space.
+
+        Args:
+            parameters: The parameters spanning the product space.
+
+        Returns:
+            The estimated memory size.
+        """
+        # Compute the dataframe shapes
+        n_cols_exp = len(parameters)
+        n_cols_comp = sum(p.comp_df.shape[1] for p in parameters)
+        n_rows = prod(p.comp_df.shape[0] for p in parameters)
+
+        # Comp rep space is estimated as the size of float times the number of matrix
+        # elements in the comp rep. The latter is the total number of parameter
+        # configurations (= number of rows) times the total number of columns.
+        comp_rep_size, comp_rep_unit = bytes_to_human_readable(
+            np.array([0.0], dtype=DTypeFloatNumpy).itemsize * n_rows * n_cols_comp
+        )
+
+        # Exp rep space is estimated as the size of the per-parameter exp rep dataframe
+        # times the number of times it will appear in the entire search space. The
+        # latter is the total number of parameter configurations (= number of rows)
+        # divided by the number of values for the respective parameter. Contributions of
+        # all parameters are summed up.
+        exp_rep_bytes = sum(
+            pd.DataFrame(p.values).memory_usage(index=False, deep=True).sum()
+            * n_rows
+            / p.comp_df.shape[0]
+            for p in parameters
+        )
+        exp_rep_size, exp_rep_unit = bytes_to_human_readable(exp_rep_bytes)
+
+        return MemorySize(
+            exp_rep_memory=np.round(exp_rep_size, 2),
+            exp_rep_unit=exp_rep_unit,
+            exp_rep_shape=(n_rows, n_cols_exp),
+            comp_rep_memory=np.round(comp_rep_size, 2),
+            comp_rep_unit=comp_rep_unit,
+            comp_rep_shape=(n_rows, n_cols_comp),
+        )
+
     def mark_as_measured(
         self,
         measurements: pd.DataFrame,
         numerical_measurements_must_be_within_tolerance: bool,
     ) -> None:
         """Mark the given elements of the space as measured.
 
@@ -577,15 +650,17 @@
             comp_rep = comp_rep[self.comp_rep.columns]
         except AttributeError:
             pass
 
         return comp_rep
 
 
-def _apply_constraint_filter(df: pd.DataFrame, constraints: list[DiscreteConstraint]):
+def _apply_constraint_filter(
+    df: pd.DataFrame, constraints: Collection[DiscreteConstraint]
+):
     """Remove discrete search space entries inplace based on constraints.
 
     Args:
         df: The data in experimental representation to be modified inplace.
         constraints: List of discrete constraints.
 
     """
@@ -611,20 +686,20 @@
 
     Args:
         parameters: List of parameter objects.
 
     Returns:
         A dataframe containing all possible discrete parameter value combinations.
     """
-    discrete_parameters = [p for p in parameters if isinstance(p, DiscreteParameter)]
+    discrete_parameters = [p for p in parameters if p.is_discrete]
     if not discrete_parameters:
         return pd.DataFrame()
 
     index = pd.MultiIndex.from_product(
-        [p.values for p in discrete_parameters],
+        [p.values for p in discrete_parameters],  # type:ignore[attr-defined]
         names=[p.name for p in discrete_parameters],
     )
     ret = pd.DataFrame(index=index).reset_index()
 
     return ret
```

### Comparing `baybe-0.8.2/baybe/searchspace/validation.py` & `baybe-0.9.0/baybe/searchspace/validation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Validation functionality for search spaces."""
 
+from collections.abc import Collection
 
 from baybe.exceptions import EmptySearchSpaceError
 from baybe.parameters import TaskParameter
 from baybe.parameters.base import Parameter
 
 
 def validate_parameter_names(  # noqa: DOC101, DOC103
-    parameters: list[Parameter],
+    parameters: Collection[Parameter],
 ) -> None:
     """Validate the parameter names.
 
     Raises:
         ValueError: If the given list contains parameters with the same name.
     """
     param_names = [p.name for p in parameters]
     if len(set(param_names)) != len(param_names):
         raise ValueError("All parameters must have unique names.")
 
 
-def validate_parameters(parameters: list[Parameter]) -> None:  # noqa: DOC101, DOC103
+def validate_parameters(parameters: Collection[Parameter]) -> None:  # noqa: DOC101, DOC103
     """Validate the parameters.
 
     Raises:
         EmptySearchSpaceError: If the parameter list is empty.
         NotImplementedError: If more than one
             :class:`baybe.parameters.categorical.TaskParameter` is requested.
     """
```

### Comparing `baybe-0.8.2/baybe/serialization/__init__.py` & `baybe-0.9.0/baybe/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/serialization/core.py` & `baybe-0.9.0/baybe/serialization/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from typing import Any, Callable, Optional, TypeVar, Union, get_type_hints
 
 import attrs
 import cattrs
 import pandas as pd
 from cattrs.gen import make_dict_structure_fn, make_dict_unstructure_fn
 
+from baybe.utils.basic import find_subclass, refers_to
+from baybe.utils.boolean import is_abstract
+
 _T = TypeVar("_T")
 
 # TODO: This urgently needs the `forbid_extra_keys=True` flag, which requires us to
 #   switch to the cattrs built-in subclass recommender.
 converter = cattrs.Converter()
 """The default converter for (de-)serializing BayBE-related objects."""
 
@@ -35,38 +38,50 @@
         **attrs_dict,
     }
 
 
 def get_base_structure_hook(
     base: type[_T],
     overrides: Optional[dict] = None,
-) -> Callable[[dict, type[_T]], _T]:
-    """Return a hook for structuring a dictionary into an appropriate subclass.
+) -> Callable[[Union[dict, str], type[_T]], _T]:
+    """Return a hook for structuring a specified subclass.
 
     Provides the inverse operation to ``unstructure_base``.
 
     Args:
-        base: The corresponding class
+        base: The corresponding class.
         overrides: An optional dictionary of cattrs-overrides for certain attributes.
 
     Returns:
         The hook.
     """
     # TODO: use include_subclasses (https://github.com/python-attrs/cattrs/issues/434)
-    from baybe.utils.basic import get_subclasses
 
-    def structure_base(val: dict, _: type[_T]) -> _T:
-        _type = val.pop("type")
-        cls = next((cl for cl in get_subclasses(base) if cl.__name__ == _type), None)
-        if cls is None:
-            raise ValueError(f"Unknown subclass '{_type}'.")
-        fun = make_dict_structure_fn(
-            cls, converter, **(overrides or {}), _cattrs_forbid_extra_keys=True
+    def structure_base(val: Union[dict, str], cls: type[_T]) -> _T:
+        # If the given class can be instantiated, only ensure there is no conflict with
+        # a potentially specified type field
+        if not is_abstract(cls):
+            if (type_ := val.pop("type", None)) and not refers_to(cls, type_):
+                raise ValueError(
+                    f"The class '{cls.__name__}' specified for deserialization "
+                    f"does not match with the given type information '{type_}'."
+                )
+            concrete_cls = cls
+
+        # Otherwise, extract the type information from the given input and find
+        # the corresponding class in the hierarchy
+        else:
+            type_ = val if isinstance(val, str) else val.pop("type")
+            concrete_cls = find_subclass(base, type_)
+
+        # Create the structuring function for the class and call it
+        fn = make_dict_structure_fn(
+            concrete_cls, converter, **(overrides or {}), _cattrs_forbid_extra_keys=True
         )
-        return fun(val, cls)
+        return fn({} if isinstance(val, str) else val, concrete_cls)
 
     return structure_base
 
 
 def _structure_dataframe_hook(obj: Union[str, dict], _) -> pd.DataFrame:
     """Deserialize a DataFrame."""
     if isinstance(obj, str):
@@ -92,26 +107,26 @@
     return base64.b64encode(pickled_df).decode("utf-8")
 
 
 def block_serialization_hook(obj: Any) -> None:  # noqa: DOC101, DOC103
     """Prevent serialization of the passed object.
 
     Raises:
-         NotImplementedError: Always.
+        NotImplementedError: Always.
     """
     raise NotImplementedError(
         f"Serializing objects of type '{obj.__class__.__name__}' is not supported."
     )
 
 
 def block_deserialization_hook(_: Any, cls: type) -> None:  # noqa: DOC101, DOC103
     """Prevent deserialization into a specific type.
 
     Raises:
-         NotImplementedError: Always.
+        NotImplementedError: Always.
     """
     raise NotImplementedError(
         f"Deserialization into '{cls.__name__}' is not supported."
     )
 
 
 def select_constructor_hook(specs: dict, cls: type[_T]) -> _T:
```

### Comparing `baybe-0.8.2/baybe/serialization/mixin.py` & `baybe-0.9.0/baybe/serialization/mixin.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/strategies/deprecation.py` & `baybe-0.9.0/baybe/strategies/deprecation.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,14 @@
 from baybe.recommenders.meta import (
     SequentialMetaRecommender,
     StreamingSequentialMetaRecommender,
     TwoPhaseMetaRecommender,
 )
 
 
-def Strategy(*args, **kwargs) -> TwoPhaseMetaRecommender:
-    """A ``Strategy`` alias for backward compatibility."""  # noqa: D401 (imperative mood)
-    warnings.warn(
-        f"Using 'Strategy' directly is deprecated and will be removed in a future "
-        f"version. Please use 'recommenders.{TwoPhaseMetaRecommender.__name__}' class "
-        f"instead.",
-        DeprecationWarning,
-    )
-
-    return TwoPhaseMetaRecommender(*args, **kwargs)
-
-
 def TwoPhaseStrategy(*args, **kwargs) -> TwoPhaseMetaRecommender:
     """A ``TwoPhaseStrategy`` alias for backward compatibility."""  # noqa: D401 (imperative mood)
     warnings.warn(
         f"'TwoPhaseStrategy' is deprecated and will be removed in a future "
         f"version. Please use 'recommenders.{TwoPhaseMetaRecommender.__name__}' class "
         f"instead.",
         DeprecationWarning,
```

### Comparing `baybe-0.8.2/baybe/surrogates/__init__.py` & `baybe-0.9.0/baybe/surrogates/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """BayBE surrogates."""
 
-from baybe.surrogates.base import get_available_surrogates
 from baybe.surrogates.custom import _ONNX_INSTALLED, register_custom_architecture
-from baybe.surrogates.gaussian_process import GaussianProcessSurrogate
+from baybe.surrogates.gaussian_process.core import GaussianProcessSurrogate
 from baybe.surrogates.linear import BayesianLinearSurrogate
 from baybe.surrogates.naive import MeanPredictionSurrogate
 from baybe.surrogates.ngboost import NGBoostSurrogate
 from baybe.surrogates.random_forest import RandomForestSurrogate
 
 __all__ = [
-    "get_available_surrogates",
     "register_custom_architecture",
     "BayesianLinearSurrogate",
     "GaussianProcessSurrogate",
     "MeanPredictionSurrogate",
     "NGBoostSurrogate",
     "RandomForestSurrogate",
 ]
```

### Comparing `baybe-0.8.2/baybe/surrogates/base.py` & `baybe-0.9.0/baybe/surrogates/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 """Base functionality for all BayBE surrogates."""
 
-import gc
-import sys
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import Any, ClassVar
+from typing import TYPE_CHECKING, ClassVar
 
-import torch
-from attr import define, field
-from torch import Tensor
+from attrs import define
+from cattrs import override
+from cattrs.dispatch import (
+    StructuredValue,
+    StructureHook,
+    TargetType,
+    UnstructuredValue,
+    UnstructureHook,
+)
 
 from baybe.searchspace import SearchSpace
-from baybe.serialization import SerialMixin, converter, unstructure_base
+from baybe.serialization.core import (
+    converter,
+    get_base_structure_hook,
+    unstructure_base,
+)
+from baybe.serialization.mixin import SerialMixin
 from baybe.surrogates.utils import _prepare_inputs, _prepare_targets
-from baybe.utils.basic import get_subclasses
+
+if TYPE_CHECKING:
+    from torch import Tensor
 
 # Define constants
 _MIN_VARIANCE = 1e-6
-_WRAPPER_MODELS = (
-    "SplitModel",
-    "ScaledModel",
-    "CustomArchitectureSurrogate",
-    "CustomONNXSurrogate",
-)
 
 _ONNX_ENCODING = "latin-1"
 """Constant signifying the encoding for onnx byte strings in pretrained models.
 
 NOTE: This encoding is selected by choice for ONNX byte strings.
 This is not a requirement from ONNX but simply for the JSON format.
 The byte string from ONNX `.SerializeToString()` method has unknown encoding,
@@ -44,35 +51,29 @@
     joint_posterior: ClassVar[bool]
     """Class variable encoding whether or not a joint posterior is calculated."""
 
     supports_transfer_learning: ClassVar[bool]
     """Class variable encoding whether or not the surrogate supports transfer
     learning."""
 
-    # Object variables
-    # TODO: In a next refactoring, the user friendliness could be improved by directly
-    #   exposing the individual model parameters via the constructor, instead of
-    #   expecting them in the form of an unstructured dictionary. This would also
-    #   remove the need for the current `_get_model_params_validator` logic.
-    model_params: dict[str, Any] = field(factory=dict)
-    """Optional model parameters."""
-
     def posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
         """Evaluate the surrogate model at the given candidate points.
 
         Args:
             candidates: The candidate points, represented as a tensor of shape
                 ``(*t, q, d)``, where ``t`` denotes the "t-batch" shape, ``q``
                 denotes the "q-batch" shape, and ``d`` is the input dimension. For
                 more details about batch shapes, see: https://botorch.org/docs/batching
 
         Returns:
             The posterior means and posterior covariance matrices of the t-batched
             candidate points.
         """
+        import torch
+
         # Prepare the input
         candidates = _prepare_inputs(candidates)
 
         # Evaluate the posterior distribution
         mean, covar = self._posterior(candidates)
 
         # Apply covariance transformation for marginal posterior models
@@ -139,121 +140,89 @@
                 "Continuous search spaces are currently only supported by GPs."
             )
 
         # Validate and prepare the training data
         train_x = _prepare_inputs(train_x)
         train_y = _prepare_targets(train_y)
 
-        return self._fit(searchspace, train_x, train_y)
+        self._fit(searchspace, train_x, train_y)
 
     @abstractmethod
     def _fit(self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor) -> None:
         """Perform the actual fitting logic.
 
         In contrast to its public counterpart :func:`baybe.surrogates.Surrogate.fit`,
         no data validation/transformation is carried out but only the raw fitting
         operation is conducted.
 
         See :func:`baybe.surrogates.Surrogate.fit` for details on the parameters.
         """
 
 
-def _decode_onnx_str(raw_unstructure_hook):
-    """Decode ONNX string for serialization purposes."""
+def _make_hook_decode_onnx_str(
+    raw_unstructure_hook: UnstructureHook
+) -> UnstructureHook:
+    """Wrap an unstructuring hook to let it also decode the contained ONNX string."""
+
+    def wrapper(obj: StructuredValue) -> UnstructuredValue:
+        dct = raw_unstructure_hook(obj)
+        if "onnx_str" in dct:
+            dct["onnx_str"] = dct["onnx_str"].decode(_ONNX_ENCODING)
 
-    def wrapper(obj):
-        dict_ = raw_unstructure_hook(obj)
-        if "onnx_str" in dict_:
-            dict_["onnx_str"] = dict_["onnx_str"].decode(_ONNX_ENCODING)
+        return dct
+
+    return wrapper
 
-        return dict_
+
+def _make_hook_encode_onnx_str(raw_structure_hook: StructureHook) -> StructureHook:
+    """Wrap a structuring hook to let it also encode the contained ONNX string."""
+
+    def wrapper(dct: UnstructuredValue, _: TargetType) -> StructuredValue:
+        if (onnx_str := dct.get("onnx_str")) and isinstance(onnx_str, str):
+            dct["onnx_str"] = onnx_str.encode(_ONNX_ENCODING)
+        obj = raw_structure_hook(dct, _)
+
+        return obj
 
     return wrapper
 
 
-def _block_serialize_custom_architecture(raw_unstructure_hook):
+def _block_serialize_custom_architecture(
+    raw_unstructure_hook: UnstructureHook
+) -> UnstructureHook:
     """Raise error if attempt to serialize a custom architecture surrogate."""
-    # TODO: Should be replaced with `serialization.block_serialization_hook`.
-    #   However, the class definition of `CustomArchitectureSurrogate` is needs
-    #   to be fixed first, which is broken due to the handling of `model_params`.
-    #   To reproduce the problem, run for example `custom_architecture_torch` and
-    #   try to print the created surrogate model object.
+    # TODO: Ideally, this hook should be removed and unstructuring the Surrogate
+    #   base class should automatically invoke the blocking hook that is already
+    #   registered for the "CustomArchitectureSurrogate" subclass. However, it's
+    #   not clear how the base unstructuring hook needs to be modified to accomplish
+    #   this, and furthermore the problem will most likely become obsolete in the future
+    #   because the role of the subclass will probably be replaced with a surrogate
+    #   protocol.
 
-    def wrapper(obj):
+    def wrapper(obj: StructuredValue) -> UnstructuredValue:
         if obj.__class__.__name__ == "CustomArchitectureSurrogate":
             raise NotImplementedError(
-                "Custom Architecture Surrogate Serialization is not supported"
+                "Serializing objects of type 'CustomArchitectureSurrogate' "
+                "is not supported."
             )
 
         return raw_unstructure_hook(obj)
 
     return wrapper
 
 
-# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>> Temporary workaround >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
-def _structure_surrogate(val, _):
-    """Structure a surrogate model."""
-    # TODO [15436]
-    # https://***REMOVED***/_boards/board/t/SDK%20Devs/Features/?workitem=15436
-
-    # NOTE:
-    # Due to above issue,
-    # it is difficult to find the wrapped class in the subclass structure.
-    # The renaming only happens in the init method of wrapper classes
-    # (classes that haven't been initialized won't have the overwritten name)
-    # Since any method revolving `cls()` will not work as expected,
-    # we rely temporarily on `getattr` to allow the wrappers to be called on demand.
-
-    _type = val["type"]
-
-    cls = getattr(sys.modules[__package__], _type, None)
-    # cls = getattr(baybe.surrogates, ...) if used in another module
-
-    if cls is None:
-        raise ValueError(f"Unknown subclass {_type}.")
-
-    # NOTE:
-    # This is a workaround for onnx str type being `str` or `bytes`
-    onnx_str = val.get("onnx_str", None)
-    if onnx_str and isinstance(onnx_str, str):
-        val["onnx_str"] = onnx_str.encode(_ONNX_ENCODING)
-
-    return converter.structure_attrs_fromdict(val, cls)
-
-
-def get_available_surrogates() -> list[type[Surrogate]]:
-    """List all available surrogate models.
-
-    Returns:
-        A list of available surrogate classes.
-    """
-    # List available names
-    available_names = {
-        cl.__name__
-        for cl in get_subclasses(Surrogate)
-        if cl.__name__ not in _WRAPPER_MODELS
-    }
-
-    # Convert them to classes
-    available_classes = [
-        getattr(sys.modules[__package__], mdl_name, None)
-        for mdl_name in available_names
-    ]
-
-    # TODO: The initialization of the classes is currently necessary for the renaming
-    #  to take place (see [15436] and NOTE in `structure_surrogate`).
-    [cl() for cl in available_classes if cl is not None]
-
-    return [cl for cl in available_classes if cl is not None]
-
-
 # Register (un-)structure hooks
-# TODO: Needs to be refactored
+# IMPROVE: Ideally, the ONNX-specific hooks should simply be registered with the ONNX
+#   class, which would avoid the nested wrapping below. However, this requires
+#   adjusting the base class (un-)structure hooks such that they consistently apply
+#   existing hooks of the concrete subclasses.
 converter.register_unstructure_hook(
     Surrogate,
-    _decode_onnx_str(_block_serialize_custom_architecture(unstructure_base)),
+    _make_hook_decode_onnx_str(
+        _block_serialize_custom_architecture(
+            lambda x: unstructure_base(x, overrides={"_model": override(omit=True)})
+        )
+    ),
+)
+converter.register_structure_hook(
+    Surrogate, _make_hook_encode_onnx_str(get_base_structure_hook(Surrogate))
 )
-converter.register_structure_hook(Surrogate, _structure_surrogate)
-
-# Related to [15436]
-gc.collect()
-# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<< Temporary workaround <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
```

### Comparing `baybe-0.8.2/baybe/surrogates/custom.py` & `baybe-0.9.0/baybe/surrogates/custom.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,43 +3,45 @@
 Note that ONNX surrogate models cannot be retrained. However, having the surrogates
 raise a ``NotImplementedError`` would currently break the code since
 :class:`baybe.recommenders.pure.bayesian.base.BayesianRecommender` assumes that
 surrogates can be trained and attempts to do so for each new DOE iteration.
 
 It is planned to solve this issue in the future.
 """
+from __future__ import annotations
 
-from typing import Callable, ClassVar
+from typing import TYPE_CHECKING, Callable, ClassVar
 
-import torch
-from attrs import define, field, validators
-from torch import Tensor
+from attrs import define, field, resolve_types, validators
 
-from baybe.exceptions import ModelParamsNotSupportedError
 from baybe.parameters import (
     CategoricalEncoding,
     CategoricalParameter,
     CustomDiscreteParameter,
     NumericalContinuousParameter,
     NumericalDiscreteParameter,
     TaskParameter,
 )
 from baybe.searchspace import SearchSpace
+from baybe.serialization.core import block_serialization_hook, converter
 from baybe.surrogates.base import Surrogate
 from baybe.surrogates.utils import batchify, catch_constant_targets
 from baybe.surrogates.validation import validate_custom_architecture_cls
-from baybe.utils.numerical import DTypeFloatONNX, DTypeFloatTorch
+from baybe.utils.numerical import DTypeFloatONNX
 
 try:
     import onnxruntime as ort
 
     _ONNX_INSTALLED = True
 except ImportError:
     _ONNX_INSTALLED = False
 
+if TYPE_CHECKING:
+    from torch import Tensor
+
 
 def register_custom_architecture(
     joint_posterior_attr: bool = False,
     constant_target_catching: bool = True,
     batchify_posterior: bool = True,
 ) -> Callable:
     """Wrap a given custom model architecture class into a ```Surrogate```.
@@ -63,23 +65,23 @@
         class CustomArchitectureSurrogate(Surrogate):
             """Wraps around a custom architecture class."""
 
             joint_posterior: ClassVar[bool] = joint_posterior_attr
             supports_transfer_learning: ClassVar[bool] = False
 
             def __init__(self, *args, **kwargs):
-                self.model = model_cls(*args, **kwargs)
+                self._model = model_cls(*args, **kwargs)
 
             def _fit(
                 self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor
             ) -> None:
-                return self.model._fit(searchspace, train_x, train_y)
+                return self._model._fit(searchspace, train_x, train_y)
 
             def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
-                return self.model._posterior(candidates)
+                return self._model._posterior(candidates)
 
             def __get_attribute__(self, attr):
                 """Access the attributes of the class instance if available.
 
                 If the attributes are not available,
                 it uses the attributes of the internal model instance.
                 """
@@ -88,27 +90,32 @@
                     val = super().__getattribute__(attr)
                 except AttributeError:
                     pass
                 else:
                     return val
 
                 # If the attribute is not overwritten, use that of the internal model
-                return self.model.__getattribute__(attr)
+                return self._model.__getattribute__(attr)
 
         # Catch constant targets if needed
         cls = (
             catch_constant_targets(CustomArchitectureSurrogate)
             if constant_target_catching
             else CustomArchitectureSurrogate
         )
 
         # batchify posterior if needed
         if batchify_posterior:
             cls._posterior = batchify(cls._posterior)
 
+        # Block serialization of custom architectures
+        converter.register_unstructure_hook(
+            CustomArchitectureSurrogate, block_serialization_hook
+        )
+
         return cls
 
     return construct_custom_architecture
 
 
 if _ONNX_INSTALLED:
 
@@ -130,32 +137,30 @@
         onnx_input_name: str = field(validator=validators.instance_of(str))
         """The input name used for constructing the ONNX str."""
 
         onnx_str: bytes = field(validator=validators.instance_of(bytes))
         """The ONNX byte str representing the model."""
 
         _model: ort.InferenceSession = field(init=False, eq=False)
-        """The internal model."""
+        """The actual model."""
 
         @_model.default
         def default_model(self) -> ort.InferenceSession:
             """Instantiate the ONNX inference session."""
             try:
                 return ort.InferenceSession(self.onnx_str)
             except Exception as exc:
                 raise ValueError("Invalid ONNX string") from exc
 
-        def __attrs_post_init__(self) -> None:
-            # TODO: This is a temporary workaround to avoid silent errors when users
-            #   provide model parameters to this class.
-            if self.model_params or not isinstance(self.model_params, dict):
-                raise ModelParamsNotSupportedError()
-
         @batchify
         def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
+            import torch
+
+            from baybe.utils.torch import DTypeFloatTorch
+
             model_inputs = {
                 self.onnx_input_name: candidates.numpy().astype(DTypeFloatONNX)
             }
             results = self._model.run(None, model_inputs)
 
             # IMPROVE: At the moment, we assume that the second model output contains
             #   standard deviations. Currently, most available ONNX converters care
@@ -206,7 +211,12 @@
                 raise TypeError(
                     f"To prevent potential hard-to-detect bugs that stem from wrong "
                     f"wiring of model inputs, {cls.__name__} "
                     f"is currently restricted for use with parameters that have "
                     f"a one-dimensional computational representation or "
                     f"{CustomDiscreteParameter.__name__}."
                 )
+
+    # FIXME: This manual resolve should not be necessary if the classes are declared
+    #   properly. Potentially related to the conditional class definition, which should
+    #   vanish as well.
+    resolve_types(CustomONNXSurrogate)
```

### Comparing `baybe-0.8.2/baybe/surrogates/linear.py` & `baybe-0.9.0/baybe/surrogates/linear.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 
 Currently, the documentation for this surrogate is not available. This is due to a bug
 in our documentation tool, see https://github.com/sphinx-doc/sphinx/issues/11750.
 
 Since we plan to refactor the surrogates, this part of the documentation will be
 available in the future. Thus, please have a look in the source code directly.
 """
+from __future__ import annotations
 
-from typing import Any, ClassVar, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Optional
 
-import torch
 from attr import define, field
 from sklearn.linear_model import ARDRegression
-from torch import Tensor
 
 from baybe.searchspace import SearchSpace
 from baybe.surrogates.base import Surrogate
-from baybe.surrogates.utils import batchify, catch_constant_targets, scale_model
+from baybe.surrogates.utils import autoscale, batchify, catch_constant_targets
 from baybe.surrogates.validation import get_model_params_validator
 
+if TYPE_CHECKING:
+    from torch import Tensor
+
 
 @catch_constant_targets
-@scale_model
-@define
+@autoscale
+@define(slots=False)
 class BayesianLinearSurrogate(Surrogate):
     """A Bayesian linear regression surrogate model."""
 
     # Class variables
     joint_posterior: ClassVar[bool] = False
     # See base class.
 
@@ -35,22 +37,25 @@
 
     # Object variables
     model_params: dict[str, Any] = field(
         factory=dict,
         converter=dict,
         validator=get_model_params_validator(ARDRegression.__init__),
     )
-    # See base class.
+    """Optional model parameter that will be passed to the surrogate constructor."""
 
-    _model: Optional[ARDRegression] = field(init=False, default=None)
+    _model: Optional[ARDRegression] = field(init=False, default=None, eq=False)
     """The actual model."""
 
     @batchify
     def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
         # See base class.
+
+        import torch
+
         # Get predictions
         dists = self._model.predict(candidates.numpy(), return_std=True)
 
         # Split into posterior mean and variance
         mean = torch.from_numpy(dists[0])
         var = torch.from_numpy(dists[1]).pow(2)
```

### Comparing `baybe-0.8.2/baybe/surrogates/naive.py` & `baybe-0.9.0/baybe/surrogates/naive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Naive surrogates."""
 
-from typing import ClassVar, Optional
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, ClassVar, Optional
 
-import torch
 from attr import define, field
-from torch import Tensor
 
 from baybe.searchspace import SearchSpace
 from baybe.surrogates.base import Surrogate
 from baybe.surrogates.utils import batchify
 
+if TYPE_CHECKING:
+    from torch import Tensor
+
 
 @define
 class MeanPredictionSurrogate(Surrogate):
     """A trivial surrogate model.
 
     It provides the average value of the training targets
     as posterior mean and a (data-independent) constant posterior variance.
@@ -23,21 +26,24 @@
     joint_posterior: ClassVar[bool] = False
     # See base class.
 
     supports_transfer_learning: ClassVar[bool] = False
     # See base class.
 
     # Object variables
-    target_value: Optional[float] = field(init=False, default=None)
-    """The value of the posterior mean."""
+    _model: Optional[float] = field(init=False, default=None, eq=False)
+    """The estimated posterior mean value of the training targets."""
 
     @batchify
     def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
         # See base class.
+
+        import torch
+
         # TODO: use target value bounds for covariance scaling when explicitly provided
-        mean = self.target_value * torch.ones([len(candidates)])
+        mean = self._model * torch.ones([len(candidates)])
         var = torch.ones(len(candidates))
         return mean, var
 
     def _fit(self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor) -> None:
         # See base class.
-        self.target_value = train_y.mean().item()
+        self._model = train_y.mean().item()
```

### Comparing `baybe-0.8.2/baybe/surrogates/ngboost.py` & `baybe-0.9.0/baybe/surrogates/ngboost.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 
 Currently, the documentation for this surrogate is not available. This is due to a bug
 in our documentation tool, see https://github.com/sphinx-doc/sphinx/issues/11750.
 
 Since we plan to refactor the surrogates, this part of the documentation will be
 available in the future. Thus, please have a look in the source code directly.
 """
+from __future__ import annotations
 
-from typing import Any, ClassVar, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Optional
 
-import torch
 from attr import define, field
 from ngboost import NGBRegressor
-from torch import Tensor
 
 from baybe.searchspace import SearchSpace
 from baybe.surrogates.base import Surrogate
-from baybe.surrogates.utils import batchify, catch_constant_targets, scale_model
+from baybe.surrogates.utils import autoscale, batchify, catch_constant_targets
 from baybe.surrogates.validation import get_model_params_validator
 
+if TYPE_CHECKING:
+    from torch import Tensor
+
 
 @catch_constant_targets
-@scale_model
-@define
+@autoscale
+@define(slots=False)
 class NGBoostSurrogate(Surrogate):
     """A natural-gradient-boosting surrogate model."""
 
     # Class variables
     joint_posterior: ClassVar[bool] = False
     # See base class.
 
@@ -38,25 +40,28 @@
 
     # Object variables
     model_params: dict[str, Any] = field(
         factory=dict,
         converter=dict,
         validator=get_model_params_validator(NGBRegressor.__init__),
     )
-    # See base class.
+    """Optional model parameter that will be passed to the surrogate constructor."""
 
-    _model: Optional[NGBRegressor] = field(init=False, default=None)
+    _model: Optional[NGBRegressor] = field(init=False, default=None, eq=False)
     """The actual model."""
 
     def __attrs_post_init__(self):
         self.model_params = {**self._default_model_params, **self.model_params}
 
     @batchify
     def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
         # See base class.
+
+        import torch
+
         # Get predictions
         dists = self._model.pred_dist(candidates)
 
         # Split into posterior mean and variance
         mean = torch.from_numpy(dists.mean())
         var = torch.from_numpy(dists.var)
```

### Comparing `baybe-0.8.2/baybe/surrogates/random_forest.py` & `baybe-0.9.0/baybe/surrogates/random_forest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 
 Currently, the documentation for this surrogate is not available. This is due to a bug
 in our documentation tool, see https://github.com/sphinx-doc/sphinx/issues/11750.
 
 Since we plan to refactor the surrogates, this part of the documentation will be
 available in the future. Thus, please have a look in the source code directly.
 """
+from __future__ import annotations
 
-from typing import Any, ClassVar, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, Optional
 
 import numpy as np
-import torch
 from attr import define, field
 from sklearn.ensemble import RandomForestRegressor
-from torch import Tensor
 
 from baybe.searchspace import SearchSpace
 from baybe.surrogates.base import Surrogate
-from baybe.surrogates.utils import batchify, catch_constant_targets, scale_model
+from baybe.surrogates.utils import autoscale, batchify, catch_constant_targets
 from baybe.surrogates.validation import get_model_params_validator
 
+if TYPE_CHECKING:
+    from torch import Tensor
+
 
 @catch_constant_targets
-@scale_model
-@define
+@autoscale
+@define(slots=False)
 class RandomForestSurrogate(Surrogate):
     """A random forest surrogate model."""
 
     # Class variables
     joint_posterior: ClassVar[bool] = False
     # See base class.
 
@@ -36,23 +38,25 @@
 
     # Object variables
     model_params: dict[str, Any] = field(
         factory=dict,
         converter=dict,
         validator=get_model_params_validator(RandomForestRegressor.__init__),
     )
-    # See base class.
+    """Optional model parameter that will be passed to the surrogate constructor."""
 
-    _model: Optional[RandomForestRegressor] = field(init=False, default=None)
+    _model: Optional[RandomForestRegressor] = field(init=False, default=None, eq=False)
     """The actual model."""
 
     @batchify
     def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
         # See base class.
 
+        import torch
+
         # Evaluate all trees
         # NOTE: explicit conversion to ndarray is needed due to a pytorch issue:
         # https://github.com/pytorch/pytorch/pull/51731
         # https://github.com/pytorch/pytorch/issues/13918
         predictions = torch.from_numpy(
             np.asarray(
                 [
```

### Comparing `baybe-0.8.2/baybe/surrogates/utils.py` & `baybe-0.9.0/baybe/surrogates/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,200 @@
 """Utilities for working with surrogates."""
 
 from __future__ import annotations
 
 from functools import wraps
-from typing import TYPE_CHECKING, Callable, ClassVar
-
-import torch
-from torch import Tensor
+from typing import TYPE_CHECKING, Callable
 
 from baybe.scaler import DefaultScaler
 from baybe.searchspace import SearchSpace
 
 if TYPE_CHECKING:
-    from baybe.surrogates.base import Surrogate
-
-# Use float64 (which is recommended at least for BoTorch models)
-_DTYPE = torch.float64
+    from torch import Tensor
 
-_MIN_TARGET_STD = 1e-6
+    from baybe.surrogates.base import Surrogate
 
 
 def _prepare_inputs(x: Tensor) -> Tensor:
     """Validate and prepare the model input.
 
     Args:
         x: The "raw" model input.
 
     Returns:
         The prepared input.
 
     Raises:
         ValueError: If the model input is empty.
     """
+    from baybe.utils.torch import DTypeFloatTorch
+
     if len(x) == 0:
         raise ValueError("The model input must be non-empty.")
-    return x.to(_DTYPE)
+    return x.to(DTypeFloatTorch)
 
 
 def _prepare_targets(y: Tensor) -> Tensor:
     """Validate and prepare the model targets.
 
     Args:
         y: The "raw" model targets.
 
     Returns:
         The prepared targets.
 
     Raises:
         NotImplementedError: If there is more than one target.
     """
+    from baybe.utils.torch import DTypeFloatTorch
+
     if y.shape[1] != 1:
         raise NotImplementedError(
             "The model currently supports only one target or multiple targets in "
             "DESIRABILITY mode."
         )
-    return y.to(_DTYPE)
+    return y.to(DTypeFloatTorch)
+
 
+def catch_constant_targets(cls: type[Surrogate], std_threshold: float = 1e-6):
+    """Make a ``Surrogate`` class robustly handle constant training targets.
 
-def catch_constant_targets(model_cls: type[Surrogate]):
-    """Wrap a ``Surrogate`` class that cannot handle constant training target values.
+    More specifically, "constant training targets" can mean either of:
+        * The standard deviation of the training targets is below the given threshold.
+        * There is only one target and the standard deviation cannot even be computed.
 
-    In the wrapped class, these cases are handled by a separate model type.
+    The modified class handles the above cases separately from "regular operation"
+    by resorting to a :class:`baybe.surrogates.naive.MeanPredictionSurrogate`,
+    which is stored as an additional temporary attribute in its objects.
 
     Args:
-        model_cls: A ``Surrogate`` class that should be wrapped.
+        cls: The :class:`baybe.surrogates.base.Surrogate` to be augmented.
+        std_threshold: The standard deviation threshold below which operation is
+            switched to the alternative model.
+
+    Raises:
+        ValueError: If the class already contains an attribute with the same name
+            as the temporary attribute to be added.
 
     Returns:
-        A wrapped version of the class.
+        The modified class.
     """
+    # Name of the attribute added to store the alternative model
+    injected_model_attr_name = "_constant_target_model"
 
-    class SplitModel(*model_cls.__bases__):
-        """The class that is used for wrapping.
-
-        It applies a separate recommender for cases where the training
-        targets are all constant and no variance can be estimated.
+    if injected_model_attr_name in (attr.name for attr in cls.__attrs_attrs__):
+        raise ValueError(
+            f"Cannot apply '{catch_constant_targets.__name__}' because "
+            f"'{cls.__name__}' already has an attribute '{injected_model_attr_name}' "
+            f"defined."
+        )
 
-        It stores an instance of the underlying model class.
-        """
+    from baybe.surrogates.naive import MeanPredictionSurrogate
 
-        # The posterior mode is chosen to match that of the wrapped model class
-        joint_posterior: ClassVar[bool] = model_cls.joint_posterior
-        # See base class.
-
-        def __init__(self, *args, **kwargs):
-            super().__init__()
-            self.model = model_cls(*args, **kwargs)
-            self.__class__.__name__ = self.model.__class__.__name__
-            self.model_params = self.model.model_params
-
-        def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
-            """Call the posterior function of the internal model instance."""
-            mean, var = self.model._posterior(candidates)
-
-            # If a joint posterior is expected but the model has been overridden by one
-            # that does not provide covariance information, construct a diagonal
-            # covariance matrix
-            if self.joint_posterior and not self.model.joint_posterior:
-                # Convert to tensor containing covariance matrices
-                var = torch.diag_embed(var)
-
-            return mean, var
-
-        def _fit(
-            self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor
-        ) -> None:
-            """Select a model based on the variance of the targets and fits it."""
-            from baybe.surrogates.naive import MeanPredictionSurrogate
-
-            # https://github.com/pytorch/pytorch/issues/29372
-            # Needs 'unbiased=False' (otherwise, the result will be NaN for scalars)
-            if torch.std(train_y.ravel(), unbiased=False) < _MIN_TARGET_STD:
-                self.model = MeanPredictionSurrogate()
-
-            # Fit the selected model with the training data
-            self.model.fit(searchspace, train_x, train_y)
-
-        def __getattribute__(self, attr):
-            """Access the attributes of the class instance if available.
-
-            If the attributes are not available, it uses the attributes of the internal
-            model instance.
-            """
-            # Try to retrieve the attribute in the class
+    # References to original methods
+    _fit_original = cls._fit
+    _posterior_original = cls._posterior
+
+    def _posterior_new(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
+        # Alternative model fallback
+        if hasattr(self, injected_model_attr_name):
+            return getattr(self, injected_model_attr_name)._posterior(candidates)
+
+        # Regular operation
+        return _posterior_original(self, candidates)
+
+    def _fit_new(
+        self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor
+    ) -> None:
+        if not (train_y.ndim == 2 and train_y.shape[-1] == 1):
+            raise NotImplementedError(
+                "The current logic is only implemented for single-target surrogates."
+            )
+
+        # Alternative model fallback
+        if train_y.numel() == 1 or train_y.std() < std_threshold:
+            model = MeanPredictionSurrogate()
+            model._fit(searchspace, train_x, train_y)
             try:
-                val = super().__getattribute__(attr)
-            except AttributeError:
-                pass
-            else:
-                return val
-
-            # If the attribute has not been overwritten, use that of the internal model
-            return self.model.__getattribute__(attr)
-
-    # Wrapping a class using a decorator does not transfer the doc, resulting in the
-    # autodocumentation not showing the correct docstring. We thus need to manually
-    # assign the docstring of the class.
-    SplitModel.__doc__ = model_cls.__doc__
-    return SplitModel
-
-
-def scale_model(model_cls: type[Surrogate]):
-    """Wrap a ``Surrogate`` class such that it operates with scaled representations.
+                setattr(self, injected_model_attr_name, model)
+            except AttributeError as ex:
+                raise TypeError(
+                    f"'{catch_constant_targets.__name__}' is only applicable to "
+                    f"non-slotted classes but '{cls.__name__}' is a slotted class."
+                ) from ex
+
+        # Regular operation
+        else:
+            if hasattr(self, injected_model_attr_name):
+                delattr(self, injected_model_attr_name)
+            _fit_original(self, searchspace, train_x, train_y)
+
+    # Replace the methods
+    cls._posterior = _posterior_new
+    cls._fit = _fit_new
+
+    return cls
+
+
+def autoscale(cls: type[Surrogate]):
+    """Make a ``Surrogate`` class automatically scale the domain it operates on.
+
+    More specifically, the modified class transforms its inputs before processing them
+    and untransforms the results before returning them. The fitted scaler used for these
+    transformations is stored in the class' objects as an additional temporary
+    attribute.
 
     Args:
-        model_cls: A ``Surrogate`` model class that should be wrapped.
+        cls: The :class:`baybe.surrogates.base.Surrogate` to be augmented.
+
+    Raises:
+        ValueError: If the class already contains an attribute with the same name
+            as the temporary attribute to be added.
 
     Returns:
-        A wrapped version of the class.
+        The modified class.
     """
+    # Name of the attribute added to store the scaler
+    injected_scaler_attr_name = "_autoscaler"
 
-    class ScaledModel(*model_cls.__bases__):
-        """Overrides the methods of the given model class such the use scaled data.
+    if injected_scaler_attr_name in (attr.name for attr in cls.__attrs_attrs__):
+        raise ValueError(
+            f"Cannot apply '{autoscale.__name__}' because "
+            f"'{cls.__name__}' already has an attribute '{injected_scaler_attr_name}' "
+            f"defined."
+        )
 
-        It stores an instance of the underlying model class and a scalar object.
-        """
+    # References to original methods
+    _fit_original = cls._fit
+    _posterior_original = cls._posterior
+
+    def _posterior_new(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
+        scaled = getattr(self, injected_scaler_attr_name).transform(candidates)
+        mean, covar = _posterior_original(self, scaled)
+        return getattr(self, injected_scaler_attr_name).untransform(mean, covar)
+
+    def _fit_new(
+        self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor
+    ) -> None:
+        scaler = DefaultScaler(searchspace.discrete.comp_rep)
+        scaled_x, scaled_y = scaler.fit_transform(train_x, train_y)
+        try:
+            setattr(self, injected_scaler_attr_name, scaler)
+        except AttributeError as ex:
+            raise TypeError(
+                f"'{autoscale.__name__}' is only applicable to "
+                f"non-slotted classes but '{cls.__name__}' is a slotted class."
+            ) from ex
+        _fit_original(self, searchspace, scaled_x, scaled_y)
+
+    # Replace the methods
+    cls._posterior = _posterior_new
+    cls._fit = _fit_new
 
-        # The posterior mode is chosen to match that of the wrapped model class
-        joint_posterior: ClassVar[bool] = model_cls.joint_posterior
-        # See base class.
-
-        def __init__(self, *args, **kwargs):
-            self.model = model_cls(*args, **kwargs)
-            self.__class__.__name__ = self.model.__class__.__name__
-            self.model_params = self.model.model_params
-            self.scaler = None
-
-        def _posterior(self, candidates: Tensor) -> tuple[Tensor, Tensor]:
-            """Call the posterior function of the internal model instance.
-
-            This call is made on a scaled version of the test data and rescales the
-            output accordingly.
-            """
-            candidates = self.scaler.transform(candidates)
-            mean, covar = self.model._posterior(candidates)
-            return self.scaler.untransform(mean, covar)
-
-        def _fit(
-            self, searchspace: SearchSpace, train_x: Tensor, train_y: Tensor
-        ) -> None:
-            """Fits the scaler and the model using the scaled training data."""
-            self.scaler = DefaultScaler(searchspace.discrete.comp_rep)
-            train_x, train_y = self.scaler.fit_transform(train_x, train_y)
-            self.model.fit(searchspace, train_x, train_y)
-
-        def __getattribute__(self, attr):
-            """Access the attributes of the class instance if available.
-
-            If the attributes are not available, it uses the attributes of the internal
-            model instance.
-            """
-            # Try to retrieve the attribute in the class
-            try:
-                val = super().__getattribute__(attr)
-            except AttributeError:
-                pass
-            else:
-                return val
-
-            # If the attribute has not been overwritten, use that of the internal model
-            return self.model.__getattribute__(attr)
-
-    # Wrapping a class using a decorator does not transfer the doc, resulting in the
-    # autodocumentation not showing the correct docstring. We thus need to manually
-    # assign the docstring of the class.
-    ScaledModel.__doc__ = model_cls.__doc__
-    return ScaledModel
+    return cls
 
 
 def batchify(
     posterior: Callable[[Surrogate, Tensor], tuple[Tensor, Tensor]]
 ) -> Callable[[Surrogate, Tensor], tuple[Tensor, Tensor]]:
     """Wrap ``Surrogate`` posterior functions to enable proper batching.
 
@@ -219,24 +205,28 @@
         posterior: The original ``posterior`` function.
 
     Returns:
         The wrapped posterior function.
     """
 
     @wraps(posterior)
-    def sequential_posterior(model: Surrogate, candidates: Tensor) -> [Tensor, Tensor]:
+    def sequential_posterior(
+        model: Surrogate, candidates: Tensor
+    ) -> tuple[Tensor, Tensor]:
         """Replace the posterior function by one that processes batches sequentially.
 
         Args:
             model: The ``Surrogate`` model.
             candidates: The candidates tensor.
 
         Returns:
             The mean and the covariance.
         """
+        import torch
+
         # If no batch dimensions are given, call the model directly
         if candidates.ndim == 2:
             return posterior(model, candidates)
 
         # Keep track of batch dimensions
         t_shape = candidates.shape[:-2]
         q_shape = candidates.shape[-2]
```

### Comparing `baybe-0.8.2/baybe/surrogates/validation.py` & `baybe-0.9.0/baybe/surrogates/validation.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/targets/base.py` & `baybe-0.9.0/baybe/targets/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 """Base functionality for all BayBE targets."""
+
+from __future__ import annotations
+
 import warnings
 from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING
 
 import pandas as pd
 from attrs import define, field
 
 from baybe.serialization import (
     SerialMixin,
     converter,
     get_base_structure_hook,
     unstructure_base,
 )
 
+if TYPE_CHECKING:
+    from baybe.objective import SingleTargetObjective
+
 
 @define(frozen=True)
 class Target(ABC, SerialMixin):
     """Abstract base class for all target variables.
 
     Stores information about the range, transformations, etc.
     """
 
     name: str = field()
     """The name of the target."""
 
+    def to_objective(self) -> SingleTargetObjective:
+        """Create a single-task objective from the target."""
+        from baybe.objectives.single import SingleTargetObjective
+
+        return SingleTargetObjective(self)
+
     @abstractmethod
     def transform(self, data: pd.DataFrame) -> pd.DataFrame:
         """Transform data into computational representation.
 
         The transformation depends on the target mode, e.g. minimization, maximization,
         matching, etc.
```

### Comparing `baybe-0.8.2/baybe/targets/enum.py` & `baybe-0.9.0/baybe/targets/enum.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/targets/numerical.py` & `baybe-0.9.0/baybe/targets/numerical.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,31 +116,42 @@
             raise ValueError(
                 f"You specified bounds for target '{self.name}', but your "
                 f"specified transformation '{value}' is not compatible "
                 f"with the target mode {self.mode}'. It must be one "
                 f"of {_VALID_TRANSFORMATIONS[self.mode]}."
             )
 
+    @property
+    def _is_transform_normalized(self) -> bool:
+        """Indicate if the computational transformation maps to the unit interval."""
+        return (self.bounds.is_bounded) and (self.transformation is not None)
+
     def transform(self, data: pd.DataFrame) -> pd.DataFrame:  # noqa: D102
         # See base class.
 
-        # When bounds are given, apply the respective transformation
-        if self.bounds.is_bounded:
+        # TODO: The method (signature) needs to be refactored, potentially when
+        #   enabling multi-target settings. The current input type suggests that passing
+        #   dataframes is allowed, but the code was designed for single targets and
+        #   desirability objectives, where only one column is present.
+        assert data.shape[1] == 1
+
+        # When a transformation is specified, apply it
+        if self.transformation is not None:
             func = _get_target_transformation(
                 # TODO[typing]: For bounded targets (see if clause), the attrs default
                 #   ensures there is always a transformation specified.
                 #   Use function overloads to make this explicit.
                 self.mode,
                 cast(TargetTransformation, self.transformation),
             )
             transformed = pd.DataFrame(
                 func(data, *self.bounds.to_tuple()), index=data.index
             )
 
-        # If no bounds are given, simply negate all target values for ``MIN`` mode.
+        # Otherwise, simply negate all target values for ``MIN`` mode.
         # For ``MAX`` mode, nothing needs to be done.
         # For ``MATCH`` mode, the validators avoid a situation without specified bounds.
         elif self.mode is TargetMode.MIN:
             transformed = -data
 
         else:
             transformed = data.copy()
```

### Comparing `baybe-0.8.2/baybe/targets/transforms.py` & `baybe-0.9.0/baybe/targets/transforms.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/telemetry.py` & `baybe-0.9.0/baybe/telemetry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,22 @@
 """Telemetry functionality for BayBE.
 
-Important:
-    BayBE collects anonymous usage statistics **only** for employees of Merck KGaA,
-    Darmstadt, Germany and/or its affiliates. The recording of metrics is turned off
-    for all other users and impossible due to a VPN block. In any case, the usage
-    statistics do **not** involve logging of recorded measurements, targets or any
-    project information that would allow for reconstruction of details. The user and
-    host machine names are irreversibly anonymized.
-
-**Monitored quantities are:**
-    * ``batch_size`` used when querying recommendations
-    * Number of parameters in the search space
-    * Number of constraints in the search space
-    * How often ``recommend`` was called
-    * How often ``add_measurements`` was called
-    * How often a search space is newly created
-    * How often initial measurements are added before recommendations were calculated
-      ("naked initial measurements")
-    * The fraction of measurements added that correspond to previous recommendations
-    * Each measurement is associated with an irreversible hash of the user- and hostname
-
-**The following environment variables control the behavior of BayBE telemetry:**
-
-``BAYBE_TELEMETRY_ENABLED``
-    Flag that can turn off telemetry entirely (default is `true`). To turn it off set it
-    to `false`.
-
-``BAYBE_TELEMETRY_ENDPOINT``
-    The receiving endpoint URL for telemetry data.
-
-``BAYBE_TELEMETRY_VPN_CHECK``
-    Flag turning an initial telemetry connectivity check on/off (default is `true`).
-
-``BAYBE_TELEMETRY_VPN_CHECK_TIMEOUT``
-    The timeout in seconds for the check whether the endpoint URL is reachable.
-
-``BAYBE_TELEMETRY_USERNAME``
-    The name of the user executing BayBE code. Defaults to an irreversible hash of
-    the username according to the OS.
-
-``BAYBE_TELEMETRY_HOSTNAME``
-    The name of the machine executing BayBE code. Defaults to an irreversible hash of
-    the machine name.
-
-If you wish to disable logging, you can set the following environment variable:
-
-.. code-block:: console
-
-    export BAYBE_TELEMETRY_ENABLED=false
-
-or in Python:
-
-.. code-block:: python
-
-    import os
-    os.environ["BAYBE_TELEMETRY_ENABLED"] = "false"
-
-before calling any BayBE functionality.
-
-Telemetry can be re-enabled by simply removing the variable:
-
-.. code-block:: console
-
-    unset BAYBE_TELEMETRY_ENABLED
-
-or in Python:
-
-.. code-block:: python
-
-    os.environ.pop["BAYBE_TELEMETRY_ENABLED"]
-
-Note, however, that (un-)setting the variable in the shell will not affect the running
-Python session.
+For more details, see https://emdgroup.github.io/baybe/userguide/envvars.html#telemetry
 """
+
 import getpass
 import hashlib
 import os
 import socket
 import warnings
+from collections.abc import Sequence
 from typing import Union
 from urllib.parse import urlparse
 
 import pandas as pd
-import requests
 
 from baybe.parameters.base import Parameter
 from baybe.utils.boolean import strtobool
 from baybe.utils.dataframe import fuzzy_row_match
 
 # Telemetry environment variable names
 VARNAME_TELEMETRY_ENABLED = "BAYBE_TELEMETRY_ENABLED"
@@ -100,27 +30,14 @@
 DEFAULT_TELEMETRY_ENABLED = "true"
 DEFAULT_TELEMETRY_ENDPOINT = (
     "https://public.telemetry.baybe.p.uptimize.merckgroup.com:4317"
 )
 DEFAULT_TELEMETRY_VPN_CHECK = "true"
 DEFAULT_TELEMETRY_VPN_CHECK_TIMEOUT = "0.5"
 
-try:
-    DEFAULT_TELEMETRY_USERNAME = (
-        hashlib.sha256(getpass.getuser().upper().encode()).hexdigest().upper()[:10]
-    )  # this hash is irreversible and cannot identify the user or their machine
-except ModuleNotFoundError:
-    # getpass.getuser() does not work on Windows if all the environment variables
-    # it checks are empty. Since then there is no way of inferring the username, we
-    # use UNKNOWN as fallback.
-    DEFAULT_TELEMETRY_USERNAME = "UNKNOWN"
-
-DEFAULT_TELEMETRY_HOSTNAME = (
-    hashlib.sha256(socket.gethostname().encode()).hexdigest().upper()[:10]
-)  # this hash is irreversible and cannot identify the user or their machine
 
 # Telemetry labels for metrics
 TELEM_LABELS = {
     "RECOMMENDED_MEASUREMENTS_PERCENTAGE": "value_recommended-measurements-percentage",
     "BATCH_SIZE": "value_batch-size",
     "COUNT_ADD_RESULTS": "count_add-results",
     "COUNT_RECOMMEND": "count_recommend",
@@ -159,14 +76,29 @@
     return strtobool(
         os.environ.get(VARNAME_TELEMETRY_ENABLED, DEFAULT_TELEMETRY_ENABLED)
     )
 
 
 # Attempt telemetry initialization
 if is_enabled():
+    # Assign default user and machine name
+    try:
+        DEFAULT_TELEMETRY_USERNAME = (
+            hashlib.sha256(getpass.getuser().upper().encode()).hexdigest().upper()[:10]
+        )
+    except ModuleNotFoundError:
+        # getpass.getuser() does not work on Windows if all the environment variables
+        # it checks are empty. Since then there is no way of inferring the username, we
+        # use UNKNOWN as fallback.
+        DEFAULT_TELEMETRY_USERNAME = "UNKNOWN"
+
+    DEFAULT_TELEMETRY_HOSTNAME = (
+        hashlib.sha256(socket.gethostname().encode()).hexdigest().upper()[:10]
+    )
+
     _endpoint_url = os.environ.get(
         VARNAME_TELEMETRY_ENDPOINT, DEFAULT_TELEMETRY_ENDPOINT
     )
 
     # Test endpoint URL
     try:
         # Parse endpoint URL
@@ -190,19 +122,15 @@
             _TIMEOUT_S = float(DEFAULT_TELEMETRY_VPN_CHECK_TIMEOUT)
 
         # Send a test request. If there is no internet connection or a firewall is
         # present this will throw an error and telemetry will be deactivated.
         if strtobool(
             os.environ.get(VARNAME_TELEMETRY_VPN_CHECK, DEFAULT_TELEMETRY_VPN_CHECK)
         ):
-            response = requests.get(
-                "http://verkehrsnachrichten.merck.de/", timeout=_TIMEOUT_S
-            )
-            if response.status_code != 200:
-                raise requests.RequestException("Cannot reach telemetry network.")
+            socket.gethostbyname("verkehrsnachrichten.merck.de")
 
         # User has connectivity to the telemetry endpoint, so we initialize
         _instruments: dict[str, Histogram] = {}
         _resource = Resource.create(
             {"service.namespace": "BayBE", "service.name": "SDK"}
         )
         _reader = PeriodicExportingMetricReader(
@@ -215,21 +143,27 @@
         set_meter_provider(_provider)
         _meter = get_meter("aws-otel", "1.0")
     except Exception as ex:
         # Catching broad exception here and disabling telemetry in that case to avoid
         # any telemetry timeouts or interference for the user in case of unexpected
         # errors. Possible ones are for instance ``socket.gaierror`` in case the user
         # has no internet connection.
-        warnings.warn(
-            f"WARNING: BayBE Telemetry endpoint {_endpoint_url} cannot be reached. "
-            "Disabling telemetry. The exception encountered was: "
-            f"{type(ex).__name__}, {ex}",
-            UserWarning,
-        )
+        if os.environ.get(VARNAME_TELEMETRY_USERNAME, "").startswith("DEV_"):
+            # This warning is only printed for developers to make them aware of
+            # potential issues
+            warnings.warn(
+                f"WARNING: BayBE Telemetry endpoint {_endpoint_url} cannot be reached. "
+                "Disabling telemetry. The exception encountered was: "
+                f"{type(ex).__name__}, {ex}",
+                UserWarning,
+            )
         os.environ[VARNAME_TELEMETRY_ENABLED] = "false"
+else:
+    DEFAULT_TELEMETRY_USERNAME = "UNKNOWN"
+    DEFAULT_TELEMETRY_HOSTNAME = "UNKNOWN"
 
 
 def get_user_details() -> dict[str, str]:
     """Generate user details.
 
     These are submitted as metadata with requested telemetry stats.
 
@@ -276,15 +210,15 @@
         _instruments[instrument_name] = histogram
     histogram.record(value, get_user_details())
 
 
 def telemetry_record_recommended_measurement_percentage(
     cached_recommendation: pd.DataFrame,
     measurements: pd.DataFrame,
-    parameters: list[Parameter],
+    parameters: Sequence[Parameter],
     numerical_measurements_must_be_within_tolerance: bool,
 ) -> None:
     """Submit the percentage of added measurements.
 
     More precisely, submit the percentage of added measurements that correspond to
     previously recommended ones (called cached recommendations).
```

### Comparing `baybe-0.8.2/baybe/utils/boolean.py` & `baybe-0.9.0/baybe/utils/boolean.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Functions implementing boolean checks."""
 
 from abc import ABC
 from typing import Any
 
-from attr import cmp_using
+from attrs import cmp_using
+from typing_extensions import is_protocol
 
 # Used for comparing pandas dataframes in attrs classes
 eq_dataframe = cmp_using(lambda x, y: x.equals(y))
 
 
 def is_abstract(cls: Any) -> bool:
     """Determine if a given class is abstract.
 
     This check is more general sense than ``inspect.abstract``, which only verifies
     if a class has abstract methods. The latter can be problematic when the class has
     no abstract methods but is nevertheless not directly usable, for example, because it
     has uninitialized members, which are only covered in its non-"abstract" subclasses.
-    By contrast, this method simply checks if the class derives from ``abc.ABC``.
+
+    By contrast, this method simply checks if the class derives from ``abc.ABC`` or
+    is a protocol class.
 
     Args:
         cls: The class to be inspected.
 
     Returns:
         ``True`` if the class is "abstract" (see definition above), ``False`` else.
     """
-    return ABC in cls.__bases__
+    return ABC in cls.__bases__ or is_protocol(cls)
 
 
 def strtobool(val: str) -> bool:
     """Convert a string representation of truth to ``True`` or ``False``.
 
     Adapted from distutils.
     True values are ``y``, ``yes``, ``t``, ``true``, ``on``, and ``1``.
```

### Comparing `baybe-0.8.2/baybe/utils/botorch_wrapper.py` & `baybe-0.9.0/baybe/utils/botorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/utils/chemistry.py` & `baybe-0.9.0/baybe/utils/chemistry.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/utils/dataframe.py` & `baybe-0.9.0/baybe/utils/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 """Dataframe utilities."""
 
 from __future__ import annotations
 
 import logging
-from collections.abc import Iterable
-from typing import TYPE_CHECKING, Literal, Optional, Union
+from collections.abc import Iterable, Iterator, Sequence
+from typing import (
+    TYPE_CHECKING,
+    Literal,
+    Optional,
+    Union,
+    overload,
+)
 
 import numpy as np
 import pandas as pd
 
-from baybe.parameters.base import ContinuousParameter, DiscreteParameter
 from baybe.targets.enum import TargetMode
-from baybe.utils.numerical import DTypeFloatNumpy, DTypeFloatTorch
+from baybe.utils.numerical import DTypeFloatNumpy
 
 if TYPE_CHECKING:
     from torch import Tensor
 
     from baybe.campaign import Campaign
     from baybe.parameters import Parameter
 
 # Logging
 _logger = logging.getLogger(__name__)
 
 
-def to_tensor(*dfs: pd.DataFrame) -> Union[Tensor, Iterable[Tensor]]:
+@overload
+def to_tensor(df: pd.DataFrame) -> Tensor:
+    ...
+
+
+@overload
+def to_tensor(*dfs: pd.DataFrame) -> Iterator[Tensor]:
+    ...
+
+
+def to_tensor(*dfs: pd.DataFrame) -> Union[Tensor, Iterator[Tensor]]:
     """Convert a given set of dataframes into tensors (dropping all indices).
 
     Args:
         *dfs: A set of dataframes
 
     Returns:
         The provided dataframe(s), transformed into Tensor(s)
@@ -37,14 +52,16 @@
     #  weirdly happen, even if all values are numeric, e.g. when a target column is
     #  looked up from a df in simulation, it can have dtype object even if it's all
     #  floats. As a simple fix (this seems to be the most reasonable place to take
     #  care of this) df.values has been changed to df.values.astype(float),
     #  even though this seems like double casting here.
     import torch
 
+    from baybe.utils.torch import DTypeFloatTorch
+
     out = (
         torch.from_numpy(df.values.astype(DTypeFloatNumpy)).to(DTypeFloatTorch)
         for df in dfs
     )
     if len(dfs) == 1:
         out = next(out)
     return out
@@ -228,16 +245,18 @@
             data[param.name] *= np.random.uniform(
                 1.0 - noise_level / 100.0, 1.0 + noise_level / 100.0, len(data)
             )
         elif noise_type == "absolute":
             data[param.name] += np.random.uniform(-noise_level, noise_level, len(data))
 
         # Respect continuous intervals
-        if isinstance(param, ContinuousParameter):
-            data[param.name].clip(param.bounds.lower, param.bounds.upper, inplace=True)
+        if param.is_continuous:
+            data[param.name] = data[param.name].clip(
+                param.bounds.lower, param.bounds.upper
+            )
 
 
 def df_drop_single_value_columns(
     df: pd.DataFrame, lst_exclude: list = None
 ) -> pd.DataFrame:
     """Drop dataframe columns with zero variance.
 
@@ -320,15 +339,15 @@
 
     return data
 
 
 def fuzzy_row_match(
     left_df: pd.DataFrame,
     right_df: pd.DataFrame,
-    parameters: list[Parameter],
+    parameters: Sequence[Parameter],
     numerical_measurements_must_be_within_tolerance: bool,
 ) -> pd.Index:
     """Match row of the right dataframe to the rows of the left dataframe.
 
     This is useful for validity checks and to automatically match measurements to
     entries in the search space, e.g. to detect which ones have been measured.
     For categorical parameters, there needs to be an exact match with any of the
@@ -382,19 +401,15 @@
                     f"the input value is within the specified tolerance/range. Set "
                     f"the flag 'numerical_measurements_must_be_within_tolerance' "
                     f"to 'False' to disable this behavior."
                 )
 
         # Differentiate category-like and discrete numerical parameters
         cat_cols = [p.name for p in parameters if not p.is_numeric]
-        num_cols = [
-            p.name
-            for p in parameters
-            if (p.is_numeric and isinstance(p, DiscreteParameter))
-        ]
+        num_cols = [p.name for p in parameters if (p.is_numeric and p.is_discrete)]
 
         # Discrete parameters must match exactly
         match = left_df[cat_cols].eq(row[cat_cols]).all(axis=1, skipna=False)
 
         # For numeric parameters, match the entry with the smallest deviation
         # TODO: allow alternative distance metrics
         for col in num_cols:
```

### Comparing `baybe-0.8.2/baybe/utils/interval.py` & `baybe-0.9.0/baybe/utils/interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 import numpy as np
 from attrs import define, field
 from packaging import version
 
 from baybe.serialization import SerialMixin, converter
-from baybe.utils.numerical import DTypeFloatNumpy, DTypeFloatTorch
+from baybe.utils.numerical import DTypeFloatNumpy
 
 if TYPE_CHECKING:
     from torch import Tensor
 
 # TODO[typing]: Add return type hints to classmethod constructors once ForwardRefs
 #   are supported: https://bugs.python.org/issue41987
 
@@ -128,29 +128,31 @@
         """Transform the interval to a :class:`numpy.ndarray`."""
         return np.array([self.lower, self.upper], dtype=DTypeFloatNumpy)
 
     def to_tensor(self) -> "Tensor":
         """Transform the interval to a :class:`torch.Tensor`."""
         import torch
 
+        from baybe.utils.torch import DTypeFloatTorch
+
         return torch.tensor([self.lower, self.upper], dtype=DTypeFloatTorch)
 
     def contains(self, number: float) -> bool:
         """Check whether the interval contains a given number.
 
         Args:
             number: The number that should be checked.
 
         Returns:
             Whether or not the interval contains the number.
         """
         return self.lower <= number <= self.upper
 
 
-def convert_bounds(bounds: Union[None, tuple, Interval]) -> Interval:
+def convert_bounds(bounds: Union[None, Iterable, Interval]) -> Interval:
     """Convert bounds given in another format to an interval.
 
     Args:
         bounds: The bounds that should be transformed to an interval.
 
     Returns:
         The interval.
```

### Comparing `baybe-0.8.2/baybe/utils/numerical.py` & `baybe-0.9.0/baybe/utils/numerical.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 """Utilities for numeric operations."""
 
+import os
+from collections.abc import Sequence
+
 import numpy as np
-import torch
+import numpy.typing as npt
 
-DTypeFloatNumpy = np.float64
-"""Floating point data type used for numpy arrays."""
+from baybe.utils.boolean import strtobool
 
-DTypeFloatTorch = torch.float64
-"""Floating point data type used for torch tensors."""
+VARNAME_NUMPY_USE_SINGLE_PRECISION = "BAYBE_NUMPY_USE_SINGLE_PRECISION"
+"""Environment variable name for enforcing single precision in numpy."""
+
+DTypeFloatNumpy = (
+    np.float32
+    if strtobool(os.environ.get(VARNAME_NUMPY_USE_SINGLE_PRECISION, "False"))
+    else np.float64
+)
+"""Floating point data type used for numpy arrays."""
 
 DTypeFloatONNX = np.float32
 """Floating point data type used for ONNX models.
 
 Currently, ONNX runtime does not seem to have full support for double precision.
 There is no clear documentation but some references can be found here (version 1.16.0):
 
  * https://onnx.ai/sklearn-onnx/auto_tutorial/plot_abegin_convert_pipeline.html#converts-the-model
  * https://onnx.ai/sklearn-onnx/auto_tutorial/plot_ebegin_float_double.html
 """  # noqa: E501
 
 
-def geom_mean(arr: np.ndarray, weights: list[float]) -> np.ndarray:
+def geom_mean(arr: np.ndarray, weights: Sequence[float]) -> np.ndarray:
     """Calculate the (weighted) geometric mean along the second axis of a 2-D array.
 
     Alternative to ``gmean`` from scipy that avoids logarithms and division errors.
 
     Args:
         arr: The array containing the values for the mean computation.
         weights: Weights for the mean computation.
 
     Returns:
         A 1-D array containing the row-wise geometric means of the given array.
     """
     return np.prod(np.power(arr, np.atleast_2d(weights) / np.sum(weights)), axis=1)
 
 
-def closest_element(array: np.ndarray, target: float) -> float:
+def closest_element(array: npt.ArrayLike, target: float) -> float:
     """Find the element of an array that is closest to a target value.
 
     Args:
-        array: The array in which the closest value should be found.
+        array: The array in which the closest value is to be found.
         target: The target value.
 
     Returns:
-        The closes element.
+        The closest element.
     """
+    if np.ndim(array) == 0:
+        return np.asarray(array).item()
+    array = np.ravel(array)
     return array[np.abs(array - target).argmin()]
 
 
 def closer_element(x: float, y: float, target: float) -> float:
     """Determine which of two given inputs is closer to a target value.
 
     Args:
```

### Comparing `baybe-0.8.2/baybe/utils/plotting.py` & `baybe-0.9.0/baybe/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe/utils/sampling_algorithms.py` & `baybe-0.9.0/baybe/utils/sampling_algorithms.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/baybe.egg-info/PKG-INFO` & `baybe-0.9.0/baybe.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baybe
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Bayesian Back End for Design of Experiments
 Author: Merck KGaA, Darmstadt, Germany
 License: Apache-2.0
 Project-URL: Homepage, https://emdgroup.github.io/baybe/
 Project-URL: Documentation, https://emdgroup.github.io/baybe/_autosummary/baybe.html
 Project-URL: Changelog, https://emdgroup.github.io/baybe/misc/changelog_link.html
 Project-URL: GitHub, https://github.com/emdgroup/baybe/
@@ -35,20 +35,19 @@
 Requires-Dist: pandas>=1.4.2
 Requires-Dist: protobuf<=3.20.3
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: scikit-learn-extra>=0.3.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: setuptools-scm>=7.1.0
 Requires-Dist: torch>=1.13.1
+Requires-Dist: typing_extensions>=4.7.0
 Requires-Dist: opentelemetry-sdk>=1.16.0
 Requires-Dist: opentelemetry-propagator-aws-xray>=1.0.0
 Requires-Dist: opentelemetry-exporter-otlp>=1.16.0
 Requires-Dist: opentelemetry-sdk-extension-aws>=2.0.0
-Requires-Dist: requests>=2.31.0
-Requires-Dist: urllib3>=2.0.7
 Provides-Extra: chem
 Requires-Dist: rdkit>=2022.3.4; extra == "chem"
 Requires-Dist: mordredcommunity>=1.2.0; extra == "chem"
 Provides-Extra: onnx
 Requires-Dist: onnx>=1.16.0; extra == "onnx"
 Requires-Dist: onnxruntime>=1.15.1; extra == "onnx"
 Requires-Dist: skl2onnx>=1.15.0; extra == "onnx"
@@ -58,15 +57,15 @@
 Requires-Dist: baybe[examples]; extra == "dev"
 Requires-Dist: baybe[lint]; extra == "dev"
 Requires-Dist: baybe[mypy]; extra == "dev"
 Requires-Dist: baybe[onnx]; extra == "dev"
 Requires-Dist: baybe[simulation]; extra == "dev"
 Requires-Dist: baybe[test]; extra == "dev"
 Requires-Dist: pip-audit>=2.5.5; extra == "dev"
-Requires-Dist: tox>=4.10.0; extra == "dev"
+Requires-Dist: tox-uv>=1.7.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: baybe[examples]; extra == "docs"
 Requires-Dist: furo>=2023.09.10; extra == "docs"
 Requires-Dist: jupyter>=1.0.0; extra == "docs"
 Requires-Dist: jupytext>=1.16.1; extra == "docs"
 Requires-Dist: myst-parser>=2.0.0; extra == "docs"
 Requires-Dist: sphinx>=7.1.1; extra == "docs"
@@ -89,15 +88,14 @@
 Requires-Dist: pydoclint==0.2.1; extra == "lint"
 Requires-Dist: ruff==0.1.6; extra == "lint"
 Requires-Dist: typos==1.16.23; extra == "lint"
 Provides-Extra: mypy
 Requires-Dist: mypy>=1.6.1; extra == "mypy"
 Requires-Dist: pandas-stubs>=2.0.3.230814; extra == "mypy"
 Requires-Dist: funcy-stubs>=0.1.1; extra == "mypy"
-Requires-Dist: types-requests>=2.31.0.20240106; extra == "mypy"
 Requires-Dist: types-seaborn>=0.12.2; extra == "mypy"
 Provides-Extra: simulation
 Requires-Dist: xyzpy>=1.2.1; extra == "simulation"
 Provides-Extra: test
 Requires-Dist: baybe[lint]; extra == "test"
 Requires-Dist: hypothesis[pandas]>=6.88.4; extra == "test"
 Requires-Dist: pytest>=7.2.0; extra == "test"
@@ -127,63 +125,62 @@
 &nbsp;•&nbsp;
 <a href="https://emdgroup.github.io/baybe/misc/contributing_link.html">Contribute<a/>
 &nbsp;
 </div>
 
 # BayBE — A Bayesian Back End for Design of Experiments
 
-The Bayesian Back End (**BayBE**) provides a general-purpose toolbox for Bayesian Design
+The Bayesian Back End (**BayBE**) is a general-purpose toolbox for Bayesian Design
 of Experiments, focusing on additions that enable real-world experimental campaigns.
 
 Besides functionality to perform a typical recommend-measure loop, BayBE's highlights are:
-- Custom parameter encodings: Improve your campaign with domain knowledge
-- Built-in chemical encodings: Improve your campaign with chemical knowledge
-- Single and multiple targets with min, max and match objectives
-- Custom surrogate models: For specialized problems or active learning
-- Hybrid (mixed continuous and discrete) spaces
-- Transfer learning: Mix data from multiple campaigns and accelerate optimization
-- Comprehensive backtest, simulation and imputation utilities: Benchmark and find your best settings
-- Fully typed and hypothesis-tested: Robust code base
-- All objects are fully de-/serializable: Useful for storing results in databases or use in wrappers like APIs
+- ✨ Custom parameter encodings: Improve your campaign with domain knowledge
+- 🧪 Built-in chemical encodings: Improve your campaign with chemical knowledge
+- 🎯 Single and multiple targets with min, max and match objectives
+- ⚙️ Custom surrogate models: For specialized problems or active learning
+- 🎭 Hybrid (mixed continuous and discrete) spaces
+- 🚀 Transfer learning: Mix data from multiple campaigns and accelerate optimization
+- 📈 Comprehensive backtest, simulation and imputation utilities: Benchmark and find your best settings
+- 📝 Fully typed and hypothesis-tested: Robust code base
+- 🔄 All objects are fully de-/serializable: Useful for storing results in databases or use in wrappers like APIs
 
 
-## Quick Start
+## ⚡ Quick Start
 
 Let us consider a simple experiment where we control three parameters and want to
 maximize a single target called `Yield`.
 
 First, install BayBE into your Python environment: 
 ```bash 
 pip install baybe 
 ``` 
 For more information on this step, see our
 [detailed installation instructions](#installation).
 
 ### Defining the Optimization Objective
 
 In BayBE's language, the `Yield` can be represented as a `NumericalTarget`,
-which we pass into an `Objective`.
+which we wrap into a `SingleTargetObjective`:
 
 ```python
 from baybe.targets import NumericalTarget
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 
 target = NumericalTarget(
     name="Yield",
     mode="MAX",
 )
-objective = Objective(mode="SINGLE", targets=[target])
+objective = SingleTargetObjective(target=target)
 ```
-
-In cases where we need to consider multiple (potentially competing) targets, the
-role of the `Objective` is to define additional settings, e.g. how these targets should
-be balanced.
-In `SINGLE` mode, however, there are no additional settings.
-For more details, see 
-[the objective section of the user guide](https://emdgroup.github.io/baybe/userguide/objective.html).
+In cases where we are confronted with multiple (potentially conflicting) targets,
+the `DesirabilityObjective` can be used instead. It allows to define additional
+settings, such as how these targets should be balanced.
+For more details, see the
+[objectives section](https://emdgroup.github.io/baybe/userguide/objectives.html)
+of the user guide.
 
 ### Defining the Search Space
 
 Next, we inform BayBE about the available "control knobs", that is, the underlying
 system parameters we can tune to optimize our targets. This also involves specifying 
 their values/ranges and other parameter-specific details.
 
@@ -226,23 +223,27 @@
 of the user guide.
 
 Additionally, we can define a set of constraints to further specify allowed ranges and
 relationships between our parameters. Details can be found in the
 [constraints section](https://emdgroup.github.io/baybe/userguide/constraints.html) of the user guide.
 In this example, we assume no further constraints.
 
-With the parameter and constraint definitions at hand, we can now create our
+With the parameter definitions at hand, we can now create our
 `SearchSpace` based on the Cartesian product of all possible parameter values:
 
 ```python
 from baybe.searchspace import SearchSpace
 
 searchspace = SearchSpace.from_product(parameters)
 ```
 
+See the [search spaces section](https://emdgroup.github.io/baybe/userguide/searchspace.html)
+of our user guide for more information on the structure of search spaces
+and alternative ways of construction. 
+
 ### Optional: Defining the Optimization Strategy
 
 As an optional step, we can specify details on how the optimization should be
 conducted. If omitted, BayBE will choose a default setting.
 
 For our example, we combine two recommenders via a so-called meta recommender named
 `TwoPhaseMetaRecommender`:
@@ -313,27 +314,27 @@
 campaign.add_measurements(df)
 ```
 
 With the newly arrived data, BayBE can produce a refined design for the next iteration.
 This loop would typically continue until a desired target value has been achieved in
 the experiment.
 
-### Advanced Example - Chemical Substances
+### Advanced Example: Chemical Substances
 BayBE has several modules to go beyond traditional approaches. One such example is the
 use of custom encodings for categorical parameters. Chemical encodings for substances
 are a special built-in case of this that comes with BayBE.
 
 In the following picture you can see
 the outcome for treating the solvent, base and ligand in a direct arylation reaction
 optimization (from [Shields, B.J. et al.](https://doi.org/10.1038/s41586-021-03213-y)) with
 chemical encodings compared to one-hot and a random baseline:
 ![Substance Encoding Example](./examples/Backtesting/full_lookup_light.svg)
 
 (installation)=
-## Installation
+## 💻 Installation
 ### From Package Index
 The easiest way to install BayBE is via PyPI:
 
 ```bash
 pip install baybe
 ```
 
@@ -394,28 +395,43 @@
 - `lint`: Required for linting and formatting.
 - `mypy`: Required for static type checking.
 - `onnx`: Required for using custom surrogate models in [ONNX format](https://onnx.ai).
 - `simulation`: Enabling the [simulation](https://emdgroup.github.io/baybe/_autosummary/baybe.simulation.html) module.
 - `test`: Required for running the tests.
 - `dev`: All of the above plus `tox` and `pip-audit`. For code contributors.
 
+## 📡 Telemetry
+BayBE collects anonymous usage statistics **only** for employees of Merck KGaA, 
+Darmstadt, Germany and/or its affiliates. The recording of metrics is turned off for
+all other users and is impossible due to a VPN block. In any case, the usage statistics
+do **not** involve logging of recorded measurements, targets/parameters or their names
+or any project information that would allow for reconstruction of details. The user and
+host machine names are anonymized with via truncated hashing.
+- You can verify the above statements by studying the open-source code in the
+  `telemetry` module.
+- You can always deactivate all telemetry by setting the environment variable 
+  `BAYBE_TELEMETRY_ENABLED` to `false` or `off`. For details please consult
+  [this page](https://emdgroup.github.io/baybe/userguide/envvars.html#telemetry).
+- If you want to be absolutely sure, you can uninstall internet related packages such
+  as `opentelemetry*` or its secondary dependencies from the environment. Due to the
+  inability of specifying opt-out dependencies, these are installed by default, but the
+  package works without them.
 
-## Authors
+## 👨🏻‍🔧 Maintainers
 
 - Martin Fitzner (Merck KGaA, Darmstadt, Germany), [Contact](mailto:martin.fitzner@merckgroup.com), [Github](https://github.com/Scienfitz)
 - Adrian Šošić (Merck Life Science KGaA, Darmstadt, Germany), [Contact](mailto:adrian.sosic@merckgroup.com), [Github](https://github.com/AdrianSosic)
 - Alexander Hopp (Merck KGaA, Darmstadt, Germany) [Contact](mailto:alexander.hopp@merckgroup.com), [Github](https://github.com/AVHopp)
-- Alex Lee (EMD Electronics, Tempe, Arizona, USA) [Contact](mailto:alex.lee@emdgroup.com), [Github](https://github.com/galaxee87)
 
 
-## Known Issues
+## 🛠️ Known Issues
 A list of know issues can be found [here](https://emdgroup.github.io/baybe/known_issues.html).
 
 
-## License
+## 📄 License
 
 Copyright 2022-2024 Merck KGaA, Darmstadt, Germany
 and/or its affiliates. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `baybe-0.8.2/baybe.egg-info/SOURCES.txt` & `baybe-0.9.0/baybe.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,43 +14,59 @@
 .github/CODEOWNERS
 .github/workflows/ci.yml
 .github/workflows/docs.yml
 .github/workflows/regular.yml
 .github/workflows/release.yml
 .github/workflows/reminders.yml
 baybe/__init__.py
-baybe/acquisition.py
 baybe/campaign.py
 baybe/deprecation.py
 baybe/exceptions.py
 baybe/objective.py
 baybe/scaler.py
-baybe/simulation.py
-baybe/surrogate.py
 baybe/telemetry.py
 baybe.egg-info/PKG-INFO
 baybe.egg-info/SOURCES.txt
 baybe.egg-info/dependency_links.txt
 baybe.egg-info/requires.txt
 baybe.egg-info/top_level.txt
+baybe/acquisition/__init__.py
+baybe/acquisition/_adapter.py
+baybe/acquisition/acqfs.py
+baybe/acquisition/base.py
+baybe/acquisition/partial.py
+baybe/acquisition/utils.py
 baybe/constraints/__init__.py
 baybe/constraints/base.py
 baybe/constraints/conditions.py
 baybe/constraints/continuous.py
 baybe/constraints/discrete.py
 baybe/constraints/validation.py
+baybe/kernels/__init__.py
+baybe/kernels/base.py
+baybe/kernels/basic.py
+baybe/kernels/composite.py
+baybe/objectives/__init__.py
+baybe/objectives/base.py
+baybe/objectives/deprecation.py
+baybe/objectives/desirability.py
+baybe/objectives/enum.py
+baybe/objectives/single.py
 baybe/parameters/__init__.py
 baybe/parameters/base.py
 baybe/parameters/categorical.py
 baybe/parameters/custom.py
 baybe/parameters/enum.py
 baybe/parameters/numerical.py
 baybe/parameters/substance.py
 baybe/parameters/utils.py
 baybe/parameters/validation.py
+baybe/priors/__init__.py
+baybe/priors/base.py
+baybe/priors/basic.py
 baybe/recommenders/__init__.py
 baybe/recommenders/base.py
 baybe/recommenders/deprecation.py
 baybe/recommenders/naive.py
 baybe/recommenders/meta/__init__.py
 baybe/recommenders/meta/base.py
 baybe/recommenders/meta/sequential.py
@@ -68,42 +84,56 @@
 baybe/searchspace/core.py
 baybe/searchspace/discrete.py
 baybe/searchspace/validation.py
 baybe/serialization/__init__.py
 baybe/serialization/core.py
 baybe/serialization/mixin.py
 baybe/serialization/utils.py
+baybe/simulation/__init__.py
+baybe/simulation/core.py
+baybe/simulation/lookup.py
+baybe/simulation/scenarios.py
+baybe/simulation/transfer_learning.py
 baybe/strategies/__init__.py
 baybe/strategies/deprecation.py
 baybe/surrogates/__init__.py
 baybe/surrogates/base.py
 baybe/surrogates/custom.py
-baybe/surrogates/gaussian_process.py
 baybe/surrogates/linear.py
 baybe/surrogates/naive.py
 baybe/surrogates/ngboost.py
 baybe/surrogates/random_forest.py
 baybe/surrogates/utils.py
 baybe/surrogates/validation.py
+baybe/surrogates/gaussian_process/__init__.py
+baybe/surrogates/gaussian_process/core.py
+baybe/surrogates/gaussian_process/kernel_factory.py
+baybe/surrogates/gaussian_process/presets/__init__.py
+baybe/surrogates/gaussian_process/presets/core.py
+baybe/surrogates/gaussian_process/presets/default.py
 baybe/targets/__init__.py
 baybe/targets/base.py
-baybe/targets/deprecation.py
 baybe/targets/enum.py
 baybe/targets/numerical.py
 baybe/targets/transforms.py
 baybe/utils/__init__.py
 baybe/utils/basic.py
 baybe/utils/boolean.py
 baybe/utils/botorch_wrapper.py
 baybe/utils/chemistry.py
+baybe/utils/conversion.py
 baybe/utils/dataframe.py
 baybe/utils/interval.py
+baybe/utils/memory.py
 baybe/utils/numerical.py
 baybe/utils/plotting.py
+baybe/utils/random.py
 baybe/utils/sampling_algorithms.py
+baybe/utils/torch.py
+baybe/utils/validation.py
 docs/conf.py
 docs/index.md
 docs/known_issues.md
 docs/_static/banner1.svg
 docs/_static/banner2.svg
 docs/_static/custom.css
 docs/_static/favicon.ico
@@ -117,18 +147,20 @@
 docs/scripts/convert_code_to_documentation.py
 docs/scripts/utils.py
 docs/templates/custom-attribute-template.rst
 docs/templates/custom-class-template.rst
 docs/templates/custom-module-template.rst
 docs/userguide/campaigns.md
 docs/userguide/constraints.md
-docs/userguide/objective.md
+docs/userguide/envvars.md
+docs/userguide/objectives.md
 docs/userguide/parameters.md
 docs/userguide/recommenders.md
 docs/userguide/searchspace.md
+docs/userguide/serialization.md
 docs/userguide/simulation.md
 docs/userguide/surrogates.md
 docs/userguide/targets.md
 docs/userguide/transfer_learning.md
 docs/userguide/userguide.md
 examples/plotting_themes.json
 examples/Backtesting/Backtesting_Header.md
@@ -182,49 +214,65 @@
 examples/Transfer_Learning/basic_transfer_learning_light.svg
 streamlit/initial_recommender.py
 streamlit/surrogate_models.py
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/simulate_telemetry.py
+tests/test_acquisition.py
 tests/test_constraints_continuous.py
 tests/test_constraints_discrete.py
 tests/test_continuous.py
 tests/test_custom_parameter.py
 tests/test_custom_surrogate.py
 tests/test_deprecations.py
+tests/test_imports.py
 tests/test_input_output.py
 tests/test_iterations.py
 tests/test_meta_recommenders.py
 tests/test_objective.py
 tests/test_searchspace.py
 tests/test_streamlit.py
 tests/test_substance_parameter.py
+tests/test_utils.py
 tests/docs/__init__.py
 tests/docs/test_docs.py
 tests/docs/test_examples.py
 tests/docs/utils.py
 tests/hypothesis_strategies/__init__.py
+tests/hypothesis_strategies/acquisition.py
+tests/hypothesis_strategies/basic.py
+tests/hypothesis_strategies/constraints.py
 tests/hypothesis_strategies/dataframes.py
+tests/hypothesis_strategies/kernels.py
+tests/hypothesis_strategies/objectives.py
 tests/hypothesis_strategies/parameters.py
+tests/hypothesis_strategies/priors.py
 tests/hypothesis_strategies/targets.py
 tests/hypothesis_strategies/utils.py
 tests/hypothesis_strategies/alternative_creation/__init__.py
+tests/hypothesis_strategies/alternative_creation/test_acquisition.py
 tests/hypothesis_strategies/alternative_creation/test_intervals.py
+tests/hypothesis_strategies/alternative_creation/test_kernels.py
 tests/hypothesis_strategies/alternative_creation/test_parameters.py
 tests/hypothesis_strategies/alternative_creation/test_searchspace.py
 tests/hypothesis_strategies/alternative_creation/test_targets.py
 tests/serialization/__init__.py
+tests/serialization/test_acquisition_serialization.py
 tests/serialization/test_campaign_serialization.py
 tests/serialization/test_constraint_serialization.py
 tests/serialization/test_dataframe_serialization.py
+tests/serialization/test_deserialization.py
+tests/serialization/test_kernel_serialization.py
 tests/serialization/test_meta_recommender_serialization.py
 tests/serialization/test_naive_hybrid_serialization.py
 tests/serialization/test_objective_serialization.py
 tests/serialization/test_parameter_serialization.py
+tests/serialization/test_prior_serialization.py
 tests/serialization/test_searchspace_serialization.py
 tests/serialization/test_surrogate_serialization.py
 tests/serialization/test_target_serialization.py
 tests/validation/__init__.py
 tests/validation/test_interval_validation.py
+tests/validation/test_objective_validation.py
 tests/validation/test_parameter_validation.py
 tests/validation/test_target_validation.py
```

### Comparing `baybe-0.8.2/baybe.egg-info/requires.txt` & `baybe-0.9.0/baybe.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 pandas>=1.4.2
 protobuf<=3.20.3
 scikit-learn>=1.1.1
 scikit-learn-extra>=0.3.0
 scipy>=1.10.1
 setuptools-scm>=7.1.0
 torch>=1.13.1
+typing_extensions>=4.7.0
 opentelemetry-sdk>=1.16.0
 opentelemetry-propagator-aws-xray>=1.0.0
 opentelemetry-exporter-otlp>=1.16.0
 opentelemetry-sdk-extension-aws>=2.0.0
-requests>=2.31.0
-urllib3>=2.0.7
 
 [chem]
 rdkit>=2022.3.4
 mordredcommunity>=1.2.0
 
 [dev]
 baybe[chem]
@@ -30,15 +29,15 @@
 baybe[examples]
 baybe[lint]
 baybe[mypy]
 baybe[onnx]
 baybe[simulation]
 baybe[test]
 pip-audit>=2.5.5
-tox>=4.10.0
+tox-uv>=1.7.0
 
 [docs]
 baybe[examples]
 furo>=2023.09.10
 jupyter>=1.0.0
 jupytext>=1.16.1
 myst-parser>=2.0.0
@@ -65,15 +64,14 @@
 ruff==0.1.6
 typos==1.16.23
 
 [mypy]
 mypy>=1.6.1
 pandas-stubs>=2.0.3.230814
 funcy-stubs>=0.1.1
-types-requests>=2.31.0.20240106
 types-seaborn>=0.12.2
 
 [onnx]
 onnx>=1.16.0
 onnxruntime>=1.15.1
 skl2onnx>=1.15.0
```

### Comparing `baybe-0.8.2/docs/_static/banner1.svg` & `baybe-0.9.0/docs/_static/banner1.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/_static/banner2.svg` & `baybe-0.9.0/docs/_static/banner2.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/_static/favicon.ico` & `baybe-0.9.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/_static/logo1.svg` & `baybe-0.9.0/docs/_static/logo1.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/_static/logo2.svg` & `baybe-0.9.0/docs/_static/logo2.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/_static/target_transforms.svg` & `baybe-0.9.0/docs/_static/target_transforms.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/conf.py` & `baybe-0.9.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import os
 import shutil
-import sys
-
-# We need to "trick" sphinx due to it thinking that decorated classes are just aliases
-# We thus need to import and later define some specific names
-from baybe.surrogates import get_available_surrogates
 
 # -- Path setup --------------------------------------------------------------
 
 __location__ = os.path.dirname(__file__)
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
@@ -107,15 +102,14 @@
 # ignore.
 nitpick_ignore_regex = [
     # Ignore everything that does not include baybe
     (r"py:.*", r"^(?!.*baybe).*"),
     # Ignore errors that are from inherited classes we cannot control
     (r"py:.*", r".*DTypeFloatNumpy.*"),
     (r"py:.*", r".*DTypeFloatONNX.*"),
-    (r"py:.*", r".*AdapterModel.*"),
     # Ignore the functions that we manually delete from in child classes
     (r"py:.*", r".*from_dict.*"),
     (r"py:.*", r".*from_json.*"),
     (r"py:.*", r".*to_dict.*"),
     (r"py:.*", r".*to_json.*"),
     (r"py:.*", r".*_T.*"),
     # Ignore files for which no __init__ is available at all
@@ -124,14 +118,16 @@
     (r"DeprecationWarning:", ""),
     # Ignore the generics in utils.basic
     # Might be able to us a regex here, is done explicitly at the moment for full
     # transparency.
     (r"py:class", "baybe.utils.basic._C"),
     (r"py:class", "baybe.utils.basic._T"),
     (r"py:class", "baybe.utils.basic._U"),
+    # Ignore custom class properties
+    (r"py:obj", "baybe.acquisition.acqfs.*.is_mc"),
 ]
 
 
 # Ignore the warnings that are given by autosectionlabel
 suppress_warnings = ["autosectionlabel.*"]
 
 # -- Options for HTML output -------------------------------------------------
@@ -249,48 +245,39 @@
     "torch": ("https://pytorch.org/docs/master/", None),
     "rdkit": ("https://rdkit.org/docs/", None),
 }
 
 # --- Options for autodoc typehints and autodoc -------------------------------
 # https://pypi.org/project/sphinx-autodoc-typehints/
 
-# For some reason, sphinx does not like it if we use the -D option to just tell it
-# that we want to include private members. We thus manually verify whether the option
-# was set.
-private_members = "True" in sys.argv[sys.argv.index("-D") + 1]
-
 # Represent typehints whenever possible.
 autodoc_typehints = "both"
 # Separate class names and init functions.
 autodoc_class_signature = "separated"
 # Do not preserve the defaults as we want them to be evaluated due to attrs
 # Seems to be bugged for attrs defaults, see
 # https://github.com/sphinx-toolbox/sphinx-toolbox/issues/146
 autodoc_preserve_defaults = False
 # Set the default options that should be used for autodoc
 autodoc_default_options = {
     # Order by type (function, attribute...), required for proper inheritance
     "member-order": "groupwise",
-    # Include private members if this was requested
-    "private-members": private_members,
 }
 # Only show parameters that are documented.
 autodoc_typehints_description_target = "documented_params"
 # Shorten the links in the function signatures
 autodoc_typehints_format = "short"
 python_use_unqualified_type_names = True
 # Typehints should be shown in the signature
 typehints_use_signature = True
 
 
 # This function enables us to hook into the internal sphinx processes
-# These allow us to change docstrings (resp. how they are processed) which is currently
-# necessary for properly rendering the surrogates
+# These allow us to change docstrings (resp. how they are processed)
 def setup(app):  # noqa: D103
-    get_available_surrogates()
     app.connect("autodoc-process-docstring", autodoc_process_docstring)
 
 
 def autodoc_process_docstring(app, what, name, obj, options, lines):
     """Process the docstrings that sphinx creates."""
     if "__init__" in name and len(lines) > 0:
         lines.append(
```

### Comparing `baybe-0.8.2/docs/index.md` & `baybe-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/known_issues.md` & `baybe-0.9.0/docs/known_issues.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/scripts/convert_code_to_documentation.py` & `baybe-0.9.0/docs/scripts/convert_code_to_documentation.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,29 +8,14 @@
 
 from utils import adjust_pictures, create_example_documentation
 
 from baybe.telemetry import VARNAME_TELEMETRY_ENABLED
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
-    "-t",
-    "--target_dir",
-    help="Destination directory in which the build will be saved (relative).\
-    Note that building the documentation actually happens within the doc folder.\
-    After building the documentation, it will be copied to this folder.\
-    Default is a subfolder 'docs' placed in `build`.",
-    default="./build/docs",
-)
-parser.add_argument(
-    "-p",
-    "--include_private",
-    help="Include private methods in the documentation. Default is false.",
-    action="store_true",
-)
-parser.add_argument(
     "-e",
     "--ignore_examples",
     help="Ignore the examples and do not include them into the documentation.",
     action="store_true",
 )
 parser.add_argument(
     "-w",
@@ -44,58 +29,42 @@
     help="Force-build the documentation, even when there are warnings or errors.",
     action="store_true",
 )
 
 
 # Parse input arguments
 args = parser.parse_args()
-DESTINATION_DIR = args.target_dir
-INCLUDE_PRIVATE = args.include_private
 IGNORE_EXAMPLES = args.ignore_examples
 INCLUDE_WARNINGS = args.include_warnings
 FORCE = args.force
 
 # We adjust the environment variable if we decide to ignore warnings
 if not INCLUDE_WARNINGS:
     os.environ["PYTHONWARNINGS"] = "ignore"
 
 # Disable telemtetry
 os.environ[VARNAME_TELEMETRY_ENABLED] = "false"
-# Directories where Sphinx will always put the build, sdk and autosummary data
+# Directory where Sphinx builds the documentation
 build_dir = pathlib.Path("docs/build")
-sdk_dir = pathlib.Path("docs/sdk")
-autosummary_dir = pathlib.Path("docs/_autosummary")
-destination_dir = pathlib.Path(DESTINATION_DIR)
-
-# Collect all of the directories and delete them if they still exist.
-directories = [sdk_dir, autosummary_dir, build_dir, destination_dir]
-
-for directory in directories:
-    if directory.is_dir():
-        shutil.rmtree(directory)
 
 # The call for checking external links.
 link_call = [
     "sphinx-build",
     "-b",
     "linkcheck",
     "docs",
     build_dir,
-    "-D",
-    f"autodoc_default_options.private_members={INCLUDE_PRIVATE}",
 ]
 # The actual call that will be made to build the documentation
 building_call = [
     "sphinx-build",
     "-b",
     "html",
     "docs",
     build_dir,
-    "-D",
-    f"autodoc_default_options.private_members={INCLUDE_PRIVATE}",
     "-n",  # Being nitpicky
     "-W",  # Fail when encountering an error or a warning
 ]
 
 # Process examples if required.
 # Note that ignoring of examples now happens by simply not executing them.
 create_example_documentation(
@@ -125,19 +94,11 @@
     "docs/build/index.html",
     match="full_lookup",
     light_version="full_lookup_light",
     dark_version="full_lookup_dark",
 )
 
 
-# Clean the other files
-for directory in [sdk_dir, autosummary_dir]:
-    if directory.is_dir():
-        shutil.rmtree(directory)
-
-documentation = pathlib.Path(build_dir)
-shutil.move(documentation, destination_dir)
-
 # Delete the created markdown files of the examples.
 example_directory = pathlib.Path("docs/examples")
 if example_directory.is_dir():
     shutil.rmtree(example_directory)
```

### Comparing `baybe-0.8.2/docs/scripts/utils.py` & `baybe-0.9.0/docs/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/templates/custom-class-template.rst` & `baybe-0.9.0/docs/templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/templates/custom-module-template.rst` & `baybe-0.9.0/docs/templates/custom-module-template.rst`

 * *Files 8% similar despite different names*

```diff
@@ -57,13 +57,13 @@
 .. rubric:: Modules
 
 .. autosummary::
    :toctree:
    :template: custom-module-template.rst
    :recursive:
 {% for item in modules %}
-{% if not item in ("baybe.deprecation", "baybe.surrogate", "baybe.strategies.deprecation", "baybe.targets.deprecation") %}
+{% if not item in ("baybe.deprecation", "baybe.strategies.deprecation", "baybe.objectives.deprecation") %}
    {{ item }}
 {%- endif %}
 {%- endfor %}
 {% endif %}
 {% endblock %}
```

### Comparing `baybe-0.8.2/docs/userguide/campaigns.md` & `baybe-0.9.0/docs/userguide/campaigns.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ### Basic creation
 
 Creating a campaign requires specifying at least two pieces of information that
 describe the underlying optimization problem at hand:
 
 | Campaign Specification                     | BayBE Class                                                                               |
 |:-------------------------------------------|:------------------------------------------------------------------------------------------|
-| What should be optimized in the campaign?  | `Objective` ([class](baybe.objective.Objective) / [user guide](./objective))              |
+| What should be optimized in the campaign?  | `Objective` ([class](baybe.objectives.base.Objective) / [user guide](./objectives))              |
 | Which experimental factors can be altered? | `SearchSpace` ([class](baybe.searchspace.core.SearchSpace) / [user guide](./searchspace)) |
 
 Apart from this basic configuration, it is possible to further define the specific
 optimization 
 `Recommender`&nbsp;([class](baybe.recommenders.pure.base.PureRecommender) 
 / [user guide](./recommenders)) to be used.
 
@@ -158,39 +158,40 @@
 This requirement can be disabled using the method's
 `numerical_measurements_must_be_within_tolerance` flag.
 ```
 
 
 ## Serialization
 
-Like most of the objects managed by BayBE, `Campaign` objects can be serialized and
-deserialized using the [`to_json`](baybe.serialization.mixin.SerialMixin.to_json) and
-[`from_json`](baybe.serialization.mixin.SerialMixin.from_json) methods, which 
-allow to convert between Python objects their corresponding representation in JSON 
-format. 
-These representations are fully equivalent, meaning that serializing and subsequently 
-deserializing a campaign yields an exact copy of the object:
-
+Like other BayBE objects, [`Campaigns`](baybe.campaign.Campaign) can be de-/serialized 
+using their [`from_json`](baybe.serialization.mixin.SerialMixin.from_json)/
+[`to_json`](baybe.serialization.mixin.SerialMixin.to_json) methods, which 
+allow to convert between Python objects and their corresponding representation in JSON 
+format:
 ~~~python
 campaign_json = campaign.to_json()
-recreated_campaign = Campaign.from_json(campaign_json)
-assert campaign == recreated_campaign
+reconstructed = Campaign.from_json(campaign_json)
+assert campaign == reconstructed
 ~~~
 
-This provides an easy way to persist the current state of your campaign for long 
-term storage and continue the experimentation at a later point in time.
-For more information on serialization, we
-refer to the corresponding [examples](./../../examples/Serialization/Serialization).
-
-```{admonition} Dataframe serialization
-:class: note
-Note that `DataFrame` objects associated with the `Campaign` object are converted to 
-a binary format during serialization, which has the consequence that their JSON 
-representation is not human-readable.
-```
+General information on this topic can be found in our 
+[serialization user guide](/userguide/serialization).
+For campaigns, however, this possibility is particularly noteworthy as it enables
+one of the most common workflows in this context –
+persisting the current state of a campaign for long-term storage and continuing the
+experimentation at a later point in time:
+
+1. Get your campaign object
+    * When initiating the workflow, create a new campaign object
+    * When coming from the last step below, **deserialize** the existing campaign object
+2. Add the latest measurement results
+3. Get a recommendation
+4. **Serialize** the campaign and store it somewhere
+5. Run your (potentially lengthy) real-world experiments
+6. Repeat
 
 ## Further information
 
 Campaigns are created as a first step in most of our 
 [examples](./../../examples/examples).
 For more details on how to define campaigns for a specific use case, we thus propose 
 to have a look at the most suitable example.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `baybe-0.8.2/docs/userguide/constraints.md` & `baybe-0.9.0/docs/userguide/constraints.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/userguide/objective.md` & `baybe-0.9.0/docs/userguide/objectives.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,104 @@
 # Objective
 
-The [`Objective`](baybe.objective.Objective) instructs BayBE how to deal with multiple
-targets (if applicable).
-
-To create an objective, it is necessary to provide the following:
-* An optimization `mode`: This can be either `SINGLE` or `DESIRABILITY`,
-  denoting the optimization of a single target function or a combination of
-  different target functions respectively.
-* A list of `targets`: The list of targets that are optimized (see user guide for
-  [`Target`](../../userguide/targets)). Note that the `SINGLE` mode also requires a
-  list containing the single target.
+Optimization problems involve either a single target quantity of interest or 
+several (potentially conflicting) targets that need to be considered simultaneously.  
+BayBE uses the concept of an [`Objective`](baybe.objective.Objective) to allow the user
+to control how these different types of scenarios are handled.
 
 ```{note}
-We are actively working on adding more objective modes for multiple targets.
+We are actively working on adding more objective types for multiple targets.
 ```
 
-## Supported Optimization Modes
-Currently, BayBE offers two optimization modes.
-
-### SINGLE
-In `SINGLE` mode, objectives focus on optimizing a single target. 
-Nearly [examples](../../examples/examples) use this objective mode.
-
+## SingleTargetObjective
+The need to optimize a single [`Target`](baybe.targets.base.Target) is the most basic
+type of situation one can encounter in experimental design. 
+In this scenario, the fact that only one target shall be considered in the design is
+communicated to BayBE by wrapping the target into a
+[`SingleTargetObjective`](baybe.objectives.single.SingleTargetObjective):
 ```python
 from baybe.targets import NumericalTarget
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
+
+target = NumericalTarget(name="Yield", mode="MAX")
+objective = SingleTargetObjective(target)
+```
+In fact, the role of the
+`SingleTargetObjective` is to merely signal the absence of other `Target`s in the
+optimization problem.
+Because this fairly trivial conversion step requires no additional user configuration,
+we provide a convenience constructor for it:
+
+````{admonition} Convenience construction and implicit conversion
+:class: tip
+* The conversion from a single [`Target`](baybe.targets.base.Target) to a
+[`SingleTargetObjective`](baybe.objectives.single.SingleTargetObjective) describes a
+one-to-one relationship and can be triggered directly from the corresponding target
+object:
+  ```python
+  objective = target.to_objective()
+  ```
+* Also, other class constructors that expect an 
+[`Objective`](baybe.objectives.base.Objective)
+object (such as [`Campaigns`](baybe.campaign.Campaign)) will happily accept
+individual [`Targets`](baybe.targets.base.Target) instead and apply the necessary
+conversion behind the scenes.
+````
+
+## DesirabilityObjective
+The [`DesirabilityObjective`](baybe.objectives.desirability.DesirabilityObjective)
+enables the combination of multiple targets via scalarization into a single numerical
+value (commonly referred to as the *overall desirability*), a method also utilized in
+classical DOE.
 
-target_1 = NumericalTarget(name="yield", mode="MIN", bounds=(0, 100))
-objective = Objective(mode="SINGLE", targets=[target_1])
+```{admonition} Mandatory target bounds
+:class: attention
+Since measurements of different targets can vary arbitrarily in scale, all targets
+passed to a
+[`DesirabilityObjective`](baybe.objectives.desirability.DesirabilityObjective) must be
+normalizable to enable meaningful combination into desirability values. This requires
+that all provided targets must have `bounds` specified (see [target user
+guide](/userguide/targets.md)).
+If provided, the necessary normalization is taken care of automatically. 
+Otherwise, an error will be thrown.
 ```
 
-### DESIRABILITY
-The `DESIRABILITY` mode enables the combination multiple targets via scalarization 
-into a single value, a method also utilized in classical DOE.
-
-Besides `mode` and `targets`, this objective type takes two additional optional
-arguments:
-* `weights`: Some targets might be more important than others.
-  It is possible to specify the relative weights of the targets in this argument.
-  BayBE automatically normalizes the numbers provided, so only their relative values 
-  matter.
-* `combine_func`: Specifies the function used for combining the transformed targets. 
+Besides the list of `targets` to be scalarized, this objective type takes two
+additional optional parameters that let us control its behavior:
+* `weights`: Specifies the relative importance of the targets in the form of a
+  sequence of positive numbers, one for each target considered.  
+  **Note:** 
+  BayBE automatically normalizes the weights, so only their relative
+  scales matter.
+* `scalarizer`: Specifies the [scalarization function](baybe.objectives.enum.Scalarizer)
+  to be used for combining the normalized target values. 
   The choices are `MEAN` and `GEOM_MEAN`, referring to the arithmetic and 
-  geometric mean respectively.
+  geometric mean, respectively.
 
-The definitions of the means are as follows, where $\{t_i\}$ enumerate the **scaled**
-target observations for a single measurement and $\{w_i\}$ are the weights associated
-with the respective target:
+The definitions of the `scalarizer`s are as follows, where $\{t_i\}$ enumerate the
+**normalized** target measurements of single experiment and $\{w_i\}$ are the
+corresponding target weights:
 
 $$
 \text{MEAN} &= \frac{1}{\sum w_i}\sum_{i} w_i \cdot t_i \\
 \text{GEOM_MEAN} &= \left( \prod_i t_i^{w_i} \right)^{1/\sum w_i}
 $$
 
-```{admonition} Mandatory Target Bounds
-:class: attention
-Due to the combination of targets of potentially different scale, in `DESIRABILITY` 
-objective mode, all provided targets must have `bounds` specified so they can be 
-normalized via scaling before being combined.
-```
 
-In the example below, we use three different targets (which all have a different goal) 
-and weigh the first target twice as important as each of the other targets:
+In the example below, we consider three different targets (all associated with a
+different goal) and give twice as much importance to the first target relative to each 
+of the other two:
 ```python
 from baybe.targets import NumericalTarget
-from baybe.objective import Objective
+from baybe.objectives import DesirabilityObjective
 
 target_1 = NumericalTarget(name="t_1", mode="MIN", bounds=(0, 100))
 target_2 = NumericalTarget(name="t_2", mode="MIN", bounds=(0, 100))
 target_3 = NumericalTarget(name="t_3", mode="MATCH", bounds=(40, 60))
-objective = Objective(
-    mode="DESIRABILITY",
+objective = DesirabilityObjective(
     targets=[target_1, target_2, target_3],
-    weights=[2.0, 1.0, 1.0],  # optional, by default all weights are equal
-    combine_func="GEOM_MEAN",  # optional, geometric mean is the default
+    weights=[2.0, 1.0, 1.0],  # optional (by default, all weights are equal)
+    scalarizer="GEOM_MEAN",  # optional
 )
 ```
 
-For a complete example demonstrating desirability mode, see [here](./../../examples/Multi_Target/desirability).
+For a complete example demonstrating desirability mode, see [here](./../../examples/Multi_Target/desirability).
```

### Comparing `baybe-0.8.2/docs/userguide/parameters.md` & `baybe-0.9.0/docs/userguide/parameters.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/userguide/recommenders.md` & `baybe-0.9.0/docs/userguide/recommenders.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/userguide/searchspace.md` & `baybe-0.9.0/docs/userguide/searchspace.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/docs/userguide/simulation.md` & `baybe-0.9.0/docs/userguide/simulation.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 
 ### Using a `Callable`
 
 The `Callable` needs to return the target values for any given parameter combination. The only requirement that BayBE imposes on using a `Callable` as a lookup mechanism is thus that it returns either a float or a tuple of floats and to accept an arbitrary number of floats as input.
 
 ## Simulating a Single Experiment
 
-The function [`simulate_experiment`](baybe.simulation.simulate_experiment) is the most basic form of simulation.
+The function [`simulate_experiment`](baybe.simulation.core.simulate_experiment) is the most basic form of simulation.
 It runs a single execution of a DoE loop for either a specific number of iteration or until the search space is fully observed.
 
 For using this function, it is necessary to provide a [`campaign`](baybe.campaign.Campaign). Although technically not necessary, we advise to also always provide a lookup mechanisms since fake results will be produced if none is provided. It is possible to specify several additional parameters like the batch size, initial data or the number of DoE iterations that should be performed
 
 ~~~python
-results = simulate_scenarios(
+results = simulate_experiment(
     # Necessary
     campaign=campaign,
     # Technically optional but should always be set
     lookup=lookup,
     # Optional
     batch_size=batch_size,
     n_doe_iterations=n_doe_iterations,
@@ -67,15 +67,15 @@
 )
 ~~~
 
 This function returns a dataframe that contains the results. For details on the columns of this dataframe as well as the dataframes returned by the other functions discussed here, we refer to the documentation of the submodule [here](baybe.simulation).
 
 ## Simulating Multiple Scenarios
 
-The function [`simulate_scenarios`](baybe.simulation.simulate_scenarios) allows to specify multiple simulation settings at once.
+The function [`simulate_scenarios`](baybe.simulation.scenarios.simulate_scenarios) allows to specify multiple simulation settings at once.
 Instead of a single campaign, this function expects a dictionary of campaigns, mapping scenario identifiers to `Campaign` objects.
 In addition to the keyword arguments available for `simulate_experiment`, this function has two different keywords available:
 1. `n_mc_iterations`: This can be used to perform multiple Monte Carlo runs with a single call. Multiple Monte Carlo runs are always advised to average out the effect of random effects such as the initial starting data.
 2. `initial_data`: This can be used to provide a list of dataframe, where each dataframe is then used as initial data for an independent run. That is, the function performs one optimization loop per dataframe in this list.
 
 Note that these two keywords are mutually exclusive.
 
@@ -92,18 +92,18 @@
     n_doe_iterations=n_doe_iterations,
     n_mc_iterations=n_mc_iterations,
 )
 ~~~
 
 ## Simulating Transfer Learning
 
-The function [`simulate_transfer_learning`](baybe.simulation.simulate_transfer_learning) partitions the search space into its tasks and simulates each task with the training data from the remaining tasks.
+The function [`simulate_transfer_learning`](baybe.simulation.transfer_learning.simulate_transfer_learning) partitions the search space into its tasks and simulates each task with the training data from the remaining tasks.
 
 ```{note}
-Currently, this only supports discrete search spaces. See [`simulate_transfer_learning`](baybe.simulation.simulate_transfer_learning) for the reasons.
+Currently, this only supports discrete search spaces. See [`simulate_transfer_learning`](baybe.simulation.transfer_learning.simulate_transfer_learning) for the reasons.
 ```
 
 ~~~python
 task_param = TaskParameter(
     name="Cell Line",
     values=["Liver Cell", "Brain Cell", "Skin Cell"],
 )
```

### Comparing `baybe-0.8.2/docs/userguide/surrogates.md` & `baybe-0.9.0/docs/userguide/surrogates.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 Surrogate models are used to model and estimate the unknown objective function of the DoE campaign. BayBE offers a diverse array of surrogate models, while also allowing for the utilization of custom models. All surrogate models are based upon the general [`Surrogate`](baybe.surrogates.base.Surrogate) class. Some models even support transfer learning, as indicated by the `supports_transfer_learning` attribute.
 
 ## Available models
 
 BayBE provides a comprehensive selection of surrogate models, empowering you to choose the most suitable option for your specific needs. The following surrogate models are available within BayBE:
 
-* [`GaussianProcessSurrogate`](baybe.surrogates.gaussian_process.GaussianProcessSurrogate)
-* `BayesianLinearSurrogate`
+* [`GaussianProcessSurrogate`](baybe.surrogates.gaussian_process.core.GaussianProcessSurrogate)
+* [`BayesianLinearSurrogate`](baybe.surrogates.linear.BayesianLinearSurrogate)
 * [`MeanPredictionSurrogate`](baybe.surrogates.naive.MeanPredictionSurrogate)
-* `NGBoostSurrogate`
-* `RandomForestSurrogate`
+* [`NGBoostSurrogate`](baybe.surrogates.ngboost.NGBoostSurrogate)
+* [`RandomForestSurrogate`](baybe.surrogates.random_forest.RandomForestSurrogate)
 
 
 ## Using custom models
 
 BayBE goes one step further by allowing you to incorporate custom models based on the ONNX architecture. Note however that these cannot be retrained.  For a detailed explanation on using custom models, refer to the comprehensive examples provided in the corresponding [example folder](./../../examples/Custom_Surrogates/Custom_Surrogates).
```

### Comparing `baybe-0.8.2/docs/userguide/targets.md` & `baybe-0.9.0/docs/userguide/targets.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Targets
 
 Targets play a crucial role as the connection between observables measured in an
 experiment and the machine learning core behind BayBE.
 In general, it is expected that you create one [`Target`](baybe.targets.base.Target)
 object for each of your observables.
 The way BayBE treats multiple targets is then controlled via the 
-[`Objective`](../../userguide/objective).
+[`Objective`](../../userguide/objectives).
 
 ## NumericalTarget
 Besides the `name`, a [`NumericalTarget`](baybe.targets.numerical.NumericalTarget)
 has the following attributes:
 * **The optimization** `mode`: Specifies whether we want to minimize/maximize
   the target or whether we want to match a specific value.
 * **Bounds**: Defines `bounds` that constrain the range of target values.
```

### Comparing `baybe-0.8.2/docs/userguide/transfer_learning.md` & `baybe-0.9.0/docs/userguide/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/botorch_analytical.py` & `baybe-0.9.0/examples/Backtesting/botorch_analytical.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 
 import numpy as np
 import seaborn as sns
 from botorch.test_functions import Rastrigin
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter
 from baybe.recommenders import RandomRecommender
 from baybe.searchspace import SearchSpace
 from baybe.simulation import simulate_scenarios
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 from baybe.utils.plotting import create_example_plots
@@ -76,17 +76,15 @@
         ),
         tolerance=0.01,
     )
     for k in range(DIMENSION)
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing campaigns
 
 seq_greedy_EI_campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
@@ -94,15 +92,15 @@
     searchspace=searchspace,
     recommender=RandomRecommender(),
     objective=objective,
 )
 
 ### Performing the simulation loop
 
-# We use [simulate_scenarios](baybe.simulation.simulate_scenarios) to simulate a full experiment.
+# We use [simulate_scenarios](baybe.simulation.scenarios.simulate_scenarios) to simulate a full experiment.
 
 scenarios = {
     "Sequential greedy EI": seq_greedy_EI_campaign,
     "Random": random_campaign,
 }
 results = simulate_scenarios(
     scenarios,
```

### Comparing `baybe-0.8.2/examples/Backtesting/botorch_analytical_dark.svg` & `baybe-0.9.0/examples/Backtesting/botorch_analytical_dark.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/botorch_analytical_light.svg` & `baybe-0.9.0/examples/Backtesting/botorch_analytical_light.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/custom_analytical.py` & `baybe-0.9.0/examples/Backtesting/custom_analytical.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter
 from baybe.recommenders import (
     RandomRecommender,
     SequentialGreedyRecommender,
     TwoPhaseMetaRecommender,
 )
 from baybe.searchspace import SearchSpace
@@ -70,25 +70,23 @@
         values=list(np.linspace(*BOUNDS[k], POINTS_PER_DIM)),
         tolerance=0.01,
     )
     for k in range(DIMENSION)
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing campaigns for the simulation loop
 
 # To simplify adjusting the example for other recommenders, we construct some recommender objects.
 # For details on recommender objects, we refer to [`recommenders`](./../Basics/recommenders.md).
 
 seq_greedy_EI_recommender = TwoPhaseMetaRecommender(
-    recommender=SequentialGreedyRecommender(acquisition_function_cls="qEI"),
+    recommender=SequentialGreedyRecommender(acquisition_function="qEI"),
 )
 random_recommender = TwoPhaseMetaRecommender(recommender=RandomRecommender())
 
 # We now create one campaign per recommender.
 
 seq_greedy_EI_campaign = Campaign(
     searchspace=searchspace,
```

### Comparing `baybe-0.8.2/examples/Backtesting/full_initial_data.py` & `baybe-0.9.0/examples/Backtesting/full_initial_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, SubstanceParameter
 from baybe.recommenders import RandomRecommender, TwoPhaseMetaRecommender
 from baybe.searchspace import SearchSpace
 from baybe.simulation import simulate_scenarios
 from baybe.targets import NumericalTarget
 
 ### Parameters for a full simulation loop
@@ -100,17 +100,15 @@
 concentration = NumericalDiscreteParameter(
     name="Concentration", values=[0.057, 0.1, 0.153], tolerance=0.005
 )
 
 parameters = [solvent, base, ligand, temperature, concentration]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="yield", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="yield", mode="MAX"))
 
 ### Constructing campaigns for the simulation loop
 
 # In this example, we create two campaigns.
 # One uses the default recommender and the other one makes random recommendations.
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
```

### Comparing `baybe-0.8.2/examples/Backtesting/full_lookup.py` & `baybe-0.9.0/examples/Backtesting/full_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 from pathlib import Path
 
 import pandas as pd
 import seaborn as sns
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.recommenders import RandomRecommender
 from baybe.searchspace import SearchSpace
@@ -86,17 +86,15 @@
     r"C4=CC(C(F)(F)F)=CC(C(F)(F)F)=C4)=CC(C(F)(F)F)=C1",
     "SCHEMBL15068049": r"C[C@]1(O2)O[C@](C[C@]2(C)P3C4=CC=CC=C4)(C)O[C@]3(C)C1",
     "Me2PPh": r"CP(C)C1=CC=CC=C1",
 }
 
 ### Creating the Objective
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="yield", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="yield", mode="MAX"))
 
 ### Constructing campaigns for the simulation loop
 
 # In this example, we create several campaigns.
 # First let us create three campaigns that each use a different chemical encoding to
 # treat substances.
```

### Comparing `baybe-0.8.2/examples/Backtesting/full_lookup_dark.svg` & `baybe-0.9.0/examples/Backtesting/full_lookup_dark.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/full_lookup_light.svg` & `baybe-0.9.0/examples/Backtesting/full_lookup_light.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/hybrid.py` & `baybe-0.9.0/examples/Backtesting/hybrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalContinuousParameter, NumericalDiscreteParameter
 from baybe.recommenders import (
     NaiveHybridSpaceRecommender,
     RandomRecommender,
     SequentialGreedyRecommender,
     TwoPhaseMetaRecommender,
 )
@@ -103,17 +103,15 @@
 
 # Concatenate the continuous and discrete parameters.
 
 parameters = cont_parameters + disc_parameters
 
 # Construct searchspace and objective.
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing campaigns for the simulation loop
 
 # This example compares three different available hybrid recommenders:
 # The `SequentialGreedyRecommender`, the `NaiveHybridSpaceRecommender` and the `RandomRecommender`.
 # For each of them, we initialize one recommender object.
 # Note that it is possible to further specify the behavior of the `SequentialGreedyRecommender`.
```

### Comparing `baybe-0.8.2/examples/Backtesting/impute_mode.py` & `baybe-0.9.0/examples/Backtesting/impute_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, SubstanceParameter
 from baybe.recommenders import RandomRecommender, TwoPhaseMetaRecommender
 from baybe.searchspace import SearchSpace
 from baybe.simulation import simulate_scenarios
 from baybe.targets import NumericalTarget
 
 ### Parameters for a full simulation loop
@@ -91,17 +91,15 @@
 concentration = NumericalDiscreteParameter(
     name="Concentration", values=[0.057, 0.1, 0.153], tolerance=0.005
 )
 
 parameters = [solvent, base, ligand, temperature, concentration]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="yield", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="yield", mode="MAX"))
 
 ### Constructing campaigns for the simulation loop
 
 # In this example, we create two campaigns.
 # One uses the default recommender and the other one makes random recommendations.
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
```

### Comparing `baybe-0.8.2/examples/Backtesting/lookup.xlsx` & `baybe-0.9.0/examples/Backtesting/lookup.xlsx`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/lookup_withmissing.xlsx` & `baybe-0.9.0/examples/Backtesting/lookup_withmissing.xlsx`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Backtesting/multi_target.py` & `baybe-0.9.0/examples/Backtesting/multi_target.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### Necessary imports for this example
 
 import os
 
 import numpy as np
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import DesirabilityObjective
 from baybe.parameters import NumericalDiscreteParameter
 from baybe.searchspace import SearchSpace
 from baybe.simulation import simulate_scenarios
 from baybe.targets import NumericalTarget
 
 ### Parameters for a full simulation loop
 
@@ -83,19 +83,18 @@
 
 ### Creating the objective object
 
 # We collect the two targets in a list and use this list to construct the objective.
 
 targets = [Target_1, Target_2]
 
-objective = Objective(
-    mode="DESIRABILITY",
+objective = DesirabilityObjective(
     targets=targets,
     weights=[20, 30],
-    combine_func="MEAN",
+    scalarizer="MEAN",
 )
 
 
 ### Constructing a campaign and performing the simulation loop
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
```

### Comparing `baybe-0.8.2/examples/Basics/campaign.py` & `baybe-0.9.0/examples/Basics/campaign.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This example shows how to create a campaign and how to use it.
 # It is intended to be used as a first point of interaction with campaign after having
 # read the corresponding [user guide](./../../userguide/campaigns).
 
 ### Necessary imports for this example
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, SubstanceParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.dataframe import add_fake_results
 
 ### Setup
 
@@ -58,17 +58,15 @@
 parameters = [solvent, base, ligand, temperature, concentration]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
 
 # In this example, we maximize the yield of a reaction and define a corresponding
 # objective.
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="yield", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="yield", mode="MAX"))
 
 # We now finally create the campaign using the objects configure previously.
 
 campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
```

### Comparing `baybe-0.8.2/examples/Basics/recommenders.py` & `baybe-0.9.0/examples/Basics/recommenders.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,26 @@
 
 # This examples assumes some basic familiarity with using BayBE.
 # We refer to [`campaign`](./campaign.md) for a more general and basic example.
 
 ### Necessary imports for this example
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, SubstanceParameter
 from baybe.recommenders import (
     RandomRecommender,
     SequentialGreedyRecommender,
     TwoPhaseMetaRecommender,
 )
 from baybe.searchspace import SearchSpace
-from baybe.surrogates import (
-    BayesianLinearSurrogate,
-    GaussianProcessSurrogate,
-    NGBoostSurrogate,
-    RandomForestSurrogate,
-)
+from baybe.surrogates import GaussianProcessSurrogate
+from baybe.surrogates.base import Surrogate
 from baybe.targets import NumericalTarget
+from baybe.utils.basic import get_subclasses
 from baybe.utils.dataframe import add_fake_results
 
 ### Available recommenders suitable for initial recommendation
 
 # For the first recommendation, the user can specify which recommender to use.
 # The following initial recommenders are available.
 # Note that it is necessary to make the corresponding import before using them.
@@ -51,25 +48,19 @@
 INITIAL_RECOMMENDER = RandomRecommender()
 
 ### Available surrogate models
 
 # This model uses available data to model the objective function as well as the uncertainty.
 # The surrogate model is then used by the acquisition function to make recommendations.
 
-# The following are some available basic surrogates
-# Use `baybe.surrogates.get_available_surrogates()` for a complete list.
-
-available_surrogate_models = [
-    GaussianProcessSurrogate(),
-    RandomForestSurrogate(),
-    NGBoostSurrogate(),
-    BayesianLinearSurrogate(),
-]
+# The following are the available basic surrogates
+print(get_subclasses(Surrogate))
 
 # Per default a Gaussian Process is used
+# You can change the used kernel by using the optional `kernel` keyword.
 
 SURROGATE_MODEL = GaussianProcessSurrogate()
 
 
 ### Acquisition function
 
 # This function looks for points where measurements of the target value could improve the model.
@@ -110,15 +101,15 @@
 # Note that they all have default values.
 # Therefore one does not need to specify all of them to create a recommender object.
 
 recommender = TwoPhaseMetaRecommender(
     initial_recommender=INITIAL_RECOMMENDER,
     recommender=SequentialGreedyRecommender(
         surrogate_model=SURROGATE_MODEL,
-        acquisition_function_cls=ACQ_FUNCTION,
+        acquisition_function=ACQ_FUNCTION,
         allow_repeated_recommendations=ALLOW_REPEATED_RECOMMENDATIONS,
         allow_recommending_already_measured=ALLOW_RECOMMENDING_ALREADY_MEASURED,
     ),
 )
 
 print(recommender)
 
@@ -163,17 +154,15 @@
 
 parameters = [solvent, base, ligand, temperature, concentration]
 
 # We create the searchspace and the objective.
 
 searchspace = SearchSpace.from_product(parameters=parameters)
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="yield", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="yield", mode="MAX"))
 
 ### Creating the campaign
 
 # The recommender object can now be used together with the searchspace and the objective as follows.
 
 campaign = Campaign(
     searchspace=searchspace,
```

### Comparing `baybe-0.8.2/examples/Constraints_Continuous/hybrid_space.py` & `baybe-0.9.0/examples/Constraints_Continuous/hybrid_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from baybe import Campaign
 from baybe.constraints import (
     ContinuousLinearEqualityConstraint,
     DiscreteSumConstraint,
     ThresholdCondition,
 )
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalContinuousParameter, NumericalDiscreteParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 
 ### Defining the test function
 
@@ -86,17 +86,15 @@
     ),
     ContinuousLinearEqualityConstraint(
         parameters=["x_3", "x_4"], coefficients=[1.0, -1.0], rhs=2.0
     ),
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters, constraints=constraints)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Construct the campaign and run some iterations
 
 campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
```

### Comparing `baybe-0.8.2/examples/Constraints_Continuous/linear_constraints.py` & `baybe-0.9.0/examples/Constraints_Continuous/linear_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from botorch.test_functions import Rastrigin
 
 from baybe import Campaign
 from baybe.constraints import (
     ContinuousLinearEqualityConstraint,
     ContinuousLinearInequalityConstraint,
 )
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalContinuousParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 
 ### Defining the test function
 
@@ -75,17 +75,15 @@
     ),
     ContinuousLinearInequalityConstraint(
         parameters=["x_2", "x_4"], coefficients=[-2.0, -3.0], rhs=-1.0
     ),
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters, constraints=constraints)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Construct the campaign and run some iterations
 
 campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
```

### Comparing `baybe-0.8.2/examples/Constraints_Discrete/custom_constraints.py` & `baybe-0.9.0/examples/Constraints_Discrete/custom_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 
 import numpy as np
 import pandas as pd
 
 from baybe import Campaign
 from baybe.constraints import DiscreteCustomConstraint
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
@@ -98,17 +98,15 @@
     parameters=["Concentration", "Solvent", "Temperature"], validator=custom_function
 )
 
 ### Creating the searchspace and the objective
 
 searchspace = SearchSpace.from_product(parameters=parameters, constraints=[constraint])
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="yield", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="yield", mode="MAX"))
 
 ### Creating and printing the campaign
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
 print(campaign)
 
 ### Manual verification of the constraint
```

### Comparing `baybe-0.8.2/examples/Constraints_Discrete/dependency_constraints.py` & `baybe-0.9.0/examples/Constraints_Discrete/dependency_constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import os
 
 import numpy as np
 
 from baybe import Campaign
 from baybe.constraints import DiscreteDependenciesConstraint, SubSelectionCondition
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
@@ -60,17 +60,15 @@
     affected_parameters=[["Solv", "Frac1"], ["FrameA", "FrameB"]],
 )
 
 ### Creating the searchspace and the objective
 
 searchspace = SearchSpace.from_product(parameters=parameters, constraints=[constraint])
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target_1", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target_1", mode="MAX"))
 
 ### Creating and printing the campaign
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
 print(campaign)
 
 ### Manual verification of the constraints
```

### Comparing `baybe-0.8.2/examples/Constraints_Discrete/exclusion_constraints.py` & `baybe-0.9.0/examples/Constraints_Discrete/exclusion_constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from baybe import Campaign
 from baybe.constraints import (
     DiscreteExcludeConstraint,
     SubSelectionCondition,
     ThresholdCondition,
 )
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
@@ -97,17 +97,15 @@
 
 # We now create the searchspace using the previously defined constraints.
 
 searchspace = SearchSpace.from_product(
     parameters=parameters, constraints=[constraint_1, constraint_2, constraint_3]
 )
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target_1", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target_1", mode="MAX"))
 
 ### Creating and printing the campaign
 campaign = Campaign(searchspace=searchspace, objective=objective)
 print(campaign)
 
 
 ### Manual verification of the constraints
```

### Comparing `baybe-0.8.2/examples/Constraints_Discrete/mixture_constraints.py` & `baybe-0.9.0/examples/Constraints_Discrete/mixture_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from baybe.constraints import (
     DiscreteDependenciesConstraint,
     DiscreteNoLabelDuplicatesConstraint,
     DiscretePermutationInvarianceConstraint,
     DiscreteSumConstraint,
     ThresholdCondition,
 )
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, SubstanceParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.dataframe import add_fake_results
 
 ### Experiment setup
 
@@ -102,17 +102,15 @@
 
 constraints = [perm_inv_constraint, sum_constraint, no_duplicates_constraint]
 
 ### Creating the searchspace and the objective
 
 searchspace = SearchSpace.from_product(parameters=parameters, constraints=constraints)
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target_1", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target_1", mode="MAX"))
 
 ### Creating and printing the campaign
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
 print(campaign)
 
 ### Manual verification of the constraint
```

### Comparing `baybe-0.8.2/examples/Constraints_Discrete/prodsum_constraints.py` & `baybe-0.9.0/examples/Constraints_Discrete/prodsum_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from baybe import Campaign
 from baybe.constraints import (
     DiscreteProductConstraint,
     DiscreteSumConstraint,
     ThresholdCondition,
 )
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
@@ -92,17 +92,15 @@
 
 constraints = [sum_constraint_1, sum_constraint_2, prod_constraint]
 
 ### Creating the searchspace and the objective
 
 searchspace = SearchSpace.from_product(parameters=parameters, constraints=constraints)
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target_1", mode="MAX")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target_1", mode="MAX"))
 
 ### Creating and printing the campaign
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
 print(campaign)
 
 ### Manual verification of the constraints
```

### Comparing `baybe-0.8.2/examples/Custom_Surrogates/custom_architecture_sklearn.py` & `baybe-0.9.0/examples/Custom_Surrogates/custom_architecture_sklearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     RandomForestRegressor,
     StackingRegressor,
 )
 from sklearn.linear_model import LinearRegression, Ridge
 from torch import Tensor
 
 from baybe.campaign import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.recommenders import (
     FPSRecommender,
@@ -129,17 +129,15 @@
 
 
 ### Run DOE iterations with custom surrogate
 # Create campaign
 
 campaign = Campaign(
     searchspace=SearchSpace.from_product(parameters=parameters, constraints=None),
-    objective=Objective(
-        mode="SINGLE", targets=[NumericalTarget(name="Yield", mode="MAX")]
-    ),
+    objective=SingleTargetObjective(target=NumericalTarget(name="Yield", mode="MAX")),
     recommender=TwoPhaseMetaRecommender(
         recommender=SequentialGreedyRecommender(
             surrogate_model=StackingRegressorSurrogate()
         ),
         initial_recommender=FPSRecommender(),
     ),
 )
```

### Comparing `baybe-0.8.2/examples/Custom_Surrogates/custom_architecture_torch.py` & `baybe-0.9.0/examples/Custom_Surrogates/custom_architecture_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Optional
 
 import numpy as np
 import torch
 from torch import Tensor, nn
 
 from baybe.campaign import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.recommenders import (
     FPSRecommender,
@@ -185,17 +185,15 @@
 
 
 ### Run DOE iterations with custom surrogate
 # Create campaign
 
 campaign = Campaign(
     searchspace=SearchSpace.from_product(parameters=parameters, constraints=None),
-    objective=Objective(
-        mode="SINGLE", targets=[NumericalTarget(name="Yield", mode="MAX")]
-    ),
+    objective=SingleTargetObjective(target=NumericalTarget(name="Yield", mode="MAX")),
     recommender=TwoPhaseMetaRecommender(
         recommender=SequentialGreedyRecommender(
             surrogate_model=NeuralNetDropoutSurrogate()
         ),
         initial_recommender=FPSRecommender(),
     ),
 )
```

### Comparing `baybe-0.8.2/examples/Custom_Surrogates/custom_pretrained.py` & `baybe-0.9.0/examples/Custom_Surrogates/custom_pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import torch
 from skl2onnx import convert_sklearn
 from skl2onnx.common.data_types import FloatTensorType
 from skl2onnx.operator_converters.linear_regressor import convert_sklearn_bayesian_ridge
 from sklearn.linear_model import BayesianRidge
 
 from baybe.campaign import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter
 from baybe.recommenders import (
     FPSRecommender,
     SequentialGreedyRecommender,
     TwoPhaseMetaRecommender,
 )
 from baybe.searchspace import SearchSpace
@@ -96,17 +96,15 @@
     onnx_input_name=ONNX_INPUT_NAME,  # specify input name
 )
 
 ### Create campaign
 
 campaign = Campaign(
     searchspace=SearchSpace.from_product(parameters=parameters, constraints=None),
-    objective=Objective(
-        mode="SINGLE", targets=[NumericalTarget(name="Yield", mode="MAX")]
-    ),
+    objective=SingleTargetObjective(target=NumericalTarget(name="Yield", mode="MAX")),
     recommender=TwoPhaseMetaRecommender(
         recommender=SequentialGreedyRecommender(surrogate_model=surrogate_model),
         initial_recommender=FPSRecommender(),
     ),
 )
 
 ### Iterate with recommendations and measurements
```

### Comparing `baybe-0.8.2/examples/Custom_Surrogates/surrogate_params.py` & `baybe-0.9.0/examples/Custom_Surrogates/surrogate_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # We thus refer to [`campaign`](./../Basics/campaign.md) for a basic example.
 
 ### Necessary imports
 
 import numpy as np
 
 from baybe.campaign import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
     SubstanceParameter,
 )
 from baybe.recommenders import (
     FPSRecommender,
@@ -70,27 +70,23 @@
     invalid_surrogate_model = NGBoostSurrogate(model_params={"NOT_A_PARAM": None})
 except ValueError as e:
     print("The validator will give an error here:")
     print(e)
 
 ### Links for documentation
 
-# Note that `GaussianProcessSurrogate` will support custom parameters in the future
-
 # [`RandomForestModel`](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)
 # [`NGBoostModel`](https://stanfordmlgroup.github.io/ngboost/1-useage.html)
 # [`BayesianLinearModel`](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.ARDRegression.html)
 
 ### Creating the campaign
 
 campaign = Campaign(
     searchspace=SearchSpace.from_product(parameters=parameters, constraints=None),
-    objective=Objective(
-        mode="SINGLE", targets=[NumericalTarget(name="Yield", mode="MAX")]
-    ),
+    objective=SingleTargetObjective(target=NumericalTarget(name="Yield", mode="MAX")),
     recommender=TwoPhaseMetaRecommender(
         recommender=SequentialGreedyRecommender(surrogate_model=surrogate_model),
         initial_recommender=FPSRecommender(),
     ),
 )
 
 ### Iterate with recommendations and measurements
```

### Comparing `baybe-0.8.2/examples/Multi_Target/desirability.py` & `baybe-0.9.0/examples/Multi_Target/desirability.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # This example assumes some basic familiarity with using BayBE.
 # We thus refer to [`campaign`](./../Basics/campaign.md) for a basic example.
 
 ### Necessary imports for this example
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import DesirabilityObjective
 from baybe.parameters import CategoricalParameter, NumericalDiscreteParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.dataframe import add_fake_results
 
 ### Experiment setup and creating the searchspace
 
@@ -71,27 +71,26 @@
 
 # Now to work with these three targets the objective object must be properly created.
 # The mode is set to `DESIRABILITY` and the targets are described in a list.
 
 targets = [Target_1, Target_2, Target_3]
 
 # As the recommender requires a single function, the different targets need to be combined.
-# Thus, a `combine_function` is used to create a single target out of the several targets given.
+# Thus, a `scalarizer` is used to create a single target out of the several targets given.
 # The combine function can either be the mean `MEAN` or the geometric mean `GEOM_MEAN`.
 # Per default, `GEOM_MEAN` is used.
 # Weights for each target can also be specified as a list of floats in the arguments
 # Per default, weights are equally distributed between all targets and are normalized internally.
 # It is thus not necessary to handle normalization or scaling.
 
 
-objective = Objective(
-    mode="DESIRABILITY",
+objective = DesirabilityObjective(
     targets=targets,
     weights=[20, 20, 60],
-    combine_func="MEAN",
+    scalarizer="MEAN",
 )
 
 print(objective)
 
 ### Creating and printing the campaign
 
 campaign = Campaign(searchspace=searchspace, objective=objective)
```

### Comparing `baybe-0.8.2/examples/Searchspaces/continuous_space_botorch_function.py` & `baybe-0.9.0/examples/Searchspaces/continuous_space_botorch_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 ### Necessary imports for this example
 
 from botorch.test_functions import Rastrigin
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalContinuousParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 
 ### Defining the test function
 
@@ -57,17 +57,15 @@
         name=f"x_{k+1}",
         bounds=(BOUNDS[0, k], BOUNDS[1, k]),
     )
     for k in range(DIMENSION)
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing the campaign and performing a recommendation
 
 campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
```

### Comparing `baybe-0.8.2/examples/Searchspaces/continuous_space_custom_function.py` & `baybe-0.9.0/examples/Searchspaces/continuous_space_custom_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # This example assumes some basic familiarity with using BayBE.
 # We thus refer to [`campaign`](./../Basics/campaign.md) for a basic example.
 
 ### Necessary imports
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalContinuousParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 
 ### Defining the custom test function
 
 # The function should accept an arbitrary or fixed amount of floats as input.
@@ -49,17 +49,15 @@
         bounds=BOUNDS[k],
     )
     for k in range(DIMENSION)
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing the campaign and performing a recommendation
 
 campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
```

### Comparing `baybe-0.8.2/examples/Searchspaces/discrete_space.py` & `baybe-0.9.0/examples/Searchspaces/discrete_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ### Necessary imports for this example
 
 import numpy as np
 from botorch.test_functions import Rastrigin
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 
 ### Defining the test function
 
@@ -75,17 +75,15 @@
         values=list(np.linspace(BOUNDS[0, k], BOUNDS[1, k], POINTS_PER_DIM)),
         tolerance=0.01,
     )
     for k in range(DIMENSION)
 ]
 
 searchspace = SearchSpace.from_product(parameters=parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing the campaign and performing a recommendation
 
 campaign = Campaign(
     searchspace=searchspace,
     objective=objective,
 )
```

### Comparing `baybe-0.8.2/examples/Searchspaces/hybrid_space.py` & `baybe-0.9.0/examples/Searchspaces/hybrid_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ### Necessary imports for this example
 
 import numpy as np
 from botorch.test_functions import Rastrigin
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalContinuousParameter, NumericalDiscreteParameter
 from baybe.recommenders import NaiveHybridSpaceRecommender, TwoPhaseMetaRecommender
 from baybe.searchspace import SearchSpace
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 
 ### Defining the test function and the hybrid dimensions
@@ -96,17 +96,15 @@
         values=list(np.linspace(BOUNDS[0, k], BOUNDS[1, k], POINTS_PER_DIM)),
         tolerance=0.01,
     )
     for k in DISC_INDICES
 ]
 
 searchspace = SearchSpace.from_product(parameters=disc_parameters + cont_parameters)
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Constructing hybrid recommenders
 
 # Here, we explicitly create a recommender object to use the `NaiveHybridSpaceRecommender`.
 # The keywords `disc_recommender` and `cont_recommender` can be used to select different
 # recommenders for the corresponding subspaces.
 # We use the default choices, which is the `SequentialGreedyRecommender`.
```

### Comparing `baybe-0.8.2/examples/Serialization/basic_serialization.py` & `baybe-0.9.0/examples/Serialization/basic_serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # We thus refer to [`campaign`](./../Basics/campaign.md) for a basic example.
 
 ### Necessary imports
 
 import numpy as np
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     NumericalDiscreteParameter,
 )
 from baybe.recommenders import (
     FPSRecommender,
     SequentialGreedyRecommender,
@@ -43,17 +43,15 @@
     ),
 ]
 
 ### Creating the campaign
 
 campaign = Campaign(
     searchspace=SearchSpace.from_product(parameters=parameters, constraints=None),
-    objective=Objective(
-        mode="SINGLE", targets=[NumericalTarget(name="Yield", mode="MAX")]
-    ),
+    objective=SingleTargetObjective(target=NumericalTarget(name="Yield", mode="MAX")),
     recommender=TwoPhaseMetaRecommender(
         recommender=SequentialGreedyRecommender(),
         initial_recommender=FPSRecommender(),
     ),
 )
 
 ### Serialization and de-serialization
```

### Comparing `baybe-0.8.2/examples/Serialization/create_from_config.py` & `baybe-0.9.0/examples/Serialization/create_from_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "type": "FPSRecommender"
         },
         "recommender": {
             "type": "SequentialGreedyRecommender",
             "surrogate_model": {
                 "type": "GaussianProcessSurrogate"
             },
-            "acquisition_function_cls": "qEI",
+            "acquisition_function": "qEI",
             "allow_repeated_recommendations": false,
             "allow_recommending_already_measured": false
         },
         "switch_after": 1
     }
 }
 """
```

### Comparing `baybe-0.8.2/examples/Serialization/validate_config.py` & `baybe-0.9.0/examples/Serialization/validate_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             "type": "FPSRecommender"
         },
         "recommender": {
             "type": "SequentialGreedyRecommender",
             "surrogate_model": {
                 "type": "GaussianProcessSurrogate"
             },
-            "acquisition_function_cls": "qEI",
+            "acquisition_function": "qEI",
             "allow_repeated_recommendations": false,
             "allow_recommending_already_measured": false
         },
         "switch_after": 1
     }
 }
 """
@@ -144,15 +144,15 @@
             "type": "FPSRecommender"
         },
         "recommender": {
             "type": "SequentialGreedyRecommender",
             "surrogate_model": {
                 "type": "GaussianProcessSurrogate"
             },
-            "acquisition_function_cls": "qEI",
+            "acquisition_function": "qEI",
             "allow_repeated_recommendations": false,
             "allow_recommending_already_measured": false
         }
     }
 }
 """
 )
```

### Comparing `baybe-0.8.2/examples/Transfer_Learning/backtesting.py` & `baybe-0.9.0/examples/Transfer_Learning/backtesting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## Backtesting
 
 # This example demonstrates the use of the
-# [`simulate_transfer_learning`](baybe.simulation.simulate_transfer_learning) function
-# to learn across tasks:
+# [`simulate_transfer_learning`](baybe.simulation.transfer_learning.simulate_transfer_learning)
+# function to learn across tasks:
 # * We construct a campaign,
 # * define two related test functions,
 # * use the data from the first function to train the second,
 # * and vice versa
 
 ### Imports
 
@@ -16,15 +16,15 @@
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from botorch.test_functions.synthetic import Hartmann
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, TaskParameter
 from baybe.searchspace import SearchSpace
 from baybe.simulation import simulate_scenarios, simulate_transfer_learning
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 from baybe.utils.plotting import create_example_plots
 
@@ -42,17 +42,15 @@
 
 ### Creating the Optimization Objective
 
 # The test functions each have a single output that is to be minimized.
 # The corresponding [Objective](baybe.objective.Objective)
 # is created as follows:
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Creating the Search Space
 
 # This example uses the [Hartmann Function](https://botorch.org/api/test_functions.html#botorch.test_functions.synthetic.Hartmann)
 # as implemented by `botorch`.
 # The bounds of the search space are dictated by the test function and can be extracted
 # from the function itself.
```

### Comparing `baybe-0.8.2/examples/Transfer_Learning/backtesting_dark.svg` & `baybe-0.9.0/examples/Transfer_Learning/backtesting_dark.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Transfer_Learning/backtesting_light.svg` & `baybe-0.9.0/examples/Transfer_Learning/backtesting_light.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Transfer_Learning/basic_transfer_learning.py` & `baybe-0.9.0/examples/Transfer_Learning/basic_transfer_learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from botorch.test_functions.synthetic import Hartmann
 
 from baybe import Campaign
-from baybe.objective import Objective
+from baybe.objectives import SingleTargetObjective
 from baybe.parameters import NumericalDiscreteParameter, TaskParameter
 from baybe.searchspace import SearchSpace
 from baybe.simulation import simulate_scenarios
 from baybe.targets import NumericalTarget
 from baybe.utils.botorch_wrapper import botorch_function_wrapper
 from baybe.utils.plotting import create_example_plots
 
@@ -41,17 +41,15 @@
 
 ### Creating the Optimization Objective
 
 # The test functions each have a single output that is to be minimized.
 # The corresponding [Objective](baybe.objective.Objective)
 # is created as follows:
 
-objective = Objective(
-    mode="SINGLE", targets=[NumericalTarget(name="Target", mode="MIN")]
-)
+objective = SingleTargetObjective(target=NumericalTarget(name="Target", mode="MIN"))
 
 ### Creating the Searchspace
 
 # The bounds of the search space are dictated by the test function:
 
 BOUNDS = Hartmann(dim=DIMENSION).bounds
```

### Comparing `baybe-0.8.2/examples/Transfer_Learning/basic_transfer_learning_dark.svg` & `baybe-0.9.0/examples/Transfer_Learning/basic_transfer_learning_dark.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/examples/Transfer_Learning/basic_transfer_learning_light.svg` & `baybe-0.9.0/examples/Transfer_Learning/basic_transfer_learning_light.svg`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/mypy.ini` & `baybe-0.9.0/mypy.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 [mypy]
 packages = baybe
 
 ; at some point, these excludes should all be gone ...
 exclude = (?x)(
-          baybe/searchspace
-          | baybe/serialization
+          baybe/serialization
+          | baybe/simulation
           | baybe/strategies
           | baybe/surrogates
           | baybe/utils/dataframe.py
-          | baybe/acquisition.py
           | baybe/deprecation.py
           | baybe/exceptions.py
-          | baybe/objective.py
           | baybe/scaler.py
           | baybe/simulation.py
-          | baybe/surrogate.py
           )
 
-[mypy-botorch.acquisition]
+[mypy-gpytorch.*]
 ignore_missing_imports = True
 
-[mypy-botorch.optim]
+[mypy-botorch.*]
 ignore_missing_imports = True
 
-[mypy-botorch.test_functions]
+[mypy-botorch.utils.sampling]
 ignore_missing_imports = True
 
 [mypy-setuptools_scm]
 ignore_missing_imports = True
 
 [mypy-scipy.spatial.distance]
 ignore_missing_imports = True
@@ -59,8 +56,8 @@
 [mypy-rdkit]
 ignore_missing_imports = True
 
 [mypy-rdkit.Chem.rdMolDescriptors]
 ignore_missing_imports = True
 
 [mypy-mordred]
-ignore_missing_imports = True
+ignore_missing_imports = True
```

### Comparing `baybe-0.8.2/pyproject.toml` & `baybe-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,21 @@
     "pandas>=1.4.2",
     "protobuf<=3.20.3",
     "scikit-learn>=1.1.1",
     "scikit-learn-extra>=0.3.0",
     "scipy>=1.10.1",
     "setuptools-scm>=7.1.0",
     "torch>=1.13.1",
+    "typing_extensions>=4.7.0",
 
     # Telemetry:
     "opentelemetry-sdk>=1.16.0",
     "opentelemetry-propagator-aws-xray>=1.0.0",
     "opentelemetry-exporter-otlp>=1.16.0",
     "opentelemetry-sdk-extension-aws>=2.0.0",
-    "requests>=2.31.0", # see AUDIT NOTE
-    "urllib3>=2.0.7", # see AUDIT NOTE
 ]
 
 [project.urls]
 Homepage = "https://emdgroup.github.io/baybe/"
 Documentation = "https://emdgroup.github.io/baybe/_autosummary/baybe.html"
 Changelog = "https://emdgroup.github.io/baybe/misc/changelog_link.html"
 GitHub = "https://github.com/emdgroup/baybe/"
@@ -86,15 +85,15 @@
     "baybe[examples]",
     "baybe[lint]",
     "baybe[mypy]",
     "baybe[onnx]",
     "baybe[simulation]",
     "baybe[test]",
     "pip-audit>=2.5.5",
-    "tox>=4.10.0",
+    "tox-uv>=1.7.0",
 ]
 
 docs = [
     "baybe[examples]", # docs cannot be built without running examples
     "furo>=2023.09.10",
     "jupyter>=1.0.0",
     "jupytext>=1.16.1",
@@ -125,15 +124,14 @@
     "typos==1.16.23" # see DEV TOOLS NOTE
 ]
 
 mypy = [
     "mypy>=1.6.1",
     "pandas-stubs>=2.0.3.230814",
     "funcy-stubs>=0.1.1",
-    "types-requests>=2.31.0.20240106",
     "types-seaborn>=0.12.2"
 ]
 
 simulation = [
     "xyzpy>=1.2.1",
 ]
```

### Comparing `baybe-0.8.2/ruff.toml` & `baybe-0.9.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/streamlit/initial_recommender.py` & `baybe-0.9.0/streamlit/initial_recommender.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/streamlit/surrogate_models.py` & `baybe-0.9.0/streamlit/surrogate_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 This means that the shown function approximation should always appear visually the same
 when the input and output scales are changed.
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 import torch
-from botorch.acquisition import qExpectedImprovement
 from botorch.optim import optimize_acqf_discrete
 from funcy import rpartial
 
 import streamlit as st
-from baybe.acquisition import debotorchize
+from baybe.acquisition import qExpectedImprovement
 from baybe.parameters import NumericalDiscreteParameter
 from baybe.searchspace import SearchSpace
-from baybe.surrogates import get_available_surrogates
+from baybe.surrogates.base import Surrogate
+from baybe.utils.basic import get_subclasses
 
 # define constants
 N_PARAMETER_VALUES = 1000
 
 
 def cubic(
     x: np.ndarray, x_min: float, x_max: float, amplitude: float, bias: float
@@ -70,15 +71,17 @@
         "Constant": constant,
         "Linear": linear,
         "Cubic": cubic,
     }
 
     # collect all available surrogate models
     surrogate_model_classes = {
-        surr.__name__: surr for surr in get_available_surrogates()
+        surr.__name__: surr
+        for surr in get_subclasses(Surrogate)
+        if surr.__name__ != "CustomONNXSurrogate"
     }
 
     # simulation parameters
     random_seed = int(st.sidebar.number_input("Random seed", value=1337))
     function_name = st.sidebar.selectbox("Test function", list(test_functions.keys()))
     surrogate_name = st.sidebar.selectbox(
         "Surrogate model", list(surrogate_model_classes.keys())
@@ -129,16 +132,17 @@
 
     # create the surrogate model, train it, and get its predictions
     surrogate_model = surrogate_model_classes[surrogate_name]()
     surrogate_model.fit(searchspace, train_x.unsqueeze(-1), train_y.unsqueeze(-1))
 
     # recommend next experiments
     # TODO: use BayBE recommender and add widgets for recommender selection
-    best_f = train_y.max().item()
-    acqf = debotorchize(qExpectedImprovement)(surrogate_model, best_f)
+    acqf = qExpectedImprovement().to_botorch(
+        surrogate_model, pd.DataFrame(train_x), pd.DataFrame(train_y)
+    )
     recommendatations = optimize_acqf_discrete(
         acqf, q=n_recommendations, choices=test_x.unsqueeze(-1)
     )[0]
 
     # create the mean and standard deviation predictions for the entire search space
     mean, covar = surrogate_model.posterior(test_x.unsqueeze(-1))
     mean = mean.detach().numpy()
```

### Comparing `baybe-0.8.2/tests/README.md` & `baybe-0.9.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/conftest.py` & `baybe-0.9.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from itertools import chain
 from typing import Union
 
 import numpy as np
 import pandas as pd
 import pytest
 import torch
+from hypothesis import settings as hypothesis_settings
 
+from baybe.acquisition import qExpectedImprovement
 from baybe.campaign import Campaign
 from baybe.constraints import (
     ContinuousLinearEqualityConstraint,
     ContinuousLinearInequalityConstraint,
     DiscreteCustomConstraint,
     DiscreteDependenciesConstraint,
     DiscreteExcludeConstraint,
@@ -22,23 +24,26 @@
     DiscretePermutationInvarianceConstraint,
     DiscreteProductConstraint,
     DiscreteSumConstraint,
     SubSelectionCondition,
     ThresholdCondition,
 )
 from baybe.exceptions import OptionalImportError
-from baybe.objective import Objective
+from baybe.kernels import MaternKernel
+from baybe.objectives.desirability import DesirabilityObjective
+from baybe.objectives.single import SingleTargetObjective
 from baybe.parameters import (
     CategoricalParameter,
     CustomDiscreteParameter,
     NumericalContinuousParameter,
     NumericalDiscreteParameter,
     SubstanceEncoding,
     TaskParameter,
 )
+from baybe.priors import GammaPrior
 from baybe.recommenders.meta.base import MetaRecommender
 from baybe.recommenders.meta.sequential import (
     SequentialMetaRecommender,
     StreamingSequentialMetaRecommender,
     TwoPhaseMetaRecommender,
 )
 from baybe.recommenders.pure.base import PureRecommender
@@ -51,14 +56,15 @@
 from baybe.targets import NumericalTarget
 from baybe.telemetry import (
     VARNAME_TELEMETRY_ENABLED,
     VARNAME_TELEMETRY_HOSTNAME,
     VARNAME_TELEMETRY_USERNAME,
 )
 from baybe.utils.basic import hilberts_factory
+from baybe.utils.boolean import strtobool
 from baybe.utils.dataframe import add_fake_results, add_parameter_noise
 
 try:
     import baybe.utils.chemistry  # noqa: F401  # Tests if chem deps are available
     from baybe.parameters.substance import SubstanceParameter
 
     _CHEM_INSTALLED = True
@@ -73,15 +79,20 @@
     # Note: due to our streamlit folder we cannot use plain `import streamlit` here
     from streamlit import info  # noqa: F401  # Tests if streamlit is available
 
     _STREAMLIT_INSTALLED = True
 except ImportError:
     _STREAMLIT_INSTALLED = False
 
-# All fixture functions have prefix 'fixture_' and explicitly declared name so they
+# Hypothesis settings
+hypothesis_settings.register_profile("ci", deadline=500, max_examples=100)
+if strtobool(os.getenv("CI", "false")):
+    hypothesis_settings.load_profile("ci")
+
+# All fixture functions have prefix 'fixture_' and explicitly declared name, so they
 # can be reused by other fixtures, see
 # https://docs.pytest.org/en/stable/reference/reference.html#pytest-fixture
 
 
 @pytest.fixture(scope="session", autouse=True)
 def disable_telemetry():
     """Disables telemetry during pytesting via fixture."""
@@ -588,42 +599,54 @@
     return StreamingSequentialMetaRecommender(
         recommenders=chain(
             (RandomRecommender(),), hilberts_factory(SequentialGreedyRecommender)
         )
     )
 
 
-@pytest.fixture(name="acquisition_function_cls")
+@pytest.fixture(name="acqf")
 def fixture_default_acquisition_function():
     """The default acquisition function to be used if not specified differently."""
-    return "qEI"
+    return qExpectedImprovement()
+
+
+@pytest.fixture(name="lengthscale_prior")
+def fixture_default_lengthscale_prior():
+    """The default lengthscale prior to be used if not specified differently."""
+    return GammaPrior(3, 1)
+
+
+@pytest.fixture(name="kernel")
+def fixture_default_kernel(lengthscale_prior):
+    """The default kernel to be used if not specified differently."""
+    return MaternKernel(nu=5 / 2, lengthscale_prior=lengthscale_prior)
 
 
 @pytest.fixture(name="surrogate_model")
-def fixture_default_surrogate_model(request, onnx_surrogate):
+def fixture_default_surrogate_model(request, onnx_surrogate, kernel):
     """The default surrogate model to be used if not specified differently."""
     if hasattr(request, "param") and request.param == "onnx":
         return onnx_surrogate
-    return GaussianProcessSurrogate()
+    return GaussianProcessSurrogate(kernel_or_factory=kernel)
 
 
 @pytest.fixture(name="initial_recommender")
 def fixture_initial_recommender():
     """The default initial recommender to be used if not specified differently."""
     return RandomRecommender()
 
 
 @pytest.fixture(name="recommender")
-def fixture_recommender(initial_recommender, surrogate_model, acquisition_function_cls):
+def fixture_recommender(initial_recommender, surrogate_model, acqf):
     """The default recommender to be used if not specified differently."""
     return TwoPhaseMetaRecommender(
         initial_recommender=initial_recommender,
         recommender=SequentialGreedyRecommender(
             surrogate_model=surrogate_model,
-            acquisition_function_cls=acquisition_function_cls,
+            acquisition_function=acqf,
         ),
     )
 
 
 @pytest.fixture(name="meta_recommender")
 def fixture_meta_recommender(
     request,
@@ -640,16 +663,19 @@
         return streaming_sequential_meta_recommender
     raise NotImplementedError("unknown recommender type")
 
 
 @pytest.fixture(name="objective")
 def fixture_default_objective(targets):
     """The default objective to be used if not specified differently."""
-    mode = "SINGLE" if len(targets) == 1 else "DESIRABILITY"
-    return Objective(mode=mode, targets=targets)
+    return (
+        SingleTargetObjective(targets[0])
+        if len(targets) == 1
+        else DesirabilityObjective(targets)
+    )
 
 
 @pytest.fixture(name="config")
 def fixture_default_config():
     """The default config to be used if not specified differently."""
     # TODO: Once `to_config` is implemented, generate the default config from the
     #   default campaign object instead of hardcoding it here. This avoids redundant
@@ -690,15 +716,15 @@
         "recommender": {
             "type": "TwoPhaseMetaRecommender",
             "initial_recommender": {
                 "type": "RandomRecommender"
             },
             "recommender": {
                 "type": "SequentialGreedyRecommender",
-                "acquisition_function_cls": "qEI",
+                "acquisition_function": "qEI",
                 "allow_repeated_recommendations": false,
                 "allow_recommending_already_measured": false
             },
             "switch_after": 1
         }
     }
     """.replace(
```

### Comparing `baybe-0.8.2/tests/docs/test_docs.py` & `baybe-0.9.0/tests/docs/test_docs.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 import pytest
 
 from baybe.recommenders import RandomRecommender, TwoPhaseMetaRecommender
 
 from ..conftest import _CHEM_INSTALLED
 from .utils import extract_code_blocks
 
-doc_files = ["README.md", *Path("docs/userguide/").rglob("*.md")]
+doc_files = list(map(str, [Path("README.md"), *Path("docs/userguide/").rglob("*.md")]))
 """Files whose code blocks are to be checked."""
-doc_files_pseudocode = [Path("docs/userguide/campaigns.md")]
-"""Files which contain pseudocode that needs to be checked using fixtures."""
+
+doc_files_pseudocode = list(map(str, [Path("docs/userguide/campaigns.md")]))
+"""Files containing pseudocode that needs to be checked with injected fixtures."""
 
 
 @pytest.mark.skipif(
     not _CHEM_INSTALLED, reason="Optional chem dependency not installed."
 )
-@pytest.mark.parametrize("file", doc_files)
+@pytest.mark.parametrize("file", doc_files, ids=doc_files)
 def test_code_executability(file: Path):
     """The code blocks in the file become a valid python script when concatenated.
 
     Blocks surrounded with "triple-tilde" are ignored.
     """
     userguide_code = "\n".join(extract_code_blocks(file, include_tilde=False))
     exec(userguide_code)
 
 
 # TODO: Needs a refactoring (files codeblocks should be auto-detected)
-@pytest.mark.parametrize("file", doc_files_pseudocode)
+@pytest.mark.parametrize("file", doc_files_pseudocode, ids=doc_files_pseudocode)
 @pytest.mark.parametrize(
     "recommender",
     [
         TwoPhaseMetaRecommender(
             initial_recommender=RandomRecommender(), recommender=RandomRecommender()
         )
     ],
@@ -47,15 +48,15 @@
     Due to a bug related to the serialization of the default recommender, this currently
     uses a non-default recommender.
     """
     userguide_pseudocode = "\n".join(extract_code_blocks(file, include_tilde=True))
     exec(userguide_pseudocode)
 
 
-@pytest.mark.parametrize("file", doc_files)
+@pytest.mark.parametrize("file", doc_files, ids=doc_files)
 def test_code_format(file: Path):
     """The code blocks in the file are properly formatted.
 
     If it fails, run `pytest` with the `-s` flag to show the necessary format changes.
     """
     code_blocks = extract_code_blocks(file)
     success = True
```

### Comparing `baybe-0.8.2/tests/docs/test_examples.py` & `baybe-0.9.0/tests/docs/test_examples.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 from ..conftest import _CHEM_INSTALLED
 
 # Run these tests in reduced settings
 _SMOKE_TEST_CACHE = os.environ.get("SMOKE_TEST", None)
 os.environ["SMOKE_TEST"] = "true"
 
 
+paths = [str(x) for x in Path("examples/").rglob("*.py")]
+
+
 @pytest.mark.slow
 @pytest.mark.skipif(
     not (_CHEM_INSTALLED and _ONNX_INSTALLED), reason="skipped for core tests"
 )
-@pytest.mark.parametrize("example", Path("examples/").rglob("*.py"))
-def test_example(example: Path):
+@pytest.mark.parametrize("example", paths, ids=paths)
+def test_example(example: str):
     """Test an individual example by running it."""
-    runpy.run_path(str(example))
+    runpy.run_path(example)
 
 
 if _SMOKE_TEST_CACHE is not None:
     os.environ["SMOKE_TEST"] = _SMOKE_TEST_CACHE
 else:
     os.environ.pop("SMOKE_TEST")
```

### Comparing `baybe-0.8.2/tests/docs/utils.py` & `baybe-0.9.0/tests/docs/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Utilities for doc testing."""
 
 import re
 from pathlib import Path
+from textwrap import dedent
 from typing import Union
 
 
 def extract_code_blocks(
     path: Union[str, Path], include_tilde: bool = True
 ) -> list[str]:
     """Extract all python code blocks from the specified file."""
     contents = Path(path).read_text()
     pattern = (
-        r"(?:```|~~~)python\s+(.*?)\s+(?:```|~~~)"
+        r"\s*(?:```|~~~)python\n*(.*?)\n*\s*(?:```|~~~)"
         if include_tilde
-        else r"```python\s+(.*?)\s+```"
+        else r"\s*```python\n*(.*?)\n*\s*```"
     )
-    code_blocks = re.findall(pattern, contents, flags=re.DOTALL)
+    code_blocks = [dedent(c) for c in re.findall(pattern, contents, flags=re.DOTALL)]
 
     return code_blocks
```

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_intervals.py` & `baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_intervals.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_parameters.py` & `baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_parameters.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_searchspace.py` & `baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_searchspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     CategoricalParameter,
     NumericalContinuousParameter,
     NumericalDiscreteParameter,
 )
 from baybe.parameters.categorical import TaskParameter
 from baybe.searchspace import SearchSpace, SubspaceContinuous
 from baybe.searchspace.discrete import SubspaceDiscrete
-from tests.hypothesis_strategies.parameters import numerical_discrete_parameter
+from tests.hypothesis_strategies.parameters import numerical_discrete_parameters
 
 # Discrete inputs for testing
 s_x = pd.Series([1, 2, 3], name="x")
 p_x = NumericalDiscreteParameter(name="x", values=[1, 2, 3])
 p_x_over = NumericalDiscreteParameter(name="x", values=[1, 2, 3, 4])
 p_x_under = NumericalDiscreteParameter(name="x", values=[1, 2])
 s_y = pd.Series(["a", "b", "c"], name="y")
@@ -38,80 +38,80 @@
 # Mixed inputs for testing
 df = pd.concat([df_discrete, df_continuous], axis=1)
 
 
 @pytest.mark.parametrize(
     ("df", "parameters", "expected"),
     [
-        param(s_x.to_frame(), [p_x], [p_x], id="num-match"),
-        param(s_x.to_frame(), [p_x_over], [p_x_over], id="num_overparametrized"),
-        param(s_x.to_frame(), [p_x_under], ValueError, id="num_underparametrized"),
-        param(df_discrete, [p_x, p_x], ValueError, id="duplicate-name"),
-        param(s_x.to_frame(), [p_x, p_y], ValueError, id="no_match"),
-        param(s_y.to_frame(), [p_y], [p_y], id="cat-match"),
-        param(df_discrete, [p_x, p_y], [p_x, p_y], id="both-match"),
-        param(df_discrete, [p_x], [p_x, p_y], id="one-unspecified"),
+        param(s_x.to_frame(), (p_x,), (p_x,), id="num-match"),
+        param(s_x.to_frame(), (p_x_over,), (p_x_over,), id="num_overparametrized"),
+        param(s_x.to_frame(), (p_x_under,), ValueError, id="num_underparametrized"),
+        param(df_discrete, (p_x, p_x), ValueError, id="duplicate-name"),
+        param(s_x.to_frame(), (p_x, p_y), ValueError, id="no_match"),
+        param(s_y.to_frame(), (p_y,), (p_y,), id="cat-match"),
+        param(df_discrete, (p_x, p_y), (p_x, p_y), id="both-match"),
+        param(df_discrete, (p_x,), (p_x, p_y), id="one-unspecified"),
     ],
 )
 def test_discrete_space_creation_from_dataframe(df, parameters, expected):
     """Parameters are automatically inferred and exceptions are triggered."""
-    if isinstance(expected, list):
+    if isinstance(expected, tuple):
         subspace = SubspaceDiscrete.from_dataframe(df, parameters)
         actual = subspace.parameters
         assert actual == expected, (actual, expected)
     else:
         with pytest.raises(expected):
             SubspaceDiscrete.from_dataframe(df, parameters)
 
 
 @pytest.mark.parametrize(
     ("df", "parameters", "expected"),
     [
-        param(s_a.to_frame(), [p_a], [p_a], id="match"),
-        param(s_a.to_frame(), [p_a_over], [p_a_over], id="overparametrized"),
-        param(s_a.to_frame(), [p_a_under], ValueError, id="underparametrized"),
-        param(df_continuous, [p_a, p_a], ValueError, id="duplicate-name"),
-        param(s_a.to_frame(), [p_a, p_b], ValueError, id="no_match"),
-        param(df_continuous, [p_a], [p_a, p_b], id="one-unspecified"),
+        param(s_a.to_frame(), (p_a,), (p_a,), id="match"),
+        param(s_a.to_frame(), (p_a_over,), (p_a_over,), id="overparametrized"),
+        param(s_a.to_frame(), (p_a_under,), ValueError, id="underparametrized"),
+        param(df_continuous, (p_a, p_a), ValueError, id="duplicate-name"),
+        param(s_a.to_frame(), (p_a, p_b), ValueError, id="no_match"),
+        param(df_continuous, (p_a,), (p_a, p_b), id="one-unspecified"),
     ],
 )
 def test_continuous_space_creation_from_dataframe(df, parameters, expected):
     """Parameters are automatically inferred and exceptions are triggered."""
-    if isinstance(expected, list):
+    if isinstance(expected, tuple):
         subspace = SubspaceContinuous.from_dataframe(df, parameters)
         actual = subspace.parameters
         assert actual == expected, (actual, expected)
     else:
         with pytest.raises(expected):
             SubspaceContinuous.from_dataframe(df, parameters)
 
 
 @pytest.mark.parametrize(
     ("df", "parameters", "expected"),
     [
-        param(df, [p_x, p_y, p_a, p_b], [p_x, p_y, p_a, p_b], id="match"),
-        param(df, [p_x, p_x, p_x, p_x], ValueError, id="duplicates"),
-        param(df, [p_x], ValueError, id="missing"),
+        param(df, (p_x, p_y, p_a, p_b), (p_x, p_y, p_a, p_b), id="match"),
+        param(df, (p_x, p_x, p_x, p_x), ValueError, id="duplicates"),
+        param(df, (p_x,), ValueError, id="missing"),
     ],
 )
 def test_searchspace_creation_from_dataframe(df, parameters, expected):
     """Parameters are automatically inferred and exceptions are triggered."""
-    if isinstance(expected, list):
+    if isinstance(expected, tuple):
         subspace = SearchSpace.from_dataframe(df, parameters)
         actual = subspace.parameters
         assert actual == expected, (actual, expected)
     else:
         with pytest.raises(expected):
             SearchSpace.from_dataframe(df, parameters)
 
 
 @pytest.mark.parametrize("boundary_only", (False, True))
 @given(
     parameters=st.lists(
-        numerical_discrete_parameter(min_value=0.0, max_value=1.0),
+        numerical_discrete_parameters(min_value=0.0, max_value=1.0),
         min_size=1,
         max_size=5,
         unique_by=lambda x: x.name,
     )
 )
 def test_discrete_space_creation_from_simplex_inner(parameters, boundary_only):
     """Candidates from a simplex space satisfy the simplex constraint."""
```

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/alternative_creation/test_targets.py` & `baybe-0.9.0/tests/hypothesis_strategies/alternative_creation/test_targets.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/dataframes.py` & `baybe-0.9.0/tests/hypothesis_strategies/dataframes.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/parameters.py` & `baybe-0.9.0/tests/hypothesis_strategies/parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from baybe.parameters.numerical import (
     NumericalContinuousParameter,
     NumericalDiscreteParameter,
 )
 from baybe.parameters.substance import SubstanceEncoding, SubstanceParameter
 from baybe.utils.numerical import DTypeFloatNumpy
 
-from .utils import interval
+from .utils import intervals
 
-decorrelation = st.one_of(
+decorrelations = st.one_of(
     st.booleans(),
     st.floats(min_value=0.0, max_value=1.0, exclude_min=True, exclude_max=True),
 )
 """A strategy that generates decorrelation settings."""
 
-parameter_name = st.text(min_size=1)
+parameter_names = st.text(min_size=1)
 """A strategy that generates parameter names."""
 
 categories = st.lists(st.text(min_size=1), min_size=2, unique=True)
 """A strategy that generates parameter categories."""
 
 
 @st.composite
@@ -72,21 +72,21 @@
         unique=True,
         dtype=DTypeFloatNumpy,
     )
     return draw(data_frames(index=index, columns=cols))
 
 
 @st.composite
-def numerical_discrete_parameter(
+def numerical_discrete_parameters(
     draw: st.DrawFn,
     min_value: Optional[float] = None,
     max_value: Optional[float] = None,
 ):
     """Generate :class:`baybe.parameters.numerical.NumericalDiscreteParameter`."""
-    name = draw(parameter_name)
+    name = draw(parameter_names)
     values = draw(
         st.lists(
             st.floats(
                 allow_infinity=False,
                 allow_nan=False,
                 min_value=min_value,
                 max_value=max_value,
@@ -107,66 +107,82 @@
                 exclude_max=True,
             )
         )
     return NumericalDiscreteParameter(name=name, values=values, tolerance=tolerance)
 
 
 @st.composite
-def numerical_continuous_parameter(draw: st.DrawFn):
+def numerical_continuous_parameters(draw: st.DrawFn):
     """Generate :class:`baybe.parameters.numerical.NumericalContinuousParameter`."""
-    name = draw(parameter_name)
-    bounds = draw(interval(exclude_half_bounded=True, exclude_fully_unbounded=True))
+    name = draw(parameter_names)
+    bounds = draw(intervals(exclude_half_bounded=True, exclude_fully_unbounded=True))
     return NumericalContinuousParameter(name=name, bounds=bounds)
 
 
 @st.composite
-def categorical_parameter(draw: st.DrawFn):
+def categorical_parameters(draw: st.DrawFn):
     """Generate :class:`baybe.parameters.categorical.CategoricalParameter`."""
-    name = draw(parameter_name)
+    name = draw(parameter_names)
     values = draw(categories)
     encoding = draw(st.sampled_from(CategoricalEncoding))
     return CategoricalParameter(name=name, values=values, encoding=encoding)
 
 
 @st.composite
-def task_parameter(draw: st.DrawFn):
+def task_parameters(draw: st.DrawFn):
     """Generate :class:`baybe.parameters.categorical.TaskParameter`."""
-    name = draw(parameter_name)
+    name = draw(parameter_names)
     values = draw(categories)
     active_values = draw(
         st.lists(st.sampled_from(values), min_size=1, max_size=len(values), unique=True)
     )
     return TaskParameter(name=name, values=values, active_values=active_values)
 
 
 @st.composite
-def substance_parameter(draw: st.DrawFn):
+def substance_parameters(draw: st.DrawFn):
     """Generate :class:`baybe.parameters.substance.SubstanceParameter`."""
-    name = draw(parameter_name)
+    name = draw(parameter_names)
     data = draw(substance_data())
-    decorrelate = draw(decorrelation)
+    decorrelate = draw(decorrelations)
     encoding = draw(st.sampled_from(SubstanceEncoding))
     return SubstanceParameter(
         name=name, data=data, decorrelate=decorrelate, encoding=encoding
     )
 
 
 @st.composite
-def custom_parameter(draw: st.DrawFn):
+def custom_parameters(draw: st.DrawFn):
     """Generate :class:`baybe.parameters.custom.CustomDiscreteParameter`."""
-    name = draw(parameter_name)
+    name = draw(parameter_names)
     data = draw(custom_descriptors())
-    decorrelate = draw(decorrelation)
+    decorrelate = draw(decorrelations)
     return CustomDiscreteParameter(name=name, data=data, decorrelate=decorrelate)
 
 
-parameter = st.one_of(
+parameters = st.one_of(
     [
-        numerical_discrete_parameter(),
-        numerical_continuous_parameter(),
-        categorical_parameter(),
-        task_parameter(),
-        substance_parameter(),
-        custom_parameter(),
+        numerical_discrete_parameters(),
+        numerical_continuous_parameters(),
+        categorical_parameters(),
+        task_parameters(),
+        substance_parameters(),
+        custom_parameters(),
     ]
 )
 """A strategy that generates parameters."""
+
+
+discrete_parameters = st.one_of(
+    [
+        numerical_discrete_parameters(),
+        categorical_parameters(),
+        task_parameters(),
+        substance_parameters(),
+        custom_parameters(),
+    ]
+)
+"""A strategy that generates discrete parameters."""
+
+
+continuous_parameters = numerical_continuous_parameters
+"""A strategy that generates continuous parameters."""
```

### Comparing `baybe-0.8.2/tests/hypothesis_strategies/targets.py` & `baybe-0.9.0/tests/hypothesis_strategies/targets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 """Hypothesis strategies for targets."""
 
+from typing import Optional
+
 import hypothesis.strategies as st
 
 from baybe.targets.enum import TargetMode
 from baybe.targets.numerical import _VALID_TRANSFORMATIONS, NumericalTarget
+from baybe.utils.interval import Interval
 
-from .utils import interval
+from .utils import intervals as st_intervals
 
 target_name = st.text(min_size=1)
 """A strategy that generates target names."""
 
 
 @st.composite
-def numerical_target(draw: st.DrawFn):
-    """Generate :class:`baybe.targets.numerical.NumericalTarget`."""
+def numerical_targets(
+    draw: st.DrawFn, bounds_strategy: Optional[st.SearchStrategy[Interval]] = None
+):
+    """Generate :class:`baybe.targets.numerical.NumericalTarget`.
+
+    Args:
+        draw: Hypothesis draw object.
+        bounds_strategy: An optional strategy for generating the target bounds.
+
+    Returns:
+        _type_: _description_
+    """
     name = draw(target_name)
     mode = draw(st.sampled_from(TargetMode))
-    bounds = draw(
-        interval(
+    if bounds_strategy is None:
+        bounds_strategy = st_intervals(
             exclude_half_bounded=True, exclude_fully_unbounded=mode is TargetMode.MATCH
         )
-    )
+    bounds = draw(bounds_strategy)
     transformation = draw(st.sampled_from(_VALID_TRANSFORMATIONS[mode]))
 
     return NumericalTarget(
         name=name, mode=mode, bounds=bounds, transformation=transformation
     )
 
 
-target = numerical_target()
+targets = numerical_targets()
 """A strategy that generates targets."""
```

### Comparing `baybe-0.8.2/tests/serialization/test_campaign_serialization.py` & `baybe-0.9.0/tests/serialization/test_campaign_serialization.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/serialization/test_dataframe_serialization.py` & `baybe-0.9.0/tests/serialization/test_dataframe_serialization.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/serialization/test_meta_recommender_serialization.py` & `baybe-0.9.0/tests/serialization/test_meta_recommender_serialization.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/serialization/test_naive_hybrid_serialization.py` & `baybe-0.9.0/tests/serialization/test_naive_hybrid_serialization.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/serialization/test_parameter_serialization.py` & `baybe-0.9.0/tests/serialization/test_parameter_serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 from hypothesis import given
 from pytest import param
 
 from baybe.parameters.base import Parameter
 
 from ..conftest import _CHEM_INSTALLED
 from ..hypothesis_strategies.parameters import (
-    categorical_parameter,
-    custom_parameter,
-    numerical_continuous_parameter,
-    numerical_discrete_parameter,
-    substance_parameter,
-    task_parameter,
+    categorical_parameters,
+    custom_parameters,
+    numerical_continuous_parameters,
+    numerical_discrete_parameters,
+    substance_parameters,
+    task_parameters,
 )
 
 
 @pytest.mark.parametrize(
     "parameter_strategy",
     [
-        param(numerical_discrete_parameter(), id="NumericalDiscreteParameter"),
-        param(numerical_continuous_parameter(), id="NumericalContinuousParameter"),
-        param(categorical_parameter(), id="CategoricalParameter"),
-        param(task_parameter(), id="TaskParameter"),
-        param(custom_parameter(), id="CustomParameter"),
+        param(numerical_discrete_parameters(), id="NumericalDiscreteParameter"),
+        param(numerical_continuous_parameters(), id="NumericalContinuousParameter"),
+        param(categorical_parameters(), id="CategoricalParameter"),
+        param(task_parameters(), id="TaskParameter"),
+        param(custom_parameters(), id="CustomParameter"),
         param(
-            substance_parameter(),
+            substance_parameters(),
             id="SubstanceParameter",
             marks=pytest.mark.skipif(
                 not _CHEM_INSTALLED, reason="Optional chem dependency not installed."
             ),
         ),
     ],
 )
```

### Comparing `baybe-0.8.2/tests/serialization/test_searchspace_serialization.py` & `baybe-0.9.0/tests/serialization/test_searchspace_serialization.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/simulate_telemetry.py` & `baybe-0.9.0/tests/simulate_telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     "recommender": TwoPhaseMetaRecommender(
         recommender=SequentialGreedyRecommender(
             allow_repeated_recommendations=False,
             allow_recommending_already_measured=False,
         ),
         initial_recommender=RandomRecommender(),
     ),
-    "numerical_measurements_must_be_within_tolerance": True,
 }
 
 # Actual User
 print(f"Actual User Details: {get_user_details()}")
 campaign = Campaign(**config)
 for k in range(randint(4, 6)):
     dat = campaign.recommend(randint(2, 3))
```

### Comparing `baybe-0.8.2/tests/test_constraints_continuous.py` & `baybe-0.9.0/tests/test_constraints_continuous.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_constraints_discrete.py` & `baybe-0.9.0/tests/test_constraints_discrete.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_continuous.py` & `baybe-0.9.0/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_custom_parameter.py` & `baybe-0.9.0/tests/test_custom_parameter.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_custom_surrogate.py` & `baybe-0.9.0/tests/test_custom_surrogate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Tests for custom surrogate models."""
 from contextlib import nullcontext
 
 import pytest
 
 from baybe import Campaign
-from baybe.exceptions import ModelParamsNotSupportedError
 from baybe.surrogates import _ONNX_INSTALLED, register_custom_architecture
 from tests.conftest import run_iterations
 
 if _ONNX_INSTALLED:
     from baybe.surrogates import CustomONNXSurrogate
 
 
@@ -25,22 +24,14 @@
     with pytest.raises(TypeError):
         CustomONNXSurrogate(onnx_str=b"onnx_str")
 
     # Scenario: No onnx str
     with pytest.raises(TypeError):
         CustomONNXSurrogate(onnx_input_name="input")
 
-    # Scenario: Model Params non-empty
-    with pytest.raises(ModelParamsNotSupportedError):
-        CustomONNXSurrogate(
-            onnx_input_name="input",
-            onnx_str=onnx_str,
-            model_params={"Non_empty_dict": None},
-        )
-
 
 @pytest.mark.skipif(
     not _ONNX_INSTALLED, reason="Optional onnx dependency not installed."
 )
 def test_invalid_onnx_str():
     """Invalid onnx string causes error."""
     with pytest.raises(Exception):
```

### Comparing `baybe-0.8.2/tests/test_deprecations.py` & `baybe-0.9.0/tests/test_deprecations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,36 @@
 """Deprecation tests."""
 
 import json
+from unittest.mock import Mock
 
 import pytest
 
-from baybe import BayBE, Campaign
+from baybe import Campaign
+from baybe.acquisition.base import AcquisitionFunction
 from baybe.exceptions import DeprecationError
+from baybe.objective import Objective as OldObjective
+from baybe.objectives.base import Objective as NewObjective
+from baybe.objectives.desirability import DesirabilityObjective
 from baybe.recommenders.meta.sequential import TwoPhaseMetaRecommender
+from baybe.recommenders.pure.bayesian import SequentialGreedyRecommender
 from baybe.recommenders.pure.nonpredictive.sampling import (
     FPSRecommender,
     RandomRecommender,
 )
-from baybe.searchspace import SearchSpace
 from baybe.strategies import (
     SequentialStrategy,
-    Strategy,
     StreamingSequentialStrategy,
     TwoPhaseStrategy,
 )
-from baybe.targets import Objective
 from baybe.targets.base import Target
+from baybe.targets.numerical import NumericalTarget
 from baybe.utils.interval import Interval
 
 
-def test_deprecated_baybe_class(parameters, objective):
-    """Using the deprecated ``BayBE`` class raises a warning."""
-    with pytest.warns(DeprecationWarning):
-        BayBE(SearchSpace.from_product(parameters), objective)
-
-
-def test_moved_objective(targets):
-    """Importing ``Objective`` from ``baybe.targets`` raises a warning."""
-    with pytest.warns(DeprecationWarning):
-        Objective(mode="SINGLE", targets=targets)
-
-
-def test_renamed_surrogate():
-    """Importing from ``baybe.surrogate`` raises a warning."""
-    with pytest.warns(DeprecationWarning):
-        from baybe.surrogate import GaussianProcessSurrogate  # noqa: F401
-
-
 def test_missing_recommender_type(config):
     """Specifying a recommender without a corresponding type raises a warning."""
     dict_ = json.loads(config)
     dict_["recommender"].pop("type")
     config_without_strategy_type = json.dumps(dict_)
     with pytest.warns(DeprecationWarning):
         Campaign.from_config(config_without_strategy_type)
@@ -54,15 +40,14 @@
 RECOMMENDERS = [RandomRecommender(), FPSRecommender()]
 assert len(RECOMMENDERS) == len({rec.__class__.__name__ for rec in RECOMMENDERS})
 
 
 @pytest.mark.parametrize(
     "test_objects",
     [
-        (Strategy, {}),
         (TwoPhaseStrategy, {}),
         (SequentialStrategy, {"recommenders": RECOMMENDERS}),
         (StreamingSequentialStrategy, {"recommenders": RECOMMENDERS}),
     ],
 )
 def test_deprecated_strategies(test_objects):
     """Using the deprecated strategy classes raises a warning."""
@@ -86,15 +71,15 @@
                     "name": "missing_type",
                     "mode": "MAX",
                 }
             )
         )
 
 
-deprecated_config = """
+old_style_config = """
 {
     "parameters": [
         {
             "type": "CategoricalParameter",
             "name": "Granularity",
             "values": ["coarse", "fine", "ultra-fine"]
         }
@@ -111,22 +96,24 @@
 }
 """
 
 
 def test_deprecated_config():
     """Using the deprecated config format raises a warning."""
     with pytest.warns(UserWarning):
-        Campaign.from_config(deprecated_config)
+        Campaign.from_config(old_style_config)
 
 
 @pytest.mark.parametrize("flag", [False, True])
 def test_deprecated_campaign_tolerance_flag(flag):
     """Constructing a Campaign with the deprecated tolerance flag raises an error."""
     with pytest.raises(DeprecationError):
-        Campaign(None, None, None, numerical_measurements_must_be_within_tolerance=flag)
+        Campaign(
+            Mock(), Mock(), Mock(), numerical_measurements_must_be_within_tolerance=flag
+        )
 
 
 def test_deprecated_batch_quantity_keyword(campaign):
     """Using the deprecated batch_quantity keyword raises an error."""
     with pytest.raises(DeprecationError):
         campaign.recommend(batch_quantity=5)
 
@@ -139,8 +126,65 @@
     with pytest.raises(DeprecationError):
         TwoPhaseMetaRecommender(allow_repeated_recommendations=flag)
 
 
 def test_deprecated_strategy_campaign_flag(recommender):
     """Using the deprecated strategy keyword raises an error."""
     with pytest.raises(DeprecationError):
-        Campaign(None, None, None, strategy=recommender)
+        Campaign(Mock(), Mock(), Mock(), strategy=recommender)
+
+
+def test_deprecated_objective_class():
+    """Using the deprecated objective class raises a warning."""
+    with pytest.warns(DeprecationWarning):
+        OldObjective(mode="SINGLE", targets=[NumericalTarget(name="a", mode="MAX")])
+
+
+deprecated_objective_config = """
+{
+    "mode": "DESIRABILITY",
+    "targets": [
+        {
+            "name": "Yield",
+            "mode": "MAX",
+            "bounds": [0, 1]
+        },
+        {
+            "name": "Waste",
+            "mode": "MIN",
+            "bounds": [0, 1]
+        }
+    ],
+    "combine_func": "MEAN",
+    "weights": [1, 2]
+}
+"""
+
+
+def test_deprecated_objective_config_deserialization():
+    """The deprecated objective config format can still be parsed."""
+    expected = DesirabilityObjective(
+        targets=[
+            NumericalTarget("Yield", "MAX", bounds=(0, 1)),
+            NumericalTarget("Waste", "MIN", bounds=(0, 1)),
+        ],
+        scalarizer="MEAN",
+        weights=[1, 2],
+    )
+    actual = NewObjective.from_json(deprecated_objective_config)
+    assert expected == actual, (expected, actual)
+
+
+@pytest.mark.parametrize("acqf", ("VarUCB", "qVarUCB"))
+def test_deprecated_acqfs(acqf):
+    """Using the deprecated acqf raises a warning."""
+    with pytest.warns(DeprecationWarning):
+        SequentialGreedyRecommender(acquisition_function=acqf)
+
+    with pytest.warns(DeprecationWarning):
+        AcquisitionFunction.from_dict({"type": acqf})
+
+
+def test_deprecated_acqf_keyword(acqf):
+    """Using the deprecated keyword raises an error."""
+    with pytest.raises(DeprecationError):
+        SequentialGreedyRecommender(acquisition_function_cls="qEI")
```

### Comparing `baybe-0.8.2/tests/test_input_output.py` & `baybe-0.9.0/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_meta_recommenders.py` & `baybe-0.9.0/tests/test_meta_recommenders.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_searchspace.py` & `baybe-0.9.0/tests/test_searchspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the searchspace module."""
+
 import numpy as np
 import pandas as pd
 import pytest
 
 from baybe.constraints import (
     ContinuousLinearEqualityConstraint,
     ContinuousLinearInequalityConstraint,
@@ -68,32 +69,32 @@
         name="num_unspecified", values=[4, 5, 6]
     )
     cat_specified = CategoricalParameter(name="cat_specified", values=["a", "b", "c"])
     cat_unspecified = CategoricalParameter(
         name="cat_unspecified", values=["d", "e", "f"]
     )
 
-    all_params = [num_specified, num_unspecified, cat_specified, cat_unspecified]
+    all_params = (num_specified, num_unspecified, cat_specified, cat_unspecified)
 
     df = pd.DataFrame({param.name: param.values for param in all_params})
     searchspace = SearchSpace(
         SubspaceDiscrete.from_dataframe(df, parameters=[num_specified, cat_specified])
     )
 
     assert searchspace.type == SearchSpaceType.DISCRETE
     assert searchspace.parameters == all_params
     assert df.equals(searchspace.discrete.exp_rep)
 
 
 def test_continuous_searchspace_creation_from_bounds():
     """A purely continuous search space is created from example bounds."""
-    parameters = [
+    parameters = (
         NumericalContinuousParameter("param1", (0, 1)),
         NumericalContinuousParameter("param2", (-1, 1)),
-    ]
+    )
     bounds = pd.DataFrame({p.name: p.bounds.to_tuple() for p in parameters})
     searchspace = SearchSpace(continuous=SubspaceContinuous.from_bounds(bounds))
 
     assert searchspace.type == SearchSpaceType.CONTINUOUS
     assert searchspace.parameters == parameters
 
 
@@ -106,18 +107,18 @@
         {
             "param1": [0, 1, 2],
             "param2": [-1, 0, 1],
         }
     )
     searchspace = SearchSpace(continuous=SubspaceContinuous.from_dataframe(points))
 
-    parameters = [
+    parameters = (
         NumericalContinuousParameter("param1", (0, 2)),
         NumericalContinuousParameter("param2", (-1, 1)),
-    ]
+    )
 
     assert searchspace.type == SearchSpaceType.CONTINUOUS
     assert searchspace.parameters == parameters
 
 
 def test_invalid_constraint_parameter_combos():
     """Testing invalid constraint-parameter combinations."""
```

### Comparing `baybe-0.8.2/tests/test_streamlit.py` & `baybe-0.9.0/tests/test_streamlit.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/test_substance_parameter.py` & `baybe-0.9.0/tests/test_substance_parameter.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/validation/test_interval_validation.py` & `baybe-0.9.0/tests/validation/test_interval_validation.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/validation/test_parameter_validation.py` & `baybe-0.9.0/tests/validation/test_parameter_validation.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tests/validation/test_target_validation.py` & `baybe-0.9.0/tests/validation/test_target_validation.py`

 * *Files identical despite different names*

### Comparing `baybe-0.8.2/tox.ini` & `baybe-0.9.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 [testenv:fulltest,fulltest-py{39,310,311,312}]
 description = Run PyTest with all extra functionality
 extras = test,chem,examples,simulation,onnx
 passenv = CI
 setenv =
     SMOKE_TEST = true
+    BAYBE_TEST_ENV = FULLTEST
 commands =
     python --version
     pytest -p no:warnings --cov=baybe --durations=5 {posargs}
 
 [testenv:coretest,coretest-py{39,310,311,312}]
 description = Run PyTest with core functionality
 extras = test
 passenv = CI
 setenv =
     SMOKE_TEST = true
+    BAYBE_TEST_ENV = CORETEST
 commands =
     python --version
     pytest -p no:warnings --cov=baybe --durations=5 {posargs}
 
 [testenv:lint,lint-py{39,310,311,312}]
 description = Run linters and format checkers
 extras = lint,examples
```

