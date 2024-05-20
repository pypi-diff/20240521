# Comparing `tmp/pydra_nireports-0.1.0.tar.gz` & `tmp/pydra_nireports-0.1.1.tar.gz`

## Comparing `pydra_nireports-0.1.0.tar` & `pydra_nireports-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,83 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/.coveragerc
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/.flake8
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/codecov.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/report_progress.py
--rw-r--r--   0        0        0    13845 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/.github/workflows/ci-cd.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/docs/make.bat
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/generate
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/requirements.txt
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/package.yaml
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/comp_cor_variance_plot.yaml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/comp_cor_variance_plot_callables.py
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/confounds_correlation_plot.yaml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/confounds_correlation_plot_callables.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/dwi_heatmap.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/dwi_heatmap_callables.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/fmri_summary.yaml
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/fmri_summary_callables.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_contours.yaml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_contours_callables.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_mosaic.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_mosaic_callables.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_spikes.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_spikes_callables.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/simple_before_after_rpt.yaml
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/simple_before_after_rpt_callables.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/pydra/tasks/nireports/_version.py
--rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/tools/increment_tool_version.py
--rwxr-xr-x   0        0        0     1392 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/tools/rename_template.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/tools/requirements.txt
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/.gitignore
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/AUTHORS
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/NOTICE
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/README.rst
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 pydra_nireports-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/.flake8
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/codecov.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/report_progress.py
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/.github/workflows/ci-cd.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/docs/make.bat
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/generate
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/requirements.txt
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/package.yaml
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/comp_cor_variance_plot.yaml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/comp_cor_variance_plot_callables.py
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/confounds_correlation_plot.yaml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/confounds_correlation_plot_callables.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/dwi_heatmap.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/dwi_heatmap_callables.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/fmri_summary.yaml
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/fmri_summary_callables.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_contours.yaml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_contours_callables.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_mosaic.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_mosaic_callables.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_spikes.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_spikes_callables.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/simple_before_after_rpt.yaml
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/simple_before_after_rpt_callables.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/__init__.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/_post_release.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/_version.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/dmri/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/dmri/dwi_heatmap.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/dmri/tests/conftest.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/dmri/tests/test_dwiheatmap.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/fmri/__init__.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/fmri/fmri_summary.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/fmri/tests/conftest.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/fmri/tests/test_fmrisummary.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/__init__.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/plot_contours.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/plot_mosaic.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/plot_spikes.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/tests/conftest.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/tests/test_plotcontours.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/tests/test_plotmosaic.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/mosaic/tests/test_plotspikes.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/nuisance/__init__.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/nuisance/comp_cor_variance_plot.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/nuisance/confounds_correlation_plot.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/nuisance/tests/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/nuisance/tests/test_compcorvarianceplot.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/nuisance/tests/test_confoundscorrelationplot.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/reporting/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/reporting/base/__init__.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/reporting/base/simple_before_after_rpt.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/reporting/base/tests/conftest.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/interfaces/reporting/base/tests/test_simplebeforeafterrpt.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/nipype_ports/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/nipype_ports/utils/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/nipype_ports/utils/filemanip.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/__init__.py
+-rw-r--r--   0        0        0    15101 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/mosaic.py
+-rw-r--r--   0        0        0    22048 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/nuisance.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/utils.py
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/xca.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/modality/__init__.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/modality/dwi.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/reportlets/modality/func.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/tools/__init__.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pydra/tasks/nireports/tools/timeseries.py
+-rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/tools/increment_tool_version.py
+-rwxr-xr-x   0        0        0     1392 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/tools/rename_template.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/tools/requirements.txt
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/.gitignore
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/AUTHORS
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/NOTICE
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/README.rst
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 pydra_nireports-0.1.1/PKG-INFO
```

### Comparing `pydra_nireports-0.1.0/report_progress.py` & `pydra_nireports-0.1.1/report_progress.py`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/.github/workflows/ci-cd.yaml` & `pydra_nireports-0.1.1/.github/workflows/ci-cd.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     - name: Set up Python
       uses: actions/setup-python@v5
 
     - name: Install build dependencies
       run: python -m pip install --upgrade pip
 
     - name: Install requirements
-      run: python -m pip install ./related-packages/fileformats -r ./nipype-auto-conv/requirements.txt
+      run: python -m pip install -r ./nipype-auto-conv/requirements.txt
 
     - name: Run automatic Nipype > Pydra conversion
       run: ./nipype-auto-conv/generate
 
     - uses: actions/upload-artifact@v4
       with:
         name: converted-nipype
-        path: pydra/tasks/nireports/auto
+        path: pydra/tasks/nireports
 
   devcheck:
     needs: [nipype-conv]
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.8', '3.11']  # Check oldest and newest versions
@@ -68,19 +68,19 @@
       if: github.event_name == 'repository_dispatch'
       run: git checkout $(git tag -l | grep 'v.*' | tail -n 1 | awk -F post '{print $1}')
 
     - name: Download tasks converted from Nipype 
       uses: actions/download-artifact@v4
       with:
         name: converted-nipype
-        path: pydra/tasks/nireports/auto
+        path: pydra/tasks/nireports
 
     - name: Strip auto package from gitignore so it is included in package
       run: |
-        sed -i '/\/pydra\/tasks\/nireports\/auto/d' .gitignore
+        sed -i '/\/pydra\/tasks\/nireports/d' .gitignore
         sed -i '/^_version.py/d' .gitignore
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
@@ -93,21 +93,17 @@
         pushd $HOME
         pip install ${{ matrix.pydra }}
         popd
         python -c "import pydra as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
 
     - name: Install task package
       run: |
-        pip install ${{ matrix.pip-flags }} "./related-packages/fileformats[dev]"
-        pip install ${{ matrix.pip-flags }} "related-packages/fileformats-extras[dev]"
         pip install ${{ matrix.pip-flags }} ".[dev]"
         python -c "import pydra.tasks.nireports as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
         python -c "import pydra as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
-        python -c "import fileformats.medimage_nireports as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
-        python -c "import fileformats.extras.medimage_nireports as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
 
   test:
     needs: [nipype-conv]
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.8', '3.11']
@@ -120,156 +116,59 @@
 
     - name: Checkout repo
       uses: actions/checkout@v4
 
     - name: Revert version to most recent version tag on Nipype or Nipype2Pydra update
       if: github.event_name == 'repository_dispatch'
       run: git checkout $(git tag -l | grep 'v.*' | tail -n 1 | awk -F post '{print $1}')
-
-    - name: Cache nireports Install
-      id: cache-install
-      uses: actions/cache@v4
-      with:
-        path: ${{ env.nireports_install_dir }}
-        key: nireports-${{ env.nireports_version }}-${{ runner.os }}
-
-    - name: Install nireports Package
-      if: steps.cache-install.outputs.cache-hit != 'true'
-      run: |
-        echo "NOT IMPLEMENTED YET (install at nireports_install_dir: $nireports_install_dir)"
-        exit 1  # This is a placeholder, replace this line and the one above with the installation procedure
-        echo "PATH=${{ env.nireports_install_dir }}/bin:$PATH" >> $GITHUB_ENV
     
     - name: Download tasks converted from Nipype 
       uses: actions/download-artifact@v4
       with:
         name: converted-nipype
-        path: pydra/tasks/nireports/auto
+        path: pydra/tasks/nireports
 
     - name: Show the contents of the auto-generated tasks
       run: tree pydra
 
     - name: Strip auto package from gitignore so it is included in package
       run: |
-        sed -i '/\/pydra\/tasks\/nireports\/auto/d' .gitignore
+        sed -i '/\/pydra\/tasks\/nireports/d' .gitignore
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install build dependencies
       run: |
         python -m pip install --upgrade pip
 
     - name: Install task package
       run: |
-        pip install "./related-packages/fileformats" "./related-packages/fileformats-extras" ".[test]"
+        pip install ".[test]"
         python -c "import pydra.tasks.nireports as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
         python -c "import pydra as m; print(f'{m.__name__} {m.__version__} @ {m.__file__}')"
 
     - name: Test with pytest
       run: >- 
         pytest -sv
         ./pydra/tasks/nireports
-        ./related-packages/fileformats
-        ./related-packages/fileformats-extras
         --cov pydra.tasks.nireports
-        --cov fileformats.medimage_nireports
-        --cov fileformats.extras.medimage_nireports
         --cov-report xml
 
     - name: Upload to CodeCov
       uses: codecov/codecov-action@v3
       if: ${{ always() }}
       with:
         files: coverage.xml
         name: pydra-nireports
 
-
-  deploy-fileformats:
-    needs: [devcheck, test]
-    runs-on: ubuntu-latest
-    steps:
-
-    - uses: actions/checkout@v4
-      with:
-        submodules: recursive
-        fetch-depth: 0
-
-    - name: Set up Python
-      uses: actions/setup-python@v5
-      with:
-        python-version: '3.11'
-
-    - name: Install build tools
-      run: python -m pip install build twine
-
-    - name: Build source and wheel distributions
-      run: python -m build ./related-packages/fileformats
-
-    - name: Check distributions
-      run: twine check ./related-packages/fileformats/dist/*
-
-    - name: Check for PyPI token on tag
-      id: deployable
-      if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
-      env:
-        PYPI_API_TOKEN: "${{ secrets.PYPI_FILEFORMATS_API_TOKEN }}"
-      run: if [ -n "$PYPI_API_TOKEN" ]; then echo "DEPLOY=true" >> $GITHUB_OUTPUT; fi
-
-    - name: Upload to PyPI
-      if: steps.deployable.outputs.DEPLOY
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_FILEFORMATS_API_TOKEN }}
-        packages-dir: ./related-packages/fileformats/dist 
-
-  deploy-fileformats-extras:
-    needs: [deploy-fileformats]
-    runs-on: ubuntu-latest
-    steps:
-
-    - uses: actions/checkout@v4
-      with:
-        submodules: recursive
-        fetch-depth: 0
-
-    - name: Set up Python
-      uses: actions/setup-python@v5
-      with:
-        python-version: '3.11'
-
-    - name: Install build tools
-      run: python -m pip install build twine
-
-    - name: Build source and wheel distributions
-      run: python -m build ./related-packages/fileformats-extras
-
-    - name: Check distributions
-      run: twine check ./related-packages/fileformats-extras/dist/*
-
-    - name: Check for PyPI token on tag
-      id: deployable
-      if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
-      env:
-        PYPI_API_TOKEN: "${{ secrets.PYPI_FILEFORMATS_EXTRAS_API_TOKEN }}"
-      run: if [ -n "$PYPI_API_TOKEN" ]; then echo "DEPLOY=true" >> $GITHUB_OUTPUT; fi
-
-    - name: Upload to PyPI
-      if: steps.deployable.outputs.DEPLOY
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_FILEFORMATS_EXTRAS_API_TOKEN }}
-        packages-dir: ./related-packages/fileformats-extras/dist 
-
   deploy:
-    needs: [nipype-conv, test, deploy-fileformats, deploy-fileformats-extras]
+    needs: [nipype-conv, test]
     runs-on: ubuntu-latest
     steps:
 
     - name: Checkout repository
       uses: actions/checkout@v4
       with:
         submodules: recursive
@@ -290,46 +189,46 @@
       if: github.event_name == 'repository_dispatch'
       run: git checkout ${{ steps.latest_tag.outputs.TAG }}
 
     - name: Download tasks converted from Nipype 
       uses: actions/download-artifact@v4
       with:
         name: converted-nipype
-        path: pydra/tasks/nireports/auto
+        path: pydra/tasks/nireports
 
     - name: Show the contents of the auto-generated tasks
       run: tree pydra
 
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.11'
 
     - name: Install build tools
       run: python -m pip install build twine
 
     - name: Strip auto package from gitignore so it is included in package
       run: |
-        sed -i '/\/pydra\/tasks\/nireports\/auto/d' .gitignore
+        sed -i '/\/pydra\/tasks\/nireports/d' .gitignore
         cat .gitignore
 
     - name: Install task package to calculate post-release tag
       run: |
-        pip install "./related-packages/fileformats" "./related-packages/fileformats-extras" ".[test]"
+        pip install ".[test]"
 
     - name: Generate post-release tag based on Nipype and Nipype2Pydra versions
       id: post_release_tag
       run: |
-        POST=$(python -c "from pydra.tasks.nireports.auto._post_release import post_release; print(post_release)")
+        POST=$(python -c "from pydra.tasks.nireports._post_release import post_release; print(post_release)")
         echo "TAG=${{ steps.latest_tag.outputs.TAG }}post${POST}" >> $GITHUB_OUTPUT
 
     - name: Add auto directory to git repo
       if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
       run: |
-        git add pydra/tasks/nireports/auto
+        git add pydra/tasks/nireports
         git commit -am"added auto-generated version to make new tag for package version"
         git status
 
     - name: Overwrite the tag of release event with latest commit (i.e. including the auto directory)
       if: github.event_name == 'release'
       run: |
         git tag -d ${{ steps.latest_tag.outputs.TAG }};
@@ -372,35 +271,35 @@
       with:
         tag_name: ${{ steps.post_release_tag.outputs.TAG }}
         release_name: Release ${{ steps.post_release_tag.outputs.TAG }}
         draft: false
         prerelease: false        
 
 
-  report_progress:
-    needs: [deploy]
-    runs-on: ubuntu-latest
-    steps:
-
-      - name: Generate progress report
-        id: generate-report
-        run: |
-          tools/report_progress.py outputs/progress-report.json
-          echo "progress_report=$(cat outputs/progress-report.json)" >> $GITHUB_OUTPUT
-
-      - name: Report progress to Nipype2Pydra repo
-        if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
-        run: >-
-          curl -XPOST -u "${{ env.POST_RELEASE_PAT }}" -H "Accept: application/vnd.github.everest-preview+json"
-          "https://api.github.com/repos/nipype/pydra-nireports/dispatches"
-          -d '{
-            "event_type": "progress-report",
-            "client_payload": ${{ steps.generate-report.output.progress_report }}
-          }'
-        env:
-          PAT: ${{ env.PROGRESS_REPORT_PAT }}
+  # report_progress:
+  #   needs: [deploy]
+  #   runs-on: ubuntu-latest
+  #   steps:
+
+  #     - name: Generate progress report
+  #       id: generate-report
+  #       run: |
+  #         tools/report_progress.py outputs/progress-report.json
+  #         echo "progress_report=$(cat outputs/progress-report.json)" >> $GITHUB_OUTPUT
+
+  #     - name: Report progress to Nipype2Pydra repo
+  #       if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
+  #       run: >-
+  #         curl -XPOST -u "${{ env.POST_RELEASE_PAT }}" -H "Accept: application/vnd.github.everest-preview+json"
+  #         "https://api.github.com/repos/nipype/pydra-nireports/dispatches"
+  #         -d '{
+  #           "event_type": "progress-report",
+  #           "client_payload": ${{ steps.generate-report.output.progress_report }}
+  #         }'
+  #       env:
+  #         PAT: ${{ env.PROGRESS_REPORT_PAT }}
 
 
 # Deploy on tags if PYPI_API_TOKEN is defined in the repository secrets.
 # Secrets are not accessible in the if: condition [0], so set an output variable [1]
 # [0] https://github.community/t/16928
 # [1] https://docs.github.com/en/actions/reference/workflow-commands-for-github-actions#setting-an-output-parameter
```

### Comparing `pydra_nireports-0.1.0/docs/Makefile` & `pydra_nireports-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/docs/conf.py` & `pydra_nireports-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/docs/make.bat` & `pydra_nireports-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/package.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/package.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/comp_cor_variance_plot.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/comp_cor_variance_plot.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/confounds_correlation_plot.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/confounds_correlation_plot.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/dwi_heatmap.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/dwi_heatmap.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/fmri_summary.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/fmri_summary.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_contours.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_contours.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_mosaic.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_mosaic.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/plot_spikes.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/plot_spikes.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/simple_before_after_rpt.yaml` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/simple_before_after_rpt.yaml`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/nipype-auto-conv/specs/interfaces/simple_before_after_rpt_callables.py` & `pydra_nireports-0.1.1/nipype-auto-conv/specs/interfaces/simple_before_after_rpt_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/tools/increment_tool_version.py` & `pydra_nireports-0.1.1/tools/increment_tool_version.py`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/tools/rename_template.py` & `pydra_nireports-0.1.1/tools/rename_template.py`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/.gitignore` & `pydra_nireports-0.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -137,8 +137,7 @@
 # VS Code
 .vscode
 
 # Mac garbarge
 .DS_store
 
 # Generated files
-/pydra/tasks/nireports
```

### Comparing `pydra_nireports-0.1.0/LICENSE` & `pydra_nireports-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/README.rst` & `pydra_nireports-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_nireports-0.1.0/pyproject.toml` & `pydra_nireports-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,40 +4,50 @@
 
 [project]
 name = "pydra-nireports"
 description = "Pydra tasks package for nireports"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
-    "pydra >=0.22",
     "fileformats >=0.8.3",
     "fileformats-datascience >=0.1",
     "fileformats-medimage >=0.4.1",
+    "importlib_resources >= 5.12; python_version < '3.12'",
+    "pydra >=0.22",
+    "matplotlib >= 3.4.2",
+    "nibabel >= 3.0.1",
+    "nilearn >= 0.5.2",
+    "numpy",
+    "pandas",
+    "pybids",
+    "pyyaml",
+    "seaborn",
+    "svgutils >= 0.3.4",
+    "templateflow",
+]
+license = { file = "LICENSE" }
+authors = [{ name = "Nipype developers", email = "neuroimaging@python.org" }]
+maintainers = [
+    { name = "Nipype developers", email = "neuroimaging@python.org" },
 ]
-license = {file = "LICENSE"}
-authors = [{name = "Nipype developers", email = "neuroimaging@python.org"}]
-maintainers = [{name = "Nipype developers", email = "neuroimaging@python.org"}]
 keywords = ["pydra"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = [
-    "black",
-    "pre-commit",
-]
+dev = ["black", "pre-commit"]
 doc = [
     "packaging",
     "sphinx >=2.1.2",
     "sphinx_rtd_theme",
     "sphinxcontrib-apidoc ~=0.3.0",
     "sphinxcontrib-napoleon",
     "sphinxcontrib-versioning",
@@ -70,13 +80,11 @@
 exclude = "_version.py"
 
 [tool.codespell]
 ignore-words = ".codespell-ignorewords"
 
 [tool.flake8]
 doctests = true
-per-file-ignores = [
-    "__init__.py:F401,F403"
-]
+per-file-ignores = ["__init__.py:F401,F403"]
 max-line-length = 88
 select = "C,E,F,W,B,B950"
 extend-ignore = ['E203', 'E501', 'E129', 'W503']
```

### Comparing `pydra_nireports-0.1.0/PKG-INFO` & `pydra_nireports-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydra-nireports
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pydra tasks package for nireports
 Author-email: Nipype developers <neuroimaging@python.org>
 Maintainer-email: Nipype developers <neuroimaging@python.org>
 License:    Copyright 2021 Nipype developers
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
@@ -29,15 +29,26 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: fileformats-datascience>=0.1
 Requires-Dist: fileformats-medimage>=0.4.1
 Requires-Dist: fileformats>=0.8.3
+Requires-Dist: importlib-resources>=5.12; python_version < '3.12'
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: nibabel>=3.0.1
+Requires-Dist: nilearn>=0.5.2
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pybids
 Requires-Dist: pydra>=0.22
+Requires-Dist: pyyaml
+Requires-Dist: seaborn
+Requires-Dist: svgutils>=0.3.4
+Requires-Dist: templateflow
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: packaging; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Requires-Dist: sphinx>=2.1.2; extra == 'doc'
```

