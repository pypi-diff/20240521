# Comparing `tmp/impsparc-3.1.5.tar.gz` & `tmp/impsparc-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impsparc-3.1.5.tar", last modified: Tue May 21 07:28:50 2024, max compression
+gzip compressed data, was "impsparc-3.1.6.tar", last modified: Tue May 21 07:48:16 2024, max compression
```

## Comparing `impsparc-3.1.5.tar` & `impsparc-3.1.6.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.598413 impsparc-3.1.5/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1064 2023-11-16 11:18:05.000000 impsparc-3.1.5/LICENSE.md
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      244 2023-11-16 18:00:04.000000 impsparc-3.1.5/MANIFEST.in
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-05-21 07:28:50.597570 impsparc-3.1.5/PKG-INFO
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      871 2023-11-16 11:18:05.000000 impsparc-3.1.5/README.md
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.218501 impsparc-3.1.5/cvsvc_apirisk/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.234138 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   363678 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   262350 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      615 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      753 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23616 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16394 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16378 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.236241 impsparc-3.1.5/cvsvc_apirisk/score/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2891 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.293166 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       80 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18889 2024-04-04 10:32:17.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1503 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.340932 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2433 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2453 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2662 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2684 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2697 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2117 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2387 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2385 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2393 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2391 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2722 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2731 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.362227 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2346 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2474 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2477 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2459 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2462 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2760 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3371 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/json_line.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23957 2024-05-21 07:28:28.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/rules_util.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     8837 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/s-origin.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.400535 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2084 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2418 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2339 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2867 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2292 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2163 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5141 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2685 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2635 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2479 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2769 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6786 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sp2_reporting.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.407046 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.211753 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.532166 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.541575 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15291 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16918 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15192 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    28781 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11370 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1363 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11350 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11421 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      966 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.570162 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      423 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16193 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      209 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3581 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3478 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3944 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      309 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      406 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6482 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     9574 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1212 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    88994 2023-11-16 18:00:53.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.422586 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.209380 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.442689 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   207965 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      687 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      756 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2033 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.454176 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    59219 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   195090 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4023 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    71478 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    56178 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.472489 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   100782 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   163872 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    80388 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11245 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      393 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11230 2023-11-16 11:18:05.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.509966 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   181852 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   105536 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    60520 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23940 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   388460 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   154228 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    10556 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4960 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    32011 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc_html_generation.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18982 2024-05-17 09:11:34.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/spec_parse.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5399 2024-04-12 10:44:03.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/spec_util.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5478 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3194 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    26214 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    12521 2023-11-16 17:30:59.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_spec_util.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1193 2023-12-05 04:59:05.000000 impsparc-3.1.5/cvsvc_apirisk/score/spec_security/yaml_line.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:28:50.595426 impsparc-3.1.5/impsparc.egg-info/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-05-21 07:28:50.000000 impsparc-3.1.5/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     7218 2024-05-21 07:28:50.000000 impsparc-3.1.5/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        1 2024-05-21 07:28:50.000000 impsparc-3.1.5/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      164 2024-05-21 07:28:50.000000 impsparc-3.1.5/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      178 2024-05-21 07:28:50.000000 impsparc-3.1.5/impsparc.egg-info/requires.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       14 2024-05-21 07:28:50.000000 impsparc-3.1.5/impsparc.egg-info/top_level.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       38 2024-05-21 07:28:50.598658 impsparc-3.1.5/setup.cfg
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1189 2024-05-21 07:28:40.000000 impsparc-3.1.5/setup.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.657459 impsparc-3.1.6/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1064 2023-11-16 11:18:05.000000 impsparc-3.1.6/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      244 2023-11-16 18:00:04.000000 impsparc-3.1.6/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-05-21 07:48:16.657143 impsparc-3.1.6/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      871 2023-11-16 11:18:05.000000 impsparc-3.1.6/README.md
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.574340 impsparc-3.1.6/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.580648 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   363678 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   262350 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      615 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      753 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23616 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16394 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16378 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.582392 impsparc-3.1.6/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2891 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.594079 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       80 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18889 2024-04-04 10:32:17.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1503 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.604340 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2433 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2453 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2662 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2684 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2697 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2117 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2387 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2385 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2393 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2391 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2722 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2731 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.611635 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2346 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2474 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2477 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2459 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2462 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2760 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3371 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/json_line.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23957 2024-05-21 07:28:28.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/rules_util.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     8837 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/s-origin.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.619637 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2084 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2418 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2339 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2867 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2292 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2163 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5141 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2685 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2635 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2479 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2769 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6786 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sp2_reporting.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.620408 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.570352 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.642248 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.644825 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15291 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16918 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15192 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    28781 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11370 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1363 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11350 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11421 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      966 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.652259 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      423 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16193 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      209 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3581 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3478 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3944 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      309 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      406 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6482 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     9574 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1212 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    88994 2023-11-16 18:00:53.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.622591 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.568050 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.626262 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   207965 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      687 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      756 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2033 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.628542 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    59219 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   195090 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4023 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    71478 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    56178 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.632761 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   100782 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   163872 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    80388 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11245 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      393 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11230 2023-11-16 11:18:05.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.638988 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   181852 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   105536 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    60520 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23940 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   388460 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   154228 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    10556 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4960 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    32011 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc_html_generation.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18982 2024-05-17 09:11:34.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/spec_parse.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5399 2024-04-12 10:44:03.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/spec_util.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5478 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3194 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    26214 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    12521 2023-11-16 17:30:59.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1193 2023-12-05 04:59:05.000000 impsparc-3.1.6/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-05-21 07:48:16.656503 impsparc-3.1.6/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-05-21 07:48:16.000000 impsparc-3.1.6/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     7218 2024-05-21 07:48:16.000000 impsparc-3.1.6/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        1 2024-05-21 07:48:16.000000 impsparc-3.1.6/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      164 2024-05-21 07:48:16.000000 impsparc-3.1.6/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      178 2024-05-21 07:48:16.000000 impsparc-3.1.6/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       14 2024-05-21 07:48:16.000000 impsparc-3.1.6/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       38 2024-05-21 07:48:16.657576 impsparc-3.1.6/setup.cfg
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1189 2024-05-21 07:47:29.000000 impsparc-3.1.6/setup.py
```

### Comparing `impsparc-3.1.5/LICENSE.md` & `impsparc-3.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/PKG-INFO` & `impsparc-3.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 3.1.5
+Version: 3.1.6
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-3.1.5/README.md` & `impsparc-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-3.1.6/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/base.py` & `impsparc-3.1.6/cvsvc_apirisk/score/base.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/rules_util.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/rules_util.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/s-origin.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/s-origin.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sp2_reporting.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sp2_reporting.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sparc_html_generation.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sparc_html_generation.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/spec_parse.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/spec_parse.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/spec_util.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/spec_util.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/sps_spec_util.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/sps_spec_util.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/cvsvc_apirisk/score/spec_security/yaml_line.py` & `impsparc-3.1.6/cvsvc_apirisk/score/spec_security/yaml_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/impsparc.egg-info/PKG-INFO` & `impsparc-3.1.6/impsparc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 3.1.5
+Version: 3.1.6
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-3.1.5/impsparc.egg-info/SOURCES.txt` & `impsparc-3.1.6/impsparc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.5/setup.py` & `impsparc-3.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "3.1.5"),
+    version=os.environ.get("VER", "3.1.6"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

