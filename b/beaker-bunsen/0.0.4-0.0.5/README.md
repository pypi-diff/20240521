# Comparing `tmp/beaker_bunsen-0.0.4.tar.gz` & `tmp/beaker_bunsen-0.0.5.tar.gz`

## Comparing `beaker_bunsen-0.0.4.tar` & `beaker_bunsen-0.0.5.tar`

### file list

```diff
@@ -1,95 +1,97 @@
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/DEFINITIONS.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/.github/workflows/build-publish.yaml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/.github/workflows/test.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/bunsen_agent.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/bunsen_context.py
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/corpus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/builder/__init__.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/builder/hooks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/__init__.py
--rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/chromadb_store.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/types.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/vector_store.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/base.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/code.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/document.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/documentation.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/examples.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/base.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/schemes.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/util/helpers.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/util/splitters.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_base_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_build.py
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_chromadb.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_code_loaders.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_corpus.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_documentation_embedder.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_example_embedder.py
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_local_file_loader.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_schemes.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_utils.py
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/test_zipped_chromadb.py
--rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/store.zip
--rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/corpus.zip
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/config.yaml
--rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/store.zip
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.__version__
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.adapters
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.api
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.auth
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.certs
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.compat
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.cookies
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.help
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.hooks
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.models
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.packages
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.sessions
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.structures
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.utils
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documentation/ruff_readme.md
--rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/yorkshire.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/yorkshire.txt.metadata
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/recipes/.metadata
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/recipes/ham_and_lentil_soup
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/recipes/irish_potato_caserole
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/recipes/tajine_maadnous
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/recipes/winter_risotto
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/documents/recipes/winter_risotto.metadata
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/examples/example_3.md
--rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/images/kitten-sad.jpg
--rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/images/kitten_hacker.jpg
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/images/puppy_hacker.jpg
--rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/images/puppy_sad.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/pyproject.toml
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/documentation/ruff_readme.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/examples/example_3.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/src/test_project/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/src/test_project/agent.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/tests/data/subproject/src/test_project/context.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/README.md
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/DEFINITIONS.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/.github/workflows/build-publish.yaml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_agent.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_context.py
+-rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/corpus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/builder/__init__.py
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/builder/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/scripts/__init__.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/scripts/bunsen.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/__init__.py
+-rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/chromadb_store.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/types.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/vector_store.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/base.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/code.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/document.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/documentation.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/examples.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/base.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/schemes.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/helpers.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/splitters.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_base_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_build.py
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_chromadb.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_code_loaders.py
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_corpus.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_documentation_embedder.py
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_example_embedder.py
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_local_file_loader.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_schemes.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_utils.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/test_zipped_chromadb.py
+-rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/store.zip
+-rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/corpus.zip
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/config.yaml
+-rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/store.zip
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.__version__
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.adapters
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.api
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.auth
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.certs
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.compat
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.cookies
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.help
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.hooks
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.models
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.packages
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.sessions
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.structures
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.utils
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documentation/ruff_readme.md
+-rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/yorkshire.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/yorkshire.txt.metadata
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/.metadata
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/ham_and_lentil_soup
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/irish_potato_caserole
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/tajine_maadnous
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/winter_risotto
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/documents/recipes/winter_risotto.metadata
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/examples/example_3.md
+-rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/kitten-sad.jpg
+-rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/kitten_hacker.jpg
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/puppy_hacker.jpg
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/images/puppy_sad.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/pyproject.toml
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/documentation/ruff_readme.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/examples/example_3.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/src/test_project/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/src/test_project/agent.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/tests/data/subproject/src/test_project/context.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/README.md
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.5/PKG-INFO
```

### Comparing `beaker_bunsen-0.0.4/DEFINITIONS.md` & `beaker_bunsen-0.0.5/DEFINITIONS.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/.github/workflows/build-publish.yaml` & `beaker_bunsen-0.0.5/.github/workflows/build-publish.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/.github/workflows/test.yaml` & `beaker_bunsen-0.0.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/bunsen_agent.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_agent.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/bunsen_context.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/bunsen_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,27 +87,40 @@
         return None
 
     async def build_prompt(
             self,
             state: dict[str,any],
             code_examples: list[str] = None,
         ) -> str:
-        variables = state.get("variables", {})
-        modules = state.get("modules", {})
-        functions = state.get("functions", {})
+        if state:
+            variables = state.get("variables", {})
+            modules = state.get("modules", [])
+            functions = state.get("functions", {})
+        else:
+            variables = {}
+            modules = []
+            functions = []
+
 
         python_libraries = self.bunsen_config.get("python_libraries", [])
         if len(python_libraries) > 1:
             python_library_str = f"Python libraries {', '.join(python_libraries)}"
         elif len(python_libraries) == 1:
             python_library_str = f"Python library {python_libraries[0]}"
         else:
             python_library_str = None
+        r_cran_libraries = self.bunsen_config.get("r_cran_libraries", [])
+        if len(r_cran_libraries) > 1:
+            r_cran_library_str = f"r_cran libraries {', '.join(r_cran_libraries)}"
+        elif len(r_cran_libraries) == 1:
+            r_cran_library_str = f"r_cran library {r_cran_libraries[0]}"
+        else:
+            r_cran_library_str = None
 
-        library_str = " and ".join([python_library_str, ])
+        library_str = " and ".join(libs for libs in (python_library_str, r_cran_library_str) if libs)
         submodule_description = None
         code_example_str = "\n".join(
             """
 ======== example {num} start ========
 {example}
 ======== example {num} end   ========
             """.strip().format(num=num, example=example)
```

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/corpus.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
                 uri_parts = urlparse(resource_uri)
                 if uri_parts.scheme in ("file", "zipped-file"):
                     uri_path = Path(uri_parts.path).relative_to(partition_common_paths[partition])
                 else:
                     uri_path = Path(uri_parts.path)
 
                 resource_path = Path(partition) / uri_path
-                # new_uri = f"corpus:{corpus_path}"
                 new_uri = CorpusResourceScheme.get_uri_for_location(resource_path)
                 content = read_from_uri(resource_uri)
                 mode = "wb" if isinstance(content, bytes) else "w"
                 dest = resource_dir / resource_path
                 if not dest.parent.exists():
                     dest.parent.mkdir(parents=True)
                 with open(dest, mode) as fh:
```

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/builder/hooks.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/builder/hooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 from hatchling.builders.config import BuilderConfig
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 from hatchling.plugin import hookimpl
 
 from beaker_kernel.lib.context import BaseContext
 from ..vectordb.embedders import DocumentationEmbedder, ExampleEmbedder, CodeEmbedder, PythonEmbedder
-from ..vectordb.loaders import LocalFileLoader, PythonLibraryLoader
+from ..vectordb.loaders import LocalFileLoader, PythonLibraryLoader, RCRANSourceLoader
+from ..vectordb.loaders.code_library_loader import RCRANLocalCache
 from ..vectordb.chromadb_store import ZippedChromaDBStore
 from ..corpus import Corpus
 
 
 logger = logging.getLogger("bunsen_build")
 
 class BuildError(Exception):
@@ -30,14 +31,15 @@
     PLUGIN_NAME = "bunsen"
 
     _BUILD_DIR = "build"
     _CONFIG_KEYS_TO_SAVE = [
         "documentation_path",
         "examples_path",
         "python_libraries",
+        "r_cran_libraries",
         "library_descriptions",
     ]
     _CONFIG_KEYS_TO_IGNORE = [
         "require-runtime-dependencies",
     ]
 
     def initialize(self, version: str, build_data: dict[str, Any]) -> None:
@@ -96,14 +98,15 @@
 
         store = ZippedChromaDBStore(path=store_path)
         corpus = Corpus(store=store)
 
         documentation_path = self.config.get("documentation_path", "documentation")
         examples_path = self.config.get("examples_path", "examples")
         python_libraries = self.config.get("python_libraries", [])
+        r_cran_libraries = self.config.get("r_cran_libraries", [])
 
         if documentation_path and os.path.exists(documentation_path):
             corpus.ingest(
                 embedder_cls=DocumentationEmbedder,
                 loader=LocalFileLoader(locations=[documentation_path]),
                 partition="documentation",
             )
@@ -114,18 +117,26 @@
                 loader=LocalFileLoader(locations=[examples_path]),
                 partition="examples",
             )
 
         if python_libraries:
             corpus.ingest(
                 embedder_cls=PythonEmbedder,
-                loader=PythonLibraryLoader(locations=python_libraries),
+                loader=PythonLibraryLoader(locations=python_libraries, metadata={"language": "python"}),
                 partition="code"
             )
 
+        if r_cran_libraries:
+            with RCRANLocalCache(locations=r_cran_libraries):
+                corpus.ingest(
+                    embedder_cls=CodeEmbedder,
+                    loader=RCRANSourceLoader(locations=r_cran_libraries, metadata={"language": "r"}),
+                    partition="code",
+                )
+
         examples = corpus.store.get_all(partition="examples")
         if examples:
             failures = self.test_examples(examples)
             if failures and not self.config.get("ignore_example_errors", False):
                 # TODO: Finish this
                 # TODO: Should example testing just be in the ExampleEmbedder durring embedding instead of here?
                 print("These examples failed")
@@ -168,78 +179,14 @@
             }
             with open(dest_file, "w") as context_file:
                 json.dump(context_file_contents, context_file, indent=2)
             return slug, dest_file
         else:
             return None, None
 
-            # with open(spec.origin, 'rb') as mod_file:
-            #     symbols = ast.parse(mod_file.read(), filename=spec.origin)
-            # # imports: set[str] = set()
-            # # import_froms: dict[str, str] = []
-            # # classes: list[ast.ClassDef] = []
-
-
-            # for symbol in symbols.body:
-            #     if isinstance(symbol, ast.ClassDef) and "BunsenContext" in [attr.id for attr in getattr(symbol, "bases", [])]:
-            #         class_name = symbol.name
-
-                # if isinstance(symbol, ast.Import):
-                #     imports.update([alias.name for alias in symbol.names])
-                # elif isinstance(symbol, ast.ImportFrom):
-                #     import_froms.append(symbol)
-                # elif isinstance(symbol, ast.ClassDef):
-                #     classes.append(symbol)
-
-            # print(imports)
-            # # print([a.name for i in imports for a in i.names])
-            # print(import_froms)
-            # # print()
-            # print(classes)
-            # for cls in classes:
-            #     for base in cls.bases:
-            #         if isinstance(base, ast.Attribute):
-            #             # parts = [base.attr]
-            #             parts = []
-            #             value = base
-            #             # value = base.value
-            #             while isinstance(value, ast.Attribute):
-            #                 parts.append(value.attr)
-            #                 value = value.value
-            #             if isinstance(value, ast.Name):
-            #                 parts.append(value.id)
-            #             parts.reverse()
-            #             print(parts)
-            #             for i in range(1, len(parts) + 1):
-            #                 key = '.'.join(parts[:i])
-            #                 if key in imports:
-            #                     remainder = parts[i:]
-            #                     print(f"{remainder=}")
-            #                     target = importlib.import_module(key)
-            #                     print(target)
-            #                     dir(target)
-            #                     for attr in remainder:
-            #                         target = getattr(target, attr)
-            #                     print(target)
-
-
-
-
-            #         elif isinstance(base, ast.Name):
-            #             print(base.id)
-
-
-                    # print(base)
-                    # print(base.attr)
-                    # print(base.value.attr)
-                    # print(base.ctx)
-
-
-
-
 
     def test_examples(self, examples):
         # TODO: Finish this
         return []
```

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/chromadb_store.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/chromadb_store.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/types.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/types.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/vector_store.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/vector_store.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/base.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/base.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/code.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/code.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/document.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/document.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/documentation.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/documentation.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/embedders/examples.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/embedders/examples.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/base.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/base.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/code_library_loader.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/local_file_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,139 +1,116 @@
-import importlib
-import importlib.util
-import logging
-import os.path
-import pkgutil
-import sys
+import json
+import os
 from collections import deque
 from pathlib import Path
-from urllib.parse import urlparse
+from typing import Optional
 
 from .base import BaseLoader
-from .schemes import LocalFileScheme, PythonModuleScheme, read_from_uri
+from .schemes import LocalFileScheme, read_from_uri
 from ..types import Resource, Default, DefaultType
 
-logger = logging.getLogger("beaker_bunsen")
 
-class BaseCodeLoader(BaseLoader):
+class LocalFileLoader(BaseLoader):
 
     Scheme = LocalFileScheme
-    # URI_SCHEME = "file"
+    SLUG = "local"
 
-
-class PythonLibraryLoader(BaseCodeLoader):
-
-    Scheme = PythonModuleScheme
-    SLUG = "python"
+    def __init__(
+        self,
+        locations: list[str] | None = None,
+        metadata: dict | None = None,
+        exclusions: list[str] | None = None,
+    ):
+        exclusions = exclusions or []
+        if locations:
+            locations, parsed_exclusions = self.parse_locations(locations)
+            exclusions.extend(parsed_exclusions)
+            self._check_locations_exist(locations)
+        super().__init__(locations, metadata, exclusions)
+
+    @staticmethod
+    def _check_locations_exist(locations: list[str]):
+        missing_locations = []
+        for location in locations:
+            if isinstance(location, Path):
+                location = str(location.absolute())
+            if not os.path.exists(location):
+                missing_locations.append(location)
+        if missing_locations:
+            raise ValueError(f"Paths do not exist: {', '.join(missing_locations)}")
+
+    @staticmethod
+    def collapse_metadata(metadata_list: list[dict|None]):
+        collapsed_metadata = {}
+        for metadata in metadata_list:
+            if metadata is not None:
+                collapsed_metadata.update(metadata)
+        return collapsed_metadata
 
     def discover(
         self,
         locations: list[str] | DefaultType = Default,
         metadata: dict | DefaultType = Default,
         exclusions: list[str] = Default,
     ):
-        """
-        The `locations` should be Python packages, modules or submodules that are installed via the pyproject
-        requirements.  Each location must be importable using the syntax `import {location}`, so you can include
-        either top-level modules such as 'pandas' or submodules such as `pandas.plotting`.  The loader will recurse
-        through and to include anything defined "below" the specified location in the import tree. I.e. location
-        `pandas` will load all submodules, but `pandas.api.extensions` will not import any other submodules under
-        `pandas.api.*` besides what is specified.
-
-        Note: "from" import syntax is not valid. Loading a module loads the entire module and it's submodules and
-        it is not possible to select only certain items from the module.
-
-        Example: locations=["requests", "os.path", "pandas.core", "pandas.util"]
-        """
-        if locations is Default:
-            locations = self.locations
-        if metadata is Default:
-            metadata = self.metadata
+        # Initialize exclusions first so we can extend it if there are any negated locations
         if exclusions is Default:
             exclusions = self.exclusions
 
-        # Update or define locations and exclusions based on '!' prefix in location.
-        locations, parsed_exclusions = self.parse_locations(locations)
-        exclusions.extend(parsed_exclusions)
-
-        modules_to_collect = deque()
-        for module_name in locations:
-            module_spec = importlib.util.find_spec(module_name)
-            if module_spec is None:
-                raise ValueError(f"Module '{module_name}' is not able to be imported. Please ensure that it is listed as a requirement and that 'require-runtime-dependencies' is enabled if error encountered during build.")
-            modules_to_collect.append(module_spec)
+        # Validate locations if they are passed in. If they are not, use location from initialization.
+        if locations is not Default:
+            # Update or define locations and exclusions based on '!' prefix in location.
+            locations, parsed_exclusions = self.parse_locations(locations)
+            exclusions.extend(parsed_exclusions)
+            self._check_locations_exist(locations)
+        else:
+            locations = self.locations
+
+        if locations is None:
+            raise ValueError("No locations specified to discover local files")
 
-        while modules_to_collect:
-            module_spec = modules_to_collect.popleft()
+        if metadata is Default:
+            metadata = {}
+            metadata.update(self.metadata)
+
+        locations_queue = deque((location, [metadata]) for location in locations)
+        while locations_queue:
+            location, location_metadata = locations_queue.popleft()
+            if isinstance(location, Path):
+                location = str(location.absolute())
 
-            if not module_spec.origin.endswith('.py'):
-                logger.info(f"Skipping importing non-python file {module_spec.origin}")
+            if self.should_exclude(str(location)):
                 continue
 
-            if getattr(module_spec, "submodule_search_locations", []):
-                subpkg_info: pkgutil.ModuleInfo = pkgutil.iter_modules(path=module_spec.submodule_search_locations)
-                subpkg_specs = (info.module_finder.find_spec(f"{module_spec.name}.{info.name}") for info in subpkg_info)
-                if self.exclusions:
-                    subpkg_specs = (
-                        spec for spec in subpkg_specs
-                        if not self.should_exclude(spec.name)
-                    )
-                modules_to_collect.extend(
-                    subpkg_specs
-                )
-
-            if hasattr(module_spec, "loader"):
-                source = module_spec.loader.get_source(module_spec.name)
-            else:
-                source = None
-
-            origin_path = Path(module_spec.origin)
-            for sys_path in sys.path:
-                if origin_path.is_relative_to(sys_path):
-                    basedir = sys_path
-                    break
-            else:
-                basedir = ""
-
-            resource = Resource(
-                uri=self.Scheme.get_uri_for_location(module_spec.name),
-                content=source,
-                metadata=metadata,
-                # basedir=basedir
-            )
-            resource.id = self.get_id_for_resource(resource)
-            yield resource
-
-
-    def read(
-            self,
-            location: str,
-            base: str = ""
-        ):
+            if os.path.isdir(location):
+                # Check for directory metadata file
+                dir_metadata_path = os.path.join(location, '.metadata')
+                if os.path.isfile(dir_metadata_path):
+                    with open(dir_metadata_path, 'r') as metadata_file:
+                        dir_metadata = json.load(metadata_file)
+                        location_metadata.append(dir_metadata)
+                locations_queue.extend((os.path.join(location, child), location_metadata[:]) for child in os.listdir(location) if not child.startswith('.'))
+            # Skip pipes, symbolic links, and other non-file types
+            # TODO: maybe allow by configuration
+            elif os.path.isfile(location):
+                if location.endswith(".metadata"):
+                    # Don't load .metadata files as regular files.
+                    # They should be found via the mechanisms below where they are looked for explicitly.
+                    continue
+                metadata_filename = f"{location}.metadata"
+                if os.path.isfile(metadata_filename):
+                    with open(metadata_filename, 'r') as metadata_file:
+                        dir_metadata = json.load(metadata_file)
+                        location_metadata.append(dir_metadata)
+
+                metadata = self.collapse_metadata(location_metadata)
+                with open(location, 'r') as doc:
+                    resource = Resource(uri=self.Scheme.get_uri_for_location(location), file_handle=doc, metadata=metadata)
+                    resource.id = self.get_id_for_resource(resource)
+                    yield resource
+
+    def read(self, location: str, base: str = ""):
         if location.startswith(self.Scheme.URI_SCHEME):
             uri = location
         else:
-            uri = self.Scheme.get_uri_for_location(location, base)
+            uri = self.Scheme.get_uri_for_location(location, base=base)
         return read_from_uri(uri)
-        # uri_parts = urlparse(uri)
-        # if uri_parts.scheme != self.URI_SCHEME:
-        #     return ValueError(f"Provided scheme ({uri_parts.scheme}) does not match expected scheme ({self.URI_SCHEME})")
-        # location = uri_parts.path
-        # with open(location, 'r') as python_file:
-        #     source = python_file.read()
-        # return source
-
-
-# class RLangLoader(BaseCodeLoader):
-#     def discover(self, locations: list[str], metadata: dict = None, *args, **kwargs):
-#         return super().discover(locations, metadata, *args, **kwargs)
-
-#     def load(self, location: str):
-#         return super().load(location)
-
-
-# class GithubLoader(BaseCodeLoader):
-#     def discover(self, locations: list[str], metadata: dict = None, *args, **kwargs):
-#         return super().discover(locations, metadata, *args, **kwargs)
-
-#     def load(self, location: str):
-#         return super().load(location)
```

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/loaders/schemes.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/loaders/schemes.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,50 +2,68 @@
 import inspect
 import os
 import os.path
 import pkgutil
 import sys
 import zipfile
 from abc import ABC, abstractmethod
+from functools import cache
 from pathlib import Path
-from typing import Any, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING, Type
 from urllib.parse import urlparse
 
 if TYPE_CHECKING:
     from ...corpus import Corpus
+    from .base import BaseLoader
 
 
 def _is_scheme(obj: Any):
     return bool(
         inspect.isclass(obj)
         and issubclass(obj, Scheme)
         and callable(getattr(obj, "read", None))
     )
 
+@cache
+def unmap_scheme(scheme: str):
+    current_module = sys.modules[__name__]
+    for _cls_name, cls in inspect.getmembers(current_module, predicate=_is_scheme):
+        cls_uri_scheme = getattr(cls, "URI_SCHEME", None)
+        if cls_uri_scheme is not None and cls_uri_scheme == scheme:
+            return cls
+
+
+def determine_scheme(uri: str) -> "Scheme | None":
+    uri = os.fsdecode(uri)
+    scheme = urlparse(uri).scheme
+    scheme_cls = unmap_scheme(scheme)
+    if scheme_cls:
+            return scheme_cls
+    else:
+        raise ValueError(f"Unable to Scheme for '{scheme}'")
+
 
 def read_from_uri(
     uri: str,
     *args,
     **kwargs,
 ) -> bytes:
-    uri = os.fsdecode(uri)
-    scheme = urlparse(uri).scheme
-    current_module = sys.modules[__name__]
-    for _cls_name, cls in inspect.getmembers(current_module, predicate=_is_scheme):
-        cls_uri_scheme = getattr(cls, "URI_SCHEME", None)
-        if cls_uri_scheme is not None and cls_uri_scheme == scheme:
-            return cls.read(uri, *args, **kwargs)
-    else:
-        raise ValueError(f"Unable to determine loader for scheme '{scheme}'")
+    scheme_cls = determine_scheme(uri)
+    return scheme_cls.read(uri, *args, **kwargs)
 
 
 class Scheme(ABC):
     URI_SCHEME: str
 
     @classmethod
+    def default_loader(cls) -> "Type[BaseLoader]":
+        from .local_file_loader import LocalFileLoader
+        return LocalFileLoader
+
+    @classmethod
     @abstractmethod
     def read(
         cls,
         uri: str,
         *args,
         **kwargs,
     ) -> bytes | str:
@@ -70,14 +88,19 @@
             return f"{cls.URI_SCHEME}:{location}"
 
 
 class LocalFileScheme(Scheme):
     URI_SCHEME = 'file'
 
     @classmethod
+    def default_loader(cls) -> "Type[BaseLoader]":
+        from .local_file_loader import LocalFileLoader
+        return LocalFileLoader
+
+    @classmethod
     def join_parts(cls, *parts: list[str]) -> str:
         return os.path.join(*parts)
 
     @classmethod
     def read(
         cls,
         uri: str,
@@ -97,18 +120,30 @@
                 result = resource_file.read()
         except UnicodeDecodeError:
             with open(path, 'rb') as resource_file:
                 result = resource_file.read()
         return result
 
 
+class ExampleScheme(LocalFileScheme):
+    URI_SCHEME = 'examples'
+
+
+class DocumentationScheme(LocalFileScheme):
+    URI_SCHEME = 'documentation'
+
 
 class PythonModuleScheme(Scheme):
     URI_SCHEME = 'py-mod'
 
+    @classmethod
+    def default_loader(cls) -> "Type[BaseLoader]":
+        from .code_library_loader import PythonLibraryLoader
+        return PythonLibraryLoader
+
     @staticmethod
     def get_module_path(mod_name) -> str | None:
         # Look for file by just looking for the file
         # First, use the loaders provided by the sys.meta_path
         head, *tail = mod_name.split('.')
         for loader in sys.meta_path:
             if not hasattr(loader, "find_spec"):
@@ -251,7 +286,49 @@
         *args,
         **kwargs,
     ):
         parsed_uri = urlparse(uri)
         if parsed_uri.scheme != cls.URI_SCHEME:
             raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
         return corpus.read_resource(parsed_uri.path)
+
+
+class RCranScheme(Scheme):
+    URI_SCHEME = "rcran-package"
+
+    local_file_cache: dict[str, str] = {}
+
+    @classmethod
+    def default_loader(cls) -> "Type[BaseLoader]":
+        from .code_library_loader import RCRANSourceLoader
+        return RCRANSourceLoader
+
+    @classmethod
+    def get_uri_for_location(
+        cls,
+        location: str,
+        base: str = "",
+    ):
+        if not (location and base):
+            raise ValueError(f"Value '{location}' in base '{base}' is not a valid rcran-package location.")
+
+        return f"{cls.URI_SCHEME}:{location}#{base}"
+
+    @classmethod
+    def read(
+        cls,
+        uri: str,
+        *args,
+        **kwargs,
+    ):
+        from .code_library_loader import RCRANLocalCache
+        parsed_uri = urlparse(uri)
+        if parsed_uri.scheme != cls.URI_SCHEME:
+            raise ValueError(f"Provided scheme '{parsed_uri.scheme}' does not match expected scheme '{cls.URI_SCHEME}'.")
+
+        package = parsed_uri.fragment
+        subpath = parsed_uri.path
+        with RCRANLocalCache([package]) as cache:
+            target_file = Path(cache[package]) / subpath
+            with target_file.open() as source:
+                content = source.read()
+        return content
```

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/util/helpers.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/helpers.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/src/beaker_bunsen/vectordb/util/splitters.py` & `beaker_bunsen-0.0.5/src/beaker_bunsen/vectordb/util/splitters.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_base_embedder.py` & `beaker_bunsen-0.0.5/tests/test_base_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_chromadb.py` & `beaker_bunsen-0.0.5/tests/test_chromadb.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_code_loaders.py` & `beaker_bunsen-0.0.5/tests/test_code_loaders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pytest
+from packaging.version import Version
 from pathlib import Path
 from urllib.parse import urlparse
 
 from beaker_bunsen.vectordb.types import Resource
-from beaker_bunsen.vectordb.loaders.code_library_loader import PythonLibraryLoader
+from beaker_bunsen.vectordb.loaders.code_library_loader import PythonLibraryLoader, RCRANSourceLoader, RCRANLocalCache
 
 
 def test_python_module_discovery():
     python_loader = PythonLibraryLoader()
 
     os_records = list(python_loader.discover(locations=["os"]))
     requests_records = list(python_loader.discover(locations=["requests"]))
@@ -91,7 +92,20 @@
 
     assert 'py-mod:requests._internal_utils' in full_record_uris
     assert 'py-mod:requests.__version__' in full_record_uris
     assert 'py-mod:requests._internal_utils' not in excluded_record_uris
     assert 'py-mod:requests.__version__' not in excluded_record_uris
 
     assert set(full_record_uris) - set(excluded_record_uris) == set(['py-mod:requests._internal_utils', 'py-mod:requests.__version__'])
+
+
+def test_r_cran_source_loader():
+    loader = RCRANSourceLoader()
+
+    resources = list(loader.discover(locations=["leaflet"]))
+
+    # TODO: More testing
+
+    assert len(RCRANLocalCache.remote_package_cache) > 0
+    assert "leaflet" in RCRANLocalCache.remote_package_cache
+    assert Version(RCRANLocalCache.remote_package_cache["leaflet"]["version"]) > Version("2.0")
+    assert len(resources) > 0
```

### Comparing `beaker_bunsen-0.0.4/tests/test_corpus.py` & `beaker_bunsen-0.0.5/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_documentation_embedder.py` & `beaker_bunsen-0.0.5/tests/test_documentation_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_example_embedder.py` & `beaker_bunsen-0.0.5/tests/test_example_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_local_file_loader.py` & `beaker_bunsen-0.0.5/tests/test_local_file_loader.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_schemes.py` & `beaker_bunsen-0.0.5/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_utils.py` & `beaker_bunsen-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/test_zipped_chromadb.py` & `beaker_bunsen-0.0.5/tests/test_zipped_chromadb.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/store.zip` & `beaker_bunsen-0.0.5/tests/data/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/corpus.zip` & `beaker_bunsen-0.0.5/tests/data/corpuses/corpus.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/store.zip` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.adapters` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.adapters`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.api` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.api`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.auth` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.auth`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.compat` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.compat`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.cookies` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.cookies`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.exceptions` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.exceptions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.help` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.help`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.hooks` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.hooks`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.models` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.models`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.packages` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.packages`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.sessions` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.sessions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.status_codes` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.status_codes`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.structures` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.structures`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/code/requests.utils` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/code/requests.utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md` & `beaker_bunsen-0.0.5/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.5/tests/data/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documentation/ruff_readme.md` & `beaker_bunsen-0.0.5/tests/data/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documents/Lunar_Sample_Laboratory_Facility.html` & `beaker_bunsen-0.0.5/tests/data/documents/Lunar_Sample_Laboratory_Facility.html`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documents/yorkshire.txt` & `beaker_bunsen-0.0.5/tests/data/documents/yorkshire.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documents/recipes/irish_potato_caserole` & `beaker_bunsen-0.0.5/tests/data/documents/recipes/irish_potato_caserole`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documents/recipes/tajine_maadnous` & `beaker_bunsen-0.0.5/tests/data/documents/recipes/tajine_maadnous`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/documents/recipes/winter_risotto` & `beaker_bunsen-0.0.5/tests/data/documents/recipes/winter_risotto`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/images/kitten-sad.jpg` & `beaker_bunsen-0.0.5/tests/data/images/kitten-sad.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/images/kitten_hacker.jpg` & `beaker_bunsen-0.0.5/tests/data/images/kitten_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/images/puppy_hacker.jpg` & `beaker_bunsen-0.0.5/tests/data/images/puppy_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/images/puppy_sad.png` & `beaker_bunsen-0.0.5/tests/data/images/puppy_sad.png`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/subproject/pyproject.toml` & `beaker_bunsen-0.0.5/tests/data/subproject/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/subproject/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.5/tests/data/subproject/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/tests/data/subproject/documentation/ruff_readme.md` & `beaker_bunsen-0.0.5/tests/data/subproject/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/.gitignore` & `beaker_bunsen-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/LICENSE.txt` & `beaker_bunsen-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/README.md` & `beaker_bunsen-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.4/pyproject.toml` & `beaker_bunsen-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -26,20 +26,26 @@
   "beaker-kernel~=1.5.1",
   "archytas~=1.1.6",
   "chromadb~=0.4.22",
   "tenacity~=8.2.3",
   "tiktoken~=0.5.2",
   "marko~=2.0.3",
   "hatchling",
+  "click~=8.1.7",
 ]
-  # "pysqlite3-binary~=0.5.2",
+
+[project.scripts]
+bunsen= "beaker_bunsen.scripts.bunsen:cli"
 
 [project.entry-points.hatch]
 bunsen = "beaker_bunsen.builder.hooks"
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [project.urls]
 Documentation = "https://github.com/unknown/beaker-bunsen#readme"
 Issues = "https://github.com/unknown/beaker-bunsen/issues"
 Source = "https://github.com/unknown/beaker-bunsen"
 
 [tool.hatch.build]
 require-runtime-dependencies = true
```

### Comparing `beaker_bunsen-0.0.4/PKG-INFO` & `beaker_bunsen-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beaker-bunsen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Quickly generate new Beaker contexts for new domains and libraries.
 Project-URL: Documentation, https://github.com/unknown/beaker-bunsen#readme
 Project-URL: Issues, https://github.com/unknown/beaker-bunsen/issues
 Project-URL: Source, https://github.com/unknown/beaker-bunsen
 Author-email: Matthew Printz <matt@jataware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: archytas~=1.1.6
 Requires-Dist: beaker-kernel~=1.5.1
 Requires-Dist: chromadb~=0.4.22
+Requires-Dist: click~=8.1.7
 Requires-Dist: hatchling
 Requires-Dist: marko~=2.0.3
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: tiktoken~=0.5.2
 Description-Content-Type: text/markdown
 
 # beaker-bunsen
```

