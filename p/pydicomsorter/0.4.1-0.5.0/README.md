# Comparing `tmp/pydicomsorter-0.4.1.tar.gz` & `tmp/pydicomsorter-0.5.0.tar.gz`

## Comparing `pydicomsorter-0.4.1.tar` & `pydicomsorter-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/pixi.lock
--rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/releaserc.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/ruff.toml
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/docs/index.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/LICENSE
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/README.md
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   231019 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/pixi.lock
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/releaserc.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/ruff.toml
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/docs/index.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/README.md
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/PKG-INFO
```

### Comparing `pydicomsorter-0.4.1/pixi.lock` & `pydicomsorter-0.5.0/pixi.lock`

 * *Files 1% similar despite different names*

```diff
@@ -117,24 +117,29 @@
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py312hf06ca03_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py312h9a8786e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py312h30efb56_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.14.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.36-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
@@ -161,72 +166,83 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py312h8fd38d8_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.4.4-py312h5715c7c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py312h8572e83_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py312h7900ff3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h75354e8_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py312h38bf5a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py312h520dd33_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py312hede676d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.14.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.36-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
@@ -246,72 +262,83 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-hd75f5a5_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py312ha04878a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.4.4-py312h675b354_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py312h49ebfd2_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py312hc2c2f20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-hde137ed_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py312h8e38eb3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py312h7e5086c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py312h20a0b95_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.14.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.36-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
@@ -331,71 +358,82 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py312h02f2b3b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py312hfa13136_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.4.4-py312h3402d49_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ukkonen-1.0.1-py312h389731b_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hcc0f68c_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py312h4389bb4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py312h53d5487_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.14.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.36-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
@@ -412,49 +450,55 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py312hd7027bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.4.4-py312h7a6832a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py312h0d7def4_4.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py312h2e8e312_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-he1f189c_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
@@ -1276,14 +1320,31 @@
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/cffi?source=conda-forge-mapping
   size: 294523
   timestamp: 1696001868949
 - kind: conda
+  name: cfgv
+  version: 3.3.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
+  sha256: fbc03537a27ef756162c49b1d0608bf7ab12fa5e38ceb8563d6f4859e835ac5c
+  md5: ebb5f5f7dc4f1a3780ef7ea7738db08c
+  depends:
+  - python >=3.6.1
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/cfgv?source=conda-forge-mapping
+  size: 10788
+  timestamp: 1629909423398
+- kind: conda
   name: charset-normalizer
   version: 3.3.2
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda
   sha256: 20cae47d31fdd58d99c4d2e65fbdcefa0b0de0c84e455ba9d6356a4bdbc4b5b9
@@ -1988,14 +2049,32 @@
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/hyperlink?source=conda-forge-mapping
   size: 72732
   timestamp: 1610092261086
 - kind: conda
+  name: identify
+  version: 2.5.36
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/identify-2.5.36-pyhd8ed1ab_0.conda
+  sha256: dc98ab2233d3ed3692499e2a06b027489ee317658cef9277ec23cab00236f31c
+  md5: ba68cb5105760379432cebc82b45af40
+  depends:
+  - python >=3.6
+  - ukkonen
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/identify?source=conda-forge-mapping
+  size: 78375
+  timestamp: 1713673091737
+- kind: conda
   name: idna
   version: '3.7'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
   sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
@@ -3433,14 +3512,32 @@
   license: BSD-2-Clause
   license_family: BSD
   purls:
   - pkg:pypi/nest-asyncio?source=conda-forge-mapping
   size: 11638
   timestamp: 1705850780510
 - kind: conda
+  name: nodeenv
+  version: 1.8.0
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
+  sha256: 1320306234552717149f36f825ddc7e27ea295f24829e9db4cc6ceaff0b032bd
+  md5: 2a75b296096adabbabadd5e9782e5fcc
+  depends:
+  - python 2.7|>=3.7
+  - setuptools
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/nodeenv?source=conda-forge-mapping
+  size: 34358
+  timestamp: 1683893151613
+- kind: conda
   name: openssl
   version: 3.3.0
   build: h0d3ecfb_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
   sha256: 51f9be8fe929c2bb3243cd0707b6dfcec27541f8284b4bd9b063c288fc46f482
   md5: 25b0e522c3131886a637e347b2ca0c0f
@@ -3637,14 +3734,36 @@
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/pluggy?source=conda-forge-mapping
   size: 23815
   timestamp: 1713667175451
 - kind: conda
+  name: pre-commit
+  version: 3.7.1
+  build: pyha770c72_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
+  sha256: 689c169ce6ed5d516d8524cc1e6ef2687dff19747c1ed1ee9b347a71f47ff12d
+  md5: 724bc4489c1174fc8e3233b0624fa51f
+  depends:
+  - cfgv >=2.0.0
+  - identify >=1.0.0
+  - nodeenv >=0.11.1
+  - python >=3.9
+  - pyyaml >=5.1
+  - virtualenv >=20.10.0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pre-commit?source=conda-forge-mapping
+  size: 179748
+  timestamp: 1715432871404
+- kind: conda
   name: prompt-toolkit
   version: 3.0.42
   build: pyha770c72_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
   sha256: 58525b2a9305fb154b2b0d43a48b9a6495441b80e4fbea44f2a34a597d2cef16
@@ -3900,17 +4019,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.4.1
+  version: 0.5.0
   path: .
-  sha256: 64335c4f4dbf9c666e3326d8854eb46d8e0740cf9931b6db34349a52cc4e1077
+  sha256: f2203ddb1c827d562e9173a6986da4fdfcd84fe2b6860dd9621e1f6e26a23322
   requires_dist:
   - rich
   - rich-click
   - pydicom
   requires_python: '>=3.12'
   editable: true
 - kind: pypi
@@ -4746,14 +4865,31 @@
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/secretstorage?source=conda-forge-mapping
   size: 31766
   timestamp: 1695551875966
 - kind: conda
+  name: setuptools
+  version: 69.5.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+  sha256: 72d143408507043628b32bed089730b6d5f5445eccc44b59911ec9f262e365e7
+  md5: 7462280d81f639363e6e63c81276bd9e
+  depends:
+  - python >=3.8
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/setuptools?source=conda-forge-mapping
+  size: 501790
+  timestamp: 1713094963112
+- kind: conda
   name: shellingham
   version: 1.5.4
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
   sha256: 3c49a0a101c41b7cf6ac05a1872d7a1f91f1b6d02eecb4a36b605a19517862bb
@@ -5136,14 +5272,98 @@
   constrains:
   - vs2015_runtime >=14.29.30037
   license: LicenseRef-Proprietary
   license_family: PROPRIETARY
   size: 1283972
   timestamp: 1666630199266
 - kind: conda
+  name: ukkonen
+  version: 1.0.1
+  build: py312h0d7def4_4
+  build_number: 4
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py312h0d7def4_4.conda
+  sha256: f5f7550991ca647f69b67b9188c7104a3456122611dd6a6e753cff555e45dfd9
+  md5: 57cfbb8ce3a1800bd343bf6afba6f878
+  depends:
+  - cffi
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ukkonen?source=conda-forge-mapping
+  size: 17235
+  timestamp: 1695549871621
+- kind: conda
+  name: ukkonen
+  version: 1.0.1
+  build: py312h389731b_4
+  build_number: 4
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ukkonen-1.0.1-py312h389731b_4.conda
+  sha256: 7336cf66feba973207f4903c20b05c3c82e351246df4b6113f72d92b9ee55b81
+  md5: 6407429e0969b58b8717dbb4c6c15513
+  depends:
+  - cffi
+  - libcxx >=15.0.7
+  - python >=3.12.0rc3,<3.13.0a0
+  - python >=3.12.0rc3,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ukkonen?source=conda-forge-mapping
+  size: 13948
+  timestamp: 1695549890285
+- kind: conda
+  name: ukkonen
+  version: 1.0.1
+  build: py312h49ebfd2_4
+  build_number: 4
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py312h49ebfd2_4.conda
+  sha256: efca19a5e73e4aacfc5e90a5389272b2508e41dc4adab9eb5353c5200ba37041
+  md5: 4e6b5a8025cd8fd97b3cfe103ffce6b1
+  depends:
+  - cffi
+  - libcxx >=15.0.7
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ukkonen?source=conda-forge-mapping
+  size: 13246
+  timestamp: 1695549689363
+- kind: conda
+  name: ukkonen
+  version: 1.0.1
+  build: py312h8572e83_4
+  build_number: 4
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py312h8572e83_4.conda
+  sha256: f9a4384d466f4d8b5b497d951329dd4407ebe02f8f93456434e9ab789d6e23ce
+  md5: 52c9e25ee0a32485a102eeecdb7eef52
+  depends:
+  - cffi
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ukkonen?source=conda-forge-mapping
+  size: 14050
+  timestamp: 1695549556745
+- kind: conda
   name: urllib3
   version: 2.2.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
   sha256: d4009dcc9327684d6409706ce17656afbeae690d8522d3c9bc4df57649a352cd
```

### Comparing `pydicomsorter-0.4.1/.github/workflows/main.yaml` & `pydicomsorter-0.5.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/config/mkdocs.yaml` & `pydicomsorter-0.5.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/config/releaserc.toml` & `pydicomsorter-0.5.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/config/ruff.toml` & `pydicomsorter-0.5.0/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/docs/CHANGELOG.md` & `pydicomsorter-0.5.0/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # CHANGELOG
 
 
 
+## v0.5.0 (2024-05-21)
+
+### Chore
+
+* chore: update pre-commit dependency version to &gt;=3.7.1,&lt;3.8 ([`446a5cc`](https://github.com/jjjermiah/PyDicomSorter/commit/446a5ccfc32a34705f0aa234113db32c6296de13))
+
+* chore: remove unused .pypackage-builder-answers.yml file and update README badges ([`bcd0a59`](https://github.com/jjjermiah/PyDicomSorter/commit/bcd0a599bceeaa38fdd29a241992237077aae7f1))
+
+### Feature
+
+* feat: update pre-commit dependency version to &gt;=3.7.1,&lt;3.8 ([`6b57254`](https://github.com/jjjermiah/PyDicomSorter/commit/6b572546a57ca0abec71d1500d10d1e769c40cb0))
+
+### Unknown
+
+* update precommit ([`69584db`](https://github.com/jjjermiah/PyDicomSorter/commit/69584db9521a65ed4348bd7037e1253cc0742bea))
+
+
 ## v0.4.1 (2024-05-21)
 
 ### Fix
 
 * fix: lock ([`9711580`](https://github.com/jjjermiah/PyDicomSorter/commit/9711580d2decb816113b45d0cb44b4b74c26d8d7))
 
 * fix: enforce code upload ([`ba93172`](https://github.com/jjjermiah/PyDicomSorter/commit/ba93172023f9c56eaac91b5f95270d0330e33d4b))
```

### Comparing `pydicomsorter-0.4.1/docs/about.md` & `pydicomsorter-0.5.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/src/pydicomsorter/parser.py` & `pydicomsorter-0.5.0/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.5.0/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.5.0/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/tests/test_parser.py` & `pydicomsorter-0.5.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/.gitignore` & `pydicomsorter-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/LICENSE` & `pydicomsorter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.1/pyproject.toml` & `pydicomsorter-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.4.1"
+version = "0.5.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
@@ -67,29 +67,30 @@
 
 [tool.pixi.feature.test.tasks.coverage]
 cmd = "coverage report --rcfile=config/coverage.toml"
 inputs = ["coverage-report/coverage.xml", "config/coverage.toml"]
 depends-on = ["test"]
 
 ############################################## STYLE ###############################################
-# See ruff.toml for the configuration
+# See config/ruff.toml for the configuration
 [tool.pixi.feature.style.dependencies]
-ruff = "*"
+ruff = ">=0.4.4"
+pre-commit = ">=3.7.1,<3.8"
 
 [tool.pixi.feature.style.tasks.lint]
 cmd = "ruff check --config=config/ruff.toml src"
 inputs = ["src", "config/ruff.toml"]
 
 [tool.pixi.feature.style.tasks.format]
 cmd = "ruff format --config=config/ruff.toml src"
 inputs = ["src", "config/ruff.toml"]
 
 ############################################## DOCS ################################################
 # Available tasks: doc-build, doc-serve, doc-deploy
-
+# See config/mkdocs.yaml for the configuration
 [tool.pixi.feature.docs.dependencies]
 mkdocs = "*"
 
 [tool.pixi.feature.docs.tasks.doc-build]
 cmd = "mkdocs build -f config/mkdocs.yaml"
 inputs = ["docs"]
 outputs = ["site"]
```

