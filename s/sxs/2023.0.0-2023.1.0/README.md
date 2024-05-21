# Comparing `tmp/sxs-2023.0.0.tar.gz` & `tmp/sxs-2023.1.0.tar.gz`

## Comparing `sxs-2023.0.0.tar` & `sxs-2023.1.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.0.0/.codecov.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.0.0/CITATION.cff
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 sxs-2023.0.0/mkdocs.yml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/scripts/parse_bump_rule.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/workflows/pr_rtd_link.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/index.md -> ../README.md
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/mathematica.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/catalog.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/horizons.md
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/load.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/metadata.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/time_series.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/waveforms.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/html/main.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/images/favicon.ico
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/javascript/mathjax.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/00-Introduction.ipynb
--rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/01-Metadata.ipynb
--rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/02-Catalog.ipynb
--rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/03-Horizons.ipynb
--rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/04-Waveforms.ipynb
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/__version__.py
--rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/handlers.py
--rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/time_series.py
--rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/caltechdata/__init__.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/caltechdata/catalog.py
--rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/caltechdata/login.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/__init__.py
--rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/catalog.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/create.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/description.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/horizons/__init__.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/horizons/spec_horizons_h5.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/horizons/xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/metadata/__init__.py
--rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/metadata/metadata.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/__init__.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/bitwise.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/dicts.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/downloads.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/files.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/formats.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/inspire.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/monotonicity.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/pretty_print.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/select.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/smooth_functions.py
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/sxs_directories.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/sxs_identifiers.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/url.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/greedy_spline.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/linear_bisection.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/peak_greed.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/suppression.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/__init__.py
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/comparisons.py
--rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/conversion.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/dataset.py
--rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/horizons.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/metadata.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/waveform_amp_phase.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/waveforms.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/__init__.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/ads.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/arxiv.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/fairchild_report.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/inspire.py
--rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/journal_abbreviations.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/references.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/__init__.py
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/alignment.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/memory.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/mode_utilities.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/transformations.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_grid.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_mixin.py
--rw-r--r--   0        0        0    53506 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_modes.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_signal.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/__init__.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/lvc.py
--rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/nrar.py
--rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/spectre_cce_v1.py
--rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/__init__.py
--rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/catalog.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/creators.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/simannex.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/surrogatemodeling.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/__init__.py
--rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/deposit.py
--rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/login.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/records.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/__init__.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_catalog.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_horizons.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_loader.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_metadata.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_time_series.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_transformations.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_utilities.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_waveform_rotations.py
--rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_waveforms.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.0.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.0.0/LICENSE
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 sxs-2023.0.0/README.md
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 sxs-2023.0.0/pyproject.toml
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 sxs-2023.0.0/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.1.0/.codecov.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.1.0/CITATION.cff
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 sxs-2023.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/scripts/parse_bump_rule.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/workflows/pr_rtd_link.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/mathematica.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/catalog.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/horizons.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/load.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/metadata.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/time_series.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/waveforms.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/html/main.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/javascript/mathjax.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/00-Introduction.ipynb
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/01-Metadata.ipynb
+-rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/02-Catalog.ipynb
+-rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/03-Horizons.ipynb
+-rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/04-Waveforms.ipynb
+-rw-r--r--   0        0        0  2744681 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/05-PreprocessingForFFTs.ipynb
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/__version__.py
+-rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/handlers.py
+-rw-r--r--   0        0        0    39641 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/time_series.py
+-rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/caltechdata/__init__.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/caltechdata/catalog.py
+-rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/caltechdata/login.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/__init__.py
+-rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/catalog.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/create.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/description.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/horizons/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/horizons/spec_horizons_h5.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/horizons/xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/metadata/__init__.py
+-rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/metadata/metadata.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/__init__.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/bitwise.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/dicts.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/downloads.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/files.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/formats.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/inspire.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/monotonicity.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/pretty_print.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/select.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/smooth_functions.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/sxs_directories.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/sxs_identifiers.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/url.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/greedy_spline.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/linear_bisection.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/peak_greed.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/suppression.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/__init__.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/comparisons.py
+-rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/conversion.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/dataset.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/horizons.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/metadata.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/waveform_amp_phase.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/waveforms.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/ads.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/arxiv.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/fairchild_report.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/inspire.py
+-rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/journal_abbreviations.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/references.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/__init__.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/alignment.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/memory.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/mode_utilities.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/transformations.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_grid.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_mixin.py
+-rw-r--r--   0        0        0    56594 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_modes.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_signal.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/__init__.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/lvc.py
+-rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/nrar.py
+-rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/spectre_cce_v1.py
+-rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/__init__.py
+-rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/catalog.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/creators.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/simannex.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/surrogatemodeling.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/__init__.py
+-rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/deposit.py
+-rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/login.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/records.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_catalog.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_horizons.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_loader.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_metadata.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_time_series.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_transformations.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_utilities.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_waveform_rotations.py
+-rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_waveforms.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.1.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.1.0/LICENSE
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 sxs-2023.1.0/README.md
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 sxs-2023.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9329 2020-02-02 00:00:00.000000 sxs-2023.1.0/PKG-INFO
```

### Comparing `sxs-2023.0.0/mkdocs.yml` & `sxs-2023.1.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   - Home: "index.md"
   - Tutorials:
     - "tutorials/00-Introduction.ipynb"
     - "tutorials/02-Catalog.ipynb"
     - "tutorials/01-Metadata.ipynb"
     - "tutorials/03-Horizons.ipynb"
     - "tutorials/04-Waveforms.ipynb"
+    - "tutorials/05-PreprocessingForFFTs.ipynb"
   - API:
     - "Load": "api/load.md"
     - "Catalog": "api/catalog.md"
     - "Metadata": "api/metadata.md"
     - "Time Series": "api/time_series.md"
     - "Horizons": "api/horizons.md"
     - "Waveforms": "api/waveforms.md"
```

### Comparing `sxs-2023.0.0/.github/workflows/build.yml` & `sxs-2023.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/mathematica.md` & `sxs-2023.1.0/docs/mathematica.md`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/images/favicon.ico` & `sxs-2023.1.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/tutorials/00-Introduction.ipynb` & `sxs-2023.1.0/docs/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/tutorials/01-Metadata.ipynb` & `sxs-2023.1.0/docs/tutorials/01-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/tutorials/02-Catalog.ipynb` & `sxs-2023.1.0/docs/tutorials/02-Catalog.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/tutorials/03-Horizons.ipynb` & `sxs-2023.1.0/docs/tutorials/03-Horizons.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/docs/tutorials/04-Waveforms.ipynb` & `sxs-2023.1.0/docs/tutorials/04-Waveforms.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/__init__.py` & `sxs-2023.1.0/sxs/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/handlers.py` & `sxs-2023.1.0/sxs/handlers.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/time_series.py` & `sxs-2023.1.0/sxs/time_series.py`

 * *Files 20% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     def __array_finalize__(self, obj):
         import copy
         if obj is None:
             return
         # # Since ndarray.__array_finalize__ is None, we skip this in its direct descendents:
         # super().__array_finalize__(obj)
-        self._metadata = copy.copy(getattr(self, '_metadata', getattr(obj, '_metadata', {})))
+        self._metadata = copy.copy(getattr(self, "_metadata", getattr(obj, "_metadata", {})))
         if "time" not in self._metadata:
             self._metadata["time"] = None  # Placeholder about to be updated
 
     def _slice(self, key):
         """Slice this object
 
         This is the core function used by __getitem__, and returns not only the sliced
@@ -236,15 +236,15 @@
                 ) from e
             new_time_axis = self.time_axis
 
         # Create the new sliced object along with its metadata
         if time_key is not None:
             new_time = self.time[time_key]
         metadata = self._metadata.copy()
-        metadata.update(**getattr(new_data, '_metadata', {}))
+        metadata.update(**getattr(new_data, "_metadata", {}))
         metadata["time"] = new_time
         metadata["time_axis"] = new_time_axis
 
         return type(self)(new_data, **metadata), time_key
 
     def __getitem__(self, key):
         """Extract a slice of this object
@@ -615,47 +615,340 @@
         kw = kwargs.copy()
         kw.update({"axis": self.time_axis})
         return xor(self.ndarray, reverse=reverse, preserve_dtype=preserve_dtype, **kw)
 
     def truncate(self, abs_tolerance):
         """Truncate the precision of this object's `data` in place
 
-        This function sets bits in the array data to 0 when they have lower
-        significance than the number given as or returned by `abs_tolerance`.  This is
-        a useful step in compressing data — though it is obviously lossy.
+        This function sets bits in the array data to 0 when they have
+        lower significance than the number given as or returned by
+        `abs_tolerance`.  This is a useful step in compressing data —
+        though it is obviously lossy.
 
         Parameters
         ----------
         abs_tolerance : {callable, float, array-like}
-            If callable, it is called with this object as the parameter, and the
-            returned value is treated as a float or array-like would be.  Floats are
-            simply treated as a uniform absolute tolerance to be applied at all times.
-            Array-like objects must broadcast against this array, and each element is
-            treated as the absolute tolerance for all the elements it broadcasts to.
+            If callable, it is called with this object as the
+            parameter, and the returned value is treated as a float or
+            array-like would be.  Floats are simply treated as a
+            uniform absolute tolerance to be applied at all times.
+            Array-like objects must broadcast against this array, and
+            each element is treated as the absolute tolerance for all
+            the elements it broadcasts to.
 
         Returns
         -------
         None
-            This value is returned to serve as a reminder that this function operates
-            in place.
+            This value is returned to serve as a reminder that this
+            function operates in place.
 
         Notes
         -----
-        The effect is achieved by multiplying the array's data by the same power of 2
-        that would be required to bring the `abs_tolerance` to between 1 and 2.  Thus,
-        all digits less significant than 1 are less significant than `abs_tolerance` —
-        meaning that we can apply the standard `round` routine to set these digits to
-        0.  We then divide by that same power of 2 to bring the array data back to
-        nearly its original value.  By working with powers of 2, we ensure that the 0s
-        at the intermediate stage are represented as 0 bits in the final result.
+        The effect is achieved by multiplying the array's data by the
+        same power of 2 that would be required to bring the
+        `abs_tolerance` to between 1 and 2.  Thus, all digits less
+        significant than 1 are less significant than `abs_tolerance` —
+        meaning that we can apply the standard `round` routine to set
+        these digits to 0.  We then divide by that same power of 2 to
+        bring the array data back to nearly its original value.  By
+        working with powers of 2, we ensure that the 0s at the
+        intermediate stage are represented as 0 bits in the final
+        result.
 
-        For floats and array-like objects, all values must be strictly positive, or
-        `inf` or `nan` will result.
+        For floats and array-like objects, all values must be strictly
+        positive, or `inf` or `nan` will result.
 
         """
         if callable(abs_tolerance):
             abs_tolerance = abs_tolerance(self)
         power_of_2 = (2.0 ** np.floor(-np.log2(abs_tolerance)))
         ndarray = self.ndarray
         ndarray *= power_of_2
         np.round(ndarray, out=ndarray)
         ndarray /= power_of_2
+
+    def taper(self, t1, t2, y1=0, y2=1, *, transition_type="smooth"):
+        """Smoothly taper (or transition) the data
+
+        This is essentially half of a standard window function, using
+        the C^∞ "compactified tanh" transition function.  By default,
+        this function smoothly transitions the data from 0 before `t1`
+        to the input data after `t2`, which is useful to prevent Gibbs
+        effects caused by a sudden "turn on" of a signal.  By swapping
+        the values of `y1` and `y2`, the transition can be reversed.
+
+        Parameters
+        ----------
+        t1 : float
+            Time before which the output will equal `y1` times the
+            data.
+        t2 : float
+            Time after which the output will equal `y2` times the
+            data.
+        y1 : float, optional
+            Value before `t1`.  Default value is 0.
+        y2 : float, optional
+            Value after `t2`.  Default value is 1.
+        transition_type : str, optional
+            Type of transition to apply.  Default value is `"smooth"`,
+            which corresponds to the C^∞ bump (compactified tanh)
+            function.  The other option is `"cosine"`, which
+            corresponds to the Tukey (cosine-taper) function.
+
+        Returns
+        -------
+        TimeSeries
+            New object with transitioned data.
+
+        See Also
+        --------
+        transition_to_constant : Smoothly transition to a constant
+            value
+        sxs.utilities.transition_function : Function that does the
+            work
+
+        """
+        from .utilities import transition_function
+        t2 = t2 or self.time[-1]
+        if transition_type == "smooth":
+            τ = transition_function(self.time, t1, t2, y1, y2)
+        elif transition_type == "cosine":
+            τ = np.empty_like(self.time)
+            τ[self.time <= t1] = y1
+            τ[(self.time > t1) & (self.time < t2)] = (y1 + y2) / 2 - (y2 - y1) / 2 * np.cos(np.pi * (self.time[(self.time > t1) & (self.time < t2)] - t1) / (t2 - t1))
+            τ[self.time >= t2] = y2
+        else:
+            raise ValueError(f"Unknown transition type {transition_type=}")
+        data = np.moveaxis(self.ndarray.copy(), self.time_axis, -1)
+        data = data * τ
+        data = np.moveaxis(data, -1, self.time_axis)
+        return type(self)(data, **self._metadata.copy())
+
+    def transition_to_constant(self, t1, t2=None):
+        """Smoothly transition from the data to a constant
+
+        This function produces a copy of the input, where the data is
+        smoothly transitioned from the value at `t1` to a constant
+        value at `t2` (which is the last time step if not given).  The
+        precise value of this constant will depend on the behavior of
+        the data between `t1` and `t2`.
+
+        Parameters
+        ----------
+        t1 : float
+            Time after which the output will equal the input data.
+        t2 : float, optional
+            Time after which the output will be constant.  Default
+            value is the last time step.
+
+        Returns
+        -------
+        TimeSeries
+            New object with transitioned data.
+
+        See Also
+        --------
+        taper : Smoothly transition the data
+        sxs.utilities.transition_to_constant : Function that does
+            the work
+        
+        """
+        from .utilities import transition_to_constant_inplace
+        t2 = t2 or self.time[-1]
+        if self.time_axis != 0:
+            data = np.moveaxis(self.ndarray.copy(), self.time_axis, 0)
+        else:
+            data = self.ndarray.copy()
+        data = transition_to_constant_inplace(data, self.time, t1, t2)
+        if self.time_axis != 0:
+            data = np.moveaxis(data, 0, self.time_axis)
+        return type(self)(data, **self._metadata.copy())
+    
+    def window(self, t1, t2, t3, t4, y1=0, y23=1, y4=None, *, window_type="smooth"):
+        """Window the data smoothly
+
+        This function creates a copy of the input and, by default,
+        zeroes it outside of the times `t1` and `t4` while reproducing
+        it precisely between `t2` and `t3`.
+
+        Parameters
+        ----------
+        t1 : float
+            Time before which the output will be multiplied by `y1`.
+        t2 : float
+            Time after which the output will be multiplied by `y23`.
+        t3 : float
+            Time before which the output will be multiplied by `y23`.
+        t4 : float
+            Time after which the output will be multiplied by `y4`.
+        y1 : float, optional
+            Multiplicative value before `t1`.  Default value is 0.
+        y23 : float, optional
+            Multiplicative value between `t2` and `t3`.  Default value
+            is 1.
+        y4 : float, optional
+            Multiplicative value after `t4`.  Default value is `y1`.
+        window_type : str, optional
+            Type of window to apply.  Default value is `"smooth"`,
+            which corresponds to the C^∞ bump (compactified tanh)
+            function.  The other option is `"cosine"`, which
+            corresponds to the Tukey (cosine-tapered) window.
+
+        Returns
+        -------
+        TimeSeries
+            New object with windowed data.
+
+        See Also
+        --------
+        sxs.utilities.bump_function : Function that does the work
+
+        """
+        from .utilities import bump_function
+        y4 = y4 or y1
+        if window_type == "smooth":
+            τ = bump_function(self.time, t1, t2, t3, t4, y1, y23, y4)
+        elif window_type == "cosine":
+            t = self.time
+            τ = np.empty_like(t)
+            τ[t <= t1] = y1
+            τ[(t > t1) & (t < t2)] = (y1 + y23) / 2 - (y23 - y1) / 2 * np.cos(np.pi * (t[(t > t1) & (t < t2)] - t1) / (t2 - t1))
+            τ[(t >= t2) & (t <= t3)] = y23
+            τ[(t > t3) & (t < t4)] = (y23 + y4) / 2 - (y4 - y23) / 2 * np.cos(np.pi * (t[(t > t3) & (t < t4)] - t3) / (t4 - t3))
+            τ[t >= t4] = y4
+        else:
+            raise ValueError(f"Unknown window type {window_type=}")
+        data = np.moveaxis(self.ndarray.copy(), self.time_axis, -1)
+        data = data * τ
+        data = np.moveaxis(data, -1, self.time_axis)
+        return type(self)(data, **self._metadata.copy())
+    
+    def pad(self, pad_length=None, mode="edge", **kwargs):
+        """Pad the data values along the time axis
+        
+        This function is based on `numpy.pad`, but the `pad_length`
+        argument is given in units of time, rather than numbers of
+        elements, and the `mode` argument defaults to `"edge"`.
+
+        As with `numpy.pad`, the `pad_length` argument may be a single
+        number, a tuple with one element, or a tuple with two
+        elements.  For just a single number or tuple with one element,
+        the padding is applied symmetrically to both ends of the data.
+        Unlike `numpy.pad`, there may only be two elements of this
+        tuple; padding other dimensions is not allowed.
+
+        Parameters
+        ----------
+        pad_length : {None, float, tuple}
+            Amount of time to pad on both sides (for a single float)
+            or the beginning and end (for a tuple) of the data.  By
+            default, the full length of the input data is added to
+            both the beginning and end of the data; that is, the
+            length of the data is tripled.
+        mode : str, optional
+            Padding mode.  Default value is `"edge"`.
+        kwargs : dict
+            Additional keyword arguments to pass to `numpy.pad`.
+
+        Returns
+        -------
+        TimeSeries
+            New object with padded data.
+
+        See Also
+        --------
+        numpy.pad : Similar function with padding in number of
+            elements, rather than time, and a different default
+            `mode`.
+        
+        """
+        if pad_length is None:
+            pad_length = self.time[-1] - self.time[0]
+        pad_length = np.asarray(pad_length)
+        if pad_length.shape == ():
+            pad_length = np.array([pad_length, pad_length])
+        elif pad_length.shape == (1,):
+            pad_length = np.array([pad_length[0], pad_length[0]])
+        elif pad_length.shape != (2,):
+            raise ValueError(
+                f"Input `pad_length` must be a scalar, a tuple with one element, "
+                f"or a tuple with two elements; it has shape {pad_length.shape}."
+            )
+        dt0 = self.time[1] - self.time[0]
+        dt1 = self.time[-1] - self.time[-2]
+        pad_width0 = int(np.ceil(pad_length[0] / dt0))
+        pad_width1 = int(np.ceil(pad_length[1] / dt1))
+        pad_width = list(
+            (0, 0) if self.time_axis != i else (pad_width0, pad_width1)
+            for i in range(self.ndarray.ndim)
+        )
+        data = np.pad(self.ndarray, pad_width, mode, **kwargs)
+        metadata = self._metadata.copy()
+        metadata["time"] = np.concatenate(
+            (
+                self.time[0] - np.arange(pad_width0, 0, -1) * dt0,
+                self.time,
+                self.time[-1] + np.arange(1, pad_width1+1) * dt1
+            )
+        )
+        return type(self)(data, **metadata)
+
+    def line_subtraction(self, treat_as_zero="begin"):
+        """Subtract a linear function of time from the data
+
+        This is very similar to the `detrend` function found in the
+        signal-processing literature and in SciPy and MATLAB, for
+        example, except that rather than fitting a line to all of the
+        data (which is more appropriate for noisy data), this function
+        subtracts the line connecting the two ends (first and last
+        time steps) of the data.  This ensures that there is no
+        discontinuity in the data at the boundaries, which is not
+        guaranteed by the usual `detrend` functions.
+
+        Parameters
+        ----------
+        treat_as_zero : str, optional
+            Whether to treat the data at the boundaries as zero.
+            Default value is `"begin"`, meaning that we pretend that
+            the data at the beginning of the time array is oscillating
+            around zero, so we can treat it as if it *is* zero.  If
+            the early data has already been tapered, it will probably
+            already be zero, so this shouldn't matter.  In that case,
+            `"neither"` would also be correct.  The option `"end"` is
+            also accepted, but this will be less likely to be needed.
+
+        Returns
+        -------
+        TimeSeries
+            New object with the linear function of time subtracted.
+
+        Notes
+        -----
+        There is a minor subtlety in the implementation of this
+        function.  It is not quite enough to simply subtract the line
+        connecting the first and last data points.  The discrete
+        Fourier transform implicitly assumes that the data is
+        periodic, so that the line should connect the first data point
+        to *one beyond the last data point*.  It is not generally
+        clear how to define that, but assuming that the data has
+        roughly settled down to be roughly constant by the end, we can
+        say that the line should connect `(time[0], data[0])` to
+        `(time[-1]+dt, data[-1])`, where `dt` is the time-step size.
+        This is the approach taken here.  Even this is only
+        approximate, but typically this should be such a tiny effect
+        as to not matter at all, though it could improve results for
+        very short or highly changing time series.
+
+        """
+        N = self.n_times
+        data = np.moveaxis(self.ndarray.copy(), self.time_axis, -1)
+        data_begin = 0 if treat_as_zero == "begin" else data[..., [0]]
+        data_end = 0 if treat_as_zero == "end" else data[..., [-1]]
+        line = (
+            data_begin
+            + (data_end - data_begin)
+            * ((self.time - self.time[0]) / (self.time[-1] - self.time[0]))
+            * ((N - 1) / N)
+        )
+        data -= line
+        data = np.moveaxis(data, -1, self.time_axis)
+        return type(self)(data, **self._metadata.copy())
```

### Comparing `sxs-2023.0.0/sxs/caltechdata/__init__.py` & `sxs-2023.1.0/sxs/caltechdata/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/caltechdata/catalog.py` & `sxs-2023.1.0/sxs/caltechdata/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/caltechdata/login.py` & `sxs-2023.1.0/sxs/caltechdata/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/catalog/catalog.py` & `sxs-2023.1.0/sxs/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/catalog/create.py` & `sxs-2023.1.0/sxs/catalog/create.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/catalog/description.py` & `sxs-2023.1.0/sxs/catalog/description.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/horizons/__init__.py` & `sxs-2023.1.0/sxs/horizons/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/horizons/spec_horizons_h5.py` & `sxs-2023.1.0/sxs/horizons/spec_horizons_h5.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/horizons/xor_multishuffle_bzip2.py` & `sxs-2023.1.0/sxs/horizons/xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/metadata/metadata.py` & `sxs-2023.1.0/sxs/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/__init__.py` & `sxs-2023.1.0/sxs/utilities/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 from .select import select_by_path_component
 from .formats import file_format
 from .pretty_print import fit_to_console
 from .files import (
     md5checksum, lock_file_manager, find_simulation_directories, find_files
 )
 from .dicts import KeyPassingDict
+from .smooth_functions import (
+    transition_function, transition_function_inplace,
+    transition_function_derivative, transition_function_derivative_inplace,
+    transition_to_constant, transition_to_constant_inplace,
+    bump_function, bump_function_inplace
+)
 
 
 def version_info():
     """Find all relevant package versions
 
     This function attempts to import each of the various packages relevant to this
     package — such as numpy, quaternionic, etc. — and returns a dictionary mapping
```

### Comparing `sxs-2023.0.0/sxs/utilities/bitwise.py` & `sxs-2023.1.0/sxs/utilities/bitwise.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/dicts.py` & `sxs-2023.1.0/sxs/utilities/dicts.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/downloads.py` & `sxs-2023.1.0/sxs/utilities/downloads.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/files.py` & `sxs-2023.1.0/sxs/utilities/files.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/formats.py` & `sxs-2023.1.0/sxs/utilities/formats.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/inspire.py` & `sxs-2023.1.0/sxs/utilities/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/monotonicity.py` & `sxs-2023.1.0/sxs/utilities/monotonicity.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/pretty_print.py` & `sxs-2023.1.0/sxs/utilities/pretty_print.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/select.py` & `sxs-2023.1.0/sxs/utilities/select.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/smooth_functions.py` & `sxs-2023.1.0/sxs/utilities/smooth_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from .. import jit
+from . import jit
 
 
 def transition_function(x, x0, x1, y0=0, y1=1, msquared=3):
     """Evaluate a C^∞ function transitioning from `y0` to `y1` in the range (`x0`, `x1`).
 
     This is a special type of [sigmoid
     function](https://en.wikipedia.org/wiki/Sigmoid_function) in which
```

### Comparing `sxs-2023.0.0/sxs/utilities/sxs_directories.py` & `sxs-2023.1.0/sxs/utilities/sxs_directories.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/sxs_identifiers.py` & `sxs-2023.1.0/sxs/utilities/sxs_identifiers.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/url.py` & `sxs-2023.1.0/sxs/utilities/url.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/decimation/__init__.py` & `sxs-2023.1.0/sxs/utilities/decimation/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/decimation/greedy_spline.py` & `sxs-2023.1.0/sxs/utilities/decimation/greedy_spline.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/decimation/linear_bisection.py` & `sxs-2023.1.0/sxs/utilities/decimation/linear_bisection.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/decimation/peak_greed.py` & `sxs-2023.1.0/sxs/utilities/decimation/peak_greed.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/decimation/suppression.py` & `sxs-2023.1.0/sxs/utilities/decimation/suppression.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/__init__.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/comparisons.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/comparisons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/conversion.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/conversion.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/dataset.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/dataset.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/horizons.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/metadata.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/waveform_amp_phase.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/waveform_amp_phase.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/lvcnr/waveforms.py` & `sxs-2023.1.0/sxs/utilities/lvcnr/waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/references/ads.py` & `sxs-2023.1.0/sxs/utilities/references/ads.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/references/arxiv.py` & `sxs-2023.1.0/sxs/utilities/references/arxiv.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/references/fairchild_report.py` & `sxs-2023.1.0/sxs/utilities/references/fairchild_report.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/references/inspire.py` & `sxs-2023.1.0/sxs/utilities/references/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/utilities/references/journal_abbreviations.py` & `sxs-2023.1.0/sxs/utilities/references/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/__init__.py` & `sxs-2023.1.0/sxs/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/alignment.py` & `sxs-2023.1.0/sxs/waveforms/alignment.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/memory.py` & `sxs-2023.1.0/sxs/waveforms/memory.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/mode_utilities.py` & `sxs-2023.1.0/sxs/waveforms/mode_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/transformations.py` & `sxs-2023.1.0/sxs/waveforms/transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/waveform_mixin.py` & `sxs-2023.1.0/sxs/waveforms/waveform_mixin.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/waveform_modes.py` & `sxs-2023.1.0/sxs/waveforms/waveform_modes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1186,14 +1186,89 @@
         """
         frame = self.coprecessing_frame(rough_direction, rough_direction_index)
         w = self.rotate(frame)
         w._metadata["frame_type"] = "coprecessing"
         w._metadata["frame"] = frame
         return w
 
+    def preprocess(self, t1=0, t2=500, t3=None, t4=None, dt=None, **kwargs):
+        """Preprocess the data to prepare for FFT
+
+        This function is a convenience function that applies a series
+        of common preprocessing steps to the data before Fourier
+        transforming it.  The steps are:
+        
+            1. `interpolate`
+            2. `taper`
+            3. `transition_to_constant`
+            4. `pad`
+            5. `line_subtraction`
+
+        Parameters
+        ----------
+        t1 : float, optional
+            Time before which the data will be zeroed, after which the
+            taper will begin.  Default is 0 (not the first time step,
+            but t=0).
+        t2 : float, optional
+            Time at which the tapering will end.  Default is 500.
+        t3 : float, optional
+            Time at which the transition to a constant value will
+            begin.  Default is max_norm_time+100.
+        t4 : float, optional
+            Time after which the data will be constant.  Default is
+            max_norm_time+200.
+        dt : float, optional
+            Time step for the new time array.  Default is the smallest
+            time step in the input data.
+
+        Keyword Parameters
+        ------------------
+        evaluate_directions : array_like, optional
+            Directions at which to evaluate the waveform.  Default is
+            `None`, in which case the waveform modes are
+            pre-processed.  See `evaluate` for more information on the
+            meaning of other possible input values.
+        pad_length : tuple, optional
+            Length of padding to apply to the data.  Default option
+            will triple the length of the data.  (See `pad` for more
+            information.)
+        pad_mode : str, optional
+            Mode of padding.  Default value is `"edge"`.  (See `pad`
+            for more information.)
+        treat_as_zero : str, optional
+            How to treat the data at the boundaries.  Default value is
+            `"begin"`.  (See `line_subtraction` for more information.)
+        
+        All other keyword arguments are passed to `numpy.pad`.
+
+        Returns
+        -------
+        TimeSeries
+            New object with preprocessed data.
+
+        """
+        # Process arguments
+        t3 = t3 or self.max_norm_time() + 100
+        t4 = t4 or self.max_norm_time() + 200
+        dt = dt or np.min(np.diff(self.time))
+        evaluate_directions = kwargs.pop("evaluate_directions", None)
+        pad_length = kwargs.pop("pad_length", None)
+        pad_mode = kwargs.pop("pad_mode", "edge")
+        treat_as_zero = kwargs.pop("treat_as_zero", "begin")
+
+        result = self.interpolate(np.arange(self.time[0], self.time[-1], dt))
+        if evaluate_directions is not None:
+            result = result.evaluate(evaluate_directions)
+        result = result.taper(t1, t2)
+        result = result.transition_to_constant(t3, t4)
+        result = result.pad(pad_length, mode=pad_mode, **kwargs)
+        result = result.line_subtraction(treat_as_zero=treat_as_zero)
+        return result
+
 
 class WaveformModesDict(MutableMapping, WaveformModes):
     """A dictionary-like class for storing waveform modes
 
     This class is a subclass of `MutableMapping`, which is essentially
     a `dict`.  The only difference is that this class silently passes
     `__delitem__`, and disables adding keys that aren't within the
```

### Comparing `sxs-2023.0.0/sxs/waveforms/format_handlers/lvc.py` & `sxs-2023.1.0/sxs/waveforms/format_handlers/lvc.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/format_handlers/nrar.py` & `sxs-2023.1.0/sxs/waveforms/format_handlers/nrar.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py` & `sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py` & `sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/waveforms/format_handlers/spectre_cce_v1.py` & `sxs-2023.1.0/sxs/waveforms/format_handlers/spectre_cce_v1.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/__init__.py` & `sxs-2023.1.0/sxs/zenodo/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/catalog.py` & `sxs-2023.1.0/sxs/zenodo/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/creators.py` & `sxs-2023.1.0/sxs/zenodo/creators.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/simannex.py` & `sxs-2023.1.0/sxs/zenodo/simannex.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/surrogatemodeling.py` & `sxs-2023.1.0/sxs/zenodo/surrogatemodeling.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/api/deposit.py` & `sxs-2023.1.0/sxs/zenodo/api/deposit.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/api/login.py` & `sxs-2023.1.0/sxs/zenodo/api/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/sxs/zenodo/api/records.py` & `sxs-2023.1.0/sxs/zenodo/api/records.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/conftest.py` & `sxs-2023.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_catalog.py` & `sxs-2023.1.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_horizons.py` & `sxs-2023.1.0/tests/test_horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_loader.py` & `sxs-2023.1.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_metadata.py` & `sxs-2023.1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_time_series.py` & `sxs-2023.1.0/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_transformations.py` & `sxs-2023.1.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_utilities.py` & `sxs-2023.1.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_waveform_rotations.py` & `sxs-2023.1.0/tests/test_waveform_rotations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/tests/test_waveforms.py` & `sxs-2023.1.0/tests/test_waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/.gitignore` & `sxs-2023.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/LICENSE` & `sxs-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/README.md` & `sxs-2023.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Test Status](https://github.com/sxs-collaboration/sxs/workflows/tests/badge.svg)](https://github.com/sxs-collaboration/sxs/actions)
 [![Documentation Status](https://readthedocs.org/projects/sxs/badge/?version=main)](https://sxs.readthedocs.io/en/main/?badge=main)
 [![PyPI Version](https://img.shields.io/pypi/v/sxs?color=)](https://pypi.org/project/sxs/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/sxs.svg?color=)](https://anaconda.org/conda-forge/sxs)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sxs-collaboration/sxs/blob/main/LICENSE)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/moble/sxs_notebooks/master)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/moble/sxs_notebooks/main)
 
 
 # Simulating eXtreme Spacetimes package
 
 The `sxs` python package provides a high-level interface for using data
 produced by the SXS collaboration.  In particular, the function `sxs.load` can
 automatically find, download, and load data, returning objects that provide
@@ -19,14 +19,16 @@
 
   * Catalog — a listing of all data produced by the SXS collaboration
   * Metadata — data describing the simulation parameters
   * Horizons — time-series data describing the apparent horizons
   * Waveforms — time-series data describing the extrapolated gravitational-wave
     modes
 
+The complete documentation is [hosted here](https://sxs.readthedocs.io/en/stable/).
+
 
 ## Installation
 
 Because this package is pure python code, installation is very simple.  In
 particular, with a reasonably modern installation, you can just run a command
 like
 
@@ -72,15 +74,15 @@
 documentation](https://sxs.readthedocs.io/en/main/api/sxs.utilities.sxs_directories/#sxsutilitiessxs_directoriessxs_directory)
 for details.
 
 
 ## Usage
 
 An extensive demonstration of this package's capabilities is available
-[here](https://mybinder.org/v2/gh/moble/sxs_notebooks/master), in the form of
+[here](https://mybinder.org/v2/gh/moble/sxs_notebooks/main), in the form of
 interactive jupyter notebooks that are actually running this code and some
 pre-downloaded data.  The following is just a very brief overview of the `sxs`
 package's main components.
 
 There are four important objects to understand in this package:
 
 ```python
```

### Comparing `sxs-2023.0.0/pyproject.toml` & `sxs-2023.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sxs-2023.0.0/PKG-INFO` & `sxs-2023.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sxs
-Version: 2023.0.0
+Version: 2023.1.0
 Summary: Interface to data produced by the Simulating eXtreme Spacetimes collaboration
 Project-URL: Homepage, https://github.com/sxs-collaboration/sxs
 Project-URL: Documentation, https://sxs.readthedocs.io/
 Author-email: Michael Boyle <michael.oliver.boyle@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Michael Boyle
@@ -70,15 +70,15 @@
 Description-Content-Type: text/markdown
 
 [![Test Status](https://github.com/sxs-collaboration/sxs/workflows/tests/badge.svg)](https://github.com/sxs-collaboration/sxs/actions)
 [![Documentation Status](https://readthedocs.org/projects/sxs/badge/?version=main)](https://sxs.readthedocs.io/en/main/?badge=main)
 [![PyPI Version](https://img.shields.io/pypi/v/sxs?color=)](https://pypi.org/project/sxs/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/sxs.svg?color=)](https://anaconda.org/conda-forge/sxs)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sxs-collaboration/sxs/blob/main/LICENSE)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/moble/sxs_notebooks/master)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/moble/sxs_notebooks/main)
 
 
 # Simulating eXtreme Spacetimes package
 
 The `sxs` python package provides a high-level interface for using data
 produced by the SXS collaboration.  In particular, the function `sxs.load` can
 automatically find, download, and load data, returning objects that provide
@@ -90,14 +90,16 @@
 
   * Catalog — a listing of all data produced by the SXS collaboration
   * Metadata — data describing the simulation parameters
   * Horizons — time-series data describing the apparent horizons
   * Waveforms — time-series data describing the extrapolated gravitational-wave
     modes
 
+The complete documentation is [hosted here](https://sxs.readthedocs.io/en/stable/).
+
 
 ## Installation
 
 Because this package is pure python code, installation is very simple.  In
 particular, with a reasonably modern installation, you can just run a command
 like
 
@@ -143,15 +145,15 @@
 documentation](https://sxs.readthedocs.io/en/main/api/sxs.utilities.sxs_directories/#sxsutilitiessxs_directoriessxs_directory)
 for details.
 
 
 ## Usage
 
 An extensive demonstration of this package's capabilities is available
-[here](https://mybinder.org/v2/gh/moble/sxs_notebooks/master), in the form of
+[here](https://mybinder.org/v2/gh/moble/sxs_notebooks/main), in the form of
 interactive jupyter notebooks that are actually running this code and some
 pre-downloaded data.  The following is just a very brief overview of the `sxs`
 package's main components.
 
 There are four important objects to understand in this package:
 
 ```python
```

