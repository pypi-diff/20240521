# Comparing `tmp/nipype2pydra-0.4.3.tar.gz` & `tmp/nipype2pydra-0.4.4.tar.gz`

## Comparing `nipype2pydra-0.4.3.tar` & `nipype2pydra-0.4.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/_version.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/exceptions.py
--rw-r--r--   0        0        0    14364 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/helpers.py
--rw-r--r--   0        0        0    40868 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/package.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/testing.py
--rw-r--r--   0        0        0    45837 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/workflow.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/cli/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/cli/base.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/cli/convert.py
--rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/cli/pkg_gen.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/__init__.py
--rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/base.py
--rw-r--r--   0        0        0    16959 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/function.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/loaders.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/shell_command.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/compute_dvars.yaml
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/non_steady_state_detector_callables.py
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/tsnr.yaml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/tsnr_callables.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/interface/tests/test_interface.py
--rw-r--r--   0        0        0    45492 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/__init__.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/NOTICE
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/README.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/init.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/pkg_gen/tests/test_pkg_gen.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/statements/__init__.py
--rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/statements/imports.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/statements/misc.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/statements/utility.py
--rw-r--r--   0        0        0    31670 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/statements/workflow_build.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/tests/test_package.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/utils/__init__.py
--rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/utils/misc.py
--rw-r--r--   0        0        0    23704 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/utils/symbols.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/utils/tests/test_utils_imports.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/nipype2pydra/utils/tests/test_utils_misc.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/LICENSE
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/README.rst
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 nipype2pydra-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/_version.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/exceptions.py
+-rw-r--r--   0        0        0    14364 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/helpers.py
+-rw-r--r--   0        0        0    42195 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/package.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/testing.py
+-rw-r--r--   0        0        0    45970 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/workflow.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/cli/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/cli/base.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/cli/convert.py
+-rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/cli/pkg_gen.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/__init__.py
+-rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/base.py
+-rw-r--r--   0        0        0    16959 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/function.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/loaders.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/shell_command.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/compute_dvars.yaml
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/non_steady_state_detector_callables.py
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/tsnr.yaml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/tsnr_callables.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/interface/tests/test_interface.py
+-rw-r--r--   0        0        0    45492 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/__init__.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/NOTICE
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/README.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/init.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
+-rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/pkg_gen/tests/test_pkg_gen.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/statements/__init__.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/statements/imports.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/statements/misc.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/statements/utility.py
+-rw-r--r--   0        0        0    31670 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/statements/workflow_build.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/tests/test_package.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/utils/__init__.py
+-rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/utils/misc.py
+-rw-r--r--   0        0        0    23704 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/utils/symbols.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/utils/tests/test_utils_imports.py
+-rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/nipype2pydra/utils/tests/test_utils_misc.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/LICENSE
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/README.rst
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    22710 2020-02-02 00:00:00.000000 nipype2pydra-0.4.4/PKG-INFO
```

### Comparing `nipype2pydra-0.4.3/nipype2pydra/helpers.py` & `nipype2pydra-0.4.4/nipype2pydra/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
             the converted function code
         used_configs : list[str]
             the names of the used configs
         """
 
         used_configs = set()
         parts = re.split(
-            r"\n    (?=[^\s])", replace_undefined(self.src), flags=re.MULTILINE
+            r"\n    (?!\s|\))", replace_undefined(self.src), flags=re.MULTILINE
         )
         converted_parts = []
         for part in parts:
             if part.startswith("def"):
                 converted_func, func_used_configs = self._convert_function(part)
                 converted_parts.append(converted_func)
                 used_configs.update(func_used_configs)
```

### Comparing `nipype2pydra-0.4.3/nipype2pydra/package.py` & `nipype2pydra-0.4.4/nipype2pydra/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from collections import defaultdict
 from pathlib import Path
 from operator import attrgetter, itemgetter
 import attrs
 import black.parsing
 import black.report
 from tqdm import tqdm
-import attrs
 import yaml
 from . import interface
 from .utils import (
     UsedSymbols,
     full_address,
     to_snake_case,
     cleanup_function_body,
@@ -1020,14 +1019,16 @@
             The depth of the package from the root up to which to generate __init__.py files
             for
         auto_import_depth: int
             the depth below which the init files should contain cascading imports from
         names : List[str]
             The names to import in the __init__.py files
         """
+        # Write base init path that imports __version__ from the auto-generated _version
+        # file
         parts = module_name.split(".")
         for i, part in enumerate(reversed(parts[depth:]), start=1):
             mod_parts = parts[:-i]
             parent_mod = ".".join(mod_parts)
             init_fspath = package_root.joinpath(*mod_parts, "__init__.py")
             if i > len(parts) - auto_import_depth:
                 # Write empty __init__.py if it doesn't exist
@@ -1095,7 +1096,47 @@
                 raise RuntimeError(
                     f"Black could not parse generated code (written to {debug_file}): "
                     f"{e}\n\n{code_str}"
                 )
 
             with open(init_fspath, "w") as f:
                 f.write(code_str)
+
+    BASE_INIT_TEMPLATE = """\"\"\"
+This is a basic doctest demonstrating that the package and pydra can both be successfully
+imported.
+
+>>> import pydra.engine
+>>> import pydra.tasks.{pkg}
+\"\"\"
+
+from warnings import warn
+from pathlib import Path
+
+pkg_path = Path(__file__).parent.parent
+
+try:
+    from ._version import __version__
+except ImportError:
+    raise RuntimeError(
+        "pydra-{pkg} has not been properly installed, please run "
+        f"`pip install -e {str(pkg_path)}` to install a development version"
+    )
+if "nipype" not in __version__:
+    try:
+        from ._post_release import src_pkg_version, nipype2pydra_version
+    except ImportError:
+        warn(
+            "Nipype interfaces haven't been automatically converted from their specs in "
+            f"`nipype-auto-conv`. Please run `{str(pkg_path / 'nipype-auto-conv' / 'generate')}` "
+            "to generated the converted Nipype interfaces in pydra.tasks.{pkg}.auto"
+        )
+    else:
+        n_ver = src_pkg_version.replace(".", "_")
+        n2p_ver = nipype2pydra_version.replace(".", "_")
+        __version__ += (
+            "_" if "+" in __version__ else "+"
+        ) + f"nipype{n_ver}_nipype2pydra{n2p_ver}"
+
+
+__all__ = ["__version__"]
+"""
```

### Comparing `nipype2pydra-0.4.3/nipype2pydra/testing.py` & `nipype2pydra-0.4.4/nipype2pydra/testing.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/workflow.py` & `nipype2pydra-0.4.4/nipype2pydra/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,19 @@
                 return (
                     type_repr_(ty.get_origin(t))
                     + "["
                     + ", ".join(type_repr_(a) for a in args)
                     + "]"
                 )
             if t in (ty.Any, ty.Union, ty.List, ty.Tuple):
-                return f"ty.{t.__name__}"
+                try:
+                    t_name = t.__name__
+                except AttributeError:
+                    t_name = t._name
+                return f"ty.{t_name}"
             elif issubclass(t, Field):
                 return t.primitive.__name__
             elif issubclass(t, FileSet):
                 return t.__name__
             elif t.__module__ == "builtins":
                 return t.__name__
             else:
```

### Comparing `nipype2pydra-0.4.3/nipype2pydra/cli/convert.py` & `nipype2pydra-0.4.4/nipype2pydra/cli/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,17 +61,24 @@
     # Initialise PackageConverter
     if package_spec.get("interface_only", None) is None:
         package_spec["interface_only"] = not workflow_yamls
     converter = PackageConverter(**package_spec)
 
     # Clean previous version of output dir
     package_dir = converter.package_dir(package_root)
-    output_dir = package_dir / "auto" if converter.interface_only else package_dir
-    if output_dir.exists():
-        shutil.rmtree(output_dir)
+    if converter.interface_only:
+        shutil.rmtree(package_dir / "auto")
+    else:
+        for fspath in package_dir.iterdir():
+            if fspath == package_dir / "__init__.py":
+                continue
+            if fspath.is_dir():
+                shutil.rmtree(fspath)
+            else:
+                fspath.unlink()
 
     # Load interface specs
     for fspath in interface_yamls:
         with open(fspath, "r") as f:
             spec = yaml.safe_load(f)
         converter.add_interface_from_spec(
             spec=spec,
```

### Comparing `nipype2pydra-0.4.3/nipype2pydra/cli/pkg_gen.py` & `nipype2pydra-0.4.4/nipype2pydra/cli/pkg_gen.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/__init__.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/base.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/base.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/function.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/function.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/loaders.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/loaders.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/shell_command.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/shell_command.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/compute_dvars.yaml` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/compute_dvars.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/tsnr.yaml` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/tsnr.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/nipype-ports/tsnr_callables.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/nipype-ports/tsnr_callables.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/interface/tests/test_interface.py` & `nipype2pydra-0.4.4/nipype2pydra/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/__init__.py` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/README.rst` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/init.py` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/init.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/pkg_gen/tests/test_pkg_gen.py` & `nipype2pydra-0.4.4/nipype2pydra/pkg_gen/tests/test_pkg_gen.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/statements/__init__.py` & `nipype2pydra-0.4.4/nipype2pydra/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/statements/imports.py` & `nipype2pydra-0.4.4/nipype2pydra/statements/imports.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/statements/misc.py` & `nipype2pydra-0.4.4/nipype2pydra/statements/misc.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/statements/utility.py` & `nipype2pydra-0.4.4/nipype2pydra/statements/utility.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/statements/workflow_build.py` & `nipype2pydra-0.4.4/nipype2pydra/statements/workflow_build.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/tests/test_package.py` & `nipype2pydra-0.4.4/nipype2pydra/tests/test_package.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,31 +12,51 @@
     "niworkflows": [
         "bids",
         "templateflow",
         "pydra-ants",
         "pydra-afni",
     ],
     "mriqc": [
+        "nipype2pydra",
         "pydra-ants",
         "pydra-afni",
         "pydra-fsl",
         "pydra-mrtrix3 >=3.0.3a0",
         "fileformats-medimage-afni-extras",
         "fileformats-medimage-mrtrix3-extras",
         "fileformats-medimage-fsl-extras",
+        "statsmodels",
+        "dipy",
+        "bids",
+        "pydra-niworkflows",
+        "pydra-nireports",
+        "matplotlib",
+        "seaborn",
+        "templateflow",
+        "nilearn",
+        # "nibael",
+        # "nilearn",
+        # "migas >= 0.4.0",
+        # "pandas ~=1.0",
+        # "pydra >=0.22",
+        # "PyYAML",
+        # "scikit-learn",
+        # "scipy",
+        # "statsmodel",
+        # "torch",
     ],
 }
 
 
 @pytest.fixture(params=[str(p.name) for p in EXAMPLE_WORKFLOWS_DIR.iterdir()])
 def package_spec(request):
     return EXAMPLE_PKG_GEN_DIR / f"{request.param}.yaml"
 
 
-@pytest.mark.xfail(reason="Fails due to missing dependencies on PyPI")
+@pytest.mark.xfail(reason="Don't have time to debug at the moment")
 def test_package_complete(package_spec, cli_runner, tmp_path, tasks_template_args):
     pkg_name = package_spec.stem
     repo_output = tmp_path / "repo"
     repo_output.mkdir()
 
     result = cli_runner(
         pkg_gen,
@@ -75,23 +95,19 @@
 
     venv_path = tmp_path / "venv"
     venv_python = str(venv_path / "bin" / "python")
     venv_pytest = str(venv_path / "bin" / "pytest")
 
     sp.check_call([sys.executable, "-m", "venv", str(venv_path)])
     pip_cmd = [venv_python, "-m", "pip", "install", "-e", str(pkg_root) + "[test]"]
-    try:
-        sp.check_call(pip_cmd)
-    except sp.CalledProcessError:
-        raise RuntimeError(
-            f"Failed to install package {pkg_name} with command:\n{' '.join(pip_cmd)}"
-        )
-    pytest_cmd = [venv_pytest, str(pkg_root)]
-    try:
-        pytest_output = sp.check_output(pytest_cmd)
-    except sp.CalledProcessError:
-        raise RuntimeError(
-            f"Tests of generated package '{pkg_name}' failed when running:\n{' '.join(pytest_cmd)}"
-        )
-
-    assert "fail" not in pytest_output
-    assert "error" not in pytest_output
+    p = sp.Popen(pip_cmd, stdout=sp.PIPE, stderr=sp.STDOUT)
+    pip_output, _ = p.communicate()
+    pip_output = pip_output.decode("utf-8")
+    assert (
+        not p.returncode
+    ), f"Failed to install package pydra-{pkg_name} with command:\n{' '.join(pip_cmd)}:\n\n{pip_output}"
+    p = sp.Popen([venv_pytest, str(pkg_root)], stderr=sp.PIPE, stdout=sp.STDOUT)
+    pytest_output, _ = p.communicate()
+    pytest_output = pytest_output.decode("utf-8")
+    assert (
+        p.returncode
+    ), f"Tests for pydra-{pkg_name} package (\n{' '.join(pip_cmd)}) failed:\n\n{pytest_output}"
```

### Comparing `nipype2pydra-0.4.3/nipype2pydra/utils/__init__.py` & `nipype2pydra-0.4.4/nipype2pydra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/utils/misc.py` & `nipype2pydra-0.4.4/nipype2pydra/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/utils/symbols.py` & `nipype2pydra-0.4.4/nipype2pydra/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/utils/tests/test_utils_imports.py` & `nipype2pydra-0.4.4/nipype2pydra/utils/tests/test_utils_imports.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/nipype2pydra/utils/tests/test_utils_misc.py` & `nipype2pydra-0.4.4/nipype2pydra/utils/tests/test_utils_misc.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/LICENSE` & `nipype2pydra-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/README.rst` & `nipype2pydra-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.3/pyproject.toml` & `nipype2pydra-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,19 @@
     "fileformats-medimage-extras",
     "fileformats-medimage-afni",
     "fileformats-medimage-ants",
     "fileformats-medimage-freesurfer",
     "fileformats-medimage-fsl",
     "niworkflows",
     "mriqc",
+    "nipy",
     "nireports",
     "nitime",
+    "datalad",
+    "nirodents",
 ]
 docs = [
     "packaging",
     "docutils>=0.10",
     "mock>1.0",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
```

### Comparing `nipype2pydra-0.4.3/PKG-INFO` & `nipype2pydra-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipype2pydra
-Version: 0.4.3
+Version: 0.4.4
 Summary: Tool for converting Nipype tasks and workflows into Pydra syntax
 Project-URL: repository, https://github.com/nipype/nipype2pydra
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -135,21 +135,24 @@
 Requires-Dist: mock>1.0; extra == 'docs'
 Requires-Dist: numpydoc>=0.6.0; extra == 'docs'
 Requires-Dist: packaging; extra == 'docs'
 Requires-Dist: sphinx-argparse>=0.2.0; extra == 'docs'
 Requires-Dist: sphinx-click>=3.1; extra == 'docs'
 Requires-Dist: sphinx>=2.1.2; extra == 'docs'
 Provides-Extra: test
+Requires-Dist: datalad; extra == 'test'
 Requires-Dist: fileformats-medimage-afni; extra == 'test'
 Requires-Dist: fileformats-medimage-ants; extra == 'test'
 Requires-Dist: fileformats-medimage-extras; extra == 'test'
 Requires-Dist: fileformats-medimage-freesurfer; extra == 'test'
 Requires-Dist: fileformats-medimage-fsl; extra == 'test'
 Requires-Dist: mriqc; extra == 'test'
+Requires-Dist: nipy; extra == 'test'
 Requires-Dist: nireports; extra == 'test'
+Requires-Dist: nirodents; extra == 'test'
 Requires-Dist: nitime; extra == 'test'
 Requires-Dist: niworkflows; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
```

