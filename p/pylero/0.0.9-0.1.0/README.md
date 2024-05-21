# Comparing `tmp/pylero-0.0.9.tar.gz` & `tmp/pylero-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylero-0.0.9.tar", last modified: Tue Mar  5 21:30:11 2024, max compression
+gzip compressed data, was "pylero-0.1.0.tar", last modified: Tue May 21 13:55:07 2024, max compression
```

## Comparing `pylero-0.0.9.tar` & `pylero-0.1.0.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.107506 pylero-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-05 21:30:07.000000 pylero-0.0.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-05 21:30:07.000000 pylero-0.0.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.067505 pylero-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.071505 pylero-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-05 21:30:07.000000 pylero-0.0.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-05 21:30:07.000000 pylero-0.0.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-05 21:30:07.000000 pylero-0.0.9/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-05 21:30:07.000000 pylero-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-05 21:30:07.000000 pylero-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-05 21:30:07.000000 pylero-0.0.9/.project
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.071505 pylero-0.0.9/.tito/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.071505 pylero-0.0.9/.tito/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-05 21:30:07.000000 pylero-0.0.9/.tito/packages/.readme
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-05 21:30:07.000000 pylero-0.0.9/.tito/packages/python-pylero
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-05 21:30:07.000000 pylero-0.0.9/.tito/tito.props
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-03-05 21:30:07.000000 pylero-0.0.9/CONTRIBUTION.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-05 21:30:07.000000 pylero-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-05 21:30:07.000000 pylero-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-03-05 21:30:11.107506 pylero-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-03-05 21:30:07.000000 pylero-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.075506 pylero-0.0.9/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.067505 pylero-0.0.9/doc/_build/
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/pylero.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-03-05 21:30:07.000000 pylero-0.0.9/doc/pylero.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.079506 pylero-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.079506 pylero-0.0.9/docs/_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.091506 pylero-0.0.9/docs/_modules/pylero/
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/activity.html
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/activity_comment.html
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/activity_custom_value.html
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/activity_custom_value_entry.html
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/activity_source.html
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/approval.html
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/attachment.html
--rw-r--r--   0 runner    (1001) docker     (127)   149879 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/base_polarion.html
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/baseline.html
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/build.html
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/build_linked_work_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/build_test_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/category.html
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/change.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.091506 pylero-0.0.9/docs/_modules/pylero/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    68275 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/cli/cmd.html
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/comment.html
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/custom.html
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/custom_field.html
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/custom_field_type.html
--rw-r--r--   0 runner    (1001) docker     (127)    68514 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/document.html
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/enum_custom_field_type.html
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/enum_option.html
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/enum_option_id.html
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/exceptions.html
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/externally_linked_work_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/field_diff.html
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/hyperlink.html
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/imported_comment.html
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/language_definition.html
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/license_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/linked_work_item.html
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/module_comment.html
--rw-r--r--   0 runner    (1001) docker     (127)    47235 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/plan.html
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/plan_record.html
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/plan_statistics.html
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/planning_constraint.html
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/priority_opt.html
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/priority_option_id.html
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/product_license.html
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/project.html
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/project_group.html
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/properties.html
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/property.html
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/revision.html
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/server.html
--rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/session.html
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/signature.html
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/signature_context.html
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/signature_data.html
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/subterra_uri.html
--rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/test_record.html
--rw-r--r--   0 runner    (1001) docker     (127)   162552 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/test_run.html
--rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/test_run_attachment.html
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/test_step.html
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/test_step_result.html
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/test_steps.html
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/tests_configuration.html
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/text.html
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/time_point.html
--rw-r--r--   0 runner    (1001) docker     (127)    25673 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/user.html
--rw-r--r--   0 runner    (1001) docker     (127)    23763 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/wiki_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/wiki_page_attachment.html
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/work_record.html
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_modules/pylero/workflow_action.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.091506 pylero-0.0.9/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_sources/modules.rst.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_sources/pylero.cli.rst.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_sources/pylero.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.091506 pylero-0.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15096 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)   113509 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    68129 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   153726 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/modules.html
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    30080 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/pylero.cli.html
--rw-r--r--   0 runner    (1001) docker     (127)   562423 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/pylero.html
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (127)   136995 2024-03-05 21:30:07.000000 pylero-0.0.9/docs/searchindex.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     3294 2024-03-05 21:30:07.000000 pylero-0.0.9/gen_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.107506 pylero-0.0.9/pylero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-03-05 21:30:11.000000 pylero-0.0.9/pylero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-05 21:30:11.000000 pylero-0.0.9/pylero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 21:30:11.000000 pylero-0.0.9/pylero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-05 21:30:11.000000 pylero-0.0.9/pylero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-05 21:30:11.000000 pylero-0.0.9/pylero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-05 21:30:07.000000 pylero-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-05 21:30:07.000000 pylero-0.0.9/python-pylero.spec
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-05 21:30:07.000000 pylero-0.0.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.095506 pylero-0.0.9/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2871 2024-03-05 21:30:07.000000 pylero-0.0.9/scripts/pylero
--rwxr-xr-x   0 runner    (1001) docker     (127)     8196 2024-03-05 21:30:07.000000 pylero-0.0.9/scripts/pylero-cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 21:30:11.107506 pylero-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-05 21:30:07.000000 pylero-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.071505 pylero-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.103506 pylero-0.0.9/src/pylero/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/_compatible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/activity_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/activity_custom_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/activity_custom_value_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/activity_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/approval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    43702 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/base_polarion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/build_linked_work_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/build_test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/category.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/change.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.107506 pylero-0.0.9/src/pylero/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/cli/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/custom_field_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/enum_custom_field_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/enum_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/enum_option_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/externally_linked_work_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/field_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/imported_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/language_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/license_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/linked_work_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/module_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/plan_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/plan_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/planning_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/priority_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/priority_option_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/product_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/project_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/pylero.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/signature_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/signature_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/subterra_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    52791 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/test_run_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/tests_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/time_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/wiki_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/wiki_page_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    56618 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/work_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/work_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-05 21:30:07.000000 pylero-0.0.9/src/pylero/workflow_action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.107506 pylero-0.0.9/src/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/attribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/document_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/plan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 21:30:11.107506 pylero-0.0.9/src/unit_tests/refs/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/refs/red_box.png
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/revert_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15810 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/test_run_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-03-05 21:30:07.000000 pylero-0.0.9/src/unit_tests/work_item_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-05 21:30:07.000000 pylero-0.0.9/tier_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-05 21:30:07.000000 pylero-0.0.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.945571 pylero-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 13:55:04.000000 pylero-0.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 13:55:04.000000 pylero-0.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.901570 pylero-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.905570 pylero-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-21 13:55:04.000000 pylero-0.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-21 13:55:04.000000 pylero-0.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-21 13:55:04.000000 pylero-0.1.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 13:55:04.000000 pylero-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-21 13:55:04.000000 pylero-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 13:55:04.000000 pylero-0.1.0/.project
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.905570 pylero-0.1.0/.tito/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.905570 pylero-0.1.0/.tito/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 13:55:04.000000 pylero-0.1.0/.tito/packages/.readme
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 13:55:04.000000 pylero-0.1.0/.tito/packages/python-pylero
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 13:55:04.000000 pylero-0.1.0/.tito/tito.props
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-21 13:55:04.000000 pylero-0.1.0/CONTRIBUTION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 13:55:04.000000 pylero-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 13:55:04.000000 pylero-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-21 13:55:07.945571 pylero-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-21 13:55:04.000000 pylero-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.909570 pylero-0.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.901570 pylero-0.1.0/doc/_build/
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/pylero.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-05-21 13:55:04.000000 pylero-0.1.0/doc/pylero.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.913571 pylero-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.913571 pylero-0.1.0/docs/_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.925571 pylero-0.1.0/docs/_modules/pylero/
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/activity.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/activity_comment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/activity_custom_value.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/activity_custom_value_entry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/activity_source.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/approval.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/attachment.html
+-rw-r--r--   0 runner    (1001) docker     (127)   153863 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/base_polarion.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/baseline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/build.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/build_linked_work_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/build_test_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/category.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/change.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.925571 pylero-0.1.0/docs/_modules/pylero/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    68281 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/cli/cmd.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/comment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/custom.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/custom_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/custom_field_type.html
+-rw-r--r--   0 runner    (1001) docker     (127)    68520 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/document.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/enum_custom_field_type.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/enum_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/enum_option_id.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/exceptions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/externally_linked_work_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/field_diff.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/hyperlink.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/imported_comment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/language_definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/license_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/linked_work_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/module_comment.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47241 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/plan.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/plan_record.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/plan_statistics.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/planning_constraint.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/priority_opt.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/priority_option_id.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/product_license.html
+-rw-r--r--   0 runner    (1001) docker     (127)    33073 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/project.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17192 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/project_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/properties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/property.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/revision.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/server.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35946 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/session.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/signature.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/signature_context.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/signature_data.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/subterra_uri.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14561 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/test_record.html
+-rw-r--r--   0 runner    (1001) docker     (127)   172443 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/test_run.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/test_run_attachment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/test_step.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/test_step_result.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/test_steps.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/tests_configuration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/text.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/time_point.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25679 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/user.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/wiki_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/wiki_page_attachment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/work_record.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_modules/pylero/workflow_action.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.925571 pylero-0.1.0/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_sources/modules.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_sources/pylero.cli.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_sources/pylero.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.929571 pylero-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15096 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20731 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)   113708 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    67699 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   154005 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/modules.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30086 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/pylero.cli.html
+-rw-r--r--   0 runner    (1001) docker     (127)   563907 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/pylero.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)   142810 2024-05-21 13:55:04.000000 pylero-0.1.0/docs/searchindex.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3294 2024-05-21 13:55:04.000000 pylero-0.1.0/gen_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.941571 pylero-0.1.0/pylero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-05-21 13:55:07.000000 pylero-0.1.0/pylero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-21 13:55:07.000000 pylero-0.1.0/pylero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:55:07.000000 pylero-0.1.0/pylero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 13:55:07.000000 pylero-0.1.0/pylero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 13:55:07.000000 pylero-0.1.0/pylero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 13:55:04.000000 pylero-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-21 13:55:04.000000 pylero-0.1.0/python-pylero.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 13:55:04.000000 pylero-0.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.929571 pylero-0.1.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2871 2024-05-21 13:55:04.000000 pylero-0.1.0/scripts/pylero
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8196 2024-05-21 13:55:04.000000 pylero-0.1.0/scripts/pylero-cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:55:07.945571 pylero-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-21 13:55:04.000000 pylero-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.901570 pylero-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.941571 pylero-0.1.0/src/pylero/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/_compatible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/activity_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/activity_custom_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/activity_custom_value_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/activity_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44776 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/base_polarion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/build_linked_work_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/build_test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/change.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.941571 pylero-0.1.0/src/pylero/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/cli/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/custom_field_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/enum_custom_field_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/enum_option_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/externally_linked_work_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/field_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/imported_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/language_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/license_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/linked_work_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/module_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/plan_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/plan_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/planning_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/priority_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/priority_option_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/product_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/project_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/pylero.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/signature_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/signature_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/subterra_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56645 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/test_run_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/tests_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/time_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/wiki_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/wiki_page_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56867 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/work_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/work_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-21 13:55:04.000000 pylero-0.1.0/src/pylero/workflow_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.941571 pylero-0.1.0/src/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/attribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/document_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/plan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:55:07.941571 pylero-0.1.0/src/unit_tests/refs/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/refs/red_box.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/revert_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15810 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/test_run_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-05-21 13:55:04.000000 pylero-0.1.0/src/unit_tests/work_item_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-21 13:55:04.000000 pylero-0.1.0/tier_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-21 13:55:04.000000 pylero-0.1.0/tox.ini
```

### Comparing `pylero-0.0.9/.github/workflows/codeql-analysis.yml` & `pylero-0.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/.github/workflows/publish-to-pypi.yml` & `pylero-0.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/.github/workflows/pull_request.yml` & `pylero-0.1.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/CONTRIBUTION.rst` & `pylero-0.1.0/CONTRIBUTION.rst`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/LICENSE` & `pylero-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/PKG-INFO` & `pylero-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylero
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python SDK for Polarion
 Home-page: https://github.com/RedHatQE/pylero
 Author: pylero Developers
 Author-email: dno-tools@redhat.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pylero-0.0.9/README.md` & `pylero-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/doc/Makefile` & `pylero-0.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/doc/conf.py` & `pylero-0.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/doc/index.rst` & `pylero-0.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/doc/make.bat` & `pylero-0.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/doc/pylero.rst` & `pylero-0.1.0/doc/pylero.rst`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/docs/_modules/index.html` & `pylero-0.1.0/docs/_modules/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Overview: module code &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../_static/alabaster.css?v=12dfc556" />
     <script src="../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../_static/doctools.js?v=888ff710"></script>
+    <script src="../_static/doctools.js?v=9a2dae69"></script>
     <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
    
   <link rel="stylesheet" href="../_static/custom.css" type="text/css" />
   
 
@@ -119,23 +119,23 @@
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="../index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -145,15 +145,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -66,9 +66,9 @@
 ************ _pp_yy_ll_ee_rr_oo ************
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/activity.html` & `pylero-0.1.0/docs/_modules/pylero/activity.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.activity &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -104,23 +104,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -130,15 +130,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -50,9 +50,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/activity_comment.html` & `pylero-0.1.0/docs/_modules/pylero/activity_comment.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.activity_comment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -86,23 +86,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -112,15 +112,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -32,9 +32,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/activity_custom_value.html` & `pylero-0.1.0/docs/_modules/pylero/activity_custom_value.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.activity_custom_value &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -78,23 +78,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -104,15 +104,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -25,9 +25,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/activity_custom_value_entry.html` & `pylero-0.1.0/docs/_modules/pylero/activity_custom_value_entry.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.activity_custom_value_entry &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -85,23 +85,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -111,15 +111,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -32,9 +32,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/activity_source.html` & `pylero-0.1.0/docs/_modules/pylero/activity_source.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.activity_source &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -86,23 +86,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -112,15 +112,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -32,9 +32,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/approval.html` & `pylero-0.1.0/docs/_modules/pylero/approval.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.approval &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -98,23 +98,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -124,15 +124,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -45,9 +45,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/attachment.html` & `pylero-0.1.0/docs/_modules/pylero/attachment.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.attachment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -103,23 +103,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -129,15 +129,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -50,9 +50,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/base_polarion.html` & `pylero-0.1.0/docs/_modules/pylero/base_polarion.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.base_polarion &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -377,21 +377,25 @@
         <span class="k">if</span> <span class="n">fields</span><span class="p">:</span>
             <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">fields</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
                 <span class="n">fields</span> <span class="o">=</span> <span class="p">[</span><span class="n">fields</span><span class="p">]</span>
             <span class="c1"># convert given fields to Polarion fields</span>
             <span class="n">p_fields</span> <span class="o">=</span> <span class="p">[</span>
                 <span class="s2">&quot;</span><span class="si">%s%s</span><span class="s2">&quot;</span>
                 <span class="o">%</span> <span class="p">(</span>
-                    <span class="s2">&quot;customFields.&quot;</span>
-                    <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">],</span> <span class="nb">dict</span><span class="p">)</span>
-                    <span class="ow">and</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">]</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;is_custom&quot;</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-                    <span class="k">else</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-                    <span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">]</span>
-                    <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">],</span> <span class="nb">dict</span><span class="p">)</span>
-                    <span class="k">else</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">][</span><span class="s2">&quot;field_name&quot;</span><span class="p">],</span>
+                    <span class="p">(</span>
+                        <span class="s2">&quot;customFields.&quot;</span>
+                        <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">],</span> <span class="nb">dict</span><span class="p">)</span>
+                        <span class="ow">and</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">]</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;is_custom&quot;</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+                        <span class="k">else</span> <span class="s2">&quot;&quot;</span>
+                    <span class="p">),</span>
+                    <span class="p">(</span>
+                        <span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">]</span>
+                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">],</span> <span class="nb">dict</span><span class="p">)</span>
+                        <span class="k">else</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="n">x</span><span class="p">][</span><span class="s2">&quot;field_name&quot;</span><span class="p">]</span>
+                    <span class="p">),</span>
                 <span class="p">)</span>
                 <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">fields</span>
             <span class="p">]</span>
             <span class="c1"># Omit &#39;URIs&#39; and &#39;URI&#39; from URIFields</span>
             <span class="n">p_fields</span> <span class="o">=</span> <span class="p">[(</span><span class="n">x</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;URIs&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;URI&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">))</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">p_fields</span><span class="p">]</span>
         <span class="k">return</span> <span class="n">p_fields</span>
 
@@ -1165,14 +1169,57 @@
 <span class="sd">        Returns:</span>
 <span class="sd">            None</span>
 <span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="k">if</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;uri&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">):</span>
             <span class="n">obj</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="vm">__class__</span><span class="p">(</span><span class="n">uri</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">uri</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_suds_object</span> <span class="o">=</span> <span class="n">obj</span><span class="o">.</span><span class="n">_suds_object</span></div>
+
+
+<div class="viewcode-block" id="BasePolarion.get_revision">
+<a class="viewcode-back" href="../../pylero.html#pylero.base_polarion.BasePolarion.get_revision">[docs]</a>
+    <span class="k">def</span> <span class="nf">get_revision</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">repository_name</span><span class="p">,</span> <span class="n">revision_id</span><span class="p">):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        Gets a revision</span>
+<span class="sd">        Args:</span>
+<span class="sd">            repository_name - The repository name. (Put &quot;default&quot; for the default repository.)</span>
+<span class="sd">            revision_id - The revision name.</span>
+<span class="sd">        Returns:</span>
+<span class="sd">            a Revision object</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">session</span><span class="o">.</span><span class="n">tracker_client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">getrevision</span><span class="p">(</span>
+            <span class="n">repository_name</span><span class="p">,</span> <span class="n">revision_id</span>
+        <span class="p">)</span></div>
+
+
+<div class="viewcode-block" id="BasePolarion.get_revision_by_uri">
+<a class="viewcode-back" href="../../pylero.html#pylero.base_polarion.BasePolarion.get_revision_by_uri">[docs]</a>
+    <span class="k">def</span> <span class="nf">get_revision_by_uri</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">revision_uri</span><span class="p">):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        Gets a revision by its URI</span>
+<span class="sd">        Args:</span>
+<span class="sd">             revision_uri - The URI of the revision.</span>
+<span class="sd">        Returns:</span>
+<span class="sd">            a Revision object</span>
+
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">session</span><span class="o">.</span><span class="n">tracker_client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">getRevisionByUri</span><span class="p">(</span><span class="n">revision_uri</span><span class="p">)</span></div>
+
+
+<div class="viewcode-block" id="BasePolarion.get_revisions">
+<a class="viewcode-back" href="../../pylero.html#pylero.base_polarion.BasePolarion.get_revisions">[docs]</a>
+    <span class="k">def</span> <span class="nf">get_revisions</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">uri</span><span class="p">):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">        Returns all revisions for a specific URI.</span>
+<span class="sd">        Args:</span>
+<span class="sd">             uri - URI of the persistence object (Work Item, Module/Document, User, etc).</span>
+<span class="sd">        Returns:</span>
+<span class="sd">            All revisions for a specific URI.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">session</span><span class="o">.</span><span class="n">tracker_client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">getRevisions</span><span class="p">(</span><span class="n">uri</span><span class="p">)</span></div>
 </div>
 
 </pre></div>
 
           </div>
           
         </div>
@@ -1198,23 +1245,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -1224,15 +1271,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -357,21 +357,25 @@
         if fields:
             if not isinstance(fields, list):
                 fields = [fields]
             # convert given fields to Polarion fields
             p_fields = [
                 "%s%s"
                 % (
-                    "customFields."
-                    if isinstance(cls._cls_suds_map[x], dict)
-                    and cls._cls_suds_map[x].get("is_custom", False)
-                    else "",
-                    cls._cls_suds_map[x]
-                    if not isinstance(cls._cls_suds_map[x], dict)
-                    else cls._cls_suds_map[x]["field_name"],
+                    (
+                        "customFields."
+                        if isinstance(cls._cls_suds_map[x], dict)
+                        and cls._cls_suds_map[x].get("is_custom", False)
+                        else ""
+                    ),
+                    (
+                        cls._cls_suds_map[x]
+                        if not isinstance(cls._cls_suds_map[x], dict)
+                        else cls._cls_suds_map[x]["field_name"]
+                    ),
                 )
                 for x in fields
             ]
             # Omit 'URIs' and 'URI' from URIFields
             p_fields = [(x.replace("URIs", "").replace("URI", "")) for x in
 p_fields]
         return p_fields
@@ -1198,17 +1202,66 @@
         """
 
         if getattr(self, "uri", None):
             obj = self.__class__(uri=self.uri)
             self._suds_object = obj._suds_object
 
 
+
+
+_[_d_o_c_s_]
+    def get_revision(self, repository_name, revision_id):
+        """
+        Gets a revision
+        Args:
+            repository_name - The repository name. (Put "default" for the
+default repository.)
+            revision_id - The revision name.
+        Returns:
+            a Revision object
+        """
+        return self.session.tracker_client.service.getrevision(
+            repository_name, revision_id
+        )
+
+
+
+
+_[_d_o_c_s_]
+    def get_revision_by_uri(self, revision_uri):
+        """
+        Gets a revision by its URI
+        Args:
+             revision_uri - The URI of the revision.
+        Returns:
+            a Revision object
+
+        """
+        return self.session.tracker_client.service.getRevisionByUri
+(revision_uri)
+
+
+
+
+_[_d_o_c_s_]
+    def get_revisions(self, uri):
+        """
+        Returns all revisions for a specific URI.
+        Args:
+             uri - URI of the persistence object (Work Item, Module/Document,
+User, etc).
+        Returns:
+            All revisions for a specific URI.
+        """
+        return self.session.tracker_client.service.getRevisions(uri)
+
+
 ************ _pp_yy_ll_ee_rr_oo ************
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/baseline.html` & `pylero-0.1.0/docs/_modules/pylero/baseline.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.baseline &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -141,23 +141,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -167,15 +167,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -89,9 +89,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/build.html` & `pylero-0.1.0/docs/_modules/pylero/build.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.build &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -125,23 +125,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -151,15 +151,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -71,9 +71,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/build_linked_work_item.html` & `pylero-0.1.0/docs/_modules/pylero/build_linked_work_item.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.build_linked_work_item &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -100,23 +100,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -126,15 +126,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -47,9 +47,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/build_test_results.html` & `pylero-0.1.0/docs/_modules/pylero/build_test_results.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.build_test_results &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -88,23 +88,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -114,15 +114,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -34,9 +34,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/category.html` & `pylero-0.1.0/docs/_modules/pylero/category.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.category &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -96,23 +96,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -122,15 +122,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -43,9 +43,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/change.html` & `pylero-0.1.0/docs/_modules/pylero/change.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.change &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -95,23 +95,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -121,15 +121,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -41,9 +41,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/cli/cmd.html` & `pylero-0.1.0/docs/_modules/pylero/cli/cmd.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.cli.cmd &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../../_static/alabaster.css?v=12dfc556" />
     <script src="../../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../../genindex.html" />
     <link rel="search" title="Search" href="../../../search.html" />
    
   <link rel="stylesheet" href="../../../_static/custom.css" type="text/css" />
   
 
@@ -505,23 +505,23 @@
 <ul>
   <li><a href="../../../index.html">Documentation overview</a><ul>
   <li><a href="../../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -531,15 +531,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -475,9 +475,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/comment.html` & `pylero-0.1.0/docs/_modules/pylero/comment.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.comment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -130,23 +130,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -156,15 +156,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -79,9 +79,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/custom.html` & `pylero-0.1.0/docs/_modules/pylero/custom.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.custom &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -100,23 +100,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -126,15 +126,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -47,9 +47,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/custom_field.html` & `pylero-0.1.0/docs/_modules/pylero/custom_field.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.custom_field &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -80,23 +80,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -106,15 +106,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -27,9 +27,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/custom_field_type.html` & `pylero-0.1.0/docs/_modules/pylero/custom_field_type.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.custom_field_type &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -99,23 +99,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -125,15 +125,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -46,9 +46,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/document.html` & `pylero-0.1.0/docs/_modules/pylero/document.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.document &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -667,23 +667,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -693,15 +693,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -637,9 +637,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/enum_custom_field_type.html` & `pylero-0.1.0/docs/_modules/pylero/enum_custom_field_type.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.enum_custom_field_type &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -100,23 +100,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -126,15 +126,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -46,9 +46,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/enum_option.html` & `pylero-0.1.0/docs/_modules/pylero/enum_option.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.enum_option &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -97,23 +97,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -123,15 +123,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -43,9 +43,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/enum_option_id.html` & `pylero-0.1.0/docs/_modules/pylero/enum_option_id.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.enum_option_id &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -93,23 +93,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -119,15 +119,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -40,9 +40,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/exceptions.html` & `pylero-0.1.0/docs/_modules/pylero/exceptions.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.exceptions &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -69,23 +69,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -95,15 +95,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -15,9 +15,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/externally_linked_work_item.html` & `pylero-0.1.0/docs/_modules/pylero/externally_linked_work_item.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.externally_linked_work_item &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -118,23 +118,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -144,15 +144,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -66,9 +66,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/field_diff.html` & `pylero-0.1.0/docs/_modules/pylero/field_diff.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.field_diff &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -92,23 +92,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -118,15 +118,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -38,9 +38,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/hyperlink.html` & `pylero-0.1.0/docs/_modules/pylero/hyperlink.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.hyperlink &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -95,23 +95,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -121,15 +121,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -42,9 +42,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/imported_comment.html` & `pylero-0.1.0/docs/_modules/pylero/imported_comment.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.imported_comment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -86,23 +86,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -112,15 +112,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -32,9 +32,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/language_definition.html` & `pylero-0.1.0/docs/_modules/pylero/language_definition.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.language_definition &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -84,23 +84,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -110,15 +110,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -30,9 +30,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/license_info.html` & `pylero-0.1.0/docs/_modules/pylero/license_info.html`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.license_info &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -84,23 +84,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -110,15 +110,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -30,9 +30,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/linked_work_item.html` & `pylero-0.1.0/docs/_modules/pylero/linked_work_item.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.linked_work_item &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -122,23 +122,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -148,15 +148,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -70,9 +70,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/module_comment.html` & `pylero-0.1.0/docs/_modules/pylero/module_comment.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.module_comment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -133,23 +133,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -159,15 +159,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -83,9 +83,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/plan.html` & `pylero-0.1.0/docs/_modules/pylero/plan.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.plan &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -506,23 +506,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -532,15 +532,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -478,9 +478,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/plan_record.html` & `pylero-0.1.0/docs/_modules/pylero/plan_record.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.plan_record &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -91,23 +91,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -117,15 +117,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -38,9 +38,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/plan_statistics.html` & `pylero-0.1.0/docs/_modules/pylero/plan_statistics.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.plan_statistics &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -106,23 +106,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -132,15 +132,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -52,9 +52,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/planning_constraint.html` & `pylero-0.1.0/docs/_modules/pylero/planning_constraint.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.planning_constraint &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -93,23 +93,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -119,15 +119,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -40,9 +40,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/priority_opt.html` & `pylero-0.1.0/docs/_modules/pylero/priority_opt.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.priority_opt &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -99,23 +99,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -125,15 +125,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -45,9 +45,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/priority_option_id.html` & `pylero-0.1.0/docs/_modules/pylero/priority_option_id.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.priority_option_id &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -106,23 +106,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -132,15 +132,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -53,9 +53,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/product_license.html` & `pylero-0.1.0/docs/_modules/pylero/product_license.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.product_license &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -105,23 +105,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -131,15 +131,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -51,9 +51,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/project.html` & `pylero-0.1.0/docs/_modules/pylero/project.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.project &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -387,23 +387,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -413,15 +413,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -352,9 +352,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/project_group.html` & `pylero-0.1.0/docs/_modules/pylero/project_group.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.project_group &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -215,23 +215,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -241,15 +241,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -171,9 +171,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/properties.html` & `pylero-0.1.0/docs/_modules/pylero/properties.html`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.properties &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -82,23 +82,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -108,15 +108,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -28,9 +28,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/property.html` & `pylero-0.1.0/docs/_modules/pylero/property.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.property &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -84,23 +84,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -110,15 +110,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -30,9 +30,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/revision.html` & `pylero-0.1.0/docs/_modules/pylero/revision.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.revision &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -149,23 +149,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -175,15 +175,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -96,9 +96,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/server.html` & `pylero-0.1.0/docs/_modules/pylero/server.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.server &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -117,23 +117,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -143,15 +143,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -64,9 +64,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/session.html` & `pylero-0.1.0/docs/_modules/pylero/session.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.session &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -330,23 +330,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -356,15 +356,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -293,9 +293,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/signature.html` & `pylero-0.1.0/docs/_modules/pylero/signature.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.signature &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -98,23 +98,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -124,15 +124,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -45,9 +45,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/signature_context.html` & `pylero-0.1.0/docs/_modules/pylero/signature_context.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.signature_context &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -103,23 +103,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -129,15 +129,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -50,9 +50,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/signature_data.html` & `pylero-0.1.0/docs/_modules/pylero/signature_data.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.signature_data &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -83,23 +83,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -109,15 +109,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -29,9 +29,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/subterra_uri.html` & `pylero-0.1.0/docs/_modules/pylero/subterra_uri.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.subterra_uri &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -87,23 +87,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -113,15 +113,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -34,9 +34,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/test_record.html` & `pylero-0.1.0/docs/_modules/pylero/test_record.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.test_record &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -159,23 +159,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -185,15 +185,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -108,9 +108,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/test_run.html` & `pylero-0.1.0/docs/_modules/pylero/test_run.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.test_run &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -32,14 +32,15 @@
   <h1>Source code for pylero.test_run</h1><div class="highlight"><pre>
 <span></span><span class="c1"># -*- coding: utf8 -*-</span>
 <span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">absolute_import</span>
 <span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">division</span>
 <span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">print_function</span>
 <span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">unicode_literals</span>
 
+<span class="kn">import</span> <span class="nn">importlib</span>
 <span class="kn">import</span> <span class="nn">os</span>
 
 <span class="kn">import</span> <span class="nn">suds</span>
 <span class="kn">from</span> <span class="nn">pylero._compatible</span> <span class="kn">import</span> <span class="n">basestring</span>
 <span class="kn">from</span> <span class="nn">pylero._compatible</span> <span class="kn">import</span> <span class="nb">classmethod</span>
 <span class="kn">from</span> <span class="nn">pylero._compatible</span> <span class="kn">import</span> <span class="nb">object</span>  <span class="c1"># noqa</span>
 <span class="kn">from</span> <span class="nn">pylero._compatible</span> <span class="kn">import</span> <span class="nb">range</span>
@@ -60,151 +61,19 @@
 <span class="kn">from</span> <span class="nn">pylero.test_record</span> <span class="kn">import</span> <span class="n">TestRecord</span>
 <span class="kn">from</span> <span class="nn">pylero.test_run_attachment</span> <span class="kn">import</span> <span class="n">ArrayOfTestRunAttachment</span>
 <span class="kn">from</span> <span class="nn">pylero.test_run_attachment</span> <span class="kn">import</span> <span class="n">TestRunAttachment</span>
 <span class="kn">from</span> <span class="nn">pylero.text</span> <span class="kn">import</span> <span class="n">Text</span>
 <span class="kn">from</span> <span class="nn">pylero.user</span> <span class="kn">import</span> <span class="n">User</span>
 <span class="kn">from</span> <span class="nn">pylero.work_item</span> <span class="kn">import</span> <span class="n">_WorkItem</span>
 
-<span class="k">try</span><span class="p">:</span>
-    <span class="kn">from</span> <span class="nn">pylero.work_item</span> <span class="kn">import</span> <span class="n">TestCase</span>
-<span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-    <span class="k">pass</span>
 
 <span class="c1"># Build is used in custom fields.</span>
 <span class="c1"># Plan is used in custom fields.</span>
 
 
-<div class="viewcode-block" id="generate_description">
-<a class="viewcode-back" href="../../pylero.html#pylero.test_run.generate_description">[docs]</a>
-<span class="k">def</span> <span class="nf">generate_description</span><span class="p">(</span><span class="n">test_run</span><span class="p">,</span> <span class="n">test_case</span><span class="p">,</span> <span class="n">test_record</span><span class="p">):</span>
-    <span class="n">tr_html</span> <span class="o">=</span> <span class="p">(</span>
-        <span class="s1">&#39;&lt;b&gt;Test Run:&lt;/b&gt; &lt;span id=&quot;link&quot; class=    &#39;</span>
-        <span class="s1">&#39;&quot;polarion-rte-link&quot; data-type=&quot;testRun&quot; &#39;</span>
-        <span class="s1">&#39;data-item-id=&quot;</span><span class="si">{0}</span><span class="s1">&quot; data-option-id=&quot;long&quot;&gt;&#39;</span>
-        <span class="s2">&quot;&lt;/span&gt;&lt;br/&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_run</span><span class="o">.</span><span class="n">test_run_id</span><span class="p">)</span>
-    <span class="p">)</span>
-    <span class="n">tc_html</span> <span class="o">=</span> <span class="p">(</span>
-        <span class="s1">&#39;&lt;b&gt;Test Case:&lt;/b&gt; &lt;span id=&quot;link&quot; class=&#39;</span>
-        <span class="s1">&#39;&quot;polarion-rte-link&quot; data-type=&quot;workItem&quot; &#39;</span>
-        <span class="s1">&#39;data-item-id=&quot;</span><span class="si">{0}</span><span class="s1">&quot; data-option-id=&quot;long&quot;&gt;&lt;/span&gt;&#39;</span>
-        <span class="s2">&quot;&lt;br/&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_case</span><span class="o">.</span><span class="n">work_item_id</span><span class="p">)</span>
-    <span class="p">)</span>
-    <span class="n">table_cell_style</span> <span class="o">=</span> <span class="p">(</span>
-        <span class="s1">&#39;style=&quot;text-align: left; padding: 10px; &#39;</span>
-        <span class="s1">&#39;vertical-align: top; background-color: #ffffff;&quot;&#39;</span>
-    <span class="p">)</span>
-    <span class="n">table_row_style</span> <span class="o">=</span> <span class="s1">&#39;style=&quot;border-bottom: 1px solid #f0f0f0;&quot;&#39;</span>
-    <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span>
-        <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="s2">&quot;#&quot;</span><span class="p">,</span>
-        <span class="s1">&#39;&lt;span title=&quot;Step&quot;&gt;Step&lt;/span&gt;&#39;</span><span class="p">,</span>
-        <span class="s1">&#39;&lt;span title=&quot;Expected Result&quot;&gt;Expected Result&lt;/span&gt;&#39;</span><span class="p">,</span>
-        <span class="s2">&quot;Actual Result&quot;</span><span class="p">,</span>
-    <span class="p">]</span>
-    <span class="n">test_step_results</span> <span class="o">=</span> <span class="p">{</span>
-        <span class="s2">&quot;passed&quot;</span><span class="p">:</span> <span class="s1">&#39;&lt;span title=&quot;Results met expected results&#39;</span>
-        <span class="s1">&#39;&quot;&gt;&lt;span style=&quot;white-space:nowrap;&quot;&gt;&lt;im&#39;</span>
-        <span class="s1">&#39;g src=&quot;/polarion/icons/default/enums/test&#39;</span>
-        <span class="s1">&#39;run_status_passed.png&quot; style=&quot;vertical-a&#39;</span>
-        <span class="s2">&quot;lign:text-bottom;border:0px;margin-right:2&quot;</span>
-        <span class="s1">&#39;px;&quot; class=&quot;polarion-no-style-cleanup&quot;/&#39;</span>
-        <span class="s2">&quot;&gt;&lt;/span&gt;&lt;/span&gt;&quot;</span><span class="p">,</span>
-        <span class="s2">&quot;failed&quot;</span><span class="p">:</span> <span class="s1">&#39;&lt;span title=&quot;Results did not meet expecte&#39;</span>
-        <span class="s1">&#39;d results&quot;&gt;&lt;span style=&quot;white-space:nowr&#39;</span>
-        <span class="s1">&#39;ap;&quot;&gt;&lt;img src=&quot;/polarion/icons/default/e&#39;</span>
-        <span class="s1">&#39;nums/testrun_status_failed.png&quot; style=&quot;v&#39;</span>
-        <span class="s2">&quot;ertical-align:text-bottom;border:0px;margi&quot;</span>
-        <span class="s1">&#39;n-right:2px;&quot; class=&quot;polarion-no-style-c&#39;</span>
-        <span class="s1">&#39;leanup&quot;/&gt;&lt;/span&gt;&lt;/span&gt;&#39;</span><span class="p">,</span>
-        <span class="s2">&quot;blocked&quot;</span><span class="p">:</span> <span class="s1">&#39;&lt;span title=&quot;Errors in the product preve&#39;</span>
-        <span class="s1">&#39;nted test from being executed&quot;&gt;&lt;span sty&#39;</span>
-        <span class="s1">&#39;le=&quot;white-space:nowrap;&quot;&gt;&lt;img src=&quot;/po&#39;</span>
-        <span class="s2">&quot;larion/icons/default/enums/testrun_status&quot;</span>
-        <span class="s1">&#39;_blocked.png&quot; style=&quot;vertical-align:tex&#39;</span>
-        <span class="s1">&#39;t-bottom;border:0px;margin-right:2px;&quot; c&#39;</span>
-        <span class="s1">&#39;lass=&quot;polarion-no-style-cleanup&quot;/&gt;&#39;</span>
-        <span class="s2">&quot;&lt;/span&gt;&lt;/span&gt;&quot;</span><span class="p">,</span>
-    <span class="p">}</span>
-    <span class="n">table_header</span> <span class="o">=</span> <span class="p">(</span>
-        <span class="s1">&#39;&lt;table class=&quot;polarion-no-style-cleanup&quot; style=&quot;border&#39;</span>
-        <span class="s1">&#39;-collapse: collapse;&quot;&gt;&lt;tr style=&quot;text-align: left; &#39;</span>
-        <span class="s2">&quot;white-space: nowrap; color: #757575; border-bottom: 1px &quot;</span>
-        <span class="s1">&#39;solid #d2d7da; background-color: #ffffff;&quot;&gt;</span><span class="si">{0}</span><span class="s1">&lt;/tr&gt;&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span>
-            <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-                <span class="p">[</span>
-                    <span class="s2">&quot;&lt;th </span><span class="si">{0}</span><span class="s2">&gt;</span><span class="si">{1}</span><span class="s2">&lt;/th&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">table_cell_style</span><span class="p">,</span> <span class="n">column</span><span class="p">)</span>
-                    <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-                <span class="p">]</span>
-            <span class="p">)</span>
-        <span class="p">)</span>
-    <span class="p">)</span>
-    <span class="n">verdict</span> <span class="o">=</span> <span class="p">(</span>
-        <span class="s1">&#39;&lt;/table&gt;&lt;table style=&quot;margin-bottom: 15px; ;border-collapse: &#39;</span>
-        <span class="s1">&#39;collapse; width:100%; ;margin-top: 13px;&quot; class=&quot;polarion-no&#39;</span>
-        <span class="s1">&#39;-style-cleanup&quot;&gt;&lt;tr&gt;&lt;th style=&quot;width: 80%; text-align: left;&#39;</span>
-        <span class="s1">&#39; background-color: #ffffff;&quot;&gt;Test Case Verdict:&lt;/th&gt;&lt;/tr&gt;&lt;tr&gt;&#39;</span>
-        <span class="s1">&#39;&lt;td style=&quot;vertical-align: top;&quot;&gt;&lt;span style=&quot;font-weight: &#39;</span>
-        <span class="s1">&#39;bold;&quot;&gt;&lt;span style=&quot;color: #C30000;&quot;&gt;&lt;span title=&quot;Results &#39;</span>
-        <span class="s1">&#39;did not meet expected results&quot;&gt;&lt;span style=&quot;white-space:&#39;</span>
-        <span class="s1">&#39;nowrap;&quot;&gt;&lt;img src=&quot;/polarion/icons/default/enums/testrun_&#39;</span>
-        <span class="s1">&#39;status_failed.png&quot; style=&quot;vertical-align:text-bottom;border:&#39;</span>
-        <span class="s1">&#39;0px;margin-right:2px;&quot; class=&quot;polarion-no-style-cleanup&quot;/&gt;&#39;</span>
-        <span class="s2">&quot;&lt;/span&gt;Failed&lt;/span&gt;&lt;/span&gt;&lt;/span&gt;&lt;span&gt; </span><span class="si">{0}</span><span class="s2">&lt;/span&gt;&lt;/td&gt;&lt;/tr&gt;&quot;</span>
-        <span class="s2">&quot;&lt;/table&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_record</span><span class="o">.</span><span class="n">comment</span><span class="p">)</span>
-    <span class="p">)</span>
-    <span class="n">table_rows</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-    <span class="k">for</span> <span class="n">step</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">test_record</span><span class="o">.</span><span class="n">test_step_results</span><span class="p">)):</span>
-        <span class="n">table_rows</span> <span class="o">+=</span> <span class="p">(</span>
-            <span class="s2">&quot;&lt;tr </span><span class="si">{0}</span><span class="s2">&gt;&quot;</span>
-            <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{2}</span><span class="s2">&lt;/td&gt;&quot;</span>
-            <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{3}</span><span class="s2">&lt;/td&gt;&quot;</span>
-            <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{4}</span><span class="s2">&lt;/td&gt;&quot;</span>
-            <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{5}</span><span class="s2">&lt;/td&gt;&quot;</span>
-            <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{6}</span><span class="s2">&lt;/td&gt;&quot;</span>
-            <span class="s2">&quot;&lt;/tr&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span>
-                <span class="n">table_row_style</span><span class="p">,</span>
-                <span class="n">table_cell_style</span><span class="p">,</span>
-                <span class="n">test_step_results</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">test_record</span><span class="o">.</span><span class="n">test_step_results</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">result</span><span class="p">),</span>
-                <span class="n">step</span> <span class="o">+</span> <span class="mi">1</span><span class="p">,</span>
-                <span class="n">test_case</span><span class="o">.</span><span class="n">test_steps</span><span class="o">.</span><span class="n">steps</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">values</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">content</span><span class="p">,</span>
-                <span class="n">test_case</span><span class="o">.</span><span class="n">test_steps</span><span class="o">.</span><span class="n">steps</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">values</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">content</span><span class="p">,</span>
-                <span class="n">test_record</span><span class="o">.</span><span class="n">test_step_results</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">comment</span><span class="p">,</span>
-            <span class="p">)</span>
-        <span class="p">)</span>
-    <span class="n">content</span> <span class="o">=</span> <span class="n">tr_html</span> <span class="o">+</span> <span class="n">tc_html</span> <span class="o">+</span> <span class="n">table_header</span> <span class="o">+</span> <span class="n">table_rows</span> <span class="o">+</span> <span class="n">verdict</span>
-
-    <span class="k">return</span> <span class="n">content</span></div>
-
-
-
-<div class="viewcode-block" id="create_incident_report">
-<a class="viewcode-back" href="../../pylero.html#pylero.test_run.create_incident_report">[docs]</a>
-<span class="k">def</span> <span class="nf">create_incident_report</span><span class="p">(</span><span class="n">test_run</span><span class="p">,</span> <span class="n">test_record</span><span class="p">,</span> <span class="n">test_case</span><span class="p">):</span>
-    <span class="n">project_id</span> <span class="o">=</span> <span class="n">test_run</span><span class="o">.</span><span class="n">project_id</span>
-    <span class="n">status</span> <span class="o">=</span> <span class="s2">&quot;open&quot;</span>
-    <span class="n">project</span> <span class="o">=</span> <span class="n">Project</span><span class="p">(</span><span class="n">project_id</span><span class="p">)</span>
-    <span class="n">tconf</span> <span class="o">=</span> <span class="n">project</span><span class="o">.</span><span class="n">get_tests_configuration</span><span class="p">()</span>
-    <span class="n">defectWorkItemType</span> <span class="o">=</span> <span class="n">tconf</span><span class="o">.</span><span class="n">defect_work_item_type</span>
-    <span class="n">title</span> <span class="o">=</span> <span class="s2">&quot;Failed: &quot;</span> <span class="o">+</span> <span class="n">test_case</span><span class="o">.</span><span class="n">title</span>
-    <span class="n">description</span> <span class="o">=</span> <span class="n">generate_description</span><span class="p">(</span><span class="n">test_run</span><span class="p">,</span> <span class="n">test_case</span><span class="p">,</span> <span class="n">test_record</span><span class="p">)</span>
-    <span class="n">kwarg_dict</span> <span class="o">=</span> <span class="p">{}</span>
-
-    <span class="k">for</span> <span class="n">prop</span> <span class="ow">in</span> <span class="n">tconf</span><span class="o">.</span><span class="n">fields_to_copy_from_test_case_to_defect</span><span class="o">.</span><span class="n">property</span><span class="p">:</span>
-        <span class="n">kwarg_dict</span><span class="p">[</span><span class="n">prop</span><span class="o">.</span><span class="n">value</span><span class="p">]</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">test_case</span><span class="p">,</span> <span class="n">prop</span><span class="o">.</span><span class="n">key</span><span class="p">)</span>
-    <span class="k">for</span> <span class="n">prop</span> <span class="ow">in</span> <span class="n">tconf</span><span class="o">.</span><span class="n">fields_to_copy_from_test_run_to_linked_defect</span><span class="o">.</span><span class="n">property</span><span class="p">:</span>
-        <span class="n">kwarg_dict</span><span class="p">[</span><span class="n">prop</span><span class="o">.</span><span class="n">value</span><span class="p">]</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">test_run</span><span class="p">,</span> <span class="n">prop</span><span class="o">.</span><span class="n">key</span><span class="p">)</span>
-
-    <span class="n">incident_report</span> <span class="o">=</span> <span class="n">_WorkItem</span><span class="o">.</span><span class="n">create</span><span class="p">(</span>
-        <span class="n">project_id</span><span class="p">,</span> <span class="n">defectWorkItemType</span><span class="p">,</span> <span class="n">title</span><span class="p">,</span> <span class="n">description</span><span class="p">,</span> <span class="n">status</span><span class="p">,</span> <span class="o">**</span><span class="n">kwarg_dict</span>
-    <span class="p">)</span>
-    <span class="n">incident_report</span><span class="o">.</span><span class="n">add_linked_item</span><span class="p">(</span><span class="n">test_case</span><span class="o">.</span><span class="n">work_item_id</span><span class="p">,</span> <span class="s2">&quot;triggered_by&quot;</span><span class="p">)</span>
-    <span class="k">return</span> <span class="n">incident_report</span><span class="o">.</span><span class="n">work_item_id</span></div>
-
-
-
 <div class="viewcode-block" id="TestRun">
 <a class="viewcode-back" href="../../pylero.html#pylero.test_run.TestRun">[docs]</a>
 <span class="k">class</span> <span class="nc">TestRun</span><span class="p">(</span><span class="n">BasePolarion</span><span class="p">):</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Object to manage the Polarion Test Management WS tns3:TestRun</span>
 
 <span class="sd">    Attributes:</span>
 <span class="sd">        attachments (list of TestRunAttachments)</span>
@@ -418,15 +287,15 @@
         <span class="bp">cls</span><span class="p">,</span>
         <span class="n">project_id</span><span class="p">,</span>
         <span class="n">template_id</span><span class="p">,</span>
         <span class="n">parent_template_id</span><span class="o">=</span><span class="s2">&quot;Empty&quot;</span><span class="p">,</span>
         <span class="n">select_test_cases_by</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">query</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">doc_with_space</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-        <span class="o">**</span><span class="n">kwargs</span>
+        <span class="o">**</span><span class="n">kwargs</span><span class="p">,</span>
     <span class="p">):</span>  <span class="c1"># , test_case_ids=[]):</span>
         <span class="c1"># see comment below regarding test_case)ids.</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;class method create_template for creating a new template in Polarion</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            project_id (string): the Polarion project to create the test run</span>
 <span class="sd">                                 in</span>
@@ -658,17 +527,19 @@
         <span class="k">if</span> <span class="ow">not</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_custom_field_cache</span><span class="p">[</span><span class="n">project_id</span><span class="p">]:</span>
             <span class="n">cfts</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">session</span><span class="o">.</span><span class="n">test_management_client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">getDefinedTestRunCustomFieldTypes</span><span class="p">(</span>
                 <span class="n">project_id</span>
             <span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">cfts</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_custom_field_cache</span><span class="p">[</span><span class="n">project_id</span><span class="p">]</span>
         <span class="n">results</span> <span class="o">=</span> <span class="p">[</span>
-            <span class="n">CustomFieldType</span><span class="p">(</span><span class="n">suds_object</span><span class="o">=</span><span class="n">item</span><span class="p">)</span>
-            <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">item</span><span class="p">,</span> <span class="n">CustomFieldType</span><span class="p">()</span><span class="o">.</span><span class="n">_suds_object</span><span class="o">.</span><span class="vm">__class__</span><span class="p">)</span>
-            <span class="k">else</span> <span class="n">EnumCustomFieldType</span><span class="p">(</span><span class="n">suds_object</span><span class="o">=</span><span class="n">item</span><span class="p">)</span>
+            <span class="p">(</span>
+                <span class="n">CustomFieldType</span><span class="p">(</span><span class="n">suds_object</span><span class="o">=</span><span class="n">item</span><span class="p">)</span>
+                <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">item</span><span class="p">,</span> <span class="n">CustomFieldType</span><span class="p">()</span><span class="o">.</span><span class="n">_suds_object</span><span class="o">.</span><span class="vm">__class__</span><span class="p">)</span>
+                <span class="k">else</span> <span class="n">EnumCustomFieldType</span><span class="p">(</span><span class="n">suds_object</span><span class="o">=</span><span class="n">item</span><span class="p">)</span>
+            <span class="p">)</span>
             <span class="k">for</span> <span class="n">item</span> <span class="ow">in</span> <span class="n">cfts</span>
         <span class="p">]</span>
         <span class="k">return</span> <span class="n">results</span></div>
 
 
     <span class="k">def</span> <span class="nf">_cache_custom_fields</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">project_id</span><span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Polarion API provides the custom fields of a TestRun.</span>
@@ -761,14 +632,15 @@
                 <span class="k">return</span> <span class="n">index</span>
         <span class="k">raise</span> <span class="n">PyleroLibException</span><span class="p">(</span>
             <span class="s2">&quot;The Test Case is either not part of &quot;</span>
             <span class="s2">&quot;this TestRun or has not been executed&quot;</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">_status_change</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Change status if necessary and possible.&quot;&quot;&quot;</span>
         <span class="c1"># load a new object to test if the status should be changed.</span>
         <span class="c1"># can&#39;t use existing object because it doesn&#39;t include the new test rec</span>
         <span class="c1"># if the status needs changing, change it in the new object, so it</span>
         <span class="c1"># doesn&#39;t update any user made changes in the existing object.</span>
         <span class="n">check_tr</span> <span class="o">=</span> <span class="n">TestRun</span><span class="p">(</span><span class="n">uri</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">uri</span><span class="p">)</span>
         <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">rec</span><span class="o">.</span><span class="n">result</span> <span class="k">for</span> <span class="n">rec</span> <span class="ow">in</span> <span class="n">check_tr</span><span class="o">.</span><span class="n">records</span> <span class="k">if</span> <span class="n">rec</span><span class="o">.</span><span class="n">result</span><span class="p">]</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">results</span><span class="p">:</span>
@@ -778,15 +650,18 @@
             <span class="n">status</span> <span class="o">=</span> <span class="s2">&quot;finished&quot;</span>
             <span class="c1"># Do not touch finished_on because it can not be reverted</span>
             <span class="c1"># DPP-171495 Web services: You cannot reset finishedOn in TestRun</span>
             <span class="c1"># check_tr.finished_on = datetime.datetime.now()</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">status</span> <span class="o">=</span> <span class="s2">&quot;inprogress&quot;</span>
             <span class="n">check_tr</span><span class="o">.</span><span class="n">finished_on</span> <span class="o">=</span> <span class="kc">None</span>
-        <span class="k">if</span> <span class="n">status</span> <span class="o">!=</span> <span class="n">check_tr</span><span class="o">.</span><span class="n">status</span><span class="p">:</span>
+        <span class="c1"># Before setting the status, check if the new value is valid</span>
+        <span class="n">status_id</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_cls_suds_map</span><span class="p">[</span><span class="s2">&quot;status&quot;</span><span class="p">][</span><span class="s2">&quot;enum_id&quot;</span><span class="p">]</span>
+        <span class="n">valid_status_values</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_valid_field_values</span><span class="p">(</span><span class="n">status_id</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">status</span> <span class="o">!=</span> <span class="n">check_tr</span><span class="o">.</span><span class="n">status</span> <span class="ow">and</span> <span class="n">status</span> <span class="ow">in</span> <span class="n">valid_status_values</span><span class="p">:</span>
             <span class="n">check_tr</span><span class="o">.</span><span class="n">status</span> <span class="o">=</span> <span class="n">status</span>
             <span class="n">check_tr</span><span class="o">.</span><span class="n">update</span><span class="p">()</span>
 
     <span class="k">def</span> <span class="nf">_verify_record_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">record_index</span><span class="p">):</span>
         <span class="c1"># verifies the number of records is not less then the index given.</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_verify_obj</span><span class="p">()</span>
         <span class="k">if</span> <span class="n">record_index</span> <span class="o">&gt;</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">records</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">):</span>
@@ -933,17 +808,18 @@
         <span class="n">executed_by</span><span class="p">,</span>
         <span class="n">executed</span><span class="p">,</span>
         <span class="n">duration</span><span class="p">,</span>
         <span class="n">defect_work_item_id</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
     <span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;method add_test_record_by_fields, adds a test record for the given</span>
 <span class="sd">        test case based on the result fields passed in.</span>
-<span class="sd">        When a test record is added, it changes the test run status to</span>
+<span class="sd">        When a test record is added and the valid options for status contain</span>
+<span class="sd">        &quot;inprogress&quot; and &quot;finished&quot;, it changes the test run status to</span>
 <span class="sd">        &quot;inprogress&quot; and when the last test record is run, it changes the</span>
-<span class="sd">        status to done.</span>
+<span class="sd">        status to &quot;finished&quot;.</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            test_case_id (str): The id of the test case that was executed</span>
 <span class="sd">            test_result (str): Must be one of the following values:</span>
 <span class="sd">                                  passed</span>
 <span class="sd">                                  failed</span>
 <span class="sd">                                  blocked</span>
@@ -970,45 +846,248 @@
         <span class="n">testrec</span><span class="o">.</span><span class="n">executed</span> <span class="o">=</span> <span class="n">executed</span>
         <span class="n">testrec</span><span class="o">.</span><span class="n">duration</span> <span class="o">=</span> <span class="n">duration</span>
         <span class="k">if</span> <span class="n">defect_work_item_id</span><span class="p">:</span>
             <span class="n">testrec</span><span class="o">.</span><span class="n">defect_case_id</span> <span class="o">=</span> <span class="n">defect_work_item_id</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">add_test_record_by_object</span><span class="p">(</span><span class="n">testrec</span><span class="p">)</span></div>
 
 
+    <span class="k">def</span> <span class="nf">__generate_description</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span> <span class="n">test_case</span><span class="p">:</span> <span class="n">_WorkItem</span><span class="p">,</span> <span class="n">test_record</span><span class="p">:</span> <span class="n">TestRecord</span>
+    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Generates the description for the incident report.</span>
+
+<span class="sd">        If the test case has test steps that match the steps of the test record,</span>
+<span class="sd">        the description will include a table with the test steps and their results.</span>
+
+<span class="sd">        Args:</span>
+<span class="sd">            test_case (_WorkItem): Test case as a work item.</span>
+<span class="sd">            test_record (TestRecord): The test record contains the results of the</span>
+<span class="sd">                test execution.</span>
+
+<span class="sd">        Returns:</span>
+<span class="sd">            str: The incident report in HTML format.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+
+        <span class="n">tr_html</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="s1">&#39;&lt;b&gt;Test Run:&lt;/b&gt; &lt;span id=&quot;link&quot; class=    &#39;</span>
+            <span class="s1">&#39;&quot;polarion-rte-link&quot; data-type=&quot;testRun&quot; &#39;</span>
+            <span class="s1">&#39;data-item-id=&quot;</span><span class="si">{0}</span><span class="s1">&quot; data-option-id=&quot;long&quot;&gt;&#39;</span>
+            <span class="s2">&quot;&lt;/span&gt;&lt;br/&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">test_run_id</span><span class="p">)</span>
+        <span class="p">)</span>
+        <span class="n">tc_html</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="s1">&#39;&lt;b&gt;Test Case:&lt;/b&gt; &lt;span id=&quot;link&quot; class=&#39;</span>
+            <span class="s1">&#39;&quot;polarion-rte-link&quot; data-type=&quot;workItem&quot; &#39;</span>
+            <span class="s1">&#39;data-item-id=&quot;</span><span class="si">{0}</span><span class="s1">&quot; data-option-id=&quot;long&quot;&gt;&lt;/span&gt;&#39;</span>
+            <span class="s2">&quot;&lt;br/&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_case</span><span class="o">.</span><span class="n">work_item_id</span><span class="p">)</span>
+        <span class="p">)</span>
+        <span class="n">table_cell_style</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="s1">&#39;style=&quot;text-align: left; padding: 10px; &#39;</span>
+            <span class="s1">&#39;vertical-align: top; background-color: #ffffff;&quot;&#39;</span>
+        <span class="p">)</span>
+        <span class="n">table_row_style</span> <span class="o">=</span> <span class="s1">&#39;style=&quot;border-bottom: 1px solid #f0f0f0;&quot;&#39;</span>
+        <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span>
+            <span class="s2">&quot;&quot;</span><span class="p">,</span>
+            <span class="s2">&quot;#&quot;</span><span class="p">,</span>
+            <span class="s1">&#39;&lt;span title=&quot;Step&quot;&gt;Step&lt;/span&gt;&#39;</span><span class="p">,</span>
+            <span class="s1">&#39;&lt;span title=&quot;Expected Result&quot;&gt;Expected Result&lt;/span&gt;&#39;</span><span class="p">,</span>
+            <span class="s2">&quot;Actual Result&quot;</span><span class="p">,</span>
+        <span class="p">]</span>
+        <span class="n">test_step_results</span> <span class="o">=</span> <span class="p">{</span>
+            <span class="s2">&quot;passed&quot;</span><span class="p">:</span> <span class="s1">&#39;&lt;span title=&quot;Results met expected results&#39;</span>
+            <span class="s1">&#39;&quot;&gt;&lt;span style=&quot;white-space:nowrap;&quot;&gt;&lt;im&#39;</span>
+            <span class="s1">&#39;g src=&quot;/polarion/icons/default/enums/test&#39;</span>
+            <span class="s1">&#39;run_status_passed.png&quot; style=&quot;vertical-a&#39;</span>
+            <span class="s2">&quot;lign:text-bottom;border:0px;margin-right:2&quot;</span>
+            <span class="s1">&#39;px;&quot; class=&quot;polarion-no-style-cleanup&quot;/&#39;</span>
+            <span class="s2">&quot;&gt;&lt;/span&gt;&lt;/span&gt;&quot;</span><span class="p">,</span>
+            <span class="s2">&quot;failed&quot;</span><span class="p">:</span> <span class="s1">&#39;&lt;span title=&quot;Results did not meet expecte&#39;</span>
+            <span class="s1">&#39;d results&quot;&gt;&lt;span style=&quot;white-space:nowr&#39;</span>
+            <span class="s1">&#39;ap;&quot;&gt;&lt;img src=&quot;/polarion/icons/default/e&#39;</span>
+            <span class="s1">&#39;nums/testrun_status_failed.png&quot; style=&quot;v&#39;</span>
+            <span class="s2">&quot;ertical-align:text-bottom;border:0px;margi&quot;</span>
+            <span class="s1">&#39;n-right:2px;&quot; class=&quot;polarion-no-style-c&#39;</span>
+            <span class="s1">&#39;leanup&quot;/&gt;&lt;/span&gt;&lt;/span&gt;&#39;</span><span class="p">,</span>
+            <span class="s2">&quot;blocked&quot;</span><span class="p">:</span> <span class="s1">&#39;&lt;span title=&quot;Errors in the product preve&#39;</span>
+            <span class="s1">&#39;nted test from being executed&quot;&gt;&lt;span sty&#39;</span>
+            <span class="s1">&#39;le=&quot;white-space:nowrap;&quot;&gt;&lt;img src=&quot;/po&#39;</span>
+            <span class="s2">&quot;larion/icons/default/enums/testrun_status&quot;</span>
+            <span class="s1">&#39;_blocked.png&quot; style=&quot;vertical-align:tex&#39;</span>
+            <span class="s1">&#39;t-bottom;border:0px;margin-right:2px;&quot; c&#39;</span>
+            <span class="s1">&#39;lass=&quot;polarion-no-style-cleanup&quot;/&gt;&#39;</span>
+            <span class="s2">&quot;&lt;/span&gt;&lt;/span&gt;&quot;</span><span class="p">,</span>
+        <span class="p">}</span>
+        <span class="n">table_header</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="s1">&#39;&lt;table class=&quot;polarion-no-style-cleanup&quot; style=&quot;border&#39;</span>
+            <span class="s1">&#39;-collapse: collapse;&quot;&gt;&lt;tr style=&quot;text-align: left; &#39;</span>
+            <span class="s2">&quot;white-space: nowrap; color: #757575; border-bottom: 1px &quot;</span>
+            <span class="s1">&#39;solid #d2d7da; background-color: #ffffff;&quot;&gt;</span><span class="si">{0}</span><span class="s1">&lt;/tr&gt;&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span>
+                <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+                    <span class="p">[</span>
+                        <span class="s2">&quot;&lt;th </span><span class="si">{0}</span><span class="s2">&gt;</span><span class="si">{1}</span><span class="s2">&lt;/th&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">table_cell_style</span><span class="p">,</span> <span class="n">column</span><span class="p">)</span>
+                        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+                    <span class="p">]</span>
+                <span class="p">)</span>
+            <span class="p">)</span>
+        <span class="p">)</span>
+        <span class="n">verdict</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="s1">&#39;&lt;/table&gt;&lt;table style=&quot;margin-bottom: 15px; ;border-collapse: &#39;</span>
+            <span class="s1">&#39;collapse; width:100%; ;margin-top: 13px;&quot; class=&quot;polarion-no&#39;</span>
+            <span class="s1">&#39;-style-cleanup&quot;&gt;&lt;tr&gt;&lt;th style=&quot;width: 80%; text-align: left;&#39;</span>
+            <span class="s1">&#39; background-color: #ffffff;&quot;&gt;Test Case Verdict:&lt;/th&gt;&lt;/tr&gt;&lt;tr&gt;&#39;</span>
+            <span class="s1">&#39;&lt;td style=&quot;vertical-align: top;&quot;&gt;&lt;span style=&quot;font-weight: &#39;</span>
+            <span class="s1">&#39;bold;&quot;&gt;&lt;span style=&quot;color: #C30000;&quot;&gt;&lt;span title=&quot;Results &#39;</span>
+            <span class="s1">&#39;did not meet expected results&quot;&gt;&lt;span style=&quot;white-space:&#39;</span>
+            <span class="s1">&#39;nowrap;&quot;&gt;&lt;img src=&quot;/polarion/icons/default/enums/testrun_&#39;</span>
+            <span class="s1">&#39;status_failed.png&quot; style=&quot;vertical-align:text-bottom;border:&#39;</span>
+            <span class="s1">&#39;0px;margin-right:2px;&quot; class=&quot;polarion-no-style-cleanup&quot;/&gt;&#39;</span>
+            <span class="s2">&quot;&lt;/span&gt;Failed&lt;/span&gt;&lt;/span&gt;&lt;/span&gt;&lt;span&gt; </span><span class="si">{0}</span><span class="s2">&lt;/span&gt;&lt;/td&gt;&lt;/tr&gt;&quot;</span>
+            <span class="s2">&quot;&lt;/table&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">test_record</span><span class="o">.</span><span class="n">comment</span><span class="p">)</span>
+        <span class="p">)</span>
+        <span class="k">try</span><span class="p">:</span>
+            <span class="n">table_rows</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+            <span class="n">test_steps</span> <span class="o">=</span> <span class="n">test_case</span><span class="o">.</span><span class="n">get_test_steps</span><span class="p">()</span>
+            <span class="k">for</span> <span class="n">step</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">test_record</span><span class="o">.</span><span class="n">test_step_results</span><span class="p">)):</span>
+                <span class="n">table_rows</span> <span class="o">+=</span> <span class="p">(</span>
+                    <span class="s2">&quot;&lt;tr </span><span class="si">{0}</span><span class="s2">&gt;&quot;</span>
+                    <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{2}</span><span class="s2">&lt;/td&gt;&quot;</span>
+                    <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{3}</span><span class="s2">&lt;/td&gt;&quot;</span>
+                    <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{4}</span><span class="s2">&lt;/td&gt;&quot;</span>
+                    <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{5}</span><span class="s2">&lt;/td&gt;&quot;</span>
+                    <span class="s2">&quot;&lt;td </span><span class="si">{1}</span><span class="s2">&gt;</span><span class="si">{6}</span><span class="s2">&lt;/td&gt;&quot;</span>
+                    <span class="s2">&quot;&lt;/tr&gt;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span>
+                        <span class="n">table_row_style</span><span class="p">,</span>
+                        <span class="n">table_cell_style</span><span class="p">,</span>
+                        <span class="n">test_step_results</span><span class="o">.</span><span class="n">get</span><span class="p">(</span>
+                            <span class="n">test_record</span><span class="o">.</span><span class="n">test_step_results</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">result</span>
+                        <span class="p">),</span>
+                        <span class="n">step</span> <span class="o">+</span> <span class="mi">1</span><span class="p">,</span>
+                        <span class="n">test_steps</span><span class="o">.</span><span class="n">steps</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">values</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">content</span><span class="p">,</span>
+                        <span class="n">test_steps</span><span class="o">.</span><span class="n">steps</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">values</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">content</span><span class="p">,</span>
+                        <span class="n">test_record</span><span class="o">.</span><span class="n">test_step_results</span><span class="p">[</span><span class="n">step</span><span class="p">]</span><span class="o">.</span><span class="n">comment</span><span class="p">,</span>
+                    <span class="p">)</span>
+                <span class="p">)</span>
+        <span class="k">except</span> <span class="p">(</span><span class="n">suds</span><span class="o">.</span><span class="n">WebFault</span><span class="p">,</span> <span class="ne">AttributeError</span><span class="p">):</span>
+            <span class="c1"># test_case.get_test_steps() can raise a webfault</span>
+            <span class="c1"># test_record.test_step_results cab raise an attribute error</span>
+            <span class="c1"># other errors should be passed up the call stack</span>
+            <span class="n">table_rows</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+        <span class="k">if</span> <span class="n">table_rows</span><span class="p">:</span>
+            <span class="n">table</span> <span class="o">=</span> <span class="n">table_header</span> <span class="o">+</span> <span class="n">table_rows</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="n">table</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+        <span class="n">content</span> <span class="o">=</span> <span class="n">tr_html</span> <span class="o">+</span> <span class="n">tc_html</span> <span class="o">+</span> <span class="n">table</span> <span class="o">+</span> <span class="n">verdict</span>
+        <span class="k">return</span> <span class="n">content</span>
+
+    <span class="k">def</span> <span class="nf">__create_incident_report</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span> <span class="n">test_case_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">test_record</span><span class="p">:</span> <span class="n">TestRecord</span>
+    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Create and populate an incident work item.</span>
+
+<span class="sd">        The work_item type of the incident and the fields to copy from the test</span>
+<span class="sd">        case and test run to the incident are defined in the tests configuration</span>
+<span class="sd">        of the project.</span>
+<span class="sd">        Throws an exception if the test case does not exists or if the incident</span>
+<span class="sd">        could not be created.</span>
+
+<span class="sd">        Args:</span>
+<span class="sd">            test_case_id (str): The ID of the test case.</span>
+<span class="sd">            test_record (TestRecord): The test record contains the results of the</span>
+<span class="sd">                test execution.</span>
+<span class="sd">                executed.</span>
+
+<span class="sd">        Returns:</span>
+<span class="sd">            str: work_item_id of the created incident.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="n">project_id</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">project_id</span>
+        <span class="n">status</span> <span class="o">=</span> <span class="s2">&quot;open&quot;</span>
+        <span class="n">project</span> <span class="o">=</span> <span class="n">Project</span><span class="p">(</span><span class="n">project_id</span><span class="p">)</span>
+        <span class="n">tconf</span> <span class="o">=</span> <span class="n">project</span><span class="o">.</span><span class="n">get_tests_configuration</span><span class="p">()</span>
+        <span class="n">defect_wi_type</span> <span class="o">=</span> <span class="n">tconf</span><span class="o">.</span><span class="n">defect_work_item_type</span>
+        <span class="n">test_case_wi_type</span> <span class="o">=</span> <span class="n">tconf</span><span class="o">.</span><span class="n">test_case_work_item_type</span>
+
+        <span class="k">try</span><span class="p">:</span>
+            <span class="n">work_item_module</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">import_module</span><span class="p">(</span><span class="s2">&quot;pylero.work_item&quot;</span><span class="p">)</span>
+            <span class="n">wi_class_names</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">work_item_module</span><span class="p">,</span> <span class="s2">&quot;workitems&quot;</span><span class="p">)</span>
+            <span class="n">test_case_class_name</span> <span class="o">=</span> <span class="n">wi_class_names</span><span class="p">[</span><span class="n">test_case_wi_type</span><span class="p">]</span>
+            <span class="n">test_case_class</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">work_item_module</span><span class="p">,</span> <span class="n">test_case_class_name</span><span class="p">)</span>
+            <span class="n">test_case</span> <span class="o">=</span> <span class="n">test_case_class</span><span class="p">(</span>
+                <span class="n">project_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">project_id</span><span class="p">,</span> <span class="n">work_item_id</span><span class="o">=</span><span class="n">test_case_id</span>
+            <span class="p">)</span>
+        <span class="k">except</span> <span class="p">(</span><span class="ne">AttributeError</span><span class="p">,</span> <span class="n">PyleroLibException</span><span class="p">):</span>
+            <span class="n">test_case</span> <span class="o">=</span> <span class="n">_WorkItem</span><span class="p">(</span><span class="n">project_id</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">project_id</span><span class="p">,</span> <span class="n">work_item_id</span><span class="o">=</span><span class="n">test_case_id</span><span class="p">)</span>
+
+        <span class="n">title</span> <span class="o">=</span> <span class="s2">&quot;Failed: &quot;</span> <span class="o">+</span> <span class="n">test_case</span><span class="o">.</span><span class="n">title</span>
+        <span class="n">description</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">__generate_description</span><span class="p">(</span><span class="n">test_case</span><span class="p">,</span> <span class="n">test_record</span><span class="p">)</span>
+        <span class="n">kwarg_dict</span> <span class="o">=</span> <span class="p">{}</span>
+        <span class="k">for</span> <span class="n">prop</span> <span class="ow">in</span> <span class="n">tconf</span><span class="o">.</span><span class="n">fields_to_copy_from_test_case_to_defect</span><span class="o">.</span><span class="n">property</span><span class="p">:</span>
+            <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">test_case</span><span class="p">,</span> <span class="n">prop</span><span class="o">.</span><span class="n">key</span><span class="p">):</span>
+                <span class="n">kwarg_dict</span><span class="p">[</span><span class="n">prop</span><span class="o">.</span><span class="n">value</span><span class="p">]</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">test_case</span><span class="p">,</span> <span class="n">prop</span><span class="o">.</span><span class="n">key</span><span class="p">)</span>
+        <span class="k">for</span> <span class="n">prop</span> <span class="ow">in</span> <span class="n">tconf</span><span class="o">.</span><span class="n">fields_to_copy_from_test_run_to_linked_defect</span><span class="o">.</span><span class="n">property</span><span class="p">:</span>
+            <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">prop</span><span class="o">.</span><span class="n">key</span><span class="p">):</span>
+                <span class="n">kwarg_dict</span><span class="p">[</span><span class="n">prop</span><span class="o">.</span><span class="n">value</span><span class="p">]</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">prop</span><span class="o">.</span><span class="n">key</span><span class="p">)</span>
+
+        <span class="k">try</span><span class="p">:</span>
+            <span class="n">incident_report</span> <span class="o">=</span> <span class="n">_WorkItem</span><span class="o">.</span><span class="n">create</span><span class="p">(</span>
+                <span class="n">project_id</span><span class="p">,</span> <span class="n">defect_wi_type</span><span class="p">,</span> <span class="n">title</span><span class="p">,</span> <span class="n">description</span><span class="p">,</span> <span class="n">status</span><span class="p">,</span> <span class="o">**</span><span class="n">kwarg_dict</span>
+            <span class="p">)</span>
+        <span class="k">except</span> <span class="n">PyleroLibException</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+            <span class="n">msg</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+                <span class="p">[</span>
+                    <span class="p">(</span>
+                        <span class="sa">f</span><span class="s2">&quot;Failed to create the work item </span><span class="si">{</span><span class="n">title</span><span class="si">}</span><span class="s2"> in&quot;</span>
+                        <span class="sa">f</span><span class="s2">&quot;project </span><span class="si">{</span><span class="n">project_id</span><span class="si">}</span><span class="s2"> of type </span><span class="si">{</span><span class="n">defect_wi_type</span><span class="si">}</span><span class="s2">.&quot;</span>
+                    <span class="p">),</span>
+                    <span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+                <span class="p">]</span>
+            <span class="p">)</span>
+            <span class="k">raise</span> <span class="n">PyleroLibException</span><span class="p">(</span><span class="n">msg</span><span class="p">)</span>
+        <span class="n">incident_report</span><span class="o">.</span><span class="n">add_linked_item</span><span class="p">(</span><span class="n">test_case</span><span class="o">.</span><span class="n">work_item_id</span><span class="p">,</span> <span class="s2">&quot;triggered_by&quot;</span><span class="p">)</span>
+        <span class="k">return</span> <span class="n">incident_report</span><span class="o">.</span><span class="n">work_item_id</span>
+
 <div class="viewcode-block" id="TestRun.add_test_record_by_object">
 <a class="viewcode-back" href="../../pylero.html#pylero.test_run.TestRun.add_test_record_by_object">[docs]</a>
     <span class="nd">@tx_wrapper</span>
-    <span class="k">def</span> <span class="nf">add_test_record_by_object</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">test_record</span><span class="p">,</span> <span class="n">manual_state_change</span><span class="o">=</span><span class="kc">False</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">add_test_record_by_object</span><span class="p">(</span>
+        <span class="bp">self</span><span class="p">,</span> <span class="n">test_record</span><span class="p">,</span> <span class="n">manual_state_change</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">create_incident</span><span class="o">=</span><span class="kc">True</span>
+    <span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;method add_test_record_by_object, adds a test record for the given</span>
 <span class="sd">        test case based on the TestRecord object passed in.</span>
 <span class="sd">        In addition, the test run is checked for completeness and the test</span>
 <span class="sd">        run state will change accordingly.</span>
-<span class="sd">        Test Run states are [&quot;notrun&quot;, &quot;finished&quot;, &quot;inprogress&quot;].</span>
+<span class="sd">        If possible, the status is set to one of</span>
+<span class="sd">        [&quot;notrun&quot;, &quot;finished&quot;, &quot;inprogress&quot;].</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            test_record (TestRecord or Polarion TestRecord):</span>
 <span class="sd">            manual_state_change (boolean): Change test run state</span>
 <span class="sd">                                           automatically or manual.</span>
+<span class="sd">            create_incident (boolean): Create an incident report if the test</span>
+<span class="sd">                                        case fails and no incident is linked.</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            None</span>
 
 <span class="sd">        References:</span>
 <span class="sd">            test_management.addTestRecordToTestRun</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_verify_obj</span><span class="p">()</span>
         <span class="n">test_case_id</span> <span class="o">=</span> <span class="n">test_record</span><span class="o">.</span><span class="n">test_case_id</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_check_test_record_exists</span><span class="p">(</span><span class="n">test_case_id</span><span class="p">)</span>
         <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">test_record</span><span class="p">,</span> <span class="n">TestRecord</span><span class="p">):</span>
             <span class="n">suds_object</span> <span class="o">=</span> <span class="n">test_record</span><span class="o">.</span><span class="n">_suds_object</span>
         <span class="k">elif</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">test_record</span><span class="p">,</span> <span class="n">TestRecord</span><span class="p">()</span><span class="o">.</span><span class="n">_suds_object</span><span class="o">.</span><span class="vm">__class__</span><span class="p">):</span>
             <span class="n">suds_object</span> <span class="o">=</span> <span class="n">test_record</span>
-        <span class="k">if</span> <span class="n">test_record</span><span class="o">.</span><span class="n">result</span> <span class="o">==</span> <span class="s2">&quot;failed&quot;</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span><span class="p">:</span>
-            <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span> <span class="o">=</span> <span class="n">create_incident_report</span><span class="p">(</span>
-                <span class="bp">self</span><span class="p">,</span> <span class="n">test_record</span><span class="p">,</span> <span class="n">TestCase</span><span class="p">(</span><span class="n">work_item_id</span><span class="o">=</span><span class="n">test_case_id</span><span class="p">)</span>
+        <span class="k">if</span> <span class="p">(</span>
+            <span class="n">test_record</span><span class="o">.</span><span class="n">result</span> <span class="o">==</span> <span class="s2">&quot;failed&quot;</span>
+            <span class="ow">and</span> <span class="ow">not</span> <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span>
+            <span class="ow">and</span> <span class="n">create_incident</span>
+        <span class="p">):</span>
+            <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">__create_incident_report</span><span class="p">(</span>
+                <span class="n">test_case_id</span><span class="p">,</span>
+                <span class="n">test_record</span><span class="p">,</span>
             <span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">session</span><span class="o">.</span><span class="n">test_management_client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">addTestRecordToTestRun</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">uri</span><span class="p">,</span> <span class="n">suds_object</span>
         <span class="p">)</span>
 
         <span class="k">if</span> <span class="n">manual_state_change</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">()</span>
@@ -1384,27 +1463,35 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">update_test_record_by_object</span><span class="p">(</span><span class="n">test_case_id</span><span class="p">,</span> <span class="n">testrec</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="TestRun.update_test_record_by_object">
 <a class="viewcode-back" href="../../pylero.html#pylero.test_run.TestRun.update_test_record_by_object">[docs]</a>
     <span class="nd">@tx_wrapper</span>
     <span class="k">def</span> <span class="nf">update_test_record_by_object</span><span class="p">(</span>
-        <span class="bp">self</span><span class="p">,</span> <span class="n">test_case_id</span><span class="p">,</span> <span class="n">test_record</span><span class="p">,</span> <span class="n">manual_state_change</span><span class="o">=</span><span class="kc">False</span>
+        <span class="bp">self</span><span class="p">,</span>
+        <span class="n">test_case_id</span><span class="p">,</span>
+        <span class="n">test_record</span><span class="p">,</span>
+        <span class="n">manual_state_change</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
+        <span class="n">create_incident</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
     <span class="p">):</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;method update_test_record_by_object, adds a test record for the</span>
 <span class="sd">        given test case based on the TestRecord object passed in.</span>
 <span class="sd">        In addition, the test run is checked for completeness and the</span>
 <span class="sd">        test run state will change accordingly.</span>
-<span class="sd">        Test Run states are [&quot;notrun&quot;, &quot;finished&quot;, &quot;inprogress&quot;].</span>
+<span class="sd">        If possible, the status is set to one of</span>
+<span class="sd">        [&quot;notrun&quot;, &quot;finished&quot;, &quot;inprogress&quot;].</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            test_case_id (str): the test case id that the record is related to.</span>
 <span class="sd">            test_record (TestRecord or Polarion TestRecord)</span>
 <span class="sd">            manual_state_change (boolean): Change the test</span>
 <span class="sd">                                           run result automatically or manual.</span>
+<span class="sd">            create_incident (boolean): Create an incident report if the test</span>
+<span class="sd">                                        record result is failed and no defect</span>
+<span class="sd">                                        case id is set.</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            None</span>
 
 <span class="sd">        References:</span>
 <span class="sd">            test_management.updateTestRecordAtIndex</span>
 <span class="sd">        &quot;&quot;&quot;</span>
@@ -1413,17 +1500,21 @@
         <span class="c1"># because this function (specifically and not documented) uses the</span>
         <span class="c1"># actual index of the test records and not the index of all</span>
         <span class="c1"># executed records.</span>
         <span class="n">test_case_ids</span> <span class="o">=</span> <span class="p">[</span><span class="n">rec</span><span class="o">.</span><span class="n">test_case_id</span> <span class="k">for</span> <span class="n">rec</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_records</span><span class="p">]</span>
         <span class="k">if</span> <span class="n">test_case_id</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">test_case_ids</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">add_test_record_by_object</span><span class="p">(</span><span class="n">test_record</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
-            <span class="k">if</span> <span class="n">test_record</span><span class="o">.</span><span class="n">result</span> <span class="o">==</span> <span class="s2">&quot;failed&quot;</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span><span class="p">:</span>
-                <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span> <span class="o">=</span> <span class="n">create_incident_report</span><span class="p">(</span>
-                    <span class="bp">self</span><span class="p">,</span> <span class="n">test_record</span><span class="p">,</span> <span class="n">TestCase</span><span class="p">(</span><span class="n">work_item_id</span><span class="o">=</span><span class="n">test_case_id</span><span class="p">)</span>
+            <span class="k">if</span> <span class="p">(</span>
+                <span class="n">test_record</span><span class="o">.</span><span class="n">result</span> <span class="o">==</span> <span class="s2">&quot;failed&quot;</span>
+                <span class="ow">and</span> <span class="ow">not</span> <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span>
+                <span class="ow">and</span> <span class="n">create_incident</span>
+            <span class="p">):</span>
+                <span class="n">test_record</span><span class="o">.</span><span class="n">defect_case_id</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">__create_incident_report</span><span class="p">(</span>
+                    <span class="n">test_case_id</span><span class="p">,</span> <span class="n">test_record</span>
                 <span class="p">)</span>
             <span class="n">index</span> <span class="o">=</span> <span class="n">test_case_ids</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">test_case_id</span><span class="p">)</span>
             <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">test_record</span><span class="p">,</span> <span class="n">TestRecord</span><span class="p">):</span>
                 <span class="n">suds_object</span> <span class="o">=</span> <span class="n">test_record</span><span class="o">.</span><span class="n">_suds_object</span>
             <span class="k">elif</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">test_record</span><span class="p">,</span> <span class="n">TestRecord</span><span class="p">()</span><span class="o">.</span><span class="n">_suds_object</span><span class="o">.</span><span class="vm">__class__</span><span class="p">):</span>
                 <span class="n">suds_object</span> <span class="o">=</span> <span class="n">test_record</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">session</span><span class="o">.</span><span class="n">test_management_client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">updateTestRecordAtIndex</span><span class="p">(</span>
@@ -1531,23 +1622,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -1557,15 +1648,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 ************ SSoouurrccee ccooddee ffoorr ppyylleerroo..tteesstt__rruunn ************
 # -*- coding: utf8 -*-
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
+import importlib
 import os
 
 import suds
 from pylero._compatible import basestring
 from pylero._compatible import classmethod
 from pylero._compatible import object  # noqa
 from pylero._compatible import range
@@ -29,157 +30,21 @@
 from pylero.test_record import TestRecord
 from pylero.test_run_attachment import ArrayOfTestRunAttachment
 from pylero.test_run_attachment import TestRunAttachment
 from pylero.text import Text
 from pylero.user import User
 from pylero.work_item import _WorkItem
 
-try:
-    from pylero.work_item import TestCase
-except ImportError:
-    pass
 
 # Build is used in custom fields.
 # Plan is used in custom fields.
 
 
 
 _[_d_o_c_s_]
-def generate_description(test_run, test_case, test_record):
-    tr_html = (
-        '<b>Test Run:</b> <span id="link" class=    '
-        '"polarion-rte-link" data-type="testRun" '
-        'data-item-id="{0}" data-option-id="long">'
-        "</span><br/>".format(test_run.test_run_id)
-    )
-    tc_html = (
-        '<b>Test Case:</b> <span id="link" class='
-        '"polarion-rte-link" data-type="workItem" '
-        'data-item-id="{0}" data-option-id="long"></span>'
-        "<br/>".format(test_case.work_item_id)
-    )
-    table_cell_style = (
-        'style="text-align: left; padding: 10px; '
-        'vertical-align: top; background-color: #ffffff;"'
-    )
-    table_row_style = 'style="border-bottom: 1px solid #f0f0f0;"'
-    columns = [
-        "",
-        "#",
-        '<span title="Step">Step</span>',
-        '<span title="Expected Result">Expected Result</span>',
-        "Actual Result",
-    ]
-    test_step_results = {
-        "passed": '<span title="Results met expected results'
-        '"><span style="white-space:nowrap;"><im'
-        'g src="/polarion/icons/default/enums/test'
-        'run_status_passed.png" style="vertical-a'
-        "lign:text-bottom;border:0px;margin-right:2"
-        'px;" class="polarion-no-style-cleanup"/'
-        "></span></span>",
-        "failed": '<span title="Results did not meet expecte'
-        'd results"><span style="white-space:nowr'
-        'ap;"><img src="/polarion/icons/default/e'
-        'nums/testrun_status_failed.png" style="v'
-        "ertical-align:text-bottom;border:0px;margi"
-        'n-right:2px;" class="polarion-no-style-c'
-        'leanup"/></span></span>',
-        "blocked": '<span title="Errors in the product preve'
-        'nted test from being executed"><span sty'
-        'le="white-space:nowrap;"><img src="/po'
-        "larion/icons/default/enums/testrun_status"
-        '_blocked.png" style="vertical-align:tex'
-        't-bottom;border:0px;margin-right:2px;" c'
-        'lass="polarion-no-style-cleanup"/>'
-        "</span></span>",
-    }
-    table_header = (
-        '<table class="polarion-no-style-cleanup" style="border'
-        '-collapse: collapse;"><tr style="text-align: left; '
-        "white-space: nowrap; color: #757575; border-bottom: 1px "
-        'solid #d2d7da; background-color: #ffffff;">{0}</tr>'.format(
-            "".join(
-                [
-                    "<th {0}>{1}</th>".format(table_cell_style, column)
-                    for column in columns
-                ]
-            )
-        )
-    )
-    verdict = (
-        '</table><table style="margin-bottom: 15px; ;border-collapse: '
-        'collapse; width:100%; ;margin-top: 13px;" class="polarion-no'
-        '-style-cleanup"><tr><th style="width: 80%; text-align: left;'
-        ' background-color: #ffffff;">Test Case Verdict:</th></tr><tr>'
-        '<td style="vertical-align: top;"><span style="font-weight: '
-        'bold;"><span style="color: #C30000;"><span title="Results '
-        'did not meet expected results"><span style="white-space:'
-        'nowrap;"><img src="/polarion/icons/default/enums/testrun_'
-        'status_failed.png" style="vertical-align:text-bottom;border:'
-        '0px;margin-right:2px;" class="polarion-no-style-cleanup"/>'
-        "</span>Failed</span></span></span><span> {0}</span></td></tr>"
-        "</table>".format(test_record.comment)
-    )
-    table_rows = ""
-    for step in range(len(test_record.test_step_results)):
-        table_rows += (
-            "<tr {0}>"
-            "<td {1}>{2}</td>"
-            "<td {1}>{3}</td>"
-            "<td {1}>{4}</td>"
-            "<td {1}>{5}</td>"
-            "<td {1}>{6}</td>"
-            "</tr>".format(
-                table_row_style,
-                table_cell_style,
-                test_step_results.get(test_record.test_step_results
-[step].result),
-                step + 1,
-                test_case.test_steps.steps[step].values[0].content,
-                test_case.test_steps.steps[step].values[1].content,
-                test_record.test_step_results[step].comment,
-            )
-        )
-    content = tr_html + tc_html + table_header + table_rows + verdict
-
-    return content
-
-
-
-
-
-_[_d_o_c_s_]
-def create_incident_report(test_run, test_record, test_case):
-    project_id = test_run.project_id
-    status = "open"
-    project = Project(project_id)
-    tconf = project.get_tests_configuration()
-    defectWorkItemType = tconf.defect_work_item_type
-    title = "Failed: " + test_case.title
-    description = generate_description(test_run, test_case, test_record)
-    kwarg_dict = {}
-
-    for prop in tconf.fields_to_copy_from_test_case_to_defect.property:
-        kwarg_dict[prop.value] = getattr(test_case, prop.key)
-    for prop in tconf.fields_to_copy_from_test_run_to_linked_defect.property:
-        kwarg_dict[prop.value] = getattr(test_run, prop.key)
-
-    incident_report = _WorkItem.create(
-        project_id, defectWorkItemType, title, description, status,
-**kwarg_dict
-    )
-    incident_report.add_linked_item(test_case.work_item_id, "triggered_by")
-    return incident_report.work_item_id
-
-
-
-
-
-_[_d_o_c_s_]
 class TestRun(BasePolarion):
     """Object to manage the Polarion Test Management WS tns3:TestRun
 
     Attributes:
         attachments (list of TestRunAttachments)
         author (User): user object of the Test Run Author
         created (datetime)
@@ -397,15 +262,15 @@
         cls,
         project_id,
         template_id,
         parent_template_id="Empty",
         select_test_cases_by=None,
         query=None,
         doc_with_space=None,
-        **kwargs
+        **kwargs,
     ):  # , test_case_ids=[]):
         # see comment below regarding test_case)ids.
         """class method create_template for creating a new template in Polarion
 
         Args:
             project_id (string): the Polarion project to create the test run
                                  in
@@ -648,17 +513,19 @@
             cfts =
 cls.session.test_management_client.service.getDefinedTestRunCustomFieldTypes(
                 project_id
             )
         else:
             cfts = cls._custom_field_cache[project_id]
         results = [
-            CustomFieldType(suds_object=item)
-            if isinstance(item, CustomFieldType()._suds_object.__class__)
-            else EnumCustomFieldType(suds_object=item)
+            (
+                CustomFieldType(suds_object=item)
+                if isinstance(item, CustomFieldType()._suds_object.__class__)
+                else EnumCustomFieldType(suds_object=item)
+            )
             for item in cfts
         ]
         return results
 
 
 
     def _cache_custom_fields(self, project_id):
@@ -752,14 +619,15 @@
                 return index
         raise PyleroLibException(
             "The Test Case is either not part of "
             "this TestRun or has not been executed"
         )
 
     def _status_change(self):
+        """Change status if necessary and possible."""
         # load a new object to test if the status should be changed.
         # can't use existing object because it doesn't include the new test rec
         # if the status needs changing, change it in the new object, so it
         # doesn't update any user made changes in the existing object.
         check_tr = TestRun(uri=self.uri)
         results = [rec.result for rec in check_tr.records if rec.result]
         if not results:
@@ -769,15 +637,18 @@
             status = "finished"
             # Do not touch finished_on because it can not be reverted
             # DPP-171495 Web services: You cannot reset finishedOn in TestRun
             # check_tr.finished_on = datetime.datetime.now()
         else:
             status = "inprogress"
             check_tr.finished_on = None
-        if status != check_tr.status:
+        # Before setting the status, check if the new value is valid
+        status_id = self._cls_suds_map["status"]["enum_id"]
+        valid_status_values = self.get_valid_field_values(status_id, None)
+        if status != check_tr.status and status in valid_status_values:
             check_tr.status = status
             check_tr.update()
 
     def _verify_record_count(self, record_index):
         # verifies the number of records is not less then the index given.
         self._verify_obj()
         if record_index > (len(self.records) - 1):
@@ -930,17 +801,18 @@
         executed_by,
         executed,
         duration,
         defect_work_item_id=None,
     ):
         """method add_test_record_by_fields, adds a test record for the given
         test case based on the result fields passed in.
-        When a test record is added, it changes the test run status to
+        When a test record is added and the valid options for status contain
+        "inprogress" and "finished", it changes the test run status to
         "inprogress" and when the last test record is run, it changes the
-        status to done.
+        status to "finished".
 
         Args:
             test_case_id (str): The id of the test case that was executed
             test_result (str): Must be one of the following values:
                                   passed
                                   failed
                                   blocked
@@ -968,46 +840,256 @@
         testrec.duration = duration
         if defect_work_item_id:
             testrec.defect_case_id = defect_work_item_id
         self.add_test_record_by_object(testrec)
 
 
 
+    def __generate_description(
+        self, test_case: _WorkItem, test_record: TestRecord
+    ) -> str:
+        """Generates the description for the incident report.
+
+        If the test case has test steps that match the steps of the test
+record,
+        the description will include a table with the test steps and their
+results.
+
+        Args:
+            test_case (_WorkItem): Test case as a work item.
+            test_record (TestRecord): The test record contains the results of
+the
+                test execution.
+
+        Returns:
+            str: The incident report in HTML format.
+        """
+
+        tr_html = (
+            '<b>Test Run:</b> <span id="link" class=    '
+            '"polarion-rte-link" data-type="testRun" '
+            'data-item-id="{0}" data-option-id="long">'
+            "</span><br/>".format(self.test_run_id)
+        )
+        tc_html = (
+            '<b>Test Case:</b> <span id="link" class='
+            '"polarion-rte-link" data-type="workItem" '
+            'data-item-id="{0}" data-option-id="long"></span>'
+            "<br/>".format(test_case.work_item_id)
+        )
+        table_cell_style = (
+            'style="text-align: left; padding: 10px; '
+            'vertical-align: top; background-color: #ffffff;"'
+        )
+        table_row_style = 'style="border-bottom: 1px solid #f0f0f0;"'
+        columns = [
+            "",
+            "#",
+            '<span title="Step">Step</span>',
+            '<span title="Expected Result">Expected Result</span>',
+            "Actual Result",
+        ]
+        test_step_results = {
+            "passed": '<span title="Results met expected results'
+            '"><span style="white-space:nowrap;"><im'
+            'g src="/polarion/icons/default/enums/test'
+            'run_status_passed.png" style="vertical-a'
+            "lign:text-bottom;border:0px;margin-right:2"
+            'px;" class="polarion-no-style-cleanup"/'
+            "></span></span>",
+            "failed": '<span title="Results did not meet expecte'
+            'd results"><span style="white-space:nowr'
+            'ap;"><img src="/polarion/icons/default/e'
+            'nums/testrun_status_failed.png" style="v'
+            "ertical-align:text-bottom;border:0px;margi"
+            'n-right:2px;" class="polarion-no-style-c'
+            'leanup"/></span></span>',
+            "blocked": '<span title="Errors in the product preve'
+            'nted test from being executed"><span sty'
+            'le="white-space:nowrap;"><img src="/po'
+            "larion/icons/default/enums/testrun_status"
+            '_blocked.png" style="vertical-align:tex'
+            't-bottom;border:0px;margin-right:2px;" c'
+            'lass="polarion-no-style-cleanup"/>'
+            "</span></span>",
+        }
+        table_header = (
+            '<table class="polarion-no-style-cleanup" style="border'
+            '-collapse: collapse;"><tr style="text-align: left; '
+            "white-space: nowrap; color: #757575; border-bottom: 1px "
+            'solid #d2d7da; background-color: #ffffff;">{0}</tr>'.format(
+                "".join(
+                    [
+                        "<th {0}>{1}</th>".format(table_cell_style, column)
+                        for column in columns
+                    ]
+                )
+            )
+        )
+        verdict = (
+            '</table><table style="margin-bottom: 15px; ;border-collapse: '
+            'collapse; width:100%; ;margin-top: 13px;" class="polarion-no'
+            '-style-cleanup"><tr><th style="width: 80%; text-align: left;'
+            ' background-color: #ffffff;">Test Case Verdict:</th></tr><tr>'
+            '<td style="vertical-align: top;"><span style="font-weight: '
+            'bold;"><span style="color: #C30000;"><span title="Results '
+            'did not meet expected results"><span style="white-space:'
+            'nowrap;"><img src="/polarion/icons/default/enums/testrun_'
+            'status_failed.png" style="vertical-align:text-bottom;border:'
+            '0px;margin-right:2px;" class="polarion-no-style-cleanup"/>'
+            "</span>Failed</span></span></span><span> {0}</span></td></tr>"
+            "</table>".format(test_record.comment)
+        )
+        try:
+            table_rows = ""
+            test_steps = test_case.get_test_steps()
+            for step in range(len(test_record.test_step_results)):
+                table_rows += (
+                    "<tr {0}>"
+                    "<td {1}>{2}</td>"
+                    "<td {1}>{3}</td>"
+                    "<td {1}>{4}</td>"
+                    "<td {1}>{5}</td>"
+                    "<td {1}>{6}</td>"
+                    "</tr>".format(
+                        table_row_style,
+                        table_cell_style,
+                        test_step_results.get(
+                            test_record.test_step_results[step].result
+                        ),
+                        step + 1,
+                        test_steps.steps[step].values[0].content,
+                        test_steps.steps[step].values[1].content,
+                        test_record.test_step_results[step].comment,
+                    )
+                )
+        except (suds.WebFault, AttributeError):
+            # test_case.get_test_steps() can raise a webfault
+            # test_record.test_step_results cab raise an attribute error
+            # other errors should be passed up the call stack
+            table_rows = ""
+        if table_rows:
+            table = table_header + table_rows
+        else:
+            table = ""
+        content = tr_html + tc_html + table + verdict
+        return content
+
+    def __create_incident_report(
+        self, test_case_id: str, test_record: TestRecord
+    ) -> str:
+        """Create and populate an incident work item.
+
+        The work_item type of the incident and the fields to copy from the test
+        case and test run to the incident are defined in the tests
+configuration
+        of the project.
+        Throws an exception if the test case does not exists or if the incident
+        could not be created.
+
+        Args:
+            test_case_id (str): The ID of the test case.
+            test_record (TestRecord): The test record contains the results of
+the
+                test execution.
+                executed.
+
+        Returns:
+            str: work_item_id of the created incident.
+        """
+        project_id = self.project_id
+        status = "open"
+        project = Project(project_id)
+        tconf = project.get_tests_configuration()
+        defect_wi_type = tconf.defect_work_item_type
+        test_case_wi_type = tconf.test_case_work_item_type
+
+        try:
+            work_item_module = importlib.import_module("pylero.work_item")
+            wi_class_names = getattr(work_item_module, "workitems")
+            test_case_class_name = wi_class_names[test_case_wi_type]
+            test_case_class = getattr(work_item_module, test_case_class_name)
+            test_case = test_case_class(
+                project_id=self.project_id, work_item_id=test_case_id
+            )
+        except (AttributeError, PyleroLibException):
+            test_case = _WorkItem(project_id=self.project_id,
+work_item_id=test_case_id)
+
+        title = "Failed: " + test_case.title
+        description = self.__generate_description(test_case, test_record)
+        kwarg_dict = {}
+        for prop in tconf.fields_to_copy_from_test_case_to_defect.property:
+            if hasattr(test_case, prop.key):
+                kwarg_dict[prop.value] = getattr(test_case, prop.key)
+        for prop in
+tconf.fields_to_copy_from_test_run_to_linked_defect.property:
+            if hasattr(self, prop.key):
+                kwarg_dict[prop.value] = getattr(self, prop.key)
+
+        try:
+            incident_report = _WorkItem.create(
+                project_id, defect_wi_type, title, description, status,
+**kwarg_dict
+            )
+        except PyleroLibException as e:
+            msg = "\n".join(
+                [
+                    (
+                        f"Failed to create the work item {title} in"
+                        f"project {project_id} of type {defect_wi_type}."
+                    ),
+                    f"Error: {e}",
+                ]
+            )
+            raise PyleroLibException(msg)
+        incident_report.add_linked_item(test_case.work_item_id, "triggered_by")
+        return incident_report.work_item_id
+
 
 _[_d_o_c_s_]
     @tx_wrapper
-    def add_test_record_by_object(self, test_record,
-manual_state_change=False):
+    def add_test_record_by_object(
+        self, test_record, manual_state_change=False, create_incident=True
+    ):
         """method add_test_record_by_object, adds a test record for the given
         test case based on the TestRecord object passed in.
         In addition, the test run is checked for completeness and the test
         run state will change accordingly.
-        Test Run states are ["notrun", "finished", "inprogress"].
+        If possible, the status is set to one of
+        ["notrun", "finished", "inprogress"].
 
         Args:
             test_record (TestRecord or Polarion TestRecord):
             manual_state_change (boolean): Change test run state
                                            automatically or manual.
+            create_incident (boolean): Create an incident report if the test
+                                        case fails and no incident is linked.
 
         Returns:
             None
 
         References:
             test_management.addTestRecordToTestRun
         """
         self._verify_obj()
         test_case_id = test_record.test_case_id
         self._check_test_record_exists(test_case_id)
         if isinstance(test_record, TestRecord):
             suds_object = test_record._suds_object
         elif isinstance(test_record, TestRecord()._suds_object.__class__):
             suds_object = test_record
-        if test_record.result == "failed" and not test_record.defect_case_id:
-            test_record.defect_case_id = create_incident_report(
-                self, test_record, TestCase(work_item_id=test_case_id)
+        if (
+            test_record.result == "failed"
+            and not test_record.defect_case_id
+            and create_incident
+        ):
+            test_record.defect_case_id = self.__create_incident_report(
+                test_case_id,
+                test_record,
             )
         self.session.test_management_client.service.addTestRecordToTestRun(
             self.uri, suds_object
         )
 
         if manual_state_change:
             self.update()
@@ -1406,27 +1488,35 @@
 
 
 
 
 _[_d_o_c_s_]
     @tx_wrapper
     def update_test_record_by_object(
-        self, test_case_id, test_record, manual_state_change=False
+        self,
+        test_case_id,
+        test_record,
+        manual_state_change=False,
+        create_incident=True,
     ):
         """method update_test_record_by_object, adds a test record for the
         given test case based on the TestRecord object passed in.
         In addition, the test run is checked for completeness and the
         test run state will change accordingly.
-        Test Run states are ["notrun", "finished", "inprogress"].
+        If possible, the status is set to one of
+        ["notrun", "finished", "inprogress"].
 
         Args:
             test_case_id (str): the test case id that the record is related to.
             test_record (TestRecord or Polarion TestRecord)
             manual_state_change (boolean): Change the test
                                            run result automatically or manual.
+            create_incident (boolean): Create an incident report if the test
+                                        record result is failed and no defect
+                                        case id is set.
 
         Returns:
             None
 
         References:
             test_management.updateTestRecordAtIndex
         """
@@ -1435,18 +1525,21 @@
         # because this function (specifically and not documented) uses the
         # actual index of the test records and not the index of all
         # executed records.
         test_case_ids = [rec.test_case_id for rec in self._records]
         if test_case_id not in test_case_ids:
             self.add_test_record_by_object(test_record)
         else:
-            if test_record.result == "failed" and not
-test_record.defect_case_id:
-                test_record.defect_case_id = create_incident_report(
-                    self, test_record, TestCase(work_item_id=test_case_id)
+            if (
+                test_record.result == "failed"
+                and not test_record.defect_case_id
+                and create_incident
+            ):
+                test_record.defect_case_id = self.__create_incident_report(
+                    test_case_id, test_record
                 )
             index = test_case_ids.index(test_case_id)
             if isinstance(test_record, TestRecord):
                 suds_object = test_record._suds_object
             elif isinstance(test_record, TestRecord()._suds_object.__class__):
                 suds_object = test_record
             self.session.test_management_client.service.updateTestRecordAtIndex
@@ -1537,9 +1630,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/test_run_attachment.html` & `pylero-0.1.0/docs/_modules/pylero/test_run_attachment.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.test_run_attachment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -105,23 +105,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -131,15 +131,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -52,9 +52,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/test_step.html` & `pylero-0.1.0/docs/_modules/pylero/test_step.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.test_step &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -96,23 +96,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -122,15 +122,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -43,9 +43,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/test_step_result.html` & `pylero-0.1.0/docs/_modules/pylero/test_step_result.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.test_step_result &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -108,23 +108,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -134,15 +134,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -55,9 +55,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/test_steps.html` & `pylero-0.1.0/docs/_modules/pylero/test_steps.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.test_steps &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -101,23 +101,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -127,15 +127,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -47,9 +47,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/tests_configuration.html` & `pylero-0.1.0/docs/_modules/pylero/tests_configuration.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.tests_configuration &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -140,23 +140,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -166,15 +166,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -86,9 +86,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/text.html` & `pylero-0.1.0/docs/_modules/pylero/text.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.text &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -111,23 +111,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -137,15 +137,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -59,9 +59,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/time_point.html` & `pylero-0.1.0/docs/_modules/pylero/time_point.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.time_point &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -93,23 +93,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -119,15 +119,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -39,9 +39,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/user.html` & `pylero-0.1.0/docs/_modules/pylero/user.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.user &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -320,23 +320,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -346,15 +346,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -280,9 +280,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/wiki_page.html` & `pylero-0.1.0/docs/_modules/pylero/wiki_page.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.wiki_page &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -257,23 +257,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -283,15 +283,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -206,9 +206,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/wiki_page_attachment.html` & `pylero-0.1.0/docs/_modules/pylero/wiki_page_attachment.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.wiki_page_attachment &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -103,23 +103,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -129,15 +129,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -50,9 +50,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/work_record.html` & `pylero-0.1.0/docs/_modules/pylero/work_record.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.work_record &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -106,23 +106,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -132,15 +132,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -53,9 +53,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_modules/pylero/workflow_action.html` & `pylero-0.1.0/docs/_modules/pylero/workflow_action.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>pylero.workflow_action &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css?v=12dfc556" />
     <script src="../../_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="../../_static/doctools.js?v=888ff710"></script>
+    <script src="../../_static/doctools.js?v=9a2dae69"></script>
     <script src="../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
     <link rel="search" title="Search" href="../../search.html" />
    
   <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
   
 
@@ -97,23 +97,23 @@
 <ul>
   <li><a href="../../index.html">Documentation overview</a><ul>
   <li><a href="../index.html">Module code</a><ul>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../../search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -123,15 +123,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -43,9 +43,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _M_o_d_u_l_e_ _c_o_d_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/_sources/index.rst.txt` & `pylero-0.1.0/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/docs/_sources/pylero.rst.txt` & `pylero-0.1.0/docs/_sources/pylero.rst.txt`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/docs/_static/alabaster.css` & `pylero-0.1.0/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/docs/_static/basic.css` & `pylero-0.1.0/docs/_static/basic.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
```

### Comparing `pylero-0.0.9/docs/_static/doctools.js` & `pylero-0.1.0/docs/_static/doctools.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * doctools.js
  * ~~~~~~~~~~~
  *
  * Base JavaScript utilities for all Sphinx HTML documentation.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 const BLACKLISTED_KEY_CONTROL_ELEMENTS = new Set([
     "TEXTAREA",
```

### Comparing `pylero-0.0.9/docs/_static/language_data.js` & `pylero-0.1.0/docs/_static/language_data.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
 
 
-/* Non-minified version is copied as a separate JS file, is available */
+/* Non-minified version is copied as a separate JS file, if available */
 
 /**
  * Porter Stemmer
  */
 var Stemmer = function() {
 
     var step2list = {
```

### Comparing `pylero-0.0.9/docs/_static/pygments.css` & `pylero-0.1.0/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/docs/_static/searchtools.js` & `pylero-0.1.0/docs/_static/searchtools.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -94,15 +94,15 @@
             highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
     } else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms)
+                    Search.makeSearchSummary(data, searchTerms, anchor)
                 );
             // highlight search terms in the summary
             if (SPHINX_HIGHLIGHT_ENABLED) // set in sphinx_highlight.js
                 highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
         });
     Search.output.appendChild(listItem);
 };
@@ -111,16 +111,16 @@
     Search.title.innerText = _("Search Results");
     if (!resultCount)
         Search.status.innerText = Documentation.gettext(
             "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
         );
     else
         Search.status.innerText = _(
-            `Search finished, found ${resultCount} page(s) matching the search query.`
-        );
+            "Search finished, found ${resultCount} page(s) matching the search query."
+        ).replace('${resultCount}', resultCount);
 };
 const _displayNextItem = (
     results,
     resultCount,
     searchTerms,
     highlightTerms,
 ) => {
@@ -132,14 +132,30 @@
             () => _displayNextItem(results, resultCount, searchTerms, highlightTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
+// Helper function used by query() to order search results.
+// Each input is an array of [docname, title, anchor, descr, score, filename].
+// Order the results by score (in opposite order of appearance, since the
+// `_displayNextItem` function uses pop() to retrieve items) and then alphabetically.
+const _orderResultsByScoreThenName = (a, b) => {
+    const leftScore = a[4];
+    const rightScore = b[4];
+    if (leftScore === rightScore) {
+        // same score: sort alphabetically
+        const leftTitle = a[1].toLowerCase();
+        const rightTitle = b[1].toLowerCase();
+        if (leftTitle === rightTitle) return 0;
+        return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
+    }
+    return leftScore > rightScore ? 1 : -1;
+};
 
 /**
  * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
  * custom function per language.
  *
  * The regular expression works by splitting the string on consecutive characters
  * that are not Unicode letters, numbers, underscores, or emoji characters.
@@ -155,23 +171,36 @@
  * Search Module
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: (htmlString) => {
+    htmlToText: (htmlString, anchor) => {
         const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
-        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
-            el.remove()
-        });
+        for (const removalQuery of [".headerlinks", "script", "style"]) {
+            htmlElement.querySelectorAll(removalQuery).forEach((el) => {
+                el.remove()
+            });
+        }
+        if (anchor) {
+            const anchorContent = htmlElement.querySelector(`[role="main"] ${anchor}`);
+            if (anchorContent) return anchorContent.textContent;
+
+            console.warn(
+                `Anchored content block not found. Sphinx search tries to obtain it via DOM query '[role=main] ${anchor}'. Check your theme or template.`
+            );
+        }
+
+        // if anchor not specified or not found, fall back to main content
         const docContent = htmlElement.querySelector('[role="main"]');
-        if (docContent !== undefined) return docContent.textContent;
+        if (docContent) return docContent.textContent;
+
         console.warn(
-            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+            "Content block not found. Sphinx search tries to obtain it via DOM query '[role=main]'. Check your theme or template."
         );
         return "";
     },
 
     init: () => {
         const query = new URLSearchParams(window.location.search).get("q");
         document
@@ -236,24 +265,15 @@
         Search.startPulse();
 
         // index already loaded, the browser was quick!
         if (Search.hasIndex()) Search.query(query);
         else Search.deferQuery(query);
     },
 
-    /**
-     * execute search (requires search index to be loaded)
-     */
-    query: (query) => {
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const titles = Search._index.titles;
-        const allTitles = Search._index.alltitles;
-        const indexEntries = Search._index.indexentries;
-
+    _parseQuery: (query) => {
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -281,92 +301,114 @@
             localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
         }
 
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
-        // array of [docname, title, anchor, descr, score, filename]
-        let results = [];
+        return [query, searchTerms, excludedTerms, highlightTerms, objectTerms];
+    },
+
+    /**
+     * execute search (requires search index to be loaded)
+     */
+    _performSearch: (query, searchTerms, excludedTerms, highlightTerms, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // Collect multiple result groups to be sorted separately and then ordered.
+        // Each is an array of [docname, title, anchor, descr, score, filename].
+        const normalResults = [];
+        const nonMainIndexResults = [];
+
         _removeChildren(document.getElementById("search-progress"));
 
-        const queryLower = query.toLowerCase();
+        const queryLower = query.toLowerCase().trim();
         for (const [title, foundTitles] of Object.entries(allTitles)) {
-            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+            if (title.toLowerCase().trim().includes(queryLower) && (queryLower.length >= title.length / 2)) {
                 for (const [file, id] of foundTitles) {
                     let score = Math.round(100 * queryLower.length / title.length)
-                    results.push([
+                    normalResults.push([
                         docNames[file],
                         titles[file] !== title ? `${titles[file]} > ${title}` : title,
                         id !== null ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
                     ]);
                 }
             }
         }
 
         // search for explicit entries in index directives
         for (const [entry, foundEntries] of Object.entries(indexEntries)) {
             if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
-                for (const [file, id] of foundEntries) {
-                    let score = Math.round(100 * queryLower.length / entry.length)
-                    results.push([
+                for (const [file, id, isMain] of foundEntries) {
+                    const score = Math.round(100 * queryLower.length / entry.length);
+                    const result = [
                         docNames[file],
                         titles[file],
                         id ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
-                    ]);
+                    ];
+                    if (isMain) {
+                        normalResults.push(result);
+                    } else {
+                        nonMainIndexResults.push(result);
+                    }
                 }
             }
         }
 
         // lookup as object
         objectTerms.forEach((term) =>
-            results.push(...Search.performObjectSearch(term, objectTerms))
+            normalResults.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
-        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
+        normalResults.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
+        if (Scorer.score) {
+            normalResults.forEach((item) => (item[4] = Scorer.score(item)));
+            nonMainIndexResults.forEach((item) => (item[4] = Scorer.score(item)));
+        }
 
-        // now sort the results by score (in opposite order of appearance, since the
-        // display function below uses pop() to retrieve items) and then
-        // alphabetically
-        results.sort((a, b) => {
-            const leftScore = a[4];
-            const rightScore = b[4];
-            if (leftScore === rightScore) {
-                // same score: sort alphabetically
-                const leftTitle = a[1].toLowerCase();
-                const rightTitle = b[1].toLowerCase();
-                if (leftTitle === rightTitle) return 0;
-                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
-            }
-            return leftScore > rightScore ? 1 : -1;
-        });
+        // Sort each group of results by score and then alphabetically by name.
+        normalResults.sort(_orderResultsByScoreThenName);
+        nonMainIndexResults.sort(_orderResultsByScoreThenName);
+
+        // Combine the result groups in (reverse) order.
+        // Non-main index entries are typically arbitrary cross-references,
+        // so display them after other results.
+        let results = [...nonMainIndexResults, ...normalResults];
 
         // remove duplicate search results
         // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
         let seen = new Set();
         results = results.reverse().reduce((acc, result) => {
             let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
             if (!seen.has(resultStr)) {
                 acc.push(result);
                 seen.add(resultStr);
             }
             return acc;
         }, []);
 
-        results = results.reverse();
+        return results.reverse();
+    },
+
+    query: (query) => {
+        const [searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms] = Search._parseQuery(query);
+        const results = Search._performSearch(searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms);
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
         _displayNextItem(results, results.length, searchTerms, highlightTerms);
@@ -466,28 +508,32 @@
             }, {
                 files: titleTerms[word],
                 score: Scorer.title
             }, ];
             // add support for partial matches
             if (word.length > 2) {
                 const escapedWord = _escapeRegExp(word);
-                Object.keys(terms).forEach((term) => {
-                    if (term.match(escapedWord) && !terms[word])
-                        arr.push({
-                            files: terms[term],
-                            score: Scorer.partialTerm
-                        });
-                });
-                Object.keys(titleTerms).forEach((term) => {
-                    if (term.match(escapedWord) && !titleTerms[word])
-                        arr.push({
-                            files: titleTerms[word],
-                            score: Scorer.partialTitle
-                        });
-                });
+                if (!terms.hasOwnProperty(word)) {
+                    Object.keys(terms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: terms[term],
+                                score: Scorer.partialTerm
+                            });
+                    });
+                }
+                if (!titleTerms.hasOwnProperty(word)) {
+                    Object.keys(titleTerms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: titleTerms[term],
+                                score: Scorer.partialTitle
+                            });
+                    });
+                }
             }
 
             // no match but word was a required one
             if (arr.every((record) => record.files === undefined)) return;
 
             // found search word in contents
             arr.forEach((record) => {
@@ -502,17 +548,16 @@
                     if (!scoreMap.has(file)) scoreMap.set(file, {});
                     scoreMap.get(file)[word] = record.score;
                 });
             });
 
             // create the mapping
             files.forEach((file) => {
-                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
-                    fileMap.get(file).push(word);
-                else fileMap.set(file, [word]);
+                if (!fileMap.has(file)) fileMap.set(file, [word]);
+                else if (fileMap.get(file).indexOf(word) === -1) fileMap.get(file).push(word);
             });
         });
 
         // now check if the files don't contain excluded terms
         const results = [];
         for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
@@ -555,16 +600,16 @@
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
      * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords) => {
-        const text = Search.htmlToText(htmlText);
+    makeSearchSummary: (htmlText, keywords, anchor) => {
+        const text = Search.htmlToText(htmlText, anchor);
         if (text === "") return null;
 
         const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
             .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
```

### Comparing `pylero-0.0.9/docs/genindex.html` & `pylero-0.1.0/docs/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Index &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
 
@@ -413,16 +413,14 @@
         <li><a href="pylero.html#pylero.document.Document.create">(pylero.document.Document class method)</a>
 </li>
         <li><a href="pylero.html#pylero.plan.Plan.create">(pylero.plan.Plan class method)</a>
 </li>
         <li><a href="pylero.html#pylero.test_run.TestRun.create">(pylero.test_run.TestRun class method)</a>
 </li>
       </ul></li>
-      <li><a href="pylero.html#pylero.test_run.create_incident_report">create_incident_report() (in module pylero.test_run)</a>
-</li>
       <li><a href="pylero.html#pylero.plan.Plan.create_plan_template">create_plan_template() (pylero.plan.Plan class method)</a>
 </li>
       <li><a href="pylero.html#pylero.session.create_ssl_context">create_ssl_context() (in module pylero.session)</a>
 </li>
       <li><a href="pylero.html#pylero.test_run.TestRun.create_summary_defect">create_summary_defect() (pylero.test_run.TestRun method)</a>
 </li>
       <li><a href="pylero.html#pylero.test_run.TestRun.create_template">create_template() (pylero.test_run.TestRun class method)</a>
@@ -667,16 +665,14 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="pylero.html#pylero.test_run.generate_description">generate_description() (in module pylero.test_run)</a>
-</li>
       <li><a href="pylero.html#pylero.product_license.ProductLicense.generated_by">generated_by (pylero.product_license.ProductLicense attribute)</a>
 </li>
       <li><a href="pylero.html#pylero.test_run.TestRun.get_attachment">get_attachment() (pylero.test_run.TestRun method)</a>
 </li>
       <li><a href="pylero.html#pylero.test_run.TestRun.get_attachments">get_attachments() (pylero.test_run.TestRun method)</a>
 </li>
       <li><a href="pylero.html#pylero.project.Project.get_categories">get_categories() (pylero.project.Project method)</a>
@@ -709,17 +705,23 @@
 </li>
       <li><a href="pylero.html#pylero.document.Document.get_documents">get_documents() (pylero.document.Document class method)</a>
 </li>
       <li><a href="pylero.html#pylero.base_polarion.BasePolarion.get_global_roles">get_global_roles() (pylero.base_polarion.BasePolarion class method)</a>
 </li>
       <li><a href="pylero.html#pylero.base_polarion.BasePolarion.get_location">get_location() (pylero.base_polarion.BasePolarion method)</a>
 </li>
+      <li><a href="pylero.html#pylero.project.Project.get_project_users">get_project_users() (pylero.project.Project method)</a>
+</li>
+      <li><a href="pylero.html#pylero.base_polarion.BasePolarion.get_revision">get_revision() (pylero.base_polarion.BasePolarion method)</a>
+</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="pylero.html#pylero.project.Project.get_project_users">get_project_users() (pylero.project.Project method)</a>
+      <li><a href="pylero.html#pylero.base_polarion.BasePolarion.get_revision_by_uri">get_revision_by_uri() (pylero.base_polarion.BasePolarion method)</a>
+</li>
+      <li><a href="pylero.html#pylero.base_polarion.BasePolarion.get_revisions">get_revisions() (pylero.base_polarion.BasePolarion method)</a>
 </li>
       <li><a href="pylero.html#pylero.user.User.get_roles">get_roles() (pylero.user.User method)</a>
 </li>
       <li><a href="pylero.html#pylero.project_group.ProjectGroup.get_root_project_group">get_root_project_group() (pylero.project_group.ProjectGroup class method)</a>
 </li>
       <li><a href="pylero.html#pylero.plan.Plan.get_statistics">get_statistics() (pylero.plan.Plan method)</a>
 </li>
@@ -2301,23 +2303,23 @@
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -2327,15 +2329,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -122,50 +122,50 @@
       _(_p_y_l_e_r_o_._b_u_i_l_d_._B_u_i_l_d_ _a_t_t_r_i_b_u_t_e_)                     * _c_o_n_t_e_n_t___l_o_s_s_y_ _(_p_y_l_e_r_o_._t_e_x_t_._T_e_x_t_ _a_t_t_r_i_b_u_t_e_)
     * _c_a_l_c_u_l_a_t_i_o_n___t_y_p_e_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)      * _c_o_n_t_e_n_t___t_y_p_e_ _(_p_y_l_e_r_o_._t_e_x_t_._T_e_x_t_ _a_t_t_r_i_b_u_t_e_)
     * _c_a_n___a_d_d___e_l_e_m_e_n_t___t_o___k_e_y_(_)_                           * _c_o_n_t_e_x_t___i_d_ _(_p_y_l_e_r_o_._a_c_t_i_v_i_t_y_._A_c_t_i_v_i_t_y_ _a_t_t_r_i_b_u_t_e_)
       _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e_(_)_ _(_p_y_l_e_r_o_._b_a_s_e_l_i_n_e_._B_a_s_e_l_i_n_e_ _c_l_a_s_s_ _m_e_t_h_o_d_)
     * _c_a_n___d_e_l_e_t_e___i_n_s_t_a_n_c_e_(_)_                                    o _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _c_l_a_s_s_ _m_e_t_h_o_d_)
       _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)               o _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
     * _c_a_n___m_o_d_i_f_y___i_n_s_t_a_n_c_e_(_)_                                    o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___i_n_c_i_d_e_n_t___r_e_p_o_r_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _p_y_l_e_r_o_._t_e_s_t___r_u_n_)
-    * _c_a_n___m_o_d_i_f_y___k_e_y_(_)_                                   * _c_r_e_a_t_e___p_l_a_n___t_e_m_p_l_a_t_e_(_)_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___s_s_l___c_o_n_t_e_x_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _p_y_l_e_r_o_._s_e_s_s_i_o_n_)
-    * _c_a_n___r_e_a_d___i_n_s_t_a_n_c_e_(_)_                                * _c_r_e_a_t_e___s_u_m_m_a_r_y___d_e_f_e_c_t_(_)_ _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___t_e_m_p_l_a_t_e_(_)_ _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
-    * _c_a_n___r_e_a_d___k_e_y_(_)_                                     * _c_r_e_a_t_e___u_s_e_r_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _c_l_a_s_s_ _m_e_t_h_o_d_)
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___w_o_r_k___i_t_e_m_(_)_ _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _m_e_t_h_o_d_)
-    * _c_a_n___r_e_m_o_v_e___e_l_e_m_e_n_t___f_r_o_m___k_e_y_(_)_                      * _c_r_e_a_t_e_d_ _(_p_y_l_e_r_o_._c_o_m_m_e_n_t_._C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)               o _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
-    * _c_a_p_a_c_i_t_y_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)                    o _(_p_y_l_e_r_o_._i_m_p_o_r_t_e_d___c_o_m_m_e_n_t_._I_m_p_o_r_t_e_d_C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
-    * _C_a_t_e_g_o_r_y_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_a_t_e_g_o_r_y_)                      o _(_p_y_l_e_r_o_._m_o_d_u_l_e___c_o_m_m_e_n_t_._M_o_d_u_l_e_C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
-    * _c_a_t_e_g_o_r_y___i_d_ _(_p_y_l_e_r_o_._c_a_t_e_g_o_r_y_._C_a_t_e_g_o_r_y                    o _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)
-      _a_t_t_r_i_b_u_t_e_)                                               o _(_p_y_l_e_r_o_._r_e_v_i_s_i_o_n_._R_e_v_i_s_i_o_n_ _a_t_t_r_i_b_u_t_e_)
-    * _c_f_t___i_d_                                                   o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _a_t_t_r_i_b_u_t_e_)
-      _(_p_y_l_e_r_o_._c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_._C_u_s_t_o_m_F_i_e_l_d_T_y_p_e                o _(_p_y_l_e_r_o_._w_i_k_i___p_a_g_e_._W_i_k_i_P_a_g_e_ _a_t_t_r_i_b_u_t_e_)
-      _a_t_t_r_i_b_u_t_e_)                                         * _c_r_e_a_t_i_o_n_ _(_p_y_l_e_r_o_._c_h_a_n_g_e_._C_h_a_n_g_e_ _a_t_t_r_i_b_u_t_e_)
-    * _C_h_a_n_g_e_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_h_a_n_g_e_)                    * _c_r_e_a_t_i_o_n___t_i_m_e_ _(_p_y_l_e_r_o_._b_u_i_l_d_._B_u_i_l_d_ _a_t_t_r_i_b_u_t_e_)
-    * _C_h_a_n_g_e_R_e_q_u_e_s_t_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._w_o_r_k___i_t_e_m_)          * _C_U_R_D_I_R___C_O_N_F_I_G_ _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._C_o_n_f_i_g_u_r_a_t_i_o_n_ _a_t_t_r_i_b_u_t_e_)
-    * _c_h_e_c_k___v_a_l_i_d___f_i_e_l_d___v_a_l_u_e_s_(_)_                         * _C_u_s_t_o_m_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_u_s_t_o_m_)
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_u_s_t_o_m___a_r_r_a_y___o_b_j_(_)_ _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n
-    * _c_h_i_l_d___c_o_m_m_e_n_t___u_r_i_s_ _(_p_y_l_e_r_o_._c_o_m_m_e_n_t_._C_o_m_m_e_n_t           _m_e_t_h_o_d_)
-      _a_t_t_r_i_b_u_t_e_)                                         * _c_u_s_t_o_m___f_i_e_l_d_s_ _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
-          o _(_p_y_l_e_r_o_._m_o_d_u_l_e___c_o_m_m_e_n_t_._M_o_d_u_l_e_C_o_m_m_e_n_t               o _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)
-            _a_t_t_r_i_b_u_t_e_)                                         o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _a_t_t_r_i_b_u_t_e_)
-    * _C_l_a_s_s_P_r_o_p_e_r_t_y_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_)      * _c_u_s_t_o_m___o_b_j_(_)_ _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)
-    * _c_l_e_a_n_e_d___f_e_a_t_u_r_e_s_                                   * _c_u_s_t_o_m___v_a_l_u_e_s_ 
-      _(_p_y_l_e_r_o_._w_o_r_k_f_l_o_w___a_c_t_i_o_n_._W_o_r_k_f_l_o_w_A_c_t_i_o_n               _(_p_y_l_e_r_o_._a_c_t_i_v_i_t_y___c_u_s_t_o_m___v_a_l_u_e___e_n_t_r_y_._A_c_t_i_v_i_t_y_C_u_s_t_o_m_V_a_l_u_e_E_n_t_r_y
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___p_l_a_n___t_e_m_p_l_a_t_e_(_)_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
+    * _c_a_n___m_o_d_i_f_y___k_e_y_(_)_                                   * _c_r_e_a_t_e___s_s_l___c_o_n_t_e_x_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _p_y_l_e_r_o_._s_e_s_s_i_o_n_)
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___s_u_m_m_a_r_y___d_e_f_e_c_t_(_)_ _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)
+    * _c_a_n___r_e_a_d___i_n_s_t_a_n_c_e_(_)_                                * _c_r_e_a_t_e___t_e_m_p_l_a_t_e_(_)_ _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _c_l_a_s_s_ _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e___u_s_e_r_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _c_l_a_s_s_ _m_e_t_h_o_d_)
+    * _c_a_n___r_e_a_d___k_e_y_(_)_                                     * _c_r_e_a_t_e___w_o_r_k___i_t_e_m_(_)_ _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)         * _c_r_e_a_t_e_d_ _(_p_y_l_e_r_o_._c_o_m_m_e_n_t_._C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
+    * _c_a_n___r_e_m_o_v_e___e_l_e_m_e_n_t___f_r_o_m___k_e_y_(_)_                            o _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)               o _(_p_y_l_e_r_o_._i_m_p_o_r_t_e_d___c_o_m_m_e_n_t_._I_m_p_o_r_t_e_d_C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
+    * _c_a_p_a_c_i_t_y_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)                    o _(_p_y_l_e_r_o_._m_o_d_u_l_e___c_o_m_m_e_n_t_._M_o_d_u_l_e_C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
+    * _C_a_t_e_g_o_r_y_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_a_t_e_g_o_r_y_)                      o _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)
+    * _c_a_t_e_g_o_r_y___i_d_ _(_p_y_l_e_r_o_._c_a_t_e_g_o_r_y_._C_a_t_e_g_o_r_y                    o _(_p_y_l_e_r_o_._r_e_v_i_s_i_o_n_._R_e_v_i_s_i_o_n_ _a_t_t_r_i_b_u_t_e_)
+      _a_t_t_r_i_b_u_t_e_)                                               o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _a_t_t_r_i_b_u_t_e_)
+    * _c_f_t___i_d_                                                   o _(_p_y_l_e_r_o_._w_i_k_i___p_a_g_e_._W_i_k_i_P_a_g_e_ _a_t_t_r_i_b_u_t_e_)
+      _(_p_y_l_e_r_o_._c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_._C_u_s_t_o_m_F_i_e_l_d_T_y_p_e          * _c_r_e_a_t_i_o_n_ _(_p_y_l_e_r_o_._c_h_a_n_g_e_._C_h_a_n_g_e_ _a_t_t_r_i_b_u_t_e_)
+      _a_t_t_r_i_b_u_t_e_)                                         * _c_r_e_a_t_i_o_n___t_i_m_e_ _(_p_y_l_e_r_o_._b_u_i_l_d_._B_u_i_l_d_ _a_t_t_r_i_b_u_t_e_)
+    * _C_h_a_n_g_e_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_h_a_n_g_e_)                    * _C_U_R_D_I_R___C_O_N_F_I_G_ _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._C_o_n_f_i_g_u_r_a_t_i_o_n_ _a_t_t_r_i_b_u_t_e_)
+    * _C_h_a_n_g_e_R_e_q_u_e_s_t_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._w_o_r_k___i_t_e_m_)          * _C_u_s_t_o_m_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_u_s_t_o_m_)
+    * _c_h_e_c_k___v_a_l_i_d___f_i_e_l_d___v_a_l_u_e_s_(_)_                         * _c_u_s_t_o_m___a_r_r_a_y___o_b_j_(_)_ _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)           _m_e_t_h_o_d_)
+    * _c_h_i_l_d___c_o_m_m_e_n_t___u_r_i_s_ _(_p_y_l_e_r_o_._c_o_m_m_e_n_t_._C_o_m_m_e_n_t         * _c_u_s_t_o_m___f_i_e_l_d_s_ _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
+      _a_t_t_r_i_b_u_t_e_)                                               o _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)
+          o _(_p_y_l_e_r_o_._m_o_d_u_l_e___c_o_m_m_e_n_t_._M_o_d_u_l_e_C_o_m_m_e_n_t               o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _a_t_t_r_i_b_u_t_e_)
+            _a_t_t_r_i_b_u_t_e_)                                   * _c_u_s_t_o_m___o_b_j_(_)_ _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n_ _m_e_t_h_o_d_)
+    * _C_l_a_s_s_P_r_o_p_e_r_t_y_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_)      * _c_u_s_t_o_m___v_a_l_u_e_s_ 
+    * _c_l_e_a_n_e_d___f_e_a_t_u_r_e_s_                                     _(_p_y_l_e_r_o_._a_c_t_i_v_i_t_y___c_u_s_t_o_m___v_a_l_u_e___e_n_t_r_y_._A_c_t_i_v_i_t_y_C_u_s_t_o_m_V_a_l_u_e_E_n_t_r_y
+      _(_p_y_l_e_r_o_._w_o_r_k_f_l_o_w___a_c_t_i_o_n_._W_o_r_k_f_l_o_w_A_c_t_i_o_n               _a_t_t_r_i_b_u_t_e_)
+      _a_t_t_r_i_b_u_t_e_)                                         * _c_u_s_t_o_m_e_r___c_o_m_p_a_n_y_ _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e
+    * _c_l_o_s_e_d_ _(_p_y_l_e_r_o_._t_i_m_e___p_o_i_n_t_._T_i_m_e_P_o_i_n_t_ _a_t_t_r_i_b_u_t_e_)       _a_t_t_r_i_b_u_t_e_)
+    * _C_m_d_L_i_s_t_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_l_i_._c_m_d_)                  * _c_u_s_t_o_m_e_r___e_m_a_i_l_ _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e
+    * _C_m_d_U_p_d_a_t_e_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_l_i_._c_m_d_)                  _a_t_t_r_i_b_u_t_e_)
+    * _c_o_l_l_e_c_t_i_o_n_ _(_p_y_l_e_r_o_._f_i_e_l_d___d_i_f_f_._F_i_e_l_d_D_i_f_f            * _c_u_s_t_o_m_e_r___n_a_m_e_ _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e
       _a_t_t_r_i_b_u_t_e_)                                           _a_t_t_r_i_b_u_t_e_)
-    * _c_l_o_s_e_d_ _(_p_y_l_e_r_o_._t_i_m_e___p_o_i_n_t_._T_i_m_e_P_o_i_n_t_ _a_t_t_r_i_b_u_t_e_)     * _c_u_s_t_o_m_e_r___c_o_m_p_a_n_y_ _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e
-    * _C_m_d_L_i_s_t_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_l_i_._c_m_d_)                    _a_t_t_r_i_b_u_t_e_)
-    * _C_m_d_U_p_d_a_t_e_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_l_i_._c_m_d_)                * _c_u_s_t_o_m_e_r___e_m_a_i_l_ _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e
-    * _c_o_l_l_e_c_t_i_o_n_ _(_p_y_l_e_r_o_._f_i_e_l_d___d_i_f_f_._F_i_e_l_d_D_i_f_f              _a_t_t_r_i_b_u_t_e_)
-      _a_t_t_r_i_b_u_t_e_)                                         * _c_u_s_t_o_m_e_r___n_a_m_e_ _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e
-    * _c_o_l_o_r_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)                   _a_t_t_r_i_b_u_t_e_)
-    * _C_o_m_m_e_n_t_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_o_m_m_e_n_t_)                  * _C_u_s_t_o_m_F_i_e_l_d_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_u_s_t_o_m___f_i_e_l_d_)
-    * _c_o_m_m_e_n_t_                                            * _C_u_s_t_o_m_F_i_e_l_d_T_y_p_e_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_)
+    * _c_o_l_o_r_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _a_t_t_r_i_b_u_t_e_)                 * _C_u_s_t_o_m_F_i_e_l_d_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_u_s_t_o_m___f_i_e_l_d_)
+    * _C_o_m_m_e_n_t_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_o_m_m_e_n_t_)                  * _C_u_s_t_o_m_F_i_e_l_d_T_y_p_e_ _(_c_l_a_s_s_ _i_n_ _p_y_l_e_r_o_._c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_)
+    * _c_o_m_m_e_n_t_ 
       _(_p_y_l_e_r_o_._t_e_s_t___s_t_e_p___r_e_s_u_l_t_._T_e_s_t_S_t_e_p_R_e_s_u_l_t
       _a_t_t_r_i_b_u_t_e_)
           o _(_p_y_l_e_r_o_._w_o_r_k___r_e_c_o_r_d_._W_o_r_k_R_e_c_o_r_d
             _a_t_t_r_i_b_u_t_e_)
     * _c_o_m_m_e_n_t___i_d_ _(_p_y_l_e_r_o_._c_o_m_m_e_n_t_._C_o_m_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
     * _c_o_m_m_e_n_t_s_ _(_p_y_l_e_r_o_._a_c_t_i_v_i_t_y_._A_c_t_i_v_i_t_y_ _a_t_t_r_i_b_u_t_e_)
           o _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
@@ -257,58 +257,61 @@
       _a_t_t_r_i_b_u_t_e_)                                                  _a_t_t_r_i_b_u_t_e_)
     * _f_i_l_e___n_a_m_e_ _(_p_y_l_e_r_o_._a_t_t_a_c_h_m_e_n_t_._A_t_t_a_c_h_m_e_n_t_ _a_t_t_r_i_b_u_t_e_)
           o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n___a_t_t_a_c_h_m_e_n_t_._T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
             _a_t_t_r_i_b_u_t_e_)
           o _(_p_y_l_e_r_o_._w_i_k_i___p_a_g_e___a_t_t_a_c_h_m_e_n_t_._W_i_k_i_P_a_g_e_A_t_t_a_c_h_m_e_n_t
             _a_t_t_r_i_b_u_t_e_)
 ********** GG **********
-    * _g_e_n_e_r_a_t_e___d_e_s_c_r_i_p_t_i_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e          * _g_e_t___p_r_o_j_e_c_t___u_s_e_r_s_(_)_ 
-      _p_y_l_e_r_o_._t_e_s_t___r_u_n_)                             _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
-    * _g_e_n_e_r_a_t_e_d___b_y_                               * _g_e_t___r_o_l_e_s_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r
-      _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e       _m_e_t_h_o_d_)
-      _a_t_t_r_i_b_u_t_e_)                                 * _g_e_t___r_o_o_t___p_r_o_j_e_c_t___g_r_o_u_p_(_)_ 
-    * _g_e_t___a_t_t_a_c_h_m_e_n_t_(_)_                             _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p
-      _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)             _c_l_a_s_s_ _m_e_t_h_o_d_)
-    * _g_e_t___a_t_t_a_c_h_m_e_n_t_s_(_)_                          * _g_e_t___s_t_a_t_i_s_t_i_c_s_(_)_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n
-      _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)             _m_e_t_h_o_d_)
-    * _g_e_t___c_a_t_e_g_o_r_i_e_s_(_)_                           * _g_e_t___t_e_s_t___s_t_e_p_s___c_o_n_f_i_g_u_r_a_t_i_o_n_(_)_ 
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)              _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
-    * _g_e_t___c_o_n_t_a_i_n_e_d___g_r_o_u_p_s_(_)_                     * _g_e_t___t_e_s_t_s___c_o_n_f_i_g_u_r_a_t_i_o_n_(_)_ 
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p           _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                    * _g_e_t___u_s_e_r___a_v_a_t_a_r___u_r_l_(_)_ 
-    * _g_e_t___c_o_n_t_a_i_n_e_d___p_r_o_j_e_c_t_s_(_)_                     _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _m_e_t_h_o_d_)
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p         * _g_e_t___u_s_e_r___f_r_o_m___t_o_k_e_n_(_)_ 
-      _m_e_t_h_o_d_)                                      _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _c_l_a_s_s_ _m_e_t_h_o_d_)
-    * _g_e_t___c_o_n_t_e_x_t___r_o_l_e_s_(_)_                        * _g_e_t___u_s_e_r_s_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _c_l_a_s_s
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _c_l_a_s_s_ _m_e_t_h_o_d_)        _m_e_t_h_o_d_)
-          o _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _m_e_t_h_o_d_)            * _g_e_t___v_a_l_i_d___f_i_e_l_d___v_a_l_u_e_s_(_)_ 
-    * _g_e_t___c_u_s_t_o_m___f_i_e_l_d_(_)_                           _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n
-      _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)             _m_e_t_h_o_d_)
-    * _g_e_t___d_e_e_p___c_o_n_t_a_i_n_e_d___p_r_o_j_e_c_t_s_(_)_              * _g_e_t___w_i_k_i___c_o_n_t_e_n_t_(_)_ 
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p           _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                          o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n
-    * _g_e_t___d_e_f_i_n_e_d___c_u_s_t_o_m___f_i_e_l_d___k_e_y_s_(_)_                    _m_e_t_h_o_d_)
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)            * _g_e_t___w_i_k_i___p_a_g_e_s_(_)_ 
-    * _g_e_t___d_e_f_i_n_e_d___c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_(_)_              _(_p_y_l_e_r_o_._w_i_k_i___p_a_g_e_._W_i_k_i_P_a_g_e_ _c_l_a_s_s
+    * _g_e_n_e_r_a_t_e_d___b_y_                               * _g_e_t___r_e_v_i_s_i_o_n___b_y___u_r_i_(_)_ 
+      _(_p_y_l_e_r_o_._p_r_o_d_u_c_t___l_i_c_e_n_s_e_._P_r_o_d_u_c_t_L_i_c_e_n_s_e       _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n
+      _a_t_t_r_i_b_u_t_e_)                                   _m_e_t_h_o_d_)
+    * _g_e_t___a_t_t_a_c_h_m_e_n_t_(_)_                           * _g_e_t___r_e_v_i_s_i_o_n_s_(_)_ 
+      _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)             _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n
+    * _g_e_t___a_t_t_a_c_h_m_e_n_t_s_(_)_                            _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)           * _g_e_t___r_o_l_e_s_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r
+    * _g_e_t___c_a_t_e_g_o_r_i_e_s_(_)_                             _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)            * _g_e_t___r_o_o_t___p_r_o_j_e_c_t___g_r_o_u_p_(_)_ 
+    * _g_e_t___c_o_n_t_a_i_n_e_d___g_r_o_u_p_s_(_)_                       _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p           _c_l_a_s_s_ _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                    * _g_e_t___s_t_a_t_i_s_t_i_c_s_(_)_ _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n
+    * _g_e_t___c_o_n_t_a_i_n_e_d___p_r_o_j_e_c_t_s_(_)_                     _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p         * _g_e_t___t_e_s_t___s_t_e_p_s___c_o_n_f_i_g_u_r_a_t_i_o_n_(_)_ 
+      _m_e_t_h_o_d_)                                      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
+    * _g_e_t___c_o_n_t_e_x_t___r_o_l_e_s_(_)_                        * _g_e_t___t_e_s_t_s___c_o_n_f_i_g_u_r_a_t_i_o_n_(_)_ 
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _c_l_a_s_s_ _m_e_t_h_o_d_)        _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
+          o _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _m_e_t_h_o_d_)            * _g_e_t___u_s_e_r___a_v_a_t_a_r___u_r_l_(_)_ 
+    * _g_e_t___c_u_s_t_o_m___f_i_e_l_d_(_)_                           _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _m_e_t_h_o_d_)           * _g_e_t___u_s_e_r___f_r_o_m___t_o_k_e_n_(_)_ 
+    * _g_e_t___d_e_e_p___c_o_n_t_a_i_n_e_d___p_r_o_j_e_c_t_s_(_)_                _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _c_l_a_s_s_ _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p         * _g_e_t___u_s_e_r_s_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r_ _c_l_a_s_s
+      _m_e_t_h_o_d_)                                      _m_e_t_h_o_d_)
+    * _g_e_t___d_e_f_i_n_e_d___c_u_s_t_o_m___f_i_e_l_d___k_e_y_s_(_)_            * _g_e_t___v_a_l_i_d___f_i_e_l_d___v_a_l_u_e_s_(_)_ 
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)              _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n
+    * _g_e_t___d_e_f_i_n_e_d___c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_(_)_              _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)            * _g_e_t___w_i_k_i___c_o_n_t_e_n_t_(_)_ 
+    * _g_e_t___d_e_f_i_n_e_d___c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_s_(_)_             _(_p_y_l_e_r_o_._p_l_a_n_._P_l_a_n_ _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)                  o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n
+          o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _c_l_a_s_s               _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                              * _g_e_t___w_i_k_i___p_a_g_e_s_(_)_ 
+    * _g_e_t___d_o_c_u_m_e_n_t___s_p_a_c_e_s_(_)_                        _(_p_y_l_e_r_o_._w_i_k_i___p_a_g_e_._W_i_k_i_P_a_g_e_ _c_l_a_s_s
       _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)              _m_e_t_h_o_d_)
-    * _g_e_t___d_e_f_i_n_e_d___c_u_s_t_o_m___f_i_e_l_d___t_y_p_e_s_(_)_           * _g_e_t___w_i_k_i___s_p_a_c_e_s_(_)_ 
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)              _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
-          o _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n_ _c_l_a_s_s       * _g_e_t___w_o_r_k___i_t_e_m_s_(_)_ 
-            _m_e_t_h_o_d_)                                _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _m_e_t_h_o_d_)
-    * _g_e_t___d_o_c_u_m_e_n_t___s_p_a_c_e_s_(_)_                      * _G_L_O_B_A_L___C_O_N_F_I_G_ 
-      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)              _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._C_o_n_f_i_g_u_r_a_t_i_o_n
-    * _g_e_t___d_o_c_u_m_e_n_t_s_(_)_                              _a_t_t_r_i_b_u_t_e_)
-      _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _c_l_a_s_s            * _g_l_o_b_a_l___i_d_ _(_p_y_l_e_r_o_._a_c_t_i_v_i_t_y_._A_c_t_i_v_i_t_y
+    * _g_e_t___d_o_c_u_m_e_n_t_s_(_)_                            * _g_e_t___w_i_k_i___s_p_a_c_e_s_(_)_ 
+      _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _c_l_a_s_s              _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                    * _g_e_t___w_o_r_k___i_t_e_m_s_(_)_ 
+    * _g_e_t___g_l_o_b_a_l___r_o_l_e_s_(_)_                           _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t_ _m_e_t_h_o_d_)
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n         * _G_L_O_B_A_L___C_O_N_F_I_G_ 
+      _c_l_a_s_s_ _m_e_t_h_o_d_)                                _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._C_o_n_f_i_g_u_r_a_t_i_o_n
+    * _g_e_t___l_o_c_a_t_i_o_n_(_)_                               _a_t_t_r_i_b_u_t_e_)
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n         * _g_l_o_b_a_l___i_d_ _(_p_y_l_e_r_o_._a_c_t_i_v_i_t_y_._A_c_t_i_v_i_t_y
+      _m_e_t_h_o_d_)                                      _a_t_t_r_i_b_u_t_e_)
+    * _g_e_t___p_r_o_j_e_c_t___u_s_e_r_s_(_)_                        * _g_r_o_u_p___i_d_ _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n
+      _(_p_y_l_e_r_o_._p_r_o_j_e_c_t_._P_r_o_j_e_c_t_ _m_e_t_h_o_d_)              _a_t_t_r_i_b_u_t_e_)
+    * _g_e_t___r_e_v_i_s_i_o_n_(_)_                             * _g_r_o_u_p___u_r_i_s_ 
+      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n           _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p
       _m_e_t_h_o_d_)                                      _a_t_t_r_i_b_u_t_e_)
-    * _g_e_t___g_l_o_b_a_l___r_o_l_e_s_(_)_                         * _g_r_o_u_p___i_d_ _(_p_y_l_e_r_o_._t_e_s_t___r_u_n_._T_e_s_t_R_u_n
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n           _a_t_t_r_i_b_u_t_e_)
-      _c_l_a_s_s_ _m_e_t_h_o_d_)                              * _g_r_o_u_p___u_r_i_s_ 
-    * _g_e_t___l_o_c_a_t_i_o_n_(_)_                               _(_p_y_l_e_r_o_._p_r_o_j_e_c_t___g_r_o_u_p_._P_r_o_j_e_c_t_G_r_o_u_p
-      _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n           _a_t_t_r_i_b_u_t_e_)
-      _m_e_t_h_o_d_)
 ********** HH **********
     * _h_a_s___c_u_r_r_e_n_t___u_s_e_r___p_e_r_m_i_s_s_i_o_n_(_)_              * _h_o_m_e___p_a_g_e___c_o_n_t_e_n_t_ 
       _(_p_y_l_e_r_o_._b_a_s_e___p_o_l_a_r_i_o_n_._B_a_s_e_P_o_l_a_r_i_o_n           _(_p_y_l_e_r_o_._d_o_c_u_m_e_n_t_._D_o_c_u_m_e_n_t
       _c_l_a_s_s_ _m_e_t_h_o_d_)                                _a_t_t_r_i_b_u_t_e_)
     * _h_a_s___p_e_r_m_i_s_s_i_o_n_(_)_ _(_p_y_l_e_r_o_._u_s_e_r_._U_s_e_r               o _(_p_y_l_e_r_o_._w_i_k_i___p_a_g_e_._W_i_k_i_P_a_g_e
       _m_e_t_h_o_d_)                                            _a_t_t_r_i_b_u_t_e_)
     * _h_i_d_d_e_n_ _(_p_y_l_e_r_o_._e_n_u_m___o_p_t_i_o_n_._E_n_u_m_O_p_t_i_o_n      * _H_y_p_e_r_l_i_n_k_ _(_c_l_a_s_s_ _i_n
@@ -799,9 +802,9 @@
 ************ _pp_yy_ll_ee_rr_oo ************
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/index.html` & `pylero-0.1.0/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
     <title>Welcome to pylero’s documentation! &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="pylero" href="modules.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -596,16 +596,14 @@
 <li class="toctree-l3"><a class="reference internal" href="pylero.html#module-pylero.test_record">pylero.test_record module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_record.ArrayOfTestRecord"><code class="docutils literal notranslate"><span class="pre">ArrayOfTestRecord</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_record.TestRecord"><code class="docutils literal notranslate"><span class="pre">TestRecord</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="pylero.html#module-pylero.test_run">pylero.test_run module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.TestRun"><code class="docutils literal notranslate"><span class="pre">TestRun</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.create_incident_report"><code class="docutils literal notranslate"><span class="pre">create_incident_report()</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.generate_description"><code class="docutils literal notranslate"><span class="pre">generate_description()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="pylero.html#module-pylero.test_run_attachment">pylero.test_run_attachment module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run_attachment.ArrayOfTestRunAttachment"><code class="docutils literal notranslate"><span class="pre">ArrayOfTestRunAttachment</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run_attachment.TestRunAttachment"><code class="docutils literal notranslate"><span class="pre">TestRunAttachment</span></code></a></li>
 </ul>
 </li>
@@ -716,23 +714,23 @@
 <h3>Related Topics</h3>
 <ul>
   <li><a href="#">Documentation overview</a><ul>
       <li>Next: <a href="modules.html" title="next chapter">pylero</a></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -742,15 +740,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
       |
       <a href="_sources/index.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -408,16 +408,14 @@
                       # _A_r_r_a_y_O_f_S_u_b_t_e_r_r_a_U_R_I
                       # _S_u_b_t_e_r_r_a_U_R_I
                 # _p_y_l_e_r_o_._t_e_s_t___r_e_c_o_r_d_ _m_o_d_u_l_e
                       # _A_r_r_a_y_O_f_T_e_s_t_R_e_c_o_r_d
                       # _T_e_s_t_R_e_c_o_r_d
                 # _p_y_l_e_r_o_._t_e_s_t___r_u_n_ _m_o_d_u_l_e
                       # _T_e_s_t_R_u_n
-                      # _c_r_e_a_t_e___i_n_c_i_d_e_n_t___r_e_p_o_r_t_(_)
-                      # _g_e_n_e_r_a_t_e___d_e_s_c_r_i_p_t_i_o_n_(_)
                 # _p_y_l_e_r_o_._t_e_s_t___r_u_n___a_t_t_a_c_h_m_e_n_t_ _m_o_d_u_l_e
                       # _A_r_r_a_y_O_f_T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
                       # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
                 # _p_y_l_e_r_o_._t_e_s_t___s_t_e_p_ _m_o_d_u_l_e
                       # _A_r_r_a_y_O_f_T_e_s_t_S_t_e_p
                       # _T_e_s_t_S_t_e_p
                 # _p_y_l_e_r_o_._t_e_s_t___s_t_e_p___r_e_s_u_l_t_ _m_o_d_u_l_e
@@ -465,9 +463,9 @@
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o Next: _p_y_l_e_r_o
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6 | _P_a_g_e_ _s_o_u_r_c_e
```

### Comparing `pylero-0.0.9/docs/modules.html` & `pylero-0.1.0/docs/modules.html`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
     <title>pylero &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="pylero package" href="pylero.html" />
     <link rel="prev" title="Welcome to pylero’s documentation!" href="index.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
@@ -144,14 +144,17 @@
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.can_remove_element_from_key"><code class="docutils literal notranslate"><span class="pre">BasePolarion.can_remove_element_from_key()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.check_valid_field_values"><code class="docutils literal notranslate"><span class="pre">BasePolarion.check_valid_field_values()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.custom_array_obj"><code class="docutils literal notranslate"><span class="pre">BasePolarion.custom_array_obj()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.custom_obj"><code class="docutils literal notranslate"><span class="pre">BasePolarion.custom_obj()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#id0"><code class="docutils literal notranslate"><span class="pre">BasePolarion.default_project</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.get_global_roles"><code class="docutils literal notranslate"><span class="pre">BasePolarion.get_global_roles()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.get_location"><code class="docutils literal notranslate"><span class="pre">BasePolarion.get_location()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.get_revision"><code class="docutils literal notranslate"><span class="pre">BasePolarion.get_revision()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.get_revision_by_uri"><code class="docutils literal notranslate"><span class="pre">BasePolarion.get_revision_by_uri()</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.get_revisions"><code class="docutils literal notranslate"><span class="pre">BasePolarion.get_revisions()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.get_valid_field_values"><code class="docutils literal notranslate"><span class="pre">BasePolarion.get_valid_field_values()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.has_current_user_permission"><code class="docutils literal notranslate"><span class="pre">BasePolarion.has_current_user_permission()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.logged_in_user_id"><code class="docutils literal notranslate"><span class="pre">BasePolarion.logged_in_user_id</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.reload"><code class="docutils literal notranslate"><span class="pre">BasePolarion.reload()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.base_polarion.BasePolarion.repo"><code class="docutils literal notranslate"><span class="pre">BasePolarion.repo</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#id1"><code class="docutils literal notranslate"><span class="pre">BasePolarion.session</span></code></a></li>
 </ul>
@@ -805,16 +808,14 @@
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.TestRun.update_test_record_by_fields"><code class="docutils literal notranslate"><span class="pre">TestRun.update_test_record_by_fields()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.TestRun.update_test_record_by_object"><code class="docutils literal notranslate"><span class="pre">TestRun.update_test_record_by_object()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.TestRun.update_wiki_content"><code class="docutils literal notranslate"><span class="pre">TestRun.update_wiki_content()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.TestRun.verify_params"><code class="docutils literal notranslate"><span class="pre">TestRun.verify_params()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run.TestRun.verify_required"><code class="docutils literal notranslate"><span class="pre">TestRun.verify_required()</span></code></a></li>
 </ul>
 </li>
-<li class="toctree-l3"><a class="reference internal" href="pylero.html#pylero.test_run.create_incident_report"><code class="docutils literal notranslate"><span class="pre">create_incident_report()</span></code></a></li>
-<li class="toctree-l3"><a class="reference internal" href="pylero.html#pylero.test_run.generate_description"><code class="docutils literal notranslate"><span class="pre">generate_description()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="pylero.html#module-pylero.test_run_attachment">pylero.test_run_attachment module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="pylero.html#pylero.test_run_attachment.ArrayOfTestRunAttachment"><code class="docutils literal notranslate"><span class="pre">ArrayOfTestRunAttachment</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="pylero.html#pylero.test_run_attachment.TestRunAttachment"><code class="docutils literal notranslate"><span class="pre">TestRunAttachment</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run_attachment.TestRunAttachment.author"><code class="docutils literal notranslate"><span class="pre">TestRunAttachment.author</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="pylero.html#pylero.test_run_attachment.TestRunAttachment.file_name"><code class="docutils literal notranslate"><span class="pre">TestRunAttachment.file_name</span></code></a></li>
@@ -1045,23 +1046,23 @@
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
       <li>Previous: <a href="index.html" title="previous chapter">Welcome to pylero’s documentation!</a></li>
       <li>Next: <a href="pylero.html" title="next chapter">pylero package</a></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -1071,15 +1072,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
       |
       <a href="_sources/modules.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -75,14 +75,17 @@
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._c_a_n___r_e_m_o_v_e___e_l_e_m_e_n_t___f_r_o_m___k_e_y_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._c_h_e_c_k___v_a_l_i_d___f_i_e_l_d___v_a_l_u_e_s_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._c_u_s_t_o_m___a_r_r_a_y___o_b_j_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._c_u_s_t_o_m___o_b_j_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._d_e_f_a_u_l_t___p_r_o_j_e_c_t
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._g_e_t___g_l_o_b_a_l___r_o_l_e_s_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._g_e_t___l_o_c_a_t_i_o_n_(_)
+                      # _B_a_s_e_P_o_l_a_r_i_o_n_._g_e_t___r_e_v_i_s_i_o_n_(_)
+                      # _B_a_s_e_P_o_l_a_r_i_o_n_._g_e_t___r_e_v_i_s_i_o_n___b_y___u_r_i_(_)
+                      # _B_a_s_e_P_o_l_a_r_i_o_n_._g_e_t___r_e_v_i_s_i_o_n_s_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._g_e_t___v_a_l_i_d___f_i_e_l_d___v_a_l_u_e_s_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._h_a_s___c_u_r_r_e_n_t___u_s_e_r___p_e_r_m_i_s_s_i_o_n_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._l_o_g_g_e_d___i_n___u_s_e_r___i_d
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._r_e_l_o_a_d_(_)
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._r_e_p_o
                       # _B_a_s_e_P_o_l_a_r_i_o_n_._s_e_s_s_i_o_n
                 # _C_l_a_s_s_P_r_o_p_e_r_t_y
@@ -554,16 +557,14 @@
                       # _T_e_s_t_R_u_n_._u_p_d_a_t_e___a_t_t_a_c_h_m_e_n_t_(_)
                       # _T_e_s_t_R_u_n_._u_p_d_a_t_e___s_u_m_m_a_r_y___d_e_f_e_c_t_(_)
                       # _T_e_s_t_R_u_n_._u_p_d_a_t_e___t_e_s_t___r_e_c_o_r_d___b_y___f_i_e_l_d_s_(_)
                       # _T_e_s_t_R_u_n_._u_p_d_a_t_e___t_e_s_t___r_e_c_o_r_d___b_y___o_b_j_e_c_t_(_)
                       # _T_e_s_t_R_u_n_._u_p_d_a_t_e___w_i_k_i___c_o_n_t_e_n_t_(_)
                       # _T_e_s_t_R_u_n_._v_e_r_i_f_y___p_a_r_a_m_s_(_)
                       # _T_e_s_t_R_u_n_._v_e_r_i_f_y___r_e_q_u_i_r_e_d_(_)
-                # _c_r_e_a_t_e___i_n_c_i_d_e_n_t___r_e_p_o_r_t_(_)
-                # _g_e_n_e_r_a_t_e___d_e_s_c_r_i_p_t_i_o_n_(_)
           o _p_y_l_e_r_o_._t_e_s_t___r_u_n___a_t_t_a_c_h_m_e_n_t_ _m_o_d_u_l_e
                 # _A_r_r_a_y_O_f_T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
                 # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
                       # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t_._a_u_t_h_o_r
                       # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t_._f_i_l_e___n_a_m_e
                       # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t_._i_d
                       # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t_._l_e_n_g_t_h
@@ -713,9 +714,9 @@
           o _p_y_l_e_r_o_ _p_a_c_k_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o Previous: _W_e_l_c_o_m_e_ _t_o_ _p_y_l_e_r_o_’_s_ _d_o_c_u_m_e_n_t_a_t_i_o_n_!
           o Next: _p_y_l_e_r_o_ _p_a_c_k_a_g_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6 | _P_a_g_e_ _s_o_u_r_c_e
```

### Comparing `pylero-0.0.9/docs/py-modindex.html` & `pylero-0.1.0/docs/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Python Module Index &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
 
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -405,23 +405,23 @@
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -431,15 +431,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -72,9 +72,9 @@
 ************ _pp_yy_ll_ee_rr_oo ************
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/pylero.cli.html` & `pylero-0.1.0/docs/pylero.cli.html`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
     <title>pylero.cli package &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="pylero package" href="pylero.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -252,23 +252,23 @@
   <li><a href="pylero.html">pylero package</a><ul>
       <li>Previous: <a href="pylero.html" title="previous chapter">pylero package</a></li>
   </ul></li>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -278,15 +278,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
       |
       <a href="_sources/pylero.cli.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -105,9 +105,9 @@
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _p_y_l_e_r_o
                 # _p_y_l_e_r_o_ _p_a_c_k_a_g_e
                       # Previous: _p_y_l_e_r_o_ _p_a_c_k_a_g_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6 | _P_a_g_e_ _s_o_u_r_c_e
```

### Comparing `pylero-0.0.9/docs/pylero.html` & `pylero-0.1.0/docs/pylero.html`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
     <title>pylero package &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="pylero.cli package" href="pylero.cli.html" />
     <link rel="prev" title="pylero" href="modules.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
@@ -598,15 +598,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.can_delete_instance">
 <span class="sig-name descname"><span class="pre">can_delete_instance</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.can_delete_instance"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.can_delete_instance" title="Link to this definition">¶</a></dt>
 <dd><p>Checks if the current user can delete the current object</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>bool</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.canDeleteInstance</p>
@@ -614,15 +614,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.can_modify_instance">
 <span class="sig-name descname"><span class="pre">can_modify_instance</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.can_modify_instance"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.can_modify_instance" title="Link to this definition">¶</a></dt>
 <dd><p>Checks if the current user can modify the current object</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>bool</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.canModifyInstance</p>
@@ -647,15 +647,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.can_read_instance">
 <span class="sig-name descname"><span class="pre">can_read_instance</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.can_read_instance"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.can_read_instance" title="Link to this definition">¶</a></dt>
 <dd><p>Checks if the current user can read the current object</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>bool</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.canReadInstance</p>
@@ -732,15 +732,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.get_global_roles">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">get_global_roles</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.get_global_roles"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.get_global_roles" title="Link to this definition">¶</a></dt>
 <dd><p>Returns all global roles.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of global roles</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.<a class="reference external" href="https://almdemo.polarion.com/polarion/sdk/doc/javadoc/com/polarion/alm/ws/client/security/SecurityWebService.html#getGlobalRoles()">getGlobalRoles()</a></p>
@@ -750,25 +750,64 @@
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.get_location">
 <span class="sig-name descname"><span class="pre">get_location</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.get_location"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.get_location" title="Link to this definition">¶</a></dt>
 <dd><p>Returns the location of the current object. In the context of this
 service the method should be used to get the location of a
 project(-group).</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>location (string)</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.getLocationForURI</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.get_revision">
+<span class="sig-name descname"><span class="pre">get_revision</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">repository_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">revision_id</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.get_revision"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.get_revision" title="Link to this definition">¶</a></dt>
+<dd><p>Gets a revision
+:param repository_name - The repository name.:
+:type repository_name - The repository name.: Put “default” for the default repository.
+:param revision_id - The revision name.:</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>a Revision object</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.get_revision_by_uri">
+<span class="sig-name descname"><span class="pre">get_revision_by_uri</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">revision_uri</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.get_revision_by_uri"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.get_revision_by_uri" title="Link to this definition">¶</a></dt>
+<dd><p>Gets a revision by its URI
+:param revision_uri - The URI of the revision.:</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>a Revision object</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.get_revisions">
+<span class="sig-name descname"><span class="pre">get_revisions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">uri</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.get_revisions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.get_revisions" title="Link to this definition">¶</a></dt>
+<dd><p>Returns all revisions for a specific URI.
+:param uri - URI of the persistence object:
+:type uri - URI of the persistence object: Work Item, Module/Document, User, etc</p>
+<dl class="field-list simple">
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>All revisions for a specific URI.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.get_valid_field_values">
 <span class="sig-name descname"><span class="pre">get_valid_field_values</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">enum_id</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">control</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.get_valid_field_values"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.get_valid_field_values" title="Link to this definition">¶</a></dt>
 <dd><p>Gets the available enumeration options.
 Uses a cache dict because the time to get valid fields from server
 is time prohibitive.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -803,38 +842,38 @@
 </dl>
 <p class="rubric">References</p>
 <p>Security.hasCurrentUserPermission</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.logged_in_user_id">
-<span class="sig-name descname"><span class="pre">logged_in_user_id</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'gsun'</span></em><a class="headerlink" href="#pylero.base_polarion.BasePolarion.logged_in_user_id" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">logged_in_user_id</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'POLARION_USERNAME'</span></em><a class="headerlink" href="#pylero.base_polarion.BasePolarion.logged_in_user_id" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.reload">
 <span class="sig-name descname"><span class="pre">reload</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#BasePolarion.reload"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.BasePolarion.reload" title="Link to this definition">¶</a></dt>
 <dd><p>Reloads the object with data from the server.
 This function is useful if the data on the server changed or if a
 data changing function was called (such as TestRun.add_attachment)</p>
 <p class="rubric">Notes</p>
 <p>This will overwrite any unsaved data in the object.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.BasePolarion.repo">
-<span class="sig-name descname"><span class="pre">repo</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'POLARION_URL/repo'</span></em><a class="headerlink" href="#pylero.base_polarion.BasePolarion.repo" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">repo</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'https://polarion.engineering.redhat.com/repo'</span></em><a class="headerlink" href="#pylero.base_polarion.BasePolarion.repo" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="id1">
 <span class="sig-name descname"><span class="pre">session</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">&lt;pylero.session.Session</span> <span class="pre">object&gt;</span></em><a class="headerlink" href="#id1" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
@@ -861,30 +900,30 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.Configuration.CURDIR_CONFIG">
 <span class="sig-name descname"><span class="pre">CURDIR_CONFIG</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'.pylero'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.CURDIR_CONFIG" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.Configuration.GLOBAL_CONFIG">
-<span class="sig-name descname"><span class="pre">GLOBAL_CONFIG</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'/home/waynesun/.local/share/virtualenvs/pylero-xZ4TB2uX/lib/python3.11/site-packages/pylero/pylero.cfg'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.GLOBAL_CONFIG" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">GLOBAL_CONFIG</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'/home/wayne/.local/share/virtualenvs/pylero-mnliz9Ju/lib/python3.12/site-packages/pylero/pylero.cfg'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.GLOBAL_CONFIG" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.Configuration.LOCAL_CONFIG">
-<span class="sig-name descname"><span class="pre">LOCAL_CONFIG</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'/home/waynesun/.pylero'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.LOCAL_CONFIG" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">LOCAL_CONFIG</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'/home/wayne/.pylero'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.LOCAL_CONFIG" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.base_polarion.Configuration.__init__">
 <span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#Configuration.__init__"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.Configuration.__init__" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.Configuration.pkgdir">
-<span class="sig-name descname"><span class="pre">pkgdir</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'/home/waynesun/.local/share/virtualenvs/pylero-xZ4TB2uX/lib/python3.11/site-packages/pylero'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.pkgdir" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">pkgdir</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'/home/wayne/.local/share/virtualenvs/pylero-mnliz9Ju/lib/python3.12/site-packages/pylero'</span></em><a class="headerlink" href="#pylero.base_polarion.Configuration.pkgdir" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="pylero.base_polarion.Connection">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">pylero.base_polarion.</span></span><span class="sig-name descname"><span class="pre">Connection</span></span><a class="reference internal" href="_modules/pylero/base_polarion.html#Connection"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.Connection" title="Link to this definition">¶</a></dt>
@@ -915,15 +954,15 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.Connection.session">
 <span class="sig-name descname"><span class="pre">session</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">&lt;pylero.session.Session</span> <span class="pre">object&gt;</span></em><a class="headerlink" href="#pylero.base_polarion.Connection.session" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="pylero.base_polarion.Connection.token_enabled">
-<span class="sig-name descname"><span class="pre">token_enabled</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">True</span></em><a class="headerlink" href="#pylero.base_polarion.Connection.token_enabled" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">token_enabled</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">False</span></em><a class="headerlink" href="#pylero.base_polarion.Connection.token_enabled" title="Link to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pylero.base_polarion.tx_wrapper">
 <span class="sig-prename descclassname"><span class="pre">pylero.base_polarion.</span></span><span class="sig-name descname"><span class="pre">tx_wrapper</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">func</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/base_polarion.html#tx_wrapper"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.base_polarion.tx_wrapper" title="Link to this definition">¶</a></dt>
@@ -1001,15 +1040,15 @@
 <dt class="sig sig-object py" id="pylero.baseline.Baseline.create">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">project_id</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">revision</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/baseline.html#Baseline.create"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.baseline.Baseline.create" title="Link to this definition">¶</a></dt>
 <dd><p>class method create Creates a Baseline from head or particular
 revision.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>project_id</strong> – </p></li>
+<li><p><strong>project_id</strong></p></li>
 <li><p><strong>name</strong> – baseline name (not None)</p></li>
 <li><p><strong>description</strong> – baseline description (can be None)</p></li>
 <li><p><strong>revision</strong> – revision or null value for head revision</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Baseline object</p>
@@ -2056,15 +2095,15 @@
 <span class="sig-name descname"><span class="pre">add_referenced_work_item</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">work_item_id</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/document.html#Document.add_referenced_work_item"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.document.Document.add_referenced_work_item" title="Link to this definition">¶</a></dt>
 <dd><p>Adds a work item to the document as a referenced work_item to the
 end of the current document.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>work_item_id</strong> (<em>str</em>) – the id of a work item in the same project as</p></li>
-<li><p><strong>document</strong> (<em>the current</em>) – </p></li>
+<li><p><strong>document</strong> (<em>the current</em>)</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 </dd></dl>
@@ -2118,15 +2157,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.document.Document.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/document.html#Document.delete"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.document.Document.delete" title="Link to this definition">¶</a></dt>
 <dd><p>delete the current document</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 </dd></dl>
 
@@ -2273,15 +2312,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.document.Document.update">
 <span class="sig-name descname"><span class="pre">update</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/document.html#Document.update"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.document.Document.update" title="Link to this definition">¶</a></dt>
 <dd><p>updates the server with the current module data</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Tracker.updateModule</p>
@@ -3322,15 +3361,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.plan.Plan.get_statistics">
 <span class="sig-name descname"><span class="pre">get_statistics</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/plan.html#Plan.get_statistics"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.plan.Plan.get_statistics" title="Link to this definition">¶</a></dt>
 <dd><p>get statistics of the plan</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>PlanStatistics object</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Planning.getPlanStatistics</p>
@@ -3338,15 +3377,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.plan.Plan.get_wiki_content">
 <span class="sig-name descname"><span class="pre">get_wiki_content</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/plan.html#Plan.get_wiki_content"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.plan.Plan.get_wiki_content" title="Link to this definition">¶</a></dt>
 <dd><p>Returns the wiki content of the plan</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Text object</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Planning.getPlanWikiContent</p>
@@ -3393,15 +3432,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.plan.Plan.set_wiki_content">
 <span class="sig-name descname"><span class="pre">set_wiki_content</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">content</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/plan.html#Plan.set_wiki_content"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.plan.Plan.set_wiki_content" title="Link to this definition">¶</a></dt>
 <dd><p>method set_wiki_content updates the wiki for the current Plan</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>Content</strong> (<em>str</em><em> or </em><em>Text object</em>) – </p>
+<dd class="field-odd"><p><strong>Content</strong> (<em>str</em><em> or </em><em>Text object</em>)</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Planning.setPlanWikiContent</p>
@@ -3409,15 +3448,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.plan.Plan.update">
 <span class="sig-name descname"><span class="pre">update</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/plan.html#Plan.update"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.plan.Plan.update" title="Link to this definition">¶</a></dt>
 <dd><p>updates the server with the current plan content</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Planning.updatePlan</p>
@@ -3425,15 +3464,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.plan.Plan.was_started">
 <span class="sig-name descname"><span class="pre">was_started</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/plan.html#Plan.was_started"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.plan.Plan.was_started" title="Link to this definition">¶</a></dt>
 <dd><p>checks if the plan was started yet</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>bool</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Planning.wasPlanStarted</p>
@@ -4070,15 +4109,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project.Project.get_categories">
 <span class="sig-name descname"><span class="pre">get_categories</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project.html#Project.get_categories"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project.Project.get_categories" title="Link to this definition">¶</a></dt>
 <dd><p>method get_categories retrieves a list of Category objects</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of Category objects</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Tracker.getCategories</p>
@@ -4155,15 +4194,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project.Project.get_document_spaces">
 <span class="sig-name descname"><span class="pre">get_document_spaces</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project.html#Project.get_document_spaces"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project.Project.get_document_spaces" title="Link to this definition">¶</a></dt>
 <dd><p>Gets the Module/Document spaces for the project.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of (string) document spaces</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Tracker.getDocumentSpaces</p>
@@ -4171,15 +4210,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project.Project.get_project_users">
 <span class="sig-name descname"><span class="pre">get_project_users</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project.html#Project.get_project_users"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project.Project.get_project_users" title="Link to this definition">¶</a></dt>
 <dd><p>Gets users of the project</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of u.User objects</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Project.getProjectUsers</p>
@@ -4188,15 +4227,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project.Project.get_test_steps_configuration">
 <span class="sig-name descname"><span class="pre">get_test_steps_configuration</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project.html#Project.get_test_steps_configuration"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project.Project.get_test_steps_configuration" title="Link to this definition">¶</a></dt>
 <dd><p>method get_test_steps_configuration retrieves a list of the
 Test Steps configuration for the project</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of configuration of the Test Steps custom field.</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>TestManagement.getTestStepsConfiguration</p>
@@ -4205,15 +4244,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project.Project.get_tests_configuration">
 <span class="sig-name descname"><span class="pre">get_tests_configuration</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project.html#Project.get_tests_configuration"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project.Project.get_tests_configuration" title="Link to this definition">¶</a></dt>
 <dd><p>method get_tests_configuration retrieves the test management
 configuration for the project</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>TestsConfiguration object</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>TestManagement.getTestsConfiguration</p>
@@ -4221,15 +4260,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project.Project.get_wiki_spaces">
 <span class="sig-name descname"><span class="pre">get_wiki_spaces</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project.html#Project.get_wiki_spaces"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project.Project.get_wiki_spaces" title="Link to this definition">¶</a></dt>
 <dd><p>Returns Wiki spaces from current project</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Array of string</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Tracker.getWikiSpaces</p>
@@ -4320,15 +4359,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project_group.ProjectGroup.get_contained_groups">
 <span class="sig-name descname"><span class="pre">get_contained_groups</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project_group.html#ProjectGroup.get_contained_groups"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project_group.ProjectGroup.get_contained_groups" title="Link to this definition">¶</a></dt>
 <dd><p>Gets all project groups located directly below the project group.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of p.ProjectGroup objects</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>p.Project.getContainedGroups</p>
@@ -4336,15 +4375,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project_group.ProjectGroup.get_contained_projects">
 <span class="sig-name descname"><span class="pre">get_contained_projects</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project_group.html#ProjectGroup.get_contained_projects"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project_group.ProjectGroup.get_contained_projects" title="Link to this definition">¶</a></dt>
 <dd><p>Gets all projects located directly below the project group.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of p.Project objects</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>p.Project.getContainedProjects</p>
@@ -4352,15 +4391,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project_group.ProjectGroup.get_deep_contained_projects">
 <span class="sig-name descname"><span class="pre">get_deep_contained_projects</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project_group.html#ProjectGroup.get_deep_contained_projects"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project_group.ProjectGroup.get_deep_contained_projects" title="Link to this definition">¶</a></dt>
 <dd><p>Gets all projects located below the project group.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of p.Project objects</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>p.Project.getDeepContainedProjects</p>
@@ -4368,15 +4407,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.project_group.ProjectGroup.get_root_project_group">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">get_root_project_group</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/project_group.html#ProjectGroup.get_root_project_group"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.project_group.ProjectGroup.get_root_project_group" title="Link to this definition">¶</a></dt>
 <dd><p>Gets the root project group.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>ProjectGroup object</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Project.getRootProjectGroup</p>
@@ -5198,54 +5237,58 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.add_test_record_by_fields">
 <span class="sig-name descname"><span class="pre">add_test_record_by_fields</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_case_id</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_result</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_comment</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">executed_by</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">executed</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">duration</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">defect_work_item_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.add_test_record_by_fields"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.add_test_record_by_fields" title="Link to this definition">¶</a></dt>
 <dd><p>method add_test_record_by_fields, adds a test record for the given
 test case based on the result fields passed in.
-When a test record is added, it changes the test run status to
+When a test record is added and the valid options for status contain
+“inprogress” and “finished”, it changes the test run status to
 “inprogress” and when the last test record is run, it changes the
-status to done.</p>
+status to “finished”.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>test_case_id</strong> (<em>str</em>) – The id of the test case that was executed</p></li>
 <li><p><strong>test_result</strong> (<em>str</em>) – Must be one of the following values:
 passed
 failed
 blocked</p></li>
 <li><p><strong>test_comment</strong> (<em>str</em><em> or </em><em>Text object</em>) – may be None</p></li>
 <li><p><strong>executed_by</strong> (<em>str</em>) – user id</p></li>
-<li><p><strong>executed</strong> (<em>datetime</em>) – </p></li>
-<li><p><strong>duration</strong> (<em>float</em>) – </p></li>
+<li><p><strong>executed</strong> (<em>datetime</em>)</p></li>
+<li><p><strong>duration</strong> (<em>float</em>)</p></li>
 <li><p><strong>defect_work_item_id</strong> (<em>str</em>) – _WorkItem id of defect, default: None</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>test_management.addTestRecordToTestRun</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.add_test_record_by_object">
-<span class="sig-name descname"><span class="pre">add_test_record_by_object</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_record</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">manual_state_change</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.add_test_record_by_object"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.add_test_record_by_object" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">add_test_record_by_object</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_record</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">manual_state_change</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_incident</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.add_test_record_by_object"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.add_test_record_by_object" title="Link to this definition">¶</a></dt>
 <dd><p>method add_test_record_by_object, adds a test record for the given
 test case based on the TestRecord object passed in.
 In addition, the test run is checked for completeness and the test
 run state will change accordingly.
-Test Run states are [“notrun”, “finished”, “inprogress”].</p>
+If possible, the status is set to one of
+[“notrun”, “finished”, “inprogress”].</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>test_record</strong> (<a class="reference internal" href="#pylero.test_record.TestRecord" title="pylero.test_record.TestRecord"><em>TestRecord</em></a><em> or </em><em>Polarion TestRecord</em>) – </p></li>
+<li><p><strong>test_record</strong> (<a class="reference internal" href="#pylero.test_record.TestRecord" title="pylero.test_record.TestRecord"><em>TestRecord</em></a><em> or </em><em>Polarion TestRecord</em>)</p></li>
 <li><p><strong>manual_state_change</strong> (<em>boolean</em>) – Change test run state
 automatically or manual.</p></li>
+<li><p><strong>create_incident</strong> (<em>boolean</em>) – Create an incident report if the test
+case fails and no incident is linked.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
@@ -5416,15 +5459,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.get_attachments">
 <span class="sig-name descname"><span class="pre">get_attachments</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.get_attachments"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.get_attachments" title="Link to this definition">¶</a></dt>
 <dd><p>method get_attachments returns all the attachments for the TestRun</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>ArrayOfTestRunAttachments object</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>test_management.getTestRunAttachments</p>
@@ -5470,15 +5513,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.get_wiki_content">
 <span class="sig-name descname"><span class="pre">get_wiki_content</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.get_wiki_content"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.get_wiki_content" title="Link to this definition">¶</a></dt>
 <dd><p>method get_wiki_content returns the wiki content for the Test Run</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Text object containing the wiki content</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>test_management.getWikiContentForTestRun</p>
@@ -5488,15 +5531,15 @@
 <dt class="sig sig-object py" id="id2">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">records</span></span><a class="headerlink" href="#id2" title="Link to this definition">¶</a></dt>
 <dd><p>function to return all the test records of a TestRun.
 The records array for dynamic queries/documents only includes executed
 records. This returns the unexecuted ones as well.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of TestRecords</p>
 </dd>
 </dl>
 </dd></dl>
 
@@ -5540,15 +5583,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.update">
 <span class="sig-name descname"><span class="pre">update</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.update"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.update" title="Link to this definition">¶</a></dt>
 <dd><p>method update updates the testRun object with the attribute values
 currently in the object.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>Returns</dt><dd><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
@@ -5639,27 +5682,31 @@
 add_test_record_by_fields function</p>
 <p class="rubric">References</p>
 <p>test_management.updateTestRecord</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.update_test_record_by_object">
-<span class="sig-name descname"><span class="pre">update_test_record_by_object</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_case_id</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_record</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">manual_state_change</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.update_test_record_by_object"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.update_test_record_by_object" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">update_test_record_by_object</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_case_id</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_record</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">manual_state_change</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_incident</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.update_test_record_by_object"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.update_test_record_by_object" title="Link to this definition">¶</a></dt>
 <dd><p>method update_test_record_by_object, adds a test record for the
 given test case based on the TestRecord object passed in.
 In addition, the test run is checked for completeness and the
 test run state will change accordingly.
-Test Run states are [“notrun”, “finished”, “inprogress”].</p>
+If possible, the status is set to one of
+[“notrun”, “finished”, “inprogress”].</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>test_case_id</strong> (<em>str</em>) – the test case id that the record is related to.</p></li>
-<li><p><strong>test_record</strong> (<a class="reference internal" href="#pylero.test_record.TestRecord" title="pylero.test_record.TestRecord"><em>TestRecord</em></a><em> or </em><em>Polarion TestRecord</em>) – </p></li>
+<li><p><strong>test_record</strong> (<a class="reference internal" href="#pylero.test_record.TestRecord" title="pylero.test_record.TestRecord"><em>TestRecord</em></a><em> or </em><em>Polarion TestRecord</em>)</p></li>
 <li><p><strong>manual_state_change</strong> (<em>boolean</em>) – Change the test
 run result automatically or manual.</p></li>
+<li><p><strong>create_incident</strong> (<em>boolean</em>) – Create an incident report if the test
+record result is failed and no defect
+case id is set.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
@@ -5668,15 +5715,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.test_run.TestRun.update_wiki_content">
 <span class="sig-name descname"><span class="pre">update_wiki_content</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">content</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#TestRun.update_wiki_content"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.TestRun.update_wiki_content" title="Link to this definition">¶</a></dt>
 <dd><p>method update_wiki_content updates the wiki for the current TestRun</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>Content</strong> (<em>str</em><em> or </em><em>Text object</em>) – </p>
+<dd class="field-odd"><p><strong>Content</strong> (<em>str</em><em> or </em><em>Text object</em>)</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>test_management.updateWikiContentForTestRun</p>
@@ -5707,24 +5754,14 @@
 <dt>Exceptions:</dt><dd><p>PyleroLibException - if required params are not passed in</p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
-<dl class="py function">
-<dt class="sig sig-object py" id="pylero.test_run.create_incident_report">
-<span class="sig-prename descclassname"><span class="pre">pylero.test_run.</span></span><span class="sig-name descname"><span class="pre">create_incident_report</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_run</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_record</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_case</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#create_incident_report"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.create_incident_report" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
-
-<dl class="py function">
-<dt class="sig sig-object py" id="pylero.test_run.generate_description">
-<span class="sig-prename descclassname"><span class="pre">pylero.test_run.</span></span><span class="sig-name descname"><span class="pre">generate_description</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">test_run</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_case</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">test_record</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run.html#generate_description"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run.generate_description" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
-
 </section>
 <section id="module-pylero.test_run_attachment">
 <span id="pylero-test-run-attachment-module"></span><h2>pylero.test_run_attachment module<a class="headerlink" href="#module-pylero.test_run_attachment" title="Link to this heading">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="pylero.test_run_attachment.ArrayOfTestRunAttachment">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">pylero.test_run_attachment.</span></span><span class="sig-name descname"><span class="pre">ArrayOfTestRunAttachment</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">obj_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">suds_object</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/test_run_attachment.html#ArrayOfTestRunAttachment"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.test_run_attachment.ArrayOfTestRunAttachment" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#pylero.base_polarion.BasePolarion" title="pylero.base_polarion.BasePolarion"><code class="xref py py-class docutils literal notranslate"><span class="pre">BasePolarion</span></code></a></p>
@@ -6446,15 +6483,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.user.User.get_roles">
 <span class="sig-name descname"><span class="pre">get_roles</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">location</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/user.html#User.get_roles"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.user.User.get_roles" title="Link to this definition">¶</a></dt>
 <dd><p>Returns all global and context roles for the context at given
 location assigned to the user.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>location</strong> – </p>
+<dd class="field-odd"><p><strong>location</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of roles</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.getRolesForUser</p>
@@ -6463,30 +6500,30 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.user.User.get_user_avatar_url">
 <span class="sig-name descname"><span class="pre">get_user_avatar_url</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/user.html#User.get_user_avatar_url"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.user.User.get_user_avatar_url" title="Link to this definition">¶</a></dt>
 <dd><p>method get_user_avatar_url, returns a string with the relative URL
 of the user’s avatar.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 </dl>
 <p class="rubric">Notes</p>
 <p>Raises an error if the User is not populated.</p>
 <p class="rubric">References</p>
 <p>Project.getUserAvatarURL</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.user.User.get_user_from_token">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">get_user_from_token</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">token</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/user.html#User.get_user_from_token"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.user.User.get_user_from_token" title="Link to this definition">¶</a></dt>
 <dd><p>Returns the username of the user that has the assigned token.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>token</strong> – </p>
+<dd class="field-odd"><p><strong>token</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>user_id</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Security.getUserFromToken</p>
@@ -6494,15 +6531,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.user.User.get_users">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">get_users</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/user.html#User.get_users"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.user.User.get_users" title="Link to this definition">¶</a></dt>
 <dd><p>class method that returns all the system users</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list containing User objects for all users.</p>
 </dd>
 </dl>
 <p class="rubric">References</p>
 <p>Project.getUsers</p>
@@ -6530,15 +6567,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pylero.user.User.update">
 <span class="sig-name descname"><span class="pre">update</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/pylero/user.html#User.update"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#pylero.user.User.update" title="Link to this definition">¶</a></dt>
 <dd><p>method update, updates Polarion with the User attributes</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>None</strong> – </p>
+<dd class="field-odd"><p><strong>None</strong></p>
 </dd>
 </dl>
 <p class="rubric">Notes</p>
 <p>Raises an error if the User is not populated.</p>
 <p class="rubric">References</p>
 <p>p.Project.updateUser</p>
 </dd></dl>
@@ -7350,16 +7387,14 @@
 <li class="toctree-l3"><a class="reference internal" href="#module-pylero.test_record">pylero.test_record module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#pylero.test_record.ArrayOfTestRecord"><code class="docutils literal notranslate"><span class="pre">ArrayOfTestRecord</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#pylero.test_record.TestRecord"><code class="docutils literal notranslate"><span class="pre">TestRecord</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#module-pylero.test_run">pylero.test_run module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#pylero.test_run.TestRun"><code class="docutils literal notranslate"><span class="pre">TestRun</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="#pylero.test_run.create_incident_report"><code class="docutils literal notranslate"><span class="pre">create_incident_report()</span></code></a></li>
-<li class="toctree-l4"><a class="reference internal" href="#pylero.test_run.generate_description"><code class="docutils literal notranslate"><span class="pre">generate_description()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="#module-pylero.test_run_attachment">pylero.test_run_attachment module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#pylero.test_run_attachment.ArrayOfTestRunAttachment"><code class="docutils literal notranslate"><span class="pre">ArrayOfTestRunAttachment</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#pylero.test_run_attachment.TestRunAttachment"><code class="docutils literal notranslate"><span class="pre">TestRunAttachment</span></code></a></li>
 </ul>
 </li>
@@ -7440,23 +7475,23 @@
   <li><a href="modules.html">pylero</a><ul>
       <li>Previous: <a href="modules.html" title="previous chapter">pylero</a></li>
       <li>Next: <a href="pylero.cli.html" title="next chapter">pylero.cli package</a></li>
   </ul></li>
   </ul></li>
 </ul>
 </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
@@ -7466,15 +7501,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
       |
       <a href="_sources/pylero.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -210,23 +210,23 @@
               Returns:
                   bool
             References
             Security.canAddElementToKey
         can_delete_instance()_[_s_o_u_r_c_e_]_¶
             Checks if the current user can delete the current object
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   bool
             References
             Security.canDeleteInstance
         can_modify_instance()_[_s_o_u_r_c_e_]_¶
             Checks if the current user can modify the current object
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   bool
             References
             Security.canModifyInstance
         can_modify_key(kkeeyy)_[_s_o_u_r_c_e_]_¶
             Checks if the current user can modify the field with given key of
             the current object.
@@ -235,15 +235,15 @@
               Returns:
                   bool
             References
             Security.canModifyKey
         can_read_instance()_[_s_o_u_r_c_e_]_¶
             Checks if the current user can read the current object
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   bool
             References
             Security.canReadInstance
         can_read_key(kkeeyy)_[_s_o_u_r_c_e_]_¶
             Checks if the current user can read the field with given key of the
             current object.
@@ -278,29 +278,46 @@
                         None
         custom_array_obj()_[_s_o_u_r_c_e_]_¶
         custom_obj()_[_s_o_u_r_c_e_]_¶
         default_project == ''PPOOLLAARRIIOONN__PPRROOJJEECCTT''_¶
         ccllaassssmmeetthhoodd get_global_roles()_[_s_o_u_r_c_e_]_¶
             Returns all global roles.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of global roles
             References
             Security._g_e_t_G_l_o_b_a_l_R_o_l_e_s_(_)
         get_location()_[_s_o_u_r_c_e_]_¶
             Returns the location of the current object. In the context of this
             service the method should be used to get the location of a project
             (-group).
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   location (string)
             References
             Security.getLocationForURI
+        get_revision(rreeppoossiittoorryy__nnaammee, rreevviissiioonn__iidd)_[_s_o_u_r_c_e_]_¶
+            Gets a revision :param repository_name - The repository name.: :
+            type repository_name - The repository name.: Put “default” for the
+            default repository. :param revision_id - The revision name.:
+              Returns:
+                  a Revision object
+        get_revision_by_uri(rreevviissiioonn__uurrii)_[_s_o_u_r_c_e_]_¶
+            Gets a revision by its URI :param revision_uri - The URI of the
+            revision.:
+              Returns:
+                  a Revision object
+        get_revisions(uurrii)_[_s_o_u_r_c_e_]_¶
+            Returns all revisions for a specific URI. :param uri - URI of the
+            persistence object: :type uri - URI of the persistence object: Work
+            Item, Module/Document, User, etc
+              Returns:
+                  All revisions for a specific URI.
         get_valid_field_values(eennuumm__iidd, ccoonnttrrooll==NNoonnee)_[_s_o_u_r_c_e_]_¶
             Gets the available enumeration options. Uses a cache dict because
             the time to get valid fields from server is time prohibitive.
               Parameters:
                       * eennuumm__iidd – The enum code to get values for
                       * ccoonnttrrooll – the control key for the enumeration. default:
                         None
@@ -315,56 +332,56 @@
                       * ppeerrmmiissssiioonn – the permission to check.
                       * pprroojjeecctt__iidd – the id of the project to check the
                         permission in, None to check global permissions.
               Returns:
                   bool
             References
             Security.hasCurrentUserPermission
-        logged_in_user_id == ''ggssuunn''_¶
+        logged_in_user_id == ''PPOOLLAARRIIOONN__UUSSEERRNNAAMMEE''_¶
         reload()_[_s_o_u_r_c_e_]_¶
             Reloads the object with data from the server. This function is
             useful if the data on the server changed or if a data changing
             function was called (such as TestRun.add_attachment)
             Notes
             This will overwrite any unsaved data in the object.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   None
-        repo == ''PPOOLLAARRIIOONN__UURRLL//rreeppoo''_¶
+        repo == ''hhttttppss::////ppoollaarriioonn..eennggiinneeeerriinngg..rreeddhhaatt..ccoomm//rreeppoo''_¶
         session == <<ppyylleerroo..sseessssiioonn..SSeessssiioonn oobbjjeecctt>>_¶
   ccllaassss pylero.base_polarion.ClassProperty(ffggeett==NNoonnee, ffsseett==NNoonnee, ffddeell==NNoonnee,
   ddoocc==NNoonnee)_[_s_o_u_r_c_e_]_¶
       Bases: property
       Returns a classmethod as the getter so that the property can be used as a
       class property. This is needed so that the property can be set for all
       child objects. This project currently has no need of a setter or deleter.
   ccllaassss pylero.base_polarion.Configuration_[_s_o_u_r_c_e_]_¶
       Bases: object
         CONFIG_SECTION == ''wweebbsseerrvviiccee''_¶
         CURDIR_CONFIG == ''..ppyylleerroo''_¶
-        GLOBAL_CONFIG == ''//hhoommee//wwaayynneessuunn//..llooccaall//sshhaarree//vviirrttuuaalleennvvss//ppyylleerroo--
-        xxZZ44TTBB22uuXX//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//ppyylleerroo//ppyylleerroo..ccffgg''_¶
-        LOCAL_CONFIG == ''//hhoommee//wwaayynneessuunn//..ppyylleerroo''_¶
+        GLOBAL_CONFIG == ''//hhoommee//wwaayynnee//..llooccaall//sshhaarree//vviirrttuuaalleennvvss//ppyylleerroo--mmnnlliizz99JJuu//
+        lliibb//ppyytthhoonn33..1122//ssiittee--ppaacckkaaggeess//ppyylleerroo//ppyylleerroo..ccffgg''_¶
+        LOCAL_CONFIG == ''//hhoommee//wwaayynnee//..ppyylleerroo''_¶
         __init__()_[_s_o_u_r_c_e_]_¶
-        pkgdir == ''//hhoommee//wwaayynneessuunn//..llooccaall//sshhaarree//vviirrttuuaalleennvvss//ppyylleerroo--xxZZ44TTBB22uuXX//lliibb//
-        ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//ppyylleerroo''_¶
+        pkgdir == ''//hhoommee//wwaayynnee//..llooccaall//sshhaarree//vviirrttuuaalleennvvss//ppyylleerroo--mmnnlliizz99JJuu//lliibb//
+        ppyytthhoonn33..1122//ssiittee--ppaacckkaaggeess//ppyylleerroo''_¶
   ccllaassss pylero.base_polarion.Connection_[_s_o_u_r_c_e_]_¶
       Bases: object
       Creates a Polarion session as a class method, so that it is used for all
       objects inherited by BasePolarion. The url, repo, user and password are
       read from config files, which are located either the current directory ./
       pylero, the user’s dir ~/.pylero or the Library config dir LIBDIR/
       pylero.cfg These can also be overridden with the following environment
       variables: POLARION_URL POLARION_REPO POLARION_USERNAME POLARION_PASSWORD
       POLARION_TOKEN POLARION_TIMEOUT POLARION_PROJECT
         connected == TTrruuee_¶
         retries == 33_¶
         session == <<ppyylleerroo..sseessssiioonn..SSeessssiioonn oobbjjeecctt>>_¶
-        token_enabled == TTrruuee_¶
+        token_enabled == FFaallssee_¶
   pylero.base_polarion.tx_wrapper(ffuunncc)_[_s_o_u_r_c_e_]_¶
 ********** ppyylleerroo..bbaasseelliinnee mmoodduullee_?¶ **********
   ccllaassss pylero.baseline.Baseline(oobbjj__iidd==NNoonnee, ssuuddss__oobbjjeecctt==NNoonnee)_[_s_o_u_r_c_e_]_¶
       Bases: _B_a_s_e_P_o_l_a_r_i_o_n
       Object to handle the Polarion WSDL tns3:Baseline class
         author_¶
               Type:
@@ -384,15 +401,15 @@
         project_¶
               Type:
                   _P_r_o_j_e_c_t
         ccllaassssmmeetthhoodd create(pprroojjeecctt__iidd, nnaammee, ddeessccrriippttiioonn, rreevviissiioonn)_[_s_o_u_r_c_e_]_¶
             class method create Creates a Baseline from head or particular
             revision.
               Parameters:
-                      * pprroojjeecctt__iidd –
+                      * pprroojjeecctt__iidd
                       * nnaammee – baseline name (not None)
                       * ddeessccrriippttiioonn – baseline description (can be None)
                       * rreevviissiioonn – revision or null value for head revision
               Returns:
                   Baseline object
             References
             Tracker.createBaseline
@@ -735,15 +752,15 @@
             Tracker.getModuleByUri Tracker.getModuleByUriWithFields
         add_referenced_work_item(wwoorrkk__iitteemm__iidd)_[_s_o_u_r_c_e_]_¶
             Adds a work item to the document as a referenced work_item to the
             end of the current document.
               Parameters:
                       * wwoorrkk__iitteemm__iidd (ssttrr) – the id of a work item in the same
                         project as
-                      * ddooccuummeenntt (tthhee ccuurrrreenntt) –
+                      * ddooccuummeenntt (tthhee ccuurrrreenntt)
               Returns:
                   None
         ccllaassssmmeetthhoodd create(pprroojjeecctt__iidd, ssppaaccee, ddooccuummeenntt__nnaammee, ddooccuummeenntt__ttiittllee,
         aalllloowweedd__wwii__ttyyppeess, ddooccuummeenntt__ttyyppee, ssttrruuccttuurree__lliinnkk__rroollee==''ppaarreenntt'',
         hhoommee__ppaaggee__ccoonntteenntt=='''')_[_s_o_u_r_c_e_]_¶
             class method create Creates a document or an old-style Module/
             Document in given location with given parameters.
@@ -774,15 +791,15 @@
               Returns:
                   The created _WorkItem
             References
             Tracker.createWorkItemInModule
         delete()_[_s_o_u_r_c_e_]_¶
             delete the current document
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   None
         ccllaassssmmeetthhoodd export_pdf(uurrii, eexxppoorrttPPddffPPrrooppeerrttiieess, oouuttppuutt__ddiirr==''//ttmmpp'',
         oouuttppuutt__nnaammee=='''')_[_s_o_u_r_c_e_]_¶
             Export a document to PDF and download it
               Parameters:
                       * uurrii – Module/Document URI
@@ -877,15 +894,15 @@
             References
             queryModuleUris queryModuleUrisBySQL queryModuleUrisInBaseline
             queryModuleUrisInBaselineBySQL queryModules queryModulesBySQL
             queryModulesInBaseline queryModulesInBaselineBySQL
         update()_[_s_o_u_r_c_e_]_¶
             updates the server with the current module data
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   None
             References
             Tracker.updateModule
 ********** ppyylleerroo..eennuumm__ccuussttoomm__ffiieelldd__ttyyppee mmoodduullee_?¶ **********
   ccllaassss pylero.enum_custom_field_type.EnumCustomFieldType(oobbjj__iidd==NNoonnee,
   ssuuddss__oobbjjeecctt==NNoonnee)_[_s_o_u_r_c_e_]_¶
@@ -1248,23 +1265,23 @@
               Returns:
                   None
             References
             Planning.deletePlans
         get_statistics()_[_s_o_u_r_c_e_]_¶
             get statistics of the plan
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   PlanStatistics object
             References
             Planning.getPlanStatistics
         get_wiki_content()_[_s_o_u_r_c_e_]_¶
             Returns the wiki content of the plan
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   Text object
             References
             Planning.getPlanWikiContent
         remove_plan_items(wwoorrkk__iitteemmss)_[_s_o_u_r_c_e_]_¶
             Remove plan records to the plan.
               Parameters:
@@ -1284,31 +1301,31 @@
                   list of Plan objects
             References
             Planning.searchPlanTemplates Planning.searchPlanTemplatesWithFields
             Planning.searchPlans Planning.searchPlansWithFields
         set_wiki_content(ccoonntteenntt)_[_s_o_u_r_c_e_]_¶
             method set_wiki_content updates the wiki for the current Plan
               Parameters:
-                  CCoonntteenntt (ssttrr oorr TTeexxtt oobbjjeecctt) –
+                  CCoonntteenntt (ssttrr oorr TTeexxtt oobbjjeecctt)
               Returns:
                   None
             References
             Planning.setPlanWikiContent
         update()_[_s_o_u_r_c_e_]_¶
             updates the server with the current plan content
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   None
             References
             Planning.updatePlan
         was_started()_[_s_o_u_r_c_e_]_¶
             checks if the plan was started yet
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   bool
             References
             Planning.wasPlanStarted
 ********** ppyylleerroo..ppllaann__rreeccoorrdd mmoodduullee_?¶ **********
   ccllaassss pylero.plan_record.ArrayOfPlanRecord(oobbjj__iidd==NNoonnee, ssuuddss__oobbjjeecctt==NNoonnee)
   _[_s_o_u_r_c_e_]_¶
@@ -1526,15 +1543,15 @@
             passed in an empty object is created
             References
             Project.getProject Project.getProjectAtLocation
             Project.getProjectByURI
         get_categories()_[_s_o_u_r_c_e_]_¶
             method get_categories retrieves a list of Category objects
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of Category objects
             References
             Tracker.getCategories
         ccllaassssmmeetthhoodd get_context_roles(llooccaattiioonn)_[_s_o_u_r_c_e_]_¶
             Returns the context (project) roles for the given location.
               Parameters:
@@ -1571,49 +1588,49 @@
               Returns:
                   list of CustomFieldType object
             References
             Tracker.getDefinedCustomFieldType
         get_document_spaces()_[_s_o_u_r_c_e_]_¶
             Gets the Module/Document spaces for the project.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of (string) document spaces
             References
             Tracker.getDocumentSpaces
         get_project_users()_[_s_o_u_r_c_e_]_¶
             Gets users of the project
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of u.User objects
             References
             Project.getProjectUsers
         get_test_steps_configuration()_[_s_o_u_r_c_e_]_¶
             method get_test_steps_configuration retrieves a list of the Test
             Steps configuration for the project
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of configuration of the Test Steps custom field.
             References
             TestManagement.getTestStepsConfiguration
         get_tests_configuration()_[_s_o_u_r_c_e_]_¶
             method get_tests_configuration retrieves the test management
             configuration for the project
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   TestsConfiguration object
             References
             TestManagement.getTestsConfiguration
         get_wiki_spaces()_[_s_o_u_r_c_e_]_¶
             Returns Wiki spaces from current project
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   Array of string
             References
             Tracker.getWikiSpaces
 ********** ppyylleerroo..pprroojjeecctt__ggrroouupp mmoodduullee_?¶ **********
   ccllaassss pylero.project_group.ProjectGroup(uurrii==NNoonnee, llooccaattiioonn==NNoonnee,
   ssuuddss__oobbjjeecctt==NNoonnee)_[_s_o_u_r_c_e_]_¶
@@ -1646,39 +1663,39 @@
             of the identifying parameters are passed in an empty object is
             created
             References
             p.Project.getProjectGroup p.Project.getProjectGroupAtLocation
         get_contained_groups()_[_s_o_u_r_c_e_]_¶
             Gets all project groups located directly below the project group.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of p.ProjectGroup objects
             References
             p.Project.getContainedGroups
         get_contained_projects()_[_s_o_u_r_c_e_]_¶
             Gets all projects located directly below the project group.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of p.Project objects
             References
             p.Project.getContainedProjects
         get_deep_contained_projects()_[_s_o_u_r_c_e_]_¶
             Gets all projects located below the project group.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of p.Project objects
             References
             p.Project.getDeepContainedProjects
         ccllaassssmmeetthhoodd get_root_project_group()_[_s_o_u_r_c_e_]_¶
             Gets the root project group.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   ProjectGroup object
             References
             Project.getRootProjectGroup
 ********** ppyylleerroo..pprrooppeerrttiieess mmoodduullee_?¶ **********
   ccllaassss pylero.properties.Properties(oobbjj__iidd==NNoonnee, ssuuddss__oobbjjeecctt==NNoonnee)_[_s_o_u_r_c_e_]_¶
       Bases: _B_a_s_e_P_o_l_a_r_i_o_n
@@ -2007,42 +2024,45 @@
             number of steps.
             References
             test_management.addAttachmentToTestStep
         add_test_record_by_fields(tteesstt__ccaassee__iidd, tteesstt__rreessuulltt, tteesstt__ccoommmmeenntt,
         eexxeeccuutteedd__bbyy, eexxeeccuutteedd, dduurraattiioonn, ddeeffeecctt__wwoorrkk__iitteemm__iidd==NNoonnee)_[_s_o_u_r_c_e_]_¶
             method add_test_record_by_fields, adds a test record for the given
             test case based on the result fields passed in. When a test record
-            is added, it changes the test run status to “inprogress” and when
-            the last test record is run, it changes the status to done.
+            is added and the valid options for status contain “inprogress” and
+            “finished”, it changes the test run status to “inprogress” and when
+            the last test record is run, it changes the status to “finished”.
               Parameters:
                       * tteesstt__ccaassee__iidd (ssttrr) – The id of the test case that was
                         executed
                       * tteesstt__rreessuulltt (ssttrr) – Must be one of the following
                         values: passed failed blocked
                       * tteesstt__ccoommmmeenntt (ssttrr oorr TTeexxtt oobbjjeecctt) – may be None
                       * eexxeeccuutteedd__bbyy (ssttrr) – user id
-                      * eexxeeccuutteedd (ddaatteettiimmee) –
-                      * dduurraattiioonn (ffllooaatt) –
+                      * eexxeeccuutteedd (ddaatteettiimmee)
+                      * dduurraattiioonn (ffllooaatt)
                       * ddeeffeecctt__wwoorrkk__iitteemm__iidd (ssttrr) – _WorkItem id of defect,
                         default: None
               Returns:
                   None
             References
             test_management.addTestRecordToTestRun
-        add_test_record_by_object(tteesstt__rreeccoorrdd, mmaannuuaall__ssttaattee__cchhaannggee==FFaallssee)
-        _[_s_o_u_r_c_e_]_¶
+        add_test_record_by_object(tteesstt__rreeccoorrdd, mmaannuuaall__ssttaattee__cchhaannggee==FFaallssee,
+        ccrreeaattee__iinncciiddeenntt==TTrruuee)_[_s_o_u_r_c_e_]_¶
             method add_test_record_by_object, adds a test record for the given
             test case based on the TestRecord object passed in. In addition,
             the test run is checked for completeness and the test run state
-            will change accordingly. Test Run states are [“notrun”, “finished”,
-            “inprogress”].
+            will change accordingly. If possible, the status is set to one of
+            [“notrun”, “finished”, “inprogress”].
               Parameters:
-                      * tteesstt__rreeccoorrdd (_TT_ee_ss_tt_RR_ee_cc_oo_rr_dd oorr PPoollaarriioonn TTeessttRReeccoorrdd) –
+                      * tteesstt__rreeccoorrdd (_TT_ee_ss_tt_RR_ee_cc_oo_rr_dd oorr PPoollaarriioonn TTeessttRReeccoorrdd)
                       * mmaannuuaall__ssttaattee__cchhaannggee (bboooolleeaann) – Change test run state
                         automatically or manual.
+                      * ccrreeaattee__iinncciiddeenntt (bboooolleeaann) – Create an incident report
+                        if the test case fails and no incident is linked.
               Returns:
                   None
             References
             test_management.addTestRecordToTestRun
         ccllaassssmmeetthhoodd create(pprroojjeecctt__iidd, tteesstt__rruunn__iidd==NNoonnee, tteemmppllaattee==NNoonnee,
         ttiittllee==NNoonnee, ****kkwwaarrggss)_[_s_o_u_r_c_e_]_¶
             class method create for creating a new test run in Polarion
@@ -2146,15 +2166,15 @@
               Returns:
                   TestRunAttachment object
             References
             test_management.getTestRunAttachment
         get_attachments()_[_s_o_u_r_c_e_]_¶
             method get_attachments returns all the attachments for the TestRun
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   ArrayOfTestRunAttachments object
             References
             test_management.getTestRunAttachments
         get_custom_field(ffiieelldd__nnaammee)_[_s_o_u_r_c_e_]_¶
             gets custom field values.
               Parameters:
@@ -2174,25 +2194,25 @@
               Returns:
                   list of all the custom fields
             References
             testmanagement.getDefinedTestRunCustomFieldTypes
         get_wiki_content()_[_s_o_u_r_c_e_]_¶
             method get_wiki_content returns the wiki content for the Test Run
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   Text object containing the wiki content
             References
             test_management.getWikiContentForTestRun
         pprrooppeerrttyy records_¶
             function to return all the test records of a TestRun. The records
             array for dynamic queries/documents only includes executed records.
             This returns the unexecuted ones as well.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list of TestRecords
         ccllaassssmmeetthhoodd search(qquueerryy, ffiieellddss==[[''tteesstt__rruunn__iidd'']], ssoorrtt==''tteesstt__rruunn__iidd'',
         lliimmiitt==NNoonnee, sseeaarrcchh__tteemmppllaatteess==FFaallssee, pprroojjeecctt__iidd==NNoonnee)_[_s_o_u_r_c_e_]_¶
             class method search executes the given query and returns the
             results
               Parameters:
@@ -2220,15 +2240,15 @@
             test_management.searchTestRuns test_management.searchTestRunLimited
             test_management.searchTestRunsWithFields
             test_management.searchTestRunsWithFieldsLimited
         update()_[_s_o_u_r_c_e_]_¶
             method update updates the testRun object with the attribute values
             currently in the object.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns
                   None
             References
             test_management.updateTestRun
         update_attachment(ppaatthh, oorriiggiinnaall__ffiilleennaammee, ttiittllee)_[_s_o_u_r_c_e_]_¶
             method update_attachment updates the specified attachment to the
             current test run
@@ -2282,34 +2302,37 @@
             Notes
             Only a test case that has already been executed may be updated
             using this function. To execute a test record use the
             add_test_record_by_fields function
             References
             test_management.updateTestRecord
         update_test_record_by_object(tteesstt__ccaassee__iidd, tteesstt__rreeccoorrdd,
-        mmaannuuaall__ssttaattee__cchhaannggee==FFaallssee)_[_s_o_u_r_c_e_]_¶
+        mmaannuuaall__ssttaattee__cchhaannggee==FFaallssee, ccrreeaattee__iinncciiddeenntt==TTrruuee)_[_s_o_u_r_c_e_]_¶
             method update_test_record_by_object, adds a test record for the
             given test case based on the TestRecord object passed in. In
             addition, the test run is checked for completeness and the test run
-            state will change accordingly. Test Run states are [“notrun”,
-            “finished”, “inprogress”].
+            state will change accordingly. If possible, the status is set to
+            one of [“notrun”, “finished”, “inprogress”].
               Parameters:
                       * tteesstt__ccaassee__iidd (ssttrr) – the test case id that the record
                         is related to.
-                      * tteesstt__rreeccoorrdd (_TT_ee_ss_tt_RR_ee_cc_oo_rr_dd oorr PPoollaarriioonn TTeessttRReeccoorrdd) –
+                      * tteesstt__rreeccoorrdd (_TT_ee_ss_tt_RR_ee_cc_oo_rr_dd oorr PPoollaarriioonn TTeessttRReeccoorrdd)
                       * mmaannuuaall__ssttaattee__cchhaannggee (bboooolleeaann) – Change the test run
                         result automatically or manual.
+                      * ccrreeaattee__iinncciiddeenntt (bboooolleeaann) – Create an incident report
+                        if the test record result is failed and no defect case
+                        id is set.
               Returns:
                   None
             References
             test_management.updateTestRecordAtIndex
         update_wiki_content(ccoonntteenntt)_[_s_o_u_r_c_e_]_¶
             method update_wiki_content updates the wiki for the current TestRun
               Parameters:
-                  CCoonntteenntt (ssttrr oorr TTeexxtt oobbjjeecctt) –
+                  CCoonntteenntt (ssttrr oorr TTeexxtt oobbjjeecctt)
               Returns:
                   None
             References
             test_management.updateWikiContentForTestRun
         verify_params(****kkwwaarrggss)_[_s_o_u_r_c_e_]_¶
             function that checks if all the kwargs are valid attributes.
               Parameters:
@@ -2318,18 +2341,14 @@
                   passed in
               Exceptions:
                   PyleroLibException - if params are unknown
         verify_required()_[_s_o_u_r_c_e_]_¶
             function that checks if all required fields are passed in
               Exceptions:
                   PyleroLibException - if required params are not passed in
-  pylero.test_run.create_incident_report(tteesstt__rruunn, tteesstt__rreeccoorrdd, tteesstt__ccaassee)
-  _[_s_o_u_r_c_e_]_¶
-  pylero.test_run.generate_description(tteesstt__rruunn, tteesstt__ccaassee, tteesstt__rreeccoorrdd)
-  _[_s_o_u_r_c_e_]_¶
 ********** ppyylleerroo..tteesstt__rruunn__aattttaacchhmmeenntt mmoodduullee_?¶ **********
   ccllaassss pylero.test_run_attachment.ArrayOfTestRunAttachment(oobbjj__iidd==NNoonnee,
   ssuuddss__oobbjjeecctt==NNoonnee)_[_s_o_u_r_c_e_]_¶
       Bases: _B_a_s_e_P_o_l_a_r_i_o_n
   ccllaassss pylero.test_run_attachment.TestRunAttachment(oobbjj__iidd==NNoonnee,
   ssuuddss__oobbjjeecctt==NNoonnee)_[_s_o_u_r_c_e_]_¶
       Bases: _B_a_s_e_P_o_l_a_r_i_o_n
@@ -2574,40 +2593,40 @@
                   list of roles
             References
             Security.getContextRolesForUser
         get_roles(llooccaattiioonn)_[_s_o_u_r_c_e_]_¶
             Returns all global and context roles for the context at given
             location assigned to the user.
               Parameters:
-                  llooccaattiioonn –
+                  llooccaattiioonn
               Returns:
                   list of roles
             References
             Security.getRolesForUser
         get_user_avatar_url()_[_s_o_u_r_c_e_]_¶
             method get_user_avatar_url, returns a string with the relative URL
             of the user’s avatar.
               Parameters:
-                  NNoonnee –
+                  NNoonnee
             Notes
             Raises an error if the User is not populated.
             References
             Project.getUserAvatarURL
         ccllaassssmmeetthhoodd get_user_from_token(ttookkeenn)_[_s_o_u_r_c_e_]_¶
             Returns the username of the user that has the assigned token.
               Parameters:
-                  ttookkeenn –
+                  ttookkeenn
               Returns:
                   user_id
             References
             Security.getUserFromToken
         ccllaassssmmeetthhoodd get_users()_[_s_o_u_r_c_e_]_¶
             class method that returns all the system users
               Parameters:
-                  NNoonnee –
+                  NNoonnee
               Returns:
                   list containing User objects for all users.
             References
             Project.getUsers
         has_permission(ppeerrmmiissssiioonn, pprroojjeecctt__iidd)_[_s_o_u_r_c_e_]_¶
             Checks if given permission is granted to the user.
               Parameters:
@@ -2617,15 +2636,15 @@
               Returns:
                   bool
             References
             Security.hasPermission
         update()_[_s_o_u_r_c_e_]_¶
             method update, updates Polarion with the User attributes
               Parameters:
-                  NNoonnee –
+                  NNoonnee
             Notes
             Raises an error if the User is not populated.
             References
             p.Project.updateUser
 ********** ppyylleerroo..wwiikkii__ppaaggee mmoodduullee_?¶ **********
   ccllaassss pylero.wiki_page.WikiPage(ffiieellddss==NNoonnee, uurrii==NNoonnee, ssuuddss__oobbjjeecctt==NNoonnee)
   _[_s_o_u_r_c_e_]_¶
@@ -2968,16 +2987,14 @@
                       # _A_r_r_a_y_O_f_S_u_b_t_e_r_r_a_U_R_I
                       # _S_u_b_t_e_r_r_a_U_R_I
                 # _p_y_l_e_r_o_._t_e_s_t___r_e_c_o_r_d_ _m_o_d_u_l_e
                       # _A_r_r_a_y_O_f_T_e_s_t_R_e_c_o_r_d
                       # _T_e_s_t_R_e_c_o_r_d
                 # _p_y_l_e_r_o_._t_e_s_t___r_u_n_ _m_o_d_u_l_e
                       # _T_e_s_t_R_u_n
-                      # _c_r_e_a_t_e___i_n_c_i_d_e_n_t___r_e_p_o_r_t_(_)
-                      # _g_e_n_e_r_a_t_e___d_e_s_c_r_i_p_t_i_o_n_(_)
                 # _p_y_l_e_r_o_._t_e_s_t___r_u_n___a_t_t_a_c_h_m_e_n_t_ _m_o_d_u_l_e
                       # _A_r_r_a_y_O_f_T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
                       # _T_e_s_t_R_u_n_A_t_t_a_c_h_m_e_n_t
                 # _p_y_l_e_r_o_._t_e_s_t___s_t_e_p_ _m_o_d_u_l_e
                       # _A_r_r_a_y_O_f_T_e_s_t_S_t_e_p
                       # _T_e_s_t_S_t_e_p
                 # _p_y_l_e_r_o_._t_e_s_t___s_t_e_p___r_e_s_u_l_t_ _m_o_d_u_l_e
@@ -3020,9 +3037,9 @@
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o _p_y_l_e_r_o
                 # Previous: _p_y_l_e_r_o
                 # Next: _p_y_l_e_r_o_._c_l_i_ _p_a_c_k_a_g_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6 | _P_a_g_e_ _s_o_u_r_c_e
```

### Comparing `pylero-0.0.9/docs/search.html` & `pylero-0.1.0/docs/search.html`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,23 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Search &#8212; pylero  documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     
     <script src="_static/documentation_options.js?v=5929fcd5"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
-  <script src="searchindex.js" defer></script>
-  
+    <script src="searchindex.js" defer="defer"></script>
+    <meta name="robots" content="noindex" />
+    
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
 
   
   
 
@@ -56,18 +57,15 @@
   <form action="" method="get">
     <input type="text" name="q" aria-labelledby="search-documentation" value="" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
     <input type="submit" value="search" />
     <span id="search-progress" style="padding-left: 10px"></span>
   </form>
   
   
-  
-  <div id="search-results">
-  
-  </div>
+  <div id="search-results"></div>
   
 
           </div>
           
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
@@ -105,15 +103,15 @@
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &#169;2021, Sim Zacks and Pylero Contributors.
       
       |
-      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.2.6</a>
+      Powered by <a href="https://www.sphinx-doc.org/">Sphinx 7.3.7</a>
       &amp; <a href="https://alabaster.readthedocs.io">Alabaster 0.7.16</a>
       
     </div>
```

#### html2text {}

```diff
@@ -3,9 +3,9 @@
 Searching for multiple words only shows matches that contain all words.
 [q                   ][search]
 ************ _pp_yy_ll_ee_rr_oo ************
 ******** NNaavviiggaattiioonn ********
     * _p_y_l_e_r_o
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
-©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._2_._6 & _A_l_a_b_a_s_t_e_r
+©2021, Sim Zacks and Pylero Contributors. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r
 _0_._7_._1_6
```

### Comparing `pylero-0.0.9/docs/searchindex.js` & `pylero-0.1.0/docs/searchindex.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,2497 +1,68 @@
 Search.setIndex({
-    "docnames": ["index", "modules", "pylero", "pylero.cli"],
-    "filenames": ["index.rst", "modules.rst", "pylero.rst", "pylero.cli.rst"],
-    "titles": ["Welcome to pylero\u2019s documentation!", "pylero", "pylero package", "pylero.cli package"],
-    "terms": {
-        "python": [0, 2],
-        "wrapper": 0,
-        "polarion": [0, 2],
-        "wsdl": [0, 2],
-        "api": [0, 2],
-        "The": [0, 2],
-        "enabl": [0, 2],
-        "nativ": 0,
-        "access": [0, 2],
-        "object": [0, 2, 3],
-        "function": [0, 2],
-        "us": [0, 2],
-        "orient": [0, 2],
-        "structur": [0, 2],
-        "thi": [0, 2],
-        "allow": [0, 2],
-        "develop": [0, 2],
-        "natur": 0,
-        "fashion": 0,
-        "without": [0, 2],
-        "being": 0,
-        "concern": 0,
-        "about": [0, 2],
-        "detail": [0, 2],
-        "all": [0, 2],
-        "inherit": [0, 2],
-        "basepolarion": [0, 1, 2],
-        "librari": [0, 2],
-        "ar": [0, 2],
-        "gener": [0, 2],
-        "soap": [0, 2],
-        "factori": 0,
-        "class": [0, 2, 3],
-        "sud": [0, 2],
-        "attribut": [0, 2],
-        "dynam": [0, 2],
-        "properti": [0, 1],
-        "base": [0, 2, 3],
-        "map": [0, 2],
-        "dict": [0, 2],
-        "between": 0,
-        "name": [0, 1, 2],
-        "convent": 0,
-        "virtual": 0,
-        "need": [0, 2],
-        "sync": 0,
-        "them": [0, 2],
-        "thei": 0,
-        "doe": [0, 2],
-        "implement": 0,
-        "valid": [0, 2],
-        "verif": [0, 2],
-        "data": [0, 2],
-        "pass": [0, 2],
-        "so": [0, 2],
-        "take": 0,
-        "care": 0,
-        "itself": 0,
-        "enum": [0, 2],
-        "sent": [0, 2],
-        "server": [0, 1],
-        "rais": [0, 2],
-        "an": [0, 2, 3],
-        "error": [0, 2],
-        "valu": [0, 1, 2],
-        "A": 0,
-        "number": [0, 2],
-        "workflow": 0,
-        "also": [0, 2],
-        "includ": [0, 2],
-        "when": [0, 2],
-        "creat": [0, 1, 2],
-        "automat": [0, 2],
-        "head": [0, 2],
-        "work": [0, 2],
-        "item": [0, 1, 2],
-        "same": [0, 2],
-        "time": [0, 1, 2],
-        "per": [0, 2],
-        "give": [0, 2],
-        "workitem": [0, 2, 3],
-        "testcas": [0, 1, 2, 3],
-        "connect": [0, 1, 2],
-        "download": [0, 2],
-        "list": [0, 2, 3],
-        "have": [0, 2],
-        "been": [0, 2],
-        "publish": [0, 2],
-        "http": [0, 2],
-        "org": 0,
-        "project": [0, 1],
-        "pip": 0,
-        "By": 0,
-        "default": [0, 1, 2],
-        "latest": 0,
-        "depend": 0,
-        "i": [0, 2],
-        "locat": [0, 1, 2],
-        "git": 0,
-        "repositori": [0, 2],
-        "can": [0, 2],
-        "clone": 0,
-        "github": 0,
-        "com": [0, 2],
-        "redhatq": 0,
-        "root": [0, 2],
-        "run": [0, 2, 3],
-        "If": [0, 2],
-        "rhel": 0,
-        "yum": 0,
-        "python3": [0, 2],
-        "could": 0,
-        "rpmbuild": 0,
-        "spec": 0,
-        "must": [0, 2],
-        "see": [0, 2],
-        "next": 0,
-        "section": 0,
-        "file": [0, 2],
-        "fill": [0, 2],
-        "out": 0,
-        "which": [0, 2],
-        "either": [0, 2],
-        "current": [0, 2],
-        "dir": [0, 2],
-        "where": [0, 2],
-        "script": 0,
-        "execut": [0, 2],
-        "user": [0, 1, 3],
-        "home": [0, 2],
-        "set": [0, 2],
-        "store": 0,
-        "libdir": [0, 2],
-        "etc": 0,
-        "cfg": [0, 2],
-        "should": [0, 2],
-        "modifi": [0, 2],
-        "overwritten": 0,
-        "ani": [0, 2],
-        "futur": 0,
-        "updat": [0, 1, 2, 3],
-        "certif": [0, 2],
-        "verifi": [0, 2],
-        "aren": 0,
-        "t": 0,
-        "add": [0, 2],
-        "path": [0, 2],
-        "your": 0,
-        "ca": [0, 2],
-        "cert_path": [0, 2],
-        "config": [0, 2],
-        "option": [0, 2],
-        "These": [0, 2],
-        "webservic": [0, 2],
-        "url": [0, 1, 2],
-        "web": 0,
-        "svn_repo": 0,
-        "usernam": [0, 2],
-        "password": [0, 2],
-        "token": [0, 2],
-        "person": 0,
-        "default_project": [0, 1, 2],
-        "my": 0,
-        "cert": 0,
-        "given": [0, 2],
-        "login": [0, 2],
-        "els": [0, 2],
-        "both": 0,
-        "provid": [0, 2],
-        "blank": [0, 2],
-        "prompt": 0,
-        "none": [0, 2, 3],
-        "overridden": [0, 2],
-        "follow": [0, 2],
-        "environ": [0, 2],
-        "variabl": [0, 2],
-        "polarion_url": [0, 2],
-        "polarion_repo": [0, 2],
-        "polarion_usernam": [0, 2],
-        "polarion_password": [0, 2],
-        "polarion_token": [0, 2],
-        "polarion_timeout": [0, 2],
-        "polarion_project": [0, 2],
-        "polarion_cert_path": 0,
-        "install_requir": 0,
-        "setup": 0,
-        "py": 0,
-        "request": [0, 2],
-        "2": [0, 2],
-        "6": 0,
-        "0": [0, 2],
-        "click": 0,
-        "readlin": 0,
-        "python_vers": 0,
-        "3": [0, 2],
-        "There": 0,
-        "txt": 0,
-        "directori": [0, 2],
-        "r": 0,
-        "open": 0,
-        "shell": 0,
-        "alreadi": [0, 2],
-        "load": [0, 2],
-        "tr": 0,
-        "testrun": [0, 1, 2],
-        "project_id": [0, 1, 2],
-        "project_nam": 0,
-        "altern": 0,
-        "import": 0,
-        "want": [0, 2],
-        "r266": 0,
-        "84292": 0,
-        "nov": 0,
-        "21": 0,
-        "2013": 0,
-        "10": [0, 2],
-        "50": 0,
-        "32": 0,
-        "gcc": 0,
-        "4": 0,
-        "7": [0, 2],
-        "20120313": 0,
-        "red": 0,
-        "hat": 0,
-        "linux2": 0,
-        "type": [0, 1, 2],
-        "help": [0, 2],
-        "copyright": 0,
-        "credit": 0,
-        "licens": [0, 1, 2],
-        "more": 0,
-        "inform": 0,
-        "test_run": [0, 1],
-        "possibl": [0, 2],
-        "mention": 0,
-        "mai": [0, 2],
-        "exactli": 0,
-        "match": 0,
-        "wa": [0, 2],
-        "In": [0, 2],
-        "those": 0,
-        "case": [0, 2],
-        "fail": [0, 2],
-        "overcom": 0,
-        "reach": 0,
-        "admin": 0,
-        "know": 0,
-        "find": [0, 2],
-        "below": [0, 2],
-        "code": [0, 2],
-        "work_item": [0, 1],
-        "global": [0, 2],
-        "dict_valu": 0,
-        "testsuit": [0, 1, 2],
-        "businesscas": [0, 1, 2],
-        "changerequest": [0, 1, 2],
-        "incidentreport": [0, 1, 2],
-        "defect": [0, 1, 2],
-        "task": [0, 1, 2],
-        "risk": [0, 1, 2],
-        "note": [0, 2],
-        "onli": [0, 2],
-        "onc": [0, 2],
-        "start": [0, 1, 2],
-        "don": 0,
-        "usual": 0,
-        "chang": [0, 1],
-        "abov": 0,
-        "ex": 0,
-        "tescas": 0,
-        "me": 0,
-        "differ": [0, 2],
-        "return": [0, 2],
-        "datetim": [0, 2],
-        "test_record": [0, 1],
-        "testrecord": [0, 1, 2],
-        "test": [0, 2],
-        "templat": [0, 1, 2, 3],
-        "create_templ": [0, 1, 2],
-        "myproj": 0,
-        "static": 0,
-        "queri": [0, 1, 2, 3],
-        "parent_template_id": [0, 2],
-        "empti": [0, 1, 2],
-        "select_test_cases_bi": [0, 1, 2],
-        "staticqueryresult": 0,
-        "AND": 0,
-        "statu": [0, 1, 2, 3],
-        "approv": [0, 1],
-        "inprogress": [0, 2],
-        "get": [0, 2],
-        "custom": [0, 1],
-        "arch": 0,
-        "get_custom_field": [0, 1, 2],
-        "i386": 0,
-        "set_custom_field": 0,
-        "save": 0,
-        "ad": [0, 1, 2],
-        "record": [0, 1, 2],
-        "add_test_record_by_field": [0, 1, 2],
-        "test_case_id": [0, 2],
-        "1813": 0,
-        "test_result": [0, 2],
-        "test_com": [0, 2],
-        "went": 0,
-        "smoothli": 0,
-        "executed_bi": [0, 2],
-        "user1": 0,
-        "now": 0,
-        "durat": [0, 2],
-        "defect_work_item_id": [0, 2],
-        "1824": 0,
-        "specif": [0, 2],
-        "tc": 0,
-        "work_item_id": [0, 1, 2],
-        "2015": 0,
-        "req": 0,
-        "2019": 0,
-        "field": [0, 2],
-        "custom_field": [0, 1],
-        "1": [0, 2],
-        "u": [0, 2],
-        "caseimport": 0,
-        "caselevel": 0,
-        "caseautom": 0,
-        "caseposneg": 0,
-        "reqtyp": 0,
-        "enumer": [0, 2],
-        "get_valid_field_valu": [0, 1, 2],
-        "critic": 0,
-        "high": 0,
-        "medium": 0,
-        "low": 0,
-        "titl": [0, 1, 2],
-        "descript": [0, 1, 2, 3],
-        "compon": [0, 2],
-        "notautom": 0,
-        "posit": [0, 2],
-        "specifi": [0, 2],
-        "except": [0, 1],
-        "like": 0,
-        "regular": 0,
-        "doc": [0, 2, 3],
-        "document_typ": [0, 2],
-        "testspecif": [0, 2],
-        "wi": [0, 2],
-        "tcmscaseid": 0,
-        "12345": 0,
-        "gui": 0,
-        "host": 0,
-        "network": 0,
-        "qo": 0,
-        "author": [0, 1, 2],
-        "tcmscategori": 0,
-        "propos": 0,
-        "dc": 0,
-        "cluster": 0,
-        "teardown": 0,
-        "proce": 0,
-        "vm": 0,
-        "paradigm": 0,
-        "entiti": 0,
-        "share": [0, 2],
-        "let": 0,
-        "refer": [0, 2],
-        "via": [0, 2],
-        "step": [0, 1, 2],
-        "teststep": [0, 1, 2],
-        "kei": [0, 1, 2],
-        "expectedresult": 0,
-        "step1": 0,
-        "expect": 0,
-        "result": [0, 1, 2, 3],
-        "step2": 0,
-        "arr_step": 0,
-        "test_step": [0, 1],
-        "new_wi": 0,
-        "create_work_item": [0, 1, 2],
-        "space": [0, 2, 3],
-        "get_docu": [0, 1, 2],
-        "proj": 0,
-        "tpl_tp_12071": 0,
-        "staticlivedoc": 0,
-        "doc_with_spac": [0, 2],
-        "tp_12071": 0,
-        "tp_12071_1": 0,
-        "process": 0,
-        "rec": 0,
-        "_workitem": [0, 2],
-        "uri": [0, 1, 2],
-        "get_test_step": 0,
-        "res1": 0,
-        "teststepresult": [0, 1, 2],
-        "comment": [0, 1, 3],
-        "1st": 0,
-        "res2": 0,
-        "2nd": 0,
-        "test_step_result": [0, 1],
-        "add_test_record_by_object": [0, 1, 2],
-        "link": 0,
-        "2828": 0,
-        "11": [0, 2],
-        "add_linked_item": 0,
-        "linked_work_item": [0, 1],
-        "print": 0,
-        "role": [0, 1, 2],
-        "linked_work_items_deriv": 0,
-        "order": [0, 2],
-        "ensur": 0,
-        "abl": 0,
-        "ci": 0,
-        "recommend": 0,
-        "command": [0, 3],
-        "pre": 0,
-        "autoupd": 0,
-        "made": 0,
-        "violat": 0,
-        "pep8": 0,
-        "standard": 0,
-        "we": [0, 2],
-        "autopep8": 0,
-        "fix": 0,
-        "failur": [0, 2],
-        "free": 0,
-        "formatt": 0,
-        "resolv": [0, 1, 2],
-        "least": 0,
-        "diff": [0, 1, 2],
-        "place": 0,
-        "edited_fil": 0,
-        "tool": 0,
-        "manag": [0, 2, 3],
-        "sourc": [0, 2, 3],
-        "To": [0, 2],
-        "new": [0, 2],
-        "tag": [0, 1, 2],
-        "automaticlli": 0,
-        "changelog": 0,
-        "after": [0, 1, 2],
-        "push": 0,
-        "trigger": 0,
-        "system": [0, 2],
-        "make": 0,
-        "third": 0,
-        "parti": 0,
-        "easi": 0,
-        "each": [0, 2],
-        "releas": 0,
-        "epel8": 0,
-        "epel9": 0,
-        "webhook": 0,
-        "defin": [0, 2],
-        "check": [0, 2],
-        "target": 0,
-        "local": [0, 2],
-        "content": [0, 1],
-        "subpackag": [0, 1],
-        "cli": [0, 1, 2],
-        "submodul": [0, 1],
-        "activ": [0, 1],
-        "modul": [0, 1],
-        "activity_com": [0, 1],
-        "activitycom": [0, 1, 2],
-        "activity_custom_valu": [0, 1],
-        "activitycustomvalu": [0, 1, 2],
-        "activity_custom_value_entri": [0, 1],
-        "activitycustomvalueentri": [0, 1, 2],
-        "activity_sourc": [0, 1],
-        "activitysourc": [0, 1, 2],
-        "arrayofapprov": [0, 1, 2],
-        "attach": [0, 1],
-        "arrayofattach": [0, 1, 2],
-        "base_polarion": [0, 1],
-        "classproperti": [0, 1, 2],
-        "tx_wrapper": [0, 1, 2],
-        "baselin": [0, 1],
-        "build_linked_work_item": [0, 1],
-        "arrayofbuildlinkedworkitem": [0, 1, 2],
-        "buildlinkedworkitem": [0, 1, 2],
-        "build_test_result": [0, 1],
-        "buildtestresult": [0, 1, 2],
-        "categori": [0, 1],
-        "arrayofcategori": [0, 1, 2],
-        "arrayofcom": [0, 1, 2],
-        "arrayofcustom": [0, 1, 2],
-        "customfield": [0, 1, 2],
-        "custom_field_typ": [0, 1],
-        "customfieldtyp": [0, 1, 2],
-        "enum_custom_field_typ": [0, 1],
-        "enumcustomfieldtyp": [0, 1, 2],
-        "enum_opt": [0, 1],
-        "enumopt": [0, 1, 2],
-        "enum_option_id": [0, 1],
-        "arrayofenumoptionid": [0, 1, 2],
-        "enumoptionid": [0, 1, 2],
-        "pylerolibexcept": [0, 1, 2],
-        "externally_linked_work_item": [0, 1],
-        "arrayofexternallylinkedworkitem": [0, 1, 2],
-        "externallylinkedworkitem": [0, 1, 2],
-        "field_diff": [0, 1],
-        "fielddiff": [0, 1, 2],
-        "hyperlink": [0, 1],
-        "arrayofhyperlink": [0, 1, 2],
-        "imported_com": [0, 1],
-        "importedcom": [0, 1, 2],
-        "language_definit": [0, 1],
-        "languagedefinit": [0, 1, 2],
-        "license_info": [0, 1],
-        "licenseinfo": [0, 1, 2],
-        "arrayoflinkedworkitem": [0, 1, 2],
-        "linkedworkitem": [0, 1, 2],
-        "module_com": [0, 1],
-        "arrayofmodulecom": [0, 1, 2],
-        "modulecom": [0, 1, 2],
-        "plan": [0, 1],
-        "arrayofplan": [0, 1, 2],
-        "plan_record": [0, 1],
-        "arrayofplanrecord": [0, 1, 2],
-        "planrecord": [0, 1, 2],
-        "plan_statist": [0, 1],
-        "planstatist": [0, 1, 2],
-        "planning_constraint": [0, 1],
-        "arrayofplanningconstraint": [0, 1, 2],
-        "planningconstraint": [0, 1, 2],
-        "priority_opt": [0, 1],
-        "priorityopt": [0, 1, 2],
-        "priority_option_id": [0, 1],
-        "arrayofpriorityoptionid": [0, 1, 2],
-        "priorityoptionid": [0, 1, 2],
-        "product_licens": [0, 1],
-        "productlicens": [0, 1, 2],
-        "project_group": [0, 1],
-        "projectgroup": [0, 1, 2],
-        "revis": [0, 1],
-        "arrayofrevis": [0, 1, 2],
-        "session": [0, 1],
-        "listenfilt": [0, 1, 2],
-        "soapnul": [0, 1, 2],
-        "create_ssl_context": [0, 1, 2],
-        "signatur": [0, 1],
-        "arrayofsignatur": [0, 1, 2],
-        "signature_context": [0, 1],
-        "arrayofsignaturecontext": [0, 1, 2],
-        "signaturecontext": [0, 1, 2],
-        "signature_data": [0, 1],
-        "signaturedata": [0, 1, 2],
-        "subterra_uri": [0, 1],
-        "arrayofsubterrauri": [0, 1, 2],
-        "subterrauri": [0, 1, 2],
-        "arrayoftestrecord": [0, 1, 2],
-        "create_incident_report": [0, 1, 2],
-        "generate_descript": [0, 1, 2],
-        "test_run_attach": [0, 1],
-        "arrayoftestrunattach": [0, 1, 2],
-        "testrunattach": [0, 1, 2],
-        "arrayofteststep": [0, 1, 2],
-        "arrayofteststepresult": [0, 1, 2],
-        "tests_configur": [0, 1],
-        "testsconfigur": [0, 1, 2],
-        "text": [0, 1],
-        "arrayoftext": [0, 1, 2],
-        "time_point": [0, 1],
-        "timepoint": [0, 1, 2],
-        "arrayofus": [0, 1, 2],
-        "wiki_pag": [0, 1],
-        "wikipag": [0, 1, 2],
-        "wiki_page_attach": [0, 1],
-        "arrayofwikipageattach": [0, 1, 2],
-        "wikipageattach": [0, 1, 2],
-        "newclass": [0, 1, 2],
-        "work_record": [0, 1],
-        "arrayofworkrecord": [0, 1, 2],
-        "workrecord": [0, 1, 2],
-        "workflow_act": [0, 1],
-        "workflowact": [0, 1, 2],
-        "index": [0, 2],
-        "search": [0, 1, 2],
-        "page": [0, 2],
-        "packag": 1,
-        "cmd": [1, 2],
-        "context_id": [1, 2],
-        "global_id": [1, 2],
-        "activity_id": [1, 2],
-        "info": [1, 2],
-        "prefix": [1, 2],
-        "resource_loc": [1, 2],
-        "source_id": [1, 2],
-        "timestamp": [1, 2],
-        "user_id": [1, 2],
-        "time_stamp": [1, 2],
-        "custom_valu": [1, 2],
-        "activity_source_id": [1, 2],
-        "file_nam": [1, 2],
-        "attachment_id": [1, 2],
-        "length": [1, 2],
-        "_cls_suds_map": [1, 2],
-        "_id_field": [1, 2],
-        "_obj_client": [1, 2],
-        "_obj_struct": [1, 2],
-        "regex_id": [1, 2],
-        "regex_proj": [1, 2],
-        "uri_id_get_replac": [1, 2],
-        "uri_id_set_replac": [1, 2],
-        "uri_struct": [1, 2],
-        "__init__": [1, 2],
-        "can_add_element_to_kei": [1, 2],
-        "can_delete_inst": [1, 2],
-        "can_modify_inst": [1, 2],
-        "can_modify_kei": [1, 2],
-        "can_read_inst": [1, 2],
-        "can_read_kei": [1, 2],
-        "can_remove_element_from_kei": [1, 2],
-        "check_valid_field_valu": [1, 2],
-        "custom_array_obj": [1, 2],
-        "custom_obj": [1, 2],
-        "get_global_rol": [1, 2],
-        "get_loc": [1, 2],
-        "has_current_user_permiss": [1, 2],
-        "logged_in_user_id": [1, 2],
-        "reload": [1, 2],
-        "repo": [1, 2],
-        "configur": [1, 2],
-        "config_sect": [1, 2],
-        "curdir_config": [1, 2],
-        "global_config": [1, 2],
-        "local_config": [1, 2],
-        "pkgdir": [1, 2],
-        "retri": [1, 2],
-        "token_en": [1, 2],
-        "base_revis": [1, 2],
-        "baseline_id": [1, 2],
-        "build": 1,
-        "bir_loc": [1, 2],
-        "build_descriptor_nam": [1, 2],
-        "build_stamp": [1, 2],
-        "build_statu": [1, 2],
-        "build_tag": [1, 2],
-        "calculation_descriptor_nam": [1, 2],
-        "creation_tim": [1, 2],
-        "finish_tim": [1, 2],
-        "build_id": [1, 2],
-        "job_id": [1, 2],
-        "local_deployment_space_nam": [1, 2],
-        "log_fil": [1, 2],
-        "start_tim": [1, 2],
-        "error_count": [1, 2],
-        "failure_count": [1, 2],
-        "skipped_count": [1, 2],
-        "test_count": [1, 2],
-        "category_id": [1, 2],
-        "creation": [1, 2],
-        "date": [1, 2],
-        "invalid": [1, 2],
-        "child_comment_uri": [1, 2],
-        "comment_id": [1, 2],
-        "parent_comment_uri": [1, 2],
-        "visible_to": [1, 2],
-        "parent_item_uri": [1, 2],
-        "default_valu": [1, 2],
-        "depends_on": [1, 2],
-        "cft_id": [1, 2],
-        "requir": [1, 2],
-        "document": 1,
-        "allowed_wi_typ": [1, 2],
-        "are_links_from_parent_to_child": [1, 2],
-        "auto_suspect": [1, 2],
-        "branched_from": [1, 2],
-        "branched_with_queri": [1, 2],
-        "derived_field": [1, 2],
-        "derived_from_link_rol": [1, 2],
-        "derived_from_uri": [1, 2],
-        "home_page_cont": [1, 2],
-        "id": [1, 2],
-        "module_absolute_loc": [1, 2],
-        "module_fold": [1, 2],
-        "module_loc": [1, 2],
-        "module_nam": [1, 2],
-        "structure_link_rol": [1, 2, 3],
-        "updated_bi": [1, 2],
-        "uses_outline_numb": [1, 2],
-        "add_referenced_work_item": [1, 2],
-        "delet": [1, 2],
-        "export_pdf": [1, 2],
-        "get_work_item": [1, 2],
-        "move_work_item_her": [1, 2],
-        "enum_id": [1, 2],
-        "hidden": [1, 2],
-        "phantom": [1, 2],
-        "sequence_numb": [1, 2],
-        "work_item_uri": [1, 2],
-        "befor": [1, 2],
-        "collect": [1, 2],
-        "field_nam": [1, 2],
-        "remov": [1, 2],
-        "initi": [1, 2],
-        "language_definition_id": [1, 2],
-        "label": [1, 2],
-        "slot": [1, 2],
-        "suspect": [1, 2],
-        "module_comment_id": [1, 2],
-        "referred_work_item_uri": [1, 2],
-        "allowed_typ": [1, 2],
-        "author_uri": [1, 2],
-        "calculation_typ": [1, 2],
-        "capac": [1, 2],
-        "color": [1, 2],
-        "default_estim": [1, 2],
-        "due_dat": [1, 2],
-        "estimation_field": [1, 2],
-        "finished_on": [1, 2],
-        "is_templ": [1, 2, 3],
-        "parent": [1, 2, 3],
-        "plan_id": [1, 2],
-        "previous_time_sp": [1, 2],
-        "prioritization_field": [1, 2],
-        "project_uri": [1, 2],
-        "sort_ord": [1, 2],
-        "start_dat": [1, 2],
-        "started_on": [1, 2],
-        "template_uri": [1, 2],
-        "add_plan_item": [1, 2],
-        "create_plan_templ": [1, 2],
-        "delete_plan": [1, 2],
-        "get_statist": [1, 2],
-        "get_wiki_cont": [1, 2],
-        "remove_plan_item": [1, 2],
-        "set_wiki_cont": [1, 2],
-        "was_start": [1, 2],
-        "done": [1, 2],
-        "done_as_str": [1, 2],
-        "ideal_progress": [1, 2],
-        "ideal_progress_as_str": [1, 2],
-        "number_of_plan": [1, 2],
-        "number_of_resolv": [1, 2],
-        "number_of_unresolv": [1, 2],
-        "planned_as_str": [1, 2],
-        "progress": [1, 2],
-        "progress_as_str": [1, 2],
-        "todo": [1, 2],
-        "todo_as_str": [1, 2],
-        "constraint": [1, 2],
-        "float": [1, 2],
-        "priority_opt_id": [1, 2],
-        "concurrent_license_data": [1, 2],
-        "customer_compani": [1, 2],
-        "customer_email": [1, 2],
-        "customer_nam": [1, 2],
-        "date_cr": [1, 2],
-        "expiration_d": [1, 2],
-        "generated_bi": [1, 2],
-        "ip_address": [1, 2],
-        "license_format": [1, 2],
-        "license_profil": [1, 2],
-        "mac_address": [1, 2],
-        "named_license_data": [1, 2],
-        "finish": [1, 2],
-        "lead": [1, 2],
-        "lock_work_records_d": [1, 2],
-        "tracker_prefix": [1, 2],
-        "get_categori": [1, 2],
-        "get_context_rol": [1, 2],
-        "get_defined_custom_field_kei": [1, 2],
-        "get_defined_custom_field_typ": [1, 2],
-        "get_document_spac": [1, 2],
-        "get_project_us": [1, 2],
-        "get_test_steps_configur": [1, 2],
-        "get_tests_configur": [1, 2],
-        "get_wiki_spac": [1, 2],
-        "group_uri": [1, 2],
-        "parent_uri": [1, 2],
-        "get_contained_group": [1, 2],
-        "get_contained_project": [1, 2],
-        "get_deep_contained_project": [1, 2],
-        "get_root_project_group": [1, 2],
-        "internal_commit": [1, 2],
-        "linked_work_item_uri": [1, 2],
-        "messag": [1, 2],
-        "repository_nam": [1, 2],
-        "filter": [1, 2],
-        "tx_begin": [1, 2],
-        "tx_commit": [1, 2],
-        "tx_in": [1, 2],
-        "tx_releas": [1, 2],
-        "tx_rollback": [1, 2],
-        "add_nil": [1, 2],
-        "marshal": [1, 2],
-        "signed_bi": [1, 2],
-        "signed_revis": [1, 2],
-        "signer_rol": [1, 2],
-        "verdict": [1, 2],
-        "verdict_tim": [1, 2],
-        "target_status_id": [1, 2],
-        "transition_data_revis": [1, 2],
-        "group_id": [1, 2],
-        "keep_in_histori": [1, 2],
-        "summary_defect": [1, 2],
-        "test_run_id": [1, 2],
-        "add_attach": [1, 2],
-        "add_attachment_to_test_record": [1, 2],
-        "add_attachment_to_test_step": [1, 2],
-        "create_summary_defect": [1, 2],
-        "delete_attach": [1, 2],
-        "delete_attachment_from_test_record": [1, 2],
-        "delete_attachment_from_test_step": [1, 2],
-        "get_attach": [1, 2],
-        "update_attach": [1, 2],
-        "update_summary_defect": [1, 2],
-        "update_test_record_by_field": [1, 2],
-        "update_test_record_by_object": [1, 2],
-        "update_wiki_cont": [1, 2],
-        "verify_param": [1, 2],
-        "verify_requir": [1, 2],
-        "test_run_uri": [1, 2],
-        "defect_auto_assignement_en": [1, 2],
-        "defect_reuse_typ": [1, 2],
-        "defect_templ": [1, 2],
-        "defect_to_test_case_link_role_id": [1, 2],
-        "defect_work_item_typ": [1, 2],
-        "defects_project": [1, 2],
-        "fields_to_copy_from_test_case_to_defect": [1, 2],
-        "fields_to_copy_from_test_run_to_linked_defect": [1, 2],
-        "fields_to_copy_from_test_run_to_new_defect": [1, 2],
-        "max_created_defect": [1, 2],
-        "max_created_defects_perc": [1, 2],
-        "result_error_enum_id": [1, 2],
-        "result_failed_enum_id": [1, 2],
-        "result_passed_enum_id": [1, 2],
-        "retest_allow": [1, 2],
-        "status_error_enum_id": [1, 2],
-        "status_failed_enum_id": [1, 2],
-        "status_ok_enum_id": [1, 2],
-        "summary_defect_sever": [1, 2],
-        "test_case_id_custom_field": [1, 2],
-        "test_case_templ": [1, 2],
-        "test_case_test_comment_field_id": [1, 2],
-        "test_case_test_result_field_id": [1, 2],
-        "test_case_work_item_typ": [1, 2],
-        "test_run_templ": [1, 2],
-        "content_typ": [1, 2],
-        "content_lossi": [1, 2],
-        "close": [1, 2],
-        "earliest_planned_start": [1, 2],
-        "time_point_id": [1, 2],
-        "disabled_notif": [1, 2],
-        "email": [1, 2],
-        "vote_uri": [1, 2],
-        "watche_uri": [1, 2],
-        "create_us": [1, 2],
-        "get_rol": [1, 2],
-        "get_user_avatar_url": [1, 2],
-        "get_user_from_token": [1, 2],
-        "get_us": [1, 2],
-        "has_permiss": [1, 2],
-        "wiki_page_id": [1, 2],
-        "linked_page_uri": [1, 2],
-        "page_loc": [1, 2],
-        "page_nam": [1, 2],
-        "space_id": [1, 2],
-        "get_wiki_pag": [1, 2],
-        "wiki_page_attachment_id": [1, 2],
-        "work_record_id": [1, 2],
-        "time_sp": [1, 2],
-        "action_id": [1, 2],
-        "action_nam": [1, 2],
-        "cleaned_featur": [1, 2],
-        "native_action_id": [1, 2],
-        "required_featur": [1, 2],
-        "suggested_featur": [1, 2],
-        "target_statu": [1, 2],
-        "unavailability_messag": [1, 2],
-        "cmdlist": [2, 3],
-        "list_documents_by_queri": [2, 3],
-        "list_workitems_by_queri": [2, 3],
-        "list_workitems_in_doc": [2, 3],
-        "print_docu": [2, 3],
-        "print_links_for_requir": [2, 3],
-        "print_links_for_testcas": [2, 3],
-        "print_plan_id": [2, 3],
-        "print_runs_by_queri": [2, 3],
-        "print_steps_for_testcas": [2, 3],
-        "print_templates_by_queri": [2, 3],
-        "print_testcases_from_run": [2, 3],
-        "print_workitem": [2, 3],
-        "cmdupdat": [2, 3],
-        "update_1_case_result_for_run": [2, 3],
-        "update_all_case_results_for_run": [2, 3],
-        "update_docu": [2, 3],
-        "update_run": [2, 3],
-        "obj_id": 2,
-        "suds_object": 2,
-        "handl": 2,
-        "tns3": 2,
-        "contextid": 2,
-        "string": 2,
-        "date\u05d0im": 2,
-        "arrayof_xsd_str": 2,
-        "tns5": 2,
-        "long": 2,
-        "contain": 2,
-        "arrai": 2,
-        "relat": 2,
-        "relationship": 2,
-        "mean": 2,
-        "repres": 2,
-        "child": 2,
-        "": 2,
-        "constructor": 2,
-        "accept": 2,
-        "paramet": 2,
-        "str": 2,
-        "client": 2,
-        "datatyp": 2,
-        "tnsx": 2,
-        "objectnam": 2,
-        "x": 2,
-        "ha": 2,
-        "one": 2,
-        "matter": 2,
-        "how": 2,
-        "mani": 2,
-        "instanti": 2,
-        "classmethod": 2,
-        "subterra": 2,
-        "servic": 2,
-        "obj": 2,
-        "element": 2,
-        "bool": 2,
-        "secur": 2,
-        "canaddelementtokei": 2,
-        "candeleteinst": 2,
-        "canmodifyinst": 2,
-        "canmodifykei": 2,
-        "read": 2,
-        "canreadinst": 2,
-        "canreadkei": 2,
-        "from": 2,
-        "canremoveelementfromkei": 2,
-        "val": 2,
-        "additional_parm": 2,
-        "control": 2,
-        "exampl": 2,
-        "try": 2,
-        "addit": 2,
-        "parm": 2,
-        "you": 2,
-        "against": 2,
-        "dataandop": 2,
-        "getglobalrol": 2,
-        "context": 2,
-        "method": 2,
-        "group": 2,
-        "getlocationforuri": 2,
-        "avail": 2,
-        "cach": 2,
-        "becaus": 2,
-        "prohibit": 2,
-        "tracker": 2,
-        "getenumoptionsforid": 2,
-        "permiss": 2,
-        "grant": 2,
-        "hascurrentuserpermiss": 2,
-        "gsun": 2,
-        "call": 2,
-        "overwrit": 2,
-        "unsav": 2,
-        "stage": 2,
-        "engin": 2,
-        "redhat": 2,
-        "fget": 2,
-        "fset": 2,
-        "fdel": 2,
-        "getter": 2,
-        "setter": 2,
-        "waynesun": 2,
-        "virtualenv": 2,
-        "xz4tb2ux": 2,
-        "lib": 2,
-        "site": 2,
-        "true": 2,
-        "func": 2,
-        "particular": 2,
-        "null": 2,
-        "createbaselin": 2,
-        "sort": 2,
-        "lucen": 2,
-        "querybaselin": 2,
-        "tns2": 2,
-        "arrayofloc": 2,
-        "int": 2,
-        "boolean": 2,
-        "arrayof_tns3_fielddiff": 2,
-        "arrayofstr": 2,
-        "testmanag": 2,
-        "w": 2,
-        "tns4": 2,
-        "anytyp": 2,
-        "modulefold": 2,
-        "doc_nam": [2, 3],
-        "getmodulebyloc": 2,
-        "getmodulebylocationwithfield": 2,
-        "getmodulebyuri": 2,
-        "getmodulebyuriwithfield": 2,
-        "referenc": 2,
-        "end": 2,
-        "document_nam": 2,
-        "document_titl": 2,
-        "old": 2,
-        "style": 2,
-        "e": 2,
-        "hierarchi": 2,
-        "insid": 2,
-        "html": 2,
-        "markup": 2,
-        "createdocu": 2,
-        "parent_id": 2,
-        "w_item": 2,
-        "createworkiteminmodul": 2,
-        "exportpdfproperti": 2,
-        "output_dir": 2,
-        "tmp": 2,
-        "output_nam": 2,
-        "export": 2,
-        "pdf": 2,
-        "papers": 2,
-        "size": 2,
-        "a4": 2,
-        "a3": 2,
-        "letter": 2,
-        "legal": 2,
-        "tabloid": 2,
-        "portrait": 2,
-        "landscap": 2,
-        "fittopagewidth": 2,
-        "fit": 2,
-        "width": 2,
-        "generatebookmark": 2,
-        "bookmark": 2,
-        "includeheaderfoot": 2,
-        "header": 2,
-        "footer": 2,
-        "watermark": 2,
-        "destin": 2,
-        "output": 2,
-        "exportdocumenttopdf": 2,
-        "getmodul": 2,
-        "getmoduleswithfield": 2,
-        "parent_work_item_id": 2,
-        "deep": 2,
-        "under": 2,
-        "whole": 2,
-        "subtre": 2,
-        "For": 2,
-        "nest": 2,
-        "syntax": 2,
-        "subset": 2,
-        "mylist": 2,
-        "g": 2,
-        "getmoduleworkitem": 2,
-        "retain_flow": 2,
-        "move": 2,
-        "yet": 2,
-        "desir": 2,
-        "children": 2,
-        "insert": 2,
-        "count": 2,
-        "retain": 2,
-        "flow": 2,
-        "even": 2,
-        "fals": [2, 3],
-        "keep": 2,
-        "moveworkitemtodocu": 2,
-        "is_sql": 2,
-        "document_id": 2,
-        "limit": 2,
-        "baseline_revis": 2,
-        "query_uri": 2,
-        "sql": 2,
-        "determin": 2,
-        "custom_field_id": 2,
-        "everyth": 2,
-        "popul": 2,
-        "rev": 2,
-        "found": 2,
-        "instead": 2,
-        "querymoduleuri": 2,
-        "querymoduleurisbysql": 2,
-        "querymoduleurisinbaselin": 2,
-        "querymoduleurisinbaselinebysql": 2,
-        "querymodul": 2,
-        "querymodulesbysql": 2,
-        "querymodulesinbaselin": 2,
-        "querymodulesinbaselinebysql": 2,
-        "updatemodul": 2,
-        "arrayof_xsd_anytyp": 2,
-        "tns6": 2,
-        "getplanbyid": 2,
-        "getplanbyuri": 2,
-        "addplanitem": 2,
-        "plan_nam": 2,
-        "template_id": 2,
-        "createplan": 2,
-        "template_nam": 2,
-        "createplantempl": 2,
-        "deleteplan": 2,
-        "statist": 2,
-        "getplanstatist": 2,
-        "wiki": 2,
-        "getplanwikicont": 2,
-        "removeplanitem": 2,
-        "search_templ": 2,
-        "arg": 2,
-        "maximum": 2,
-        "searchplantempl": 2,
-        "searchplantemplateswithfield": 2,
-        "searchplan": 2,
-        "searchplanswithfield": 2,
-        "setplanwikicont": 2,
-        "updateplan": 2,
-        "wasplanstart": 2,
-        "prioriti": 2,
-        "arrayof_tns3_licenseinfo": 2,
-        "polarionproject": 2,
-        "identifi": 2,
-        "getproject": 2,
-        "getprojectatloc": 2,
-        "getprojectbyuri": 2,
-        "retriev": 2,
-        "getcategori": 2,
-        "getcontextrol": 2,
-        "work_item_type_id": 2,
-        "getdefinedcustomfieldkei": 2,
-        "definit": 2,
-        "getdefinedcustomfieldtyp": 2,
-        "getdocumentspac": 2,
-        "getprojectus": 2,
-        "getteststepsconfigur": 2,
-        "gettestsconfigur": 2,
-        "getwikispac": 2,
-        "p": 2,
-        "getprojectgroup": 2,
-        "getprojectgroupatloc": 2,
-        "directli": 2,
-        "getcontainedgroup": 2,
-        "getcontainedproject": 2,
-        "getdeepcontainedproject": 2,
-        "getrootprojectgroup": 2,
-        "queryrevis": 2,
-        "relogin_timeout": 2,
-        "60": 2,
-        "timeout": 2,
-        "120": 2,
-        "configuar": 2,
-        "again": 2,
-        "tiemout": 2,
-        "bundl": 2,
-        "log": 2,
-        "nonzero": 2,
-        "ye": 2,
-        "caching_polici": 2,
-        "polici": 2,
-        "conn": 2,
-        "transact": 2,
-        "within": 2,
-        "anoth": 2,
-        "middl": 2,
-        "messageplugin": 2,
-        "plugin": 2,
-        "remot": 2,
-        "It": 2,
-        "xsi": 2,
-        "nil": 2,
-        "were": 2,
-        "suppos": 2,
-        "did": 2,
-        "walk": 2,
-        "attr": 2,
-        "send": 2,
-        "envelop": 2,
-        "opportun": 2,
-        "inspect": 2,
-        "param": 2,
-        "l": 2,
-        "messagecontext": 2,
-        "ssl": 2,
-        "version": 2,
-        "defect_case_id": 2,
-        "test_case_revis": 2,
-        "indic": 2,
-        "automated_process": 2,
-        "dynamic_queri": 2,
-        "dynamic_livedoc": 2,
-        "manual_select": 2,
-        "static_queri": 2,
-        "static_livedoc": 2,
-        "uniqu": 2,
-        "test_manag": 2,
-        "gettestrunbyid": 2,
-        "gettestrunbyuri": 2,
-        "upload": 2,
-        "friendli": 2,
-        "addattachmenttotestrun": 2,
-        "addattachmenttotestrecord": 2,
-        "test_step_index": 2,
-        "record_index": 2,
-        "higher": 2,
-        "addattachmenttoteststep": 2,
-        "last": 2,
-        "block": 2,
-        "addtestrecordtotestrun": 2,
-        "manual_state_chang": 2,
-        "complet": 2,
-        "state": 2,
-        "accordingli": 2,
-        "notrun": 2,
-        "manual": 2,
-        "kwarg": 2,
-        "mark": 2,
-        "ignor": 2,
-        "cannot": 2,
-        "exist": 2,
-        "caus": 2,
-        "autogen": 2,
-        "keyword": 2,
-        "argument": 2,
-        "upon": 2,
-        "createtestrun": 2,
-        "defect_template_id": 2,
-        "summari": 2,
-        "createsummarydefect": 2,
-        "choos": 2,
-        "select": 2,
-        "filenam": 2,
-        "applic": 2,
-        "deletetestrunattach": 2,
-        "deleteattachmentfromtestrecord": 2,
-        "gettestrunattach": 2,
-        "do": 2,
-        "mostli": 2,
-        "interchang": 2,
-        "getdefinedtestruncustomfieldtyp": 2,
-        "getwikicontentfortestrun": 2,
-        "unexecut": 2,
-        "ones": 2,
-        "well": 2,
-        "other": 2,
-        "searchtestruntempl": 2,
-        "searchtestruntemplateslimit": 2,
-        "searchtestruntemplateswithfield": 2,
-        "searchtestruntemplateswithfieldslimit": 2,
-        "searchtestrun": 2,
-        "searchtestrunlimit": 2,
-        "searchtestrunswithfield": 2,
-        "searchtestrunswithfieldslimit": 2,
-        "updatetestrun": 2,
-        "original_filenam": 2,
-        "updatetestrunattach": 2,
-        "total_failur": 2,
-        "total_error": 2,
-        "total_test": 2,
-        "amount": 2,
-        "total": 2,
-        "updatesummarydefect": 2,
-        "neg": 2,
-        "treat": 2,
-        "updatetestrecord": 2,
-        "updatetestrecordatindex": 2,
-        "updatewikicontentfortestrun": 2,
-        "unknown": 2,
-        "test_cas": 2,
-        "rich": 2,
-        "format": 2,
-        "eg": 2,
-        "multipl": 2,
-        "getus": 2,
-        "getuserbyuri": 2,
-        "createus": 2,
-        "java": 2,
-        "lang": 2,
-        "getcontextrolesforus": 2,
-        "assign": 2,
-        "getrolesforus": 2,
-        "rel": 2,
-        "avatar": 2,
-        "getuseravatarurl": 2,
-        "getuserfromtoken": 2,
-        "haspermiss": 2,
-        "updateus": 2,
-        "getwikipagebyuri": 2,
-        "getwikipagebyuriwithfield": 2,
-        "querywikipageuri": 2,
-        "querywikipageurisbysql": 2,
-        "querywikipageurisinbaselin": 2,
-        "querywikipageurisinbaselinebysql": 2,
-        "querywikipag": 2,
-        "querywikipagesbysql": 2,
-        "querywikipagesinbaselin": 2,
-        "querywikipagesinbaselinebysql": 2,
-        "_specificworkitem": 2,
-        "alia": 2,
-        "wi_typ": 3,
-        "doc_name_with_spac": 3,
-        "req_id": 3,
-        "case_id": 3,
-        "doc_titl": 3,
-        "doc_typ": 3,
-        "plannedin": 3,
-        "assigne": 3
-    },
-    "objects": {
-        "": [
-            [2, 0, 0, "-", "pylero"]
-        ],
-        "pylero": [
-            [2, 0, 0, "-", "activity"],
-            [2, 0, 0, "-", "activity_comment"],
-            [2, 0, 0, "-", "activity_custom_value"],
-            [2, 0, 0, "-", "activity_custom_value_entry"],
-            [2, 0, 0, "-", "activity_source"],
-            [2, 0, 0, "-", "approval"],
-            [2, 0, 0, "-", "attachment"],
-            [2, 0, 0, "-", "base_polarion"],
-            [2, 0, 0, "-", "baseline"],
-            [2, 0, 0, "-", "build"],
-            [2, 0, 0, "-", "build_linked_work_item"],
-            [2, 0, 0, "-", "build_test_results"],
-            [2, 0, 0, "-", "category"],
-            [2, 0, 0, "-", "change"],
-            [3, 0, 0, "-", "cli"],
-            [2, 0, 0, "-", "comment"],
-            [2, 0, 0, "-", "custom"],
-            [2, 0, 0, "-", "custom_field"],
-            [2, 0, 0, "-", "custom_field_type"],
-            [2, 0, 0, "-", "document"],
-            [2, 0, 0, "-", "enum_custom_field_type"],
-            [2, 0, 0, "-", "enum_option"],
-            [2, 0, 0, "-", "enum_option_id"],
-            [2, 0, 0, "-", "exceptions"],
-            [2, 0, 0, "-", "externally_linked_work_item"],
-            [2, 0, 0, "-", "field_diff"],
-            [2, 0, 0, "-", "hyperlink"],
-            [2, 0, 0, "-", "imported_comment"],
-            [2, 0, 0, "-", "language_definition"],
-            [2, 0, 0, "-", "license_info"],
-            [2, 0, 0, "-", "linked_work_item"],
-            [2, 0, 0, "-", "module_comment"],
-            [2, 0, 0, "-", "plan"],
-            [2, 0, 0, "-", "plan_record"],
-            [2, 0, 0, "-", "plan_statistics"],
-            [2, 0, 0, "-", "planning_constraint"],
-            [2, 0, 0, "-", "priority_opt"],
-            [2, 0, 0, "-", "priority_option_id"],
-            [2, 0, 0, "-", "product_license"],
-            [2, 0, 0, "-", "project"],
-            [2, 0, 0, "-", "project_group"],
-            [2, 0, 0, "-", "properties"],
-            [2, 0, 0, "-", "property"],
-            [2, 0, 0, "-", "revision"],
-            [2, 0, 0, "-", "server"],
-            [2, 0, 0, "-", "session"],
-            [2, 0, 0, "-", "signature"],
-            [2, 0, 0, "-", "signature_context"],
-            [2, 0, 0, "-", "signature_data"],
-            [2, 0, 0, "-", "subterra_uri"],
-            [2, 0, 0, "-", "test_record"],
-            [2, 0, 0, "-", "test_run"],
-            [2, 0, 0, "-", "test_run_attachment"],
-            [2, 0, 0, "-", "test_step"],
-            [2, 0, 0, "-", "test_step_result"],
-            [2, 0, 0, "-", "test_steps"],
-            [2, 0, 0, "-", "tests_configuration"],
-            [2, 0, 0, "-", "text"],
-            [2, 0, 0, "-", "time_point"],
-            [2, 0, 0, "-", "user"],
-            [2, 0, 0, "-", "wiki_page"],
-            [2, 0, 0, "-", "wiki_page_attachment"],
-            [2, 0, 0, "-", "work_item"],
-            [2, 0, 0, "-", "work_record"],
-            [2, 0, 0, "-", "workflow_action"]
-        ],
-        "pylero.activity": [
-            [2, 1, 1, "", "Activity"]
-        ],
-        "pylero.activity.Activity": [
-            [2, 2, 1, "", "activity_custom_values"],
-            [2, 2, 1, "", "activity_id"],
-            [2, 2, 1, "", "comments"],
-            [2, 2, 1, "", "context_id"],
-            [2, 2, 1, "", "global_id"],
-            [2, 2, 1, "", "info"],
-            [2, 2, 1, "", "prefix"],
-            [2, 2, 1, "", "resource_locations"],
-            [2, 2, 1, "", "source_id"],
-            [2, 2, 1, "", "timestamp"],
-            [2, 2, 1, "", "type"],
-            [2, 2, 1, "", "user_id"]
-        ],
-        "pylero.activity_comment": [
-            [2, 1, 1, "", "ActivityComment"]
-        ],
-        "pylero.activity_comment.ActivityComment": [
-            [2, 2, 1, "", "text"],
-            [2, 2, 1, "", "time_stamp"],
-            [2, 2, 1, "", "user_id"]
-        ],
-        "pylero.activity_custom_value": [
-            [2, 1, 1, "", "ActivityCustomValue"]
-        ],
-        "pylero.activity_custom_value.ActivityCustomValue": [
-            [2, 2, 1, "", "values"]
-        ],
-        "pylero.activity_custom_value_entry": [
-            [2, 1, 1, "", "ActivityCustomValueEntry"]
-        ],
-        "pylero.activity_custom_value_entry.ActivityCustomValueEntry": [
-            [2, 2, 1, "", "custom_values"],
-            [2, 2, 1, "", "key"]
-        ],
-        "pylero.activity_source": [
-            [2, 1, 1, "", "ActivitySource"]
-        ],
-        "pylero.activity_source.ActivitySource": [
-            [2, 2, 1, "", "activity_source_id"],
-            [2, 2, 1, "", "prefix"],
-            [2, 2, 1, "", "types"]
-        ],
-        "pylero.approval": [
-            [2, 1, 1, "", "Approval"],
-            [2, 1, 1, "", "ArrayOfApproval"]
-        ],
-        "pylero.approval.Approval": [
-            [2, 2, 1, "", "status"],
-            [2, 2, 1, "", "user"]
-        ],
-        "pylero.attachment": [
-            [2, 1, 1, "", "ArrayOfAttachment"],
-            [2, 1, 1, "", "Attachment"]
-        ],
-        "pylero.attachment.Attachment": [
-            [2, 2, 1, "", "attachment_id"],
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "file_name"],
-            [2, 2, 1, "", "length"],
-            [2, 2, 1, "", "title"],
-            [2, 2, 1, "", "updated"],
-            [2, 2, 1, "", "url"]
-        ],
-        "pylero.base_polarion": [
-            [2, 1, 1, "", "BasePolarion"],
-            [2, 1, 1, "", "ClassProperty"],
-            [2, 1, 1, "", "Configuration"],
-            [2, 1, 1, "", "Connection"],
-            [2, 4, 1, "", "tx_wrapper"]
-        ],
-        "pylero.base_polarion.BasePolarion": [
-            [2, 2, 1, "", "REGEX_ID"],
-            [2, 2, 1, "", "REGEX_PROJ"],
-            [2, 3, 1, "", "URI_ID_GET_REPLACE"],
-            [2, 3, 1, "", "URI_ID_SET_REPLACE"],
-            [2, 2, 1, "", "URI_STRUCT"],
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "_cls_suds_map"],
-            [2, 2, 1, "", "_id_field"],
-            [2, 2, 1, "", "_obj_client"],
-            [2, 2, 1, "", "_obj_struct"],
-            [2, 3, 1, "", "can_add_element_to_key"],
-            [2, 3, 1, "", "can_delete_instance"],
-            [2, 3, 1, "", "can_modify_instance"],
-            [2, 3, 1, "", "can_modify_key"],
-            [2, 3, 1, "", "can_read_instance"],
-            [2, 3, 1, "", "can_read_key"],
-            [2, 3, 1, "", "can_remove_element_from_key"],
-            [2, 3, 1, "", "check_valid_field_values"],
-            [2, 3, 1, "", "custom_array_obj"],
-            [2, 3, 1, "", "custom_obj"],
-            [2, 2, 1, "id0", "default_project"],
-            [2, 3, 1, "", "get_global_roles"],
-            [2, 3, 1, "", "get_location"],
-            [2, 3, 1, "", "get_valid_field_values"],
-            [2, 3, 1, "", "has_current_user_permission"],
-            [2, 2, 1, "", "logged_in_user_id"],
-            [2, 3, 1, "", "reload"],
-            [2, 2, 1, "", "repo"],
-            [2, 2, 1, "id1", "session"]
-        ],
-        "pylero.base_polarion.Configuration": [
-            [2, 2, 1, "", "CONFIG_SECTION"],
-            [2, 2, 1, "", "CURDIR_CONFIG"],
-            [2, 2, 1, "", "GLOBAL_CONFIG"],
-            [2, 2, 1, "", "LOCAL_CONFIG"],
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "pkgdir"]
-        ],
-        "pylero.base_polarion.Connection": [
-            [2, 2, 1, "", "connected"],
-            [2, 2, 1, "", "retries"],
-            [2, 2, 1, "", "session"],
-            [2, 2, 1, "", "token_enabled"]
-        ],
-        "pylero.baseline": [
-            [2, 1, 1, "", "Baseline"]
-        ],
-        "pylero.baseline.Baseline": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "base_revision"],
-            [2, 2, 1, "", "baseline_id"],
-            [2, 3, 1, "", "create"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "project"],
-            [2, 3, 1, "", "query"]
-        ],
-        "pylero.build": [
-            [2, 1, 1, "", "Build"]
-        ],
-        "pylero.build.Build": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "bir_location"],
-            [2, 2, 1, "", "build_descriptor_name"],
-            [2, 2, 1, "", "build_id"],
-            [2, 2, 1, "", "build_stamp"],
-            [2, 2, 1, "", "build_status"],
-            [2, 2, 1, "", "build_tag"],
-            [2, 2, 1, "", "build_test_results"],
-            [2, 2, 1, "", "calculation_descriptor_name"],
-            [2, 2, 1, "", "creation_time"],
-            [2, 2, 1, "", "finish_time"],
-            [2, 2, 1, "", "job_id"],
-            [2, 2, 1, "", "linked_work_items"],
-            [2, 2, 1, "", "local_deployment_space_name"],
-            [2, 2, 1, "", "log_files"],
-            [2, 2, 1, "", "start_time"]
-        ],
-        "pylero.build_linked_work_item": [
-            [2, 1, 1, "", "ArrayOfBuildLinkedWorkItem"],
-            [2, 1, 1, "", "BuildLinkedWorkItem"]
-        ],
-        "pylero.build_linked_work_item.BuildLinkedWorkItem": [
-            [2, 2, 1, "", "revision"],
-            [2, 2, 1, "", "role"],
-            [2, 2, 1, "", "work_item"]
-        ],
-        "pylero.build_test_results": [
-            [2, 1, 1, "", "BuildTestResults"]
-        ],
-        "pylero.build_test_results.BuildTestResults": [
-            [2, 2, 1, "", "error_count"],
-            [2, 2, 1, "", "failure_count"],
-            [2, 2, 1, "", "skipped_count"],
-            [2, 2, 1, "", "test_count"]
-        ],
-        "pylero.category": [
-            [2, 1, 1, "", "ArrayOfCategory"],
-            [2, 1, 1, "", "Category"]
-        ],
-        "pylero.category.Category": [
-            [2, 2, 1, "", "category_id"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "name"]
-        ],
-        "pylero.change": [
-            [2, 1, 1, "", "Change"]
-        ],
-        "pylero.change.Change": [
-            [2, 2, 1, "", "creation"],
-            [2, 2, 1, "", "date"],
-            [2, 2, 1, "", "diffs"],
-            [2, 2, 1, "", "empty"],
-            [2, 2, 1, "", "invalid"],
-            [2, 2, 1, "", "revision"],
-            [2, 2, 1, "", "user"]
-        ],
-        "pylero.cli": [
-            [3, 0, 0, "-", "cmd"]
-        ],
-        "pylero.cli.cmd": [
-            [3, 1, 1, "", "CmdList"],
-            [3, 1, 1, "", "CmdUpdate"]
-        ],
-        "pylero.cli.cmd.CmdList": [
-            [3, 3, 1, "", "list_documents_by_query"],
-            [3, 3, 1, "", "list_workitems_by_query"],
-            [3, 3, 1, "", "list_workitems_in_doc"],
-            [3, 3, 1, "", "print_documents"],
-            [3, 3, 1, "", "print_links_for_requirement"],
-            [3, 3, 1, "", "print_links_for_testcase"],
-            [3, 3, 1, "", "print_plan_ids"],
-            [3, 3, 1, "", "print_runs_by_query"],
-            [3, 3, 1, "", "print_steps_for_testcase"],
-            [3, 3, 1, "", "print_templates_by_query"],
-            [3, 3, 1, "", "print_testcases_from_run"],
-            [3, 3, 1, "", "print_workitems"]
-        ],
-        "pylero.cli.cmd.CmdUpdate": [
-            [3, 3, 1, "", "update_1_case_result_for_run"],
-            [3, 3, 1, "", "update_all_case_results_for_run"],
-            [3, 3, 1, "", "update_all_case_results_for_runs"],
-            [3, 3, 1, "", "update_document"],
-            [3, 3, 1, "", "update_run"],
-            [3, 3, 1, "", "update_runs"]
-        ],
-        "pylero.comment": [
-            [2, 1, 1, "", "ArrayOfComment"],
-            [2, 1, 1, "", "Comment"]
-        ],
-        "pylero.comment.Comment": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "child_comment_uris"],
-            [2, 2, 1, "", "comment_id"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "parent_comment_uri"],
-            [2, 2, 1, "", "resolved"],
-            [2, 2, 1, "", "signature_data"],
-            [2, 2, 1, "", "tags"],
-            [2, 2, 1, "", "text"],
-            [2, 2, 1, "", "title"],
-            [2, 2, 1, "", "visible_to"]
-        ],
-        "pylero.custom": [
-            [2, 1, 1, "", "ArrayOfCustom"],
-            [2, 1, 1, "", "Custom"]
-        ],
-        "pylero.custom.Custom": [
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "key"],
-            [2, 2, 1, "", "value"]
-        ],
-        "pylero.custom_field": [
-            [2, 1, 1, "", "CustomField"]
-        ],
-        "pylero.custom_field.CustomField": [
-            [2, 2, 1, "", "key"],
-            [2, 2, 1, "", "parent_item_uri"],
-            [2, 2, 1, "", "value"]
-        ],
-        "pylero.custom_field_type": [
-            [2, 1, 1, "", "CustomFieldType"]
-        ],
-        "pylero.custom_field_type.CustomFieldType": [
-            [2, 2, 1, "", "cft_id"],
-            [2, 2, 1, "", "default_value"],
-            [2, 2, 1, "", "depends_on"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "required"],
-            [2, 2, 1, "", "type"]
-        ],
-        "pylero.document": [
-            [2, 1, 1, "", "Document"]
-        ],
-        "pylero.document.Document": [
-            [2, 3, 1, "", "URI_ID_GET_REPLACE"],
-            [2, 3, 1, "", "URI_ID_SET_REPLACE"],
-            [2, 2, 1, "", "URI_STRUCT"],
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "add_referenced_work_item"],
-            [2, 2, 1, "", "allowed_wi_types"],
-            [2, 2, 1, "", "are_links_from_parent_to_child"],
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "auto_suspect"],
-            [2, 2, 1, "", "branched_from"],
-            [2, 2, 1, "", "branched_with_query"],
-            [2, 2, 1, "", "comments"],
-            [2, 3, 1, "", "create"],
-            [2, 3, 1, "", "create_work_item"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "custom_fields"],
-            [2, 3, 1, "", "delete"],
-            [2, 2, 1, "", "derived_fields"],
-            [2, 2, 1, "", "derived_from_link_role"],
-            [2, 2, 1, "", "derived_from_uri"],
-            [2, 3, 1, "", "export_pdf"],
-            [2, 3, 1, "", "get_documents"],
-            [2, 3, 1, "", "get_work_items"],
-            [2, 2, 1, "", "home_page_content"],
-            [2, 2, 1, "", "id"],
-            [2, 2, 1, "", "location"],
-            [2, 2, 1, "", "module_absolute_location"],
-            [2, 2, 1, "", "module_folder"],
-            [2, 2, 1, "", "module_location"],
-            [2, 2, 1, "", "module_name"],
-            [2, 3, 1, "", "move_work_item_here"],
-            [2, 2, 1, "", "project"],
-            [2, 3, 1, "", "query"],
-            [2, 2, 1, "", "signature_contexts"],
-            [2, 2, 1, "", "status"],
-            [2, 2, 1, "", "structure_link_role"],
-            [2, 2, 1, "", "title"],
-            [2, 2, 1, "", "type"],
-            [2, 3, 1, "", "update"],
-            [2, 2, 1, "", "updated"],
-            [2, 2, 1, "", "updated_by"],
-            [2, 2, 1, "", "uses_outline_numbering"]
-        ],
-        "pylero.enum_custom_field_type": [
-            [2, 1, 1, "", "EnumCustomFieldType"]
-        ],
-        "pylero.enum_custom_field_type.EnumCustomFieldType": [
-            [2, 2, 1, "", "default_value"],
-            [2, 2, 1, "", "depends_on"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "enum_id"],
-            [2, 2, 1, "", "id"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "required"],
-            [2, 2, 1, "", "type"]
-        ],
-        "pylero.enum_option": [
-            [2, 1, 1, "", "EnumOption"]
-        ],
-        "pylero.enum_option.EnumOption": [
-            [2, 2, 1, "", "default"],
-            [2, 2, 1, "", "enum_id"],
-            [2, 2, 1, "", "enum_option_id"],
-            [2, 2, 1, "", "hidden"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "phantom"],
-            [2, 2, 1, "", "properties"],
-            [2, 2, 1, "", "sequence_number"]
-        ],
-        "pylero.enum_option_id": [
-            [2, 1, 1, "", "ArrayOfEnumOptionId"],
-            [2, 1, 1, "", "EnumOptionId"]
-        ],
-        "pylero.enum_option_id.EnumOptionId": [
-            [2, 3, 1, "", "__init__"]
-        ],
-        "pylero.exceptions": [
-            [2, 5, 1, "", "PyleroLibException"]
-        ],
-        "pylero.externally_linked_work_item": [
-            [2, 1, 1, "", "ArrayOfExternallyLinkedWorkItem"],
-            [2, 1, 1, "", "ExternallyLinkedWorkItem"]
-        ],
-        "pylero.externally_linked_work_item.ExternallyLinkedWorkItem": [
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "role"],
-            [2, 2, 1, "", "work_item_uri"]
-        ],
-        "pylero.field_diff": [
-            [2, 1, 1, "", "FieldDiff"]
-        ],
-        "pylero.field_diff.FieldDiff": [
-            [2, 2, 1, "", "added"],
-            [2, 2, 1, "", "after"],
-            [2, 2, 1, "", "before"],
-            [2, 2, 1, "", "collection"],
-            [2, 2, 1, "", "field_name"],
-            [2, 2, 1, "", "removed"]
-        ],
-        "pylero.hyperlink": [
-            [2, 1, 1, "", "ArrayOfHyperlink"],
-            [2, 1, 1, "", "Hyperlink"]
-        ],
-        "pylero.hyperlink.Hyperlink": [
-            [2, 2, 1, "", "role"],
-            [2, 2, 1, "", "uri"]
-        ],
-        "pylero.imported_comment": [
-            [2, 1, 1, "", "ImportedComment"]
-        ],
-        "pylero.imported_comment.ImportedComment": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "initials"]
-        ],
-        "pylero.language_definition": [
-            [2, 1, 1, "", "LanguageDefinition"]
-        ],
-        "pylero.language_definition.LanguageDefinition": [
-            [2, 2, 1, "", "label"],
-            [2, 2, 1, "", "language_definition_id"]
-        ],
-        "pylero.license_info": [
-            [2, 1, 1, "", "LicenseInfo"]
-        ],
-        "pylero.license_info.LicenseInfo": [
-            [2, 2, 1, "", "license"],
-            [2, 2, 1, "", "slots"]
-        ],
-        "pylero.linked_work_item": [
-            [2, 1, 1, "", "ArrayOfLinkedWorkItem"],
-            [2, 1, 1, "", "LinkedWorkItem"]
-        ],
-        "pylero.linked_work_item.LinkedWorkItem": [
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "revision"],
-            [2, 2, 1, "", "role"],
-            [2, 2, 1, "", "suspect"],
-            [2, 2, 1, "", "work_item_id"]
-        ],
-        "pylero.module_comment": [
-            [2, 1, 1, "", "ArrayOfModuleComment"],
-            [2, 1, 1, "", "ModuleComment"]
-        ],
-        "pylero.module_comment.ModuleComment": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "child_comment_uris"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "imported_comment"],
-            [2, 2, 1, "", "module_comment_id"],
-            [2, 2, 1, "", "parent_comment_uri"],
-            [2, 2, 1, "", "referred_work_item_uri"],
-            [2, 2, 1, "", "resolved"],
-            [2, 2, 1, "", "signature_data"],
-            [2, 2, 1, "", "tags"],
-            [2, 2, 1, "", "text"]
-        ],
-        "pylero.plan": [
-            [2, 1, 1, "", "ArrayOfPlan"],
-            [2, 1, 1, "", "Plan"]
-        ],
-        "pylero.plan.Plan": [
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "add_plan_items"],
-            [2, 2, 1, "", "allowed_types"],
-            [2, 2, 1, "", "author_uri"],
-            [2, 2, 1, "", "calculation_type"],
-            [2, 2, 1, "", "capacity"],
-            [2, 2, 1, "", "color"],
-            [2, 3, 1, "", "create"],
-            [2, 3, 1, "", "create_plan_template"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "custom_fields"],
-            [2, 2, 1, "", "default_estimate"],
-            [2, 3, 1, "", "delete_plans"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "due_date"],
-            [2, 2, 1, "", "estimation_field"],
-            [2, 2, 1, "", "finished_on"],
-            [2, 3, 1, "", "get_statistics"],
-            [2, 3, 1, "", "get_wiki_content"],
-            [2, 2, 1, "", "is_template"],
-            [2, 2, 1, "", "location"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "parent"],
-            [2, 2, 1, "", "plan_id"],
-            [2, 2, 1, "", "previous_time_spent"],
-            [2, 2, 1, "", "prioritization_field"],
-            [2, 2, 1, "", "project_uri"],
-            [2, 2, 1, "", "records"],
-            [2, 3, 1, "", "remove_plan_items"],
-            [2, 3, 1, "", "search"],
-            [2, 3, 1, "", "set_wiki_content"],
-            [2, 2, 1, "", "sort_order"],
-            [2, 2, 1, "", "start_date"],
-            [2, 2, 1, "", "started_on"],
-            [2, 2, 1, "", "status"],
-            [2, 2, 1, "", "template_uri"],
-            [2, 3, 1, "", "update"],
-            [2, 2, 1, "", "updated"],
-            [2, 3, 1, "", "was_started"]
-        ],
-        "pylero.plan_record": [
-            [2, 1, 1, "", "ArrayOfPlanRecord"],
-            [2, 1, 1, "", "PlanRecord"]
-        ],
-        "pylero.plan_record.PlanRecord": [
-            [2, 2, 1, "", "item"]
-        ],
-        "pylero.plan_statistics": [
-            [2, 1, 1, "", "PlanStatistics"]
-        ],
-        "pylero.plan_statistics.PlanStatistics": [
-            [2, 2, 1, "", "done"],
-            [2, 2, 1, "", "done_as_string"],
-            [2, 2, 1, "", "ideal_progress"],
-            [2, 2, 1, "", "ideal_progress_as_string"],
-            [2, 2, 1, "", "number_of_planned"],
-            [2, 2, 1, "", "number_of_resolved"],
-            [2, 2, 1, "", "number_of_unresolved"],
-            [2, 2, 1, "", "planned"],
-            [2, 2, 1, "", "planned_as_string"],
-            [2, 2, 1, "", "progress"],
-            [2, 2, 1, "", "progress_as_string"],
-            [2, 2, 1, "", "todo"],
-            [2, 2, 1, "", "todo_as_string"]
-        ],
-        "pylero.planning_constraint": [
-            [2, 1, 1, "", "ArrayOfPlanningConstraint"],
-            [2, 1, 1, "", "PlanningConstraint"]
-        ],
-        "pylero.planning_constraint.PlanningConstraint": [
-            [2, 2, 1, "", "constraint"],
-            [2, 2, 1, "", "date"]
-        ],
-        "pylero.priority_opt": [
-            [2, 1, 1, "", "PriorityOpt"]
-        ],
-        "pylero.priority_opt.PriorityOpt": [
-            [2, 2, 1, "", "default"],
-            [2, 2, 1, "", "enum_id"],
-            [2, 2, 1, "", "float"],
-            [2, 2, 1, "", "hidden"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "phantom"],
-            [2, 2, 1, "", "priority_opt_id"],
-            [2, 2, 1, "", "properties"],
-            [2, 2, 1, "", "sequence_number"]
-        ],
-        "pylero.priority_option_id": [
-            [2, 1, 1, "", "ArrayOfPriorityOptionId"],
-            [2, 1, 1, "", "PriorityOptionId"]
-        ],
-        "pylero.priority_option_id.PriorityOptionId": [
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "id"]
-        ],
-        "pylero.product_license": [
-            [2, 1, 1, "", "ProductLicense"]
-        ],
-        "pylero.product_license.ProductLicense": [
-            [2, 2, 1, "", "concurrent_license_data"],
-            [2, 2, 1, "", "customer_company"],
-            [2, 2, 1, "", "customer_email"],
-            [2, 2, 1, "", "customer_name"],
-            [2, 2, 1, "", "date_created"],
-            [2, 2, 1, "", "expiration_date"],
-            [2, 2, 1, "", "generated_by"],
-            [2, 2, 1, "", "ip_address"],
-            [2, 2, 1, "", "license_format"],
-            [2, 2, 1, "", "license_profile"],
-            [2, 2, 1, "", "mac_address"],
-            [2, 2, 1, "", "named_license_data"]
-        ],
-        "pylero.project": [
-            [2, 1, 1, "", "Project"]
-        ],
-        "pylero.project.Project": [
-            [2, 2, 1, "", "URI_STRUCT"],
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "active"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "finish"],
-            [2, 3, 1, "", "get_categories"],
-            [2, 3, 1, "", "get_context_roles"],
-            [2, 3, 1, "", "get_defined_custom_field_keys"],
-            [2, 3, 1, "", "get_defined_custom_field_type"],
-            [2, 3, 1, "", "get_defined_custom_field_types"],
-            [2, 3, 1, "", "get_document_spaces"],
-            [2, 3, 1, "", "get_project_users"],
-            [2, 3, 1, "", "get_test_steps_configuration"],
-            [2, 3, 1, "", "get_tests_configuration"],
-            [2, 3, 1, "", "get_wiki_spaces"],
-            [2, 2, 1, "", "lead"],
-            [2, 2, 1, "", "location"],
-            [2, 2, 1, "", "lock_work_records_date"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "project_group"],
-            [2, 2, 1, "", "project_id"],
-            [2, 2, 1, "", "start"],
-            [2, 2, 1, "", "tracker_prefix"]
-        ],
-        "pylero.project_group": [
-            [2, 1, 1, "", "ProjectGroup"]
-        ],
-        "pylero.project_group.ProjectGroup": [
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "get_contained_groups"],
-            [2, 3, 1, "", "get_contained_projects"],
-            [2, 3, 1, "", "get_deep_contained_projects"],
-            [2, 3, 1, "", "get_root_project_group"],
-            [2, 2, 1, "", "group_uris"],
-            [2, 2, 1, "", "location"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "parent_uri"],
-            [2, 2, 1, "", "project_ids"]
-        ],
-        "pylero.properties": [
-            [2, 1, 1, "", "Properties"]
-        ],
-        "pylero.properties.Properties": [
-            [2, 2, 1, "", "property"]
-        ],
-        "pylero.property": [
-            [2, 1, 1, "", "Property"]
-        ],
-        "pylero.property.Property": [
-            [2, 2, 1, "", "key"],
-            [2, 2, 1, "", "value"]
-        ],
-        "pylero.revision": [
-            [2, 1, 1, "", "ArrayOfRevision"],
-            [2, 1, 1, "", "Revision"]
-        ],
-        "pylero.revision.Revision": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "internal_commit"],
-            [2, 2, 1, "", "linked_work_item_uris"],
-            [2, 2, 1, "", "message"],
-            [2, 2, 1, "", "name"],
-            [2, 3, 1, "", "query"],
-            [2, 2, 1, "", "repository_name"]
-        ],
-        "pylero.server": [
-            [2, 1, 1, "", "Server"]
-        ],
-        "pylero.server.Server": [
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "session"]
-        ],
-        "pylero.session": [
-            [2, 1, 1, "", "ListenFilter"],
-            [2, 1, 1, "", "Session"],
-            [2, 1, 1, "", "SoapNull"],
-            [2, 4, 1, "", "create_ssl_context"]
-        ],
-        "pylero.session.ListenFilter": [
-            [2, 3, 1, "", "filter"]
-        ],
-        "pylero.session.Session": [
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "tx_begin"],
-            [2, 3, 1, "", "tx_commit"],
-            [2, 3, 1, "", "tx_in"],
-            [2, 3, 1, "", "tx_release"],
-            [2, 3, 1, "", "tx_rollback"]
-        ],
-        "pylero.session.SoapNull": [
-            [2, 3, 1, "", "add_nil"],
-            [2, 3, 1, "", "marshalled"]
-        ],
-        "pylero.signature": [
-            [2, 1, 1, "", "ArrayOfSignature"],
-            [2, 1, 1, "", "Signature"]
-        ],
-        "pylero.signature.Signature": [
-            [2, 2, 1, "", "signed_by"],
-            [2, 2, 1, "", "signed_revision"],
-            [2, 2, 1, "", "signer_role"],
-            [2, 2, 1, "", "verdict"],
-            [2, 2, 1, "", "verdict_time"]
-        ],
-        "pylero.signature_context": [
-            [2, 1, 1, "", "ArrayOfSignatureContext"],
-            [2, 1, 1, "", "SignatureContext"]
-        ],
-        "pylero.signature_context.SignatureContext": [
-            [2, 2, 1, "", "signatures"],
-            [2, 2, 1, "", "target_status_id"],
-            [2, 2, 1, "", "transition_data_revision"],
-            [2, 2, 1, "", "user"]
-        ],
-        "pylero.signature_data": [
-            [2, 1, 1, "", "SignatureData"]
-        ],
-        "pylero.signature_data.SignatureData": [
-            [2, 2, 1, "", "target_status_id"],
-            [2, 2, 1, "", "verdict"]
-        ],
-        "pylero.subterra_uri": [
-            [2, 1, 1, "", "ArrayOfSubterraURI"],
-            [2, 1, 1, "", "SubterraURI"]
-        ],
-        "pylero.subterra_uri.ArrayOfSubterraURI": [
-            [2, 3, 1, "", "__init__"]
-        ],
-        "pylero.subterra_uri.SubterraURI": [
-            [2, 3, 1, "", "__init__"]
-        ],
-        "pylero.test_record": [
-            [2, 1, 1, "", "ArrayOfTestRecord"],
-            [2, 1, 1, "", "TestRecord"]
-        ],
-        "pylero.test_record.TestRecord": [
-            [2, 3, 1, "", "__init__"]
-        ],
-        "pylero.test_run": [
-            [2, 1, 1, "", "TestRun"],
-            [2, 4, 1, "", "create_incident_report"],
-            [2, 4, 1, "", "generate_description"]
-        ],
-        "pylero.test_run.TestRun": [
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "add_attachment"],
-            [2, 3, 1, "", "add_attachment_to_test_record"],
-            [2, 3, 1, "", "add_attachment_to_test_step"],
-            [2, 3, 1, "", "add_test_record_by_fields"],
-            [2, 3, 1, "", "add_test_record_by_object"],
-            [2, 2, 1, "", "attachments"],
-            [2, 2, 1, "", "author"],
-            [2, 3, 1, "", "create"],
-            [2, 3, 1, "", "create_summary_defect"],
-            [2, 3, 1, "", "create_template"],
-            [2, 2, 1, "", "created"],
-            [2, 2, 1, "", "custom_fields"],
-            [2, 3, 1, "", "delete_attachment"],
-            [2, 3, 1, "", "delete_attachment_from_test_record"],
-            [2, 3, 1, "", "delete_attachment_from_test_step"],
-            [2, 2, 1, "", "document"],
-            [2, 2, 1, "", "finished_on"],
-            [2, 3, 1, "", "get_attachment"],
-            [2, 3, 1, "", "get_attachments"],
-            [2, 3, 1, "", "get_custom_field"],
-            [2, 3, 1, "", "get_defined_custom_field_types"],
-            [2, 3, 1, "", "get_wiki_content"],
-            [2, 2, 1, "", "group_id"],
-            [2, 2, 1, "", "is_template"],
-            [2, 2, 1, "", "keep_in_history"],
-            [2, 2, 1, "", "location"],
-            [2, 2, 1, "", "project"],
-            [2, 2, 1, "", "query"],
-            [2, 6, 1, "id2", "records"],
-            [2, 3, 1, "", "search"],
-            [2, 2, 1, "", "select_test_cases_by"],
-            [2, 2, 1, "", "status"],
-            [2, 2, 1, "", "summary_defect"],
-            [2, 2, 1, "", "template"],
-            [2, 2, 1, "", "test_run_id"],
-            [2, 2, 1, "", "type"],
-            [2, 3, 1, "", "update"],
-            [2, 3, 1, "", "update_attachment"],
-            [2, 3, 1, "", "update_summary_defect"],
-            [2, 3, 1, "", "update_test_record_by_fields"],
-            [2, 3, 1, "", "update_test_record_by_object"],
-            [2, 3, 1, "", "update_wiki_content"],
-            [2, 2, 1, "", "updated"],
-            [2, 3, 1, "", "verify_params"],
-            [2, 3, 1, "", "verify_required"]
-        ],
-        "pylero.test_run_attachment": [
-            [2, 1, 1, "", "ArrayOfTestRunAttachment"],
-            [2, 1, 1, "", "TestRunAttachment"]
-        ],
-        "pylero.test_run_attachment.TestRunAttachment": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "file_name"],
-            [2, 2, 1, "", "id"],
-            [2, 2, 1, "", "length"],
-            [2, 2, 1, "", "test_run_uri"],
-            [2, 2, 1, "", "title"],
-            [2, 2, 1, "", "updated"],
-            [2, 2, 1, "", "url"]
-        ],
-        "pylero.test_step": [
-            [2, 1, 1, "", "ArrayOfTestStep"],
-            [2, 1, 1, "", "TestStep"]
-        ],
-        "pylero.test_step.TestStep": [
-            [2, 2, 1, "", "values"]
-        ],
-        "pylero.test_step_result": [
-            [2, 1, 1, "", "ArrayOfTestStepResult"],
-            [2, 1, 1, "", "TestStepResult"]
-        ],
-        "pylero.test_step_result.TestStepResult": [
-            [2, 2, 1, "", "attachments"],
-            [2, 2, 1, "", "comment"],
-            [2, 2, 1, "", "result"]
-        ],
-        "pylero.test_steps": [
-            [2, 1, 1, "", "TestSteps"]
-        ],
-        "pylero.test_steps.TestSteps": [
-            [2, 2, 1, "", "keys"],
-            [2, 2, 1, "", "steps"]
-        ],
-        "pylero.tests_configuration": [
-            [2, 1, 1, "", "TestsConfiguration"]
-        ],
-        "pylero.tests_configuration.TestsConfiguration": [
-            [2, 2, 1, "", "defect_auto_assignement_enabled"],
-            [2, 2, 1, "", "defect_reuse_type"],
-            [2, 2, 1, "", "defect_template"],
-            [2, 2, 1, "", "defect_to_test_case_link_role_id"],
-            [2, 2, 1, "", "defect_work_item_type"],
-            [2, 2, 1, "", "defects_project"],
-            [2, 2, 1, "", "fields_to_copy_from_test_case_to_defect"],
-            [2, 2, 1, "", "fields_to_copy_from_test_run_to_linked_defect"],
-            [2, 2, 1, "", "fields_to_copy_from_test_run_to_new_defect"],
-            [2, 2, 1, "", "max_created_defects"],
-            [2, 2, 1, "", "max_created_defects_percent"],
-            [2, 2, 1, "", "result_error_enum_id"],
-            [2, 2, 1, "", "result_failed_enum_id"],
-            [2, 2, 1, "", "result_passed_enum_id"],
-            [2, 2, 1, "", "retest_allowed"],
-            [2, 2, 1, "", "status_error_enum_id"],
-            [2, 2, 1, "", "status_failed_enum_id"],
-            [2, 2, 1, "", "status_ok_enum_id"],
-            [2, 2, 1, "", "summary_defect_severity"],
-            [2, 2, 1, "", "test_case_id_custom_field"],
-            [2, 2, 1, "", "test_case_template"],
-            [2, 2, 1, "", "test_case_test_comment_field_id"],
-            [2, 2, 1, "", "test_case_test_result_field_id"],
-            [2, 2, 1, "", "test_case_work_item_type"],
-            [2, 2, 1, "", "test_run_template"]
-        ],
-        "pylero.text": [
-            [2, 1, 1, "", "ArrayOfText"],
-            [2, 1, 1, "", "Text"]
-        ],
-        "pylero.text.Text": [
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "content"],
-            [2, 2, 1, "", "content_lossy"],
-            [2, 2, 1, "", "content_type"]
-        ],
-        "pylero.time_point": [
-            [2, 1, 1, "", "TimePoint"]
-        ],
-        "pylero.time_point.TimePoint": [
-            [2, 2, 1, "", "closed"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "earliest_planned_start"],
-            [2, 2, 1, "", "name"],
-            [2, 2, 1, "", "time"],
-            [2, 2, 1, "", "time_point_id"]
-        ],
-        "pylero.user": [
-            [2, 1, 1, "", "ArrayOfUser"],
-            [2, 1, 1, "", "User"]
-        ],
-        "pylero.user.User": [
-            [2, 3, 1, "", "__init__"],
-            [2, 3, 1, "", "create_user"],
-            [2, 2, 1, "", "description"],
-            [2, 2, 1, "", "disabled_notifications"],
-            [2, 2, 1, "", "email"],
-            [2, 3, 1, "", "get_context_roles"],
-            [2, 3, 1, "", "get_roles"],
-            [2, 3, 1, "", "get_user_avatar_url"],
-            [2, 3, 1, "", "get_user_from_token"],
-            [2, 3, 1, "", "get_users"],
-            [2, 3, 1, "", "has_permission"],
-            [2, 2, 1, "", "name"],
-            [2, 3, 1, "", "update"],
-            [2, 2, 1, "", "user_id"],
-            [2, 2, 1, "", "vote_uris"],
-            [2, 2, 1, "", "watche_uris"]
-        ],
-        "pylero.wiki_page": [
-            [2, 1, 1, "", "WikiPage"]
-        ],
-        "pylero.wiki_page.WikiPage": [
-            [2, 3, 1, "", "__init__"],
-            [2, 2, 1, "", "attachments"],
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "created"],
-            [2, 3, 1, "", "get_wiki_pages"],
-            [2, 2, 1, "", "home_page_content"],
-            [2, 2, 1, "", "linked_page_uris"],
-            [2, 2, 1, "", "location"],
-            [2, 2, 1, "", "page_location"],
-            [2, 2, 1, "", "page_name"],
-            [2, 2, 1, "", "project"],
-            [2, 3, 1, "", "query"],
-            [2, 2, 1, "", "space_id"],
-            [2, 2, 1, "", "title"],
-            [2, 2, 1, "", "type"],
-            [2, 2, 1, "", "updated"],
-            [2, 2, 1, "", "updated_by"],
-            [2, 2, 1, "", "wiki_page_id"]
-        ],
-        "pylero.wiki_page_attachment": [
-            [2, 1, 1, "", "ArrayOfWikiPageAttachment"],
-            [2, 1, 1, "", "WikiPageAttachment"]
-        ],
-        "pylero.wiki_page_attachment.WikiPageAttachment": [
-            [2, 2, 1, "", "author"],
-            [2, 2, 1, "", "file_name"],
-            [2, 2, 1, "", "length"],
-            [2, 2, 1, "", "title"],
-            [2, 2, 1, "", "updated"],
-            [2, 2, 1, "", "url"],
-            [2, 2, 1, "", "wiki_page_attachment_id"]
-        ],
-        "pylero.work_item": [
-            [2, 1, 1, "", "BusinessCase"],
-            [2, 1, 1, "", "ChangeRequest"],
-            [2, 1, 1, "", "Defect"],
-            [2, 1, 1, "", "IncidentReport"],
-            [2, 1, 1, "", "Requirement"],
-            [2, 1, 1, "", "Risk"],
-            [2, 1, 1, "", "Task"],
-            [2, 1, 1, "", "TestCase"],
-            [2, 1, 1, "", "TestSuite"],
-            [2, 2, 1, "", "newclass"]
+    "alltitles": {
+        "Before you commit": [
+            [0, "before-you-commit"]
         ],
-        "pylero.work_record": [
-            [2, 1, 1, "", "ArrayOfWorkRecord"],
-            [2, 1, 1, "", "WorkRecord"]
+        "Configuration": [
+            [0, "configuration"]
         ],
-        "pylero.work_record.WorkRecord": [
-            [2, 2, 1, "", "comment"],
-            [2, 2, 1, "", "date"],
-            [2, 2, 1, "", "time_spent"],
-            [2, 2, 1, "", "type"],
-            [2, 2, 1, "", "user"],
-            [2, 2, 1, "", "work_record_id"]
+        "Copr": [
+            [0, "copr"]
         ],
-        "pylero.workflow_action": [
-            [2, 1, 1, "", "WorkflowAction"]
+        "Examples": [
+            [0, "examples"]
         ],
-        "pylero.workflow_action.WorkflowAction": [
-            [2, 2, 1, "", "action_id"],
-            [2, 2, 1, "", "action_name"],
-            [2, 2, 1, "", "cleaned_features"],
-            [2, 2, 1, "", "native_action_id"],
-            [2, 2, 1, "", "required_features"],
-            [2, 2, 1, "", "suggested_features"],
-            [2, 2, 1, "", "target_status"],
-            [2, 2, 1, "", "unavailability_message"]
-        ]
-    },
-    "objtypes": {
-        "0": "py:module",
-        "1": "py:class",
-        "2": "py:attribute",
-        "3": "py:method",
-        "4": "py:function",
-        "5": "py:exception",
-        "6": "py:property"
-    },
-    "objnames": {
-        "0": ["py", "module", "Python module"],
-        "1": ["py", "class", "Python class"],
-        "2": ["py", "attribute", "Python attribute"],
-        "3": ["py", "method", "Python method"],
-        "4": ["py", "function", "Python function"],
-        "5": ["py", "exception", "Python exception"],
-        "6": ["py", "property", "Python property"]
-    },
-    "titleterms": {
-        "welcom": 0,
-        "pylero": [0, 1, 2, 3],
-        "": 0,
-        "document": [0, 2],
-        "instal": 0,
-        "from": 0,
-        "pypi": 0,
-        "repo": 0,
-        "fedora": 0,
-        "epel": 0,
-        "configur": 0,
-        "requir": 0,
-        "usag": 0,
-        "exampl": 0,
-        "befor": 0,
-        "you": 0,
-        "commit": 0,
-        "rpm": 0,
-        "packag": [0, 2, 3],
-        "build": [0, 2],
-        "tito": 0,
-        "copr": 0,
-        "indic": 0,
-        "tabl": 0,
-        "subpackag": 2,
-        "submodul": [2, 3],
-        "activ": 2,
-        "modul": [2, 3],
-        "activity_com": 2,
-        "activity_custom_valu": 2,
-        "activity_custom_value_entri": 2,
-        "activity_sourc": 2,
-        "approv": 2,
-        "attach": 2,
-        "base_polarion": 2,
-        "baselin": 2,
-        "build_linked_work_item": 2,
-        "build_test_result": 2,
-        "categori": 2,
-        "chang": 2,
-        "comment": 2,
-        "custom": 2,
-        "custom_field": 2,
-        "custom_field_typ": 2,
-        "enum_custom_field_typ": 2,
-        "enum_opt": 2,
-        "enum_option_id": 2,
-        "except": 2,
-        "externally_linked_work_item": 2,
-        "field_diff": 2,
-        "hyperlink": 2,
-        "imported_com": 2,
-        "language_definit": 2,
-        "license_info": 2,
-        "linked_work_item": 2,
-        "module_com": 2,
-        "plan": 2,
-        "plan_record": 2,
-        "plan_statist": 2,
-        "planning_constraint": 2,
-        "priority_opt": 2,
-        "priority_option_id": 2,
-        "product_licens": 2,
-        "project": 2,
-        "project_group": 2,
-        "properti": 2,
-        "revis": 2,
-        "server": 2,
-        "session": 2,
-        "signatur": 2,
-        "signature_context": 2,
-        "signature_data": 2,
-        "subterra_uri": 2,
-        "test_record": 2,
-        "test_run": 2,
-        "test_run_attach": 2,
-        "test_step": 2,
-        "test_step_result": 2,
-        "tests_configur": 2,
-        "text": 2,
-        "time_point": 2,
-        "user": 2,
-        "wiki_pag": 2,
-        "wiki_page_attach": 2,
-        "work_item": 2,
-        "work_record": 2,
-        "workflow_act": 2,
-        "content": [2, 3],
-        "cli": 3,
-        "cmd": 3
-    },
-    "envversion": {
-        "sphinx.domains.c": 3,
-        "sphinx.domains.changeset": 1,
-        "sphinx.domains.citation": 1,
-        "sphinx.domains.cpp": 9,
-        "sphinx.domains.index": 1,
-        "sphinx.domains.javascript": 3,
-        "sphinx.domains.math": 2,
-        "sphinx.domains.python": 4,
-        "sphinx.domains.rst": 2,
-        "sphinx.domains.std": 2,
-        "sphinx.ext.todo": 2,
-        "sphinx.ext.viewcode": 1,
-        "sphinx": 60
-    },
-    "alltitles": {
-        "Welcome to pylero\u2019s documentation!": [
-            [0, "welcome-to-pyleros-documentation"]
+        "Fedora RPM package build": [
+            [0, "fedora-rpm-package-build"]
         ],
-        "Installation": [
-            [0, "installation"]
+        "Indices and tables": [
+            [0, "indices-and-tables"]
         ],
         "Install from Pypi": [
             [0, "install-from-pypi"]
         ],
         "Install from repo": [
             [0, "install-from-repo"]
         ],
         "Install on Fedora & EPEL": [
             [0, "install-on-fedora-epel"]
         ],
-        "Configuration": [
-            [0, "configuration"]
+        "Installation": [
+            [0, "installation"]
+        ],
+        "Module contents": [
+            [2, "module-pylero"],
+            [3, "module-pylero.cli"]
         ],
         "Requirements": [
             [0, "requirements"]
         ],
-        "Usage": [
-            [0, "usage"]
-        ],
-        "Examples": [
-            [0, "examples"]
-        ],
-        "Before you commit": [
-            [0, "before-you-commit"]
+        "Submodules": [
+            [2, "submodules"],
+            [3, "submodules"]
         ],
-        "Fedora RPM package build": [
-            [0, "fedora-rpm-package-build"]
+        "Subpackages": [
+            [2, "subpackages"]
         ],
         "Tito": [
             [0, "tito"]
         ],
-        "Copr": [
-            [0, "copr"]
+        "Usage": [
+            [0, "usage"]
         ],
-        "Indices and tables": [
-            [0, "indices-and-tables"]
+        "Welcome to pylero\u2019s documentation!": [
+            [0, "welcome-to-pyleros-documentation"]
         ],
         "pylero": [
             [1, "pylero"]
         ],
         "pylero package": [
             [2, "pylero-package"]
         ],
-        "Subpackages": [
-            [2, "subpackages"]
-        ],
-        "Submodules": [
-            [2, "submodules"],
-            [3, "submodules"]
-        ],
         "pylero.activity module": [
             [2, "module-pylero.activity"]
         ],
         "pylero.activity_comment module": [
             [2, "module-pylero.activity_comment"]
         ],
         "pylero.activity_custom_value module": [
@@ -2526,14 +97,20 @@
         ],
         "pylero.category module": [
             [2, "module-pylero.category"]
         ],
         "pylero.change module": [
             [2, "module-pylero.change"]
         ],
+        "pylero.cli package": [
+            [3, "pylero-cli-package"]
+        ],
+        "pylero.cli.cmd module": [
+            [3, "module-pylero.cli.cmd"]
+        ],
         "pylero.comment module": [
             [2, "module-pylero.comment"]
         ],
         "pylero.custom module": [
             [2, "module-pylero.custom"]
         ],
         "pylero.custom_field module": [
@@ -2675,2256 +252,4691 @@
             [2, "module-pylero.work_item"]
         ],
         "pylero.work_record module": [
             [2, "module-pylero.work_record"]
         ],
         "pylero.workflow_action module": [
             [2, "module-pylero.workflow_action"]
-        ],
-        "Module contents": [
-            [2, "module-pylero"],
-            [3, "module-pylero.cli"]
-        ],
-        "pylero.cli package": [
-            [3, "pylero-cli-package"]
-        ],
-        "pylero.cli.cmd module": [
-            [3, "module-pylero.cli.cmd"]
         ]
     },
+    "docnames": ["index", "modules", "pylero", "pylero.cli"],
+    "envversion": {
+        "sphinx": 61,
+        "sphinx.domains.c": 3,
+        "sphinx.domains.changeset": 1,
+        "sphinx.domains.citation": 1,
+        "sphinx.domains.cpp": 9,
+        "sphinx.domains.index": 1,
+        "sphinx.domains.javascript": 3,
+        "sphinx.domains.math": 2,
+        "sphinx.domains.python": 4,
+        "sphinx.domains.rst": 2,
+        "sphinx.domains.std": 2,
+        "sphinx.ext.todo": 2,
+        "sphinx.ext.viewcode": 1
+    },
+    "filenames": ["index.rst", "modules.rst", "pylero.rst", "pylero.cli.rst"],
     "indexentries": {
-        "activity (class in pylero.activity)": [
-            [2, "pylero.activity.Activity"]
-        ],
-        "activitycomment (class in pylero.activity_comment)": [
-            [2, "pylero.activity_comment.ActivityComment"]
-        ],
-        "activitycustomvalue (class in pylero.activity_custom_value)": [
-            [2, "pylero.activity_custom_value.ActivityCustomValue"]
-        ],
-        "activitycustomvalueentry (class in pylero.activity_custom_value_entry)": [
-            [2, "pylero.activity_custom_value_entry.ActivityCustomValueEntry"]
-        ],
-        "activitysource (class in pylero.activity_source)": [
-            [2, "pylero.activity_source.ActivitySource"]
-        ],
-        "approval (class in pylero.approval)": [
-            [2, "pylero.approval.Approval"]
-        ],
-        "arrayofapproval (class in pylero.approval)": [
-            [2, "pylero.approval.ArrayOfApproval"]
-        ],
-        "arrayofattachment (class in pylero.attachment)": [
-            [2, "pylero.attachment.ArrayOfAttachment"]
-        ],
-        "arrayofbuildlinkedworkitem (class in pylero.build_linked_work_item)": [
-            [2, "pylero.build_linked_work_item.ArrayOfBuildLinkedWorkItem"]
-        ],
-        "arrayofcategory (class in pylero.category)": [
-            [2, "pylero.category.ArrayOfCategory"]
-        ],
-        "arrayofcomment (class in pylero.comment)": [
-            [2, "pylero.comment.ArrayOfComment"]
-        ],
-        "arrayofcustom (class in pylero.custom)": [
-            [2, "pylero.custom.ArrayOfCustom"]
-        ],
-        "arrayofenumoptionid (class in pylero.enum_option_id)": [
-            [2, "pylero.enum_option_id.ArrayOfEnumOptionId"]
-        ],
-        "arrayofexternallylinkedworkitem (class in pylero.externally_linked_work_item)": [
-            [2, "pylero.externally_linked_work_item.ArrayOfExternallyLinkedWorkItem"]
-        ],
-        "arrayofhyperlink (class in pylero.hyperlink)": [
-            [2, "pylero.hyperlink.ArrayOfHyperlink"]
-        ],
-        "arrayoflinkedworkitem (class in pylero.linked_work_item)": [
-            [2, "pylero.linked_work_item.ArrayOfLinkedWorkItem"]
-        ],
-        "arrayofmodulecomment (class in pylero.module_comment)": [
-            [2, "pylero.module_comment.ArrayOfModuleComment"]
-        ],
-        "arrayofplan (class in pylero.plan)": [
-            [2, "pylero.plan.ArrayOfPlan"]
-        ],
-        "arrayofplanrecord (class in pylero.plan_record)": [
-            [2, "pylero.plan_record.ArrayOfPlanRecord"]
-        ],
-        "arrayofplanningconstraint (class in pylero.planning_constraint)": [
-            [2, "pylero.planning_constraint.ArrayOfPlanningConstraint"]
-        ],
-        "arrayofpriorityoptionid (class in pylero.priority_option_id)": [
-            [2, "pylero.priority_option_id.ArrayOfPriorityOptionId"]
-        ],
-        "arrayofrevision (class in pylero.revision)": [
-            [2, "pylero.revision.ArrayOfRevision"]
-        ],
-        "arrayofsignature (class in pylero.signature)": [
-            [2, "pylero.signature.ArrayOfSignature"]
-        ],
-        "arrayofsignaturecontext (class in pylero.signature_context)": [
-            [2, "pylero.signature_context.ArrayOfSignatureContext"]
-        ],
-        "arrayofsubterrauri (class in pylero.subterra_uri)": [
-            [2, "pylero.subterra_uri.ArrayOfSubterraURI"]
-        ],
-        "arrayoftestrecord (class in pylero.test_record)": [
-            [2, "pylero.test_record.ArrayOfTestRecord"]
-        ],
-        "arrayoftestrunattachment (class in pylero.test_run_attachment)": [
-            [2, "pylero.test_run_attachment.ArrayOfTestRunAttachment"]
-        ],
-        "arrayofteststep (class in pylero.test_step)": [
-            [2, "pylero.test_step.ArrayOfTestStep"]
-        ],
-        "arrayofteststepresult (class in pylero.test_step_result)": [
-            [2, "pylero.test_step_result.ArrayOfTestStepResult"]
-        ],
-        "arrayoftext (class in pylero.text)": [
-            [2, "pylero.text.ArrayOfText"]
-        ],
-        "arrayofuser (class in pylero.user)": [
-            [2, "pylero.user.ArrayOfUser"]
-        ],
-        "arrayofwikipageattachment (class in pylero.wiki_page_attachment)": [
-            [2, "pylero.wiki_page_attachment.ArrayOfWikiPageAttachment"]
-        ],
-        "arrayofworkrecord (class in pylero.work_record)": [
-            [2, "pylero.work_record.ArrayOfWorkRecord"]
-        ],
-        "attachment (class in pylero.attachment)": [
-            [2, "pylero.attachment.Attachment"]
-        ],
-        "basepolarion (class in pylero.base_polarion)": [
-            [2, "pylero.base_polarion.BasePolarion"]
-        ],
-        "baseline (class in pylero.baseline)": [
-            [2, "pylero.baseline.Baseline"]
-        ],
-        "build (class in pylero.build)": [
-            [2, "pylero.build.Build"]
-        ],
-        "buildlinkedworkitem (class in pylero.build_linked_work_item)": [
-            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem"]
-        ],
-        "buildtestresults (class in pylero.build_test_results)": [
-            [2, "pylero.build_test_results.BuildTestResults"]
-        ],
-        "businesscase (class in pylero.work_item)": [
-            [2, "pylero.work_item.BusinessCase"]
-        ],
-        "config_section (pylero.base_polarion.configuration attribute)": [
-            [2, "pylero.base_polarion.Configuration.CONFIG_SECTION"]
-        ],
-        "curdir_config (pylero.base_polarion.configuration attribute)": [
-            [2, "pylero.base_polarion.Configuration.CURDIR_CONFIG"]
-        ],
-        "category (class in pylero.category)": [
-            [2, "pylero.category.Category"]
-        ],
-        "change (class in pylero.change)": [
-            [2, "pylero.change.Change"]
-        ],
-        "changerequest (class in pylero.work_item)": [
-            [2, "pylero.work_item.ChangeRequest"]
-        ],
-        "classproperty (class in pylero.base_polarion)": [
-            [2, "pylero.base_polarion.ClassProperty"]
-        ],
-        "comment (class in pylero.comment)": [
-            [2, "pylero.comment.Comment"]
-        ],
-        "configuration (class in pylero.base_polarion)": [
-            [2, "pylero.base_polarion.Configuration"]
-        ],
-        "connection (class in pylero.base_polarion)": [
-            [2, "pylero.base_polarion.Connection"]
-        ],
-        "custom (class in pylero.custom)": [
-            [2, "pylero.custom.Custom"]
-        ],
-        "customfield (class in pylero.custom_field)": [
-            [2, "pylero.custom_field.CustomField"]
-        ],
-        "customfieldtype (class in pylero.custom_field_type)": [
-            [2, "pylero.custom_field_type.CustomFieldType"]
-        ],
-        "defect (class in pylero.work_item)": [
-            [2, "pylero.work_item.Defect"]
-        ],
-        "document (class in pylero.document)": [
-            [2, "pylero.document.Document"]
-        ],
-        "enumcustomfieldtype (class in pylero.enum_custom_field_type)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType"]
-        ],
-        "enumoption (class in pylero.enum_option)": [
-            [2, "pylero.enum_option.EnumOption"]
-        ],
-        "enumoptionid (class in pylero.enum_option_id)": [
-            [2, "pylero.enum_option_id.EnumOptionId"]
-        ],
-        "externallylinkedworkitem (class in pylero.externally_linked_work_item)": [
-            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem"]
-        ],
-        "fielddiff (class in pylero.field_diff)": [
-            [2, "pylero.field_diff.FieldDiff"]
-        ],
-        "global_config (pylero.base_polarion.configuration attribute)": [
-            [2, "pylero.base_polarion.Configuration.GLOBAL_CONFIG"]
-        ],
-        "hyperlink (class in pylero.hyperlink)": [
-            [2, "pylero.hyperlink.Hyperlink"]
-        ],
-        "importedcomment (class in pylero.imported_comment)": [
-            [2, "pylero.imported_comment.ImportedComment"]
-        ],
-        "incidentreport (class in pylero.work_item)": [
-            [2, "pylero.work_item.IncidentReport"]
-        ],
-        "local_config (pylero.base_polarion.configuration attribute)": [
-            [2, "pylero.base_polarion.Configuration.LOCAL_CONFIG"]
-        ],
-        "languagedefinition (class in pylero.language_definition)": [
-            [2, "pylero.language_definition.LanguageDefinition"]
-        ],
-        "licenseinfo (class in pylero.license_info)": [
-            [2, "pylero.license_info.LicenseInfo"]
-        ],
-        "linkedworkitem (class in pylero.linked_work_item)": [
-            [2, "pylero.linked_work_item.LinkedWorkItem"]
-        ],
-        "listenfilter (class in pylero.session)": [
-            [2, "pylero.session.ListenFilter"]
-        ],
-        "modulecomment (class in pylero.module_comment)": [
-            [2, "pylero.module_comment.ModuleComment"]
-        ],
-        "plan (class in pylero.plan)": [
-            [2, "pylero.plan.Plan"]
-        ],
-        "planrecord (class in pylero.plan_record)": [
-            [2, "pylero.plan_record.PlanRecord"]
-        ],
-        "planstatistics (class in pylero.plan_statistics)": [
-            [2, "pylero.plan_statistics.PlanStatistics"]
-        ],
-        "planningconstraint (class in pylero.planning_constraint)": [
-            [2, "pylero.planning_constraint.PlanningConstraint"]
-        ],
-        "priorityopt (class in pylero.priority_opt)": [
-            [2, "pylero.priority_opt.PriorityOpt"]
-        ],
-        "priorityoptionid (class in pylero.priority_option_id)": [
-            [2, "pylero.priority_option_id.PriorityOptionId"]
-        ],
-        "productlicense (class in pylero.product_license)": [
-            [2, "pylero.product_license.ProductLicense"]
-        ],
-        "project (class in pylero.project)": [
-            [2, "pylero.project.Project"]
-        ],
-        "projectgroup (class in pylero.project_group)": [
-            [2, "pylero.project_group.ProjectGroup"]
-        ],
-        "properties (class in pylero.properties)": [
-            [2, "pylero.properties.Properties"]
-        ],
-        "property (class in pylero.property)": [
-            [2, "pylero.property.Property"]
-        ],
-        "pylerolibexception": [
-            [2, "pylero.exceptions.PyleroLibException"]
-        ],
-        "regex_id (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion.REGEX_ID"]
-        ],
-        "regex_proj (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion.REGEX_PROJ"]
-        ],
-        "requirement (class in pylero.work_item)": [
-            [2, "pylero.work_item.Requirement"]
-        ],
-        "revision (class in pylero.revision)": [
-            [2, "pylero.revision.Revision"]
-        ],
-        "risk (class in pylero.work_item)": [
-            [2, "pylero.work_item.Risk"]
-        ],
-        "server (class in pylero.server)": [
-            [2, "pylero.server.Server"]
-        ],
-        "session (class in pylero.session)": [
-            [2, "pylero.session.Session"]
-        ],
-        "signature (class in pylero.signature)": [
-            [2, "pylero.signature.Signature"]
-        ],
-        "signaturecontext (class in pylero.signature_context)": [
-            [2, "pylero.signature_context.SignatureContext"]
-        ],
-        "signaturedata (class in pylero.signature_data)": [
-            [2, "pylero.signature_data.SignatureData"]
-        ],
-        "soapnull (class in pylero.session)": [
-            [2, "pylero.session.SoapNull"]
-        ],
-        "subterrauri (class in pylero.subterra_uri)": [
-            [2, "pylero.subterra_uri.SubterraURI"]
-        ],
-        "task (class in pylero.work_item)": [
-            [2, "pylero.work_item.Task"]
-        ],
-        "testcase (class in pylero.work_item)": [
-            [2, "pylero.work_item.TestCase"]
-        ],
-        "testrecord (class in pylero.test_record)": [
-            [2, "pylero.test_record.TestRecord"]
-        ],
-        "testrun (class in pylero.test_run)": [
-            [2, "pylero.test_run.TestRun"]
-        ],
-        "testrunattachment (class in pylero.test_run_attachment)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment"]
-        ],
-        "teststep (class in pylero.test_step)": [
-            [2, "pylero.test_step.TestStep"]
-        ],
-        "teststepresult (class in pylero.test_step_result)": [
-            [2, "pylero.test_step_result.TestStepResult"]
-        ],
-        "teststeps (class in pylero.test_steps)": [
-            [2, "pylero.test_steps.TestSteps"]
-        ],
-        "testsuite (class in pylero.work_item)": [
-            [2, "pylero.work_item.TestSuite"]
-        ],
-        "testsconfiguration (class in pylero.tests_configuration)": [
-            [2, "pylero.tests_configuration.TestsConfiguration"]
-        ],
-        "text (class in pylero.text)": [
-            [2, "pylero.text.Text"]
-        ],
-        "timepoint (class in pylero.time_point)": [
-            [2, "pylero.time_point.TimePoint"]
-        ],
-        "uri_id_get_replace() (pylero.base_polarion.basepolarion class method)": [
-            [2, "pylero.base_polarion.BasePolarion.URI_ID_GET_REPLACE"]
-        ],
-        "uri_id_get_replace() (pylero.document.document class method)": [
-            [2, "pylero.document.Document.URI_ID_GET_REPLACE"]
-        ],
-        "uri_id_set_replace() (pylero.base_polarion.basepolarion class method)": [
-            [2, "pylero.base_polarion.BasePolarion.URI_ID_SET_REPLACE"]
-        ],
-        "uri_id_set_replace() (pylero.document.document class method)": [
-            [2, "pylero.document.Document.URI_ID_SET_REPLACE"]
-        ],
-        "uri_struct (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion.URI_STRUCT"]
-        ],
-        "uri_struct (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.URI_STRUCT"]
-        ],
-        "uri_struct (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.URI_STRUCT"]
-        ],
-        "user (class in pylero.user)": [
-            [2, "pylero.user.User"]
-        ],
-        "wikipage (class in pylero.wiki_page)": [
-            [2, "pylero.wiki_page.WikiPage"]
-        ],
-        "wikipageattachment (class in pylero.wiki_page_attachment)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment"]
-        ],
-        "workrecord (class in pylero.work_record)": [
-            [2, "pylero.work_record.WorkRecord"]
-        ],
-        "workflowaction (class in pylero.workflow_action)": [
-            [2, "pylero.workflow_action.WorkflowAction"]
-        ],
         "__init__() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.__init__"]
+            [2, "pylero.base_polarion.BasePolarion.__init__", false]
         ],
         "__init__() (pylero.base_polarion.configuration method)": [
-            [2, "pylero.base_polarion.Configuration.__init__"]
+            [2, "pylero.base_polarion.Configuration.__init__", false]
         ],
         "__init__() (pylero.custom.custom method)": [
-            [2, "pylero.custom.Custom.__init__"]
+            [2, "pylero.custom.Custom.__init__", false]
         ],
         "__init__() (pylero.document.document method)": [
-            [2, "pylero.document.Document.__init__"]
+            [2, "pylero.document.Document.__init__", false]
         ],
         "__init__() (pylero.enum_option_id.enumoptionid method)": [
-            [2, "pylero.enum_option_id.EnumOptionId.__init__"]
+            [2, "pylero.enum_option_id.EnumOptionId.__init__", false]
         ],
         "__init__() (pylero.externally_linked_work_item.externallylinkedworkitem method)": [
-            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem.__init__"]
+            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem.__init__", false]
         ],
         "__init__() (pylero.linked_work_item.linkedworkitem method)": [
-            [2, "pylero.linked_work_item.LinkedWorkItem.__init__"]
+            [2, "pylero.linked_work_item.LinkedWorkItem.__init__", false]
         ],
         "__init__() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.__init__"]
+            [2, "pylero.plan.Plan.__init__", false]
         ],
         "__init__() (pylero.priority_option_id.priorityoptionid method)": [
-            [2, "pylero.priority_option_id.PriorityOptionId.__init__"]
+            [2, "pylero.priority_option_id.PriorityOptionId.__init__", false]
         ],
         "__init__() (pylero.project.project method)": [
-            [2, "pylero.project.Project.__init__"]
+            [2, "pylero.project.Project.__init__", false]
         ],
         "__init__() (pylero.project_group.projectgroup method)": [
-            [2, "pylero.project_group.ProjectGroup.__init__"]
+            [2, "pylero.project_group.ProjectGroup.__init__", false]
         ],
         "__init__() (pylero.server.server method)": [
-            [2, "pylero.server.Server.__init__"]
+            [2, "pylero.server.Server.__init__", false]
         ],
         "__init__() (pylero.session.session method)": [
-            [2, "pylero.session.Session.__init__"]
+            [2, "pylero.session.Session.__init__", false]
         ],
         "__init__() (pylero.subterra_uri.arrayofsubterrauri method)": [
-            [2, "pylero.subterra_uri.ArrayOfSubterraURI.__init__"]
+            [2, "pylero.subterra_uri.ArrayOfSubterraURI.__init__", false]
         ],
         "__init__() (pylero.subterra_uri.subterrauri method)": [
-            [2, "pylero.subterra_uri.SubterraURI.__init__"]
+            [2, "pylero.subterra_uri.SubterraURI.__init__", false]
         ],
         "__init__() (pylero.test_record.testrecord method)": [
-            [2, "pylero.test_record.TestRecord.__init__"]
+            [2, "pylero.test_record.TestRecord.__init__", false]
         ],
         "__init__() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.__init__"]
+            [2, "pylero.test_run.TestRun.__init__", false]
         ],
         "__init__() (pylero.text.text method)": [
-            [2, "pylero.text.Text.__init__"]
+            [2, "pylero.text.Text.__init__", false]
         ],
         "__init__() (pylero.user.user method)": [
-            [2, "pylero.user.User.__init__"]
+            [2, "pylero.user.User.__init__", false]
         ],
         "__init__() (pylero.wiki_page.wikipage method)": [
-            [2, "pylero.wiki_page.WikiPage.__init__"]
+            [2, "pylero.wiki_page.WikiPage.__init__", false]
         ],
         "_cls_suds_map (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion._cls_suds_map"]
+            [2, "pylero.base_polarion.BasePolarion._cls_suds_map", false]
         ],
         "_id_field (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion._id_field"]
+            [2, "pylero.base_polarion.BasePolarion._id_field", false]
         ],
         "_obj_client (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion._obj_client"]
+            [2, "pylero.base_polarion.BasePolarion._obj_client", false]
         ],
         "_obj_struct (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion._obj_struct"]
+            [2, "pylero.base_polarion.BasePolarion._obj_struct", false]
         ],
         "action_id (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.action_id"]
+            [2, "pylero.workflow_action.WorkflowAction.action_id", false]
         ],
         "action_name (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.action_name"]
+            [2, "pylero.workflow_action.WorkflowAction.action_name", false]
         ],
         "active (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.active"]
+            [2, "pylero.project.Project.active", false]
+        ],
+        "activity (class in pylero.activity)": [
+            [2, "pylero.activity.Activity", false]
         ],
         "activity_custom_values (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.activity_custom_values"]
+            [2, "pylero.activity.Activity.activity_custom_values", false]
         ],
         "activity_id (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.activity_id"]
+            [2, "pylero.activity.Activity.activity_id", false]
         ],
         "activity_source_id (pylero.activity_source.activitysource attribute)": [
-            [2, "pylero.activity_source.ActivitySource.activity_source_id"]
+            [2, "pylero.activity_source.ActivitySource.activity_source_id", false]
+        ],
+        "activitycomment (class in pylero.activity_comment)": [
+            [2, "pylero.activity_comment.ActivityComment", false]
+        ],
+        "activitycustomvalue (class in pylero.activity_custom_value)": [
+            [2, "pylero.activity_custom_value.ActivityCustomValue", false]
+        ],
+        "activitycustomvalueentry (class in pylero.activity_custom_value_entry)": [
+            [2, "pylero.activity_custom_value_entry.ActivityCustomValueEntry", false]
+        ],
+        "activitysource (class in pylero.activity_source)": [
+            [2, "pylero.activity_source.ActivitySource", false]
         ],
         "add_attachment() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.add_attachment"]
+            [2, "pylero.test_run.TestRun.add_attachment", false]
         ],
         "add_attachment_to_test_record() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.add_attachment_to_test_record"]
+            [2, "pylero.test_run.TestRun.add_attachment_to_test_record", false]
         ],
         "add_attachment_to_test_step() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.add_attachment_to_test_step"]
+            [2, "pylero.test_run.TestRun.add_attachment_to_test_step", false]
         ],
         "add_nil() (pylero.session.soapnull method)": [
-            [2, "pylero.session.SoapNull.add_nil"]
+            [2, "pylero.session.SoapNull.add_nil", false]
         ],
         "add_plan_items() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.add_plan_items"]
+            [2, "pylero.plan.Plan.add_plan_items", false]
         ],
         "add_referenced_work_item() (pylero.document.document method)": [
-            [2, "pylero.document.Document.add_referenced_work_item"]
+            [2, "pylero.document.Document.add_referenced_work_item", false]
         ],
         "add_test_record_by_fields() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.add_test_record_by_fields"]
+            [2, "pylero.test_run.TestRun.add_test_record_by_fields", false]
         ],
         "add_test_record_by_object() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.add_test_record_by_object"]
+            [2, "pylero.test_run.TestRun.add_test_record_by_object", false]
         ],
         "added (pylero.field_diff.fielddiff attribute)": [
-            [2, "pylero.field_diff.FieldDiff.added"]
+            [2, "pylero.field_diff.FieldDiff.added", false]
         ],
         "after (pylero.field_diff.fielddiff attribute)": [
-            [2, "pylero.field_diff.FieldDiff.after"]
+            [2, "pylero.field_diff.FieldDiff.after", false]
         ],
         "allowed_types (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.allowed_types"]
+            [2, "pylero.plan.Plan.allowed_types", false]
         ],
         "allowed_wi_types (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.allowed_wi_types"]
+            [2, "pylero.document.Document.allowed_wi_types", false]
+        ],
+        "approval (class in pylero.approval)": [
+            [2, "pylero.approval.Approval", false]
         ],
         "are_links_from_parent_to_child (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.are_links_from_parent_to_child"]
+            [2, "pylero.document.Document.are_links_from_parent_to_child", false]
+        ],
+        "arrayofapproval (class in pylero.approval)": [
+            [2, "pylero.approval.ArrayOfApproval", false]
+        ],
+        "arrayofattachment (class in pylero.attachment)": [
+            [2, "pylero.attachment.ArrayOfAttachment", false]
+        ],
+        "arrayofbuildlinkedworkitem (class in pylero.build_linked_work_item)": [
+            [2, "pylero.build_linked_work_item.ArrayOfBuildLinkedWorkItem", false]
+        ],
+        "arrayofcategory (class in pylero.category)": [
+            [2, "pylero.category.ArrayOfCategory", false]
+        ],
+        "arrayofcomment (class in pylero.comment)": [
+            [2, "pylero.comment.ArrayOfComment", false]
+        ],
+        "arrayofcustom (class in pylero.custom)": [
+            [2, "pylero.custom.ArrayOfCustom", false]
+        ],
+        "arrayofenumoptionid (class in pylero.enum_option_id)": [
+            [2, "pylero.enum_option_id.ArrayOfEnumOptionId", false]
+        ],
+        "arrayofexternallylinkedworkitem (class in pylero.externally_linked_work_item)": [
+            [2, "pylero.externally_linked_work_item.ArrayOfExternallyLinkedWorkItem", false]
+        ],
+        "arrayofhyperlink (class in pylero.hyperlink)": [
+            [2, "pylero.hyperlink.ArrayOfHyperlink", false]
+        ],
+        "arrayoflinkedworkitem (class in pylero.linked_work_item)": [
+            [2, "pylero.linked_work_item.ArrayOfLinkedWorkItem", false]
+        ],
+        "arrayofmodulecomment (class in pylero.module_comment)": [
+            [2, "pylero.module_comment.ArrayOfModuleComment", false]
+        ],
+        "arrayofplan (class in pylero.plan)": [
+            [2, "pylero.plan.ArrayOfPlan", false]
+        ],
+        "arrayofplanningconstraint (class in pylero.planning_constraint)": [
+            [2, "pylero.planning_constraint.ArrayOfPlanningConstraint", false]
+        ],
+        "arrayofplanrecord (class in pylero.plan_record)": [
+            [2, "pylero.plan_record.ArrayOfPlanRecord", false]
+        ],
+        "arrayofpriorityoptionid (class in pylero.priority_option_id)": [
+            [2, "pylero.priority_option_id.ArrayOfPriorityOptionId", false]
+        ],
+        "arrayofrevision (class in pylero.revision)": [
+            [2, "pylero.revision.ArrayOfRevision", false]
+        ],
+        "arrayofsignature (class in pylero.signature)": [
+            [2, "pylero.signature.ArrayOfSignature", false]
+        ],
+        "arrayofsignaturecontext (class in pylero.signature_context)": [
+            [2, "pylero.signature_context.ArrayOfSignatureContext", false]
+        ],
+        "arrayofsubterrauri (class in pylero.subterra_uri)": [
+            [2, "pylero.subterra_uri.ArrayOfSubterraURI", false]
+        ],
+        "arrayoftestrecord (class in pylero.test_record)": [
+            [2, "pylero.test_record.ArrayOfTestRecord", false]
+        ],
+        "arrayoftestrunattachment (class in pylero.test_run_attachment)": [
+            [2, "pylero.test_run_attachment.ArrayOfTestRunAttachment", false]
+        ],
+        "arrayofteststep (class in pylero.test_step)": [
+            [2, "pylero.test_step.ArrayOfTestStep", false]
+        ],
+        "arrayofteststepresult (class in pylero.test_step_result)": [
+            [2, "pylero.test_step_result.ArrayOfTestStepResult", false]
+        ],
+        "arrayoftext (class in pylero.text)": [
+            [2, "pylero.text.ArrayOfText", false]
+        ],
+        "arrayofuser (class in pylero.user)": [
+            [2, "pylero.user.ArrayOfUser", false]
+        ],
+        "arrayofwikipageattachment (class in pylero.wiki_page_attachment)": [
+            [2, "pylero.wiki_page_attachment.ArrayOfWikiPageAttachment", false]
+        ],
+        "arrayofworkrecord (class in pylero.work_record)": [
+            [2, "pylero.work_record.ArrayOfWorkRecord", false]
+        ],
+        "attachment (class in pylero.attachment)": [
+            [2, "pylero.attachment.Attachment", false]
         ],
         "attachment_id (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.attachment_id"]
+            [2, "pylero.attachment.Attachment.attachment_id", false]
         ],
         "attachments (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.attachments"]
+            [2, "pylero.test_run.TestRun.attachments", false]
         ],
         "attachments (pylero.test_step_result.teststepresult attribute)": [
-            [2, "pylero.test_step_result.TestStepResult.attachments"]
+            [2, "pylero.test_step_result.TestStepResult.attachments", false]
         ],
         "attachments (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.attachments"]
+            [2, "pylero.wiki_page.WikiPage.attachments", false]
         ],
         "author (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.author"]
+            [2, "pylero.attachment.Attachment.author", false]
         ],
         "author (pylero.baseline.baseline attribute)": [
-            [2, "pylero.baseline.Baseline.author"]
+            [2, "pylero.baseline.Baseline.author", false]
         ],
         "author (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.author"]
+            [2, "pylero.build.Build.author", false]
         ],
         "author (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.author"]
+            [2, "pylero.comment.Comment.author", false]
         ],
         "author (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.author"]
+            [2, "pylero.document.Document.author", false]
         ],
         "author (pylero.imported_comment.importedcomment attribute)": [
-            [2, "pylero.imported_comment.ImportedComment.author"]
+            [2, "pylero.imported_comment.ImportedComment.author", false]
         ],
         "author (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.author"]
+            [2, "pylero.module_comment.ModuleComment.author", false]
         ],
         "author (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.author"]
+            [2, "pylero.revision.Revision.author", false]
         ],
         "author (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.author"]
+            [2, "pylero.test_run.TestRun.author", false]
         ],
         "author (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.author"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.author", false]
         ],
         "author (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.author"]
+            [2, "pylero.wiki_page.WikiPage.author", false]
         ],
         "author (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.author"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.author", false]
         ],
         "author_uri (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.author_uri"]
+            [2, "pylero.plan.Plan.author_uri", false]
         ],
         "auto_suspect (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.auto_suspect"]
+            [2, "pylero.document.Document.auto_suspect", false]
         ],
         "base_revision (pylero.baseline.baseline attribute)": [
-            [2, "pylero.baseline.Baseline.base_revision"]
+            [2, "pylero.baseline.Baseline.base_revision", false]
+        ],
+        "baseline (class in pylero.baseline)": [
+            [2, "pylero.baseline.Baseline", false]
         ],
         "baseline_id (pylero.baseline.baseline attribute)": [
-            [2, "pylero.baseline.Baseline.baseline_id"]
+            [2, "pylero.baseline.Baseline.baseline_id", false]
+        ],
+        "basepolarion (class in pylero.base_polarion)": [
+            [2, "pylero.base_polarion.BasePolarion", false]
         ],
         "before (pylero.field_diff.fielddiff attribute)": [
-            [2, "pylero.field_diff.FieldDiff.before"]
+            [2, "pylero.field_diff.FieldDiff.before", false]
         ],
         "bir_location (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.bir_location"]
+            [2, "pylero.build.Build.bir_location", false]
         ],
         "branched_from (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.branched_from"]
+            [2, "pylero.document.Document.branched_from", false]
         ],
         "branched_with_query (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.branched_with_query"]
+            [2, "pylero.document.Document.branched_with_query", false]
+        ],
+        "build (class in pylero.build)": [
+            [2, "pylero.build.Build", false]
         ],
         "build_descriptor_name (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.build_descriptor_name"]
+            [2, "pylero.build.Build.build_descriptor_name", false]
         ],
         "build_id (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.build_id"]
+            [2, "pylero.build.Build.build_id", false]
         ],
         "build_stamp (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.build_stamp"]
+            [2, "pylero.build.Build.build_stamp", false]
         ],
         "build_status (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.build_status"]
+            [2, "pylero.build.Build.build_status", false]
         ],
         "build_tag (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.build_tag"]
+            [2, "pylero.build.Build.build_tag", false]
         ],
         "build_test_results (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.build_test_results"]
+            [2, "pylero.build.Build.build_test_results", false]
+        ],
+        "buildlinkedworkitem (class in pylero.build_linked_work_item)": [
+            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem", false]
+        ],
+        "buildtestresults (class in pylero.build_test_results)": [
+            [2, "pylero.build_test_results.BuildTestResults", false]
+        ],
+        "businesscase (class in pylero.work_item)": [
+            [2, "pylero.work_item.BusinessCase", false]
         ],
         "calculation_descriptor_name (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.calculation_descriptor_name"]
+            [2, "pylero.build.Build.calculation_descriptor_name", false]
         ],
         "calculation_type (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.calculation_type"]
+            [2, "pylero.plan.Plan.calculation_type", false]
         ],
         "can_add_element_to_key() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_add_element_to_key"]
+            [2, "pylero.base_polarion.BasePolarion.can_add_element_to_key", false]
         ],
         "can_delete_instance() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_delete_instance"]
+            [2, "pylero.base_polarion.BasePolarion.can_delete_instance", false]
         ],
         "can_modify_instance() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_modify_instance"]
+            [2, "pylero.base_polarion.BasePolarion.can_modify_instance", false]
         ],
         "can_modify_key() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_modify_key"]
+            [2, "pylero.base_polarion.BasePolarion.can_modify_key", false]
         ],
         "can_read_instance() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_read_instance"]
+            [2, "pylero.base_polarion.BasePolarion.can_read_instance", false]
         ],
         "can_read_key() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_read_key"]
+            [2, "pylero.base_polarion.BasePolarion.can_read_key", false]
         ],
         "can_remove_element_from_key() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.can_remove_element_from_key"]
+            [2, "pylero.base_polarion.BasePolarion.can_remove_element_from_key", false]
         ],
         "capacity (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.capacity"]
+            [2, "pylero.plan.Plan.capacity", false]
+        ],
+        "category (class in pylero.category)": [
+            [2, "pylero.category.Category", false]
         ],
         "category_id (pylero.category.category attribute)": [
-            [2, "pylero.category.Category.category_id"]
+            [2, "pylero.category.Category.category_id", false]
         ],
         "cft_id (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.cft_id"]
+            [2, "pylero.custom_field_type.CustomFieldType.cft_id", false]
+        ],
+        "change (class in pylero.change)": [
+            [2, "pylero.change.Change", false]
+        ],
+        "changerequest (class in pylero.work_item)": [
+            [2, "pylero.work_item.ChangeRequest", false]
         ],
         "check_valid_field_values() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.check_valid_field_values"]
+            [2, "pylero.base_polarion.BasePolarion.check_valid_field_values", false]
         ],
         "child_comment_uris (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.child_comment_uris"]
+            [2, "pylero.comment.Comment.child_comment_uris", false]
         ],
         "child_comment_uris (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.child_comment_uris"]
+            [2, "pylero.module_comment.ModuleComment.child_comment_uris", false]
+        ],
+        "classproperty (class in pylero.base_polarion)": [
+            [2, "pylero.base_polarion.ClassProperty", false]
         ],
         "cleaned_features (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.cleaned_features"]
+            [2, "pylero.workflow_action.WorkflowAction.cleaned_features", false]
         ],
         "closed (pylero.time_point.timepoint attribute)": [
-            [2, "pylero.time_point.TimePoint.closed"]
+            [2, "pylero.time_point.TimePoint.closed", false]
+        ],
+        "cmdlist (class in pylero.cli.cmd)": [
+            [3, "pylero.cli.cmd.CmdList", false]
+        ],
+        "cmdupdate (class in pylero.cli.cmd)": [
+            [3, "pylero.cli.cmd.CmdUpdate", false]
         ],
         "collection (pylero.field_diff.fielddiff attribute)": [
-            [2, "pylero.field_diff.FieldDiff.collection"]
+            [2, "pylero.field_diff.FieldDiff.collection", false]
         ],
         "color (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.color"]
+            [2, "pylero.plan.Plan.color", false]
+        ],
+        "comment (class in pylero.comment)": [
+            [2, "pylero.comment.Comment", false]
         ],
         "comment (pylero.test_step_result.teststepresult attribute)": [
-            [2, "pylero.test_step_result.TestStepResult.comment"]
+            [2, "pylero.test_step_result.TestStepResult.comment", false]
         ],
         "comment (pylero.work_record.workrecord attribute)": [
-            [2, "pylero.work_record.WorkRecord.comment"]
+            [2, "pylero.work_record.WorkRecord.comment", false]
         ],
         "comment_id (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.comment_id"]
+            [2, "pylero.comment.Comment.comment_id", false]
         ],
         "comments (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.comments"]
+            [2, "pylero.activity.Activity.comments", false]
         ],
         "comments (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.comments"]
+            [2, "pylero.document.Document.comments", false]
         ],
         "concurrent_license_data (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.concurrent_license_data"]
+            [2, "pylero.product_license.ProductLicense.concurrent_license_data", false]
+        ],
+        "config_section (pylero.base_polarion.configuration attribute)": [
+            [2, "pylero.base_polarion.Configuration.CONFIG_SECTION", false]
+        ],
+        "configuration (class in pylero.base_polarion)": [
+            [2, "pylero.base_polarion.Configuration", false]
         ],
         "connected (pylero.base_polarion.connection attribute)": [
-            [2, "pylero.base_polarion.Connection.connected"]
+            [2, "pylero.base_polarion.Connection.connected", false]
+        ],
+        "connection (class in pylero.base_polarion)": [
+            [2, "pylero.base_polarion.Connection", false]
         ],
         "constraint (pylero.planning_constraint.planningconstraint attribute)": [
-            [2, "pylero.planning_constraint.PlanningConstraint.constraint"]
+            [2, "pylero.planning_constraint.PlanningConstraint.constraint", false]
         ],
         "content (pylero.text.text attribute)": [
-            [2, "pylero.text.Text.content"]
+            [2, "pylero.text.Text.content", false]
         ],
         "content_lossy (pylero.text.text attribute)": [
-            [2, "pylero.text.Text.content_lossy"]
+            [2, "pylero.text.Text.content_lossy", false]
         ],
         "content_type (pylero.text.text attribute)": [
-            [2, "pylero.text.Text.content_type"]
+            [2, "pylero.text.Text.content_type", false]
         ],
         "context_id (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.context_id"]
+            [2, "pylero.activity.Activity.context_id", false]
         ],
         "create() (pylero.baseline.baseline class method)": [
-            [2, "pylero.baseline.Baseline.create"]
+            [2, "pylero.baseline.Baseline.create", false]
         ],
         "create() (pylero.document.document class method)": [
-            [2, "pylero.document.Document.create"]
+            [2, "pylero.document.Document.create", false]
         ],
         "create() (pylero.plan.plan class method)": [
-            [2, "pylero.plan.Plan.create"]
+            [2, "pylero.plan.Plan.create", false]
         ],
         "create() (pylero.test_run.testrun class method)": [
-            [2, "pylero.test_run.TestRun.create"]
-        ],
-        "create_incident_report() (in module pylero.test_run)": [
-            [2, "pylero.test_run.create_incident_report"]
+            [2, "pylero.test_run.TestRun.create", false]
         ],
         "create_plan_template() (pylero.plan.plan class method)": [
-            [2, "pylero.plan.Plan.create_plan_template"]
+            [2, "pylero.plan.Plan.create_plan_template", false]
         ],
         "create_ssl_context() (in module pylero.session)": [
-            [2, "pylero.session.create_ssl_context"]
+            [2, "pylero.session.create_ssl_context", false]
         ],
         "create_summary_defect() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.create_summary_defect"]
+            [2, "pylero.test_run.TestRun.create_summary_defect", false]
         ],
         "create_template() (pylero.test_run.testrun class method)": [
-            [2, "pylero.test_run.TestRun.create_template"]
+            [2, "pylero.test_run.TestRun.create_template", false]
         ],
         "create_user() (pylero.user.user class method)": [
-            [2, "pylero.user.User.create_user"]
+            [2, "pylero.user.User.create_user", false]
         ],
         "create_work_item() (pylero.document.document method)": [
-            [2, "pylero.document.Document.create_work_item"]
+            [2, "pylero.document.Document.create_work_item", false]
         ],
         "created (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.created"]
+            [2, "pylero.comment.Comment.created", false]
         ],
         "created (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.created"]
+            [2, "pylero.document.Document.created", false]
         ],
         "created (pylero.imported_comment.importedcomment attribute)": [
-            [2, "pylero.imported_comment.ImportedComment.created"]
+            [2, "pylero.imported_comment.ImportedComment.created", false]
         ],
         "created (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.created"]
+            [2, "pylero.module_comment.ModuleComment.created", false]
         ],
         "created (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.created"]
+            [2, "pylero.plan.Plan.created", false]
         ],
         "created (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.created"]
+            [2, "pylero.revision.Revision.created", false]
         ],
         "created (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.created"]
+            [2, "pylero.test_run.TestRun.created", false]
         ],
         "created (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.created"]
+            [2, "pylero.wiki_page.WikiPage.created", false]
         ],
         "creation (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.creation"]
+            [2, "pylero.change.Change.creation", false]
         ],
         "creation_time (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.creation_time"]
+            [2, "pylero.build.Build.creation_time", false]
+        ],
+        "curdir_config (pylero.base_polarion.configuration attribute)": [
+            [2, "pylero.base_polarion.Configuration.CURDIR_CONFIG", false]
+        ],
+        "custom (class in pylero.custom)": [
+            [2, "pylero.custom.Custom", false]
         ],
         "custom_array_obj() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.custom_array_obj"]
+            [2, "pylero.base_polarion.BasePolarion.custom_array_obj", false]
         ],
         "custom_fields (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.custom_fields"]
+            [2, "pylero.document.Document.custom_fields", false]
         ],
         "custom_fields (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.custom_fields"]
+            [2, "pylero.plan.Plan.custom_fields", false]
         ],
         "custom_fields (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.custom_fields"]
+            [2, "pylero.test_run.TestRun.custom_fields", false]
         ],
         "custom_obj() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.custom_obj"]
+            [2, "pylero.base_polarion.BasePolarion.custom_obj", false]
         ],
         "custom_values (pylero.activity_custom_value_entry.activitycustomvalueentry attribute)": [
-            [2, "pylero.activity_custom_value_entry.ActivityCustomValueEntry.custom_values"]
+            [2, "pylero.activity_custom_value_entry.ActivityCustomValueEntry.custom_values", false]
         ],
         "customer_company (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.customer_company"]
+            [2, "pylero.product_license.ProductLicense.customer_company", false]
         ],
         "customer_email (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.customer_email"]
+            [2, "pylero.product_license.ProductLicense.customer_email", false]
         ],
         "customer_name (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.customer_name"]
+            [2, "pylero.product_license.ProductLicense.customer_name", false]
+        ],
+        "customfield (class in pylero.custom_field)": [
+            [2, "pylero.custom_field.CustomField", false]
+        ],
+        "customfieldtype (class in pylero.custom_field_type)": [
+            [2, "pylero.custom_field_type.CustomFieldType", false]
         ],
         "date (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.date"]
+            [2, "pylero.change.Change.date", false]
         ],
         "date (pylero.planning_constraint.planningconstraint attribute)": [
-            [2, "pylero.planning_constraint.PlanningConstraint.date"]
+            [2, "pylero.planning_constraint.PlanningConstraint.date", false]
         ],
         "date (pylero.work_record.workrecord attribute)": [
-            [2, "pylero.work_record.WorkRecord.date"]
+            [2, "pylero.work_record.WorkRecord.date", false]
         ],
         "date_created (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.date_created"]
+            [2, "pylero.product_license.ProductLicense.date_created", false]
         ],
         "default (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.default"]
+            [2, "pylero.enum_option.EnumOption.default", false]
         ],
         "default (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.default"]
+            [2, "pylero.priority_opt.PriorityOpt.default", false]
         ],
         "default_estimate (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.default_estimate"]
+            [2, "pylero.plan.Plan.default_estimate", false]
         ],
         "default_project (pylero.base_polarion.basepolarion attribute)": [
-            [2, "id0"],
-            [2, "pylero.base_polarion.BasePolarion.default_project"]
+            [2, "id0", false],
+            [2, "pylero.base_polarion.BasePolarion.default_project", false]
         ],
         "default_value (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.default_value"]
+            [2, "pylero.custom_field_type.CustomFieldType.default_value", false]
         ],
         "default_value (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.default_value"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.default_value", false]
+        ],
+        "defect (class in pylero.work_item)": [
+            [2, "pylero.work_item.Defect", false]
         ],
         "defect_auto_assignement_enabled (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.defect_auto_assignement_enabled"]
+            [2, "pylero.tests_configuration.TestsConfiguration.defect_auto_assignement_enabled", false]
         ],
         "defect_reuse_type (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.defect_reuse_type"]
+            [2, "pylero.tests_configuration.TestsConfiguration.defect_reuse_type", false]
         ],
         "defect_template (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.defect_template"]
+            [2, "pylero.tests_configuration.TestsConfiguration.defect_template", false]
         ],
         "defect_to_test_case_link_role_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.defect_to_test_case_link_role_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.defect_to_test_case_link_role_id", false]
         ],
         "defect_work_item_type (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.defect_work_item_type"]
+            [2, "pylero.tests_configuration.TestsConfiguration.defect_work_item_type", false]
         ],
         "defects_project (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.defects_project"]
+            [2, "pylero.tests_configuration.TestsConfiguration.defects_project", false]
         ],
         "delete() (pylero.document.document method)": [
-            [2, "pylero.document.Document.delete"]
+            [2, "pylero.document.Document.delete", false]
         ],
         "delete_attachment() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.delete_attachment"]
+            [2, "pylero.test_run.TestRun.delete_attachment", false]
         ],
         "delete_attachment_from_test_record() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.delete_attachment_from_test_record"]
+            [2, "pylero.test_run.TestRun.delete_attachment_from_test_record", false]
         ],
         "delete_attachment_from_test_step() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.delete_attachment_from_test_step"]
+            [2, "pylero.test_run.TestRun.delete_attachment_from_test_step", false]
         ],
         "delete_plans() (pylero.plan.plan class method)": [
-            [2, "pylero.plan.Plan.delete_plans"]
+            [2, "pylero.plan.Plan.delete_plans", false]
         ],
         "depends_on (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.depends_on"]
+            [2, "pylero.custom_field_type.CustomFieldType.depends_on", false]
         ],
         "depends_on (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.depends_on"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.depends_on", false]
         ],
         "derived_fields (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.derived_fields"]
+            [2, "pylero.document.Document.derived_fields", false]
         ],
         "derived_from_link_role (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.derived_from_link_role"]
+            [2, "pylero.document.Document.derived_from_link_role", false]
         ],
         "derived_from_uri (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.derived_from_uri"]
+            [2, "pylero.document.Document.derived_from_uri", false]
         ],
         "description (pylero.baseline.baseline attribute)": [
-            [2, "pylero.baseline.Baseline.description"]
+            [2, "pylero.baseline.Baseline.description", false]
         ],
         "description (pylero.category.category attribute)": [
-            [2, "pylero.category.Category.description"]
+            [2, "pylero.category.Category.description", false]
         ],
         "description (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.description"]
+            [2, "pylero.custom_field_type.CustomFieldType.description", false]
         ],
         "description (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.description"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.description", false]
         ],
         "description (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.description"]
+            [2, "pylero.plan.Plan.description", false]
         ],
         "description (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.description"]
+            [2, "pylero.project.Project.description", false]
         ],
         "description (pylero.time_point.timepoint attribute)": [
-            [2, "pylero.time_point.TimePoint.description"]
+            [2, "pylero.time_point.TimePoint.description", false]
         ],
         "description (pylero.user.user attribute)": [
-            [2, "pylero.user.User.description"]
+            [2, "pylero.user.User.description", false]
         ],
         "diffs (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.diffs"]
+            [2, "pylero.change.Change.diffs", false]
         ],
         "disabled_notifications (pylero.user.user attribute)": [
-            [2, "pylero.user.User.disabled_notifications"]
+            [2, "pylero.user.User.disabled_notifications", false]
+        ],
+        "document (class in pylero.document)": [
+            [2, "pylero.document.Document", false]
         ],
         "document (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.document"]
+            [2, "pylero.test_run.TestRun.document", false]
         ],
         "done (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.done"]
+            [2, "pylero.plan_statistics.PlanStatistics.done", false]
         ],
         "done_as_string (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.done_as_string"]
+            [2, "pylero.plan_statistics.PlanStatistics.done_as_string", false]
         ],
         "due_date (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.due_date"]
+            [2, "pylero.plan.Plan.due_date", false]
         ],
         "earliest_planned_start (pylero.time_point.timepoint attribute)": [
-            [2, "pylero.time_point.TimePoint.earliest_planned_start"]
+            [2, "pylero.time_point.TimePoint.earliest_planned_start", false]
         ],
         "email (pylero.user.user attribute)": [
-            [2, "pylero.user.User.email"]
+            [2, "pylero.user.User.email", false]
         ],
         "empty (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.empty"]
+            [2, "pylero.change.Change.empty", false]
         ],
         "enum_id (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.enum_id"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.enum_id", false]
         ],
         "enum_id (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.enum_id"]
+            [2, "pylero.enum_option.EnumOption.enum_id", false]
         ],
         "enum_id (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.enum_id"]
+            [2, "pylero.priority_opt.PriorityOpt.enum_id", false]
         ],
         "enum_option_id (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.enum_option_id"]
+            [2, "pylero.enum_option.EnumOption.enum_option_id", false]
+        ],
+        "enumcustomfieldtype (class in pylero.enum_custom_field_type)": [
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType", false]
+        ],
+        "enumoption (class in pylero.enum_option)": [
+            [2, "pylero.enum_option.EnumOption", false]
+        ],
+        "enumoptionid (class in pylero.enum_option_id)": [
+            [2, "pylero.enum_option_id.EnumOptionId", false]
         ],
         "error_count (pylero.build_test_results.buildtestresults attribute)": [
-            [2, "pylero.build_test_results.BuildTestResults.error_count"]
+            [2, "pylero.build_test_results.BuildTestResults.error_count", false]
         ],
         "estimation_field (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.estimation_field"]
+            [2, "pylero.plan.Plan.estimation_field", false]
         ],
         "expiration_date (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.expiration_date"]
+            [2, "pylero.product_license.ProductLicense.expiration_date", false]
         ],
         "export_pdf() (pylero.document.document class method)": [
-            [2, "pylero.document.Document.export_pdf"]
+            [2, "pylero.document.Document.export_pdf", false]
+        ],
+        "externallylinkedworkitem (class in pylero.externally_linked_work_item)": [
+            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem", false]
         ],
         "failure_count (pylero.build_test_results.buildtestresults attribute)": [
-            [2, "pylero.build_test_results.BuildTestResults.failure_count"]
+            [2, "pylero.build_test_results.BuildTestResults.failure_count", false]
         ],
         "field_name (pylero.field_diff.fielddiff attribute)": [
-            [2, "pylero.field_diff.FieldDiff.field_name"]
+            [2, "pylero.field_diff.FieldDiff.field_name", false]
+        ],
+        "fielddiff (class in pylero.field_diff)": [
+            [2, "pylero.field_diff.FieldDiff", false]
         ],
         "fields_to_copy_from_test_case_to_defect (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.fields_to_copy_from_test_case_to_defect"]
+            [2, "pylero.tests_configuration.TestsConfiguration.fields_to_copy_from_test_case_to_defect", false]
         ],
         "fields_to_copy_from_test_run_to_linked_defect (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.fields_to_copy_from_test_run_to_linked_defect"]
+            [2, "pylero.tests_configuration.TestsConfiguration.fields_to_copy_from_test_run_to_linked_defect", false]
         ],
         "fields_to_copy_from_test_run_to_new_defect (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.fields_to_copy_from_test_run_to_new_defect"]
+            [2, "pylero.tests_configuration.TestsConfiguration.fields_to_copy_from_test_run_to_new_defect", false]
         ],
         "file_name (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.file_name"]
+            [2, "pylero.attachment.Attachment.file_name", false]
         ],
         "file_name (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.file_name"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.file_name", false]
         ],
         "file_name (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.file_name"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.file_name", false]
         ],
         "filter() (pylero.session.listenfilter method)": [
-            [2, "pylero.session.ListenFilter.filter"]
+            [2, "pylero.session.ListenFilter.filter", false]
         ],
         "finish (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.finish"]
+            [2, "pylero.project.Project.finish", false]
         ],
         "finish_time (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.finish_time"]
+            [2, "pylero.build.Build.finish_time", false]
         ],
         "finished_on (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.finished_on"]
+            [2, "pylero.plan.Plan.finished_on", false]
         ],
         "finished_on (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.finished_on"]
+            [2, "pylero.test_run.TestRun.finished_on", false]
         ],
         "float (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.float"]
-        ],
-        "generate_description() (in module pylero.test_run)": [
-            [2, "pylero.test_run.generate_description"]
+            [2, "pylero.priority_opt.PriorityOpt.float", false]
         ],
         "generated_by (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.generated_by"]
+            [2, "pylero.product_license.ProductLicense.generated_by", false]
         ],
         "get_attachment() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.get_attachment"]
+            [2, "pylero.test_run.TestRun.get_attachment", false]
         ],
         "get_attachments() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.get_attachments"]
+            [2, "pylero.test_run.TestRun.get_attachments", false]
         ],
         "get_categories() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_categories"]
+            [2, "pylero.project.Project.get_categories", false]
         ],
         "get_contained_groups() (pylero.project_group.projectgroup method)": [
-            [2, "pylero.project_group.ProjectGroup.get_contained_groups"]
+            [2, "pylero.project_group.ProjectGroup.get_contained_groups", false]
         ],
         "get_contained_projects() (pylero.project_group.projectgroup method)": [
-            [2, "pylero.project_group.ProjectGroup.get_contained_projects"]
+            [2, "pylero.project_group.ProjectGroup.get_contained_projects", false]
         ],
         "get_context_roles() (pylero.project.project class method)": [
-            [2, "pylero.project.Project.get_context_roles"]
+            [2, "pylero.project.Project.get_context_roles", false]
         ],
         "get_context_roles() (pylero.user.user method)": [
-            [2, "pylero.user.User.get_context_roles"]
+            [2, "pylero.user.User.get_context_roles", false]
         ],
         "get_custom_field() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.get_custom_field"]
+            [2, "pylero.test_run.TestRun.get_custom_field", false]
         ],
         "get_deep_contained_projects() (pylero.project_group.projectgroup method)": [
-            [2, "pylero.project_group.ProjectGroup.get_deep_contained_projects"]
+            [2, "pylero.project_group.ProjectGroup.get_deep_contained_projects", false]
         ],
         "get_defined_custom_field_keys() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_defined_custom_field_keys"]
+            [2, "pylero.project.Project.get_defined_custom_field_keys", false]
         ],
         "get_defined_custom_field_type() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_defined_custom_field_type"]
+            [2, "pylero.project.Project.get_defined_custom_field_type", false]
         ],
         "get_defined_custom_field_types() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_defined_custom_field_types"]
+            [2, "pylero.project.Project.get_defined_custom_field_types", false]
         ],
         "get_defined_custom_field_types() (pylero.test_run.testrun class method)": [
-            [2, "pylero.test_run.TestRun.get_defined_custom_field_types"]
+            [2, "pylero.test_run.TestRun.get_defined_custom_field_types", false]
         ],
         "get_document_spaces() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_document_spaces"]
+            [2, "pylero.project.Project.get_document_spaces", false]
         ],
         "get_documents() (pylero.document.document class method)": [
-            [2, "pylero.document.Document.get_documents"]
+            [2, "pylero.document.Document.get_documents", false]
         ],
         "get_global_roles() (pylero.base_polarion.basepolarion class method)": [
-            [2, "pylero.base_polarion.BasePolarion.get_global_roles"]
+            [2, "pylero.base_polarion.BasePolarion.get_global_roles", false]
         ],
         "get_location() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.get_location"]
+            [2, "pylero.base_polarion.BasePolarion.get_location", false]
         ],
         "get_project_users() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_project_users"]
+            [2, "pylero.project.Project.get_project_users", false]
+        ],
+        "get_revision() (pylero.base_polarion.basepolarion method)": [
+            [2, "pylero.base_polarion.BasePolarion.get_revision", false]
+        ],
+        "get_revision_by_uri() (pylero.base_polarion.basepolarion method)": [
+            [2, "pylero.base_polarion.BasePolarion.get_revision_by_uri", false]
+        ],
+        "get_revisions() (pylero.base_polarion.basepolarion method)": [
+            [2, "pylero.base_polarion.BasePolarion.get_revisions", false]
         ],
         "get_roles() (pylero.user.user method)": [
-            [2, "pylero.user.User.get_roles"]
+            [2, "pylero.user.User.get_roles", false]
         ],
         "get_root_project_group() (pylero.project_group.projectgroup class method)": [
-            [2, "pylero.project_group.ProjectGroup.get_root_project_group"]
+            [2, "pylero.project_group.ProjectGroup.get_root_project_group", false]
         ],
         "get_statistics() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.get_statistics"]
+            [2, "pylero.plan.Plan.get_statistics", false]
         ],
         "get_test_steps_configuration() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_test_steps_configuration"]
+            [2, "pylero.project.Project.get_test_steps_configuration", false]
         ],
         "get_tests_configuration() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_tests_configuration"]
+            [2, "pylero.project.Project.get_tests_configuration", false]
         ],
         "get_user_avatar_url() (pylero.user.user method)": [
-            [2, "pylero.user.User.get_user_avatar_url"]
+            [2, "pylero.user.User.get_user_avatar_url", false]
         ],
         "get_user_from_token() (pylero.user.user class method)": [
-            [2, "pylero.user.User.get_user_from_token"]
+            [2, "pylero.user.User.get_user_from_token", false]
         ],
         "get_users() (pylero.user.user class method)": [
-            [2, "pylero.user.User.get_users"]
+            [2, "pylero.user.User.get_users", false]
         ],
         "get_valid_field_values() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.get_valid_field_values"]
+            [2, "pylero.base_polarion.BasePolarion.get_valid_field_values", false]
         ],
         "get_wiki_content() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.get_wiki_content"]
+            [2, "pylero.plan.Plan.get_wiki_content", false]
         ],
         "get_wiki_content() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.get_wiki_content"]
+            [2, "pylero.test_run.TestRun.get_wiki_content", false]
         ],
         "get_wiki_pages() (pylero.wiki_page.wikipage class method)": [
-            [2, "pylero.wiki_page.WikiPage.get_wiki_pages"]
+            [2, "pylero.wiki_page.WikiPage.get_wiki_pages", false]
         ],
         "get_wiki_spaces() (pylero.project.project method)": [
-            [2, "pylero.project.Project.get_wiki_spaces"]
+            [2, "pylero.project.Project.get_wiki_spaces", false]
         ],
         "get_work_items() (pylero.document.document method)": [
-            [2, "pylero.document.Document.get_work_items"]
+            [2, "pylero.document.Document.get_work_items", false]
+        ],
+        "global_config (pylero.base_polarion.configuration attribute)": [
+            [2, "pylero.base_polarion.Configuration.GLOBAL_CONFIG", false]
         ],
         "global_id (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.global_id"]
+            [2, "pylero.activity.Activity.global_id", false]
         ],
         "group_id (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.group_id"]
+            [2, "pylero.test_run.TestRun.group_id", false]
         ],
         "group_uris (pylero.project_group.projectgroup attribute)": [
-            [2, "pylero.project_group.ProjectGroup.group_uris"]
+            [2, "pylero.project_group.ProjectGroup.group_uris", false]
         ],
         "has_current_user_permission() (pylero.base_polarion.basepolarion class method)": [
-            [2, "pylero.base_polarion.BasePolarion.has_current_user_permission"]
+            [2, "pylero.base_polarion.BasePolarion.has_current_user_permission", false]
         ],
         "has_permission() (pylero.user.user method)": [
-            [2, "pylero.user.User.has_permission"]
+            [2, "pylero.user.User.has_permission", false]
         ],
         "hidden (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.hidden"]
+            [2, "pylero.enum_option.EnumOption.hidden", false]
         ],
         "hidden (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.hidden"]
+            [2, "pylero.priority_opt.PriorityOpt.hidden", false]
         ],
         "home_page_content (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.home_page_content"]
+            [2, "pylero.document.Document.home_page_content", false]
         ],
         "home_page_content (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.home_page_content"]
+            [2, "pylero.wiki_page.WikiPage.home_page_content", false]
+        ],
+        "hyperlink (class in pylero.hyperlink)": [
+            [2, "pylero.hyperlink.Hyperlink", false]
         ],
         "id (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.id"]
+            [2, "pylero.document.Document.id", false]
         ],
         "id (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.id"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.id", false]
         ],
         "id (pylero.priority_option_id.priorityoptionid attribute)": [
-            [2, "pylero.priority_option_id.PriorityOptionId.id"]
+            [2, "pylero.priority_option_id.PriorityOptionId.id", false]
         ],
         "id (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.id"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.id", false]
         ],
         "ideal_progress (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.ideal_progress"]
+            [2, "pylero.plan_statistics.PlanStatistics.ideal_progress", false]
         ],
         "ideal_progress_as_string (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.ideal_progress_as_string"]
+            [2, "pylero.plan_statistics.PlanStatistics.ideal_progress_as_string", false]
         ],
         "imported_comment (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.imported_comment"]
+            [2, "pylero.module_comment.ModuleComment.imported_comment", false]
+        ],
+        "importedcomment (class in pylero.imported_comment)": [
+            [2, "pylero.imported_comment.ImportedComment", false]
+        ],
+        "incidentreport (class in pylero.work_item)": [
+            [2, "pylero.work_item.IncidentReport", false]
         ],
         "info (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.info"]
+            [2, "pylero.activity.Activity.info", false]
         ],
         "initials (pylero.imported_comment.importedcomment attribute)": [
-            [2, "pylero.imported_comment.ImportedComment.initials"]
+            [2, "pylero.imported_comment.ImportedComment.initials", false]
         ],
         "internal_commit (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.internal_commit"]
+            [2, "pylero.revision.Revision.internal_commit", false]
         ],
         "invalid (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.invalid"]
+            [2, "pylero.change.Change.invalid", false]
         ],
         "ip_address (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.ip_address"]
+            [2, "pylero.product_license.ProductLicense.ip_address", false]
         ],
         "is_template (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.is_template"]
+            [2, "pylero.plan.Plan.is_template", false]
         ],
         "is_template (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.is_template"]
+            [2, "pylero.test_run.TestRun.is_template", false]
         ],
         "item (pylero.plan_record.planrecord attribute)": [
-            [2, "pylero.plan_record.PlanRecord.item"]
+            [2, "pylero.plan_record.PlanRecord.item", false]
         ],
         "job_id (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.job_id"]
+            [2, "pylero.build.Build.job_id", false]
         ],
         "keep_in_history (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.keep_in_history"]
+            [2, "pylero.test_run.TestRun.keep_in_history", false]
         ],
         "key (pylero.activity_custom_value_entry.activitycustomvalueentry attribute)": [
-            [2, "pylero.activity_custom_value_entry.ActivityCustomValueEntry.key"]
+            [2, "pylero.activity_custom_value_entry.ActivityCustomValueEntry.key", false]
         ],
         "key (pylero.custom.custom attribute)": [
-            [2, "pylero.custom.Custom.key"]
+            [2, "pylero.custom.Custom.key", false]
         ],
         "key (pylero.custom_field.customfield attribute)": [
-            [2, "pylero.custom_field.CustomField.key"]
+            [2, "pylero.custom_field.CustomField.key", false]
         ],
         "key (pylero.property.property attribute)": [
-            [2, "pylero.property.Property.key"]
+            [2, "pylero.property.Property.key", false]
         ],
         "keys (pylero.test_steps.teststeps attribute)": [
-            [2, "pylero.test_steps.TestSteps.keys"]
+            [2, "pylero.test_steps.TestSteps.keys", false]
         ],
         "label (pylero.language_definition.languagedefinition attribute)": [
-            [2, "pylero.language_definition.LanguageDefinition.label"]
+            [2, "pylero.language_definition.LanguageDefinition.label", false]
         ],
         "language_definition_id (pylero.language_definition.languagedefinition attribute)": [
-            [2, "pylero.language_definition.LanguageDefinition.language_definition_id"]
+            [2, "pylero.language_definition.LanguageDefinition.language_definition_id", false]
+        ],
+        "languagedefinition (class in pylero.language_definition)": [
+            [2, "pylero.language_definition.LanguageDefinition", false]
         ],
         "lead (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.lead"]
+            [2, "pylero.project.Project.lead", false]
         ],
         "length (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.length"]
+            [2, "pylero.attachment.Attachment.length", false]
         ],
         "length (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.length"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.length", false]
         ],
         "length (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.length"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.length", false]
         ],
         "license (pylero.license_info.licenseinfo attribute)": [
-            [2, "pylero.license_info.LicenseInfo.license"]
+            [2, "pylero.license_info.LicenseInfo.license", false]
         ],
         "license_format (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.license_format"]
+            [2, "pylero.product_license.ProductLicense.license_format", false]
         ],
         "license_profile (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.license_profile"]
+            [2, "pylero.product_license.ProductLicense.license_profile", false]
+        ],
+        "licenseinfo (class in pylero.license_info)": [
+            [2, "pylero.license_info.LicenseInfo", false]
         ],
         "linked_page_uris (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.linked_page_uris"]
+            [2, "pylero.wiki_page.WikiPage.linked_page_uris", false]
         ],
         "linked_work_item_uris (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.linked_work_item_uris"]
+            [2, "pylero.revision.Revision.linked_work_item_uris", false]
         ],
         "linked_work_items (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.linked_work_items"]
+            [2, "pylero.build.Build.linked_work_items", false]
+        ],
+        "linkedworkitem (class in pylero.linked_work_item)": [
+            [2, "pylero.linked_work_item.LinkedWorkItem", false]
+        ],
+        "list_documents_by_query() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.list_documents_by_query", false]
+        ],
+        "list_workitems_by_query() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.list_workitems_by_query", false]
+        ],
+        "list_workitems_in_doc() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.list_workitems_in_doc", false]
+        ],
+        "listenfilter (class in pylero.session)": [
+            [2, "pylero.session.ListenFilter", false]
+        ],
+        "local_config (pylero.base_polarion.configuration attribute)": [
+            [2, "pylero.base_polarion.Configuration.LOCAL_CONFIG", false]
         ],
         "local_deployment_space_name (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.local_deployment_space_name"]
+            [2, "pylero.build.Build.local_deployment_space_name", false]
         ],
         "location (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.location"]
+            [2, "pylero.document.Document.location", false]
         ],
         "location (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.location"]
+            [2, "pylero.plan.Plan.location", false]
         ],
         "location (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.location"]
+            [2, "pylero.project.Project.location", false]
         ],
         "location (pylero.project_group.projectgroup attribute)": [
-            [2, "pylero.project_group.ProjectGroup.location"]
+            [2, "pylero.project_group.ProjectGroup.location", false]
         ],
         "location (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.location"]
+            [2, "pylero.test_run.TestRun.location", false]
         ],
         "location (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.location"]
+            [2, "pylero.wiki_page.WikiPage.location", false]
         ],
         "lock_work_records_date (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.lock_work_records_date"]
+            [2, "pylero.project.Project.lock_work_records_date", false]
         ],
         "log_files (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.log_files"]
+            [2, "pylero.build.Build.log_files", false]
         ],
         "logged_in_user_id (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion.logged_in_user_id"]
+            [2, "pylero.base_polarion.BasePolarion.logged_in_user_id", false]
         ],
         "mac_address (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.mac_address"]
+            [2, "pylero.product_license.ProductLicense.mac_address", false]
         ],
         "marshalled() (pylero.session.soapnull method)": [
-            [2, "pylero.session.SoapNull.marshalled"]
+            [2, "pylero.session.SoapNull.marshalled", false]
         ],
         "max_created_defects (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.max_created_defects"]
+            [2, "pylero.tests_configuration.TestsConfiguration.max_created_defects", false]
         ],
         "max_created_defects_percent (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.max_created_defects_percent"]
+            [2, "pylero.tests_configuration.TestsConfiguration.max_created_defects_percent", false]
         ],
         "message (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.message"]
+            [2, "pylero.revision.Revision.message", false]
         ],
         "module": [
-            [2, "module-pylero"],
-            [2, "module-pylero.activity"],
-            [2, "module-pylero.activity_comment"],
-            [2, "module-pylero.activity_custom_value"],
-            [2, "module-pylero.activity_custom_value_entry"],
-            [2, "module-pylero.activity_source"],
-            [2, "module-pylero.approval"],
-            [2, "module-pylero.attachment"],
-            [2, "module-pylero.base_polarion"],
-            [2, "module-pylero.baseline"],
-            [2, "module-pylero.build"],
-            [2, "module-pylero.build_linked_work_item"],
-            [2, "module-pylero.build_test_results"],
-            [2, "module-pylero.category"],
-            [2, "module-pylero.change"],
-            [2, "module-pylero.comment"],
-            [2, "module-pylero.custom"],
-            [2, "module-pylero.custom_field"],
-            [2, "module-pylero.custom_field_type"],
-            [2, "module-pylero.document"],
-            [2, "module-pylero.enum_custom_field_type"],
-            [2, "module-pylero.enum_option"],
-            [2, "module-pylero.enum_option_id"],
-            [2, "module-pylero.exceptions"],
-            [2, "module-pylero.externally_linked_work_item"],
-            [2, "module-pylero.field_diff"],
-            [2, "module-pylero.hyperlink"],
-            [2, "module-pylero.imported_comment"],
-            [2, "module-pylero.language_definition"],
-            [2, "module-pylero.license_info"],
-            [2, "module-pylero.linked_work_item"],
-            [2, "module-pylero.module_comment"],
-            [2, "module-pylero.plan"],
-            [2, "module-pylero.plan_record"],
-            [2, "module-pylero.plan_statistics"],
-            [2, "module-pylero.planning_constraint"],
-            [2, "module-pylero.priority_opt"],
-            [2, "module-pylero.priority_option_id"],
-            [2, "module-pylero.product_license"],
-            [2, "module-pylero.project"],
-            [2, "module-pylero.project_group"],
-            [2, "module-pylero.properties"],
-            [2, "module-pylero.property"],
-            [2, "module-pylero.revision"],
-            [2, "module-pylero.server"],
-            [2, "module-pylero.session"],
-            [2, "module-pylero.signature"],
-            [2, "module-pylero.signature_context"],
-            [2, "module-pylero.signature_data"],
-            [2, "module-pylero.subterra_uri"],
-            [2, "module-pylero.test_record"],
-            [2, "module-pylero.test_run"],
-            [2, "module-pylero.test_run_attachment"],
-            [2, "module-pylero.test_step"],
-            [2, "module-pylero.test_step_result"],
-            [2, "module-pylero.test_steps"],
-            [2, "module-pylero.tests_configuration"],
-            [2, "module-pylero.text"],
-            [2, "module-pylero.time_point"],
-            [2, "module-pylero.user"],
-            [2, "module-pylero.wiki_page"],
-            [2, "module-pylero.wiki_page_attachment"],
-            [2, "module-pylero.work_item"],
-            [2, "module-pylero.work_record"],
-            [2, "module-pylero.workflow_action"],
-            [3, "module-pylero.cli"],
-            [3, "module-pylero.cli.cmd"]
+            [2, "module-pylero", false],
+            [2, "module-pylero.activity", false],
+            [2, "module-pylero.activity_comment", false],
+            [2, "module-pylero.activity_custom_value", false],
+            [2, "module-pylero.activity_custom_value_entry", false],
+            [2, "module-pylero.activity_source", false],
+            [2, "module-pylero.approval", false],
+            [2, "module-pylero.attachment", false],
+            [2, "module-pylero.base_polarion", false],
+            [2, "module-pylero.baseline", false],
+            [2, "module-pylero.build", false],
+            [2, "module-pylero.build_linked_work_item", false],
+            [2, "module-pylero.build_test_results", false],
+            [2, "module-pylero.category", false],
+            [2, "module-pylero.change", false],
+            [2, "module-pylero.comment", false],
+            [2, "module-pylero.custom", false],
+            [2, "module-pylero.custom_field", false],
+            [2, "module-pylero.custom_field_type", false],
+            [2, "module-pylero.document", false],
+            [2, "module-pylero.enum_custom_field_type", false],
+            [2, "module-pylero.enum_option", false],
+            [2, "module-pylero.enum_option_id", false],
+            [2, "module-pylero.exceptions", false],
+            [2, "module-pylero.externally_linked_work_item", false],
+            [2, "module-pylero.field_diff", false],
+            [2, "module-pylero.hyperlink", false],
+            [2, "module-pylero.imported_comment", false],
+            [2, "module-pylero.language_definition", false],
+            [2, "module-pylero.license_info", false],
+            [2, "module-pylero.linked_work_item", false],
+            [2, "module-pylero.module_comment", false],
+            [2, "module-pylero.plan", false],
+            [2, "module-pylero.plan_record", false],
+            [2, "module-pylero.plan_statistics", false],
+            [2, "module-pylero.planning_constraint", false],
+            [2, "module-pylero.priority_opt", false],
+            [2, "module-pylero.priority_option_id", false],
+            [2, "module-pylero.product_license", false],
+            [2, "module-pylero.project", false],
+            [2, "module-pylero.project_group", false],
+            [2, "module-pylero.properties", false],
+            [2, "module-pylero.property", false],
+            [2, "module-pylero.revision", false],
+            [2, "module-pylero.server", false],
+            [2, "module-pylero.session", false],
+            [2, "module-pylero.signature", false],
+            [2, "module-pylero.signature_context", false],
+            [2, "module-pylero.signature_data", false],
+            [2, "module-pylero.subterra_uri", false],
+            [2, "module-pylero.test_record", false],
+            [2, "module-pylero.test_run", false],
+            [2, "module-pylero.test_run_attachment", false],
+            [2, "module-pylero.test_step", false],
+            [2, "module-pylero.test_step_result", false],
+            [2, "module-pylero.test_steps", false],
+            [2, "module-pylero.tests_configuration", false],
+            [2, "module-pylero.text", false],
+            [2, "module-pylero.time_point", false],
+            [2, "module-pylero.user", false],
+            [2, "module-pylero.wiki_page", false],
+            [2, "module-pylero.wiki_page_attachment", false],
+            [2, "module-pylero.work_item", false],
+            [2, "module-pylero.work_record", false],
+            [2, "module-pylero.workflow_action", false],
+            [3, "module-pylero.cli", false],
+            [3, "module-pylero.cli.cmd", false]
         ],
         "module_absolute_location (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.module_absolute_location"]
+            [2, "pylero.document.Document.module_absolute_location", false]
         ],
         "module_comment_id (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.module_comment_id"]
+            [2, "pylero.module_comment.ModuleComment.module_comment_id", false]
         ],
         "module_folder (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.module_folder"]
+            [2, "pylero.document.Document.module_folder", false]
         ],
         "module_location (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.module_location"]
+            [2, "pylero.document.Document.module_location", false]
         ],
         "module_name (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.module_name"]
+            [2, "pylero.document.Document.module_name", false]
+        ],
+        "modulecomment (class in pylero.module_comment)": [
+            [2, "pylero.module_comment.ModuleComment", false]
         ],
         "move_work_item_here() (pylero.document.document method)": [
-            [2, "pylero.document.Document.move_work_item_here"]
+            [2, "pylero.document.Document.move_work_item_here", false]
         ],
         "name (pylero.baseline.baseline attribute)": [
-            [2, "pylero.baseline.Baseline.name"]
+            [2, "pylero.baseline.Baseline.name", false]
         ],
         "name (pylero.category.category attribute)": [
-            [2, "pylero.category.Category.name"]
+            [2, "pylero.category.Category.name", false]
         ],
         "name (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.name"]
+            [2, "pylero.custom_field_type.CustomFieldType.name", false]
         ],
         "name (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.name"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.name", false]
         ],
         "name (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.name"]
+            [2, "pylero.enum_option.EnumOption.name", false]
         ],
         "name (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.name"]
+            [2, "pylero.plan.Plan.name", false]
         ],
         "name (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.name"]
+            [2, "pylero.priority_opt.PriorityOpt.name", false]
         ],
         "name (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.name"]
+            [2, "pylero.project.Project.name", false]
         ],
         "name (pylero.project_group.projectgroup attribute)": [
-            [2, "pylero.project_group.ProjectGroup.name"]
+            [2, "pylero.project_group.ProjectGroup.name", false]
         ],
         "name (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.name"]
+            [2, "pylero.revision.Revision.name", false]
         ],
         "name (pylero.time_point.timepoint attribute)": [
-            [2, "pylero.time_point.TimePoint.name"]
+            [2, "pylero.time_point.TimePoint.name", false]
         ],
         "name (pylero.user.user attribute)": [
-            [2, "pylero.user.User.name"]
+            [2, "pylero.user.User.name", false]
         ],
         "named_license_data (pylero.product_license.productlicense attribute)": [
-            [2, "pylero.product_license.ProductLicense.named_license_data"]
+            [2, "pylero.product_license.ProductLicense.named_license_data", false]
         ],
         "native_action_id (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.native_action_id"]
+            [2, "pylero.workflow_action.WorkflowAction.native_action_id", false]
         ],
         "newclass (in module pylero.work_item)": [
-            [2, "pylero.work_item.newclass"]
+            [2, "pylero.work_item.newclass", false]
         ],
         "number_of_planned (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.number_of_planned"]
+            [2, "pylero.plan_statistics.PlanStatistics.number_of_planned", false]
         ],
         "number_of_resolved (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.number_of_resolved"]
+            [2, "pylero.plan_statistics.PlanStatistics.number_of_resolved", false]
         ],
         "number_of_unresolved (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.number_of_unresolved"]
+            [2, "pylero.plan_statistics.PlanStatistics.number_of_unresolved", false]
         ],
         "page_location (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.page_location"]
+            [2, "pylero.wiki_page.WikiPage.page_location", false]
         ],
         "page_name (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.page_name"]
+            [2, "pylero.wiki_page.WikiPage.page_name", false]
         ],
         "parent (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.parent"]
+            [2, "pylero.plan.Plan.parent", false]
         ],
         "parent_comment_uri (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.parent_comment_uri"]
+            [2, "pylero.comment.Comment.parent_comment_uri", false]
         ],
         "parent_comment_uri (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.parent_comment_uri"]
+            [2, "pylero.module_comment.ModuleComment.parent_comment_uri", false]
         ],
         "parent_item_uri (pylero.custom_field.customfield attribute)": [
-            [2, "pylero.custom_field.CustomField.parent_item_uri"]
+            [2, "pylero.custom_field.CustomField.parent_item_uri", false]
         ],
         "parent_uri (pylero.project_group.projectgroup attribute)": [
-            [2, "pylero.project_group.ProjectGroup.parent_uri"]
+            [2, "pylero.project_group.ProjectGroup.parent_uri", false]
         ],
         "phantom (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.phantom"]
+            [2, "pylero.enum_option.EnumOption.phantom", false]
         ],
         "phantom (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.phantom"]
+            [2, "pylero.priority_opt.PriorityOpt.phantom", false]
         ],
         "pkgdir (pylero.base_polarion.configuration attribute)": [
-            [2, "pylero.base_polarion.Configuration.pkgdir"]
+            [2, "pylero.base_polarion.Configuration.pkgdir", false]
+        ],
+        "plan (class in pylero.plan)": [
+            [2, "pylero.plan.Plan", false]
         ],
         "plan_id (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.plan_id"]
+            [2, "pylero.plan.Plan.plan_id", false]
         ],
         "planned (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.planned"]
+            [2, "pylero.plan_statistics.PlanStatistics.planned", false]
         ],
         "planned_as_string (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.planned_as_string"]
+            [2, "pylero.plan_statistics.PlanStatistics.planned_as_string", false]
+        ],
+        "planningconstraint (class in pylero.planning_constraint)": [
+            [2, "pylero.planning_constraint.PlanningConstraint", false]
+        ],
+        "planrecord (class in pylero.plan_record)": [
+            [2, "pylero.plan_record.PlanRecord", false]
+        ],
+        "planstatistics (class in pylero.plan_statistics)": [
+            [2, "pylero.plan_statistics.PlanStatistics", false]
         ],
         "prefix (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.prefix"]
+            [2, "pylero.activity.Activity.prefix", false]
         ],
         "prefix (pylero.activity_source.activitysource attribute)": [
-            [2, "pylero.activity_source.ActivitySource.prefix"]
+            [2, "pylero.activity_source.ActivitySource.prefix", false]
         ],
         "previous_time_spent (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.previous_time_spent"]
+            [2, "pylero.plan.Plan.previous_time_spent", false]
+        ],
+        "print_documents() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_documents", false]
+        ],
+        "print_links_for_requirement() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_links_for_requirement", false]
+        ],
+        "print_links_for_testcase() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_links_for_testcase", false]
+        ],
+        "print_plan_ids() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_plan_ids", false]
+        ],
+        "print_runs_by_query() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_runs_by_query", false]
+        ],
+        "print_steps_for_testcase() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_steps_for_testcase", false]
+        ],
+        "print_templates_by_query() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_templates_by_query", false]
+        ],
+        "print_testcases_from_run() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_testcases_from_run", false]
+        ],
+        "print_workitems() (pylero.cli.cmd.cmdlist method)": [
+            [3, "pylero.cli.cmd.CmdList.print_workitems", false]
         ],
         "prioritization_field (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.prioritization_field"]
+            [2, "pylero.plan.Plan.prioritization_field", false]
         ],
         "priority_opt_id (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.priority_opt_id"]
+            [2, "pylero.priority_opt.PriorityOpt.priority_opt_id", false]
+        ],
+        "priorityopt (class in pylero.priority_opt)": [
+            [2, "pylero.priority_opt.PriorityOpt", false]
+        ],
+        "priorityoptionid (class in pylero.priority_option_id)": [
+            [2, "pylero.priority_option_id.PriorityOptionId", false]
+        ],
+        "productlicense (class in pylero.product_license)": [
+            [2, "pylero.product_license.ProductLicense", false]
         ],
         "progress (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.progress"]
+            [2, "pylero.plan_statistics.PlanStatistics.progress", false]
         ],
         "progress_as_string (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.progress_as_string"]
+            [2, "pylero.plan_statistics.PlanStatistics.progress_as_string", false]
+        ],
+        "project (class in pylero.project)": [
+            [2, "pylero.project.Project", false]
         ],
         "project (pylero.baseline.baseline attribute)": [
-            [2, "pylero.baseline.Baseline.project"]
+            [2, "pylero.baseline.Baseline.project", false]
         ],
         "project (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.project"]
+            [2, "pylero.document.Document.project", false]
         ],
         "project (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.project"]
+            [2, "pylero.test_run.TestRun.project", false]
         ],
         "project (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.project"]
+            [2, "pylero.wiki_page.WikiPage.project", false]
         ],
         "project_group (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.project_group"]
+            [2, "pylero.project.Project.project_group", false]
         ],
         "project_id (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.project_id"]
+            [2, "pylero.project.Project.project_id", false]
         ],
         "project_ids (pylero.project_group.projectgroup attribute)": [
-            [2, "pylero.project_group.ProjectGroup.project_ids"]
+            [2, "pylero.project_group.ProjectGroup.project_ids", false]
         ],
         "project_uri (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.project_uri"]
+            [2, "pylero.plan.Plan.project_uri", false]
+        ],
+        "projectgroup (class in pylero.project_group)": [
+            [2, "pylero.project_group.ProjectGroup", false]
+        ],
+        "properties (class in pylero.properties)": [
+            [2, "pylero.properties.Properties", false]
         ],
         "properties (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.properties"]
+            [2, "pylero.enum_option.EnumOption.properties", false]
         ],
         "properties (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.properties"]
+            [2, "pylero.priority_opt.PriorityOpt.properties", false]
+        ],
+        "property (class in pylero.property)": [
+            [2, "pylero.property.Property", false]
         ],
         "property (pylero.properties.properties attribute)": [
-            [2, "pylero.properties.Properties.property"]
+            [2, "pylero.properties.Properties.property", false]
         ],
         "pylero": [
-            [2, "module-pylero"]
+            [2, "module-pylero", false]
         ],
         "pylero.activity": [
-            [2, "module-pylero.activity"]
+            [2, "module-pylero.activity", false]
         ],
         "pylero.activity_comment": [
-            [2, "module-pylero.activity_comment"]
+            [2, "module-pylero.activity_comment", false]
         ],
         "pylero.activity_custom_value": [
-            [2, "module-pylero.activity_custom_value"]
+            [2, "module-pylero.activity_custom_value", false]
         ],
         "pylero.activity_custom_value_entry": [
-            [2, "module-pylero.activity_custom_value_entry"]
+            [2, "module-pylero.activity_custom_value_entry", false]
         ],
         "pylero.activity_source": [
-            [2, "module-pylero.activity_source"]
+            [2, "module-pylero.activity_source", false]
         ],
         "pylero.approval": [
-            [2, "module-pylero.approval"]
+            [2, "module-pylero.approval", false]
         ],
         "pylero.attachment": [
-            [2, "module-pylero.attachment"]
+            [2, "module-pylero.attachment", false]
         ],
         "pylero.base_polarion": [
-            [2, "module-pylero.base_polarion"]
+            [2, "module-pylero.base_polarion", false]
         ],
         "pylero.baseline": [
-            [2, "module-pylero.baseline"]
+            [2, "module-pylero.baseline", false]
         ],
         "pylero.build": [
-            [2, "module-pylero.build"]
+            [2, "module-pylero.build", false]
         ],
         "pylero.build_linked_work_item": [
-            [2, "module-pylero.build_linked_work_item"]
+            [2, "module-pylero.build_linked_work_item", false]
         ],
         "pylero.build_test_results": [
-            [2, "module-pylero.build_test_results"]
+            [2, "module-pylero.build_test_results", false]
         ],
         "pylero.category": [
-            [2, "module-pylero.category"]
+            [2, "module-pylero.category", false]
         ],
         "pylero.change": [
-            [2, "module-pylero.change"]
+            [2, "module-pylero.change", false]
+        ],
+        "pylero.cli": [
+            [3, "module-pylero.cli", false]
+        ],
+        "pylero.cli.cmd": [
+            [3, "module-pylero.cli.cmd", false]
         ],
         "pylero.comment": [
-            [2, "module-pylero.comment"]
+            [2, "module-pylero.comment", false]
         ],
         "pylero.custom": [
-            [2, "module-pylero.custom"]
+            [2, "module-pylero.custom", false]
         ],
         "pylero.custom_field": [
-            [2, "module-pylero.custom_field"]
+            [2, "module-pylero.custom_field", false]
         ],
         "pylero.custom_field_type": [
-            [2, "module-pylero.custom_field_type"]
+            [2, "module-pylero.custom_field_type", false]
         ],
         "pylero.document": [
-            [2, "module-pylero.document"]
+            [2, "module-pylero.document", false]
         ],
         "pylero.enum_custom_field_type": [
-            [2, "module-pylero.enum_custom_field_type"]
+            [2, "module-pylero.enum_custom_field_type", false]
         ],
         "pylero.enum_option": [
-            [2, "module-pylero.enum_option"]
+            [2, "module-pylero.enum_option", false]
         ],
         "pylero.enum_option_id": [
-            [2, "module-pylero.enum_option_id"]
+            [2, "module-pylero.enum_option_id", false]
         ],
         "pylero.exceptions": [
-            [2, "module-pylero.exceptions"]
+            [2, "module-pylero.exceptions", false]
         ],
         "pylero.externally_linked_work_item": [
-            [2, "module-pylero.externally_linked_work_item"]
+            [2, "module-pylero.externally_linked_work_item", false]
         ],
         "pylero.field_diff": [
-            [2, "module-pylero.field_diff"]
+            [2, "module-pylero.field_diff", false]
         ],
         "pylero.hyperlink": [
-            [2, "module-pylero.hyperlink"]
+            [2, "module-pylero.hyperlink", false]
         ],
         "pylero.imported_comment": [
-            [2, "module-pylero.imported_comment"]
+            [2, "module-pylero.imported_comment", false]
         ],
         "pylero.language_definition": [
-            [2, "module-pylero.language_definition"]
+            [2, "module-pylero.language_definition", false]
         ],
         "pylero.license_info": [
-            [2, "module-pylero.license_info"]
+            [2, "module-pylero.license_info", false]
         ],
         "pylero.linked_work_item": [
-            [2, "module-pylero.linked_work_item"]
+            [2, "module-pylero.linked_work_item", false]
         ],
         "pylero.module_comment": [
-            [2, "module-pylero.module_comment"]
+            [2, "module-pylero.module_comment", false]
         ],
         "pylero.plan": [
-            [2, "module-pylero.plan"]
+            [2, "module-pylero.plan", false]
         ],
         "pylero.plan_record": [
-            [2, "module-pylero.plan_record"]
+            [2, "module-pylero.plan_record", false]
         ],
         "pylero.plan_statistics": [
-            [2, "module-pylero.plan_statistics"]
+            [2, "module-pylero.plan_statistics", false]
         ],
         "pylero.planning_constraint": [
-            [2, "module-pylero.planning_constraint"]
+            [2, "module-pylero.planning_constraint", false]
         ],
         "pylero.priority_opt": [
-            [2, "module-pylero.priority_opt"]
+            [2, "module-pylero.priority_opt", false]
         ],
         "pylero.priority_option_id": [
-            [2, "module-pylero.priority_option_id"]
+            [2, "module-pylero.priority_option_id", false]
         ],
         "pylero.product_license": [
-            [2, "module-pylero.product_license"]
+            [2, "module-pylero.product_license", false]
         ],
         "pylero.project": [
-            [2, "module-pylero.project"]
+            [2, "module-pylero.project", false]
         ],
         "pylero.project_group": [
-            [2, "module-pylero.project_group"]
+            [2, "module-pylero.project_group", false]
         ],
         "pylero.properties": [
-            [2, "module-pylero.properties"]
+            [2, "module-pylero.properties", false]
         ],
         "pylero.property": [
-            [2, "module-pylero.property"]
+            [2, "module-pylero.property", false]
         ],
         "pylero.revision": [
-            [2, "module-pylero.revision"]
+            [2, "module-pylero.revision", false]
         ],
         "pylero.server": [
-            [2, "module-pylero.server"]
+            [2, "module-pylero.server", false]
         ],
         "pylero.session": [
-            [2, "module-pylero.session"]
+            [2, "module-pylero.session", false]
         ],
         "pylero.signature": [
-            [2, "module-pylero.signature"]
+            [2, "module-pylero.signature", false]
         ],
         "pylero.signature_context": [
-            [2, "module-pylero.signature_context"]
+            [2, "module-pylero.signature_context", false]
         ],
         "pylero.signature_data": [
-            [2, "module-pylero.signature_data"]
+            [2, "module-pylero.signature_data", false]
         ],
         "pylero.subterra_uri": [
-            [2, "module-pylero.subterra_uri"]
+            [2, "module-pylero.subterra_uri", false]
         ],
         "pylero.test_record": [
-            [2, "module-pylero.test_record"]
+            [2, "module-pylero.test_record", false]
         ],
         "pylero.test_run": [
-            [2, "module-pylero.test_run"]
+            [2, "module-pylero.test_run", false]
         ],
         "pylero.test_run_attachment": [
-            [2, "module-pylero.test_run_attachment"]
+            [2, "module-pylero.test_run_attachment", false]
         ],
         "pylero.test_step": [
-            [2, "module-pylero.test_step"]
+            [2, "module-pylero.test_step", false]
         ],
         "pylero.test_step_result": [
-            [2, "module-pylero.test_step_result"]
+            [2, "module-pylero.test_step_result", false]
         ],
         "pylero.test_steps": [
-            [2, "module-pylero.test_steps"]
+            [2, "module-pylero.test_steps", false]
         ],
         "pylero.tests_configuration": [
-            [2, "module-pylero.tests_configuration"]
+            [2, "module-pylero.tests_configuration", false]
         ],
         "pylero.text": [
-            [2, "module-pylero.text"]
+            [2, "module-pylero.text", false]
         ],
         "pylero.time_point": [
-            [2, "module-pylero.time_point"]
+            [2, "module-pylero.time_point", false]
         ],
         "pylero.user": [
-            [2, "module-pylero.user"]
+            [2, "module-pylero.user", false]
         ],
         "pylero.wiki_page": [
-            [2, "module-pylero.wiki_page"]
+            [2, "module-pylero.wiki_page", false]
         ],
         "pylero.wiki_page_attachment": [
-            [2, "module-pylero.wiki_page_attachment"]
+            [2, "module-pylero.wiki_page_attachment", false]
         ],
         "pylero.work_item": [
-            [2, "module-pylero.work_item"]
+            [2, "module-pylero.work_item", false]
         ],
         "pylero.work_record": [
-            [2, "module-pylero.work_record"]
+            [2, "module-pylero.work_record", false]
         ],
         "pylero.workflow_action": [
-            [2, "module-pylero.workflow_action"]
+            [2, "module-pylero.workflow_action", false]
+        ],
+        "pylerolibexception": [
+            [2, "pylero.exceptions.PyleroLibException", false]
         ],
         "query (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.query"]
+            [2, "pylero.test_run.TestRun.query", false]
         ],
         "query() (pylero.baseline.baseline class method)": [
-            [2, "pylero.baseline.Baseline.query"]
+            [2, "pylero.baseline.Baseline.query", false]
         ],
         "query() (pylero.document.document class method)": [
-            [2, "pylero.document.Document.query"]
+            [2, "pylero.document.Document.query", false]
         ],
         "query() (pylero.revision.revision class method)": [
-            [2, "pylero.revision.Revision.query"]
+            [2, "pylero.revision.Revision.query", false]
         ],
         "query() (pylero.wiki_page.wikipage class method)": [
-            [2, "pylero.wiki_page.WikiPage.query"]
+            [2, "pylero.wiki_page.WikiPage.query", false]
         ],
         "records (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.records"]
+            [2, "pylero.plan.Plan.records", false]
         ],
         "records (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.records"]
+            [2, "pylero.test_run.TestRun.records", false]
         ],
         "records (pylero.test_run.testrun property)": [
-            [2, "id2"]
+            [2, "id2", false]
         ],
         "referred_work_item_uri (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.referred_work_item_uri"]
+            [2, "pylero.module_comment.ModuleComment.referred_work_item_uri", false]
+        ],
+        "regex_id (pylero.base_polarion.basepolarion attribute)": [
+            [2, "pylero.base_polarion.BasePolarion.REGEX_ID", false]
+        ],
+        "regex_proj (pylero.base_polarion.basepolarion attribute)": [
+            [2, "pylero.base_polarion.BasePolarion.REGEX_PROJ", false]
         ],
         "reload() (pylero.base_polarion.basepolarion method)": [
-            [2, "pylero.base_polarion.BasePolarion.reload"]
+            [2, "pylero.base_polarion.BasePolarion.reload", false]
         ],
         "remove_plan_items() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.remove_plan_items"]
+            [2, "pylero.plan.Plan.remove_plan_items", false]
         ],
         "removed (pylero.field_diff.fielddiff attribute)": [
-            [2, "pylero.field_diff.FieldDiff.removed"]
+            [2, "pylero.field_diff.FieldDiff.removed", false]
         ],
         "repo (pylero.base_polarion.basepolarion attribute)": [
-            [2, "pylero.base_polarion.BasePolarion.repo"]
+            [2, "pylero.base_polarion.BasePolarion.repo", false]
         ],
         "repository_name (pylero.revision.revision attribute)": [
-            [2, "pylero.revision.Revision.repository_name"]
+            [2, "pylero.revision.Revision.repository_name", false]
         ],
         "required (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.required"]
+            [2, "pylero.custom_field_type.CustomFieldType.required", false]
         ],
         "required (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.required"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.required", false]
         ],
         "required_features (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.required_features"]
+            [2, "pylero.workflow_action.WorkflowAction.required_features", false]
+        ],
+        "requirement (class in pylero.work_item)": [
+            [2, "pylero.work_item.Requirement", false]
         ],
         "resolved (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.resolved"]
+            [2, "pylero.comment.Comment.resolved", false]
         ],
         "resolved (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.resolved"]
+            [2, "pylero.module_comment.ModuleComment.resolved", false]
         ],
         "resource_locations (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.resource_locations"]
+            [2, "pylero.activity.Activity.resource_locations", false]
         ],
         "result (pylero.test_step_result.teststepresult attribute)": [
-            [2, "pylero.test_step_result.TestStepResult.result"]
+            [2, "pylero.test_step_result.TestStepResult.result", false]
         ],
         "result_error_enum_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.result_error_enum_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.result_error_enum_id", false]
         ],
         "result_failed_enum_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.result_failed_enum_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.result_failed_enum_id", false]
         ],
         "result_passed_enum_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.result_passed_enum_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.result_passed_enum_id", false]
         ],
         "retest_allowed (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.retest_allowed"]
+            [2, "pylero.tests_configuration.TestsConfiguration.retest_allowed", false]
         ],
         "retries (pylero.base_polarion.connection attribute)": [
-            [2, "pylero.base_polarion.Connection.retries"]
+            [2, "pylero.base_polarion.Connection.retries", false]
+        ],
+        "revision (class in pylero.revision)": [
+            [2, "pylero.revision.Revision", false]
         ],
         "revision (pylero.build_linked_work_item.buildlinkedworkitem attribute)": [
-            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem.revision"]
+            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem.revision", false]
         ],
         "revision (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.revision"]
+            [2, "pylero.change.Change.revision", false]
         ],
         "revision (pylero.linked_work_item.linkedworkitem attribute)": [
-            [2, "pylero.linked_work_item.LinkedWorkItem.revision"]
+            [2, "pylero.linked_work_item.LinkedWorkItem.revision", false]
+        ],
+        "risk (class in pylero.work_item)": [
+            [2, "pylero.work_item.Risk", false]
         ],
         "role (pylero.build_linked_work_item.buildlinkedworkitem attribute)": [
-            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem.role"]
+            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem.role", false]
         ],
         "role (pylero.externally_linked_work_item.externallylinkedworkitem attribute)": [
-            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem.role"]
+            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem.role", false]
         ],
         "role (pylero.hyperlink.hyperlink attribute)": [
-            [2, "pylero.hyperlink.Hyperlink.role"]
+            [2, "pylero.hyperlink.Hyperlink.role", false]
         ],
         "role (pylero.linked_work_item.linkedworkitem attribute)": [
-            [2, "pylero.linked_work_item.LinkedWorkItem.role"]
+            [2, "pylero.linked_work_item.LinkedWorkItem.role", false]
         ],
         "search() (pylero.plan.plan class method)": [
-            [2, "pylero.plan.Plan.search"]
+            [2, "pylero.plan.Plan.search", false]
         ],
         "search() (pylero.test_run.testrun class method)": [
-            [2, "pylero.test_run.TestRun.search"]
+            [2, "pylero.test_run.TestRun.search", false]
         ],
         "select_test_cases_by (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.select_test_cases_by"]
+            [2, "pylero.test_run.TestRun.select_test_cases_by", false]
         ],
         "sequence_number (pylero.enum_option.enumoption attribute)": [
-            [2, "pylero.enum_option.EnumOption.sequence_number"]
+            [2, "pylero.enum_option.EnumOption.sequence_number", false]
         ],
         "sequence_number (pylero.priority_opt.priorityopt attribute)": [
-            [2, "pylero.priority_opt.PriorityOpt.sequence_number"]
+            [2, "pylero.priority_opt.PriorityOpt.sequence_number", false]
+        ],
+        "server (class in pylero.server)": [
+            [2, "pylero.server.Server", false]
+        ],
+        "session (class in pylero.session)": [
+            [2, "pylero.session.Session", false]
         ],
         "session (pylero.base_polarion.basepolarion attribute)": [
-            [2, "id1"],
-            [2, "pylero.base_polarion.BasePolarion.session"]
+            [2, "id1", false],
+            [2, "pylero.base_polarion.BasePolarion.session", false]
         ],
         "session (pylero.base_polarion.connection attribute)": [
-            [2, "pylero.base_polarion.Connection.session"]
+            [2, "pylero.base_polarion.Connection.session", false]
         ],
         "session() (pylero.server.server method)": [
-            [2, "pylero.server.Server.session"]
+            [2, "pylero.server.Server.session", false]
         ],
         "set_wiki_content() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.set_wiki_content"]
+            [2, "pylero.plan.Plan.set_wiki_content", false]
+        ],
+        "signature (class in pylero.signature)": [
+            [2, "pylero.signature.Signature", false]
         ],
         "signature_contexts (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.signature_contexts"]
+            [2, "pylero.document.Document.signature_contexts", false]
         ],
         "signature_data (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.signature_data"]
+            [2, "pylero.comment.Comment.signature_data", false]
         ],
         "signature_data (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.signature_data"]
+            [2, "pylero.module_comment.ModuleComment.signature_data", false]
+        ],
+        "signaturecontext (class in pylero.signature_context)": [
+            [2, "pylero.signature_context.SignatureContext", false]
+        ],
+        "signaturedata (class in pylero.signature_data)": [
+            [2, "pylero.signature_data.SignatureData", false]
         ],
         "signatures (pylero.signature_context.signaturecontext attribute)": [
-            [2, "pylero.signature_context.SignatureContext.signatures"]
+            [2, "pylero.signature_context.SignatureContext.signatures", false]
         ],
         "signed_by (pylero.signature.signature attribute)": [
-            [2, "pylero.signature.Signature.signed_by"]
+            [2, "pylero.signature.Signature.signed_by", false]
         ],
         "signed_revision (pylero.signature.signature attribute)": [
-            [2, "pylero.signature.Signature.signed_revision"]
+            [2, "pylero.signature.Signature.signed_revision", false]
         ],
         "signer_role (pylero.signature.signature attribute)": [
-            [2, "pylero.signature.Signature.signer_role"]
+            [2, "pylero.signature.Signature.signer_role", false]
         ],
         "skipped_count (pylero.build_test_results.buildtestresults attribute)": [
-            [2, "pylero.build_test_results.BuildTestResults.skipped_count"]
+            [2, "pylero.build_test_results.BuildTestResults.skipped_count", false]
         ],
         "slots (pylero.license_info.licenseinfo attribute)": [
-            [2, "pylero.license_info.LicenseInfo.slots"]
+            [2, "pylero.license_info.LicenseInfo.slots", false]
+        ],
+        "soapnull (class in pylero.session)": [
+            [2, "pylero.session.SoapNull", false]
         ],
         "sort_order (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.sort_order"]
+            [2, "pylero.plan.Plan.sort_order", false]
         ],
         "source_id (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.source_id"]
+            [2, "pylero.activity.Activity.source_id", false]
         ],
         "space_id (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.space_id"]
+            [2, "pylero.wiki_page.WikiPage.space_id", false]
         ],
         "start (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.start"]
+            [2, "pylero.project.Project.start", false]
         ],
         "start_date (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.start_date"]
+            [2, "pylero.plan.Plan.start_date", false]
         ],
         "start_time (pylero.build.build attribute)": [
-            [2, "pylero.build.Build.start_time"]
+            [2, "pylero.build.Build.start_time", false]
         ],
         "started_on (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.started_on"]
+            [2, "pylero.plan.Plan.started_on", false]
         ],
         "status (pylero.approval.approval attribute)": [
-            [2, "pylero.approval.Approval.status"]
+            [2, "pylero.approval.Approval.status", false]
         ],
         "status (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.status"]
+            [2, "pylero.document.Document.status", false]
         ],
         "status (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.status"]
+            [2, "pylero.plan.Plan.status", false]
         ],
         "status (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.status"]
+            [2, "pylero.test_run.TestRun.status", false]
         ],
         "status_error_enum_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.status_error_enum_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.status_error_enum_id", false]
         ],
         "status_failed_enum_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.status_failed_enum_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.status_failed_enum_id", false]
         ],
         "status_ok_enum_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.status_ok_enum_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.status_ok_enum_id", false]
         ],
         "steps (pylero.test_steps.teststeps attribute)": [
-            [2, "pylero.test_steps.TestSteps.steps"]
+            [2, "pylero.test_steps.TestSteps.steps", false]
         ],
         "structure_link_role (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.structure_link_role"]
+            [2, "pylero.document.Document.structure_link_role", false]
+        ],
+        "subterrauri (class in pylero.subterra_uri)": [
+            [2, "pylero.subterra_uri.SubterraURI", false]
         ],
         "suggested_features (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.suggested_features"]
+            [2, "pylero.workflow_action.WorkflowAction.suggested_features", false]
         ],
         "summary_defect (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.summary_defect"]
+            [2, "pylero.test_run.TestRun.summary_defect", false]
         ],
         "summary_defect_severity (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.summary_defect_severity"]
+            [2, "pylero.tests_configuration.TestsConfiguration.summary_defect_severity", false]
         ],
         "suspect (pylero.linked_work_item.linkedworkitem attribute)": [
-            [2, "pylero.linked_work_item.LinkedWorkItem.suspect"]
+            [2, "pylero.linked_work_item.LinkedWorkItem.suspect", false]
         ],
         "tags (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.tags"]
+            [2, "pylero.comment.Comment.tags", false]
         ],
         "tags (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.tags"]
+            [2, "pylero.module_comment.ModuleComment.tags", false]
         ],
         "target_status (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.target_status"]
+            [2, "pylero.workflow_action.WorkflowAction.target_status", false]
         ],
         "target_status_id (pylero.signature_context.signaturecontext attribute)": [
-            [2, "pylero.signature_context.SignatureContext.target_status_id"]
+            [2, "pylero.signature_context.SignatureContext.target_status_id", false]
         ],
         "target_status_id (pylero.signature_data.signaturedata attribute)": [
-            [2, "pylero.signature_data.SignatureData.target_status_id"]
+            [2, "pylero.signature_data.SignatureData.target_status_id", false]
+        ],
+        "task (class in pylero.work_item)": [
+            [2, "pylero.work_item.Task", false]
         ],
         "template (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.template"]
+            [2, "pylero.test_run.TestRun.template", false]
         ],
         "template_uri (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.template_uri"]
+            [2, "pylero.plan.Plan.template_uri", false]
         ],
         "test_case_id_custom_field (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.test_case_id_custom_field"]
+            [2, "pylero.tests_configuration.TestsConfiguration.test_case_id_custom_field", false]
         ],
         "test_case_template (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.test_case_template"]
+            [2, "pylero.tests_configuration.TestsConfiguration.test_case_template", false]
         ],
         "test_case_test_comment_field_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.test_case_test_comment_field_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.test_case_test_comment_field_id", false]
         ],
         "test_case_test_result_field_id (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.test_case_test_result_field_id"]
+            [2, "pylero.tests_configuration.TestsConfiguration.test_case_test_result_field_id", false]
         ],
         "test_case_work_item_type (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.test_case_work_item_type"]
+            [2, "pylero.tests_configuration.TestsConfiguration.test_case_work_item_type", false]
         ],
         "test_count (pylero.build_test_results.buildtestresults attribute)": [
-            [2, "pylero.build_test_results.BuildTestResults.test_count"]
+            [2, "pylero.build_test_results.BuildTestResults.test_count", false]
         ],
         "test_run_id (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.test_run_id"]
+            [2, "pylero.test_run.TestRun.test_run_id", false]
         ],
         "test_run_template (pylero.tests_configuration.testsconfiguration attribute)": [
-            [2, "pylero.tests_configuration.TestsConfiguration.test_run_template"]
+            [2, "pylero.tests_configuration.TestsConfiguration.test_run_template", false]
         ],
         "test_run_uri (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.test_run_uri"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.test_run_uri", false]
+        ],
+        "testcase (class in pylero.work_item)": [
+            [2, "pylero.work_item.TestCase", false]
+        ],
+        "testrecord (class in pylero.test_record)": [
+            [2, "pylero.test_record.TestRecord", false]
+        ],
+        "testrun (class in pylero.test_run)": [
+            [2, "pylero.test_run.TestRun", false]
+        ],
+        "testrunattachment (class in pylero.test_run_attachment)": [
+            [2, "pylero.test_run_attachment.TestRunAttachment", false]
+        ],
+        "testsconfiguration (class in pylero.tests_configuration)": [
+            [2, "pylero.tests_configuration.TestsConfiguration", false]
+        ],
+        "teststep (class in pylero.test_step)": [
+            [2, "pylero.test_step.TestStep", false]
+        ],
+        "teststepresult (class in pylero.test_step_result)": [
+            [2, "pylero.test_step_result.TestStepResult", false]
+        ],
+        "teststeps (class in pylero.test_steps)": [
+            [2, "pylero.test_steps.TestSteps", false]
+        ],
+        "testsuite (class in pylero.work_item)": [
+            [2, "pylero.work_item.TestSuite", false]
+        ],
+        "text (class in pylero.text)": [
+            [2, "pylero.text.Text", false]
         ],
         "text (pylero.activity_comment.activitycomment attribute)": [
-            [2, "pylero.activity_comment.ActivityComment.text"]
+            [2, "pylero.activity_comment.ActivityComment.text", false]
         ],
         "text (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.text"]
+            [2, "pylero.comment.Comment.text", false]
         ],
         "text (pylero.module_comment.modulecomment attribute)": [
-            [2, "pylero.module_comment.ModuleComment.text"]
+            [2, "pylero.module_comment.ModuleComment.text", false]
         ],
         "time (pylero.time_point.timepoint attribute)": [
-            [2, "pylero.time_point.TimePoint.time"]
+            [2, "pylero.time_point.TimePoint.time", false]
         ],
         "time_point_id (pylero.time_point.timepoint attribute)": [
-            [2, "pylero.time_point.TimePoint.time_point_id"]
+            [2, "pylero.time_point.TimePoint.time_point_id", false]
         ],
         "time_spent (pylero.work_record.workrecord attribute)": [
-            [2, "pylero.work_record.WorkRecord.time_spent"]
+            [2, "pylero.work_record.WorkRecord.time_spent", false]
         ],
         "time_stamp (pylero.activity_comment.activitycomment attribute)": [
-            [2, "pylero.activity_comment.ActivityComment.time_stamp"]
+            [2, "pylero.activity_comment.ActivityComment.time_stamp", false]
+        ],
+        "timepoint (class in pylero.time_point)": [
+            [2, "pylero.time_point.TimePoint", false]
         ],
         "timestamp (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.timestamp"]
+            [2, "pylero.activity.Activity.timestamp", false]
         ],
         "title (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.title"]
+            [2, "pylero.attachment.Attachment.title", false]
         ],
         "title (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.title"]
+            [2, "pylero.comment.Comment.title", false]
         ],
         "title (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.title"]
+            [2, "pylero.document.Document.title", false]
         ],
         "title (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.title"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.title", false]
         ],
         "title (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.title"]
+            [2, "pylero.wiki_page.WikiPage.title", false]
         ],
         "title (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.title"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.title", false]
         ],
         "todo (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.todo"]
+            [2, "pylero.plan_statistics.PlanStatistics.todo", false]
         ],
         "todo_as_string (pylero.plan_statistics.planstatistics attribute)": [
-            [2, "pylero.plan_statistics.PlanStatistics.todo_as_string"]
+            [2, "pylero.plan_statistics.PlanStatistics.todo_as_string", false]
         ],
         "token_enabled (pylero.base_polarion.connection attribute)": [
-            [2, "pylero.base_polarion.Connection.token_enabled"]
+            [2, "pylero.base_polarion.Connection.token_enabled", false]
         ],
         "tracker_prefix (pylero.project.project attribute)": [
-            [2, "pylero.project.Project.tracker_prefix"]
+            [2, "pylero.project.Project.tracker_prefix", false]
         ],
         "transition_data_revision (pylero.signature_context.signaturecontext attribute)": [
-            [2, "pylero.signature_context.SignatureContext.transition_data_revision"]
+            [2, "pylero.signature_context.SignatureContext.transition_data_revision", false]
         ],
         "tx_begin() (pylero.session.session method)": [
-            [2, "pylero.session.Session.tx_begin"]
+            [2, "pylero.session.Session.tx_begin", false]
         ],
         "tx_commit() (pylero.session.session method)": [
-            [2, "pylero.session.Session.tx_commit"]
+            [2, "pylero.session.Session.tx_commit", false]
         ],
         "tx_in() (pylero.session.session method)": [
-            [2, "pylero.session.Session.tx_in"]
+            [2, "pylero.session.Session.tx_in", false]
         ],
         "tx_release() (pylero.session.session method)": [
-            [2, "pylero.session.Session.tx_release"]
+            [2, "pylero.session.Session.tx_release", false]
         ],
         "tx_rollback() (pylero.session.session method)": [
-            [2, "pylero.session.Session.tx_rollback"]
+            [2, "pylero.session.Session.tx_rollback", false]
         ],
         "tx_wrapper() (in module pylero.base_polarion)": [
-            [2, "pylero.base_polarion.tx_wrapper"]
+            [2, "pylero.base_polarion.tx_wrapper", false]
         ],
         "type (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.type"]
+            [2, "pylero.activity.Activity.type", false]
         ],
         "type (pylero.custom_field_type.customfieldtype attribute)": [
-            [2, "pylero.custom_field_type.CustomFieldType.type"]
+            [2, "pylero.custom_field_type.CustomFieldType.type", false]
         ],
         "type (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.type"]
+            [2, "pylero.document.Document.type", false]
         ],
         "type (pylero.enum_custom_field_type.enumcustomfieldtype attribute)": [
-            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.type"]
+            [2, "pylero.enum_custom_field_type.EnumCustomFieldType.type", false]
         ],
         "type (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.type"]
+            [2, "pylero.test_run.TestRun.type", false]
         ],
         "type (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.type"]
+            [2, "pylero.wiki_page.WikiPage.type", false]
         ],
         "type (pylero.work_record.workrecord attribute)": [
-            [2, "pylero.work_record.WorkRecord.type"]
+            [2, "pylero.work_record.WorkRecord.type", false]
         ],
         "types (pylero.activity_source.activitysource attribute)": [
-            [2, "pylero.activity_source.ActivitySource.types"]
+            [2, "pylero.activity_source.ActivitySource.types", false]
         ],
         "unavailability_message (pylero.workflow_action.workflowaction attribute)": [
-            [2, "pylero.workflow_action.WorkflowAction.unavailability_message"]
+            [2, "pylero.workflow_action.WorkflowAction.unavailability_message", false]
         ],
         "update() (pylero.document.document method)": [
-            [2, "pylero.document.Document.update"]
+            [2, "pylero.document.Document.update", false]
         ],
         "update() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.update"]
+            [2, "pylero.plan.Plan.update", false]
         ],
         "update() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.update"]
+            [2, "pylero.test_run.TestRun.update", false]
         ],
         "update() (pylero.user.user method)": [
-            [2, "pylero.user.User.update"]
+            [2, "pylero.user.User.update", false]
+        ],
+        "update_1_case_result_for_run() (pylero.cli.cmd.cmdupdate method)": [
+            [3, "pylero.cli.cmd.CmdUpdate.update_1_case_result_for_run", false]
+        ],
+        "update_all_case_results_for_run() (pylero.cli.cmd.cmdupdate method)": [
+            [3, "pylero.cli.cmd.CmdUpdate.update_all_case_results_for_run", false]
+        ],
+        "update_all_case_results_for_runs() (pylero.cli.cmd.cmdupdate method)": [
+            [3, "pylero.cli.cmd.CmdUpdate.update_all_case_results_for_runs", false]
         ],
         "update_attachment() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.update_attachment"]
+            [2, "pylero.test_run.TestRun.update_attachment", false]
+        ],
+        "update_document() (pylero.cli.cmd.cmdupdate method)": [
+            [3, "pylero.cli.cmd.CmdUpdate.update_document", false]
+        ],
+        "update_run() (pylero.cli.cmd.cmdupdate method)": [
+            [3, "pylero.cli.cmd.CmdUpdate.update_run", false]
+        ],
+        "update_runs() (pylero.cli.cmd.cmdupdate method)": [
+            [3, "pylero.cli.cmd.CmdUpdate.update_runs", false]
         ],
         "update_summary_defect() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.update_summary_defect"]
+            [2, "pylero.test_run.TestRun.update_summary_defect", false]
         ],
         "update_test_record_by_fields() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.update_test_record_by_fields"]
+            [2, "pylero.test_run.TestRun.update_test_record_by_fields", false]
         ],
         "update_test_record_by_object() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.update_test_record_by_object"]
+            [2, "pylero.test_run.TestRun.update_test_record_by_object", false]
         ],
         "update_wiki_content() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.update_wiki_content"]
+            [2, "pylero.test_run.TestRun.update_wiki_content", false]
         ],
         "updated (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.updated"]
+            [2, "pylero.attachment.Attachment.updated", false]
         ],
         "updated (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.updated"]
+            [2, "pylero.document.Document.updated", false]
         ],
         "updated (pylero.plan.plan attribute)": [
-            [2, "pylero.plan.Plan.updated"]
+            [2, "pylero.plan.Plan.updated", false]
         ],
         "updated (pylero.test_run.testrun attribute)": [
-            [2, "pylero.test_run.TestRun.updated"]
+            [2, "pylero.test_run.TestRun.updated", false]
         ],
         "updated (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.updated"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.updated", false]
         ],
         "updated (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.updated"]
+            [2, "pylero.wiki_page.WikiPage.updated", false]
         ],
         "updated (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.updated"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.updated", false]
         ],
         "updated_by (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.updated_by"]
+            [2, "pylero.document.Document.updated_by", false]
         ],
         "updated_by (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.updated_by"]
+            [2, "pylero.wiki_page.WikiPage.updated_by", false]
         ],
         "uri (pylero.hyperlink.hyperlink attribute)": [
-            [2, "pylero.hyperlink.Hyperlink.uri"]
+            [2, "pylero.hyperlink.Hyperlink.uri", false]
+        ],
+        "uri_id_get_replace() (pylero.base_polarion.basepolarion class method)": [
+            [2, "pylero.base_polarion.BasePolarion.URI_ID_GET_REPLACE", false]
+        ],
+        "uri_id_get_replace() (pylero.document.document class method)": [
+            [2, "pylero.document.Document.URI_ID_GET_REPLACE", false]
+        ],
+        "uri_id_set_replace() (pylero.base_polarion.basepolarion class method)": [
+            [2, "pylero.base_polarion.BasePolarion.URI_ID_SET_REPLACE", false]
+        ],
+        "uri_id_set_replace() (pylero.document.document class method)": [
+            [2, "pylero.document.Document.URI_ID_SET_REPLACE", false]
+        ],
+        "uri_struct (pylero.base_polarion.basepolarion attribute)": [
+            [2, "pylero.base_polarion.BasePolarion.URI_STRUCT", false]
+        ],
+        "uri_struct (pylero.document.document attribute)": [
+            [2, "pylero.document.Document.URI_STRUCT", false]
+        ],
+        "uri_struct (pylero.project.project attribute)": [
+            [2, "pylero.project.Project.URI_STRUCT", false]
         ],
         "url (pylero.attachment.attachment attribute)": [
-            [2, "pylero.attachment.Attachment.url"]
+            [2, "pylero.attachment.Attachment.url", false]
         ],
         "url (pylero.test_run_attachment.testrunattachment attribute)": [
-            [2, "pylero.test_run_attachment.TestRunAttachment.url"]
+            [2, "pylero.test_run_attachment.TestRunAttachment.url", false]
         ],
         "url (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.url"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.url", false]
+        ],
+        "user (class in pylero.user)": [
+            [2, "pylero.user.User", false]
         ],
         "user (pylero.approval.approval attribute)": [
-            [2, "pylero.approval.Approval.user"]
+            [2, "pylero.approval.Approval.user", false]
         ],
         "user (pylero.change.change attribute)": [
-            [2, "pylero.change.Change.user"]
+            [2, "pylero.change.Change.user", false]
         ],
         "user (pylero.signature_context.signaturecontext attribute)": [
-            [2, "pylero.signature_context.SignatureContext.user"]
+            [2, "pylero.signature_context.SignatureContext.user", false]
         ],
         "user (pylero.work_record.workrecord attribute)": [
-            [2, "pylero.work_record.WorkRecord.user"]
+            [2, "pylero.work_record.WorkRecord.user", false]
         ],
         "user_id (pylero.activity.activity attribute)": [
-            [2, "pylero.activity.Activity.user_id"]
+            [2, "pylero.activity.Activity.user_id", false]
         ],
         "user_id (pylero.activity_comment.activitycomment attribute)": [
-            [2, "pylero.activity_comment.ActivityComment.user_id"]
+            [2, "pylero.activity_comment.ActivityComment.user_id", false]
         ],
         "user_id (pylero.user.user attribute)": [
-            [2, "pylero.user.User.user_id"]
+            [2, "pylero.user.User.user_id", false]
         ],
         "uses_outline_numbering (pylero.document.document attribute)": [
-            [2, "pylero.document.Document.uses_outline_numbering"]
+            [2, "pylero.document.Document.uses_outline_numbering", false]
         ],
         "value (pylero.custom.custom attribute)": [
-            [2, "pylero.custom.Custom.value"]
+            [2, "pylero.custom.Custom.value", false]
         ],
         "value (pylero.custom_field.customfield attribute)": [
-            [2, "pylero.custom_field.CustomField.value"]
+            [2, "pylero.custom_field.CustomField.value", false]
         ],
         "value (pylero.property.property attribute)": [
-            [2, "pylero.property.Property.value"]
+            [2, "pylero.property.Property.value", false]
         ],
         "values (pylero.activity_custom_value.activitycustomvalue attribute)": [
-            [2, "pylero.activity_custom_value.ActivityCustomValue.values"]
+            [2, "pylero.activity_custom_value.ActivityCustomValue.values", false]
         ],
         "values (pylero.test_step.teststep attribute)": [
-            [2, "pylero.test_step.TestStep.values"]
+            [2, "pylero.test_step.TestStep.values", false]
         ],
         "verdict (pylero.signature.signature attribute)": [
-            [2, "pylero.signature.Signature.verdict"]
+            [2, "pylero.signature.Signature.verdict", false]
         ],
         "verdict (pylero.signature_data.signaturedata attribute)": [
-            [2, "pylero.signature_data.SignatureData.verdict"]
+            [2, "pylero.signature_data.SignatureData.verdict", false]
         ],
         "verdict_time (pylero.signature.signature attribute)": [
-            [2, "pylero.signature.Signature.verdict_time"]
+            [2, "pylero.signature.Signature.verdict_time", false]
         ],
         "verify_params() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.verify_params"]
+            [2, "pylero.test_run.TestRun.verify_params", false]
         ],
         "verify_required() (pylero.test_run.testrun method)": [
-            [2, "pylero.test_run.TestRun.verify_required"]
+            [2, "pylero.test_run.TestRun.verify_required", false]
         ],
         "visible_to (pylero.comment.comment attribute)": [
-            [2, "pylero.comment.Comment.visible_to"]
+            [2, "pylero.comment.Comment.visible_to", false]
         ],
         "vote_uris (pylero.user.user attribute)": [
-            [2, "pylero.user.User.vote_uris"]
+            [2, "pylero.user.User.vote_uris", false]
         ],
         "was_started() (pylero.plan.plan method)": [
-            [2, "pylero.plan.Plan.was_started"]
+            [2, "pylero.plan.Plan.was_started", false]
         ],
         "watche_uris (pylero.user.user attribute)": [
-            [2, "pylero.user.User.watche_uris"]
+            [2, "pylero.user.User.watche_uris", false]
         ],
         "wiki_page_attachment_id (pylero.wiki_page_attachment.wikipageattachment attribute)": [
-            [2, "pylero.wiki_page_attachment.WikiPageAttachment.wiki_page_attachment_id"]
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment.wiki_page_attachment_id", false]
         ],
         "wiki_page_id (pylero.wiki_page.wikipage attribute)": [
-            [2, "pylero.wiki_page.WikiPage.wiki_page_id"]
+            [2, "pylero.wiki_page.WikiPage.wiki_page_id", false]
+        ],
+        "wikipage (class in pylero.wiki_page)": [
+            [2, "pylero.wiki_page.WikiPage", false]
+        ],
+        "wikipageattachment (class in pylero.wiki_page_attachment)": [
+            [2, "pylero.wiki_page_attachment.WikiPageAttachment", false]
         ],
         "work_item (pylero.build_linked_work_item.buildlinkedworkitem attribute)": [
-            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem.work_item"]
+            [2, "pylero.build_linked_work_item.BuildLinkedWorkItem.work_item", false]
         ],
         "work_item_id (pylero.linked_work_item.linkedworkitem attribute)": [
-            [2, "pylero.linked_work_item.LinkedWorkItem.work_item_id"]
+            [2, "pylero.linked_work_item.LinkedWorkItem.work_item_id", false]
         ],
         "work_item_uri (pylero.externally_linked_work_item.externallylinkedworkitem attribute)": [
-            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem.work_item_uri"]
+            [2, "pylero.externally_linked_work_item.ExternallyLinkedWorkItem.work_item_uri", false]
         ],
         "work_record_id (pylero.work_record.workrecord attribute)": [
-            [2, "pylero.work_record.WorkRecord.work_record_id"]
+            [2, "pylero.work_record.WorkRecord.work_record_id", false]
         ],
-        "cmdlist (class in pylero.cli.cmd)": [
-            [3, "pylero.cli.cmd.CmdList"]
+        "workflowaction (class in pylero.workflow_action)": [
+            [2, "pylero.workflow_action.WorkflowAction", false]
         ],
-        "cmdupdate (class in pylero.cli.cmd)": [
-            [3, "pylero.cli.cmd.CmdUpdate"]
+        "workrecord (class in pylero.work_record)": [
+            [2, "pylero.work_record.WorkRecord", false]
+        ]
+    },
+    "objects": {
+        "": [
+            [2, 0, 0, "-", "pylero"]
         ],
-        "list_documents_by_query() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.list_documents_by_query"]
+        "pylero": [
+            [2, 0, 0, "-", "activity"],
+            [2, 0, 0, "-", "activity_comment"],
+            [2, 0, 0, "-", "activity_custom_value"],
+            [2, 0, 0, "-", "activity_custom_value_entry"],
+            [2, 0, 0, "-", "activity_source"],
+            [2, 0, 0, "-", "approval"],
+            [2, 0, 0, "-", "attachment"],
+            [2, 0, 0, "-", "base_polarion"],
+            [2, 0, 0, "-", "baseline"],
+            [2, 0, 0, "-", "build"],
+            [2, 0, 0, "-", "build_linked_work_item"],
+            [2, 0, 0, "-", "build_test_results"],
+            [2, 0, 0, "-", "category"],
+            [2, 0, 0, "-", "change"],
+            [3, 0, 0, "-", "cli"],
+            [2, 0, 0, "-", "comment"],
+            [2, 0, 0, "-", "custom"],
+            [2, 0, 0, "-", "custom_field"],
+            [2, 0, 0, "-", "custom_field_type"],
+            [2, 0, 0, "-", "document"],
+            [2, 0, 0, "-", "enum_custom_field_type"],
+            [2, 0, 0, "-", "enum_option"],
+            [2, 0, 0, "-", "enum_option_id"],
+            [2, 0, 0, "-", "exceptions"],
+            [2, 0, 0, "-", "externally_linked_work_item"],
+            [2, 0, 0, "-", "field_diff"],
+            [2, 0, 0, "-", "hyperlink"],
+            [2, 0, 0, "-", "imported_comment"],
+            [2, 0, 0, "-", "language_definition"],
+            [2, 0, 0, "-", "license_info"],
+            [2, 0, 0, "-", "linked_work_item"],
+            [2, 0, 0, "-", "module_comment"],
+            [2, 0, 0, "-", "plan"],
+            [2, 0, 0, "-", "plan_record"],
+            [2, 0, 0, "-", "plan_statistics"],
+            [2, 0, 0, "-", "planning_constraint"],
+            [2, 0, 0, "-", "priority_opt"],
+            [2, 0, 0, "-", "priority_option_id"],
+            [2, 0, 0, "-", "product_license"],
+            [2, 0, 0, "-", "project"],
+            [2, 0, 0, "-", "project_group"],
+            [2, 0, 0, "-", "properties"],
+            [2, 0, 0, "-", "property"],
+            [2, 0, 0, "-", "revision"],
+            [2, 0, 0, "-", "server"],
+            [2, 0, 0, "-", "session"],
+            [2, 0, 0, "-", "signature"],
+            [2, 0, 0, "-", "signature_context"],
+            [2, 0, 0, "-", "signature_data"],
+            [2, 0, 0, "-", "subterra_uri"],
+            [2, 0, 0, "-", "test_record"],
+            [2, 0, 0, "-", "test_run"],
+            [2, 0, 0, "-", "test_run_attachment"],
+            [2, 0, 0, "-", "test_step"],
+            [2, 0, 0, "-", "test_step_result"],
+            [2, 0, 0, "-", "test_steps"],
+            [2, 0, 0, "-", "tests_configuration"],
+            [2, 0, 0, "-", "text"],
+            [2, 0, 0, "-", "time_point"],
+            [2, 0, 0, "-", "user"],
+            [2, 0, 0, "-", "wiki_page"],
+            [2, 0, 0, "-", "wiki_page_attachment"],
+            [2, 0, 0, "-", "work_item"],
+            [2, 0, 0, "-", "work_record"],
+            [2, 0, 0, "-", "workflow_action"]
         ],
-        "list_workitems_by_query() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.list_workitems_by_query"]
+        "pylero.activity": [
+            [2, 1, 1, "", "Activity"]
         ],
-        "list_workitems_in_doc() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.list_workitems_in_doc"]
+        "pylero.activity.Activity": [
+            [2, 2, 1, "", "activity_custom_values"],
+            [2, 2, 1, "", "activity_id"],
+            [2, 2, 1, "", "comments"],
+            [2, 2, 1, "", "context_id"],
+            [2, 2, 1, "", "global_id"],
+            [2, 2, 1, "", "info"],
+            [2, 2, 1, "", "prefix"],
+            [2, 2, 1, "", "resource_locations"],
+            [2, 2, 1, "", "source_id"],
+            [2, 2, 1, "", "timestamp"],
+            [2, 2, 1, "", "type"],
+            [2, 2, 1, "", "user_id"]
         ],
-        "print_documents() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_documents"]
+        "pylero.activity_comment": [
+            [2, 1, 1, "", "ActivityComment"]
         ],
-        "print_links_for_requirement() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_links_for_requirement"]
+        "pylero.activity_comment.ActivityComment": [
+            [2, 2, 1, "", "text"],
+            [2, 2, 1, "", "time_stamp"],
+            [2, 2, 1, "", "user_id"]
         ],
-        "print_links_for_testcase() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_links_for_testcase"]
+        "pylero.activity_custom_value": [
+            [2, 1, 1, "", "ActivityCustomValue"]
         ],
-        "print_plan_ids() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_plan_ids"]
+        "pylero.activity_custom_value.ActivityCustomValue": [
+            [2, 2, 1, "", "values"]
         ],
-        "print_runs_by_query() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_runs_by_query"]
+        "pylero.activity_custom_value_entry": [
+            [2, 1, 1, "", "ActivityCustomValueEntry"]
         ],
-        "print_steps_for_testcase() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_steps_for_testcase"]
+        "pylero.activity_custom_value_entry.ActivityCustomValueEntry": [
+            [2, 2, 1, "", "custom_values"],
+            [2, 2, 1, "", "key"]
         ],
-        "print_templates_by_query() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_templates_by_query"]
+        "pylero.activity_source": [
+            [2, 1, 1, "", "ActivitySource"]
         ],
-        "print_testcases_from_run() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_testcases_from_run"]
+        "pylero.activity_source.ActivitySource": [
+            [2, 2, 1, "", "activity_source_id"],
+            [2, 2, 1, "", "prefix"],
+            [2, 2, 1, "", "types"]
         ],
-        "print_workitems() (pylero.cli.cmd.cmdlist method)": [
-            [3, "pylero.cli.cmd.CmdList.print_workitems"]
+        "pylero.approval": [
+            [2, 1, 1, "", "Approval"],
+            [2, 1, 1, "", "ArrayOfApproval"]
+        ],
+        "pylero.approval.Approval": [
+            [2, 2, 1, "", "status"],
+            [2, 2, 1, "", "user"]
+        ],
+        "pylero.attachment": [
+            [2, 1, 1, "", "ArrayOfAttachment"],
+            [2, 1, 1, "", "Attachment"]
+        ],
+        "pylero.attachment.Attachment": [
+            [2, 2, 1, "", "attachment_id"],
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "file_name"],
+            [2, 2, 1, "", "length"],
+            [2, 2, 1, "", "title"],
+            [2, 2, 1, "", "updated"],
+            [2, 2, 1, "", "url"]
+        ],
+        "pylero.base_polarion": [
+            [2, 1, 1, "", "BasePolarion"],
+            [2, 1, 1, "", "ClassProperty"],
+            [2, 1, 1, "", "Configuration"],
+            [2, 1, 1, "", "Connection"],
+            [2, 4, 1, "", "tx_wrapper"]
+        ],
+        "pylero.base_polarion.BasePolarion": [
+            [2, 2, 1, "", "REGEX_ID"],
+            [2, 2, 1, "", "REGEX_PROJ"],
+            [2, 3, 1, "", "URI_ID_GET_REPLACE"],
+            [2, 3, 1, "", "URI_ID_SET_REPLACE"],
+            [2, 2, 1, "", "URI_STRUCT"],
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "_cls_suds_map"],
+            [2, 2, 1, "", "_id_field"],
+            [2, 2, 1, "", "_obj_client"],
+            [2, 2, 1, "", "_obj_struct"],
+            [2, 3, 1, "", "can_add_element_to_key"],
+            [2, 3, 1, "", "can_delete_instance"],
+            [2, 3, 1, "", "can_modify_instance"],
+            [2, 3, 1, "", "can_modify_key"],
+            [2, 3, 1, "", "can_read_instance"],
+            [2, 3, 1, "", "can_read_key"],
+            [2, 3, 1, "", "can_remove_element_from_key"],
+            [2, 3, 1, "", "check_valid_field_values"],
+            [2, 3, 1, "", "custom_array_obj"],
+            [2, 3, 1, "", "custom_obj"],
+            [2, 2, 1, "id0", "default_project"],
+            [2, 3, 1, "", "get_global_roles"],
+            [2, 3, 1, "", "get_location"],
+            [2, 3, 1, "", "get_revision"],
+            [2, 3, 1, "", "get_revision_by_uri"],
+            [2, 3, 1, "", "get_revisions"],
+            [2, 3, 1, "", "get_valid_field_values"],
+            [2, 3, 1, "", "has_current_user_permission"],
+            [2, 2, 1, "", "logged_in_user_id"],
+            [2, 3, 1, "", "reload"],
+            [2, 2, 1, "", "repo"],
+            [2, 2, 1, "id1", "session"]
+        ],
+        "pylero.base_polarion.Configuration": [
+            [2, 2, 1, "", "CONFIG_SECTION"],
+            [2, 2, 1, "", "CURDIR_CONFIG"],
+            [2, 2, 1, "", "GLOBAL_CONFIG"],
+            [2, 2, 1, "", "LOCAL_CONFIG"],
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "pkgdir"]
+        ],
+        "pylero.base_polarion.Connection": [
+            [2, 2, 1, "", "connected"],
+            [2, 2, 1, "", "retries"],
+            [2, 2, 1, "", "session"],
+            [2, 2, 1, "", "token_enabled"]
+        ],
+        "pylero.baseline": [
+            [2, 1, 1, "", "Baseline"]
+        ],
+        "pylero.baseline.Baseline": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "base_revision"],
+            [2, 2, 1, "", "baseline_id"],
+            [2, 3, 1, "", "create"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "project"],
+            [2, 3, 1, "", "query"]
+        ],
+        "pylero.build": [
+            [2, 1, 1, "", "Build"]
+        ],
+        "pylero.build.Build": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "bir_location"],
+            [2, 2, 1, "", "build_descriptor_name"],
+            [2, 2, 1, "", "build_id"],
+            [2, 2, 1, "", "build_stamp"],
+            [2, 2, 1, "", "build_status"],
+            [2, 2, 1, "", "build_tag"],
+            [2, 2, 1, "", "build_test_results"],
+            [2, 2, 1, "", "calculation_descriptor_name"],
+            [2, 2, 1, "", "creation_time"],
+            [2, 2, 1, "", "finish_time"],
+            [2, 2, 1, "", "job_id"],
+            [2, 2, 1, "", "linked_work_items"],
+            [2, 2, 1, "", "local_deployment_space_name"],
+            [2, 2, 1, "", "log_files"],
+            [2, 2, 1, "", "start_time"]
+        ],
+        "pylero.build_linked_work_item": [
+            [2, 1, 1, "", "ArrayOfBuildLinkedWorkItem"],
+            [2, 1, 1, "", "BuildLinkedWorkItem"]
+        ],
+        "pylero.build_linked_work_item.BuildLinkedWorkItem": [
+            [2, 2, 1, "", "revision"],
+            [2, 2, 1, "", "role"],
+            [2, 2, 1, "", "work_item"]
+        ],
+        "pylero.build_test_results": [
+            [2, 1, 1, "", "BuildTestResults"]
+        ],
+        "pylero.build_test_results.BuildTestResults": [
+            [2, 2, 1, "", "error_count"],
+            [2, 2, 1, "", "failure_count"],
+            [2, 2, 1, "", "skipped_count"],
+            [2, 2, 1, "", "test_count"]
+        ],
+        "pylero.category": [
+            [2, 1, 1, "", "ArrayOfCategory"],
+            [2, 1, 1, "", "Category"]
+        ],
+        "pylero.category.Category": [
+            [2, 2, 1, "", "category_id"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "name"]
+        ],
+        "pylero.change": [
+            [2, 1, 1, "", "Change"]
+        ],
+        "pylero.change.Change": [
+            [2, 2, 1, "", "creation"],
+            [2, 2, 1, "", "date"],
+            [2, 2, 1, "", "diffs"],
+            [2, 2, 1, "", "empty"],
+            [2, 2, 1, "", "invalid"],
+            [2, 2, 1, "", "revision"],
+            [2, 2, 1, "", "user"]
         ],
         "pylero.cli": [
-            [3, "module-pylero.cli"]
+            [3, 0, 0, "-", "cmd"]
         ],
         "pylero.cli.cmd": [
-            [3, "module-pylero.cli.cmd"]
+            [3, 1, 1, "", "CmdList"],
+            [3, 1, 1, "", "CmdUpdate"]
         ],
-        "update_1_case_result_for_run() (pylero.cli.cmd.cmdupdate method)": [
-            [3, "pylero.cli.cmd.CmdUpdate.update_1_case_result_for_run"]
+        "pylero.cli.cmd.CmdList": [
+            [3, 3, 1, "", "list_documents_by_query"],
+            [3, 3, 1, "", "list_workitems_by_query"],
+            [3, 3, 1, "", "list_workitems_in_doc"],
+            [3, 3, 1, "", "print_documents"],
+            [3, 3, 1, "", "print_links_for_requirement"],
+            [3, 3, 1, "", "print_links_for_testcase"],
+            [3, 3, 1, "", "print_plan_ids"],
+            [3, 3, 1, "", "print_runs_by_query"],
+            [3, 3, 1, "", "print_steps_for_testcase"],
+            [3, 3, 1, "", "print_templates_by_query"],
+            [3, 3, 1, "", "print_testcases_from_run"],
+            [3, 3, 1, "", "print_workitems"]
         ],
-        "update_all_case_results_for_run() (pylero.cli.cmd.cmdupdate method)": [
-            [3, "pylero.cli.cmd.CmdUpdate.update_all_case_results_for_run"]
+        "pylero.cli.cmd.CmdUpdate": [
+            [3, 3, 1, "", "update_1_case_result_for_run"],
+            [3, 3, 1, "", "update_all_case_results_for_run"],
+            [3, 3, 1, "", "update_all_case_results_for_runs"],
+            [3, 3, 1, "", "update_document"],
+            [3, 3, 1, "", "update_run"],
+            [3, 3, 1, "", "update_runs"]
         ],
-        "update_all_case_results_for_runs() (pylero.cli.cmd.cmdupdate method)": [
-            [3, "pylero.cli.cmd.CmdUpdate.update_all_case_results_for_runs"]
+        "pylero.comment": [
+            [2, 1, 1, "", "ArrayOfComment"],
+            [2, 1, 1, "", "Comment"]
         ],
-        "update_document() (pylero.cli.cmd.cmdupdate method)": [
-            [3, "pylero.cli.cmd.CmdUpdate.update_document"]
+        "pylero.comment.Comment": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "child_comment_uris"],
+            [2, 2, 1, "", "comment_id"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "parent_comment_uri"],
+            [2, 2, 1, "", "resolved"],
+            [2, 2, 1, "", "signature_data"],
+            [2, 2, 1, "", "tags"],
+            [2, 2, 1, "", "text"],
+            [2, 2, 1, "", "title"],
+            [2, 2, 1, "", "visible_to"]
         ],
-        "update_run() (pylero.cli.cmd.cmdupdate method)": [
-            [3, "pylero.cli.cmd.CmdUpdate.update_run"]
+        "pylero.custom": [
+            [2, 1, 1, "", "ArrayOfCustom"],
+            [2, 1, 1, "", "Custom"]
         ],
-        "update_runs() (pylero.cli.cmd.cmdupdate method)": [
-            [3, "pylero.cli.cmd.CmdUpdate.update_runs"]
+        "pylero.custom.Custom": [
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "key"],
+            [2, 2, 1, "", "value"]
+        ],
+        "pylero.custom_field": [
+            [2, 1, 1, "", "CustomField"]
+        ],
+        "pylero.custom_field.CustomField": [
+            [2, 2, 1, "", "key"],
+            [2, 2, 1, "", "parent_item_uri"],
+            [2, 2, 1, "", "value"]
+        ],
+        "pylero.custom_field_type": [
+            [2, 1, 1, "", "CustomFieldType"]
+        ],
+        "pylero.custom_field_type.CustomFieldType": [
+            [2, 2, 1, "", "cft_id"],
+            [2, 2, 1, "", "default_value"],
+            [2, 2, 1, "", "depends_on"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "required"],
+            [2, 2, 1, "", "type"]
+        ],
+        "pylero.document": [
+            [2, 1, 1, "", "Document"]
+        ],
+        "pylero.document.Document": [
+            [2, 3, 1, "", "URI_ID_GET_REPLACE"],
+            [2, 3, 1, "", "URI_ID_SET_REPLACE"],
+            [2, 2, 1, "", "URI_STRUCT"],
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "add_referenced_work_item"],
+            [2, 2, 1, "", "allowed_wi_types"],
+            [2, 2, 1, "", "are_links_from_parent_to_child"],
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "auto_suspect"],
+            [2, 2, 1, "", "branched_from"],
+            [2, 2, 1, "", "branched_with_query"],
+            [2, 2, 1, "", "comments"],
+            [2, 3, 1, "", "create"],
+            [2, 3, 1, "", "create_work_item"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "custom_fields"],
+            [2, 3, 1, "", "delete"],
+            [2, 2, 1, "", "derived_fields"],
+            [2, 2, 1, "", "derived_from_link_role"],
+            [2, 2, 1, "", "derived_from_uri"],
+            [2, 3, 1, "", "export_pdf"],
+            [2, 3, 1, "", "get_documents"],
+            [2, 3, 1, "", "get_work_items"],
+            [2, 2, 1, "", "home_page_content"],
+            [2, 2, 1, "", "id"],
+            [2, 2, 1, "", "location"],
+            [2, 2, 1, "", "module_absolute_location"],
+            [2, 2, 1, "", "module_folder"],
+            [2, 2, 1, "", "module_location"],
+            [2, 2, 1, "", "module_name"],
+            [2, 3, 1, "", "move_work_item_here"],
+            [2, 2, 1, "", "project"],
+            [2, 3, 1, "", "query"],
+            [2, 2, 1, "", "signature_contexts"],
+            [2, 2, 1, "", "status"],
+            [2, 2, 1, "", "structure_link_role"],
+            [2, 2, 1, "", "title"],
+            [2, 2, 1, "", "type"],
+            [2, 3, 1, "", "update"],
+            [2, 2, 1, "", "updated"],
+            [2, 2, 1, "", "updated_by"],
+            [2, 2, 1, "", "uses_outline_numbering"]
+        ],
+        "pylero.enum_custom_field_type": [
+            [2, 1, 1, "", "EnumCustomFieldType"]
+        ],
+        "pylero.enum_custom_field_type.EnumCustomFieldType": [
+            [2, 2, 1, "", "default_value"],
+            [2, 2, 1, "", "depends_on"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "enum_id"],
+            [2, 2, 1, "", "id"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "required"],
+            [2, 2, 1, "", "type"]
+        ],
+        "pylero.enum_option": [
+            [2, 1, 1, "", "EnumOption"]
+        ],
+        "pylero.enum_option.EnumOption": [
+            [2, 2, 1, "", "default"],
+            [2, 2, 1, "", "enum_id"],
+            [2, 2, 1, "", "enum_option_id"],
+            [2, 2, 1, "", "hidden"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "phantom"],
+            [2, 2, 1, "", "properties"],
+            [2, 2, 1, "", "sequence_number"]
+        ],
+        "pylero.enum_option_id": [
+            [2, 1, 1, "", "ArrayOfEnumOptionId"],
+            [2, 1, 1, "", "EnumOptionId"]
+        ],
+        "pylero.enum_option_id.EnumOptionId": [
+            [2, 3, 1, "", "__init__"]
+        ],
+        "pylero.exceptions": [
+            [2, 5, 1, "", "PyleroLibException"]
+        ],
+        "pylero.externally_linked_work_item": [
+            [2, 1, 1, "", "ArrayOfExternallyLinkedWorkItem"],
+            [2, 1, 1, "", "ExternallyLinkedWorkItem"]
+        ],
+        "pylero.externally_linked_work_item.ExternallyLinkedWorkItem": [
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "role"],
+            [2, 2, 1, "", "work_item_uri"]
+        ],
+        "pylero.field_diff": [
+            [2, 1, 1, "", "FieldDiff"]
+        ],
+        "pylero.field_diff.FieldDiff": [
+            [2, 2, 1, "", "added"],
+            [2, 2, 1, "", "after"],
+            [2, 2, 1, "", "before"],
+            [2, 2, 1, "", "collection"],
+            [2, 2, 1, "", "field_name"],
+            [2, 2, 1, "", "removed"]
+        ],
+        "pylero.hyperlink": [
+            [2, 1, 1, "", "ArrayOfHyperlink"],
+            [2, 1, 1, "", "Hyperlink"]
+        ],
+        "pylero.hyperlink.Hyperlink": [
+            [2, 2, 1, "", "role"],
+            [2, 2, 1, "", "uri"]
+        ],
+        "pylero.imported_comment": [
+            [2, 1, 1, "", "ImportedComment"]
+        ],
+        "pylero.imported_comment.ImportedComment": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "initials"]
+        ],
+        "pylero.language_definition": [
+            [2, 1, 1, "", "LanguageDefinition"]
+        ],
+        "pylero.language_definition.LanguageDefinition": [
+            [2, 2, 1, "", "label"],
+            [2, 2, 1, "", "language_definition_id"]
+        ],
+        "pylero.license_info": [
+            [2, 1, 1, "", "LicenseInfo"]
+        ],
+        "pylero.license_info.LicenseInfo": [
+            [2, 2, 1, "", "license"],
+            [2, 2, 1, "", "slots"]
+        ],
+        "pylero.linked_work_item": [
+            [2, 1, 1, "", "ArrayOfLinkedWorkItem"],
+            [2, 1, 1, "", "LinkedWorkItem"]
+        ],
+        "pylero.linked_work_item.LinkedWorkItem": [
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "revision"],
+            [2, 2, 1, "", "role"],
+            [2, 2, 1, "", "suspect"],
+            [2, 2, 1, "", "work_item_id"]
+        ],
+        "pylero.module_comment": [
+            [2, 1, 1, "", "ArrayOfModuleComment"],
+            [2, 1, 1, "", "ModuleComment"]
+        ],
+        "pylero.module_comment.ModuleComment": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "child_comment_uris"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "imported_comment"],
+            [2, 2, 1, "", "module_comment_id"],
+            [2, 2, 1, "", "parent_comment_uri"],
+            [2, 2, 1, "", "referred_work_item_uri"],
+            [2, 2, 1, "", "resolved"],
+            [2, 2, 1, "", "signature_data"],
+            [2, 2, 1, "", "tags"],
+            [2, 2, 1, "", "text"]
+        ],
+        "pylero.plan": [
+            [2, 1, 1, "", "ArrayOfPlan"],
+            [2, 1, 1, "", "Plan"]
+        ],
+        "pylero.plan.Plan": [
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "add_plan_items"],
+            [2, 2, 1, "", "allowed_types"],
+            [2, 2, 1, "", "author_uri"],
+            [2, 2, 1, "", "calculation_type"],
+            [2, 2, 1, "", "capacity"],
+            [2, 2, 1, "", "color"],
+            [2, 3, 1, "", "create"],
+            [2, 3, 1, "", "create_plan_template"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "custom_fields"],
+            [2, 2, 1, "", "default_estimate"],
+            [2, 3, 1, "", "delete_plans"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "due_date"],
+            [2, 2, 1, "", "estimation_field"],
+            [2, 2, 1, "", "finished_on"],
+            [2, 3, 1, "", "get_statistics"],
+            [2, 3, 1, "", "get_wiki_content"],
+            [2, 2, 1, "", "is_template"],
+            [2, 2, 1, "", "location"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "parent"],
+            [2, 2, 1, "", "plan_id"],
+            [2, 2, 1, "", "previous_time_spent"],
+            [2, 2, 1, "", "prioritization_field"],
+            [2, 2, 1, "", "project_uri"],
+            [2, 2, 1, "", "records"],
+            [2, 3, 1, "", "remove_plan_items"],
+            [2, 3, 1, "", "search"],
+            [2, 3, 1, "", "set_wiki_content"],
+            [2, 2, 1, "", "sort_order"],
+            [2, 2, 1, "", "start_date"],
+            [2, 2, 1, "", "started_on"],
+            [2, 2, 1, "", "status"],
+            [2, 2, 1, "", "template_uri"],
+            [2, 3, 1, "", "update"],
+            [2, 2, 1, "", "updated"],
+            [2, 3, 1, "", "was_started"]
+        ],
+        "pylero.plan_record": [
+            [2, 1, 1, "", "ArrayOfPlanRecord"],
+            [2, 1, 1, "", "PlanRecord"]
+        ],
+        "pylero.plan_record.PlanRecord": [
+            [2, 2, 1, "", "item"]
+        ],
+        "pylero.plan_statistics": [
+            [2, 1, 1, "", "PlanStatistics"]
+        ],
+        "pylero.plan_statistics.PlanStatistics": [
+            [2, 2, 1, "", "done"],
+            [2, 2, 1, "", "done_as_string"],
+            [2, 2, 1, "", "ideal_progress"],
+            [2, 2, 1, "", "ideal_progress_as_string"],
+            [2, 2, 1, "", "number_of_planned"],
+            [2, 2, 1, "", "number_of_resolved"],
+            [2, 2, 1, "", "number_of_unresolved"],
+            [2, 2, 1, "", "planned"],
+            [2, 2, 1, "", "planned_as_string"],
+            [2, 2, 1, "", "progress"],
+            [2, 2, 1, "", "progress_as_string"],
+            [2, 2, 1, "", "todo"],
+            [2, 2, 1, "", "todo_as_string"]
+        ],
+        "pylero.planning_constraint": [
+            [2, 1, 1, "", "ArrayOfPlanningConstraint"],
+            [2, 1, 1, "", "PlanningConstraint"]
+        ],
+        "pylero.planning_constraint.PlanningConstraint": [
+            [2, 2, 1, "", "constraint"],
+            [2, 2, 1, "", "date"]
+        ],
+        "pylero.priority_opt": [
+            [2, 1, 1, "", "PriorityOpt"]
+        ],
+        "pylero.priority_opt.PriorityOpt": [
+            [2, 2, 1, "", "default"],
+            [2, 2, 1, "", "enum_id"],
+            [2, 2, 1, "", "float"],
+            [2, 2, 1, "", "hidden"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "phantom"],
+            [2, 2, 1, "", "priority_opt_id"],
+            [2, 2, 1, "", "properties"],
+            [2, 2, 1, "", "sequence_number"]
+        ],
+        "pylero.priority_option_id": [
+            [2, 1, 1, "", "ArrayOfPriorityOptionId"],
+            [2, 1, 1, "", "PriorityOptionId"]
+        ],
+        "pylero.priority_option_id.PriorityOptionId": [
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "id"]
+        ],
+        "pylero.product_license": [
+            [2, 1, 1, "", "ProductLicense"]
+        ],
+        "pylero.product_license.ProductLicense": [
+            [2, 2, 1, "", "concurrent_license_data"],
+            [2, 2, 1, "", "customer_company"],
+            [2, 2, 1, "", "customer_email"],
+            [2, 2, 1, "", "customer_name"],
+            [2, 2, 1, "", "date_created"],
+            [2, 2, 1, "", "expiration_date"],
+            [2, 2, 1, "", "generated_by"],
+            [2, 2, 1, "", "ip_address"],
+            [2, 2, 1, "", "license_format"],
+            [2, 2, 1, "", "license_profile"],
+            [2, 2, 1, "", "mac_address"],
+            [2, 2, 1, "", "named_license_data"]
+        ],
+        "pylero.project": [
+            [2, 1, 1, "", "Project"]
+        ],
+        "pylero.project.Project": [
+            [2, 2, 1, "", "URI_STRUCT"],
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "active"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "finish"],
+            [2, 3, 1, "", "get_categories"],
+            [2, 3, 1, "", "get_context_roles"],
+            [2, 3, 1, "", "get_defined_custom_field_keys"],
+            [2, 3, 1, "", "get_defined_custom_field_type"],
+            [2, 3, 1, "", "get_defined_custom_field_types"],
+            [2, 3, 1, "", "get_document_spaces"],
+            [2, 3, 1, "", "get_project_users"],
+            [2, 3, 1, "", "get_test_steps_configuration"],
+            [2, 3, 1, "", "get_tests_configuration"],
+            [2, 3, 1, "", "get_wiki_spaces"],
+            [2, 2, 1, "", "lead"],
+            [2, 2, 1, "", "location"],
+            [2, 2, 1, "", "lock_work_records_date"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "project_group"],
+            [2, 2, 1, "", "project_id"],
+            [2, 2, 1, "", "start"],
+            [2, 2, 1, "", "tracker_prefix"]
+        ],
+        "pylero.project_group": [
+            [2, 1, 1, "", "ProjectGroup"]
+        ],
+        "pylero.project_group.ProjectGroup": [
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "get_contained_groups"],
+            [2, 3, 1, "", "get_contained_projects"],
+            [2, 3, 1, "", "get_deep_contained_projects"],
+            [2, 3, 1, "", "get_root_project_group"],
+            [2, 2, 1, "", "group_uris"],
+            [2, 2, 1, "", "location"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "parent_uri"],
+            [2, 2, 1, "", "project_ids"]
+        ],
+        "pylero.properties": [
+            [2, 1, 1, "", "Properties"]
+        ],
+        "pylero.properties.Properties": [
+            [2, 2, 1, "", "property"]
+        ],
+        "pylero.property": [
+            [2, 1, 1, "", "Property"]
+        ],
+        "pylero.property.Property": [
+            [2, 2, 1, "", "key"],
+            [2, 2, 1, "", "value"]
+        ],
+        "pylero.revision": [
+            [2, 1, 1, "", "ArrayOfRevision"],
+            [2, 1, 1, "", "Revision"]
+        ],
+        "pylero.revision.Revision": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "internal_commit"],
+            [2, 2, 1, "", "linked_work_item_uris"],
+            [2, 2, 1, "", "message"],
+            [2, 2, 1, "", "name"],
+            [2, 3, 1, "", "query"],
+            [2, 2, 1, "", "repository_name"]
+        ],
+        "pylero.server": [
+            [2, 1, 1, "", "Server"]
+        ],
+        "pylero.server.Server": [
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "session"]
+        ],
+        "pylero.session": [
+            [2, 1, 1, "", "ListenFilter"],
+            [2, 1, 1, "", "Session"],
+            [2, 1, 1, "", "SoapNull"],
+            [2, 4, 1, "", "create_ssl_context"]
+        ],
+        "pylero.session.ListenFilter": [
+            [2, 3, 1, "", "filter"]
+        ],
+        "pylero.session.Session": [
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "tx_begin"],
+            [2, 3, 1, "", "tx_commit"],
+            [2, 3, 1, "", "tx_in"],
+            [2, 3, 1, "", "tx_release"],
+            [2, 3, 1, "", "tx_rollback"]
+        ],
+        "pylero.session.SoapNull": [
+            [2, 3, 1, "", "add_nil"],
+            [2, 3, 1, "", "marshalled"]
+        ],
+        "pylero.signature": [
+            [2, 1, 1, "", "ArrayOfSignature"],
+            [2, 1, 1, "", "Signature"]
+        ],
+        "pylero.signature.Signature": [
+            [2, 2, 1, "", "signed_by"],
+            [2, 2, 1, "", "signed_revision"],
+            [2, 2, 1, "", "signer_role"],
+            [2, 2, 1, "", "verdict"],
+            [2, 2, 1, "", "verdict_time"]
+        ],
+        "pylero.signature_context": [
+            [2, 1, 1, "", "ArrayOfSignatureContext"],
+            [2, 1, 1, "", "SignatureContext"]
+        ],
+        "pylero.signature_context.SignatureContext": [
+            [2, 2, 1, "", "signatures"],
+            [2, 2, 1, "", "target_status_id"],
+            [2, 2, 1, "", "transition_data_revision"],
+            [2, 2, 1, "", "user"]
+        ],
+        "pylero.signature_data": [
+            [2, 1, 1, "", "SignatureData"]
+        ],
+        "pylero.signature_data.SignatureData": [
+            [2, 2, 1, "", "target_status_id"],
+            [2, 2, 1, "", "verdict"]
+        ],
+        "pylero.subterra_uri": [
+            [2, 1, 1, "", "ArrayOfSubterraURI"],
+            [2, 1, 1, "", "SubterraURI"]
+        ],
+        "pylero.subterra_uri.ArrayOfSubterraURI": [
+            [2, 3, 1, "", "__init__"]
+        ],
+        "pylero.subterra_uri.SubterraURI": [
+            [2, 3, 1, "", "__init__"]
+        ],
+        "pylero.test_record": [
+            [2, 1, 1, "", "ArrayOfTestRecord"],
+            [2, 1, 1, "", "TestRecord"]
+        ],
+        "pylero.test_record.TestRecord": [
+            [2, 3, 1, "", "__init__"]
+        ],
+        "pylero.test_run": [
+            [2, 1, 1, "", "TestRun"]
+        ],
+        "pylero.test_run.TestRun": [
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "add_attachment"],
+            [2, 3, 1, "", "add_attachment_to_test_record"],
+            [2, 3, 1, "", "add_attachment_to_test_step"],
+            [2, 3, 1, "", "add_test_record_by_fields"],
+            [2, 3, 1, "", "add_test_record_by_object"],
+            [2, 2, 1, "", "attachments"],
+            [2, 2, 1, "", "author"],
+            [2, 3, 1, "", "create"],
+            [2, 3, 1, "", "create_summary_defect"],
+            [2, 3, 1, "", "create_template"],
+            [2, 2, 1, "", "created"],
+            [2, 2, 1, "", "custom_fields"],
+            [2, 3, 1, "", "delete_attachment"],
+            [2, 3, 1, "", "delete_attachment_from_test_record"],
+            [2, 3, 1, "", "delete_attachment_from_test_step"],
+            [2, 2, 1, "", "document"],
+            [2, 2, 1, "", "finished_on"],
+            [2, 3, 1, "", "get_attachment"],
+            [2, 3, 1, "", "get_attachments"],
+            [2, 3, 1, "", "get_custom_field"],
+            [2, 3, 1, "", "get_defined_custom_field_types"],
+            [2, 3, 1, "", "get_wiki_content"],
+            [2, 2, 1, "", "group_id"],
+            [2, 2, 1, "", "is_template"],
+            [2, 2, 1, "", "keep_in_history"],
+            [2, 2, 1, "", "location"],
+            [2, 2, 1, "", "project"],
+            [2, 2, 1, "", "query"],
+            [2, 6, 1, "id2", "records"],
+            [2, 3, 1, "", "search"],
+            [2, 2, 1, "", "select_test_cases_by"],
+            [2, 2, 1, "", "status"],
+            [2, 2, 1, "", "summary_defect"],
+            [2, 2, 1, "", "template"],
+            [2, 2, 1, "", "test_run_id"],
+            [2, 2, 1, "", "type"],
+            [2, 3, 1, "", "update"],
+            [2, 3, 1, "", "update_attachment"],
+            [2, 3, 1, "", "update_summary_defect"],
+            [2, 3, 1, "", "update_test_record_by_fields"],
+            [2, 3, 1, "", "update_test_record_by_object"],
+            [2, 3, 1, "", "update_wiki_content"],
+            [2, 2, 1, "", "updated"],
+            [2, 3, 1, "", "verify_params"],
+            [2, 3, 1, "", "verify_required"]
+        ],
+        "pylero.test_run_attachment": [
+            [2, 1, 1, "", "ArrayOfTestRunAttachment"],
+            [2, 1, 1, "", "TestRunAttachment"]
+        ],
+        "pylero.test_run_attachment.TestRunAttachment": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "file_name"],
+            [2, 2, 1, "", "id"],
+            [2, 2, 1, "", "length"],
+            [2, 2, 1, "", "test_run_uri"],
+            [2, 2, 1, "", "title"],
+            [2, 2, 1, "", "updated"],
+            [2, 2, 1, "", "url"]
+        ],
+        "pylero.test_step": [
+            [2, 1, 1, "", "ArrayOfTestStep"],
+            [2, 1, 1, "", "TestStep"]
+        ],
+        "pylero.test_step.TestStep": [
+            [2, 2, 1, "", "values"]
+        ],
+        "pylero.test_step_result": [
+            [2, 1, 1, "", "ArrayOfTestStepResult"],
+            [2, 1, 1, "", "TestStepResult"]
+        ],
+        "pylero.test_step_result.TestStepResult": [
+            [2, 2, 1, "", "attachments"],
+            [2, 2, 1, "", "comment"],
+            [2, 2, 1, "", "result"]
+        ],
+        "pylero.test_steps": [
+            [2, 1, 1, "", "TestSteps"]
+        ],
+        "pylero.test_steps.TestSteps": [
+            [2, 2, 1, "", "keys"],
+            [2, 2, 1, "", "steps"]
+        ],
+        "pylero.tests_configuration": [
+            [2, 1, 1, "", "TestsConfiguration"]
+        ],
+        "pylero.tests_configuration.TestsConfiguration": [
+            [2, 2, 1, "", "defect_auto_assignement_enabled"],
+            [2, 2, 1, "", "defect_reuse_type"],
+            [2, 2, 1, "", "defect_template"],
+            [2, 2, 1, "", "defect_to_test_case_link_role_id"],
+            [2, 2, 1, "", "defect_work_item_type"],
+            [2, 2, 1, "", "defects_project"],
+            [2, 2, 1, "", "fields_to_copy_from_test_case_to_defect"],
+            [2, 2, 1, "", "fields_to_copy_from_test_run_to_linked_defect"],
+            [2, 2, 1, "", "fields_to_copy_from_test_run_to_new_defect"],
+            [2, 2, 1, "", "max_created_defects"],
+            [2, 2, 1, "", "max_created_defects_percent"],
+            [2, 2, 1, "", "result_error_enum_id"],
+            [2, 2, 1, "", "result_failed_enum_id"],
+            [2, 2, 1, "", "result_passed_enum_id"],
+            [2, 2, 1, "", "retest_allowed"],
+            [2, 2, 1, "", "status_error_enum_id"],
+            [2, 2, 1, "", "status_failed_enum_id"],
+            [2, 2, 1, "", "status_ok_enum_id"],
+            [2, 2, 1, "", "summary_defect_severity"],
+            [2, 2, 1, "", "test_case_id_custom_field"],
+            [2, 2, 1, "", "test_case_template"],
+            [2, 2, 1, "", "test_case_test_comment_field_id"],
+            [2, 2, 1, "", "test_case_test_result_field_id"],
+            [2, 2, 1, "", "test_case_work_item_type"],
+            [2, 2, 1, "", "test_run_template"]
+        ],
+        "pylero.text": [
+            [2, 1, 1, "", "ArrayOfText"],
+            [2, 1, 1, "", "Text"]
+        ],
+        "pylero.text.Text": [
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "content"],
+            [2, 2, 1, "", "content_lossy"],
+            [2, 2, 1, "", "content_type"]
+        ],
+        "pylero.time_point": [
+            [2, 1, 1, "", "TimePoint"]
+        ],
+        "pylero.time_point.TimePoint": [
+            [2, 2, 1, "", "closed"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "earliest_planned_start"],
+            [2, 2, 1, "", "name"],
+            [2, 2, 1, "", "time"],
+            [2, 2, 1, "", "time_point_id"]
+        ],
+        "pylero.user": [
+            [2, 1, 1, "", "ArrayOfUser"],
+            [2, 1, 1, "", "User"]
+        ],
+        "pylero.user.User": [
+            [2, 3, 1, "", "__init__"],
+            [2, 3, 1, "", "create_user"],
+            [2, 2, 1, "", "description"],
+            [2, 2, 1, "", "disabled_notifications"],
+            [2, 2, 1, "", "email"],
+            [2, 3, 1, "", "get_context_roles"],
+            [2, 3, 1, "", "get_roles"],
+            [2, 3, 1, "", "get_user_avatar_url"],
+            [2, 3, 1, "", "get_user_from_token"],
+            [2, 3, 1, "", "get_users"],
+            [2, 3, 1, "", "has_permission"],
+            [2, 2, 1, "", "name"],
+            [2, 3, 1, "", "update"],
+            [2, 2, 1, "", "user_id"],
+            [2, 2, 1, "", "vote_uris"],
+            [2, 2, 1, "", "watche_uris"]
+        ],
+        "pylero.wiki_page": [
+            [2, 1, 1, "", "WikiPage"]
+        ],
+        "pylero.wiki_page.WikiPage": [
+            [2, 3, 1, "", "__init__"],
+            [2, 2, 1, "", "attachments"],
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "created"],
+            [2, 3, 1, "", "get_wiki_pages"],
+            [2, 2, 1, "", "home_page_content"],
+            [2, 2, 1, "", "linked_page_uris"],
+            [2, 2, 1, "", "location"],
+            [2, 2, 1, "", "page_location"],
+            [2, 2, 1, "", "page_name"],
+            [2, 2, 1, "", "project"],
+            [2, 3, 1, "", "query"],
+            [2, 2, 1, "", "space_id"],
+            [2, 2, 1, "", "title"],
+            [2, 2, 1, "", "type"],
+            [2, 2, 1, "", "updated"],
+            [2, 2, 1, "", "updated_by"],
+            [2, 2, 1, "", "wiki_page_id"]
+        ],
+        "pylero.wiki_page_attachment": [
+            [2, 1, 1, "", "ArrayOfWikiPageAttachment"],
+            [2, 1, 1, "", "WikiPageAttachment"]
+        ],
+        "pylero.wiki_page_attachment.WikiPageAttachment": [
+            [2, 2, 1, "", "author"],
+            [2, 2, 1, "", "file_name"],
+            [2, 2, 1, "", "length"],
+            [2, 2, 1, "", "title"],
+            [2, 2, 1, "", "updated"],
+            [2, 2, 1, "", "url"],
+            [2, 2, 1, "", "wiki_page_attachment_id"]
+        ],
+        "pylero.work_item": [
+            [2, 1, 1, "", "BusinessCase"],
+            [2, 1, 1, "", "ChangeRequest"],
+            [2, 1, 1, "", "Defect"],
+            [2, 1, 1, "", "IncidentReport"],
+            [2, 1, 1, "", "Requirement"],
+            [2, 1, 1, "", "Risk"],
+            [2, 1, 1, "", "Task"],
+            [2, 1, 1, "", "TestCase"],
+            [2, 1, 1, "", "TestSuite"],
+            [2, 2, 1, "", "newclass"]
+        ],
+        "pylero.work_record": [
+            [2, 1, 1, "", "ArrayOfWorkRecord"],
+            [2, 1, 1, "", "WorkRecord"]
+        ],
+        "pylero.work_record.WorkRecord": [
+            [2, 2, 1, "", "comment"],
+            [2, 2, 1, "", "date"],
+            [2, 2, 1, "", "time_spent"],
+            [2, 2, 1, "", "type"],
+            [2, 2, 1, "", "user"],
+            [2, 2, 1, "", "work_record_id"]
+        ],
+        "pylero.workflow_action": [
+            [2, 1, 1, "", "WorkflowAction"]
+        ],
+        "pylero.workflow_action.WorkflowAction": [
+            [2, 2, 1, "", "action_id"],
+            [2, 2, 1, "", "action_name"],
+            [2, 2, 1, "", "cleaned_features"],
+            [2, 2, 1, "", "native_action_id"],
+            [2, 2, 1, "", "required_features"],
+            [2, 2, 1, "", "suggested_features"],
+            [2, 2, 1, "", "target_status"],
+            [2, 2, 1, "", "unavailability_message"]
         ]
+    },
+    "objnames": {
+        "0": ["py", "module", "Python module"],
+        "1": ["py", "class", "Python class"],
+        "2": ["py", "attribute", "Python attribute"],
+        "3": ["py", "method", "Python method"],
+        "4": ["py", "function", "Python function"],
+        "5": ["py", "exception", "Python exception"],
+        "6": ["py", "property", "Python property"]
+    },
+    "objtypes": {
+        "0": "py:module",
+        "1": "py:class",
+        "2": "py:attribute",
+        "3": "py:method",
+        "4": "py:function",
+        "5": "py:exception",
+        "6": "py:property"
+    },
+    "terms": {
+        "": 2,
+        "0": [0, 2],
+        "1": [0, 2],
+        "10": [0, 2],
+        "11": 0,
+        "12": 2,
+        "120": 2,
+        "12345": 0,
+        "1813": 0,
+        "1824": 0,
+        "1st": 0,
+        "2": [0, 2],
+        "20120313": 0,
+        "2013": 0,
+        "2015": 0,
+        "2019": 0,
+        "21": 0,
+        "2828": 0,
+        "2nd": 0,
+        "3": [0, 2],
+        "32": 0,
+        "4": 0,
+        "50": 0,
+        "6": 0,
+        "60": 2,
+        "7": [0, 2],
+        "84292": 0,
+        "A": 0,
+        "AND": 0,
+        "By": 0,
+        "For": 2,
+        "If": [0, 2],
+        "In": [0, 2],
+        "It": 2,
+        "The": [0, 2],
+        "There": 0,
+        "These": [0, 2],
+        "To": [0, 2],
+        "__init__": [1, 2],
+        "_cls_suds_map": [1, 2],
+        "_id_field": [1, 2],
+        "_obj_client": [1, 2],
+        "_obj_struct": [1, 2],
+        "_specificworkitem": 2,
+        "_workitem": [0, 2],
+        "a3": 2,
+        "a4": 2,
+        "abl": 0,
+        "about": [0, 2],
+        "abov": 0,
+        "accept": 2,
+        "access": [0, 2],
+        "accordingli": 2,
+        "action_id": [1, 2],
+        "action_nam": [1, 2],
+        "activ": [0, 1],
+        "activity_com": [0, 1],
+        "activity_custom_valu": [0, 1],
+        "activity_custom_value_entri": [0, 1],
+        "activity_id": [1, 2],
+        "activity_sourc": [0, 1],
+        "activity_source_id": [1, 2],
+        "activitycom": [0, 1, 2],
+        "activitycustomvalu": [0, 1, 2],
+        "activitycustomvalueentri": [0, 1, 2],
+        "activitysourc": [0, 1, 2],
+        "ad": [0, 1, 2],
+        "add": [0, 2],
+        "add_attach": [1, 2],
+        "add_attachment_to_test_record": [1, 2],
+        "add_attachment_to_test_step": [1, 2],
+        "add_linked_item": 0,
+        "add_nil": [1, 2],
+        "add_plan_item": [1, 2],
+        "add_referenced_work_item": [1, 2],
+        "add_test_record_by_field": [0, 1, 2],
+        "add_test_record_by_object": [0, 1, 2],
+        "addattachmenttotestrecord": 2,
+        "addattachmenttotestrun": 2,
+        "addattachmenttoteststep": 2,
+        "addit": 2,
+        "additional_parm": 2,
+        "addplanitem": 2,
+        "addtestrecordtotestrun": 2,
+        "admin": 0,
+        "after": [0, 1, 2],
+        "again": 2,
+        "against": 2,
+        "alia": 2,
+        "all": [0, 2],
+        "allow": [0, 2],
+        "allowed_typ": [1, 2],
+        "allowed_wi_typ": [1, 2],
+        "alreadi": [0, 2],
+        "also": [0, 2],
+        "altern": 0,
+        "amount": 2,
+        "an": [0, 2, 3],
+        "ani": [0, 2],
+        "anoth": 2,
+        "anytyp": 2,
+        "api": [0, 2],
+        "applic": 2,
+        "approv": [0, 1],
+        "ar": [0, 2],
+        "arch": 0,
+        "are_links_from_parent_to_child": [1, 2],
+        "aren": 0,
+        "arg": 2,
+        "argument": 2,
+        "arr_step": 0,
+        "arrai": 2,
+        "arrayof_tns3_fielddiff": 2,
+        "arrayof_tns3_licenseinfo": 2,
+        "arrayof_xsd_anytyp": 2,
+        "arrayof_xsd_str": 2,
+        "arrayofapprov": [0, 1, 2],
+        "arrayofattach": [0, 1, 2],
+        "arrayofbuildlinkedworkitem": [0, 1, 2],
+        "arrayofcategori": [0, 1, 2],
+        "arrayofcom": [0, 1, 2],
+        "arrayofcustom": [0, 1, 2],
+        "arrayofenumoptionid": [0, 1, 2],
+        "arrayofexternallylinkedworkitem": [0, 1, 2],
+        "arrayofhyperlink": [0, 1, 2],
+        "arrayoflinkedworkitem": [0, 1, 2],
+        "arrayofloc": 2,
+        "arrayofmodulecom": [0, 1, 2],
+        "arrayofplan": [0, 1, 2],
+        "arrayofplanningconstraint": [0, 1, 2],
+        "arrayofplanrecord": [0, 1, 2],
+        "arrayofpriorityoptionid": [0, 1, 2],
+        "arrayofrevis": [0, 1, 2],
+        "arrayofsignatur": [0, 1, 2],
+        "arrayofsignaturecontext": [0, 1, 2],
+        "arrayofstr": 2,
+        "arrayofsubterrauri": [0, 1, 2],
+        "arrayoftestrecord": [0, 1, 2],
+        "arrayoftestrunattach": [0, 1, 2],
+        "arrayofteststep": [0, 1, 2],
+        "arrayofteststepresult": [0, 1, 2],
+        "arrayoftext": [0, 1, 2],
+        "arrayofus": [0, 1, 2],
+        "arrayofwikipageattach": [0, 1, 2],
+        "arrayofworkrecord": [0, 1, 2],
+        "assign": 2,
+        "assigne": 3,
+        "attach": [0, 1],
+        "attachment_id": [1, 2],
+        "attr": 2,
+        "attribut": [0, 2],
+        "author": [0, 1, 2],
+        "author_uri": [1, 2],
+        "auto_suspect": [1, 2],
+        "autogen": 2,
+        "automat": [0, 2],
+        "automated_process": 2,
+        "automaticlli": 0,
+        "autopep8": 0,
+        "autoupd": 0,
+        "avail": 2,
+        "avatar": 2,
+        "base": [0, 2, 3],
+        "base_polarion": [0, 1],
+        "base_revis": [1, 2],
+        "baselin": [0, 1],
+        "baseline_id": [1, 2],
+        "baseline_revis": 2,
+        "basepolarion": [0, 1, 2],
+        "becaus": 2,
+        "been": [0, 2],
+        "befor": [1, 2],
+        "being": 0,
+        "below": [0, 2],
+        "between": 0,
+        "bir_loc": [1, 2],
+        "blank": [0, 2],
+        "block": 2,
+        "bookmark": 2,
+        "bool": 2,
+        "boolean": 2,
+        "both": 0,
+        "branched_from": [1, 2],
+        "branched_with_queri": [1, 2],
+        "build": 1,
+        "build_descriptor_nam": [1, 2],
+        "build_id": [1, 2],
+        "build_linked_work_item": [0, 1],
+        "build_stamp": [1, 2],
+        "build_statu": [1, 2],
+        "build_tag": [1, 2],
+        "build_test_result": [0, 1],
+        "buildlinkedworkitem": [0, 1, 2],
+        "buildtestresult": [0, 1, 2],
+        "bundl": 2,
+        "businesscas": [0, 1, 2],
+        "ca": [0, 2],
+        "cach": 2,
+        "caching_polici": 2,
+        "calculation_descriptor_nam": [1, 2],
+        "calculation_typ": [1, 2],
+        "call": 2,
+        "can": [0, 2],
+        "can_add_element_to_kei": [1, 2],
+        "can_delete_inst": [1, 2],
+        "can_modify_inst": [1, 2],
+        "can_modify_kei": [1, 2],
+        "can_read_inst": [1, 2],
+        "can_read_kei": [1, 2],
+        "can_remove_element_from_kei": [1, 2],
+        "canaddelementtokei": 2,
+        "candeleteinst": 2,
+        "canmodifyinst": 2,
+        "canmodifykei": 2,
+        "cannot": 2,
+        "canreadinst": 2,
+        "canreadkei": 2,
+        "canremoveelementfromkei": 2,
+        "capac": [1, 2],
+        "care": 0,
+        "case": [0, 2],
+        "case_id": 3,
+        "caseautom": 0,
+        "caseimport": 0,
+        "caselevel": 0,
+        "caseposneg": 0,
+        "categori": [0, 1],
+        "category_id": [1, 2],
+        "caus": 2,
+        "cert": 0,
+        "cert_path": [0, 2],
+        "certif": [0, 2],
+        "cfg": [0, 2],
+        "cft_id": [1, 2],
+        "chang": [0, 1],
+        "changelog": 0,
+        "changerequest": [0, 1, 2],
+        "check": [0, 2],
+        "check_valid_field_valu": [1, 2],
+        "child": 2,
+        "child_comment_uri": [1, 2],
+        "children": 2,
+        "choos": 2,
+        "ci": 0,
+        "class": [0, 2, 3],
+        "classmethod": 2,
+        "classproperti": [0, 1, 2],
+        "cleaned_featur": [1, 2],
+        "cli": [0, 1, 2],
+        "click": 0,
+        "client": 2,
+        "clone": 0,
+        "close": [1, 2],
+        "cluster": 0,
+        "cmd": [1, 2],
+        "cmdlist": [2, 3],
+        "cmdupdat": [2, 3],
+        "code": [0, 2],
+        "collect": [1, 2],
+        "color": [1, 2],
+        "com": [0, 2],
+        "command": [0, 3],
+        "comment": [0, 1, 3],
+        "comment_id": [1, 2],
+        "complet": 2,
+        "compon": [0, 2],
+        "concern": 0,
+        "concurrent_license_data": [1, 2],
+        "config": [0, 2],
+        "config_sect": [1, 2],
+        "configuar": 2,
+        "configur": [1, 2],
+        "conn": 2,
+        "connect": [0, 1, 2],
+        "constraint": [1, 2],
+        "constructor": 2,
+        "contain": 2,
+        "content": [0, 1],
+        "content_lossi": [1, 2],
+        "content_typ": [1, 2],
+        "context": 2,
+        "context_id": [1, 2],
+        "contextid": 2,
+        "control": 2,
+        "convent": 0,
+        "copyright": 0,
+        "could": 0,
+        "count": 2,
+        "creat": [0, 1, 2],
+        "create_incid": 2,
+        "create_plan_templ": [1, 2],
+        "create_ssl_context": [0, 1, 2],
+        "create_summary_defect": [1, 2],
+        "create_templ": [0, 1, 2],
+        "create_us": [1, 2],
+        "create_work_item": [0, 1, 2],
+        "createbaselin": 2,
+        "createdocu": 2,
+        "createplan": 2,
+        "createplantempl": 2,
+        "createsummarydefect": 2,
+        "createtestrun": 2,
+        "createus": 2,
+        "createworkiteminmodul": 2,
+        "creation": [1, 2],
+        "creation_tim": [1, 2],
+        "credit": 0,
+        "critic": 0,
+        "curdir_config": [1, 2],
+        "current": [0, 2],
+        "custom": [0, 1],
+        "custom_array_obj": [1, 2],
+        "custom_field": [0, 1],
+        "custom_field_id": 2,
+        "custom_field_typ": [0, 1],
+        "custom_obj": [1, 2],
+        "custom_valu": [1, 2],
+        "customer_compani": [1, 2],
+        "customer_email": [1, 2],
+        "customer_nam": [1, 2],
+        "customfield": [0, 1, 2],
+        "customfieldtyp": [0, 1, 2],
+        "data": [0, 2],
+        "dataandop": 2,
+        "datatyp": 2,
+        "date": [1, 2],
+        "date_cr": [1, 2],
+        "datetim": [0, 2],
+        "date\u05d0im": 2,
+        "dc": 0,
+        "deep": 2,
+        "default": [0, 1, 2],
+        "default_estim": [1, 2],
+        "default_project": [0, 1, 2],
+        "default_valu": [1, 2],
+        "defect": [0, 1, 2],
+        "defect_auto_assignement_en": [1, 2],
+        "defect_case_id": 2,
+        "defect_reuse_typ": [1, 2],
+        "defect_templ": [1, 2],
+        "defect_template_id": 2,
+        "defect_to_test_case_link_role_id": [1, 2],
+        "defect_work_item_id": [0, 2],
+        "defect_work_item_typ": [1, 2],
+        "defects_project": [1, 2],
+        "defin": [0, 2],
+        "definit": 2,
+        "delet": [1, 2],
+        "delete_attach": [1, 2],
+        "delete_attachment_from_test_record": [1, 2],
+        "delete_attachment_from_test_step": [1, 2],
+        "delete_plan": [1, 2],
+        "deleteattachmentfromtestrecord": 2,
+        "deleteplan": 2,
+        "deletetestrunattach": 2,
+        "depend": 0,
+        "depends_on": [1, 2],
+        "derived_field": [1, 2],
+        "derived_from_link_rol": [1, 2],
+        "derived_from_uri": [1, 2],
+        "descript": [0, 1, 2, 3],
+        "desir": 2,
+        "destin": 2,
+        "detail": [0, 2],
+        "determin": 2,
+        "develop": [0, 2],
+        "dict": [0, 2],
+        "dict_valu": 0,
+        "did": 2,
+        "diff": [0, 1, 2],
+        "differ": [0, 2],
+        "dir": [0, 2],
+        "directli": 2,
+        "directori": [0, 2],
+        "disabled_notif": [1, 2],
+        "dno": 2,
+        "do": 2,
+        "doc": [0, 2, 3],
+        "doc_nam": [2, 3],
+        "doc_name_with_spac": 3,
+        "doc_titl": 3,
+        "doc_typ": 3,
+        "doc_with_spac": [0, 2],
+        "document": 1,
+        "document_id": 2,
+        "document_nam": 2,
+        "document_titl": 2,
+        "document_typ": [0, 2],
+        "doe": [0, 2],
+        "don": 0,
+        "done": [1, 2],
+        "done_as_str": [1, 2],
+        "download": [0, 2],
+        "due_dat": [1, 2],
+        "durat": [0, 2],
+        "dynam": [0, 2],
+        "dynamic_livedoc": 2,
+        "dynamic_queri": 2,
+        "e": 2,
+        "each": [0, 2],
+        "earliest_planned_start": [1, 2],
+        "easi": 0,
+        "edited_fil": 0,
+        "eg": 2,
+        "either": [0, 2],
+        "element": 2,
+        "els": [0, 2],
+        "email": [1, 2],
+        "empti": [0, 1, 2],
+        "enabl": [0, 2],
+        "end": 2,
+        "engin": 2,
+        "ensur": 0,
+        "entiti": 0,
+        "enum": [0, 2],
+        "enum_custom_field_typ": [0, 1],
+        "enum_id": [1, 2],
+        "enum_opt": [0, 1],
+        "enum_option_id": [0, 1],
+        "enumcustomfieldtyp": [0, 1, 2],
+        "enumer": [0, 2],
+        "enumopt": [0, 1, 2],
+        "enumoptionid": [0, 1, 2],
+        "envelop": 2,
+        "environ": [0, 2],
+        "epel8": 0,
+        "epel9": 0,
+        "error": [0, 2],
+        "error_count": [1, 2],
+        "estimation_field": [1, 2],
+        "etc": [0, 2],
+        "even": 2,
+        "everyth": 2,
+        "ex": 0,
+        "exactli": 0,
+        "exampl": 2,
+        "except": [0, 1],
+        "execut": [0, 2],
+        "executed_bi": [0, 2],
+        "exist": 2,
+        "expect": 0,
+        "expectedresult": 0,
+        "expiration_d": [1, 2],
+        "export": 2,
+        "export_pdf": [1, 2],
+        "exportdocumenttopdf": 2,
+        "exportpdfproperti": 2,
+        "externally_linked_work_item": [0, 1],
+        "externallylinkedworkitem": [0, 1, 2],
+        "factori": 0,
+        "fail": [0, 2],
+        "failur": [0, 2],
+        "failure_count": [1, 2],
+        "fals": [2, 3],
+        "fashion": 0,
+        "fdel": 2,
+        "fget": 2,
+        "field": [0, 2],
+        "field_diff": [0, 1],
+        "field_nam": [1, 2],
+        "fielddiff": [0, 1, 2],
+        "fields_to_copy_from_test_case_to_defect": [1, 2],
+        "fields_to_copy_from_test_run_to_linked_defect": [1, 2],
+        "fields_to_copy_from_test_run_to_new_defect": [1, 2],
+        "file": [0, 2],
+        "file_nam": [1, 2],
+        "filenam": 2,
+        "fill": [0, 2],
+        "filter": [1, 2],
+        "find": [0, 2],
+        "finish": [1, 2],
+        "finish_tim": [1, 2],
+        "finished_on": [1, 2],
+        "fit": 2,
+        "fittopagewidth": 2,
+        "fix": 0,
+        "float": [1, 2],
+        "flow": 2,
+        "follow": [0, 2],
+        "footer": 2,
+        "format": 2,
+        "formatt": 0,
+        "found": 2,
+        "free": 0,
+        "friendli": 2,
+        "from": 2,
+        "fset": 2,
+        "func": 2,
+        "function": [0, 2],
+        "futur": 0,
+        "g": 2,
+        "gcc": 0,
+        "gener": [0, 2],
+        "generatebookmark": 2,
+        "generated_bi": [1, 2],
+        "get": [0, 2],
+        "get_attach": [1, 2],
+        "get_categori": [1, 2],
+        "get_contained_group": [1, 2],
+        "get_contained_project": [1, 2],
+        "get_context_rol": [1, 2],
+        "get_custom_field": [0, 1, 2],
+        "get_deep_contained_project": [1, 2],
+        "get_defined_custom_field_kei": [1, 2],
+        "get_defined_custom_field_typ": [1, 2],
+        "get_docu": [0, 1, 2],
+        "get_document_spac": [1, 2],
+        "get_global_rol": [1, 2],
+        "get_loc": [1, 2],
+        "get_project_us": [1, 2],
+        "get_revis": [1, 2],
+        "get_revision_by_uri": [1, 2],
+        "get_rol": [1, 2],
+        "get_root_project_group": [1, 2],
+        "get_statist": [1, 2],
+        "get_test_step": 0,
+        "get_test_steps_configur": [1, 2],
+        "get_tests_configur": [1, 2],
+        "get_us": [1, 2],
+        "get_user_avatar_url": [1, 2],
+        "get_user_from_token": [1, 2],
+        "get_valid_field_valu": [0, 1, 2],
+        "get_wiki_cont": [1, 2],
+        "get_wiki_pag": [1, 2],
+        "get_wiki_spac": [1, 2],
+        "get_work_item": [1, 2],
+        "getcategori": 2,
+        "getcontainedgroup": 2,
+        "getcontainedproject": 2,
+        "getcontextrol": 2,
+        "getcontextrolesforus": 2,
+        "getdeepcontainedproject": 2,
+        "getdefinedcustomfieldkei": 2,
+        "getdefinedcustomfieldtyp": 2,
+        "getdefinedtestruncustomfieldtyp": 2,
+        "getdocumentspac": 2,
+        "getenumoptionsforid": 2,
+        "getglobalrol": 2,
+        "getlocationforuri": 2,
+        "getmodul": 2,
+        "getmodulebyloc": 2,
+        "getmodulebylocationwithfield": 2,
+        "getmodulebyuri": 2,
+        "getmodulebyuriwithfield": 2,
+        "getmoduleswithfield": 2,
+        "getmoduleworkitem": 2,
+        "getplanbyid": 2,
+        "getplanbyuri": 2,
+        "getplanstatist": 2,
+        "getplanwikicont": 2,
+        "getproject": 2,
+        "getprojectatloc": 2,
+        "getprojectbyuri": 2,
+        "getprojectgroup": 2,
+        "getprojectgroupatloc": 2,
+        "getprojectus": 2,
+        "getrolesforus": 2,
+        "getrootprojectgroup": 2,
+        "getter": 2,
+        "gettestrunattach": 2,
+        "gettestrunbyid": 2,
+        "gettestrunbyuri": 2,
+        "gettestsconfigur": 2,
+        "getteststepsconfigur": 2,
+        "getus": 2,
+        "getuseravatarurl": 2,
+        "getuserbyuri": 2,
+        "getuserfromtoken": 2,
+        "getwikicontentfortestrun": 2,
+        "getwikipagebyuri": 2,
+        "getwikipagebyuriwithfield": 2,
+        "getwikispac": 2,
+        "git": 0,
+        "github": 0,
+        "give": [0, 2],
+        "given": [0, 2],
+        "global": [0, 2],
+        "global_config": [1, 2],
+        "global_id": [1, 2],
+        "grant": 2,
+        "group": 2,
+        "group_id": [1, 2],
+        "group_uri": [1, 2],
+        "gui": 0,
+        "ha": 2,
+        "handl": 2,
+        "has_current_user_permiss": [1, 2],
+        "has_permiss": [1, 2],
+        "hascurrentuserpermiss": 2,
+        "haspermiss": 2,
+        "hat": 0,
+        "have": [0, 2],
+        "head": [0, 2],
+        "header": 2,
+        "help": [0, 2],
+        "hidden": [1, 2],
+        "hierarchi": 2,
+        "high": 0,
+        "higher": 2,
+        "home": [0, 2],
+        "home_page_cont": [1, 2],
+        "host": 0,
+        "how": 2,
+        "html": 2,
+        "http": [0, 2],
+        "hyperlink": [0, 1],
+        "i": [0, 2],
+        "i386": 0,
+        "id": [1, 2],
+        "ideal_progress": [1, 2],
+        "ideal_progress_as_str": [1, 2],
+        "identifi": 2,
+        "ignor": 2,
+        "implement": 0,
+        "import": 0,
+        "imported_com": [0, 1],
+        "importedcom": [0, 1, 2],
+        "incid": 2,
+        "incidentreport": [0, 1, 2],
+        "includ": [0, 2],
+        "includeheaderfoot": 2,
+        "index": [0, 2],
+        "indic": 2,
+        "info": [1, 2],
+        "inform": 0,
+        "inherit": [0, 2],
+        "initi": [1, 2],
+        "inprogress": [0, 2],
+        "insert": 2,
+        "insid": 2,
+        "inspect": 2,
+        "install_requir": 0,
+        "instanti": 2,
+        "instead": 2,
+        "int": 2,
+        "interchang": 2,
+        "internal_commit": [1, 2],
+        "invalid": [1, 2],
+        "ip_address": [1, 2],
+        "is_sql": 2,
+        "is_templ": [1, 2, 3],
+        "item": [0, 1, 2],
+        "its": 2,
+        "itself": 0,
+        "java": 2,
+        "job_id": [1, 2],
+        "keep": 2,
+        "keep_in_histori": [1, 2],
+        "kei": [0, 1, 2],
+        "keyword": 2,
+        "know": 0,
+        "kwarg": 2,
+        "l": 2,
+        "label": [1, 2],
+        "landscap": 2,
+        "lang": 2,
+        "language_definit": [0, 1],
+        "language_definition_id": [1, 2],
+        "languagedefinit": [0, 1, 2],
+        "last": 2,
+        "latest": 0,
+        "lead": [1, 2],
+        "least": 0,
+        "legal": 2,
+        "length": [1, 2],
+        "let": 0,
+        "letter": 2,
+        "lib": 2,
+        "libdir": [0, 2],
+        "librari": [0, 2],
+        "licens": [0, 1, 2],
+        "license_format": [1, 2],
+        "license_info": [0, 1],
+        "license_profil": [1, 2],
+        "licenseinfo": [0, 1, 2],
+        "like": 0,
+        "limit": 2,
+        "link": [0, 2],
+        "linked_page_uri": [1, 2],
+        "linked_work_item": [0, 1],
+        "linked_work_item_uri": [1, 2],
+        "linked_work_items_deriv": 0,
+        "linkedworkitem": [0, 1, 2],
+        "linux2": 0,
+        "list": [0, 2, 3],
+        "list_documents_by_queri": [2, 3],
+        "list_workitems_by_queri": [2, 3],
+        "list_workitems_in_doc": [2, 3],
+        "listenfilt": [0, 1, 2],
+        "load": [0, 2],
+        "local": [0, 2],
+        "local_config": [1, 2],
+        "local_deployment_space_nam": [1, 2],
+        "locat": [0, 1, 2],
+        "lock_work_records_d": [1, 2],
+        "log": 2,
+        "log_fil": [1, 2],
+        "logged_in_user_id": [1, 2],
+        "login": [0, 2],
+        "long": 2,
+        "low": 0,
+        "lucen": 2,
+        "mac_address": [1, 2],
+        "made": 0,
+        "mai": [0, 2],
+        "make": 0,
+        "manag": [0, 2, 3],
+        "mani": 2,
+        "manual": 2,
+        "manual_select": 2,
+        "manual_state_chang": 2,
+        "map": [0, 2],
+        "mark": 2,
+        "markup": 2,
+        "marshal": [1, 2],
+        "match": 0,
+        "matter": 2,
+        "max_created_defect": [1, 2],
+        "max_created_defects_perc": [1, 2],
+        "maximum": 2,
+        "me": 0,
+        "mean": 2,
+        "medium": 0,
+        "mention": 0,
+        "messag": [1, 2],
+        "messagecontext": 2,
+        "messageplugin": 2,
+        "method": 2,
+        "middl": 2,
+        "mnliz9ju": 2,
+        "modifi": [0, 2],
+        "modul": [0, 1],
+        "module_absolute_loc": [1, 2],
+        "module_com": [0, 1],
+        "module_comment_id": [1, 2],
+        "module_fold": [1, 2],
+        "module_loc": [1, 2],
+        "module_nam": [1, 2],
+        "modulecom": [0, 1, 2],
+        "modulefold": 2,
+        "more": 0,
+        "mostli": 2,
+        "move": 2,
+        "move_work_item_her": [1, 2],
+        "moveworkitemtodocu": 2,
+        "multipl": 2,
+        "must": [0, 2],
+        "my": 0,
+        "mylist": 2,
+        "myproj": 0,
+        "name": [0, 1, 2],
+        "named_license_data": [1, 2],
+        "nativ": 0,
+        "native_action_id": [1, 2],
+        "natur": 0,
+        "need": [0, 2],
+        "neg": 2,
+        "nest": 2,
+        "network": 0,
+        "new": [0, 2],
+        "new_wi": 0,
+        "newclass": [0, 1, 2],
+        "next": 0,
+        "nil": 2,
+        "none": [0, 2, 3],
+        "nonzero": 2,
+        "notautom": 0,
+        "note": [0, 2],
+        "notrun": 2,
+        "nov": 0,
+        "now": 0,
+        "null": 2,
+        "number": [0, 2],
+        "number_of_plan": [1, 2],
+        "number_of_resolv": [1, 2],
+        "number_of_unresolv": [1, 2],
+        "obj": 2,
+        "obj_id": 2,
+        "object": [0, 2, 3],
+        "objectnam": 2,
+        "old": 2,
+        "onc": [0, 2],
+        "one": 2,
+        "ones": 2,
+        "onli": [0, 2],
+        "open": 0,
+        "opportun": 2,
+        "option": [0, 2],
+        "order": [0, 2],
+        "org": 0,
+        "orient": [0, 2],
+        "original_filenam": 2,
+        "other": 2,
+        "out": 0,
+        "output": 2,
+        "output_dir": 2,
+        "output_nam": 2,
+        "overcom": 0,
+        "overridden": [0, 2],
+        "overwrit": 2,
+        "overwritten": 0,
+        "p": 2,
+        "packag": 1,
+        "page": [0, 2],
+        "page_loc": [1, 2],
+        "page_nam": [1, 2],
+        "papers": 2,
+        "paradigm": 0,
+        "param": 2,
+        "paramet": 2,
+        "parent": [1, 2, 3],
+        "parent_comment_uri": [1, 2],
+        "parent_id": 2,
+        "parent_item_uri": [1, 2],
+        "parent_template_id": [0, 2],
+        "parent_uri": [1, 2],
+        "parent_work_item_id": 2,
+        "parm": 2,
+        "parti": 0,
+        "particular": 2,
+        "pass": [0, 2],
+        "password": [0, 2],
+        "path": [0, 2],
+        "pdf": 2,
+        "pep8": 0,
+        "per": [0, 2],
+        "permiss": 2,
+        "persist": 2,
+        "person": 0,
+        "phantom": [1, 2],
+        "pip": 0,
+        "pkgdir": [1, 2],
+        "place": 0,
+        "plan": [0, 1],
+        "plan_id": [1, 2],
+        "plan_nam": 2,
+        "plan_record": [0, 1],
+        "plan_statist": [0, 1],
+        "planned_as_str": [1, 2],
+        "plannedin": 3,
+        "planning_constraint": [0, 1],
+        "planningconstraint": [0, 1, 2],
+        "planrecord": [0, 1, 2],
+        "planstatist": [0, 1, 2],
+        "plugin": 2,
+        "polarion": [0, 2],
+        "polarion_cert_path": 0,
+        "polarion_password": [0, 2],
+        "polarion_project": [0, 2],
+        "polarion_repo": [0, 2],
+        "polarion_timeout": [0, 2],
+        "polarion_token": [0, 2],
+        "polarion_url": [0, 2],
+        "polarion_usernam": [0, 2],
+        "polarionproject": 2,
+        "polici": 2,
+        "popul": 2,
+        "portrait": 2,
+        "posit": [0, 2],
+        "possibl": [0, 2],
+        "pre": 0,
+        "prefix": [1, 2],
+        "previous_time_sp": [1, 2],
+        "print": 0,
+        "print_docu": [2, 3],
+        "print_links_for_requir": [2, 3],
+        "print_links_for_testcas": [2, 3],
+        "print_plan_id": [2, 3],
+        "print_runs_by_queri": [2, 3],
+        "print_steps_for_testcas": [2, 3],
+        "print_templates_by_queri": [2, 3],
+        "print_testcases_from_run": [2, 3],
+        "print_workitem": [2, 3],
+        "prioriti": 2,
+        "prioritization_field": [1, 2],
+        "priority_opt": [0, 1],
+        "priority_opt_id": [1, 2],
+        "priority_option_id": [0, 1],
+        "priorityopt": [0, 1, 2],
+        "priorityoptionid": [0, 1, 2],
+        "proce": 0,
+        "process": 0,
+        "product_licens": [0, 1],
+        "productlicens": [0, 1, 2],
+        "progress": [1, 2],
+        "progress_as_str": [1, 2],
+        "prohibit": 2,
+        "proj": 0,
+        "project": [0, 1],
+        "project_group": [0, 1],
+        "project_id": [0, 1, 2],
+        "project_nam": 0,
+        "project_uri": [1, 2],
+        "projectgroup": [0, 1, 2],
+        "prompt": 0,
+        "properti": [0, 1],
+        "propos": 0,
+        "provid": [0, 2],
+        "publish": [0, 2],
+        "push": 0,
+        "put": 2,
+        "py": 0,
+        "pylerolibexcept": [0, 1, 2],
+        "python": [0, 2],
+        "python3": [0, 2],
+        "python_vers": 0,
+        "qo": 0,
+        "queri": [0, 1, 2, 3],
+        "query_uri": 2,
+        "querybaselin": 2,
+        "querymodul": 2,
+        "querymodulesbysql": 2,
+        "querymodulesinbaselin": 2,
+        "querymodulesinbaselinebysql": 2,
+        "querymoduleuri": 2,
+        "querymoduleurisbysql": 2,
+        "querymoduleurisinbaselin": 2,
+        "querymoduleurisinbaselinebysql": 2,
+        "queryrevis": 2,
+        "querywikipag": 2,
+        "querywikipagesbysql": 2,
+        "querywikipagesinbaselin": 2,
+        "querywikipagesinbaselinebysql": 2,
+        "querywikipageuri": 2,
+        "querywikipageurisbysql": 2,
+        "querywikipageurisinbaselin": 2,
+        "querywikipageurisinbaselinebysql": 2,
+        "r": 0,
+        "r266": 0,
+        "rais": [0, 2],
+        "reach": 0,
+        "read": 2,
+        "readlin": 0,
+        "rec": 0,
+        "recommend": 0,
+        "record": [0, 1, 2],
+        "record_index": 2,
+        "red": 0,
+        "redhat": 2,
+        "redhatq": 0,
+        "refer": [0, 2],
+        "referenc": 2,
+        "referred_work_item_uri": [1, 2],
+        "regex_id": [1, 2],
+        "regex_proj": [1, 2],
+        "regular": 0,
+        "rel": 2,
+        "relat": 2,
+        "relationship": 2,
+        "releas": 0,
+        "reload": [1, 2],
+        "relogin_timeout": 2,
+        "remot": 2,
+        "remov": [1, 2],
+        "remove_plan_item": [1, 2],
+        "removeplanitem": 2,
+        "repo": [1, 2],
+        "report": 2,
+        "repositori": [0, 2],
+        "repository_nam": [1, 2],
+        "repres": 2,
+        "req": 0,
+        "req_id": 3,
+        "reqtyp": 0,
+        "request": [0, 2],
+        "requir": [1, 2],
+        "required_featur": [1, 2],
+        "res1": 0,
+        "res2": 0,
+        "resolv": [0, 1, 2],
+        "resource_loc": [1, 2],
+        "result": [0, 1, 2, 3],
+        "result_error_enum_id": [1, 2],
+        "result_failed_enum_id": [1, 2],
+        "result_passed_enum_id": [1, 2],
+        "retain": 2,
+        "retain_flow": 2,
+        "retest_allow": [1, 2],
+        "retri": [1, 2],
+        "retriev": 2,
+        "return": [0, 2],
+        "rev": 2,
+        "revis": [0, 1],
+        "revision_id": 2,
+        "revision_uri": 2,
+        "rhel": 0,
+        "rich": 2,
+        "risk": [0, 1, 2],
+        "role": [0, 1, 2],
+        "root": [0, 2],
+        "router": 2,
+        "rpmbuild": 0,
+        "run": [0, 2, 3],
+        "same": [0, 2],
+        "save": 0,
+        "script": 0,
+        "search": [0, 1, 2],
+        "search_templ": 2,
+        "searchplan": 2,
+        "searchplanswithfield": 2,
+        "searchplantempl": 2,
+        "searchplantemplateswithfield": 2,
+        "searchtestrun": 2,
+        "searchtestrunlimit": 2,
+        "searchtestrunswithfield": 2,
+        "searchtestrunswithfieldslimit": 2,
+        "searchtestruntempl": 2,
+        "searchtestruntemplateslimit": 2,
+        "searchtestruntemplateswithfield": 2,
+        "searchtestruntemplateswithfieldslimit": 2,
+        "section": 0,
+        "secur": 2,
+        "see": [0, 2],
+        "select": 2,
+        "select_test_cases_bi": [0, 1, 2],
+        "send": 2,
+        "sent": [0, 2],
+        "sequence_numb": [1, 2],
+        "server": [0, 1],
+        "servic": 2,
+        "session": [0, 1],
+        "set": [0, 2],
+        "set_custom_field": 0,
+        "set_wiki_cont": [1, 2],
+        "setplanwikicont": 2,
+        "setter": 2,
+        "setup": 0,
+        "share": [0, 2],
+        "shell": 0,
+        "should": [0, 2],
+        "signatur": [0, 1],
+        "signature_context": [0, 1],
+        "signature_data": [0, 1],
+        "signaturecontext": [0, 1, 2],
+        "signaturedata": [0, 1, 2],
+        "signed_bi": [1, 2],
+        "signed_revis": [1, 2],
+        "signer_rol": [1, 2],
+        "site": 2,
+        "size": 2,
+        "skipped_count": [1, 2],
+        "slot": [1, 2],
+        "smoothli": 0,
+        "so": [0, 2],
+        "soap": [0, 2],
+        "soapnul": [0, 1, 2],
+        "sort": 2,
+        "sort_ord": [1, 2],
+        "sourc": [0, 2, 3],
+        "source_id": [1, 2],
+        "space": [0, 2, 3],
+        "space_id": [1, 2],
+        "spec": 0,
+        "specif": [0, 2],
+        "specifi": [0, 2],
+        "sql": 2,
+        "ssl": 2,
+        "standard": 0,
+        "start": [0, 1, 2],
+        "start_dat": [1, 2],
+        "start_tim": [1, 2],
+        "started_on": [1, 2],
+        "state": 2,
+        "static": 0,
+        "static_livedoc": 2,
+        "static_queri": 2,
+        "staticlivedoc": 0,
+        "staticqueryresult": 0,
+        "statist": 2,
+        "statu": [0, 1, 2, 3],
+        "status_error_enum_id": [1, 2],
+        "status_failed_enum_id": [1, 2],
+        "status_ok_enum_id": [1, 2],
+        "step": [0, 1, 2],
+        "step1": 0,
+        "step2": 0,
+        "store": 0,
+        "str": 2,
+        "string": 2,
+        "structur": [0, 2],
+        "structure_link_rol": [1, 2, 3],
+        "style": 2,
+        "submodul": [0, 1],
+        "subpackag": [0, 1],
+        "subset": 2,
+        "subterra": 2,
+        "subterra_uri": [0, 1],
+        "subterrauri": [0, 1, 2],
+        "subtre": 2,
+        "sud": [0, 2],
+        "suds_object": 2,
+        "suggested_featur": [1, 2],
+        "summari": 2,
+        "summary_defect": [1, 2],
+        "summary_defect_sever": [1, 2],
+        "suppos": 2,
+        "suspect": [1, 2],
+        "svn_repo": 0,
+        "sync": 0,
+        "syntax": 2,
+        "system": [0, 2],
+        "t": 0,
+        "tabloid": 2,
+        "tag": [0, 1, 2],
+        "take": 0,
+        "target": 0,
+        "target_statu": [1, 2],
+        "target_status_id": [1, 2],
+        "task": [0, 1, 2],
+        "tc": 0,
+        "tcmscaseid": 0,
+        "tcmscategori": 0,
+        "teardown": 0,
+        "templat": [0, 1, 2, 3],
+        "template_id": 2,
+        "template_nam": 2,
+        "template_uri": [1, 2],
+        "tescas": 0,
+        "test": [0, 2],
+        "test_case_id": [0, 2],
+        "test_case_id_custom_field": [1, 2],
+        "test_case_revis": 2,
+        "test_case_templ": [1, 2],
+        "test_case_test_comment_field_id": [1, 2],
+        "test_case_test_result_field_id": [1, 2],
+        "test_case_work_item_typ": [1, 2],
+        "test_com": [0, 2],
+        "test_count": [1, 2],
+        "test_manag": 2,
+        "test_record": [0, 1],
+        "test_result": [0, 2],
+        "test_run": [0, 1],
+        "test_run_attach": [0, 1],
+        "test_run_id": [1, 2],
+        "test_run_templ": [1, 2],
+        "test_run_uri": [1, 2],
+        "test_step": [0, 1],
+        "test_step_index": 2,
+        "test_step_result": [0, 1],
+        "testcas": [0, 1, 2, 3],
+        "testmanag": 2,
+        "testrecord": [0, 1, 2],
+        "testrun": [0, 1, 2],
+        "testrunattach": [0, 1, 2],
+        "tests_configur": [0, 1],
+        "testsconfigur": [0, 1, 2],
+        "testspecif": [0, 2],
+        "teststep": [0, 1, 2],
+        "teststepresult": [0, 1, 2],
+        "testsuit": [0, 1, 2],
+        "text": [0, 1],
+        "thei": 0,
+        "them": [0, 2],
+        "thi": [0, 2],
+        "third": 0,
+        "those": 0,
+        "tiemout": 2,
+        "time": [0, 1, 2],
+        "time_point": [0, 1],
+        "time_point_id": [1, 2],
+        "time_sp": [1, 2],
+        "time_stamp": [1, 2],
+        "timeout": 2,
+        "timepoint": [0, 1, 2],
+        "timestamp": [1, 2],
+        "titl": [0, 1, 2],
+        "tmp": 2,
+        "tns2": 2,
+        "tns3": 2,
+        "tns4": 2,
+        "tns5": 2,
+        "tns6": 2,
+        "tnsx": 2,
+        "todo": [1, 2],
+        "todo_as_str": [1, 2],
+        "token": [0, 2],
+        "token_en": [1, 2],
+        "tool": 0,
+        "total": 2,
+        "total_error": 2,
+        "total_failur": 2,
+        "total_test": 2,
+        "tp_12071": 0,
+        "tp_12071_1": 0,
+        "tpl_tp_12071": 0,
+        "tr": 0,
+        "tracker": 2,
+        "tracker_prefix": [1, 2],
+        "transact": 2,
+        "transition_data_revis": [1, 2],
+        "treat": 2,
+        "trigger": 0,
+        "true": 2,
+        "try": 2,
+        "tx_begin": [1, 2],
+        "tx_commit": [1, 2],
+        "tx_in": [1, 2],
+        "tx_releas": [1, 2],
+        "tx_rollback": [1, 2],
+        "tx_wrapper": [0, 1, 2],
+        "txt": 0,
+        "type": [0, 1, 2],
+        "u": [0, 2],
+        "unavailability_messag": [1, 2],
+        "under": 2,
+        "unexecut": 2,
+        "uniqu": 2,
+        "unknown": 2,
+        "unsav": 2,
+        "updat": [0, 1, 2, 3],
+        "update_1_case_result_for_run": [2, 3],
+        "update_all_case_results_for_run": [2, 3],
+        "update_attach": [1, 2],
+        "update_docu": [2, 3],
+        "update_run": [2, 3],
+        "update_summary_defect": [1, 2],
+        "update_test_record_by_field": [1, 2],
+        "update_test_record_by_object": [1, 2],
+        "update_wiki_cont": [1, 2],
+        "updated_bi": [1, 2],
+        "updatemodul": 2,
+        "updateplan": 2,
+        "updatesummarydefect": 2,
+        "updatetestrecord": 2,
+        "updatetestrecordatindex": 2,
+        "updatetestrun": 2,
+        "updatetestrunattach": 2,
+        "updateus": 2,
+        "updatewikicontentfortestrun": 2,
+        "upload": 2,
+        "upon": 2,
+        "uri": [0, 1, 2],
+        "uri_id_get_replac": [1, 2],
+        "uri_id_set_replac": [1, 2],
+        "uri_struct": [1, 2],
+        "url": [0, 1, 2],
+        "us": [0, 2],
+        "user": [0, 1, 3],
+        "user1": 0,
+        "user_id": [1, 2],
+        "usernam": [0, 2],
+        "uses_outline_numb": [1, 2],
+        "usual": 0,
+        "val": 2,
+        "valid": [0, 2],
+        "valu": [0, 1, 2],
+        "variabl": [0, 2],
+        "verdict": [1, 2],
+        "verdict_tim": [1, 2],
+        "verif": [0, 2],
+        "verifi": [0, 2],
+        "verify_param": [1, 2],
+        "verify_requir": [1, 2],
+        "version": 2,
+        "via": [0, 2],
+        "violat": 0,
+        "virtual": 0,
+        "virtualenv": 2,
+        "visible_to": [1, 2],
+        "vm": 0,
+        "vote_uri": [1, 2],
+        "w": 2,
+        "w_item": 2,
+        "wa": [0, 2],
+        "walk": 2,
+        "want": [0, 2],
+        "was_start": [1, 2],
+        "wasplanstart": 2,
+        "watche_uri": [1, 2],
+        "watermark": 2,
+        "wayn": 2,
+        "we": [0, 2],
+        "web": 0,
+        "webhook": 0,
+        "webservic": [0, 2],
+        "well": 2,
+        "went": 0,
+        "were": 2,
+        "when": [0, 2],
+        "where": [0, 2],
+        "which": [0, 2],
+        "whole": 2,
+        "wi": [0, 2],
+        "wi_typ": 3,
+        "width": 2,
+        "wiki": 2,
+        "wiki_pag": [0, 1],
+        "wiki_page_attach": [0, 1],
+        "wiki_page_attachment_id": [1, 2],
+        "wiki_page_id": [1, 2],
+        "wikipag": [0, 1, 2],
+        "wikipageattach": [0, 1, 2],
+        "within": 2,
+        "without": [0, 2],
+        "work": [0, 2],
+        "work_item": [0, 1],
+        "work_item_id": [0, 1, 2],
+        "work_item_type_id": 2,
+        "work_item_uri": [1, 2],
+        "work_record": [0, 1],
+        "work_record_id": [1, 2],
+        "workflow": 0,
+        "workflow_act": [0, 1],
+        "workflowact": [0, 1, 2],
+        "workitem": [0, 2, 3],
+        "workrecord": [0, 1, 2],
+        "wrapper": 0,
+        "wsdl": [0, 2],
+        "x": 2,
+        "xsi": 2,
+        "ye": 2,
+        "yet": 2,
+        "you": 2,
+        "your": 0,
+        "yum": 0
+    },
+    "titles": ["Welcome to pylero\u2019s documentation!", "pylero", "pylero package", "pylero.cli package"],
+    "titleterms": {
+        "": 0,
+        "activ": 2,
+        "activity_com": 2,
+        "activity_custom_valu": 2,
+        "activity_custom_value_entri": 2,
+        "activity_sourc": 2,
+        "approv": 2,
+        "attach": 2,
+        "base_polarion": 2,
+        "baselin": 2,
+        "befor": 0,
+        "build": [0, 2],
+        "build_linked_work_item": 2,
+        "build_test_result": 2,
+        "categori": 2,
+        "chang": 2,
+        "cli": 3,
+        "cmd": 3,
+        "comment": 2,
+        "commit": 0,
+        "configur": 0,
+        "content": [2, 3],
+        "copr": 0,
+        "custom": 2,
+        "custom_field": 2,
+        "custom_field_typ": 2,
+        "document": [0, 2],
+        "enum_custom_field_typ": 2,
+        "enum_opt": 2,
+        "enum_option_id": 2,
+        "epel": 0,
+        "exampl": 0,
+        "except": 2,
+        "externally_linked_work_item": 2,
+        "fedora": 0,
+        "field_diff": 2,
+        "from": 0,
+        "hyperlink": 2,
+        "imported_com": 2,
+        "indic": 0,
+        "instal": 0,
+        "language_definit": 2,
+        "license_info": 2,
+        "linked_work_item": 2,
+        "modul": [2, 3],
+        "module_com": 2,
+        "packag": [0, 2, 3],
+        "plan": 2,
+        "plan_record": 2,
+        "plan_statist": 2,
+        "planning_constraint": 2,
+        "priority_opt": 2,
+        "priority_option_id": 2,
+        "product_licens": 2,
+        "project": 2,
+        "project_group": 2,
+        "properti": 2,
+        "pylero": [0, 1, 2, 3],
+        "pypi": 0,
+        "repo": 0,
+        "requir": 0,
+        "revis": 2,
+        "rpm": 0,
+        "server": 2,
+        "session": 2,
+        "signatur": 2,
+        "signature_context": 2,
+        "signature_data": 2,
+        "submodul": [2, 3],
+        "subpackag": 2,
+        "subterra_uri": 2,
+        "tabl": 0,
+        "test_record": 2,
+        "test_run": 2,
+        "test_run_attach": 2,
+        "test_step": 2,
+        "test_step_result": 2,
+        "tests_configur": 2,
+        "text": 2,
+        "time_point": 2,
+        "tito": 0,
+        "usag": 0,
+        "user": 2,
+        "welcom": 0,
+        "wiki_pag": 2,
+        "wiki_page_attach": 2,
+        "work_item": 2,
+        "work_record": 2,
+        "workflow_act": 2,
+        "you": 0
     }
 })
```

### Comparing `pylero-0.0.9/gen_docs.sh` & `pylero-0.1.0/gen_docs.sh`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/pylero.egg-info/PKG-INFO` & `pylero-0.1.0/pylero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylero
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python SDK for Polarion
 Home-page: https://github.com/RedHatQE/pylero
 Author: pylero Developers
 Author-email: dno-tools@redhat.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pylero-0.0.9/pylero.egg-info/SOURCES.txt` & `pylero-0.1.0/pylero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/python-pylero.spec` & `pylero-0.1.0/python-pylero.spec`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:           python-pylero
-Version:        0.0.9
+Version:        0.1.0
 Release:        1%{?dist}
 Summary:        Python SDK for Polarion
 
 License:        MIT
 URL:            https://github.com/RedHatQE/pylero
 Source:         %{url}/archive/%{version}/pylero-%{version}.tar.gz
 
@@ -78,14 +78,31 @@
 %files -n python3-pylero -f %{pyproject_files}
 %doc README.md
 %{_bindir}/pylero
 %{_bindir}/pylero-cmd
 
 
 %changelog
+* Mon May 20 2024 Wayne Sun <gsun@redhat.com> 0.1.0-1
+- feat: add flag for incident creation (konstantin.althaus.ext@vaillant-
+  group.com)
+- refactor: safely import test case workitem type
+  (konstantin.althaus.ext@vaillant-group.com)
+- fix: catch exceptions, avoid empty tables (konstantin.althaus.ext@vaillant-
+  group.com)
+- refactor: auxiliary functions become methods
+  (konstantin.althaus.ext@vaillant-group.com)
+- feat: add dummy TestCase class (konstantin.althaus.ext@vaillant-group.com)
+- fix: add project_id to _WorkItem (konstantin.althaus.ext@vaillant-group.com)
+- Adding methods that get document revision/s (emesika@redhat.com)
+- fix: erase title only for subcomments
+  (45875998+AlthausKonstantin@users.noreply.github.com)
+- Feat/link external workitmes (#176)
+  (45875998+AlthausKonstantin@users.noreply.github.com)
+
 * Tue Mar 05 2024 Wayne Sun <gsun@redhat.com>
 - Remove Python 3.6 and add 3.12
 - Bug fix and doc update
 
 * Tue Mar 14 2023 Wayne Sun <gsun@redhat.com> 0.0.8-1
 - Add token config support
```

### Comparing `pylero-0.0.9/scripts/pylero` & `pylero-0.1.0/scripts/pylero`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/scripts/pylero-cmd` & `pylero-0.1.0/scripts/pylero-cmd`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/setup.py` & `pylero-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 RELEASE_FILE = "/etc/system-release-cpe"
 
 install_requires_ = ["click", "suds"]
 
 if __name__ == "__main__":
     setup(
         name=PACKAGE_NAME,
-        version="0.0.9",
+        version="0.1.0",
         description="Python SDK for Polarion",
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         url="https://github.com/RedHatQE/pylero",
         author="%s Developers" % PACKAGE_NAME,
         author_email="dno-tools@redhat.com",
         license="MIT",
```

### Comparing `pylero-0.0.9/src/pylero/_compatible.py` & `pylero-0.1.0/src/pylero/_compatible.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/activity.py` & `pylero-0.1.0/src/pylero/activity.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/activity_comment.py` & `pylero-0.1.0/src/pylero/activity_comment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/activity_custom_value.py` & `pylero-0.1.0/src/pylero/activity_custom_value.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/activity_custom_value_entry.py` & `pylero-0.1.0/src/pylero/activity_custom_value_entry.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/activity_source.py` & `pylero-0.1.0/src/pylero/activity_source.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/approval.py` & `pylero-0.1.0/src/pylero/approval.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/attachment.py` & `pylero-0.1.0/src/pylero/attachment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/base_polarion.py` & `pylero-0.1.0/src/pylero/base_polarion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1073,7 +1073,41 @@
         Returns:
             None
         """
 
         if getattr(self, "uri", None):
             obj = self.__class__(uri=self.uri)
             self._suds_object = obj._suds_object
+
+    def get_revision(self, repository_name, revision_id):
+        """
+        Gets a revision
+        Args:
+            repository_name - The repository name. (Put "default" for the default repository.)
+            revision_id - The revision name.
+        Returns:
+            a Revision object
+        """
+        return self.session.tracker_client.service.getrevision(
+            repository_name, revision_id
+        )
+
+    def get_revision_by_uri(self, revision_uri):
+        """
+        Gets a revision by its URI
+        Args:
+             revision_uri - The URI of the revision.
+        Returns:
+            a Revision object
+
+        """
+        return self.session.tracker_client.service.getRevisionByUri(revision_uri)
+
+    def get_revisions(self, uri):
+        """
+        Returns all revisions for a specific URI.
+        Args:
+             uri - URI of the persistence object (Work Item, Module/Document, User, etc).
+        Returns:
+            All revisions for a specific URI.
+        """
+        return self.session.tracker_client.service.getRevisions(uri)
```

### Comparing `pylero-0.0.9/src/pylero/baseline.py` & `pylero-0.1.0/src/pylero/baseline.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/build.py` & `pylero-0.1.0/src/pylero/build.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/build_linked_work_item.py` & `pylero-0.1.0/src/pylero/build_linked_work_item.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/build_test_results.py` & `pylero-0.1.0/src/pylero/build_test_results.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/category.py` & `pylero-0.1.0/src/pylero/category.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/change.py` & `pylero-0.1.0/src/pylero/change.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/cli/cmd.py` & `pylero-0.1.0/src/pylero/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/comment.py` & `pylero-0.1.0/src/pylero/comment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/custom.py` & `pylero-0.1.0/src/pylero/custom.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/custom_field.py` & `pylero-0.1.0/src/pylero/custom_field.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/custom_field_type.py` & `pylero-0.1.0/src/pylero/custom_field_type.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/document.py` & `pylero-0.1.0/src/pylero/document.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/enum_custom_field_type.py` & `pylero-0.1.0/src/pylero/enum_custom_field_type.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/enum_option.py` & `pylero-0.1.0/src/pylero/enum_option.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/enum_option_id.py` & `pylero-0.1.0/src/pylero/enum_option_id.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/externally_linked_work_item.py` & `pylero-0.1.0/src/pylero/externally_linked_work_item.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/field_diff.py` & `pylero-0.1.0/src/pylero/field_diff.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/hyperlink.py` & `pylero-0.1.0/src/pylero/hyperlink.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/imported_comment.py` & `pylero-0.1.0/src/pylero/imported_comment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/language_definition.py` & `pylero-0.1.0/src/pylero/language_definition.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/license_info.py` & `pylero-0.1.0/src/pylero/license_info.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/linked_work_item.py` & `pylero-0.1.0/src/pylero/linked_work_item.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/module_comment.py` & `pylero-0.1.0/src/pylero/module_comment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/plan.py` & `pylero-0.1.0/src/pylero/plan.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/plan_record.py` & `pylero-0.1.0/src/pylero/plan_record.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/plan_statistics.py` & `pylero-0.1.0/src/pylero/plan_statistics.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/planning_constraint.py` & `pylero-0.1.0/src/pylero/planning_constraint.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/priority_opt.py` & `pylero-0.1.0/src/pylero/priority_opt.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/priority_option_id.py` & `pylero-0.1.0/src/pylero/priority_option_id.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/product_license.py` & `pylero-0.1.0/src/pylero/product_license.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/project.py` & `pylero-0.1.0/src/pylero/project.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/project_group.py` & `pylero-0.1.0/src/pylero/project_group.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/properties.py` & `pylero-0.1.0/src/pylero/properties.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/property.py` & `pylero-0.1.0/src/pylero/property.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/revision.py` & `pylero-0.1.0/src/pylero/revision.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/server.py` & `pylero-0.1.0/src/pylero/server.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/session.py` & `pylero-0.1.0/src/pylero/session.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/signature.py` & `pylero-0.1.0/src/pylero/signature.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/signature_context.py` & `pylero-0.1.0/src/pylero/signature_context.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/signature_data.py` & `pylero-0.1.0/src/pylero/signature_data.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/test_record.py` & `pylero-0.1.0/src/pylero/test_record.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/test_run.py` & `pylero-0.1.0/src/pylero/test_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf8 -*-
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
+import importlib
 import os
 
 import suds
 from pylero._compatible import basestring
 from pylero._compatible import classmethod
 from pylero._compatible import object  # noqa
 from pylero._compatible import range
@@ -28,145 +29,19 @@
 from pylero.test_record import TestRecord
 from pylero.test_run_attachment import ArrayOfTestRunAttachment
 from pylero.test_run_attachment import TestRunAttachment
 from pylero.text import Text
 from pylero.user import User
 from pylero.work_item import _WorkItem
 
-try:
-    from pylero.work_item import TestCase
-except ImportError:
-    pass
 
 # Build is used in custom fields.
 # Plan is used in custom fields.
 
 
-def generate_description(test_run, test_case, test_record):
-    tr_html = (
-        '<b>Test Run:</b> <span id="link" class=    '
-        '"polarion-rte-link" data-type="testRun" '
-        'data-item-id="{0}" data-option-id="long">'
-        "</span><br/>".format(test_run.test_run_id)
-    )
-    tc_html = (
-        '<b>Test Case:</b> <span id="link" class='
-        '"polarion-rte-link" data-type="workItem" '
-        'data-item-id="{0}" data-option-id="long"></span>'
-        "<br/>".format(test_case.work_item_id)
-    )
-    table_cell_style = (
-        'style="text-align: left; padding: 10px; '
-        'vertical-align: top; background-color: #ffffff;"'
-    )
-    table_row_style = 'style="border-bottom: 1px solid #f0f0f0;"'
-    columns = [
-        "",
-        "#",
-        '<span title="Step">Step</span>',
-        '<span title="Expected Result">Expected Result</span>',
-        "Actual Result",
-    ]
-    test_step_results = {
-        "passed": '<span title="Results met expected results'
-        '"><span style="white-space:nowrap;"><im'
-        'g src="/polarion/icons/default/enums/test'
-        'run_status_passed.png" style="vertical-a'
-        "lign:text-bottom;border:0px;margin-right:2"
-        'px;" class="polarion-no-style-cleanup"/'
-        "></span></span>",
-        "failed": '<span title="Results did not meet expecte'
-        'd results"><span style="white-space:nowr'
-        'ap;"><img src="/polarion/icons/default/e'
-        'nums/testrun_status_failed.png" style="v'
-        "ertical-align:text-bottom;border:0px;margi"
-        'n-right:2px;" class="polarion-no-style-c'
-        'leanup"/></span></span>',
-        "blocked": '<span title="Errors in the product preve'
-        'nted test from being executed"><span sty'
-        'le="white-space:nowrap;"><img src="/po'
-        "larion/icons/default/enums/testrun_status"
-        '_blocked.png" style="vertical-align:tex'
-        't-bottom;border:0px;margin-right:2px;" c'
-        'lass="polarion-no-style-cleanup"/>'
-        "</span></span>",
-    }
-    table_header = (
-        '<table class="polarion-no-style-cleanup" style="border'
-        '-collapse: collapse;"><tr style="text-align: left; '
-        "white-space: nowrap; color: #757575; border-bottom: 1px "
-        'solid #d2d7da; background-color: #ffffff;">{0}</tr>'.format(
-            "".join(
-                [
-                    "<th {0}>{1}</th>".format(table_cell_style, column)
-                    for column in columns
-                ]
-            )
-        )
-    )
-    verdict = (
-        '</table><table style="margin-bottom: 15px; ;border-collapse: '
-        'collapse; width:100%; ;margin-top: 13px;" class="polarion-no'
-        '-style-cleanup"><tr><th style="width: 80%; text-align: left;'
-        ' background-color: #ffffff;">Test Case Verdict:</th></tr><tr>'
-        '<td style="vertical-align: top;"><span style="font-weight: '
-        'bold;"><span style="color: #C30000;"><span title="Results '
-        'did not meet expected results"><span style="white-space:'
-        'nowrap;"><img src="/polarion/icons/default/enums/testrun_'
-        'status_failed.png" style="vertical-align:text-bottom;border:'
-        '0px;margin-right:2px;" class="polarion-no-style-cleanup"/>'
-        "</span>Failed</span></span></span><span> {0}</span></td></tr>"
-        "</table>".format(test_record.comment)
-    )
-    table_rows = ""
-    for step in range(len(test_record.test_step_results)):
-        table_rows += (
-            "<tr {0}>"
-            "<td {1}>{2}</td>"
-            "<td {1}>{3}</td>"
-            "<td {1}>{4}</td>"
-            "<td {1}>{5}</td>"
-            "<td {1}>{6}</td>"
-            "</tr>".format(
-                table_row_style,
-                table_cell_style,
-                test_step_results.get(test_record.test_step_results[step].result),
-                step + 1,
-                test_case.test_steps.steps[step].values[0].content,
-                test_case.test_steps.steps[step].values[1].content,
-                test_record.test_step_results[step].comment,
-            )
-        )
-    content = tr_html + tc_html + table_header + table_rows + verdict
-
-    return content
-
-
-def create_incident_report(test_run, test_record, test_case):
-    project_id = test_run.project_id
-    status = "open"
-    project = Project(project_id)
-    tconf = project.get_tests_configuration()
-    defectWorkItemType = tconf.defect_work_item_type
-    title = "Failed: " + test_case.title
-    description = generate_description(test_run, test_case, test_record)
-    kwarg_dict = {}
-
-    for prop in tconf.fields_to_copy_from_test_case_to_defect.property:
-        kwarg_dict[prop.value] = getattr(test_case, prop.key)
-    for prop in tconf.fields_to_copy_from_test_run_to_linked_defect.property:
-        kwarg_dict[prop.value] = getattr(test_run, prop.key)
-
-    incident_report = _WorkItem.create(
-        project_id, defectWorkItemType, title, description, status, **kwarg_dict
-    )
-    incident_report.add_linked_item(test_case.work_item_id, "triggered_by")
-    return incident_report.work_item_id
-
-
 class TestRun(BasePolarion):
     """Object to manage the Polarion Test Management WS tns3:TestRun
 
     Attributes:
         attachments (list of TestRunAttachments)
         author (User): user object of the Test Run Author
         created (datetime)
@@ -373,15 +248,15 @@
         cls,
         project_id,
         template_id,
         parent_template_id="Empty",
         select_test_cases_by=None,
         query=None,
         doc_with_space=None,
-        **kwargs
+        **kwargs,
     ):  # , test_case_ids=[]):
         # see comment below regarding test_case)ids.
         """class method create_template for creating a new template in Polarion
 
         Args:
             project_id (string): the Polarion project to create the test run
                                  in
@@ -910,44 +785,246 @@
         testrec.executed_by = executed_by
         testrec.executed = executed
         testrec.duration = duration
         if defect_work_item_id:
             testrec.defect_case_id = defect_work_item_id
         self.add_test_record_by_object(testrec)
 
+    def __generate_description(
+        self, test_case: _WorkItem, test_record: TestRecord
+    ) -> str:
+        """Generates the description for the incident report.
+
+        If the test case has test steps that match the steps of the test record,
+        the description will include a table with the test steps and their results.
+
+        Args:
+            test_case (_WorkItem): Test case as a work item.
+            test_record (TestRecord): The test record contains the results of the
+                test execution.
+
+        Returns:
+            str: The incident report in HTML format.
+        """
+
+        tr_html = (
+            '<b>Test Run:</b> <span id="link" class=    '
+            '"polarion-rte-link" data-type="testRun" '
+            'data-item-id="{0}" data-option-id="long">'
+            "</span><br/>".format(self.test_run_id)
+        )
+        tc_html = (
+            '<b>Test Case:</b> <span id="link" class='
+            '"polarion-rte-link" data-type="workItem" '
+            'data-item-id="{0}" data-option-id="long"></span>'
+            "<br/>".format(test_case.work_item_id)
+        )
+        table_cell_style = (
+            'style="text-align: left; padding: 10px; '
+            'vertical-align: top; background-color: #ffffff;"'
+        )
+        table_row_style = 'style="border-bottom: 1px solid #f0f0f0;"'
+        columns = [
+            "",
+            "#",
+            '<span title="Step">Step</span>',
+            '<span title="Expected Result">Expected Result</span>',
+            "Actual Result",
+        ]
+        test_step_results = {
+            "passed": '<span title="Results met expected results'
+            '"><span style="white-space:nowrap;"><im'
+            'g src="/polarion/icons/default/enums/test'
+            'run_status_passed.png" style="vertical-a'
+            "lign:text-bottom;border:0px;margin-right:2"
+            'px;" class="polarion-no-style-cleanup"/'
+            "></span></span>",
+            "failed": '<span title="Results did not meet expecte'
+            'd results"><span style="white-space:nowr'
+            'ap;"><img src="/polarion/icons/default/e'
+            'nums/testrun_status_failed.png" style="v'
+            "ertical-align:text-bottom;border:0px;margi"
+            'n-right:2px;" class="polarion-no-style-c'
+            'leanup"/></span></span>',
+            "blocked": '<span title="Errors in the product preve'
+            'nted test from being executed"><span sty'
+            'le="white-space:nowrap;"><img src="/po'
+            "larion/icons/default/enums/testrun_status"
+            '_blocked.png" style="vertical-align:tex'
+            't-bottom;border:0px;margin-right:2px;" c'
+            'lass="polarion-no-style-cleanup"/>'
+            "</span></span>",
+        }
+        table_header = (
+            '<table class="polarion-no-style-cleanup" style="border'
+            '-collapse: collapse;"><tr style="text-align: left; '
+            "white-space: nowrap; color: #757575; border-bottom: 1px "
+            'solid #d2d7da; background-color: #ffffff;">{0}</tr>'.format(
+                "".join(
+                    [
+                        "<th {0}>{1}</th>".format(table_cell_style, column)
+                        for column in columns
+                    ]
+                )
+            )
+        )
+        verdict = (
+            '</table><table style="margin-bottom: 15px; ;border-collapse: '
+            'collapse; width:100%; ;margin-top: 13px;" class="polarion-no'
+            '-style-cleanup"><tr><th style="width: 80%; text-align: left;'
+            ' background-color: #ffffff;">Test Case Verdict:</th></tr><tr>'
+            '<td style="vertical-align: top;"><span style="font-weight: '
+            'bold;"><span style="color: #C30000;"><span title="Results '
+            'did not meet expected results"><span style="white-space:'
+            'nowrap;"><img src="/polarion/icons/default/enums/testrun_'
+            'status_failed.png" style="vertical-align:text-bottom;border:'
+            '0px;margin-right:2px;" class="polarion-no-style-cleanup"/>'
+            "</span>Failed</span></span></span><span> {0}</span></td></tr>"
+            "</table>".format(test_record.comment)
+        )
+        try:
+            table_rows = ""
+            test_steps = test_case.get_test_steps()
+            for step in range(len(test_record.test_step_results)):
+                table_rows += (
+                    "<tr {0}>"
+                    "<td {1}>{2}</td>"
+                    "<td {1}>{3}</td>"
+                    "<td {1}>{4}</td>"
+                    "<td {1}>{5}</td>"
+                    "<td {1}>{6}</td>"
+                    "</tr>".format(
+                        table_row_style,
+                        table_cell_style,
+                        test_step_results.get(
+                            test_record.test_step_results[step].result
+                        ),
+                        step + 1,
+                        test_steps.steps[step].values[0].content,
+                        test_steps.steps[step].values[1].content,
+                        test_record.test_step_results[step].comment,
+                    )
+                )
+        except (suds.WebFault, AttributeError):
+            # test_case.get_test_steps() can raise a webfault
+            # test_record.test_step_results cab raise an attribute error
+            # other errors should be passed up the call stack
+            table_rows = ""
+        if table_rows:
+            table = table_header + table_rows
+        else:
+            table = ""
+        content = tr_html + tc_html + table + verdict
+        return content
+
+    def __create_incident_report(
+        self, test_case_id: str, test_record: TestRecord
+    ) -> str:
+        """Create and populate an incident work item.
+
+        The work_item type of the incident and the fields to copy from the test
+        case and test run to the incident are defined in the tests configuration
+        of the project.
+        Throws an exception if the test case does not exists or if the incident
+        could not be created.
+
+        Args:
+            test_case_id (str): The ID of the test case.
+            test_record (TestRecord): The test record contains the results of the
+                test execution.
+                executed.
+
+        Returns:
+            str: work_item_id of the created incident.
+        """
+        project_id = self.project_id
+        status = "open"
+        project = Project(project_id)
+        tconf = project.get_tests_configuration()
+        defect_wi_type = tconf.defect_work_item_type
+        test_case_wi_type = tconf.test_case_work_item_type
+
+        try:
+            work_item_module = importlib.import_module("pylero.work_item")
+            wi_class_names = getattr(work_item_module, "workitems")
+            test_case_class_name = wi_class_names[test_case_wi_type]
+            test_case_class = getattr(work_item_module, test_case_class_name)
+            test_case = test_case_class(
+                project_id=self.project_id, work_item_id=test_case_id
+            )
+        except (AttributeError, PyleroLibException):
+            test_case = _WorkItem(project_id=self.project_id, work_item_id=test_case_id)
+
+        title = "Failed: " + test_case.title
+        description = self.__generate_description(test_case, test_record)
+        kwarg_dict = {}
+        for prop in tconf.fields_to_copy_from_test_case_to_defect.property:
+            if hasattr(test_case, prop.key):
+                kwarg_dict[prop.value] = getattr(test_case, prop.key)
+        for prop in tconf.fields_to_copy_from_test_run_to_linked_defect.property:
+            if hasattr(self, prop.key):
+                kwarg_dict[prop.value] = getattr(self, prop.key)
+
+        try:
+            incident_report = _WorkItem.create(
+                project_id, defect_wi_type, title, description, status, **kwarg_dict
+            )
+        except PyleroLibException as e:
+            msg = "\n".join(
+                [
+                    (
+                        f"Failed to create the work item {title} in"
+                        f"project {project_id} of type {defect_wi_type}."
+                    ),
+                    f"Error: {e}",
+                ]
+            )
+            raise PyleroLibException(msg)
+        incident_report.add_linked_item(test_case.work_item_id, "triggered_by")
+        return incident_report.work_item_id
+
     @tx_wrapper
-    def add_test_record_by_object(self, test_record, manual_state_change=False):
+    def add_test_record_by_object(
+        self, test_record, manual_state_change=False, create_incident=True
+    ):
         """method add_test_record_by_object, adds a test record for the given
         test case based on the TestRecord object passed in.
         In addition, the test run is checked for completeness and the test
         run state will change accordingly.
         If possible, the status is set to one of
         ["notrun", "finished", "inprogress"].
 
         Args:
             test_record (TestRecord or Polarion TestRecord):
             manual_state_change (boolean): Change test run state
                                            automatically or manual.
+            create_incident (boolean): Create an incident report if the test
+                                        case fails and no incident is linked.
 
         Returns:
             None
 
         References:
             test_management.addTestRecordToTestRun
         """
         self._verify_obj()
         test_case_id = test_record.test_case_id
         self._check_test_record_exists(test_case_id)
         if isinstance(test_record, TestRecord):
             suds_object = test_record._suds_object
         elif isinstance(test_record, TestRecord()._suds_object.__class__):
             suds_object = test_record
-        if test_record.result == "failed" and not test_record.defect_case_id:
-            test_record.defect_case_id = create_incident_report(
-                self, test_record, TestCase(work_item_id=test_case_id)
+        if (
+            test_record.result == "failed"
+            and not test_record.defect_case_id
+            and create_incident
+        ):
+            test_record.defect_case_id = self.__create_incident_report(
+                test_case_id,
+                test_record,
             )
         self.session.test_management_client.service.addTestRecordToTestRun(
             self.uri, suds_object
         )
 
         if manual_state_change:
             self.update()
@@ -1284,28 +1361,35 @@
         testrec.duration = duration
         if defect_work_item_id:
             testrec.defect_case_id = defect_work_item_id
         self.update_test_record_by_object(test_case_id, testrec)
 
     @tx_wrapper
     def update_test_record_by_object(
-        self, test_case_id, test_record, manual_state_change=False
+        self,
+        test_case_id,
+        test_record,
+        manual_state_change=False,
+        create_incident=True,
     ):
         """method update_test_record_by_object, adds a test record for the
         given test case based on the TestRecord object passed in.
         In addition, the test run is checked for completeness and the
         test run state will change accordingly.
         If possible, the status is set to one of
         ["notrun", "finished", "inprogress"].
 
         Args:
             test_case_id (str): the test case id that the record is related to.
             test_record (TestRecord or Polarion TestRecord)
             manual_state_change (boolean): Change the test
                                            run result automatically or manual.
+            create_incident (boolean): Create an incident report if the test
+                                        record result is failed and no defect
+                                        case id is set.
 
         Returns:
             None
 
         References:
             test_management.updateTestRecordAtIndex
         """
@@ -1314,17 +1398,21 @@
         # because this function (specifically and not documented) uses the
         # actual index of the test records and not the index of all
         # executed records.
         test_case_ids = [rec.test_case_id for rec in self._records]
         if test_case_id not in test_case_ids:
             self.add_test_record_by_object(test_record)
         else:
-            if test_record.result == "failed" and not test_record.defect_case_id:
-                test_record.defect_case_id = create_incident_report(
-                    self, test_record, TestCase(work_item_id=test_case_id)
+            if (
+                test_record.result == "failed"
+                and not test_record.defect_case_id
+                and create_incident
+            ):
+                test_record.defect_case_id = self.__create_incident_report(
+                    test_case_id, test_record
                 )
             index = test_case_ids.index(test_case_id)
             if isinstance(test_record, TestRecord):
                 suds_object = test_record._suds_object
             elif isinstance(test_record, TestRecord()._suds_object.__class__):
                 suds_object = test_record
             self.session.test_management_client.service.updateTestRecordAtIndex(
```

### Comparing `pylero-0.0.9/src/pylero/test_run_attachment.py` & `pylero-0.1.0/src/pylero/test_run_attachment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/test_step.py` & `pylero-0.1.0/src/pylero/test_step.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/test_step_result.py` & `pylero-0.1.0/src/pylero/test_step_result.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/test_steps.py` & `pylero-0.1.0/src/pylero/test_steps.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/tests_configuration.py` & `pylero-0.1.0/src/pylero/tests_configuration.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/text.py` & `pylero-0.1.0/src/pylero/text.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/time_point.py` & `pylero-0.1.0/src/pylero/time_point.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/user.py` & `pylero-0.1.0/src/pylero/user.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/wiki_page.py` & `pylero-0.1.0/src/pylero/wiki_page.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/wiki_page_attachment.py` & `pylero-0.1.0/src/pylero/wiki_page_attachment.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/work_item.py` & `pylero-0.1.0/src/pylero/work_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,15 +632,17 @@
         self._verify_obj()
         self.check_valid_field_values(role, "hyperlink-role", {})
         suds_role = EnumOptionId(role)._suds_object
         return self.session.tracker_client.service.addHyperlink(
             self.uri, url, suds_role
         )
 
-    def add_linked_item(self, linked_work_item_id, role, revision=None, suspect=None):
+    def add_linked_item(
+        self, linked_work_item_id, role, revision=None, suspect=None, project_id=None
+    ):
         """method add_linked_item adds a linked _WorkItem to current _WorkItem
         The linking is done to the "child" object. For example, if you have a
         Test Case that verifies a requirement, you would add the
         linked item to the Test Case with the "verifies" role and
         not the Requirement.
 
         Args:
@@ -649,28 +651,31 @@
             role (str): the role of the hyperlink to add.
             revision (str): optional, specific revision for linked item
                            (None means HEAD revision)
                            default: None
             suspect (bool): true if the link should be marked with suspect flag
                       Only valid if revision is set.
                       default: None
+            project_id (str): optional, the project where the target item is.
+                    If not set, the current project is used.
+                    default: None
 
         Returns:
             bool
 
         References:
             Tracker.addLinkedItem
             Tracker.addLinkedItemWithRev
         """
         self._verify_obj()
         # validates the role. Will raise PyleroLibException if invalid
         self.check_valid_field_values(role, "workitem-link-role", {})
-        wi_linked = _WorkItem(
-            work_item_id=linked_work_item_id, project_id=self.project_id
-        )
+        if project_id is None:
+            project_id = self.project_id
+        wi_linked = _WorkItem(work_item_id=linked_work_item_id, project_id=project_id)
         enum_role = EnumOptionId(role)._suds_object
         function_name = "addLinkedItem"
         parms = [self.uri, wi_linked.uri, enum_role]
         if revision:
             function_name += "WithRev"
             parms += [revision, suspect]
         return getattr(self.session.tracker_client.service, function_name)(*parms)
@@ -740,17 +745,17 @@
                 suds_content = content._suds_object
             else:  # is a suds object
                 suds_content = content
         else:
             suds_content = suds.null()
         if parent_uri is None:
             parent_uri = self.uri
-            title = None
         else:
             parent_uri = str(parent_uri)
+            title = None
             is_existing_comment = any([str(c.uri) == parent_uri for c in self.comments])
             if not is_existing_comment:
                 raise PyleroLibException(
                     "The parent_uri is not a valid comment for this work item"
                 )
         self.session.tracker_client.service.addComment(
             str(parent_uri), title, suds_content
```

### Comparing `pylero-0.0.9/src/pylero/work_record.py` & `pylero-0.1.0/src/pylero/work_record.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/pylero/workflow_action.py` & `pylero-0.1.0/src/pylero/workflow_action.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/unit_tests/attribute_test.py` & `pylero-0.1.0/src/unit_tests/attribute_test.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/unit_tests/document_test.py` & `pylero-0.1.0/src/unit_tests/document_test.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/unit_tests/plan_test.py` & `pylero-0.1.0/src/unit_tests/plan_test.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/unit_tests/revert_tests.py` & `pylero-0.1.0/src/unit_tests/revert_tests.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/unit_tests/test_run_test.py` & `pylero-0.1.0/src/unit_tests/test_run_test.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/src/unit_tests/work_item_test.py` & `pylero-0.1.0/src/unit_tests/work_item_test.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/tier_tests.py` & `pylero-0.1.0/tier_tests.py`

 * *Files identical despite different names*

### Comparing `pylero-0.0.9/tox.ini` & `pylero-0.1.0/tox.ini`

 * *Files identical despite different names*

