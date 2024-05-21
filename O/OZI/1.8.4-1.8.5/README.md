# Comparing `tmp/OZI-1.8.4.tar.gz` & `tmp/OZI-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.8.4.tar", last modified: Mon May 20 01:15:31 2024, max compression
+gzip compressed data, was "OZI-1.8.5.tar", last modified: Tue May 21 13:18:07 2024, max compression
```

## Comparing `OZI-1.8.4.tar` & `OZI-1.8.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.747186 OZI-1.8.4/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.719186 OZI-1.8.4/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.719186 OZI-1.8.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.719186 OZI-1.8.4/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2901 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-20 01:12:00.000000 OZI-1.8.4/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-20 01:12:00.000000 OZI-1.8.4/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   313368 2024-05-20 01:12:00.000000 OZI-1.8.4/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-20 01:12:00.000000 OZI-1.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-20 01:15:14.515185 OZI-1.8.4/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6969 2024-05-20 01:12:00.000000 OZI-1.8.4/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    17469 2024-05-20 01:12:00.000000 OZI-1.8.4/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7549 2024-05-20 01:12:00.000000 OZI-1.8.4/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.743186 OZI-1.8.4/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5880 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.727186 OZI-1.8.4/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.727186 OZI-1.8.4/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.731186 OZI-1.8.4/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.731186 OZI-1.8.4/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4097 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6391 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.735186 OZI-1.8.4/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.731186 OZI-1.8.4/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.731186 OZI-1.8.4/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.731186 OZI-1.8.4/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.731186 OZI-1.8.4/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.735186 OZI-1.8.4/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.735186 OZI-1.8.4/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.735186 OZI-1.8.4/ozi/lint/readme-renderer/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/readme-renderer/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       19 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/lint/readme-renderer/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.735186 OZI-1.8.4/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4745 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.739186 OZI-1.8.4/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.743186 OZI-1.8.4/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      503 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2513 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6164 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4504 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1409 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.743186 OZI-1.8.4/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.743186 OZI-1.8.4/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.743186 OZI-1.8.4/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.747186 OZI-1.8.4/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.747186 OZI-1.8.4/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-20 01:12:00.000000 OZI-1.8.4/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10976 2024-05-20 01:12:00.000000 OZI-1.8.4/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-20 01:12:00.000000 OZI-1.8.4/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.747186 OZI-1.8.4/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-20 01:12:00.000000 OZI-1.8.4/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:14.747186 OZI-1.8.4/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-20 01:12:00.000000 OZI-1.8.4/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-20 01:12:00.000000 OZI-1.8.4/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-20 01:12:00.000000 OZI-1.8.4/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-20 01:12:00.000000 OZI-1.8.4/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.622977 OZI-1.8.5/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.594977 OZI-1.8.5/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.594977 OZI-1.8.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.594977 OZI-1.8.5/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2901 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-21 13:14:42.000000 OZI-1.8.5/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-21 13:14:42.000000 OZI-1.8.5/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   314741 2024-05-21 13:14:42.000000 OZI-1.8.5/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-21 13:14:42.000000 OZI-1.8.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-21 13:17:51.386976 OZI-1.8.5/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6969 2024-05-21 13:14:42.000000 OZI-1.8.5/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    17469 2024-05-21 13:14:42.000000 OZI-1.8.5/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7549 2024-05-21 13:14:42.000000 OZI-1.8.5/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.618977 OZI-1.8.5/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5880 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.606977 OZI-1.8.5/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.606977 OZI-1.8.5/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.606977 OZI-1.8.5/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.606977 OZI-1.8.5/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4097 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6391 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.606977 OZI-1.8.5/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.606977 OZI-1.8.5/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/lint/readme-renderer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/readme-renderer/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       19 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/lint/readme-renderer/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.610977 OZI-1.8.5/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4745 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.614977 OZI-1.8.5/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.618977 OZI-1.8.5/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      503 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2513 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6164 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4504 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1409 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.618977 OZI-1.8.5/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.618977 OZI-1.8.5/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.618977 OZI-1.8.5/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.622977 OZI-1.8.5/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.622977 OZI-1.8.5/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-21 13:14:42.000000 OZI-1.8.5/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10976 2024-05-21 13:14:42.000000 OZI-1.8.5/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-21 13:14:42.000000 OZI-1.8.5/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.622977 OZI-1.8.5/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-21 13:14:42.000000 OZI-1.8.5/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:17:51.622977 OZI-1.8.5/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-21 13:14:42.000000 OZI-1.8.5/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-21 13:14:42.000000 OZI-1.8.5/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-21 13:14:42.000000 OZI-1.8.5/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-21 13:14:42.000000 OZI-1.8.5/tests/test_tap.py
```

### Comparing `OZI-1.8.4/.github/CODEOWNERS` & `OZI-1.8.5/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/CODE_OF_CONDUCT.md` & `OZI-1.8.5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/CONTRIBUTING.md` & `OZI-1.8.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.8.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.8.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/SECURITY.md` & `OZI-1.8.5/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/workflows/codeql.yml` & `OZI-1.8.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/workflows/dependency-review.yml` & `OZI-1.8.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/workflows/dev-workflow.yml` & `OZI-1.8.5/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.github/workflows/dist-workflow.yml` & `OZI-1.8.5/.github/workflows/dist-workflow.yml`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             files.pythonhosted.org:443
             fulcio.sigstore.dev:443
             github.com:443
             pypi.org:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/release@8b5e46e9d8899289f676ca2b432a63fe2faa93f9
+      - uses: OZI-Project/release@033e98adfa7086d1b1273bcc80b0576297e733bd
         id: release
         with:
           tag: ${{ needs.draft.outputs.tag }}
           python-dist: ${{ matrix.py }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
   generate-provenance:
@@ -204,10 +204,10 @@
         disable-sudo: true
         egress-policy: block
         allowed-endpoints: >
           api.github.com:443
           upload.pypi.org:443
           uploads.github.com:443
 
-    - uses: OZI-Project/publish@87aae4bed7ea3ab8b864689945200ecd71ecc29f
+    - uses: OZI-Project/publish@e0a606616e2ff69a1b564f151f1061601683668f
       with:
         github-token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `OZI-1.8.4/.github/workflows/scorecard.yml` & `OZI-1.8.5/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/.gitignore` & `OZI-1.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/CHANGELOG.md` & `OZI-1.8.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,42 @@
 # CHANGELOG
+## 1.8.5 (2024-05-21)
+
+### :arrow_up:
+
+* :arrow_up: Bump OZI-Project/publish from 0.1.1 to 0.1.2
+
+Bumps [OZI-Project/publish](https://github.com/ozi-project/publish) from 0.1.1 to 0.1.2.
+- [Release notes](https://github.com/ozi-project/publish/releases)
+- [Commits](https://github.com/ozi-project/publish/compare/87aae4bed7ea3ab8b864689945200ecd71ecc29f...e0a606616e2ff69a1b564f151f1061601683668f)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/publish
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`a7903eb`](https://github.com/OZI-Project/OZI/commit/a7903eb30aec3bc1afd7a90b3f641bc59a30945c))
+
+* :arrow_up: Bump OZI-Project/release from 0.4.0 to 0.4.1
+
+Bumps [OZI-Project/release](https://github.com/ozi-project/release) from 0.4.0 to 0.4.1.
+- [Release notes](https://github.com/ozi-project/release/releases)
+- [Commits](https://github.com/ozi-project/release/compare/8b5e46e9d8899289f676ca2b432a63fe2faa93f9...033e98adfa7086d1b1273bcc80b0576297e733bd)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/release
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`04a849d`](https://github.com/OZI-Project/OZI/commit/04a849d5ffc200d5f5f609dcee64fcde0f516a9d))
+
 ## 1.8.4 (2024-05-20)
 
 ### :bug:
 
 * :bug: Shorten reprs of pkg and project spec.
 
 Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`0dc3f21`](https://github.com/OZI-Project/OZI/commit/0dc3f21e2a61d02ca7af9ffdbf60644dfa4ac511))
```

### Comparing `OZI-1.8.4/LICENSE.txt` & `OZI-1.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/PKG-INFO` & `OZI-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.8.4
+Version: 1.8.5
 Summary: Package Python projects with Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.8.4.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.8.5.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.8.4/README.rst` & `OZI-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/meson.build` & `OZI-1.8.5/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/meson.options` & `OZI-1.8.5/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/__main__.py` & `OZI-1.8.5/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/actions.py` & `OZI-1.8.5/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/comment.py` & `OZI-1.8.5/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/fix/__main__.py` & `OZI-1.8.5/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/fix/build_definition.py` & `OZI-1.8.5/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/fix/meson.build` & `OZI-1.8.5/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/fix/missing.py` & `OZI-1.8.5/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/fix/parser.py` & `OZI-1.8.5/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/fix/rewrite_command.py` & `OZI-1.8.5/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/lint/meson.build` & `OZI-1.8.5/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/lint/pyright/meson.build` & `OZI-1.8.5/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/meson.build` & `OZI-1.8.5/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/meson.py` & `OZI-1.8.5/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/new/__main__.py` & `OZI-1.8.5/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/new/meson.build` & `OZI-1.8.5/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/new/parser.py` & `OZI-1.8.5/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/new/validate.py` & `OZI-1.8.5/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/pkg_extra.py` & `OZI-1.8.5/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/render.py` & `OZI-1.8.5/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/core_metadata_template.py` & `OZI-1.8.5/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/meson.build` & `OZI-1.8.5/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.8.5/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.8.5/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/render_requirements.py` & `OZI-1.8.5/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.8.5/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/scm_version_snip.py` & `OZI-1.8.5/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/to_distribution_template.py` & `OZI-1.8.5/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/scripts/version_metadata_template.py` & `OZI-1.8.5/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spdx.py` & `OZI-1.8.5/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/_license.py` & `OZI-1.8.5/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/_spec.py` & `OZI-1.8.5/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/base.py` & `OZI-1.8.5/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/ci.py` & `OZI-1.8.5/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/meson.build` & `OZI-1.8.5/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/pkg.py` & `OZI-1.8.5/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/project.py` & `OZI-1.8.5/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/python.py` & `OZI-1.8.5/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/spec/src.py` & `OZI-1.8.5/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/tap.py` & `OZI-1.8.5/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/trove.py` & `OZI-1.8.5/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/__init__.py` & `OZI-1.8.5/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/__main__.py` & `OZI-1.8.5/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/deliverability.py` & `OZI-1.8.5/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.8.5/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/meson.build` & `OZI-1.8.5/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.8.5/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/syntax.py` & `OZI-1.8.5/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/email_validator/validate_email.py` & `OZI-1.8.5/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/ozi/vendor/meson.build` & `OZI-1.8.5/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/pyproject.toml` & `OZI-1.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/templates/CHANGELOG.md.j2` & `OZI-1.8.5/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/tests/meson.build` & `OZI-1.8.5/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/tests/test_ozi_fix.py` & `OZI-1.8.5/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/tests/test_ozi_new.py` & `OZI-1.8.5/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.4/tests/test_tap.py` & `OZI-1.8.5/tests/test_tap.py`

 * *Files identical despite different names*

