# Comparing `tmp/max_ble_hci-1.1.tar.gz` & `tmp/max_ble_hci-1.1.1.tar.gz`

## Comparing `max_ble_hci-1.1.tar` & `max_ble_hci-1.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.1/install.bat
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.1/install.sh
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/black-format-check.yml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/black-format-run.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/pypi-deploy.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.github/workflows/test-installer.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/make.bat
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/ble_hci.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/ble_standard.rst
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/constants.rst
--rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/controller_cmds.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/data_params.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/examples.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/hci_packets.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/hci_reference.rst
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/index.rst
--rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/informational_cmds.rst
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/installation.rst
--rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/le_controller_cmds.rst
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/link_control_cmds.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/modules.rst
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/overview.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/packet_codes.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/packet_defs.rst
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/status_cmds.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/utils.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/vendor_spec.rst
--rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/vendor_spec_cmds.rst
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/examples/dtm.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/examples/hello_hci.py
--rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.1/docs/source/images/ble_stack_diagram.jpeg
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.1/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1/examples/dtm.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.1/examples/hello_hci.py
--rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci_cli.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/__init__.py
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/_hci_logger.py
--rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/_transport.py
--rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/ble_hci.py
--rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/ble_standard_cmds.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/constants.py
--rw-r--r--   0        0        0    17185 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/data_params.py
--rw-r--r--   0        0        0    19610 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/hci_packets.py
--rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/packet_codes.py
--rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/packet_defs.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/utils.py
--rw-r--r--   0        0        0    56077 2020-02-02 00:00:00.000000 max_ble_hci-1.1/src/max_ble_hci/vendor_spec_cmds.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.1/tests/test.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.1/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.1/LICENSE
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.1/README.md
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 max_ble_hci-1.1/pyproject.toml
--rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 max_ble_hci-1.1/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/install.bat
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/install.sh
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/black-format-check.yml
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/black-format-run.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.github/workflows/test-installer.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/ble_hci.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/ble_standard.rst
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/constants.rst
+-rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/controller_cmds.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/data_params.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/examples.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/hci_packets.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/hci_reference.rst
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/informational_cmds.rst
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/installation.rst
+-rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/le_controller_cmds.rst
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/link_control_cmds.rst
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/modules.rst
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/overview.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/packet_codes.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/packet_defs.rst
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/status_cmds.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/utils.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/vendor_spec.rst
+-rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/vendor_spec_cmds.rst
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/examples/dtm.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/examples/hello_hci.py
+-rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/docs/source/images/ble_stack_diagram.jpeg
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/examples/dtm.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/examples/hello_hci.py
+-rw-r--r--   0        0        0    25454 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci_cli.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/__init__.py
+-rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/_hci_logger.py
+-rw-r--r--   0        0        0    14622 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/_transport.py
+-rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/ble_hci.py
+-rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/ble_standard_cmds.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/constants.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/data_params.py
+-rw-r--r--   0        0        0    19610 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/hci_packets.py
+-rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/packet_codes.py
+-rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/packet_defs.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/utils.py
+-rw-r--r--   0        0        0    56073 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/src/max_ble_hci/vendor_spec_cmds.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/tests/test.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.1.1/PKG-INFO
```

### Comparing `max_ble_hci-1.1/.github/workflows/black-format-run.yml` & `max_ble_hci-1.1.1/.github/workflows/black-format-run.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/.github/workflows/documentation.yml` & `max_ble_hci-1.1.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/.github/workflows/pylint.yml` & `max_ble_hci-1.1.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/.github/workflows/pypi-deploy.yml` & `max_ble_hci-1.1.1/.github/workflows/pypi-deploy.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/.github/workflows/python-package-conda.yml` & `max_ble_hci-1.1.1/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/.github/workflows/test-installer.yml` & `max_ble_hci-1.1.1/.github/workflows/test-installer.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/Makefile` & `max_ble_hci-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/make.bat` & `max_ble_hci-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/conf.py` & `max_ble_hci-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/controller_cmds.rst` & `max_ble_hci-1.1.1/docs/source/controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/examples.rst` & `max_ble_hci-1.1.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/index.rst` & `max_ble_hci-1.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/informational_cmds.rst` & `max_ble_hci-1.1.1/docs/source/informational_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/installation.rst` & `max_ble_hci-1.1.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/le_controller_cmds.rst` & `max_ble_hci-1.1.1/docs/source/le_controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/link_control_cmds.rst` & `max_ble_hci-1.1.1/docs/source/link_control_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/overview.rst` & `max_ble_hci-1.1.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/status_cmds.rst` & `max_ble_hci-1.1.1/docs/source/status_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/vendor_spec_cmds.rst` & `max_ble_hci-1.1.1/docs/source/vendor_spec_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/examples/connection.py` & `max_ble_hci-1.1.1/docs/source/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/examples/dtm.py` & `max_ble_hci-1.1.1/docs/source/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/examples/hello_hci.py` & `max_ble_hci-1.1.1/docs/source/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/docs/source/images/ble_stack_diagram.jpeg` & `max_ble_hci-1.1.1/docs/source/images/ble_stack_diagram.jpeg`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/examples/connection.py` & `max_ble_hci-1.1.1/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/examples/dtm.py` & `max_ble_hci-1.1.1/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/examples/hello_hci.py` & `max_ble_hci-1.1.1/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci_cli.py` & `max_ble_hci-1.1.1/src/max_ble_hci_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,19 @@
 except ImportError:
     import gnureadline as readline
 
 # pylint: enable=unused-import
 import sys
 from argparse import RawTextHelpFormatter
 
+# pylint: disable=import-error
 from colorlog import ColoredFormatter
 
+# pylint: enable=import-error
+
 from max_ble_hci import BleHci
 from max_ble_hci.constants import PhyOption, PayloadOption
 from max_ble_hci.data_params import ConnParams, AdvParams, ScanParams
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -183,14 +186,22 @@
         "-b",
         "--baud",
         dest="baudRate",
         type=int,
         default=DEFAULT_BAUD,
         help="Serial port baud rate. Default: " + str(DEFAULT_BAUD),
     )
+
+    parser.add_argument(
+        "-efc",
+        "--enable-flow-control",
+        action="store_false",
+        default=False,
+        help="Serial port baud rate. Default: " + str(DEFAULT_BAUD),
+    )
     parser.add_argument(
         "-m",
         "--monitor-trace-port",
         dest="monPort",
         default=None,
         help="Monitor Trace Msg Serial Port path or COM#. Default: None",
     )
@@ -229,14 +240,15 @@
 
     hci = BleHci(
         args.serial_port,
         baud=args.baudRate,
         id_tag=args.idtag,
         async_callback=print,
         evt_callback=print,
+        flowcontrol=args.enable_flow_control,
     )
     hci.logger.setLevel(args.trace_level)
 
     print("Bluetooth Low Energy HCI tool")
     print(f"Serial port: {args.serial_port}")
     print(f"Monitor Trace Msg Serial Port: {args.monPort}")
     print(f"8N1 {args.baudRate}")
```

### Comparing `max_ble_hci-1.1/src/max_ble_hci/__init__.py` & `max_ble_hci-1.1.1/src/max_ble_hci/__init__.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/_hci_logger.py` & `max_ble_hci-1.1.1/src/max_ble_hci/_hci_logger.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/_transport.py` & `max_ble_hci-1.1.1/src/max_ble_hci/_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         id_tag: str = "DUT",
         logger_name: str = "BLE-HCI",
         retries: int = 0,
         timeout: float = 1.0,
         async_callback: Optional[Callable[[AsyncPacket], Any]] = None,
         evt_callback: Optional[Callable[[EventPacket], Any]] = None,
         exclusive_port: bool = True,
+        flowcontrol: bool = False,
     ):
         self.port_id = port_id
         self.port = None
         self.id_tag = id_tag
         self.logger = get_formatted_logger(name=logger_name)
         self.retries = retries
         self.timeout = timeout
@@ -166,15 +167,15 @@
 
         self._event_packets = []
         self._read_thread = None
         self._kill_evt = None
         self._data_lock = None
         self._port_lock = None
 
-        self._init_port(port_id, baud, exclusive_port)
+        self._init_port(port_id, baud, exclusive_port, flowcontrol)
         self._init_read_thread()
 
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -307,28 +308,30 @@
             daemon=True,
             name=f"Thread-{self.id_tag}",
         )
         self._data_lock = Lock()
         self._port_lock = Lock()
         self.start()
 
-    def _init_port(self, port_id: str, baud: int, exclusive: bool) -> None:
+    def _init_port(
+        self, port_id: str, baud: int, exclusive: bool, flowcontrol=False
+    ) -> None:
         """Initializes serial port.
 
         PRIVATE
 
         """
         try:
             self.port = serial.Serial(
                 port=port_id,
                 baudrate=baud,
                 parity=serial.PARITY_NONE,
                 stopbits=serial.STOPBITS_ONE,
                 bytesize=serial.EIGHTBITS,
-                rtscts=False,
+                rtscts=flowcontrol,
                 dsrdtr=False,
                 timeout=2.0,
                 exclusive=exclusive,
             )
 
         except serial.SerialException as err:
             self.logger.error("%s: %s", type(err).__name__, err)
```

### Comparing `max_ble_hci-1.1/src/max_ble_hci/ble_hci.py` & `max_ble_hci-1.1.1/src/max_ble_hci/ble_hci.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,22 +126,25 @@
         id_tag: str = "DUT",
         log_level: Union[str, int] = "INFO",
         logger_name: str = "BLE-HCI",
         retries: int = 0,
         timeout: float = 1.0,
         async_callback: Optional[Callable[[AsyncPacket], Any]] = None,
         evt_callback: Optional[Callable[[EventPacket], Any]] = None,
+        flowcontrol=False,
     ):
         self.port_id = port_id
         self.port = None
         self.id_tag = id_tag
         self.logger = get_formatted_logger(log_level=log_level, name=logger_name)
         self.retries = retries
         self.timeout = timeout
-        self._init_ports(port_id, baud, logger_name, async_callback, evt_callback)
+        self._init_ports(
+            port_id, baud, logger_name, async_callback, evt_callback, flowcontrol
+        )
         super().__init__(self.port, logger_name)
 
     def get_log_level(self) -> str:
         """Retrieve the current log level.
 
         Retrieved the current logging level in string
         format.
@@ -415,14 +418,15 @@
     def _init_ports(
         self,
         port_id: str,
         baud: int,
         logger_name: str,
         async_callback: Optional[Callable[[AsyncPacket], Any]],
         evt_callback: Optional[Callable[[EventPacket], Any]],
+        flowcontrol=False,
     ) -> None:
         """Initializes serial ports.
 
         PRIVATE
 
         """
         self.port = SerialUartTransport(
@@ -430,8 +434,9 @@
             baud=baud,
             id_tag=self.id_tag,
             logger_name=logger_name,
             retries=self.retries,
             timeout=self.timeout,
             async_callback=async_callback,
             evt_callback=evt_callback,
+            flowcontrol=flowcontrol,
         )
```

### Comparing `max_ble_hci-1.1/src/max_ble_hci/ble_standard_cmds.py` & `max_ble_hci-1.1.1/src/max_ble_hci/ble_standard_cmds.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/constants.py` & `max_ble_hci-1.1.1/src/max_ble_hci/constants.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/data_params.py` & `max_ble_hci-1.1.1/src/max_ble_hci/data_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,16 +273,16 @@
         -------
         float
             Calculated PER value.
 
         """
         if peer_tx_data:
             return 100 - 100 * (self.rx_data / peer_tx_data)
-        return 100 - self.rx_data / (
-            self.rx_data + self.rx_data_crc + self.rx_data_timeout
+        return 100 * (
+            1 - self.rx_data / (self.rx_data + self.rx_data_crc + self.rx_data_timeout)
         )
 
 
 @dataclass
 class AdvPktStats:
     """Advertising statistics data container."""
```

### Comparing `max_ble_hci-1.1/src/max_ble_hci/hci_packets.py` & `max_ble_hci-1.1.1/src/max_ble_hci/hci_packets.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/packet_codes.py` & `max_ble_hci-1.1.1/src/max_ble_hci/packet_codes.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/packet_defs.py` & `max_ble_hci-1.1.1/src/max_ble_hci/packet_defs.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/utils.py` & `max_ble_hci-1.1.1/src/max_ble_hci/utils.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/src/max_ble_hci/vendor_spec_cmds.py` & `max_ble_hci-1.1.1/src/max_ble_hci/vendor_spec_cmds.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,20 +312,18 @@
                 f"Packet length too large ({packet_len}), must be 255 or less."
             )
         if num_packets > 0xFFFF:
             raise ValueError(
                 f"Num packets too large ({num_packets}), must be 65535 or less."
             )
 
-        if isinstance(payload, PayloadOption):
-            payload = payload.value
-        if isinstance(phy, PhyOption):
-            phy = phy.value
-
+        payload = payload.value if isinstance(payload, PayloadOption) else payload
+        phy = phy.value if isinstance(phy, PhyOption) else phy
         params = [channel, packet_len, payload, phy]
+
         params.extend(to_le_nbyte_list(num_packets, 2))
         return self.send_vs_command(OCF.VENDOR_SPEC.TX_TEST, params=params)
 
     def rx_test_vs(
         self,
         channel: int = 0,
         phy: Union[PhyOption, int] = PhyOption.PHY_1M,
```

### Comparing `max_ble_hci-1.1/tests/test.py` & `max_ble_hci-1.1.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/LICENSE` & `max_ble_hci-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/README.md` & `max_ble_hci-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1/pyproject.toml` & `max_ble_hci-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/max_ble_hci", "src/max_ble_hci_cli.py"]
 
 [project]
 name = "max_ble_hci"
-version = "1.1"
+version = "1.1.1"
 dependencies = [
     "pyserial",
     "pyreadline3 ; platform_system == 'Windows'",
     "gnureadline ; platform_system == 'Darwin'",
     "colorlog"
 ]
 requires-python = ">=3.8"
```

### Comparing `max_ble_hci-1.1/PKG-INFO` & `max_ble_hci-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: max_ble_hci
-Version: 1.1
+Version: 1.1.1
 Summary: BLE HCI Test interface for controllers capable of the UART transport
 Project-URL: Homepage, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Repository, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Documentation, https://analog-devices-msdk.github.io/MAX-BLE-HCI/
 Project-URL: Bug Tracker, https://github.com/Analog-Devices-MSDK/BLE-HCI/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
```

