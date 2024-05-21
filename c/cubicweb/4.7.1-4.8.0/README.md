# Comparing `tmp/cubicweb-4.7.1.tar.gz` & `tmp/cubicweb-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-4.7.1.tar", last modified: Fri Apr 19 09:51:48 2024, max compression
+gzip compressed data, was "cubicweb-4.8.0.tar", last modified: Tue May 21 12:44:37 2024, max compression
```

## Comparing `cubicweb-4.7.1.tar` & `cubicweb-4.8.0.tar`

### file list

```diff
@@ -1,1320 +1,1321 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.820646 cubicweb-4.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-19 09:51:16.000000 cubicweb-4.7.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    17987 2024-04-19 09:51:16.000000 cubicweb-4.7.1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    26527 2024-04-19 09:51:16.000000 cubicweb-4.7.1/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)     4977 2024-04-19 09:51:16.000000 cubicweb-4.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5161 2024-04-19 09:51:48.820646 cubicweb-4.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.320640 cubicweb-4.7.1/cubicweb/
--rw-rw-rw-   0 root         (0) root         (0)     7503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       69 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     6885 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3860 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/_gcdebug.py
--rw-rw-rw-   0 root         (0) root         (0)     5211 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/appobject.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)    66337 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    32638 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)     4899 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwgettext.py
--rw-rw-rw-   0 root         (0) root         (0)    25982 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwvreg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.328640 cubicweb-4.7.1/cubicweb/dataimport/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    21081 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/importer.py
--rw-rw-rw-   0 root         (0) root         (0)    26515 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/massive_store.py
--rw-rw-rw-   0 root         (0) root         (0)    15503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/pgstore.py
--rw-rw-rw-   0 root         (0) root         (0)    18127 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/stores.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.332640 cubicweb-4.7.1/cubicweb/dataimport/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.332640 cubicweb-4.7.1/cubicweb/dataimport/test/data/
--rw-rw-rw-   0 root         (0) root         (0)   474710 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/geonames.csv
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/people.csv
--rw-rw-rw-   0 root         (0) root         (0)     1231 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/timeZones.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.336640 cubicweb-4.7.1/cubicweb/dataimport/test/data-massimport/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data-massimport/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_csv.py
--rw-rw-rw-   0 root         (0) root         (0)    16176 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_massive_store.py
--rw-rw-rw-   0 root         (0) root         (0)     4179 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_pgstore.py
--rw-rw-rw-   0 root         (0) root         (0)     8221 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/unittest_importer.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.340640 cubicweb-4.7.1/cubicweb/devtools/
--rw-rw-rw-   0 root         (0) root         (0)    27112 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5449 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/apptest_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.340640 cubicweb-4.7.1/cubicweb/devtools/data/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/data/cwmock.js
--rw-rw-rw-   0 root         (0) root         (0)     5146 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/data/qunit.css
--rw-rw-rw-   0 root         (0) root         (0)   115758 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/data/qunit.js
--rw-rw-rw-   0 root         (0) root         (0)    39808 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/devctl.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/fake.py
--rw-rw-rw-   0 root         (0) root         (0)    24531 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/fill.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/fix_po_encoding
--rw-rw-rw-   0 root         (0) root         (0)    10982 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/htmlparser.py
--rw-rw-rw-   0 root         (0) root         (0)     5298 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/httptest.py
--rw-rw-rw-   0 root         (0) root         (0)     9195 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/realdbtest.py
--rw-rw-rw-   0 root         (0) root         (0)    10873 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/repotest.py
--rw-rw-rw-   0 root         (0) root         (0)     6796 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/stresstester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.344640 cubicweb-4.7.1/cubicweb/devtools/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.344640 cubicweb-4.7.1/cubicweb/devtools/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)    11311 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/firstnames.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.240639 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
--rw-rw-rw-   0 root         (0) root         (0)     1720 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.244639 cubicweb-4.7.1/cubicweb/devtools/test/data/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.352640 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/dep_1.js
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/deps_2.js
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4354 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_dbfill.py
--rw-rw-rw-   0 root         (0) root         (0)     6402 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_devctl.py
--rw-rw-rw-   0 root         (0) root         (0)     2475 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_fill.py
--rw-rw-rw-   0 root         (0) root         (0)     3225 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     4687 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_testlib.py
--rw-rw-rw-   0 root         (0) root         (0)    20848 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/testlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.352640 cubicweb-4.7.1/cubicweb/entities/
--rw-rw-rw-   0 root         (0) root         (0)     5324 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24563 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/authobjs.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     5944 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/schemaobjs.py
--rw-rw-rw-   0 root         (0) root         (0)     4095 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/entities/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/entities/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/entities/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9992 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/unittest_base.py
--rw-rw-rw-   0 root         (0) root         (0)    36719 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/unittest_wfobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    22858 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/wfobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    59384 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/ext/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5821 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/html4zope.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/ext/test/
--rw-rw-rw-   0 root         (0) root         (0)     2013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/test/unittest_markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.364640 cubicweb-4.7.1/cubicweb/hooks/
--rw-rw-rw-   0 root         (0) root         (0)     4593 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/email.py
--rw-rw-rw-   0 root         (0) root         (0)    13217 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     5680 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     9725 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     8157 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/security.py
--rw-rw-rw-   0 root         (0) root         (0)    10630 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/synccomputed.py
--rw-rw-rw-   0 root         (0) root         (0)    60802 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/syncschema.py
--rw-rw-rw-   0 root         (0) root         (0)     4913 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/syncsession.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/syncsources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.368641 cubicweb-4.7.1/cubicweb/hooks/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.368641 cubicweb-4.7.1/cubicweb/hooks/test/data/
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.368641 cubicweb-4.7.1/cubicweb/hooks/test/data-computed/
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/data-computed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_bookmarks.py
--rw-rw-rw-   0 root         (0) root         (0)    13062 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     8490 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_notificationhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_security.py
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_synccomputed.py
--rw-rw-rw-   0 root         (0) root         (0)    24424 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncschema.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsession.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsources.py
--rw-rw-rw-   0 root         (0) root         (0)    15886 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.372640 cubicweb-4.7.1/cubicweb/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    93082 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/de.po
--rw-rw-rw-   0 root         (0) root         (0)    61668 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)   112148 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)   106920 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     3749 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     5624 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3352 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/md5crypt.py
--rw-rw-rw-   0 root         (0) root         (0)    22356 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/migration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.372640 cubicweb-4.7.1/cubicweb/misc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.376641 cubicweb-4.7.1/cubicweb/misc/migration/
--rw-rw-rw-   0 root         (0) root         (0)      688 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.22.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.22.1_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.22.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.23.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.24.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.24.4_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.27.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.30.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.31.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.32.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.38.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)    20108 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/bootstrapmigration_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/postcreate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.380641 cubicweb-4.7.1/cubicweb/misc/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/chpasswd.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/detect_cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     5710 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/fast_drop_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/ldap_change_base_dn.py
--rw-rw-rw-   0 root         (0) root         (0)     3466 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/migration_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/source_highlight.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/mttransforms.py
--rw-rw-rw-   0 root         (0) root         (0)    17397 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/multipart.py
--rw-rw-rw-   0 root         (0) root         (0)    50906 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/predicates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.388641 cubicweb-4.7.1/cubicweb/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     9523 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4474 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/csrf.py
--rw-rw-rw-   0 root         (0) root         (0)     7077 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_source_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.388641 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
--rw-rw-rw-   0 root         (0) root         (0)     3912 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     4852 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     2980 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     8484 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debugtoolbar_panels.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/default_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/development.ini.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     3767 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/pyramid.ini.tmpl
--rw-rw-rw-   0 root         (0) root         (0)    13622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/pyramidctl.py
--rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     7395 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     9651 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.392641 cubicweb-4.7.1/cubicweb/pyramid/test/
--rw-rw-rw-   0 root         (0) root         (0)     2447 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.392641 cubicweb-4.7.1/cubicweb/pyramid/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.392641 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3624 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     3652 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_content_negociation.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1929 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/repoapi.py
--rw-rw-rw-   0 root         (0) root         (0)    17494 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/req.py
--rw-rw-rw-   0 root         (0) root         (0)    41745 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rqlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)    11503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rqlsuggestions.py
--rw-rw-rw-   0 root         (0) root         (0)    27291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rset.py
--rw-rw-rw-   0 root         (0) root         (0)    11656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rtags.py
--rw-rw-rw-   0 root         (0) root         (0)    57848 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     6149 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schema_exporters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.396641 cubicweb-4.7.1/cubicweb/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     2279 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/Bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/_regproc.postgres.sql
--rw-rw-rw-   0 root         (0) root         (0)    13898 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15024 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    11853 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.404641 cubicweb-4.7.1/cubicweb/server/
--rw-rw-rw-   0 root         (0) root         (0)    14107 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/check_unused_index.py
--rw-rw-rw-   0 root         (0) root         (0)    23043 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/checkintegrity.py
--rw-rw-rw-   0 root         (0) root         (0)     6110 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/edition.py
--rw-rw-rw-   0 root         (0) root         (0)    38571 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/hook.py
--rw-rw-rw-   0 root         (0) root         (0)    77833 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/migractions.py
--rw-rw-rw-   0 root         (0) root         (0)    35925 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/querier.py
--rw-rw-rw-   0 root         (0) root         (0)    47931 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/repository.py
--rw-rw-rw-   0 root         (0) root         (0)    19156 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/rqlannotation.py
--rw-rw-rw-   0 root         (0) root         (0)    13785 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/schema2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    28692 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/schemaserial.py
--rw-rw-rw-   0 root         (0) root         (0)     3168 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/serverconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    56204 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/serverctl.py
--rw-rw-rw-   0 root         (0) root         (0)    32564 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.408641 cubicweb-4.7.1/cubicweb/server/sources/
--rw-rw-rw-   0 root         (0) root         (0)    13281 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18181 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/datafeed.py
--rw-rw-rw-   0 root         (0) root         (0)    16896 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/ldapfeed.py
--rw-rw-rw-   0 root         (0) root         (0)    78080 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/native.py
--rw-rw-rw-   0 root         (0) root         (0)    71034 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/rql2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    11149 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/storages.py
--rw-rw-rw-   0 root         (0) root         (0)    22712 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)    22485 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/ssplanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.416641 cubicweb-4.7.1/cubicweb/server/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.420641 cubicweb-4.7.1/cubicweb/server/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.448641 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.448641 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.452642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.452642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.452642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/ldap_test.ldif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/slapd.conf.in
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/sources_extern
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/sources_multi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-cwep002/
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-cwep002/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.428641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.428641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.436641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.436641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.436641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.440641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.440641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.440641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.444641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.444641 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.444641 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Company.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Dates.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/State.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/toignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.448641 cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/
--rw-rw-rw-   0 root         (0) root         (0)     1345 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8829 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_datafeed.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_edition.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_hook.py
--rw-rw-rw-   0 root         (0) root         (0)    26126 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_ldapsource.py
--rw-rw-rw-   0 root         (0) root         (0)    96689 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_querier.py
--rw-rw-rw-   0 root         (0) root         (0)   101040 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_rql2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    23306 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_rqlannotation.py
--rw-rw-rw-   0 root         (0) root         (0)    11087 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_schema2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    28561 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_schemaserial.py
--rw-rw-rw-   0 root         (0) root         (0)    38100 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_server_security.py
--rw-rw-rw-   0 root         (0) root         (0)     5431 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_serverctl.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_sources_native.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_ssplanner.py
--rw-rw-rw-   0 root         (0) root         (0)    17465 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21764 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_undo.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.460642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.460642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.460642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.464642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.464642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.464642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.468642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.468642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     3596 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.468642 cubicweb-4.7.1/cubicweb/server/test_migractions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.472642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.492642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.472642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.472642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.476642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.476642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.476642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.480642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.480642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.480642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.484642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.484642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.484642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.488642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.488642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.488642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.492642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.492642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    47791 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.524643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.528643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.528643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.528643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.508642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.508642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.512642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.512642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.512642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.516642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.516642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.516642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.520642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.520642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.520642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.524643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.524643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9724 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.536643 cubicweb-4.7.1/cubicweb/server/test_migractions3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.536643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.560643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.560643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.560643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.536643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.540643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.540643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.540643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.544643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.544643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.544643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.548643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.548643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.548643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.552643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.552643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.552643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.556643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.556643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.556643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.568643 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.568643 cubicweb-4.7.1/cubicweb/server/test_postgres/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.568643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.572643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.572643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.572643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.576643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.576643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.576643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.580643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/unittest_postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.580643 cubicweb-4.7.1/cubicweb/server/test_repository/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.580643 cubicweb-4.7.1/cubicweb/server/test_repository/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.584643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.584643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.588643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.588643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.592643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.592643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.584643 cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/
--rw-rw-rw-   0 root         (0) root         (0)     1345 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    38041 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/unittest_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     5178 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.596644 cubicweb-4.7.1/cubicweb/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/.gitlab-ci.yml.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/.hgignore.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/.yamllint.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/Dockerfile.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      367 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/MANIFEST.in.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/README.rst.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.600643 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.600643 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/data/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/migration/
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     2030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     2001 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/test/realdb_test_CUBENAME.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/tox.ini.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.608644 cubicweb-4.7.1/cubicweb/smoke_test/
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.608644 cubicweb-4.7.1/cubicweb/sobjects/
--rw-rw-rw-   0 root         (0) root         (0)     1364 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12938 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/ldapparser.py
--rw-rw-rw-   0 root         (0) root         (0)    14419 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/services.py
--rw-rw-rw-   0 root         (0) root         (0)     8236 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/supervising.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.612644 cubicweb-4.7.1/cubicweb/sobjects/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.612644 cubicweb-4.7.1/cubicweb/sobjects/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.612644 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.616644 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.616644 cubicweb-4.7.1/cubicweb/sobjects/test/data/sobjects/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/sobjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4020 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_email.py
--rw-rw-rw-   0 root         (0) root         (0)     3059 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5404 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_register_user.py
--rw-rw-rw-   0 root         (0) root         (0)     5051 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_supervising.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.624644 cubicweb-4.7.1/cubicweb/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.628644 cubicweb-4.7.1/cubicweb/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.636644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.636644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/entities.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/views/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/entities/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/hooks/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.644644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.644644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.644644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/ccplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.648644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/
--rw-rw-rw-   0 root         (0) root         (0)      857 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.648644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/erqlexpr_on_ertype.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/lowered_etype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.652644 cubicweb-4.7.1/cubicweb/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.0.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.0.4_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_common.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rqlexpr_on_computedrel.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rqlexpr_on_ertype_read.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_attr.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_eetype.py
--rw-rw-rw-   0 root         (0) root         (0)     4319 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.652644 cubicweb-4.7.1/cubicweb/test/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/scripts/script1.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/scripts/script2.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/scripts/script3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.656644 cubicweb-4.7.1/cubicweb/test/data/server_migration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/2.10.2_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/2.5.0_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/2.6.0_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)      882 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/uppered_rtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.632644 cubicweb-4.7.1/cubicweb/test/data-rewrite/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.632644 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.632644 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.656644 cubicweb-4.7.1/cubicweb/test/data_schemareader/
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data_schemareader/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_binary.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_crypto.py
--rw-rw-rw-   0 root         (0) root         (0)    17592 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_cwconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     7457 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)    48020 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     4855 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_fast_drop_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     8357 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_mail.py
--rw-rw-rw-   0 root         (0) root         (0)     7471 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_migration.py
--rw-rw-rw-   0 root         (0) root         (0)    15441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     3879 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_repoapi.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_req.py
--rw-rw-rw-   0 root         (0) root         (0)    46300 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rqlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     6503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rqlsuggestions.py
--rw-rw-rw-   0 root         (0) root         (0)    32589 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rset.py
--rw-rw-rw-   0 root         (0) root         (0)     6543 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rtags.py
--rw-rw-rw-   0 root         (0) root         (0)    34435 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_toolsutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9658 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_uilib.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_vregistry.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_wfutils.py
--rw-rw-rw-   0 root         (0) root         (0)    16545 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/toolsutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)    19530 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/uilib.py
--rw-rw-rw-   0 root         (0) root         (0)    12356 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/wfutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/xy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.816646 cubicweb-4.7.1/cubicweb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5161 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    51739 2024-04-19 09:51:48.000000 cubicweb-4.7.1/cubicweb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.660644 cubicweb-4.7.1/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7511 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/4.0.0_how_to_migrate.rst
--rw-rw-rw-   0 root         (0) root         (0)     2811 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.660644 cubicweb-4.7.1/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)    34494 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/_static/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     9202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/_static/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/announce.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     1982 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/announce.fr.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.668645 cubicweb-4.7.1/doc/api/
--rw-rw-rw-   0 root         (0) root         (0)     2251 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/__init__.rst
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/appobject.rst
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/cwvreg.rst
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/dataimport.rst
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2540 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/predicates.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.668645 cubicweb-4.7.1/doc/api/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/auth.rst
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/bwcompat.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/core.rst
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/login.rst
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/profile.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/session.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/url_redirection.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid.rst
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/req.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/rset.rst
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/urlpublishing.rst
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/urlrewrite.rst
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/web.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.672644 cubicweb-4.7.1/doc/book/
--rw-rw-rw-   0 root         (0) root         (0)    14655 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-app.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     7806 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-gae-app.en.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.672644 cubicweb-4.7.1/doc/book/_maybe_to_integrate/
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/_maybe_to_integrate/D050-architecture.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/_maybe_to_integrate/rss-xml.rst
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/_maybe_to_integrate/template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.672644 cubicweb-4.7.1/doc/book/additionnal_services/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/additionnal_services/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    13562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/additionnal_services/undo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.680645 cubicweb-4.7.1/doc/book/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/backups.rst
--rw-rw-rw-   0 root         (0) root         (0)     5658 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/config.rst
--rw-rw-rw-   0 root         (0) root         (0)     3879 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/create-instance.rst
--rw-rw-rw-   0 root         (0) root         (0)     3396 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/cubicweb-ctl.rst
--rw-rw-rw-   0 root         (0) root         (0)     4034 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/deploy.rst
--rw-rw-rw-   0 root         (0) root         (0)      409 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5265 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/instance-config.rst
--rw-rw-rw-   0 root         (0) root         (0)     4825 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/ldap.rst
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/multisources.rst
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/rql-logs.rst
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/setup.rst
--rw-rw-rw-   0 root         (0) root         (0)     3596 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/site-config.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.680645 cubicweb-4.7.1/doc/book/annexes/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/depends.rst
--rw-rw-rw-   0 root         (0) root         (0)     3257 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/docstrings-conventions.rst
--rw-rw-rw-   0 root         (0) root         (0)    16153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/faq.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/mercurial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.684645 cubicweb-4.7.1/doc/book/annexes/rql/
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/Graph-ex.gif
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/debugging.rst
--rw-rw-rw-   0 root         (0) root         (0)     4697 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/implementation.rst
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5570 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/intro.rst
--rw-rw-rw-   0 root         (0) root         (0)    27490 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/language.rst
--rw-rw-rw-   0 root         (0) root         (0)     2703 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/usecases.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.688645 cubicweb-4.7.1/doc/book/devrepo/
--rw-rw-rw-   0 root         (0) root         (0)     2147 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/connections_pooler.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.692645 cubicweb-4.7.1/doc/book/devrepo/cubes/
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/available-cubes.rst
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/cc-newcube.rst
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6827 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/layout.rst
--rw-rw-rw-   0 root         (0) root         (0)     1967 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/what-is-a-cube.rst
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/dataimport.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.692645 cubicweb-4.7.1/doc/book/devrepo/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)     1389 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/baseschema.rst
--rw-rw-rw-   0 root         (0) root         (0)     6178 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/define-workflows.rst
--rw-rw-rw-   0 root         (0) root         (0)    34880 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/definition.rst
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/metadata.rst
--rw-rw-rw-   0 root         (0) root         (0)     2940 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/debug_channels.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.696645 cubicweb-4.7.1/doc/book/devrepo/devcore/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/devcore/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/devcore/reqbase.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.696645 cubicweb-4.7.1/doc/book/devrepo/entityclasses/
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/adapters.rst
--rw-rw-rw-   0 root         (0) root         (0)     7268 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/application-logic.rst
--rw-rw-rw-   0 root         (0) root         (0)     5285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/data-as-objects.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/load-sort.rst
--rw-rw-rw-   0 root         (0) root         (0)     4399 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/fti.rst
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9469 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/migration.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/profiling.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.700645 cubicweb-4.7.1/doc/book/devrepo/repo/
--rw-rw-rw-   0 root         (0) root         (0)     9731 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/hooks.rst
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)    11467 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/sessions.rst
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/tasks.rst
--rw-rw-rw-   0 root         (0) root         (0)    21316 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)    18289 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/vreg.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.704645 cubicweb-4.7.1/doc/book/devweb/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/ajax.rst
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/controllers.rst
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/css.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.708645 cubicweb-4.7.1/doc/book/devweb/edition/
--rw-rw-rw-   0 root         (0) root         (0)    11979 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/dissection.rst
--rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/editcontroller.rst
--rw-rw-rw-   0 root         (0) root         (0)     9905 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)    15506 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/form.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/facets.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/httpcaching.rst
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    10057 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/internationalization.rst
--rw-rw-rw-   0 root         (0) root         (0)    14107 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/js.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/property.rst
--rw-rw-rw-   0 root         (0) root         (0)     2017 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/publisher.rst
--rw-rw-rw-   0 root         (0) root         (0)     5119 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/request.rst
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/resource.rst
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/rtags.rst
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/searchbar.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.716645 cubicweb-4.7.1/doc/book/devweb/views/
--rw-rw-rw-   0 root         (0) root         (0)     5889 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/basetemplates.rst
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/baseviews.rst
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/boxes.rst
--rw-rw-rw-   0 root         (0) root         (0)     2320 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/breadcrumbs.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/idownloadable.rst
--rw-rw-rw-   0 root         (0) root         (0)      476 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    10179 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/primary.rst
--rw-rw-rw-   0 root         (0) root         (0)     5991 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/reledit.rst
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/startup.rst
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/table.rst
--rw-rw-rw-   0 root         (0) root         (0)     5506 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/urlpublish.rst
--rw-rw-rw-   0 root         (0) root         (0)     4192 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/views.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/wdoc.rst
--rw-rw-rw-   0 root         (0) root         (0)     1703 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/xmlrss.rst
--rw-rw-rw-   0 root         (0) root         (0)      947 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/warning.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.716645 cubicweb-4.7.1/doc/book/intro/
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/intro/concepts.rst
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/intro/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      385 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/intro/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.720645 cubicweb-4.7.1/doc/book/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/auth.rst
--rw-rw-rw-   0 root         (0) root         (0)     1314 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/ctl.rst
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/debug_toolbar.rst
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1795 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     5411 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/settings.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.720645 cubicweb-4.7.1/doc/book/security/
--rw-rw-rw-   0 root         (0) root         (0)     8041 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/security/csrf.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.720645 cubicweb-4.7.1/doc/book/src/
--rw-rw-rw-   0 root         (0) root         (0)     2930 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/src/archi_globale.dia
--rw-rw-rw-   0 root         (0) root         (0)     1735 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/src/main_template_layout.dia
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.736645 cubicweb-4.7.1/doc/changes/
--rw-rw-rw-   0 root         (0) root         (0)     6619 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.14.rst
--rw-rw-rw-   0 root         (0) root         (0)     3904 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.15.rst
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.16.rst
--rw-rw-rw-   0 root         (0) root         (0)     1815 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.17.rst
--rw-rw-rw-   0 root         (0) root         (0)     3632 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.18.rst
--rw-rw-rw-   0 root         (0) root         (0)     6757 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.19.rst
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.20.rst
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.21.rst
--rw-rw-rw-   0 root         (0) root         (0)     3689 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.22.rst
--rw-rw-rw-   0 root         (0) root         (0)     2799 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.23.rst
--rw-rw-rw-   0 root         (0) root         (0)     4033 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.24.rst
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.25.rst
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.26.rst
--rw-rw-rw-   0 root         (0) root         (0)     6870 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.27.rst
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.28.rst
--rw-rw-rw-   0 root         (0) root         (0)     1249 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.29.rst
--rw-rw-rw-   0 root         (0) root         (0)     5588 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.30.rst
--rw-rw-rw-   0 root         (0) root         (0)     3683 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.31.rst
--rw-rw-rw-   0 root         (0) root         (0)     7979 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.32.rst
--rw-rw-rw-   0 root         (0) root         (0)     1728 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.32_reledit.rst
--rw-rw-rw-   0 root         (0) root         (0)     5635 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.33.rst
--rw-rw-rw-   0 root         (0) root         (0)     4524 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.34.rst
--rw-rw-rw-   0 root         (0) root         (0)     4849 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.35.rst
--rw-rw-rw-   0 root         (0) root         (0)     4507 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.36.rst
--rw-rw-rw-   0 root         (0) root         (0)     5437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.37.rst
--rw-rw-rw-   0 root         (0) root         (0)     8870 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.38.rst
--rw-rw-rw-   0 root         (0) root         (0)     6425 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      746 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     7654 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.796646 cubicweb-4.7.1/doc/images/
--rw-rw-rw-   0 root         (0) root         (0)    98393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/03-transitions-view_en.png
--rw-rw-rw-   0 root         (0) root         (0)    12650 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/breadcrumbs_header.png
--rw-rw-rw-   0 root         (0) root         (0)    85073 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_general_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   124385 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_registry_content_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   111325 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_registry_decisions_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   134505 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_rql_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   192629 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_rql_traceback_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   107766 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_show_source.png
--rw-rw-rw-   0 root         (0) root         (0)    55625 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_show_source_link.png
--rw-rw-rw-   0 root         (0) root         (0)   126845 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_sql_panel.png
--rw-rw-rw-   0 root         (0) root         (0)    97343 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_traceback_source_link.png
--rw-rw-rw-   0 root         (0) root         (0)    57300 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/example-card-with-rql-directive.png
--rw-rw-rw-   0 root         (0) root         (0)    55168 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/example-card-with-rql-table-directive.png
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_date_range.png
--rw-rw-rw-   0 root         (0) root         (0)     6013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_has_image.png
--rw-rw-rw-   0 root         (0) root         (0)    22016 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_overview.png
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_range.png
--rw-rw-rw-   0 root         (0) root         (0)    21685 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_00-login_en.png
--rw-rw-rw-   0 root         (0) root         (0)    30326 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_01-start_en.png
--rw-rw-rw-   0 root         (0) root         (0)    35859 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_02-cookie-values_en.png
--rw-rw-rw-   0 root         (0) root         (0)    33922 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_02-create-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    28123 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-list-one-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    82897 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-site-config-panel_en.png
--rw-rw-rw-   0 root         (0) root         (0)   119813 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-state-submitted_en.png
--rw-rw-rw-   0 root         (0) root         (0)    98393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-transitions-view_en.png
--rw-rw-rw-   0 root         (0) root         (0)    34771 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_04-detail-one-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    28345 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_05-list-two-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    49230 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_06-add-relation-entryof_en.png
--rw-rw-rw-   0 root         (0) root         (0)    96838 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_06-main-template-logo_en.png
--rw-rw-rw-   0 root         (0) root         (0)    40383 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_07-detail-one-blogentry_en.png
--rw-rw-rw-   0 root         (0) root         (0)    30591 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_08-schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    33091 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_09-new-view-blogentry_en.png
--rw-rw-rw-   0 root         (0) root         (0)    42230 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_10-blog-with-two-entries_en.png
--rw-rw-rw-   0 root         (0) root         (0)    17757 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/main_template.png
--rw-rw-rw-   0 root         (0) root         (0)     8674 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/main_template.svg
--rw-rw-rw-   0 root         (0) root         (0)    13842 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/main_template_layout.png
--rw-rw-rw-   0 root         (0) root         (0)    46411 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/primaryview_template.png
--rw-rw-rw-   0 root         (0) root         (0)    14758 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/primaryview_template.svg
--rw-rw-rw-   0 root         (0) root         (0)    22773 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/request_session.png
--rw-rw-rw-   0 root         (0) root         (0)     7211 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/request_session.svg
--rw-rw-rw-   0 root         (0) root         (0)    12030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/server-class-diagram.png
--rw-rw-rw-   0 root         (0) root         (0)    62022 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blog-form_en.png
--rw-rw-rw-   0 root         (0) root         (0)   105173 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blog-primary-after-post-creation_en.png
--rw-rw-rw-   0 root         (0) root         (0)    58500 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blog-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    42013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blogs-list_en.png
--rw-rw-rw-   0 root         (0) root         (0)   109769 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_form-generic-relations_en.png
--rw-rw-rw-   0 root         (0) root         (0)    65646 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_index_en.png
--rw-rw-rw-   0 root         (0) root         (0)    13605 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_index_gettext_en.png
--rw-rw-rw-   0 root         (0) root         (0)    88970 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_index_logged_in_en.png
--rw-rw-rw-   0 root         (0) root         (0)    11548 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_login-form_en.png
--rw-rw-rw-   0 root         (0) root         (0)   100347 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    63097 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-community-custom-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    62431 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-community-default-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    74856 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-community-taggable-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    79709 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-custom-footer_en.png
--rw-rw-rw-   0 root         (0) root         (0)   128406 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    71500 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-siteinfo_en.png
--rw-rw-rw-   0 root         (0) root         (0)   104834 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    22098 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_schema_graphviz_en.png
--rw-rw-rw-   0 root         (0) root         (0)   150520 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_siteconfig_en.png
--rw-rw-rw-   0 root         (0) root         (0)    60672 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_admin.png
--rw-rw-rw-   0 root         (0) root         (0)    61388 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_city_created.png
--rw-rw-rw-   0 root         (0) root         (0)    50694 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_city_creation.png
--rw-rw-rw-   0 root         (0) root         (0)    71561 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_data_model_schema.png
--rw-rw-rw-   0 root         (0) root         (0)    48896 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_empty_instance.png
--rw-rw-rw-   0 root         (0) root         (0)    55671 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_finished_import.png
--rw-rw-rw-   0 root         (0) root         (0)    57063 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_list_view.png
--rw-rw-rw-   0 root         (0) root         (0)    70893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_museum_created.png
--rw-rw-rw-   0 root         (0) root         (0)    61656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_museum_creation.png
--rw-rw-rw-   0 root         (0) root         (0)    74005 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_museum_with_city_name.png
--rw-rw-rw-   0 root         (0) root         (0)   225824 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_react_map.png
--rw-rw-rw-   0 root         (0) root         (0)    53544 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_with_schema.png
--rw-rw-rw-   0 root         (0) root         (0)   354637 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_background-image.png
--rw-rw-rw-   0 root         (0) root         (0)    30437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_boxes.png
--rw-rw-rw-   0 root         (0) root         (0)    54643 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_breadcrumbs.png
--rw-rw-rw-   0 root         (0) root         (0)   324086 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_facets.png
--rw-rw-rw-   0 root         (0) root         (0)    40520 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_grey-box.png
--rw-rw-rw-   0 root         (0) root         (0)    16843 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_index-after.png
--rw-rw-rw-   0 root         (0) root         (0)    26875 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_index-before.png
--rw-rw-rw-   0 root         (0) root         (0)    17580 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_login-box.png
--rw-rw-rw-   0 root         (0) root         (0)    57814 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_prevnext.png
--rw-rw-rw-   0 root         (0) root         (0)    81362 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_ui1.png
--rw-rw-rw-   0 root         (0) root         (0)    93291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_ui2.png
--rw-rw-rw-   0 root         (0) root         (0)   290338 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_ui3.png
--rw-rw-rw-   0 root         (0) root         (0)    43051 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/undo_history-view_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    26036 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/undo_mesage_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    39625 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/undo_startup-link_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    17558 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table-filter-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)    14013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table-filter.png
--rw-rw-rw-   0 root         (0) root         (0)    12375 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)     9676 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table.png
--rw-rw-rw-   0 root         (0) root         (0)     7344 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/plan_formation_python_cubicweb.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/stdlib.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.800646 cubicweb-4.7.1/doc/tools/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tools/generate_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tools/mode_plan.py
--rwxrwxrwx   0 root         (0) root         (0)     4944 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tools/pyjsrest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.800646 cubicweb-4.7.1/doc/tutorials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.800646 cubicweb-4.7.1/doc/tutorials/advanced/
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5486 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part01_create-cube.rst
--rw-rw-rw-   0 root         (0) root         (0)    17016 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part02_security.rst
--rw-rw-rw-   0 root         (0) root         (0)     5614 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part03_bfss.rst
--rw-rw-rw-   0 root         (0) root         (0)    15384 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part04_ui-base.rst
--rw-rw-rw-   0 root         (0) root         (0)    15114 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part05_ui-advanced.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.804646 cubicweb-4.7.1/doc/tutorials/base/
--rw-rw-rw-   0 root         (0) root         (0)     3867 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/blog-in-five-minutes.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/conclusion.rst
--rw-rw-rw-   0 root         (0) root         (0)    20435 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/customizing-the-application.rst
--rw-rw-rw-   0 root         (0) root         (0)     7821 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/discovering-the-ui.rst
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.804646 cubicweb-4.7.1/doc/tutorials/dataimport/
--rw-rw-rw-   0 root         (0) root         (0)     9014 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_import.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    29917 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6576 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.808646 cubicweb-4.7.1/doc/tutorials/museum/
--rw-rw-rw-   0 root         (0) root         (0)     5961 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/data-management.rst
--rw-rw-rw-   0 root         (0) root         (0)     6403 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/develop-app.rst
--rw-rw-rw-   0 root         (0) root         (0)     3860 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/develop-ui.rst
--rw-rw-rw-   0 root         (0) root         (0)     8840 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/enhance-views.rst
--rw-rw-rw-   0 root         (0) root         (0)     2702 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/getting-started.rst
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.808646 cubicweb-4.7.1/extras/
--rw-rw-rw-   0 root         (0) root         (0)     3545 2024-04-19 09:51:16.000000 cubicweb-4.7.1/extras/cubicweb-ctl.bash_completion
--rw-rw-rw-   0 root         (0) root         (0)     7414 2024-04-19 09:51:16.000000 cubicweb-4.7.1/jshintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.812646 cubicweb-4.7.1/man/
--rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-19 09:51:16.000000 cubicweb-4.7.1/man/cubicweb-ctl.1
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-19 09:51:16.000000 cubicweb-4.7.1/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-19 09:51:16.000000 cubicweb-4.7.1/pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.816646 cubicweb-4.7.1/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/doc.txt
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/from-forge.txt
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-base.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-dataimport.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-devtools.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-ext.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-hooks.txt
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-pyramid.txt
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-server.txt
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-19 09:51:48.820646 cubicweb-4.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3279 2024-04-19 09:51:16.000000 cubicweb-4.7.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     9036 2024-04-19 09:51:16.000000 cubicweb-4.7.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.187147 cubicweb-4.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-05-21 12:44:07.000000 cubicweb-4.8.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2024-05-21 12:44:07.000000 cubicweb-4.8.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2024-05-21 12:44:07.000000 cubicweb-4.8.0/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)     4977 2024-05-21 12:44:07.000000 cubicweb-4.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5161 2024-05-21 12:44:37.187147 cubicweb-4.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.615135 cubicweb-4.8.0/cubicweb/
+-rw-rw-rw-   0 root         (0) root         (0)     7503 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       69 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6885 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/_gcdebug.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/appobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    67217 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    32638 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/cwgettext.py
+-rw-rw-rw-   0 root         (0) root         (0)    25982 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/cwvreg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.623135 cubicweb-4.8.0/cubicweb/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    21081 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    26515 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    15503 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)    18127 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/stores.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.623135 cubicweb-4.8.0/cubicweb/dataimport/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.627135 cubicweb-4.8.0/cubicweb/dataimport/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)   474710 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/data/geonames.csv
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/data/people.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/data/timeZones.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.627135 cubicweb-4.8.0/cubicweb/dataimport/test/data-massimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/data-massimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/test_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    16176 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/test_massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     4179 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/test_pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8221 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/dataimport/test/unittest_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.635135 cubicweb-4.8.0/cubicweb/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)    27112 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5449 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/apptest_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.635135 cubicweb-4.8.0/cubicweb/devtools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/data/cwmock.js
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/data/qunit.css
+-rw-rw-rw-   0 root         (0) root         (0)   115758 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/data/qunit.js
+-rw-rw-rw-   0 root         (0) root         (0)    39808 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/fake.py
+-rw-rw-rw-   0 root         (0) root         (0)    24531 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/fill.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/fix_po_encoding
+-rw-rw-rw-   0 root         (0) root         (0)    10982 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/htmlparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5298 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9195 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/realdbtest.py
+-rw-rw-rw-   0 root         (0) root         (0)    10873 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/repotest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6796 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/stresstester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.639135 cubicweb-4.8.0/cubicweb/devtools/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.639135 cubicweb-4.8.0/cubicweb/devtools/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/firstnames.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.515133 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.643135 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.643135 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.643135 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.643135 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.515133 cubicweb-4.8.0/cubicweb/devtools/test/data/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.647135 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/unittest_dbfill.py
+-rw-rw-rw-   0 root         (0) root         (0)     6402 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/unittest_devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/unittest_fill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/unittest_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/test/unittest_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    20848 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.651135 cubicweb-4.8.0/cubicweb/entities/
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24563 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/authobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     5944 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/schemaobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4095 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.651135 cubicweb-4.8.0/cubicweb/entities/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.651135 cubicweb-4.8.0/cubicweb/entities/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.655135 cubicweb-4.8.0/cubicweb/entities/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9992 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/test/unittest_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    36719 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/test/unittest_wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    22858 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entities/wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    59384 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.655135 cubicweb-4.8.0/cubicweb/ext/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/ext/html4zope.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/ext/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.655135 cubicweb-4.8.0/cubicweb/ext/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/ext/test/unittest_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.663136 cubicweb-4.8.0/cubicweb/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/email.py
+-rw-rw-rw-   0 root         (0) root         (0)    13217 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5680 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     9725 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8157 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/security.py
+-rw-rw-rw-   0 root         (0) root         (0)    10630 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    60802 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4913 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/syncsources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.667136 cubicweb-4.8.0/cubicweb/hooks/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.667136 cubicweb-4.8.0/cubicweb/hooks/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.667136 cubicweb-4.8.0/cubicweb/hooks/test/data-computed/
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/data-computed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_bookmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8490 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_notificationhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    24424 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/test/unittest_syncsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    15886 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/hooks/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.671136 cubicweb-4.8.0/cubicweb/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    93082 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    61668 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)   112148 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)   106920 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     5624 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3352 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/md5crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)    22356 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/migration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.671136 cubicweb-4.8.0/cubicweb/misc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.675136 cubicweb-4.8.0/cubicweb/misc/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.22.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.22.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.22.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.23.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.24.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.24.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.27.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.30.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.31.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.32.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/3.38.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)    20108 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/migration/postcreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.679136 cubicweb-4.8.0/cubicweb/misc/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/scripts/chpasswd.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/scripts/detect_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     5710 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/scripts/fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/scripts/ldap_change_base_dn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3466 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/scripts/migration_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/misc/source_highlight.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/mttransforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17397 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/multipart.py
+-rw-rw-rw-   0 root         (0) root         (0)    50906 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/predicates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.687136 cubicweb-4.8.0/cubicweb/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     9523 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11835 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4474 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7077 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_source_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.691136 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     4852 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/debugtoolbar_panels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/default_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/development.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     3767 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/pyramid.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)    13622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/pyramidctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     7395 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9651 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.691136 cubicweb-4.8.0/cubicweb/pyramid/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.691136 cubicweb-4.8.0/cubicweb/pyramid/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.695136 cubicweb-4.8.0/cubicweb/pyramid/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6447 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/test_content_negociation.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/test/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pyramid/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    17494 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/req.py
+-rw-rw-rw-   0 root         (0) root         (0)    41745 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    11503 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27291 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/rset.py
+-rw-rw-rw-   0 root         (0) root         (0)    11656 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    57848 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     6149 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schema_exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.695136 cubicweb-4.8.0/cubicweb/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schemas/Bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schemas/_regproc.postgres.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13898 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schemas/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15024 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schemas/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    11853 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/schemas/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.707137 cubicweb-4.8.0/cubicweb/server/
+-rw-rw-rw-   0 root         (0) root         (0)    14107 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/check_unused_index.py
+-rw-rw-rw-   0 root         (0) root         (0)    23043 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/checkintegrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/edition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38571 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    77833 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/migractions.py
+-rw-rw-rw-   0 root         (0) root         (0)    35925 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/querier.py
+-rw-rw-rw-   0 root         (0) root         (0)    47931 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)    19156 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13785 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28692 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)     3168 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/serverconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    57884 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    32564 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.711137 cubicweb-4.8.0/cubicweb/server/sources/
+-rw-rw-rw-   0 root         (0) root         (0)    13281 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18181 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sources/datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    16896 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sources/ldapfeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    78080 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sources/native.py
+-rw-rw-rw-   0 root         (0) root         (0)    71034 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sources/rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    11149 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sources/storages.py
+-rw-rw-rw-   0 root         (0) root         (0)    22712 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22485 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/ssplanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.719137 cubicweb-4.8.0/cubicweb/server/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.723137 cubicweb-4.8.0/cubicweb/server/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.755138 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.759138 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.759138 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.759138 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.763138 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.763138 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/ldap_test.ldif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.763138 cubicweb-4.8.0/cubicweb/server/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/slapd.conf.in
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/sources_extern
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data/sources_multi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.723137 cubicweb-4.8.0/cubicweb/server/test/data-cwep002/
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-cwep002/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.727137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.727137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.727137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.731137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.731137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.731137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.735137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.735137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.739137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.739137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.739137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.743137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.743137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.743137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.747137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.747137 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.747137 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.751138 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/Company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/State.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/toignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.755138 cubicweb-4.8.0/cubicweb/server/test/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.763138 cubicweb-4.8.0/cubicweb/server/test/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.763138 cubicweb-4.8.0/cubicweb/server/test/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8829 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_edition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    26126 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_ldapsource.py
+-rw-rw-rw-   0 root         (0) root         (0)    96689 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_querier.py
+-rw-rw-rw-   0 root         (0) root         (0)   101040 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    23306 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11087 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28561 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)    38100 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_server_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_sources_native.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_ssplanner.py
+-rw-rw-rw-   0 root         (0) root         (0)    17465 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21764 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_undo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.767138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.767138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.767138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.771138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.771138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.771138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.775138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.775138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.779138 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.779138 cubicweb-4.8.0/cubicweb/server/test_migractions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.783138 cubicweb-4.8.0/cubicweb/server/test_migractions/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.815139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.815139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.815139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.819139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.819139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.819139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.823139 cubicweb-4.8.0/cubicweb/server/test_migractions/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.783138 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.783138 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.787138 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.787138 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.791139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.791139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.795138 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.795138 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.799139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.799139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.803139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.803139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.807139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.807139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.811139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.811139 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.823139 cubicweb-4.8.0/cubicweb/server/test_migractions/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.823139 cubicweb-4.8.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    47791 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.823139 cubicweb-4.8.0/cubicweb/server/test_migractions2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.827139 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.855140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.855140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.859140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.859140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.859140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.863140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.863140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.827139 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.831139 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.831139 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.835139 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.839140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.839140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.839140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.843140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.843140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.847140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.847140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.847140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.851140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.851140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.851140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.855140 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.863140 cubicweb-4.8.0/cubicweb/server/test_migractions2/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.863140 cubicweb-4.8.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9724 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions2/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.863140 cubicweb-4.8.0/cubicweb/server/test_migractions3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.867140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.891141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.891141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.895141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.895141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.895141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.899141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.899141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.867140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.867140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.871140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.871140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.875140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.875140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.875140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.879140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.879140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.879140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.883140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.883140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.883140 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.887141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.887141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.887141 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.899141 cubicweb-4.8.0/cubicweb/server/test_migractions3/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.899141 cubicweb-4.8.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_migractions3/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.899141 cubicweb-4.8.0/cubicweb/server/test_postgres/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.903141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.903141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.903141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.907141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.907141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.907141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.911141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.911141 cubicweb-4.8.0/cubicweb/server/test_postgres/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_postgres/unittest_postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.911141 cubicweb-4.8.0/cubicweb/server/test_repository/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.915141 cubicweb-4.8.0/cubicweb/server/test_repository/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.915141 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.919141 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.919141 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.919141 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.923141 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.923141 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.915141 cubicweb-4.8.0/cubicweb/server/test_repository/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    38041 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/test_repository/unittest_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     5178 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/server/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.927141 cubicweb-4.8.0/cubicweb/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/.hgignore.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/.yamllint.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/Dockerfile.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/MANIFEST.in.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/README.rst.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.931141 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.931141 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.931141 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.935142 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.935142 cubicweb-4.8.0/cubicweb/skeleton/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.935142 cubicweb-4.8.0/cubicweb/skeleton/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/skeleton/tox.ini.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.935142 cubicweb-4.8.0/cubicweb/smoke_test/
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.939142 cubicweb-4.8.0/cubicweb/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/ldapparser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14419 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5861 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     8236 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/supervising.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.939142 cubicweb-4.8.0/cubicweb/sobjects/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.943142 cubicweb-4.8.0/cubicweb/sobjects/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.943142 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.943142 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.943142 cubicweb-4.8.0/cubicweb/sobjects/test/data/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/data/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/unittest_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     3059 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/unittest_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5404 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/unittest_register_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/sobjects/test/unittest_supervising.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.955142 cubicweb-4.8.0/cubicweb/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.959142 cubicweb-4.8.0/cubicweb/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.963142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.967142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.967142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.967142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/views/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.971142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.971142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/entities/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.971142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.971142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_forge/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_forge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.975142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.975142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_mycube/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_mycube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.975142 cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.979143 cubicweb-4.8.0/cubicweb/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_tag/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/erqlexpr_on_ertype.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/lowered_etype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.979143 cubicweb-4.8.0/cubicweb/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/migration/0.0.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/migration/0.0.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/migration/0.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/migration/0.1.0_common.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/migration/0.1.0_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/migration/0.1.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/rqlexpr_on_computedrel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/rrqlexpr_on_attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/rrqlexpr_on_eetype.py
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.983143 cubicweb-4.8.0/cubicweb/test/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/scripts/script1.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/scripts/script2.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/scripts/script3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.983143 cubicweb-4.8.0/cubicweb/test/data/server_migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)      882 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data/uppered_rtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.959142 cubicweb-4.8.0/cubicweb/test/data-rewrite/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.963142 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.963142 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data-rewrite/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.983143 cubicweb-4.8.0/cubicweb/test/data_schemareader/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/data_schemareader/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    17592 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     7457 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    48020 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8357 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     7471 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_migration.py
+-rw-rw-rw-   0 root         (0) root         (0)    15441 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_req.py
+-rw-rw-rw-   0 root         (0) root         (0)    46300 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6503 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    32589 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     6543 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    34435 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9658 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/test/unittest_wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16545 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)    19530 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12356 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-21 12:44:07.000000 cubicweb-4.8.0/cubicweb/xy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.187147 cubicweb-4.8.0/cubicweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5161 2024-05-21 12:44:35.000000 cubicweb-4.8.0/cubicweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    51759 2024-05-21 12:44:36.000000 cubicweb-4.8.0/cubicweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 12:44:35.000000 cubicweb-4.8.0/cubicweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-21 12:44:35.000000 cubicweb-4.8.0/cubicweb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 12:44:35.000000 cubicweb-4.8.0/cubicweb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      500 2024-05-21 12:44:35.000000 cubicweb-4.8.0/cubicweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 12:44:35.000000 cubicweb-4.8.0/cubicweb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.987143 cubicweb-4.8.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7511 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/4.0.0_how_to_migrate.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.987143 cubicweb-4.8.0/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/_static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/_static/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/announce.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/announce.fr.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.995143 cubicweb-4.8.0/doc/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/__init__.rst
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/appobject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/cwvreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/dataimport.rst
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/predicates.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:36.999143 cubicweb-4.8.0/doc/api/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/bwcompat.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/login.rst
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/profile.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/session.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid/url_redirection.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/pyramid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/req.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/rset.rst
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/urlpublishing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/urlrewrite.rst
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/api/web.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.003143 cubicweb-4.8.0/doc/book/
+-rw-rw-rw-   0 root         (0) root         (0)    14655 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/MERGE_ME-tut-create-app.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7806 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.003143 cubicweb-4.8.0/doc/book/_maybe_to_integrate/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/_maybe_to_integrate/rss-xml.rst
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/_maybe_to_integrate/template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.003143 cubicweb-4.8.0/doc/book/additionnal_services/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/additionnal_services/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/additionnal_services/undo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.011143 cubicweb-4.8.0/doc/book/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/backups.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/create-instance.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/cubicweb-ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4034 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/deploy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      409 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/instance-config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/ldap.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/multisources.rst
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/rql-logs.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/admin/site-config.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.015143 cubicweb-4.8.0/doc/book/annexes/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/depends.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/docstrings-conventions.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16153 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/faq.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/mercurial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.019143 cubicweb-4.8.0/doc/book/annexes/rql/
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/Graph-ex.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/debugging.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/implementation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5570 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)    27490 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/language.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/annexes/rql/usecases.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.023143 cubicweb-4.8.0/doc/book/devrepo/
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/connections_pooler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.027144 cubicweb-4.8.0/doc/book/devrepo/cubes/
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/cubes/available-cubes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/cubes/cc-newcube.rst
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/cubes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6827 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/cubes/layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/cubes/what-is-a-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/dataimport.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.031144 cubicweb-4.8.0/doc/book/devrepo/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/datamodel/baseschema.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6178 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/datamodel/define-workflows.rst
+-rw-rw-rw-   0 root         (0) root         (0)    34880 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/datamodel/definition.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/datamodel/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/datamodel/metadata.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/debug_channels.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.031144 cubicweb-4.8.0/doc/book/devrepo/devcore/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/devcore/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/devcore/reqbase.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.035144 cubicweb-4.8.0/doc/book/devrepo/entityclasses/
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/entityclasses/adapters.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7268 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/entityclasses/application-logic.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/entityclasses/data-as-objects.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/entityclasses/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/entityclasses/load-sort.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4399 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/fti.rst
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/migration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/profiling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.039144 cubicweb-4.8.0/doc/book/devrepo/repo/
+-rw-rw-rw-   0 root         (0) root         (0)     9731 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/repo/hooks.rst
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/repo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/repo/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11467 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/repo/sessions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/repo/tasks.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21316 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    18289 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devrepo/vreg.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.047144 cubicweb-4.8.0/doc/book/devweb/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/ajax.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/controllers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/css.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.051144 cubicweb-4.8.0/doc/book/devweb/edition/
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/edition/dissection.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/edition/editcontroller.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9905 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/edition/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15506 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/edition/form.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/edition/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/facets.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/httpcaching.rst
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10057 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/internationalization.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14107 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/js.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/property.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/publisher.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/request.rst
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/resource.rst
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/rtags.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/searchbar.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.059144 cubicweb-4.8.0/doc/book/devweb/views/
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/basetemplates.rst
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/baseviews.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/boxes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/breadcrumbs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/idownloadable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      476 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10179 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/primary.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5991 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/startup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/urlpublish.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/views.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/wdoc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/views/xmlrss.rst
+-rw-rw-rw-   0 root         (0) root         (0)      947 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/devweb/warning.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.059144 cubicweb-4.8.0/doc/book/intro/
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/intro/concepts.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/intro/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/intro/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.063144 cubicweb-4.8.0/doc/book/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/pyramid/ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/pyramid/debug_toolbar.rst
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/pyramid/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/pyramid/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/pyramid/settings.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.063144 cubicweb-4.8.0/doc/book/security/
+-rw-rw-rw-   0 root         (0) root         (0)     8041 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/security/csrf.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.063144 cubicweb-4.8.0/doc/book/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/src/archi_globale.dia
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/book/src/main_template_layout.dia
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.087145 cubicweb-4.8.0/doc/changes/
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.14.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.15.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.16.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.17.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.18.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.19.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.20.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.21.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.22.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.23.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.24.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.25.rst
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.26.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6870 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.27.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.28.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.29.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.30.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.31.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.32.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.32_reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5635 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.33.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.34.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4849 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.35.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4507 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.36.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5437 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.37.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8870 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/3.38.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6425 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/changes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7654 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.163147 cubicweb-4.8.0/doc/images/
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    12650 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/breadcrumbs_header.png
+-rw-rw-rw-   0 root         (0) root         (0)    85073 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_general_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   124385 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_registry_content_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   111325 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_registry_decisions_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   134505 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_rql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   192629 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_rql_traceback_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   107766 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_show_source.png
+-rw-rw-rw-   0 root         (0) root         (0)    55625 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_show_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)   126845 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_sql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)    97343 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/debugtoolbar_traceback_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)    57300 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/example-card-with-rql-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)    55168 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/example-card-with-rql-table-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/facet_date_range.png
+-rw-rw-rw-   0 root         (0) root         (0)     6013 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/facet_has_image.png
+-rw-rw-rw-   0 root         (0) root         (0)    22016 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/facet_overview.png
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/facet_range.png
+-rw-rw-rw-   0 root         (0) root         (0)    21685 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_00-login_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30326 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_01-start_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    35859 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_02-cookie-values_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33922 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_02-create-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28123 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_03-list-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    82897 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_03-site-config-panel_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   119813 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_03-state-submitted_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    34771 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_04-detail-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28345 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_05-list-two-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    49230 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_06-add-relation-entryof_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    96838 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_06-main-template-logo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    40383 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_07-detail-one-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30591 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_08-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33091 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_09-new-view-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42230 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/lax-book_10-blog-with-two-entries_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    17757 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/main_template.png
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/main_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13842 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/main_template_layout.png
+-rw-rw-rw-   0 root         (0) root         (0)    46411 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/primaryview_template.png
+-rw-rw-rw-   0 root         (0) root         (0)    14758 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/primaryview_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    22773 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/request_session.png
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/request_session.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12030 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/server-class-diagram.png
+-rw-rw-rw-   0 root         (0) root         (0)    62022 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_blog-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   105173 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    58500 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_blog-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42013 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_blogs-list_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   109769 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_form-generic-relations_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    65646 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_index_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    13605 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_index_gettext_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    88970 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_index_logged_in_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_login-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   100347 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    63097 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    62431 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-community-default-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    74856 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    79709 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-custom-footer_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   128406 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    71500 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_myblog-siteinfo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   104834 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    22098 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_schema_graphviz_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   150520 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-base_siteconfig_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    60672 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_admin.png
+-rw-rw-rw-   0 root         (0) root         (0)    61388 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_city_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    50694 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_city_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    71561 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_data_model_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)    48896 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_empty_instance.png
+-rw-rw-rw-   0 root         (0) root         (0)    55671 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_finished_import.png
+-rw-rw-rw-   0 root         (0) root         (0)    57063 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_list_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    70893 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_museum_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    61656 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_museum_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    74005 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_museum_with_city_name.png
+-rw-rw-rw-   0 root         (0) root         (0)   225824 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_react_map.png
+-rw-rw-rw-   0 root         (0) root         (0)    53544 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-museum_with_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)   354637 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_background-image.png
+-rw-rw-rw-   0 root         (0) root         (0)    30437 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_boxes.png
+-rw-rw-rw-   0 root         (0) root         (0)    54643 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_breadcrumbs.png
+-rw-rw-rw-   0 root         (0) root         (0)   324086 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_facets.png
+-rw-rw-rw-   0 root         (0) root         (0)    40520 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_grey-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    16843 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_index-after.png
+-rw-rw-rw-   0 root         (0) root         (0)    26875 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_index-before.png
+-rw-rw-rw-   0 root         (0) root         (0)    17580 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_login-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    57814 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_prevnext.png
+-rw-rw-rw-   0 root         (0) root         (0)    81362 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_ui1.png
+-rw-rw-rw-   0 root         (0) root         (0)    93291 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_ui2.png
+-rw-rw-rw-   0 root         (0) root         (0)   290338 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/tutos-photowebsite_ui3.png
+-rw-rw-rw-   0 root         (0) root         (0)    43051 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/undo_history-view_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    26036 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/undo_mesage_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    39625 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/undo_startup-link_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    17558 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/views-table-filter-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)    14013 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/views-table-filter.png
+-rw-rw-rw-   0 root         (0) root         (0)    12375 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/views-table-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/images/views-table.png
+-rw-rw-rw-   0 root         (0) root         (0)     7344 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/plan_formation_python_cubicweb.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/stdlib.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.167147 cubicweb-4.8.0/doc/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tools/generate_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tools/mode_plan.py
+-rwxrwxrwx   0 root         (0) root         (0)     4944 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tools/pyjsrest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.167147 cubicweb-4.8.0/doc/tutorials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.171147 cubicweb-4.8.0/doc/tutorials/advanced/
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/advanced/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5486 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/advanced/part01_create-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17016 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/advanced/part02_security.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5614 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/advanced/part03_bfss.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15384 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/advanced/part04_ui-base.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15114 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/advanced/part05_ui-advanced.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.171147 cubicweb-4.8.0/doc/tutorials/base/
+-rw-rw-rw-   0 root         (0) root         (0)     3867 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/base/blog-in-five-minutes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/base/conclusion.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20435 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/base/customizing-the-application.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7821 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/base/discovering-the-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/base/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.175147 cubicweb-4.8.0/doc/tutorials/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     9014 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/dataimport/diseasome_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/dataimport/diseasome_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    29917 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/dataimport/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6576 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/dataimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.179147 cubicweb-4.8.0/doc/tutorials/museum/
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/museum/data-management.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/museum/develop-app.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/museum/develop-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8840 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/museum/enhance-views.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/museum/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-21 12:44:07.000000 cubicweb-4.8.0/doc/tutorials/museum/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.179147 cubicweb-4.8.0/extras/
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2024-05-21 12:44:07.000000 cubicweb-4.8.0/extras/cubicweb-ctl.bash_completion
+-rw-rw-rw-   0 root         (0) root         (0)     7414 2024-05-21 12:44:07.000000 cubicweb-4.8.0/jshintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.179147 cubicweb-4.8.0/man/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-05-21 12:44:07.000000 cubicweb-4.8.0/man/cubicweb-ctl.1
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-21 12:44:07.000000 cubicweb-4.8.0/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-21 12:44:07.000000 cubicweb-4.8.0/pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 12:44:37.183147 cubicweb-4.8.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/from-forge.txt
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-base.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-dataimport.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-devtools.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-ext.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-hooks.txt
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-pyramid.txt
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-21 12:44:07.000000 cubicweb-4.8.0/requirements/test-server.txt
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-21 12:44:37.191147 cubicweb-4.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-21 12:44:07.000000 cubicweb-4.8.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     9036 2024-05-21 12:44:07.000000 cubicweb-4.8.0/tox.ini
```

### Comparing `cubicweb-4.7.1/CONTRIBUTING.rst` & `cubicweb-4.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/COPYING` & `cubicweb-4.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/COPYING.LESSER` & `cubicweb-4.8.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/MANIFEST.in` & `cubicweb-4.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/PKG-INFO` & `cubicweb-4.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb
-Version: 4.7.1
+Version: 4.8.0
 Summary: a repository of entities / relations for knowledge management
 Home-page: https://www.cubicweb.org
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Requires-Python: >=3.7
 License-File: COPYING
```

### Comparing `cubicweb-4.7.1/README.rst` & `cubicweb-4.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/__init__.py` & `cubicweb-4.8.0/cubicweb/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/__pkginfo__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb global packaging information for the cubicweb knowledge management
 software
 """
 
 modname = distname = "cubicweb"
 
-numversion = (4, 7, 1)
+numversion = (4, 8, 0)
 version = ".".join(str(num) for num in numversion)
 
 description = "a repository of entities / relations for knowledge management"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = "https://www.cubicweb.org"
 license = "LGPL"
```

### Comparing `cubicweb-4.7.1/cubicweb/_exceptions.py` & `cubicweb-4.8.0/cubicweb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/_gcdebug.py` & `cubicweb-4.8.0/cubicweb/_gcdebug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/appobject.py` & `cubicweb-4.8.0/cubicweb/appobject.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/crypto.py` & `cubicweb-4.8.0/cubicweb/crypto.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/cwconfig.py` & `cubicweb-4.8.0/cubicweb/cwconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -875,14 +875,44 @@
                 "type": "string",
                 "default": None,
                 "help": "S3 secret key for database dump/restore",
                 "group": "dbdump",
                 "level": 3,
             },
         ),
+        (
+            "dump-s3-region",
+            {
+                "type": "string",
+                "default": None,
+                "help": "S3 region name of buckets for database dump/restore",
+                "group": "dbdump",
+                "level": 3,
+            },
+        ),
+        (
+            "dump-s3-secure",
+            {
+                "type": "yn",
+                "default": True,
+                "help": "Activate the secure flag to use TLS connection with S3",
+                "group": "dbdump",
+                "level": 3,
+            },
+        ),
+        (
+            "dump-s3-cert-check",
+            {
+                "type": "yn",
+                "default": True,
+                "help": "Activate the verification of the certificat for HTTPS connections",
+                "group": "dbdump",
+                "level": 3,
+            },
+        ),
     )
 
     def load_defaults(self) -> None:
         """overload the parent `load_defaults` to load REQUIRED variables with
         environment values
         """
         for opt, optdict in self.options:
```

### Comparing `cubicweb-4.7.1/cubicweb/cwctl.py` & `cubicweb-4.8.0/cubicweb/cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/cwgettext.py` & `cubicweb-4.8.0/cubicweb/cwgettext.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/cwvreg.py` & `cubicweb-4.8.0/cubicweb/cwvreg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/__init__.py` & `cubicweb-4.8.0/cubicweb/dataimport/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/csv.py` & `cubicweb-4.8.0/cubicweb/dataimport/csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/importer.py` & `cubicweb-4.8.0/cubicweb/dataimport/importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/massive_store.py` & `cubicweb-4.8.0/cubicweb/dataimport/massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/pgstore.py` & `cubicweb-4.8.0/cubicweb/dataimport/pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/stores.py` & `cubicweb-4.8.0/cubicweb/dataimport/stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/data/geonames.csv` & `cubicweb-4.8.0/cubicweb/dataimport/test/data/geonames.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/data/timeZones.txt` & `cubicweb-4.8.0/cubicweb/dataimport/test/data/timeZones.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/data-massimport/schema.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/data-massimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/test_csv.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/test_massive_store.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/test_massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/test_pgstore.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/test_pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/test_stores.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/test_stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/dataimport/test/unittest_importer.py` & `cubicweb-4.8.0/cubicweb/dataimport/test/unittest_importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/debug.py` & `cubicweb-4.8.0/cubicweb/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/__init__.py` & `cubicweb-4.8.0/cubicweb/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/apptest_config.py` & `cubicweb-4.8.0/cubicweb/devtools/apptest_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/data/qunit.css` & `cubicweb-4.8.0/cubicweb/devtools/data/qunit.css`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/data/qunit.js` & `cubicweb-4.8.0/cubicweb/devtools/data/qunit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/devctl.py` & `cubicweb-4.8.0/cubicweb/devtools/devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/fake.py` & `cubicweb-4.8.0/cubicweb/devtools/fake.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/fill.py` & `cubicweb-4.8.0/cubicweb/devtools/fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/fix_po_encoding` & `cubicweb-4.8.0/cubicweb/devtools/fix_po_encoding`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/htmlparser.py` & `cubicweb-4.8.0/cubicweb/devtools/htmlparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/httptest.py` & `cubicweb-4.8.0/cubicweb/devtools/httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/instrument.py` & `cubicweb-4.8.0/cubicweb/devtools/instrument.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/realdbtest.py` & `cubicweb-4.8.0/cubicweb/devtools/realdbtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/repotest.py` & `cubicweb-4.8.0/cubicweb/devtools/repotest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/stresstester.py` & `cubicweb-4.8.0/cubicweb/devtools/stresstester.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/data/firstnames.txt` & `cubicweb-4.8.0/cubicweb/devtools/test/data/firstnames.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-4.8.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/devtools/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/utils.js` & `cubicweb-4.8.0/cubicweb/devtools/test/data/static/js_examples/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/unittest_dbfill.py` & `cubicweb-4.8.0/cubicweb/devtools/test/unittest_dbfill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/unittest_devctl.py` & `cubicweb-4.8.0/cubicweb/devtools/test/unittest_devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/unittest_fill.py` & `cubicweb-4.8.0/cubicweb/devtools/test/unittest_fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/unittest_i18n.py` & `cubicweb-4.8.0/cubicweb/devtools/test/unittest_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/test/unittest_testlib.py` & `cubicweb-4.8.0/cubicweb/devtools/test/unittest_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/devtools/testlib.py` & `cubicweb-4.8.0/cubicweb/devtools/testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/__init__.py` & `cubicweb-4.8.0/cubicweb/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/adapters.py` & `cubicweb-4.8.0/cubicweb/entities/adapters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/authobjs.py` & `cubicweb-4.8.0/cubicweb/entities/authobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/lib.py` & `cubicweb-4.8.0/cubicweb/entities/lib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/schemaobjs.py` & `cubicweb-4.8.0/cubicweb/entities/schemaobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/sources.py` & `cubicweb-4.8.0/cubicweb/entities/sources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/test/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/entities/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/entities/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/test/unittest_base.py` & `cubicweb-4.8.0/cubicweb/entities/test/unittest_base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/test/unittest_wfobjs.py` & `cubicweb-4.8.0/cubicweb/entities/test/unittest_wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entities/wfobjs.py` & `cubicweb-4.8.0/cubicweb/entities/wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/entity.py` & `cubicweb-4.8.0/cubicweb/entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/ext/__init__.py` & `cubicweb-4.8.0/cubicweb/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/ext/html4zope.py` & `cubicweb-4.8.0/cubicweb/ext/html4zope.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/ext/markdown.py` & `cubicweb-4.8.0/cubicweb/ext/markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/ext/test/unittest_markdown.py` & `cubicweb-4.8.0/cubicweb/ext/test/unittest_markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/__init__.py` & `cubicweb-4.8.0/cubicweb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/bookmark.py` & `cubicweb-4.8.0/cubicweb/hooks/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/email.py` & `cubicweb-4.8.0/cubicweb/hooks/email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/integrity.py` & `cubicweb-4.8.0/cubicweb/hooks/integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/metadata.py` & `cubicweb-4.8.0/cubicweb/hooks/metadata.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/notification.py` & `cubicweb-4.8.0/cubicweb/hooks/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/security.py` & `cubicweb-4.8.0/cubicweb/hooks/security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/synccomputed.py` & `cubicweb-4.8.0/cubicweb/hooks/synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/syncschema.py` & `cubicweb-4.8.0/cubicweb/hooks/syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/syncsession.py` & `cubicweb-4.8.0/cubicweb/hooks/syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/syncsources.py` & `cubicweb-4.8.0/cubicweb/hooks/syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/hooks/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/data-computed/schema.py` & `cubicweb-4.8.0/cubicweb/hooks/test/data-computed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_bookmarks.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_bookmarks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_hooks.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_integrity.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_notificationhooks.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_notificationhooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_security.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_synccomputed.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncschema.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsession.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsources.py` & `cubicweb-4.8.0/cubicweb/hooks/test/unittest_syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/hooks/workflow.py` & `cubicweb-4.8.0/cubicweb/hooks/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/i18n/de.po` & `cubicweb-4.8.0/cubicweb/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/i18n/en.po` & `cubicweb-4.8.0/cubicweb/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/i18n/es.po` & `cubicweb-4.8.0/cubicweb/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/i18n/fr.po` & `cubicweb-4.8.0/cubicweb/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/i18n.py` & `cubicweb-4.8.0/cubicweb/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/mail.py` & `cubicweb-4.8.0/cubicweb/mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/md5crypt.py` & `cubicweb-4.8.0/cubicweb/md5crypt.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/migration.py` & `cubicweb-4.8.0/cubicweb/migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/migration/3.22.0_Any.py` & `cubicweb-4.8.0/cubicweb/misc/migration/3.22.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/migration/3.23.0_Any.py` & `cubicweb-4.8.0/cubicweb/misc/migration/3.23.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/migration/3.24.0_Any.py` & `cubicweb-4.8.0/cubicweb/misc/migration/3.24.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/migration/3.24.4_Any.py` & `cubicweb-4.8.0/cubicweb/misc/migration/3.24.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/migration/bootstrapmigration_repository.py` & `cubicweb-4.8.0/cubicweb/misc/migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/misc/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/scripts/chpasswd.py` & `cubicweb-4.8.0/cubicweb/misc/scripts/chpasswd.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/scripts/fast_drop_entities.py` & `cubicweb-4.8.0/cubicweb/misc/scripts/fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/scripts/ldap_change_base_dn.py` & `cubicweb-4.8.0/cubicweb/misc/scripts/ldap_change_base_dn.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/scripts/migration_helper.py` & `cubicweb-4.8.0/cubicweb/misc/scripts/migration_helper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/misc/source_highlight.py` & `cubicweb-4.8.0/cubicweb/misc/source_highlight.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/mttransforms.py` & `cubicweb-4.8.0/cubicweb/mttransforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/multipart.py` & `cubicweb-4.8.0/cubicweb/multipart.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/predicates.py` & `cubicweb-4.8.0/cubicweb/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/__init__.py` & `cubicweb-4.8.0/cubicweb/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/auth.py` & `cubicweb-4.8.0/cubicweb/pyramid/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/config.py` & `cubicweb-4.8.0/cubicweb/pyramid/config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/core.py` & `cubicweb-4.8.0/cubicweb/pyramid/core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/csrf.py` & `cubicweb-4.8.0/cubicweb/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_source_code.py` & `cubicweb-4.8.0/cubicweb/pyramid/debug_source_code.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako` & `cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako` & `cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako` & `cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako` & `cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako` & `cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako` & `cubicweb-4.8.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/debugtoolbar_panels.py` & `cubicweb-4.8.0/cubicweb/pyramid/debugtoolbar_panels.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/default_session.py` & `cubicweb-4.8.0/cubicweb/pyramid/default_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/development.ini.tmpl` & `cubicweb-4.8.0/cubicweb/pyramid/development.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/predicates.py` & `cubicweb-4.8.0/cubicweb/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/pyramid.ini.tmpl` & `cubicweb-4.8.0/cubicweb/pyramid/pyramid.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/pyramidctl.py` & `cubicweb-4.8.0/cubicweb/pyramid/pyramidctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/resources.py` & `cubicweb-4.8.0/cubicweb/pyramid/resources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/rest_api.py` & `cubicweb-4.8.0/cubicweb/pyramid/rest_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/session.py` & `cubicweb-4.8.0/cubicweb/pyramid/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/__init__.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/schema.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/test_auth.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/test_config.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/test_content_negociation.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/test_content_negociation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/test_core.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/test_core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/test/test_tools.py` & `cubicweb-4.8.0/cubicweb/pyramid/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pyramid/tools.py` & `cubicweb-4.8.0/cubicweb/pyramid/tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/pytestconf.py` & `cubicweb-4.8.0/cubicweb/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/rdf.py` & `cubicweb-4.8.0/cubicweb/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/repoapi.py` & `cubicweb-4.8.0/cubicweb/repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/req.py` & `cubicweb-4.8.0/cubicweb/req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/rqlrewrite.py` & `cubicweb-4.8.0/cubicweb/rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/rqlsuggestions.py` & `cubicweb-4.8.0/cubicweb/rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/rset.py` & `cubicweb-4.8.0/cubicweb/rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/rtags.py` & `cubicweb-4.8.0/cubicweb/rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schema.py` & `cubicweb-4.8.0/cubicweb/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schema_exporters.py` & `cubicweb-4.8.0/cubicweb/schema_exporters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schemas/Bookmark.py` & `cubicweb-4.8.0/cubicweb/schemas/Bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schemas/__init__.py` & `cubicweb-4.8.0/cubicweb/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schemas/_regproc.postgres.sql` & `cubicweb-4.8.0/cubicweb/schemas/_regproc.postgres.sql`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schemas/base.py` & `cubicweb-4.8.0/cubicweb/schemas/base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schemas/bootstrap.py` & `cubicweb-4.8.0/cubicweb/schemas/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/schemas/workflow.py` & `cubicweb-4.8.0/cubicweb/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/__init__.py` & `cubicweb-4.8.0/cubicweb/server/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/check_unused_index.py` & `cubicweb-4.8.0/cubicweb/server/check_unused_index.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/checkintegrity.py` & `cubicweb-4.8.0/cubicweb/server/checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/edition.py` & `cubicweb-4.8.0/cubicweb/server/edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/hook.py` & `cubicweb-4.8.0/cubicweb/server/hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/migractions.py` & `cubicweb-4.8.0/cubicweb/server/migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/querier.py` & `cubicweb-4.8.0/cubicweb/server/querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/repository.py` & `cubicweb-4.8.0/cubicweb/server/repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/rqlannotation.py` & `cubicweb-4.8.0/cubicweb/server/rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/schema2sql.py` & `cubicweb-4.8.0/cubicweb/server/schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/schemaserial.py` & `cubicweb-4.8.0/cubicweb/server/schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/serverconfig.py` & `cubicweb-4.8.0/cubicweb/server/serverconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/serverctl.py` & `cubicweb-4.8.0/cubicweb/server/serverctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # *ctl module should limit the number of import to be imported as quickly as
 # possible (for cubicweb-ctl reactivity, necessary for instance for usable bash
 # completion). So import locally in command helpers.
 import sched
 import sys
 from contextlib import contextmanager
 
+from glob import glob
 from tempfile import NamedTemporaryFile
 
 from logilab.common.configuration import Configuration, merge_options
 from logilab.common.deprecation import callable_deprecated
 from logilab.common.shellutils import ASK, generate_password
 from logilab.database import get_db_helper, get_connection
 
@@ -895,28 +896,28 @@
     config.quick_start = True
     mih = config.migration_handler(verbosity=1)
     backupfile = mih.backup_database(output, askconfirm=False, format=format)
     mih.shutdown()
     return backupfile
 
 
-def _get_s3_client(url, access_key, secret_key, bucket):
+def _get_s3_client(url, bucket, **kwargs):
     try:
         from minio import Minio
     except ImportError:
         raise ExecutionError(
             "Minio module is missing, s3 dump cannot be used. Install it with pip install .[s3]"
         )
 
     if not url:
         print("dump-s3-endpoint-url is not defined in all-in-one.conf")
         return
 
     # open s3 connection
-    client = Minio(url, access_key=access_key, secret_key=secret_key)
+    client = Minio(url, **kwargs)
 
     if not bucket:
         print("dump-s3-bucket-name is not defined in all-in-one.conf")
         return
 
     if not client.bucket_exists(bucket):
         print(f"dump-s3-bucket-name {bucket} do not exists")
@@ -928,17 +929,20 @@
 def _s3_dump(appid, output, clean, format="native"):
     config = CubicWebConfiguration.config_for(appid)
     s3_bucket_name = config.get("dump-s3-bucket-name")
 
     # open s3 connection
     client = _get_s3_client(
         config.get("dump-s3-endpoint-url"),
-        config.get("dump-s3-access-key"),
-        config.get("dump-s3-secret-key"),
         s3_bucket_name,
+        access_key=config.get("dump-s3-access-key"),
+        secret_key=config.get("dump-s3-secret-key"),
+        region=config.get("dump-s3-region"),
+        secure=config.get("dump-s3-secure"),
+        cert_check=config.get("dump-s3-cert-check"),
     )
 
     # create backup in tmp file
     backupfile = _local_dump(appid, None, format=format)
     backupname = os.path.basename(backupfile)
     backuppath = output if output else backupname
 
@@ -1109,15 +1113,16 @@
 
     <instance>
       the identifier of the instance to restore
     """
 
     name = "db-restore"
     arguments = "<instance> <backupfile>"
-    min_args = max_args = 2
+    min_args = 1
+    max_args = 2
 
     options = (
         (
             "no-drop",
             {
                 "short": "n",
                 "action": "store_true",
@@ -1133,62 +1138,103 @@
             {
                 "action": "store_true",
                 "default": False,
                 "help": "Pull dump from S3 bucket.",
             },
         ),
         (
+            "latest",
+            {
+                "action": "store_true",
+                "default": False,
+                "help": "Restore latest backup file of directory or s3 bucket.",
+            },
+        ),
+        (
             "format",
             {
                 "short": "f",
                 "default": "native",
                 "type": "choice",
                 "choices": ("native", "portable"),
                 "help": "the format used when dumping the database",
             },
         ),
     )
 
-    def _get_dump_from_s3(self, appid, filepath):
+    def _get_latest_filename_from_s3_bucket(self, client, bucket_name):
+        files = client.list_objects(bucket_name)
+        latest_file = None
+        for file in files:
+            if not latest_file or file.last_modified > latest_file.last_modified:
+                latest_file = file
+
+        if not latest_file:
+            raise ExecutionError(f"No file found in S3 bucket {bucket_name}")
+
+        return latest_file.object_name
+
+    def _get_latest_filename_from_path(self, directory):
+        files = glob(f"{directory}/*")
+        if not files:
+            raise ExecutionError(f"No file found in {directory}")
+        return max(files, key=os.path.getctime)
+
+    def _get_dump_from_s3(self, appid, filepath, get_latest=False):
         # fget_object(bucket_name, object_name, file_path, request_headers=None, ssec=None, version_id=None, extra_query_params=None, tmp_file_path=None)
         config = CubicWebConfiguration.config_for(appid)
         s3_bucket_name = config.get("dump-s3-bucket-name")
 
         # open s3 connection
         client = _get_s3_client(
             config.get("dump-s3-endpoint-url"),
-            config.get("dump-s3-access-key"),
-            config.get("dump-s3-secret-key"),
             s3_bucket_name,
+            access_key=config.get("dump-s3-access-key"),
+            secret_key=config.get("dump-s3-secret-key"),
+            region=config.get("dump-s3-region"),
+            secure=config.get("dump-s3-secure"),
+            cert_check=config.get("dump-s3-cert-check"),
         )
 
+        if get_latest:
+            filepath = self._get_latest_filename_from_s3_bucket(client, s3_bucket_name)
+
         tmpfile = NamedTemporaryFile(suffix=f".{filepath.split('.', maxsplit=1)[-1]}")
 
         # download file to tmp file
         client.fget_object(s3_bucket_name, filepath, tmpfile.name)
         print(f"-> {filepath} has been downloaded as {tmpfile.name}")
 
         return tmpfile
 
     def run(self, args):
-        appid, backupfile = args
+        appid = args[0]
+        backupfile = None
+        if len(args) == 2:
+            backupfile = args[1]
+
         if self.config.format == "portable":
             # we need to ensure a DB exist before restoring from portable format
             if not self.config.no_drop:
                 try:
                     CWCTL.run(["db-create", "--automatic", appid])
                 except SystemExit as exc:
                     # continue if the command exited with status 0 (success)
                     if exc.code:
                         raise
 
         if self.config.s3:
-            tmpfile = self._get_dump_from_s3(appid, backupfile)
+            tmpfile = self._get_dump_from_s3(appid, backupfile, self.config.latest)
             backupfile = tmpfile.name
 
+        # if --latest, backupfile must be a directory path.
+        # get latest file in this directory
+        if not self.config.s3 and self.config.latest:
+            backupfile = self._get_latest_filename_from_path(backupfile)
+
         _local_restore(
             appid, backupfile, drop=not self.config.no_drop, format=self.config.format
         )
 
         # clean
         if self.config.s3:
             print(f"-> delete {tmpfile.name}")
```

### Comparing `cubicweb-4.7.1/cubicweb/server/session.py` & `cubicweb-4.8.0/cubicweb/server/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sources/__init__.py` & `cubicweb-4.8.0/cubicweb/server/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sources/datafeed.py` & `cubicweb-4.8.0/cubicweb/server/sources/datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sources/ldapfeed.py` & `cubicweb-4.8.0/cubicweb/server/sources/ldapfeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sources/native.py` & `cubicweb-4.8.0/cubicweb/server/sources/native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sources/rql2sql.py` & `cubicweb-4.8.0/cubicweb/server/sources/rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sources/storages.py` & `cubicweb-4.8.0/cubicweb/server/sources/storages.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/sqlutils.py` & `cubicweb-4.8.0/cubicweb/server/sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/ssplanner.py` & `cubicweb-4.8.0/cubicweb/server/ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/ldap_test.ldif` & `cubicweb-4.8.0/cubicweb/server/test/data/ldap_test.ldif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/server/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data/slapd.conf.in` & `cubicweb-4.8.0/cubicweb/server/test/data/slapd.conf.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-cwep002/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-cwep002/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/__init__.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-migractions/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Company.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/Company.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Dates.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/State.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/State.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/__init__.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schema2sql/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/datacomputed/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/datacomputed/schema.py` & `cubicweb-4.8.0/cubicweb/server/test/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_datafeed.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_edition.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_hook.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_ldapsource.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_ldapsource.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_querier.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_rql2sql.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_rqlannotation.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_schema2sql.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_schemaserial.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_server_security.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_server_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_server_utils.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_server_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_serverctl.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_session.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_sources_native.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_sources_native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_sqlutils.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_ssplanner.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_storage.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_storage.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_tools.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_undo.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_undo.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test/unittest_utils.py` & `cubicweb-4.8.0/cubicweb/server/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py` & `cubicweb-4.8.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions/unittest_migractions.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions2/unittest_migractions.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions2/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_migractions3/unittest_migractions.py` & `cubicweb-4.8.0/cubicweb/server/test_migractions3/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/migration/postcreate.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_postgres/unittest_postgres.py` & `cubicweb-4.8.0/cubicweb/server/test_postgres/unittest_postgres.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/entities.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/hooks.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/schema.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/test_repository/unittest_repository.py` & `cubicweb-4.8.0/cubicweb/server/test_repository/unittest_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/server/utils.py` & `cubicweb-4.8.0/cubicweb/server/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/.gitlab-ci.yml.tmpl` & `cubicweb-4.8.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/README.rst.tmpl` & `cubicweb-4.8.0/cubicweb/skeleton/README.rst.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl` & `cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl` & `cubicweb-4.8.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/setup.py.tmpl` & `cubicweb-4.8.0/cubicweb/skeleton/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/test/realdb_test_CUBENAME.py` & `cubicweb-4.8.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/skeleton/tox.ini.tmpl` & `cubicweb-4.8.0/cubicweb/skeleton/tox.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py` & `cubicweb-4.8.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py` & `cubicweb-4.8.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/__init__.py` & `cubicweb-4.8.0/cubicweb/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/ldapparser.py` & `cubicweb-4.8.0/cubicweb/sobjects/ldapparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/notification.py` & `cubicweb-4.8.0/cubicweb/sobjects/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/services.py` & `cubicweb-4.8.0/cubicweb/sobjects/services.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/supervising.py` & `cubicweb-4.8.0/cubicweb/sobjects/supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/data/sobjects/__init__.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/data/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_email.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/unittest_email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_notification.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/unittest_notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_register_user.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/unittest_register_user.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_supervising.py` & `cubicweb-4.8.0/cubicweb/sobjects/test/unittest_supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/tags.py` & `cubicweb-4.8.0/cubicweb/tags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/schema.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__init__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__init__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__init__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_forge/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__init__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_mycube/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__init__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/schema.py` & `cubicweb-4.8.0/cubicweb/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/entities.py` & `cubicweb-4.8.0/cubicweb/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/erqlexpr_on_ertype.py` & `cubicweb-4.8.0/cubicweb/test/data/erqlexpr_on_ertype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/migration/0.0.3_Any.py` & `cubicweb-4.8.0/cubicweb/test/data/migration/0.0.3_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/migration/0.0.4_Any.py` & `cubicweb-4.8.0/cubicweb/test/data/migration/0.0.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_Any.py` & `cubicweb-4.8.0/cubicweb/test/data/migration/0.1.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_common.py` & `cubicweb-4.8.0/cubicweb/test/data/migration/0.1.0_common.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_repository.py` & `cubicweb-4.8.0/cubicweb/test/data/migration/0.1.0_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.2_Any.py` & `cubicweb-4.8.0/cubicweb/test/data/migration/0.1.2_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/rqlexpr_on_ertype_read.py` & `cubicweb-4.8.0/cubicweb/test/data/rqlexpr_on_ertype_read.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_attr.py` & `cubicweb-4.8.0/cubicweb/test/data/rrqlexpr_on_attr.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_eetype.py` & `cubicweb-4.8.0/cubicweb/test/data/rrqlexpr_on_eetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/schema.py` & `cubicweb-4.8.0/cubicweb/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data/server_migration/bootstrapmigration_repository.py` & `cubicweb-4.8.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/schema.py` & `cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py` & `cubicweb-4.8.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data-rewrite/schema.py` & `cubicweb-4.8.0/cubicweb/test/data-rewrite/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/data_schemareader/schema.py` & `cubicweb-4.8.0/cubicweb/test/data_schemareader/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_binary.py` & `cubicweb-4.8.0/cubicweb/test/unittest_binary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_cwconfig.py` & `cubicweb-4.8.0/cubicweb/test/unittest_cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_cwctl.py` & `cubicweb-4.8.0/cubicweb/test/unittest_cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_entity.py` & `cubicweb-4.8.0/cubicweb/test/unittest_entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_fast_drop_entities.py` & `cubicweb-4.8.0/cubicweb/test/unittest_fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_mail.py` & `cubicweb-4.8.0/cubicweb/test/unittest_mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_migration.py` & `cubicweb-4.8.0/cubicweb/test/unittest_migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_predicates.py` & `cubicweb-4.8.0/cubicweb/test/unittest_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_repoapi.py` & `cubicweb-4.8.0/cubicweb/test/unittest_repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_req.py` & `cubicweb-4.8.0/cubicweb/test/unittest_req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_rqlrewrite.py` & `cubicweb-4.8.0/cubicweb/test/unittest_rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_rqlsuggestions.py` & `cubicweb-4.8.0/cubicweb/test/unittest_rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_rset.py` & `cubicweb-4.8.0/cubicweb/test/unittest_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_rtags.py` & `cubicweb-4.8.0/cubicweb/test/unittest_rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_schema.py` & `cubicweb-4.8.0/cubicweb/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_toolsutils.py` & `cubicweb-4.8.0/cubicweb/test/unittest_toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_uilib.py` & `cubicweb-4.8.0/cubicweb/test/unittest_uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_vregistry.py` & `cubicweb-4.8.0/cubicweb/test/unittest_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/test/unittest_wfutils.py` & `cubicweb-4.8.0/cubicweb/test/unittest_wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/toolsutils.py` & `cubicweb-4.8.0/cubicweb/toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/transaction.py` & `cubicweb-4.8.0/cubicweb/transaction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/uilib.py` & `cubicweb-4.8.0/cubicweb/uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/utils.py` & `cubicweb-4.8.0/cubicweb/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/wfutils.py` & `cubicweb-4.8.0/cubicweb/wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb/xy.py` & `cubicweb-4.8.0/cubicweb/xy.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/cubicweb.egg-info/PKG-INFO` & `cubicweb-4.8.0/cubicweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb
-Version: 4.7.1
+Version: 4.8.0
 Summary: a repository of entities / relations for knowledge management
 Home-page: https://www.cubicweb.org
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Requires-Python: >=3.7
 License-File: COPYING
```

### Comparing `cubicweb-4.7.1/cubicweb.egg-info/SOURCES.txt` & `cubicweb-4.8.0/cubicweb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -935,14 +935,15 @@
 doc/changes/4.1.rst
 doc/changes/4.2.rst
 doc/changes/4.3.rst
 doc/changes/4.4.rst
 doc/changes/4.5.rst
 doc/changes/4.6.rst
 doc/changes/4.7.rst
+doc/changes/4.8.rst
 doc/changes/changelog.rst
 doc/changes/index.rst
 doc/images/03-transitions-view_en.png
 doc/images/breadcrumbs_header.png
 doc/images/debugtoolbar_general_panel.png
 doc/images/debugtoolbar_registry_content_panel.png
 doc/images/debugtoolbar_registry_decisions_panel.png
```

### Comparing `cubicweb-4.7.1/doc/4.0.0_how_to_migrate.rst` & `cubicweb-4.8.0/doc/4.0.0_how_to_migrate.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/Makefile` & `cubicweb-4.8.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/_static/favicon.ico` & `cubicweb-4.8.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/_static/logo-cubicweb.svg` & `cubicweb-4.8.0/doc/_static/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/announce.en.txt` & `cubicweb-4.8.0/doc/announce.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/announce.fr.txt` & `cubicweb-4.8.0/doc/announce.fr.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/api/__init__.rst` & `cubicweb-4.8.0/doc/api/__init__.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/api/cwvreg.rst` & `cubicweb-4.8.0/doc/api/cwvreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/api/predicates.rst` & `cubicweb-4.8.0/doc/api/predicates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/api/pyramid/core.rst` & `cubicweb-4.8.0/doc/api/pyramid/core.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/api/urlpublishing.rst` & `cubicweb-4.8.0/doc/api/urlpublishing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/api/web.rst` & `cubicweb-4.8.0/doc/api/web.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-app.en.txt` & `cubicweb-4.8.0/doc/book/MERGE_ME-tut-create-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-gae-app.en.txt` & `cubicweb-4.8.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/_maybe_to_integrate/rss-xml.rst` & `cubicweb-4.8.0/doc/book/_maybe_to_integrate/rss-xml.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/_maybe_to_integrate/template.rst` & `cubicweb-4.8.0/doc/book/_maybe_to_integrate/template.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/additionnal_services/undo.rst` & `cubicweb-4.8.0/doc/book/additionnal_services/undo.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/backups.rst` & `cubicweb-4.8.0/doc/book/admin/backups.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/config.rst` & `cubicweb-4.8.0/doc/book/admin/config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/create-instance.rst` & `cubicweb-4.8.0/doc/book/admin/create-instance.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/cubicweb-ctl.rst` & `cubicweb-4.8.0/doc/book/admin/cubicweb-ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/deploy.rst` & `cubicweb-4.8.0/doc/book/admin/deploy.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/instance-config.rst` & `cubicweb-4.8.0/doc/book/admin/instance-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/ldap.rst` & `cubicweb-4.8.0/doc/book/admin/ldap.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/setup.rst` & `cubicweb-4.8.0/doc/book/admin/setup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/admin/site-config.rst` & `cubicweb-4.8.0/doc/book/admin/site-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/depends.rst` & `cubicweb-4.8.0/doc/book/annexes/depends.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/docstrings-conventions.rst` & `cubicweb-4.8.0/doc/book/annexes/docstrings-conventions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/faq.rst` & `cubicweb-4.8.0/doc/book/annexes/faq.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/mercurial.rst` & `cubicweb-4.8.0/doc/book/annexes/mercurial.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/rql/Graph-ex.gif` & `cubicweb-4.8.0/doc/book/annexes/rql/Graph-ex.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/rql/debugging.rst` & `cubicweb-4.8.0/doc/book/annexes/rql/debugging.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/rql/implementation.rst` & `cubicweb-4.8.0/doc/book/annexes/rql/implementation.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/rql/intro.rst` & `cubicweb-4.8.0/doc/book/annexes/rql/intro.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/rql/language.rst` & `cubicweb-4.8.0/doc/book/annexes/rql/language.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/annexes/rql/usecases.rst` & `cubicweb-4.8.0/doc/book/annexes/rql/usecases.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/connections_pooler.rst` & `cubicweb-4.8.0/doc/book/devrepo/connections_pooler.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/cubes/available-cubes.rst` & `cubicweb-4.8.0/doc/book/devrepo/cubes/available-cubes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/cubes/cc-newcube.rst` & `cubicweb-4.8.0/doc/book/devrepo/cubes/cc-newcube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/cubes/layout.rst` & `cubicweb-4.8.0/doc/book/devrepo/cubes/layout.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/cubes/what-is-a-cube.rst` & `cubicweb-4.8.0/doc/book/devrepo/cubes/what-is-a-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/dataimport.rst` & `cubicweb-4.8.0/doc/book/devrepo/dataimport.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/datamodel/baseschema.rst` & `cubicweb-4.8.0/doc/book/devrepo/datamodel/baseschema.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/datamodel/define-workflows.rst` & `cubicweb-4.8.0/doc/book/devrepo/datamodel/define-workflows.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/datamodel/definition.rst` & `cubicweb-4.8.0/doc/book/devrepo/datamodel/definition.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/datamodel/metadata.rst` & `cubicweb-4.8.0/doc/book/devrepo/datamodel/metadata.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/debug_channels.rst` & `cubicweb-4.8.0/doc/book/devrepo/debug_channels.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/devcore/reqbase.rst` & `cubicweb-4.8.0/doc/book/devrepo/devcore/reqbase.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/entityclasses/adapters.rst` & `cubicweb-4.8.0/doc/book/devrepo/entityclasses/adapters.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/entityclasses/application-logic.rst` & `cubicweb-4.8.0/doc/book/devrepo/entityclasses/application-logic.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/entityclasses/data-as-objects.rst` & `cubicweb-4.8.0/doc/book/devrepo/entityclasses/data-as-objects.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/entityclasses/load-sort.rst` & `cubicweb-4.8.0/doc/book/devrepo/entityclasses/load-sort.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/fti.rst` & `cubicweb-4.8.0/doc/book/devrepo/fti.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/migration.rst` & `cubicweb-4.8.0/doc/book/devrepo/migration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/profiling.rst` & `cubicweb-4.8.0/doc/book/devrepo/profiling.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/repo/hooks.rst` & `cubicweb-4.8.0/doc/book/devrepo/repo/hooks.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/repo/notifications.rst` & `cubicweb-4.8.0/doc/book/devrepo/repo/notifications.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/repo/sessions.rst` & `cubicweb-4.8.0/doc/book/devrepo/repo/sessions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/testing.rst` & `cubicweb-4.8.0/doc/book/devrepo/testing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devrepo/vreg.rst` & `cubicweb-4.8.0/doc/book/devrepo/vreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/ajax.rst` & `cubicweb-4.8.0/doc/book/devweb/ajax.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/controllers.rst` & `cubicweb-4.8.0/doc/book/devweb/controllers.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/css.rst` & `cubicweb-4.8.0/doc/book/devweb/css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/edition/dissection.rst` & `cubicweb-4.8.0/doc/book/devweb/edition/dissection.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/edition/editcontroller.rst` & `cubicweb-4.8.0/doc/book/devweb/edition/editcontroller.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/edition/examples.rst` & `cubicweb-4.8.0/doc/book/devweb/edition/examples.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/edition/form.rst` & `cubicweb-4.8.0/doc/book/devweb/edition/form.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/facets.rst` & `cubicweb-4.8.0/doc/book/devweb/facets.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/httpcaching.rst` & `cubicweb-4.8.0/doc/book/devweb/httpcaching.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/internationalization.rst` & `cubicweb-4.8.0/doc/book/devweb/internationalization.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/js.rst` & `cubicweb-4.8.0/doc/book/devweb/js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/publisher.rst` & `cubicweb-4.8.0/doc/book/devweb/publisher.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/request.rst` & `cubicweb-4.8.0/doc/book/devweb/request.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/resource.rst` & `cubicweb-4.8.0/doc/book/devweb/resource.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/searchbar.rst` & `cubicweb-4.8.0/doc/book/devweb/searchbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/basetemplates.rst` & `cubicweb-4.8.0/doc/book/devweb/views/basetemplates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/baseviews.rst` & `cubicweb-4.8.0/doc/book/devweb/views/baseviews.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/boxes.rst` & `cubicweb-4.8.0/doc/book/devweb/views/boxes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/breadcrumbs.rst` & `cubicweb-4.8.0/doc/book/devweb/views/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/idownloadable.rst` & `cubicweb-4.8.0/doc/book/devweb/views/idownloadable.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/primary.rst` & `cubicweb-4.8.0/doc/book/devweb/views/primary.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/reledit.rst` & `cubicweb-4.8.0/doc/book/devweb/views/reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/startup.rst` & `cubicweb-4.8.0/doc/book/devweb/views/startup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/table.rst` & `cubicweb-4.8.0/doc/book/devweb/views/table.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/urlpublish.rst` & `cubicweb-4.8.0/doc/book/devweb/views/urlpublish.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/views.rst` & `cubicweb-4.8.0/doc/book/devweb/views/views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/views/xmlrss.rst` & `cubicweb-4.8.0/doc/book/devweb/views/xmlrss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/devweb/warning.rst` & `cubicweb-4.8.0/doc/book/devweb/warning.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/intro/concepts.rst` & `cubicweb-4.8.0/doc/book/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/intro/history.rst` & `cubicweb-4.8.0/doc/book/intro/history.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/pyramid/auth.rst` & `cubicweb-4.8.0/doc/book/pyramid/auth.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/pyramid/ctl.rst` & `cubicweb-4.8.0/doc/book/pyramid/ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/pyramid/debug_toolbar.rst` & `cubicweb-4.8.0/doc/book/pyramid/debug_toolbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/pyramid/index.rst` & `cubicweb-4.8.0/doc/book/pyramid/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/pyramid/quickstart.rst` & `cubicweb-4.8.0/doc/book/pyramid/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/pyramid/settings.rst` & `cubicweb-4.8.0/doc/book/pyramid/settings.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/security/csrf.rst` & `cubicweb-4.8.0/doc/book/security/csrf.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/src/archi_globale.dia` & `cubicweb-4.8.0/doc/book/src/archi_globale.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/book/src/main_template_layout.dia` & `cubicweb-4.8.0/doc/book/src/main_template_layout.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.14.rst` & `cubicweb-4.8.0/doc/changes/3.14.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.15.rst` & `cubicweb-4.8.0/doc/changes/3.15.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.16.rst` & `cubicweb-4.8.0/doc/changes/3.16.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.17.rst` & `cubicweb-4.8.0/doc/changes/3.17.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.18.rst` & `cubicweb-4.8.0/doc/changes/3.18.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.19.rst` & `cubicweb-4.8.0/doc/changes/3.19.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.20.rst` & `cubicweb-4.8.0/doc/changes/3.20.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.21.rst` & `cubicweb-4.8.0/doc/changes/3.21.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.22.rst` & `cubicweb-4.8.0/doc/changes/3.22.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.23.rst` & `cubicweb-4.8.0/doc/changes/3.23.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.24.rst` & `cubicweb-4.8.0/doc/changes/3.24.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.25.rst` & `cubicweb-4.8.0/doc/changes/3.25.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.27.rst` & `cubicweb-4.8.0/doc/changes/3.27.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.28.rst` & `cubicweb-4.8.0/doc/changes/3.28.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.29.rst` & `cubicweb-4.8.0/doc/changes/3.29.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.30.rst` & `cubicweb-4.8.0/doc/changes/3.30.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.31.rst` & `cubicweb-4.8.0/doc/changes/3.31.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.32.rst` & `cubicweb-4.8.0/doc/changes/3.32.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.32_reledit.rst` & `cubicweb-4.8.0/doc/changes/3.32_reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.33.rst` & `cubicweb-4.8.0/doc/changes/3.33.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.34.rst` & `cubicweb-4.8.0/doc/changes/3.34.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.35.rst` & `cubicweb-4.8.0/doc/changes/3.35.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.36.rst` & `cubicweb-4.8.0/doc/changes/3.36.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.37.rst` & `cubicweb-4.8.0/doc/changes/3.37.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/3.38.rst` & `cubicweb-4.8.0/doc/changes/3.38.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/4.0.rst` & `cubicweb-4.8.0/doc/changes/4.0.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/4.1.rst` & `cubicweb-4.8.0/doc/changes/4.1.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/4.3.rst` & `cubicweb-4.8.0/doc/changes/4.3.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/4.5.rst` & `cubicweb-4.8.0/doc/changes/4.5.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/4.6.rst` & `cubicweb-4.8.0/doc/changes/4.6.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/changes/changelog.rst` & `cubicweb-4.8.0/doc/changes/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .. -*- coding: utf-8 -*-
 
+.. include:: 4.8.rst
 .. include:: 4.7.rst
 .. include:: 4.6.rst
 .. include:: 4.5.rst
 .. include:: 4.4.rst
 .. include:: 4.3.rst
 .. include:: 4.2.rst
 .. include:: 4.1.rst
```

### Comparing `cubicweb-4.7.1/doc/conf.py` & `cubicweb-4.8.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/03-transitions-view_en.png` & `cubicweb-4.8.0/doc/images/03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/breadcrumbs_header.png` & `cubicweb-4.8.0/doc/images/breadcrumbs_header.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_general_panel.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_general_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_registry_content_panel.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_registry_content_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_registry_decisions_panel.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_registry_decisions_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_rql_panel.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_rql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_rql_traceback_panel.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_rql_traceback_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_show_source.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_show_source.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_show_source_link.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_show_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_sql_panel.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_sql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/debugtoolbar_traceback_source_link.png` & `cubicweb-4.8.0/doc/images/debugtoolbar_traceback_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/example-card-with-rql-directive.png` & `cubicweb-4.8.0/doc/images/example-card-with-rql-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/example-card-with-rql-table-directive.png` & `cubicweb-4.8.0/doc/images/example-card-with-rql-table-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/facet_date_range.png` & `cubicweb-4.8.0/doc/images/facet_date_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/facet_has_image.png` & `cubicweb-4.8.0/doc/images/facet_has_image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/facet_overview.png` & `cubicweb-4.8.0/doc/images/facet_overview.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/facet_range.png` & `cubicweb-4.8.0/doc/images/facet_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_00-login_en.png` & `cubicweb-4.8.0/doc/images/lax-book_00-login_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_01-start_en.png` & `cubicweb-4.8.0/doc/images/lax-book_01-start_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_02-cookie-values_en.png` & `cubicweb-4.8.0/doc/images/lax-book_02-cookie-values_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_02-create-blog_en.png` & `cubicweb-4.8.0/doc/images/lax-book_02-create-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_03-list-one-blog_en.png` & `cubicweb-4.8.0/doc/images/lax-book_03-list-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_03-site-config-panel_en.png` & `cubicweb-4.8.0/doc/images/lax-book_03-site-config-panel_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_03-state-submitted_en.png` & `cubicweb-4.8.0/doc/images/lax-book_03-state-submitted_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_03-transitions-view_en.png` & `cubicweb-4.8.0/doc/images/lax-book_03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_04-detail-one-blog_en.png` & `cubicweb-4.8.0/doc/images/lax-book_04-detail-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_05-list-two-blog_en.png` & `cubicweb-4.8.0/doc/images/lax-book_05-list-two-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_06-add-relation-entryof_en.png` & `cubicweb-4.8.0/doc/images/lax-book_06-add-relation-entryof_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_06-main-template-logo_en.png` & `cubicweb-4.8.0/doc/images/lax-book_06-main-template-logo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_07-detail-one-blogentry_en.png` & `cubicweb-4.8.0/doc/images/lax-book_07-detail-one-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_08-schema_en.png` & `cubicweb-4.8.0/doc/images/lax-book_08-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_09-new-view-blogentry_en.png` & `cubicweb-4.8.0/doc/images/lax-book_09-new-view-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/lax-book_10-blog-with-two-entries_en.png` & `cubicweb-4.8.0/doc/images/lax-book_10-blog-with-two-entries_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/main_template.png` & `cubicweb-4.8.0/doc/images/main_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/main_template.svg` & `cubicweb-4.8.0/doc/images/main_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/main_template_layout.png` & `cubicweb-4.8.0/doc/images/main_template_layout.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/primaryview_template.png` & `cubicweb-4.8.0/doc/images/primaryview_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/primaryview_template.svg` & `cubicweb-4.8.0/doc/images/primaryview_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/request_session.png` & `cubicweb-4.8.0/doc/images/request_session.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/request_session.svg` & `cubicweb-4.8.0/doc/images/request_session.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/server-class-diagram.png` & `cubicweb-4.8.0/doc/images/server-class-diagram.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_blog-form_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_blog-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_blog-primary-after-post-creation_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_blog-primary_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_blog-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_blogs-list_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_blogs-list_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_form-generic-relations_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_form-generic-relations_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_index_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_index_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_index_gettext_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_index_gettext_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_index_logged_in_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_index_logged_in_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_login-form_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_login-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-community-custom-primary_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-community-custom-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-community-default-primary_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-community-default-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-community-taggable-primary_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-custom-footer_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-custom-footer_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-schema_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_myblog-siteinfo_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_myblog-siteinfo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_schema_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_schema_graphviz_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_schema_graphviz_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-base_siteconfig_en.png` & `cubicweb-4.8.0/doc/images/tutos-base_siteconfig_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_admin.png` & `cubicweb-4.8.0/doc/images/tutos-museum_admin.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_city_created.png` & `cubicweb-4.8.0/doc/images/tutos-museum_city_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_city_creation.png` & `cubicweb-4.8.0/doc/images/tutos-museum_city_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_data_model_schema.png` & `cubicweb-4.8.0/doc/images/tutos-museum_data_model_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_empty_instance.png` & `cubicweb-4.8.0/doc/images/tutos-museum_empty_instance.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_finished_import.png` & `cubicweb-4.8.0/doc/images/tutos-museum_finished_import.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_list_view.png` & `cubicweb-4.8.0/doc/images/tutos-museum_list_view.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_museum_created.png` & `cubicweb-4.8.0/doc/images/tutos-museum_museum_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_museum_creation.png` & `cubicweb-4.8.0/doc/images/tutos-museum_museum_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_museum_with_city_name.png` & `cubicweb-4.8.0/doc/images/tutos-museum_museum_with_city_name.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_react_map.png` & `cubicweb-4.8.0/doc/images/tutos-museum_react_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-museum_with_schema.png` & `cubicweb-4.8.0/doc/images/tutos-museum_with_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_background-image.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_background-image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_boxes.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_boxes.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_breadcrumbs.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_breadcrumbs.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_facets.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_facets.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_grey-box.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_grey-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_index-after.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_index-after.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_index-before.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_index-before.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_login-box.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_login-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_prevnext.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_prevnext.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_ui1.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_ui1.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_ui2.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_ui2.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/tutos-photowebsite_ui3.png` & `cubicweb-4.8.0/doc/images/tutos-photowebsite_ui3.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/undo_history-view_w600.png` & `cubicweb-4.8.0/doc/images/undo_history-view_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/undo_mesage_w600.png` & `cubicweb-4.8.0/doc/images/undo_mesage_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/undo_startup-link_w600.png` & `cubicweb-4.8.0/doc/images/undo_startup-link_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/views-table-filter-shadow.png` & `cubicweb-4.8.0/doc/images/views-table-filter-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/views-table-filter.png` & `cubicweb-4.8.0/doc/images/views-table-filter.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/views-table-shadow.png` & `cubicweb-4.8.0/doc/images/views-table-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/images/views-table.png` & `cubicweb-4.8.0/doc/images/views-table.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/index.rst` & `cubicweb-4.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/plan_formation_python_cubicweb.txt` & `cubicweb-4.8.0/doc/plan_formation_python_cubicweb.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tools/generate_modules.py` & `cubicweb-4.8.0/doc/tools/generate_modules.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tools/mode_plan.py` & `cubicweb-4.8.0/doc/tools/mode_plan.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tools/pyjsrest.py` & `cubicweb-4.8.0/doc/tools/pyjsrest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/advanced/index.rst` & `cubicweb-4.8.0/doc/tutorials/advanced/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/advanced/part01_create-cube.rst` & `cubicweb-4.8.0/doc/tutorials/advanced/part01_create-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/advanced/part02_security.rst` & `cubicweb-4.8.0/doc/tutorials/advanced/part02_security.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/advanced/part03_bfss.rst` & `cubicweb-4.8.0/doc/tutorials/advanced/part03_bfss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/advanced/part04_ui-base.rst` & `cubicweb-4.8.0/doc/tutorials/advanced/part04_ui-base.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/advanced/part05_ui-advanced.rst` & `cubicweb-4.8.0/doc/tutorials/advanced/part05_ui-advanced.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/base/blog-in-five-minutes.rst` & `cubicweb-4.8.0/doc/tutorials/base/blog-in-five-minutes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/base/conclusion.rst` & `cubicweb-4.8.0/doc/tutorials/base/conclusion.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/base/customizing-the-application.rst` & `cubicweb-4.8.0/doc/tutorials/base/customizing-the-application.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/base/discovering-the-ui.rst` & `cubicweb-4.8.0/doc/tutorials/base/discovering-the-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/base/index.rst` & `cubicweb-4.8.0/doc/tutorials/base/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_import.py` & `cubicweb-4.8.0/doc/tutorials/dataimport/diseasome_import.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_parser.py` & `cubicweb-4.8.0/doc/tutorials/dataimport/diseasome_parser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/dataimport/index.rst` & `cubicweb-4.8.0/doc/tutorials/dataimport/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/dataimport/schema.py` & `cubicweb-4.8.0/doc/tutorials/dataimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/index.rst` & `cubicweb-4.8.0/doc/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/museum/data-management.rst` & `cubicweb-4.8.0/doc/tutorials/museum/data-management.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/museum/develop-app.rst` & `cubicweb-4.8.0/doc/tutorials/museum/develop-app.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/museum/develop-ui.rst` & `cubicweb-4.8.0/doc/tutorials/museum/develop-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/museum/enhance-views.rst` & `cubicweb-4.8.0/doc/tutorials/museum/enhance-views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/museum/getting-started.rst` & `cubicweb-4.8.0/doc/tutorials/museum/getting-started.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/doc/tutorials/museum/index.rst` & `cubicweb-4.8.0/doc/tutorials/museum/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/extras/cubicweb-ctl.bash_completion` & `cubicweb-4.8.0/extras/cubicweb-ctl.bash_completion`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/jshintrc` & `cubicweb-4.8.0/jshintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/man/cubicweb-ctl.1` & `cubicweb-4.8.0/man/cubicweb-ctl.1`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/pylintrc` & `cubicweb-4.8.0/pylintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/setup.py` & `cubicweb-4.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.1/tox.ini` & `cubicweb-4.8.0/tox.ini`

 * *Files identical despite different names*

