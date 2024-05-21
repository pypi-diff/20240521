# Comparing `tmp/deeploy-1.37.3.tar.gz` & `tmp/deeploy-1.37.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeploy-1.37.3.tar", last modified: Mon May 20 11:32:39 2024, max compression
+gzip compressed data, was "deeploy-1.37.4.tar", last modified: Tue May 21 14:34:06 2024, max compression
```

## Comparing `deeploy-1.37.3.tar` & `deeploy-1.37.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/
--rw-rw-rw-   0 root         (0) root         (0)    11346 2024-05-20 11:32:37.000000 deeploy-1.37.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-20 11:32:39.220363 deeploy-1.37.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1900 2024-05-20 11:32:37.000000 deeploy-1.37.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/cli/custom_instances/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/model.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/model_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     7165 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deeploycli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/cli/deploy_instances/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     4894 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/parser_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/parser_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/parser_transformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/explainer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/explainer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/transformer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/transformer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/explainer_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/model_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1748 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/transformer_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)    20741 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/common/
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/common/constants/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/constants/pytorch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/common/functions/
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/functions/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/deepfair/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/deepfair/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6549 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/deepfair/fair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/enums/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/algo.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/auth_type.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/explainer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/prediction_version.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/qf.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/query_param.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/transformer_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.216363 deeploy-1.37.3/deeploy/fairsd/
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30522 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/algorithms.py
--rw-rw-rw-   0 root         (0) root         (0)    13196 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/discretization.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/qualitymeasures.py
--rw-rw-rw-   0 root         (0) root         (0)     8381 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/searchspace.py
--rw-rw-rw-   0 root         (0) root         (0)     7701 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/sgdescription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/models/
--rw-rw-rw-   0 root         (0) root         (0)     1543 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/actual_response.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/client_options.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_actuals.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_azure_ml_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     6608 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_deployment_base.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_explainer_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_model_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_sagemaker_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_transformer_reference.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/feature.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/get_prediction_logs_options.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/metadata_json.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/prediction_log.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/reference_json.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_azure_ml_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     6807 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_deployment_base.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_deployment_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_sagemaker_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/services/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16781 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/deeploy_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4727 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainer_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/services/explainers/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/alibi.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/base_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/omni_tabular.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/shap.py
--rw-rw-rw-   0 root         (0) root         (0)     3432 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/file_service.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/git_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/model_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/services/models/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/onnx.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/pytorch.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/tensorflow.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/triton.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/xgboost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3647 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 11:32:39.224363 deeploy-1.37.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1806 2024-05-20 11:32:37.000000 deeploy-1.37.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/test/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-20 11:32:37.000000 deeploy-1.37.3/test/test_deeploy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.727051 deeploy-1.37.4/
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2024-05-21 14:30:56.000000 deeploy-1.37.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-21 14:34:06.727051 deeploy-1.37.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2024-05-21 14:30:56.000000 deeploy-1.37.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.715051 deeploy-1.37.4/deeploy/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.715051 deeploy-1.37.4/deeploy/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.715051 deeploy-1.37.4/deeploy/cli/custom_instances/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/custom_instances/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/custom_instances/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/custom_instances/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/custom_instances/model_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1643 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/custom_instances/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7196 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/deeploycli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.715051 deeploy-1.37.4/deeploy/cli/deploy_instances/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/deploy_instances/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/deploy_instances/deeploy_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/deploy_instances/deeploy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/deploy_instances/deeploy_transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4894 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.715051 deeploy-1.37.4/deeploy/cli/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/parsers/parser_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/parsers/parser_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/parsers/parser_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/cli/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/cli/templates/explainer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/templates/explainer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/cli/templates/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/templates/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/cli/templates/transformer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/templates/transformer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/cli/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/wrappers/explainer_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/wrappers/model_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/cli/wrappers/transformer_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)    20741 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/common/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/common/constants/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/common/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/common/constants/pytorch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/common/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/common/functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/common/functions/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/deepfair/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/deepfair/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6549 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/deepfair/fair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.719051 deeploy-1.37.4/deeploy/enums/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/algo.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/auth_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/explainer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/prediction_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/qf.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/query_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/enums/transformer_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.723051 deeploy-1.37.4/deeploy/fairsd/
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/fairsd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30522 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/fairsd/algorithms.py
+-rw-rw-rw-   0 root         (0) root         (0)    13196 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/fairsd/discretization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/fairsd/qualitymeasures.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/fairsd/searchspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     7701 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/fairsd/sgdescription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.727051 deeploy-1.37.4/deeploy/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/actual_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/client_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_actuals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_azure_ml_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6608 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_deployment_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_explainer_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_model_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_sagemaker_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/create_transformer_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/get_prediction_logs_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/metadata_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/prediction_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/reference_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/update_azure_ml_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6807 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/update_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/update_deployment_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/update_deployment_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/update_sagemaker_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/models/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.727051 deeploy-1.37.4/deeploy/services/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16781 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/deeploy_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/explainer_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.727051 deeploy-1.37.4/deeploy/services/explainers/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/explainers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/explainers/alibi.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/explainers/base_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/explainers/omni_tabular.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/explainers/shap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3432 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/file_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/git_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/model_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.727051 deeploy-1.37.4/deeploy/services/models/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/onnx.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/pytorch.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/sklearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/tensorflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/triton.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-21 14:30:56.000000 deeploy-1.37.4/deeploy/services/models/xgboost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.715051 deeploy-1.37.4/deeploy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-21 14:34:06.000000 deeploy-1.37.4/deeploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3647 2024-05-21 14:34:06.000000 deeploy-1.37.4/deeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 14:34:06.000000 deeploy-1.37.4/deeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-21 14:34:06.000000 deeploy-1.37.4/deeploy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-21 14:34:06.000000 deeploy-1.37.4/deeploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-21 14:34:06.000000 deeploy-1.37.4/deeploy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 14:34:06.727051 deeploy-1.37.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2024-05-21 14:30:56.000000 deeploy-1.37.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:34:06.727051 deeploy-1.37.4/test/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-21 14:30:56.000000 deeploy-1.37.4/test/test_deeploy.py
```

### Comparing `deeploy-1.37.3/LICENSE` & `deeploy-1.37.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/PKG-INFO` & `deeploy-1.37.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 1.37.3
+Version: 1.37.4
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-1.37.3/README.md` & `deeploy-1.37.4/README.md`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/__init__.py` & `deeploy-1.37.4/deeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/custom_instances/explainer.py` & `deeploy-1.37.4/deeploy/cli/custom_instances/explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/custom_instances/model.py` & `deeploy-1.37.4/deeploy/cli/custom_instances/model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/custom_instances/model_repository.py` & `deeploy-1.37.4/deeploy/cli/custom_instances/model_repository.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/custom_instances/transformer.py` & `deeploy-1.37.4/deeploy/cli/custom_instances/transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,28 +31,19 @@
         Parameters:
             payload (Dict): To be predicted input values for model.
             headers (Dict): Request headers.
 
         Returns:
             Dict: Return the pre model prediction transformed inputs.
         """
-        return {
-            "instances": [
-                self.transformer._preprocess(inputs=instance) for instance in payload["instances"]
-            ]
-        }
+        return self.transformer._preprocess(payload=payload)
 
     def postprocess(self, response: Dict, headers: Dict[str, str] = None) -> Dict:
         """
         Parameters:
             payload (Dict): Predicted values from model.
             headers (Dict): Request headers.
 
         Returns:
             Dict: Return the post model prediction transformed result.
         """
-        return {
-            "predictions": [
-                self.transformer._postprocess(inputs=prediction)
-                for prediction in response["predictions"]
-            ]
-        }
+        return self.transformer._postprocess(response=response)
```

### Comparing `deeploy-1.37.3/deeploy/cli/deeploycli.py` & `deeploy-1.37.4/deeploy/cli/deeploycli.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     os.makedirs(projectname, exist_ok=True)
 
     template_vars = {
         "projectname": projectname,
         "model": True if Instances.model.value in initialization else False,
         "explainer": True if Instances.explainer.value in initialization else False,
         "transformer": True if Instances.transformer.value in initialization else False,
+        "version": __version__
     }
     generate_readme(projectname, template_vars)
     click.echo("Generated README.")
 
     generate_metadata(projectname)
     click.echo("Generated metadata.")
```

### Comparing `deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_explainer.py` & `deeploy-1.37.4/deeploy/cli/deploy_instances/deeploy_explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_model.py` & `deeploy-1.37.4/deeploy/cli/deploy_instances/deeploy_model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_transformer.py` & `deeploy-1.37.4/deeploy/cli/deploy_instances/deeploy_transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/interface.py` & `deeploy-1.37.4/deeploy/cli/interface.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/parsers/parser_explainer.py` & `deeploy-1.37.4/deeploy/cli/parsers/parser_explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/parsers/parser_model.py` & `deeploy-1.37.4/deeploy/cli/parsers/parser_model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/parsers/parser_transformer.py` & `deeploy-1.37.4/deeploy/cli/parsers/parser_transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/utils.py` & `deeploy-1.37.4/deeploy/cli/utils.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/wrappers/explainer_wrapper.py` & `deeploy-1.37.4/deeploy/cli/wrappers/explainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/wrappers/model_wrapper.py` & `deeploy-1.37.4/deeploy/cli/wrappers/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/cli/wrappers/transformer_wrapper.py` & `deeploy-1.37.4/deeploy/cli/wrappers/transformer_wrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,43 +10,58 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from typing import List
+from typing import Dict
 
 import kserve
 
 
 class TransformerWrapper:
     logging.basicConfig(level=kserve.constants.KSERVE_LOGLEVEL)
 
     def __init__(self):
         """Initializes the Transformer Wrapper Class"""
 
-    def _preprocess(self, inputs: List) -> List:
+    def _preprocess(self, payload: Dict) -> Dict:
         """Preprocess transformation before model prediction
         Parameters:
-            inputs (List): \
-                Receive one input that needs to be transformed before model prediction \
-                  eg. [0, 0, 1]
+            payload (Dict): \
+                Receives the entire request payload that needs to be transformed before model prediction \
+                  {
+                    "instances": [
+                        [
+                        3.5,
+                        5.1,
+                        1.4,
+                        0.2
+                        ]
+                    ]
+                  }
 
         Returns
-            transformed input as List
-                Note: For no transformation return inputs
+            transformed payload as Dict 
+                Note: For no transformation return payload
         """
         raise NotImplementedError
 
-    def _postprocess(self, inputs: List) -> List:
+    def _postprocess(self, response: Dict) -> Dict:
         """Postprocess transformation on model prediction output
         Parameters:
-            inputs (List): \
-                Receive one input that needs to be transformed after model prediction \
-                  eg. [0, 0, 1]
+            response (Dict): \
+                Receive the entire response of model that needs modification \
+                    {
+                    "predictions": [
+                        [
+                        true
+                        ]
+                    ]
+                    }
 
         Returns
-            transformed input as List
-                Note: For no transformation return inputs
+            transformed response as Dict 
+                Note: For no transformation return response
         """
         raise NotImplementedError
```

### Comparing `deeploy-1.37.3/deeploy/client.py` & `deeploy-1.37.4/deeploy/client.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/common/constants/pytorch.py` & `deeploy-1.37.4/deeploy/common/constants/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/common/functions/functions.py` & `deeploy-1.37.4/deeploy/common/functions/functions.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/deepfair/fair.py` & `deeploy-1.37.4/deeploy/deepfair/fair.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/fairsd/algorithms.py` & `deeploy-1.37.4/deeploy/fairsd/algorithms.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/fairsd/discretization.py` & `deeploy-1.37.4/deeploy/fairsd/discretization.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/fairsd/qualitymeasures.py` & `deeploy-1.37.4/deeploy/fairsd/qualitymeasures.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/fairsd/searchspace.py` & `deeploy-1.37.4/deeploy/fairsd/searchspace.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/fairsd/sgdescription.py` & `deeploy-1.37.4/deeploy/fairsd/sgdescription.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/__init__.py` & `deeploy-1.37.4/deeploy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/client_options.py` & `deeploy-1.37.4/deeploy/models/client_options.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_actuals.py` & `deeploy-1.37.4/deeploy/models/create_actuals.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_azure_ml_deployment.py` & `deeploy-1.37.4/deeploy/models/create_azure_ml_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_deployment.py` & `deeploy-1.37.4/deeploy/models/create_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_deployment_base.py` & `deeploy-1.37.4/deeploy/models/create_deployment_base.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_evaluation.py` & `deeploy-1.37.4/deeploy/models/create_evaluation.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_explainer_reference.py` & `deeploy-1.37.4/deeploy/models/create_explainer_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_metadata.py` & `deeploy-1.37.4/deeploy/models/create_metadata.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_model_reference.py` & `deeploy-1.37.4/deeploy/models/create_model_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_sagemaker_deployment.py` & `deeploy-1.37.4/deeploy/models/create_sagemaker_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/create_transformer_reference.py` & `deeploy-1.37.4/deeploy/models/create_transformer_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/deployment.py` & `deeploy-1.37.4/deeploy/models/deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/get_prediction_logs_options.py` & `deeploy-1.37.4/deeploy/models/get_prediction_logs_options.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/prediction_log.py` & `deeploy-1.37.4/deeploy/models/prediction_log.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/reference_json.py` & `deeploy-1.37.4/deeploy/models/reference_json.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/update_azure_ml_deployment.py` & `deeploy-1.37.4/deeploy/models/update_azure_ml_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/update_deployment.py` & `deeploy-1.37.4/deeploy/models/update_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/update_deployment_base.py` & `deeploy-1.37.4/deeploy/models/update_deployment_base.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/update_deployment_description.py` & `deeploy-1.37.4/deeploy/models/update_deployment_description.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/models/update_sagemaker_deployment.py` & `deeploy-1.37.4/deeploy/models/update_sagemaker_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/deeploy_service.py` & `deeploy-1.37.4/deeploy/services/deeploy_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/explainer_wrapper.py` & `deeploy-1.37.4/deeploy/services/explainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/explainers/alibi.py` & `deeploy-1.37.4/deeploy/services/explainers/alibi.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/explainers/omni_tabular.py` & `deeploy-1.37.4/deeploy/services/explainers/omni_tabular.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/explainers/shap.py` & `deeploy-1.37.4/deeploy/services/explainers/shap.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/file_service.py` & `deeploy-1.37.4/deeploy/services/file_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/git_service.py` & `deeploy-1.37.4/deeploy/services/git_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/model_wrapper.py` & `deeploy-1.37.4/deeploy/services/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/models/pytorch.py` & `deeploy-1.37.4/deeploy/services/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/models/sklearn.py` & `deeploy-1.37.4/deeploy/services/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/models/tensorflow.py` & `deeploy-1.37.4/deeploy/services/models/tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy/services/models/xgboost.py` & `deeploy-1.37.4/deeploy/services/models/xgboost.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/deeploy.egg-info/PKG-INFO` & `deeploy-1.37.4/deeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 1.37.3
+Version: 1.37.4
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-1.37.3/deeploy.egg-info/SOURCES.txt` & `deeploy-1.37.4/deeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.3/setup.py` & `deeploy-1.37.4/setup.py`

 * *Files identical despite different names*

