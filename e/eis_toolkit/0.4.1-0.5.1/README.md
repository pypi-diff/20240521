# Comparing `tmp/eis_toolkit-0.4.1.tar.gz` & `tmp/eis_toolkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis_toolkit-0.4.1.tar", max compression
+gzip compressed data, was "eis_toolkit-0.5.1.tar", max compression
```

## Comparing `eis_toolkit-0.4.1.tar` & `eis_toolkit-0.5.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.4.1/LICENSE
--rwxr-xr-x   0        0        0     5864 2024-04-24 11:26:53.983156 eis_toolkit-0.4.1/README.md
--rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.4.1/eis_toolkit/__init__.py
--rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.4.1/eis_toolkit/__main__.py
--rw-r--r--   0        0        0   101955 2024-04-29 07:18:52.216497 eis_toolkit-0.4.1/eis_toolkit/cli.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/conversions/__init__.py
--rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.4.1/eis_toolkit/conversions/csv_to_geodataframe.py
--rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-0.4.1/eis_toolkit/conversions/raster_to_dataframe.py
--rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/__init__.py
--rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/calculate_base_metrics.py
--rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/classification_label_evaluation.py
--rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/classification_probability_evaluation.py
--rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_confusion_matrix.py
--rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_nn_model_performance.py
--rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_prediction_area_curves.py
--rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_rate_curve.py
--rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-0.4.1/eis_toolkit/evaluation/scoring.py
--rw-r--r--   0        0        0     2643 2024-02-22 09:12:29.156927 eis_toolkit-0.4.1/eis_toolkit/exceptions.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/__init__.py
--rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
--rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/chi_square_test.py
--rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/correlation_matrix.py
--rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/covariance_matrix.py
--rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/dbscan.py
--rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py
--rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/feature_importance.py
--rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/k_means_cluster.py
--rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/local_morans_i.py
--rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/normality_test.py
--rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py
--rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/pca.py
--rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/plot_utils.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/prediction/__init__.py
--rw-r--r--   0        0        0     5228 2024-04-29 06:12:57.053049 eis_toolkit-0.4.1/eis_toolkit/prediction/fuzzy_overlay.py
--rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.4.1/eis_toolkit/prediction/gradient_boosting.py
--rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.4.1/eis_toolkit/prediction/logistic_regression.py
--rw-r--r--   0        0        0    13336 2024-04-29 05:55:02.267130 eis_toolkit-0.4.1/eis_toolkit/prediction/machine_learning_general.py
--rw-r--r--   0        0        0     1837 2024-04-25 10:25:47.565371 eis_toolkit-0.4.1/eis_toolkit/prediction/machine_learning_predict.py
--rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.4.1/eis_toolkit/prediction/mlp.py
--rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.4.1/eis_toolkit/prediction/random_forests.py
--rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-0.4.1/eis_toolkit/prediction/weights_of_evidence.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/raster_processing/__init__.py
--rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/clipping.py
--rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/create_constant_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/__init__.py
--rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/classification.py
--rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/parameters.py
--rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
--rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/utilities.py
--rw-r--r--   0        0        0    10388 2024-04-29 07:18:52.216497 eis_toolkit-0.4.1/eis_toolkit/raster_processing/distance_to_anomaly.py
--rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/extract_values_from_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/__init__.py
--rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/focal.py
--rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/kernels.py
--rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/speckle.py
--rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/utilities.py
--rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.4.1/eis_toolkit/raster_processing/reclassify.py
--rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/raster_processing/reprojecting.py
--rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/raster_processing/resampling.py
--rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.4.1/eis_toolkit/raster_processing/snapping.py
--rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/raster_processing/unifying.py
--rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/unique_combinations.py
--rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.4.1/eis_toolkit/raster_processing/windowing.py
--rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/training_data_tools/__init__.py
--rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/training_data_tools/class_balancing.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/transformations/__init__.py
--rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.4.1/eis_toolkit/transformations/binarize.py
--rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/clip.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/__init__.py
--rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/alr.py
--rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/clr.py
--rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/ilr.py
--rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/pairwise.py
--rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/plr.py
--rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/linear.py
--rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/logarithmic.py
--rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/one_hot_encoding.py
--rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/sigmoid.py
--rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.4.1/eis_toolkit/transformations/winsorize.py
--rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.4.1/eis_toolkit/utilities/__init__.py
--rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.4.1/eis_toolkit/utilities/aitchison_geometry.py
--rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/compositional.py
--rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/dataframe.py
--rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/geometry.py
--rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/parameter.py
--rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/raster.py
--rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/conversions.py
--rw-r--r--   0        0        0     8640 2024-04-24 06:18:14.118407 eis_toolkit-0.4.1/eis_toolkit/utilities/file_io.py
--rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-0.4.1/eis_toolkit/utilities/miscellaneous.py
--rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-0.4.1/eis_toolkit/utilities/nodata.py
--rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-0.4.1/eis_toolkit/utilities/raster.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/vector_processing/__init__.py
--rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.4.1/eis_toolkit/vector_processing/calculate_geometry.py
--rw-r--r--   0        0        0    22658 2024-02-22 09:12:29.168927 eis_toolkit-0.4.1/eis_toolkit/vector_processing/cell_based_association.py
--rw-r--r--   0        0        0     3240 2024-04-29 07:18:52.216497 eis_toolkit-0.4.1/eis_toolkit/vector_processing/distance_computation.py
--rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.4.1/eis_toolkit/vector_processing/extract_shared_lines.py
--rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-0.4.1/eis_toolkit/vector_processing/idw_interpolation.py
--rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-0.4.1/eis_toolkit/vector_processing/kriging_interpolation.py
--rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-0.4.1/eis_toolkit/vector_processing/rasterize_vector.py
--rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.4.1/eis_toolkit/vector_processing/reproject_vector.py
--rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-0.4.1/eis_toolkit/vector_processing/vector_density.py
--rwxr-xr-x   0        0        0     1778 2024-04-29 07:41:48.254374 eis_toolkit-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 eis_toolkit-0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0     5864 2024-05-13 10:15:39.840704 eis_toolkit-0.5.1/README.md
+-rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.5.1/eis_toolkit/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.5.1/eis_toolkit/__main__.py
+-rw-r--r--   0        0        0   115903 2024-05-21 06:37:53.189336 eis_toolkit-0.5.1/eis_toolkit/cli.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/conversions/__init__.py
+-rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.5.1/eis_toolkit/conversions/csv_to_geodataframe.py
+-rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-0.5.1/eis_toolkit/conversions/raster_to_dataframe.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/__init__.py
+-rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/calculate_base_metrics.py
+-rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_label_evaluation.py
+-rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_probability_evaluation.py
+-rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_confusion_matrix.py
+-rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_nn_model_performance.py
+-rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_prediction_area_curves.py
+-rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_rate_curve.py
+-rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-0.5.1/eis_toolkit/evaluation/scoring.py
+-rw-r--r--   0        0        0     2739 2024-05-21 06:37:53.189336 eis_toolkit-0.5.1/eis_toolkit/exceptions.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/__init__.py
+-rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
+-rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/chi_square_test.py
+-rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/correlation_matrix.py
+-rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/covariance_matrix.py
+-rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/dbscan.py
+-rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py
+-rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/feature_importance.py
+-rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/k_means_cluster.py
+-rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/local_morans_i.py
+-rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/normality_test.py
+-rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py
+-rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/pca.py
+-rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/plot_utils.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/prediction/__init__.py
+-rw-r--r--   0        0        0     5350 2024-04-30 08:53:14.418579 eis_toolkit-0.5.1/eis_toolkit/prediction/fuzzy_overlay.py
+-rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.5.1/eis_toolkit/prediction/gradient_boosting.py
+-rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.5.1/eis_toolkit/prediction/logistic_regression.py
+-rw-r--r--   0        0        0    16273 2024-05-20 10:32:28.957217 eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_general.py
+-rw-r--r--   0        0        0     3251 2024-05-21 06:37:53.189336 eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_predict.py
+-rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.5.1/eis_toolkit/prediction/mlp.py
+-rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.5.1/eis_toolkit/prediction/random_forests.py
+-rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-0.5.1/eis_toolkit/prediction/weights_of_evidence.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/raster_processing/__init__.py
+-rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/clipping.py
+-rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/create_constant_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/__init__.py
+-rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/classification.py
+-rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/parameters.py
+-rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
+-rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/utilities.py
+-rw-r--r--   0        0        0    10388 2024-04-29 09:13:31.923148 eis_toolkit-0.5.1/eis_toolkit/raster_processing/distance_to_anomaly.py
+-rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/extract_values_from_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/__init__.py
+-rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/focal.py
+-rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/kernels.py
+-rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/speckle.py
+-rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/utilities.py
+-rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.5.1/eis_toolkit/raster_processing/reclassify.py
+-rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/raster_processing/reprojecting.py
+-rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/raster_processing/resampling.py
+-rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.5.1/eis_toolkit/raster_processing/snapping.py
+-rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/raster_processing/unifying.py
+-rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/unique_combinations.py
+-rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.5.1/eis_toolkit/raster_processing/windowing.py
+-rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/training_data_tools/__init__.py
+-rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/training_data_tools/class_balancing.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/transformations/__init__.py
+-rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.5.1/eis_toolkit/transformations/binarize.py
+-rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/clip.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/__init__.py
+-rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/alr.py
+-rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/clr.py
+-rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/ilr.py
+-rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/pairwise.py
+-rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/plr.py
+-rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/linear.py
+-rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/logarithmic.py
+-rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/one_hot_encoding.py
+-rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/sigmoid.py
+-rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.5.1/eis_toolkit/transformations/winsorize.py
+-rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.5.1/eis_toolkit/utilities/__init__.py
+-rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.5.1/eis_toolkit/utilities/aitchison_geometry.py
+-rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/compositional.py
+-rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/dataframe.py
+-rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/geometry.py
+-rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/parameter.py
+-rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/raster.py
+-rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/conversions.py
+-rw-r--r--   0        0        0     8640 2024-05-03 06:58:41.674662 eis_toolkit-0.5.1/eis_toolkit/utilities/file_io.py
+-rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-0.5.1/eis_toolkit/utilities/miscellaneous.py
+-rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-0.5.1/eis_toolkit/utilities/nodata.py
+-rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-0.5.1/eis_toolkit/utilities/raster.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/vector_processing/__init__.py
+-rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.5.1/eis_toolkit/vector_processing/calculate_geometry.py
+-rw-r--r--   0        0        0    22658 2024-02-22 09:12:29.168927 eis_toolkit-0.5.1/eis_toolkit/vector_processing/cell_based_association.py
+-rw-r--r--   0        0        0     3240 2024-05-02 10:42:43.425579 eis_toolkit-0.5.1/eis_toolkit/vector_processing/distance_computation.py
+-rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.5.1/eis_toolkit/vector_processing/extract_shared_lines.py
+-rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-0.5.1/eis_toolkit/vector_processing/idw_interpolation.py
+-rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-0.5.1/eis_toolkit/vector_processing/kriging_interpolation.py
+-rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-0.5.1/eis_toolkit/vector_processing/rasterize_vector.py
+-rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.5.1/eis_toolkit/vector_processing/reproject_vector.py
+-rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-0.5.1/eis_toolkit/vector_processing/vector_density.py
+-rwxr-xr-x   0        0        0     1778 2024-05-21 06:38:06.857439 eis_toolkit-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 eis_toolkit-0.5.1/PKG-INFO
```

### Comparing `eis_toolkit-0.4.1/LICENSE` & `eis_toolkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/README.md` & `eis_toolkit-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 EIS Toolkit is available in conda-forge and PyPI and can be installed with one of the following commands.
 
 ```console
 pip install eis_toolkit
 ```
 
 ```console
-conda-install -c conda-forge eis_toolkit
+conda install -c conda-forge eis_toolkit
 ```
 
 You can find the latest release of EIS Toolkit also in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a Python wheel. Just download the wheel and install with pip
 
 ```console
 pip install eis_toolkit-0.4.0-py3-none-any.whl
 ```
 
 > [!TIP]
-> GDAL installation can cause issues on various platforms, especially on Windows. If you have trouble installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
+> GDAL needs to be installed separately on Windows when using pip / PyPI. If you have trouble installing EIS Toolkit in a venv due to GDAL, you can download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
 
 
 ## Usage
 EIS Toolkit can be used in Python scripts, Jupyter notebooks or via the CLI. At the moment, most tools have their own module and are imported like this:
 ```python
 # In general
 from eis_toolkit.category.module import module_function
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ihsae3_t_/tmpi57aw4kc_TarContainer/0/1.md", line 6, column 35: Levels of opening and closing headings don't match*

```diff
@@ -15,58 +15,59 @@
 (https://github.com/GispoCoding/eis_qgis_plugin). > [!NOTE] > This repository
 is still in development. Check the [wiki page of EIS Toolkit](https://
 github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap]
 (#roadmap) for more details about the project. ## Installation We recommend
 installing EIS Toolkit in an empty virtual environment to ensure compatibility
 between package versions. EIS Toolkit is available in conda-forge and PyPI and
 can be installed with one of the following commands. ```console pip install
-eis_toolkit ``` ```console conda-install -c conda-forge eis_toolkit ``` You can
+eis_toolkit ``` ```console conda install -c conda-forge eis_toolkit ``` You can
 find the latest release of EIS Toolkit also in the [releases page](https://
 github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a
 Python wheel. Just download the wheel and install with pip ```console pip
-install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL installation can
-cause issues on various platforms, especially on Windows. If you have trouble
-installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel
-(for example from [this repository](https://github.com/cgohlke/geospatial-
-wheels/releases)), install it first, and then attempt to install EIS Toolkit
-again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter notebooks or
-via the CLI. At the moment, most tools have their own module and are imported
-like this: ```python # In general from eis_toolkit.category.module import
-module_function # Some examples from eis_toolkit.raster_processing.reprojecting
-import reproject_raster from eis_toolkit.exploratory_analyses.pca import
-compute_pca ``` You can find several Jupyter notebooks in this repostiory that
-demonstrate how tools of EIS Toolkit can be used. The documentation of EIS
-Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/). ### EIS
-QGIS Plugin For those that prefer using tools of EIS Toolkit via a graphical
-user interface, check [EIS QGIS Plugin](https://github.com/GispoCoding/
-eis_qgis_plugin). The plugin includes the main GUI application called EIS
-Wizard and all individual EIS Toolkit tools as QGIS processing algorithms. The
-plugin is developed by the same core team that develops EIS Toolkit. ### CLI
-EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line
-interface that serves as a common interface for integrating the toolkit with
-external applications, such as QGIS. However, it can be used directly too. To
-use the CLI, simply use the command ```console eis ``` or ```console eis --help
-``` to get started. However, please note that the CLI has been primarily
-designed to communicate with external programs and may feel clunky in direct
-use. ## Roadmap - Milestone 1: **Beta release 0.1** (November 2023). The
-toolkit should have the basic funtionalities required for a full MPM workflow.
-Official testing phase begins. The plugin will be still under active
-development. - Milestone 2: **Release 1.0** (April 2024). All features should
-be incorporated at this time and the toolkit useful for actual MPM work.
-Testing will continue, potential bugs will be fixed and the user experience
-refined. ## Contributing We welcome contributions to EIS Toolkit in various
-forms: - â¨ Developing new tools - ð Fixing bugs in the code - ð Bug and
-other reporting - ð¡ Feature suggestions To contribute with code or
-documentation, you'll need a local development environment and a copy of the
-repository. Please refer to the **For developers** section below for detailed
-setup instructions. If you're interested in bug reporting or making feature
-suggestions, you can familiarize yourself with the toolkit and test it as
-described in the **Usage** section. When you encounter bugs or have ideas for
-new features, you can create an issue in this repository. ### For developers
-All contributing developers need Git and a copy of the repository. ```console
-git clone https://github.com/GispoCoding/eis_toolkit.git ``` After this you
-have three options for setting up your local development environment. 1. Docker
-- [instructions](./instructions/dev_setup_with_docker.md) 2. Poetry -
-[instructions](./instructions/dev_setup_without_docker.md) 3. Conda -
-[instructions](./instructions/dev_setup_without_docker_with_conda.md) *For
-general contributing guidelines, see [CONTRIBUTING](./CONTRIBUTING.md).* ##
-License Licensed under the EUPL-1.2 or later.
+install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL needs to be
+installed separately on Windows when using pip / PyPI. If you have trouble
+installing EIS Toolkit in a venv due to GDAL, you can download a compatible
+GDAL wheel (for example from [this repository](https://github.com/cgohlke/
+geospatial-wheels/releases)), install it first, and then attempt to install EIS
+Toolkit again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter
+notebooks or via the CLI. At the moment, most tools have their own module and
+are imported like this: ```python # In general from eis_toolkit.category.module
+import module_function # Some examples from
+eis_toolkit.raster_processing.reprojecting import reproject_raster from
+eis_toolkit.exploratory_analyses.pca import compute_pca ``` You can find
+several Jupyter notebooks in this repostiory that demonstrate how tools of EIS
+Toolkit can be used. The documentation of EIS Toolkit can be read [here](https:
+//gispocoding.github.io/eis_toolkit/). ### EIS QGIS Plugin For those that
+prefer using tools of EIS Toolkit via a graphical user interface, check [EIS
+QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin
+includes the main GUI application called EIS Wizard and all individual EIS
+Toolkit tools as QGIS processing algorithms. The plugin is developed by the
+same core team that develops EIS Toolkit. ### CLI EIS Toolkit includes a
+[Typer](https://typer.tiangolo.com/) command-line interface that serves as a
+common interface for integrating the toolkit with external applications, such
+as QGIS. However, it can be used directly too. To use the CLI, simply use the
+command ```console eis ``` or ```console eis --help ``` to get started.
+However, please note that the CLI has been primarily designed to communicate
+with external programs and may feel clunky in direct use. ## Roadmap -
+Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the
+basic funtionalities required for a full MPM workflow. Official testing phase
+begins. The plugin will be still under active development. - Milestone 2:
+**Release 1.0** (April 2024). All features should be incorporated at this time
+and the toolkit useful for actual MPM work. Testing will continue, potential
+bugs will be fixed and the user experience refined. ## Contributing We welcome
+contributions to EIS Toolkit in various forms: - â¨ Developing new tools -
+ð Fixing bugs in the code - ð Bug and other reporting - ð¡ Feature
+suggestions To contribute with code or documentation, you'll need a local
+development environment and a copy of the repository. Please refer to the **For
+developers** section below for detailed setup instructions. If you're
+interested in bug reporting or making feature suggestions, you can familiarize
+yourself with the toolkit and test it as described in the **Usage** section.
+When you encounter bugs or have ideas for new features, you can create an issue
+in this repository. ### For developers All contributing developers need Git and
+a copy of the repository. ```console git clone https://github.com/GispoCoding/
+eis_toolkit.git ``` After this you have three options for setting up your local
+development environment. 1. Docker - [instructions](./instructions/
+dev_setup_with_docker.md) 2. Poetry - [instructions](./instructions/
+dev_setup_without_docker.md) 3. Conda - [instructions](./instructions/
+dev_setup_without_docker_with_conda.md) *For general contributing guidelines,
+see [CONTRIBUTING](./CONTRIBUTING.md).* ## License Licensed under the EUPL-1.2
+or later.
```

### Comparing `eis_toolkit-0.4.1/eis_toolkit/cli.py` & `eis_toolkit-0.5.1/eis_toolkit/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -718,18 +718,22 @@
     typer.echo("Progress: 10%")
 
     with rasterio.open(input_file) as raster:
         typer.echo("Progress: 25%")
         results_dict = descriptive_statistics_raster(raster)
     typer.echo("Progress: 75%")
 
-    json_str = json.dumps(results_dict)
-    typer.echo("Progress: 100%")
-    typer.echo(f"Results: {json_str}")
-    typer.echo("Descriptive statistics (raster) completed")
+    # json_str = json.dumps(results_dict)
+    typer.echo("Progress: 100%\n")
+    # typer.echo(f"Results: {json_str}")
+    # typer.echo("Results:\n")
+    for key, value in results_dict.items():
+        typer.echo(f"{key}: {value}")
+
+    typer.echo("\nDescriptive statistics (raster) completed")
 
 
 # DESCRIPTIVE STATISTICS (VECTOR)
 @app.command()
 def descriptive_statistics_vector_cli(input_file: INPUT_FILE_OPTION, column: str = None):
     """Generate descriptive statistics from vector or tabular data."""
     from eis_toolkit.exploratory_analyses.descriptive_statistics import descriptive_statistics_dataframe
@@ -2305,92 +2309,184 @@
     json_str = json.dumps(metrics_dict)
     typer.echo("Progress: 100%")
     typer.echo(f"Results: {json_str}")
 
     typer.echo("Gradient boosting regressor training completed")
 
 
-# EVALUATE ML MODEL
+# TEST CLASSIFIER ML MODEL
 @app.command()
-def evaluate_trained_model_cli(
+def classifier_test_cli(
+    input_rasters: INPUT_FILES_ARGUMENT,
+    target_labels: INPUT_FILE_OPTION,
+    model_file: INPUT_FILE_OPTION,
+    output_raster_probability: OUTPUT_FILE_OPTION,
+    output_raster_classified: OUTPUT_FILE_OPTION,
+    classification_threshold: float = 0.5,
+    test_metrics: Annotated[List[ClassifierMetrics], typer.Option(case_sensitive=False)] = [ClassifierMetrics.accuracy],
+):
+    """Test trained machine learning classifier model by predicting and scoring."""
+    from eis_toolkit.evaluation.scoring import score_predictions
+    from eis_toolkit.prediction.machine_learning_general import load_model, prepare_data_for_ml, reshape_predictions
+    from eis_toolkit.prediction.machine_learning_predict import predict_classifier
+
+    X, y, reference_profile, nodata_mask = prepare_data_for_ml(input_rasters, target_labels)
+    typer.echo("Progress: 30%")
+
+    model = load_model(model_file)
+    predictions, probabilities = predict_classifier(X, model, classification_threshold, True)
+    probabilities_reshaped = reshape_predictions(
+        probabilities, reference_profile["height"], reference_profile["width"], nodata_mask
+    )
+    predictions_reshaped = reshape_predictions(
+        predictions, reference_profile["height"], reference_profile["width"], nodata_mask
+    )
+
+    metrics_dict = score_predictions(y, predictions, get_enum_values(test_metrics))
+    typer.echo("Progress: 80%")
+
+    out_profile = reference_profile.copy()
+    out_profile.update({"count": 1, "dtype": np.float32})
+
+    with rasterio.open(output_raster_probability, "w", **out_profile) as dst:
+        dst.write(probabilities_reshaped, 1)
+    with rasterio.open(output_raster_classified, "w", **out_profile) as dst:
+        dst.write(predictions_reshaped, 1)
+
+    typer.echo("\n")
+    for key, value in metrics_dict.items():
+        typer.echo(f"{key}: {value}")
+    typer.echo("\n")
+
+    typer.echo("Progress: 100%")
+    typer.echo(
+        (
+            "Testing classifier model completed, writing rasters to "
+            f"{output_raster_probability} and {output_raster_classified}."
+        )
+    )
+
+
+# TEST REGRESSOR ML MODEL
+@app.command()
+def regressor_test_cli(
     input_rasters: INPUT_FILES_ARGUMENT,
     target_labels: INPUT_FILE_OPTION,
     model_file: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
-    validation_metrics: Annotated[List[str], typer.Option()],
+    test_metrics: Annotated[List[RegressorMetrics], typer.Option(case_sensitive=False)] = [RegressorMetrics.mse],
 ):
-    """Train and optionally validate a Gradient boosting regressor model using Sklearn."""
-    from eis_toolkit.prediction.machine_learning_general import (
-        evaluate_model,
-        load_model,
-        prepare_data_for_ml,
-        reshape_predictions,
-    )
+    """Test trained machine learning regressor model by predicting and scoring."""
+    from eis_toolkit.evaluation.scoring import score_predictions
+    from eis_toolkit.prediction.machine_learning_general import load_model, prepare_data_for_ml, reshape_predictions
+    from eis_toolkit.prediction.machine_learning_predict import predict_regressor
 
     X, y, reference_profile, nodata_mask = prepare_data_for_ml(input_rasters, target_labels)
-
     typer.echo("Progress: 30%")
 
     model = load_model(model_file)
-    predictions, metrics_dict = evaluate_model(X, y, model, validation_metrics)
+    predictions = predict_regressor(X, model)
     predictions_reshaped = reshape_predictions(
         predictions, reference_profile["height"], reference_profile["width"], nodata_mask
     )
 
+    metrics_dict = score_predictions(y, predictions, get_enum_values(test_metrics))
     typer.echo("Progress: 80%")
 
-    json_str = json.dumps(metrics_dict)
-
     out_profile = reference_profile.copy()
-    out_profile.update({"count": 1, "dtype": predictions_reshaped.dtype})
+    out_profile.update({"count": 1, "dtype": np.float32})
 
     with rasterio.open(output_raster, "w", **out_profile) as dst:
         dst.write(predictions_reshaped, 1)
 
-    typer.echo("Progress: 100%")
-    typer.echo(f"Results: {json_str}")
+    typer.echo("\n")
+    for key, value in metrics_dict.items():
+        typer.echo(f"{key}: {value}")
+    typer.echo("\n")
+
+    typer.echo("Progress: 100%\n")
+
+    typer.echo(f"Testing regressor model completed, writing raster to {output_raster}.")
+
+
+# PREDICT WITH TRAINED ML MODEL
+@app.command()
+def classifier_predict_cli(
+    input_rasters: INPUT_FILES_ARGUMENT,
+    model_file: INPUT_FILE_OPTION,
+    output_raster_probability: OUTPUT_FILE_OPTION,
+    output_raster_classified: OUTPUT_FILE_OPTION,
+    classification_threshold: float = 0.5,
+):
+    """Predict with a trained machine learning classifier model."""
+    from eis_toolkit.prediction.machine_learning_general import load_model, prepare_data_for_ml, reshape_predictions
+    from eis_toolkit.prediction.machine_learning_predict import predict_classifier
+
+    X, _, reference_profile, nodata_mask = prepare_data_for_ml(input_rasters)
 
-    typer.echo("Evaluating trained model completed")
+    typer.echo("Progress: 30%")
+
+    model = load_model(model_file)
+    predictions, probabilities = predict_classifier(X, model, classification_threshold, True)
+    probabilities_reshaped = reshape_predictions(
+        probabilities, reference_profile["height"], reference_profile["width"], nodata_mask
+    )
+    predictions_reshaped = reshape_predictions(
+        predictions, reference_profile["height"], reference_profile["width"], nodata_mask
+    )
+    typer.echo("Progress: 80%")
+
+    out_profile = reference_profile.copy()
+    out_profile.update({"count": 1, "dtype": np.float32})
+
+    with rasterio.open(output_raster_probability, "w", **out_profile) as dst:
+        dst.write(probabilities_reshaped, 1)
+    with rasterio.open(output_raster_classified, "w", **out_profile) as dst:
+        dst.write(predictions_reshaped, 1)
+
+    typer.echo("Progress: 100%")
+    typer.echo(
+        (
+            "Predicting with classifier model completed, writing rasters to "
+            f"{output_raster_probability} and {output_raster_classified}."
+        )
+    )
 
 
 # PREDICT WITH TRAINED ML MODEL
 @app.command()
-def predict_with_trained_model_cli(
+def regressor_predict_cli(
     input_rasters: INPUT_FILES_ARGUMENT,
     model_file: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
 ):
-    """Train and optionally validate a Gradient boosting regressor model using Sklearn."""
-    from eis_toolkit.prediction.machine_learning_general import (
-        load_model,
-        predict,
-        prepare_data_for_ml,
-        reshape_predictions,
-    )
+    """Predict with a trained machine learning regressor model."""
+    from eis_toolkit.prediction.machine_learning_general import load_model, prepare_data_for_ml, reshape_predictions
+    from eis_toolkit.prediction.machine_learning_predict import predict_regressor
 
     X, _, reference_profile, nodata_mask = prepare_data_for_ml(input_rasters)
 
     typer.echo("Progress: 30%")
 
     model = load_model(model_file)
-    predictions = predict(X, model)
+    predictions = predict_regressor(X, model)
     predictions_reshaped = reshape_predictions(
         predictions, reference_profile["height"], reference_profile["width"], nodata_mask
     )
 
     typer.echo("Progress: 80%")
 
     out_profile = reference_profile.copy()
-    out_profile.update({"count": 1, "dtype": predictions_reshaped.dtype})
+    out_profile.update({"count": 1, "dtype": np.float32})
 
     with rasterio.open(output_raster, "w", **out_profile) as dst:
         dst.write(predictions_reshaped, 1)
 
     typer.echo("Progress: 100%")
-    typer.echo("Predicting completed")
+    typer.echo(f"Predicting with regressor model completed, writing raster to {output_raster}.")
 
 
 # FUZZY OVERLAYS
 
 # AND OVERLAY
 @app.command()
 def and_overlay_cli(
@@ -2963,15 +3059,287 @@
         dst.write(out_image)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Winsorize transform completed, writing raster to {output_raster}.")
 
 
 # ---EVALUATION ---
-# TODO
+
+
+@app.command()
+def summarize_probability_metrics_cli(true_labels: INPUT_FILE_OPTION, probabilities: INPUT_FILE_OPTION):
+    """
+    Generate a comprehensive report of various evaluation metrics for classification probabilities.
+
+    The output includes ROC AUC, log loss, average precision and Brier score loss.
+    """
+    from eis_toolkit.evaluation.classification_probability_evaluation import summarize_probability_metrics
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
+    typer.echo("Progress: 25%")
+
+    results_dict = summarize_probability_metrics(y_true=y_true, y_prob=y_prob)
+
+    typer.echo("Progress: 75%")
+
+    # json_str = json.dumps(results_dict)
+    typer.echo("Progress: 100% \n")
+    # typer.echo("Results:\n")
+    for key, value in results_dict.items():
+        typer.echo(f"{key}: {value}")
+    # typer.echo(f"Results: {json_str}")
+    typer.echo("\nGenerating probability metrics summary completed.")
+
+
+@app.command()
+def summarize_label_metrics_binary_cli(true_labels: INPUT_FILE_OPTION, predictions: INPUT_FILE_OPTION):
+    """
+    Generate a comprehensive report of various evaluation metrics for binary classification results.
+
+    The output includes accuracy, precision, recall, F1 scores and confusion matrix elements
+    (true negatives, false positives, false negatives, true positives).
+    """
+    from eis_toolkit.evaluation.classification_label_evaluation import summarize_label_metrics_binary
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_pred, y_true), _, _ = read_data_for_evaluation([predictions, true_labels])
+    typer.echo("Progress: 25%")
+
+    results_dict = summarize_label_metrics_binary(y_true=y_true, y_pred=y_pred)
+    typer.echo("Progress: 75%")
+
+    # json_str = json.dumps(results_dict)
+    typer.echo("Progress: 100% \n")
+    for key, value in results_dict.items():
+        typer.echo(f"{key}: {value}")
+    # typer.echo(f"Results: {json_str}")
+    typer.echo("\n Generating prediction label metrics summary completed.")
+
+
+@app.command()
+def plot_roc_curve_cli(
+    true_labels: INPUT_FILE_OPTION,
+    probabilities: INPUT_FILE_OPTION,
+    output_file: OUTPUT_FILE_OPTION,
+    show_plot: bool = False,
+    save_dpi: Optional[int] = None,
+):
+    """
+    Plot ROC (receiver operating characteristic) curve.
+
+    ROC curve is a binary classification multi-threshold metric. The ideal performance corner of the plot
+    is top-left. AUC of the ROC curve summarizes model performance across different classification thresholds.
+    """
+    import matplotlib.pyplot as plt
+
+    from eis_toolkit.evaluation.classification_probability_evaluation import plot_roc_curve
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
+    typer.echo("Progress: 25%")
+
+    _ = plot_roc_curve(y_true=y_true, y_prob=y_prob)
+    typer.echo("Progress: 75%")
+    if show_plot:
+        plt.show()
+
+    if output_file is not None:
+        dpi = "figure" if save_dpi is None else save_dpi
+        plt.savefig(output_file, dpi=dpi)
+        echo_str_end = f", output figure saved to {output_file}."
+    typer.echo("Progress: 100% \n")
+
+    typer.echo("ROC curve plot completed" + echo_str_end)
+
+
+@app.command()
+def plot_det_curve_cli(
+    true_labels: INPUT_FILE_OPTION,
+    probabilities: INPUT_FILE_OPTION,
+    output_file: OUTPUT_FILE_OPTION,
+    show_plot: bool = False,
+    save_dpi: Optional[int] = None,
+):
+    """
+    Plot DET (detection error tradeoff) curve.
+
+    DET curve is a binary classification multi-threshold metric. DET curves are a variation of ROC curves where
+    False Negative Rate is plotted on the y-axis instead of True Positive Rate. The ideal performance corner of
+    the plot is bottom-left. When comparing the performance of different models, DET curves can be
+    slightly easier to assess visually than ROC curves.
+    """
+    import matplotlib.pyplot as plt
+
+    from eis_toolkit.evaluation.classification_probability_evaluation import plot_det_curve
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
+    typer.echo("Progress: 25%")
+
+    _ = plot_det_curve(y_true=y_true, y_prob=y_prob)
+    typer.echo("Progress: 75%")
+    if show_plot:
+        plt.show()
+
+    if output_file is not None:
+        dpi = "figure" if save_dpi is None else save_dpi
+        plt.savefig(output_file, dpi=dpi)
+        echo_str_end = f", output figure saved to {output_file}."
+    typer.echo("Progress: 100% \n")
+
+    typer.echo("DET curve plot completed" + echo_str_end)
+
+
+@app.command()
+def plot_precision_recall_curve_cli(
+    true_labels: INPUT_FILE_OPTION,
+    probabilities: INPUT_FILE_OPTION,
+    output_file: OUTPUT_FILE_OPTION,
+    show_plot: bool = False,
+    save_dpi: Optional[int] = None,
+):
+    """
+    Plot precision-recall curve.
+
+    Precision-recall curve is a binary classification multi-threshold metric. Precision-recall curve shows
+    the tradeoff between precision and recall for different classification thresholds.
+    It can be a useful measure of success when classes are imbalanced.
+    """
+    import matplotlib.pyplot as plt
+
+    from eis_toolkit.evaluation.classification_probability_evaluation import plot_precision_recall_curve
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
+    typer.echo("Progress: 25%")
+
+    _ = plot_precision_recall_curve(y_true=y_true, y_prob=y_prob)
+    typer.echo("Progress: 75%")
+    if show_plot:
+        plt.show()
+
+    if output_file is not None:
+        dpi = "figure" if save_dpi is None else save_dpi
+        plt.savefig(output_file, dpi=dpi)
+        echo_str_end = f", output figure saved to {output_file}."
+    typer.echo("Progress: 100% \n")
+
+    typer.echo("Precision-Recall curve plot completed" + echo_str_end)
+
+
+@app.command()
+def plot_calibration_curve_cli(
+    true_labels: INPUT_FILE_OPTION,
+    probabilities: INPUT_FILE_OPTION,
+    output_file: OUTPUT_FILE_OPTION,
+    n_bins: int = 5,
+    show_plot: bool = False,
+    save_dpi: Optional[int] = None,
+):
+    """
+    Plot calibration curve (aka realibity diagram).
+
+    Calibration curve has the frequency of the positive labels on the y-axis and the predicted probability on
+    the x-axis. Generally, the close the calibration curve is to line x=y, the better the model is calibrated.
+    """
+    import matplotlib.pyplot as plt
+
+    from eis_toolkit.evaluation.classification_probability_evaluation import plot_calibration_curve
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
+    typer.echo("Progress: 25%")
+
+    _ = plot_calibration_curve(y_true=y_true, y_prob=y_prob, n_bins=n_bins)
+    typer.echo("Progress: 75%")
+    if show_plot:
+        plt.show()
+
+    if output_file is not None:
+        dpi = "figure" if save_dpi is None else save_dpi
+        plt.savefig(output_file, dpi=dpi)
+        echo_str_end = f", output figure saved to {output_file}."
+    typer.echo("Progress: 100% \n")
+
+    typer.echo("Calibration curve plot completed" + echo_str_end)
+
+
+@app.command()
+def plot_confusion_matrix_cli(
+    true_labels: INPUT_FILE_OPTION,
+    predictions: INPUT_FILE_OPTION,
+    output_file: OUTPUT_FILE_OPTION,
+    show_plot: bool = False,
+    save_dpi: Optional[int] = None,
+):
+    """Plot confusion matrix to visualize classification results."""
+    import matplotlib.pyplot as plt
+    from sklearn.metrics import confusion_matrix
+
+    from eis_toolkit.evaluation.plot_confusion_matrix import plot_confusion_matrix
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_pred, y_true), _, _ = read_data_for_evaluation([predictions, true_labels])
+    typer.echo("Progress: 25%")
+
+    matrix = confusion_matrix(y_true, y_pred)
+    _ = plot_confusion_matrix(confusion_matrix=matrix)
+    typer.echo("Progress: 75%")
+    if show_plot:
+        plt.show()
+
+    if output_file is not None:
+        dpi = "figure" if save_dpi is None else save_dpi
+        plt.savefig(output_file, dpi=dpi)
+        echo_str_end = f", output figure saved to {output_file}."
+    typer.echo("Progress: 100% \n")
+
+    typer.echo("Confusion matrix plot completed" + echo_str_end)
+
+
+@app.command()
+def score_predictions_cli(
+    true_labels: INPUT_FILE_OPTION,
+    predictions: INPUT_FILE_OPTION,
+    metrics: Annotated[List[str], typer.Option()],
+):
+    """Score predictions."""
+    from eis_toolkit.evaluation.scoring import score_predictions
+    from eis_toolkit.prediction.machine_learning_general import read_data_for_evaluation
+
+    typer.echo("Progress: 10%")
+
+    (y_pred, y_true), _, _ = read_data_for_evaluation([predictions, true_labels])
+    typer.echo("Progress: 25%")
+
+    outputs = score_predictions(y_true, y_pred, metrics)
+    typer.echo("Progress: 100% \n")
+
+    if isinstance(outputs, dict):
+        for key, value in outputs.items():
+            typer.echo(f"{key}: {value}")
+    else:
+        typer.echo(outputs)
+
+    typer.echo("\nScoring predictions completed.")
 
 
 # --- UTILITIES ---
 @app.command()
 def split_raster_bands_cli(input_raster: INPUT_FILE_OPTION, output_dir: OUTPUT_DIR_OPTION):  # CHECK
     """Split multiband raster into singleband rasters."""
     from eis_toolkit.utilities.file_io import get_output_paths_from_common_name
```

### Comparing `eis_toolkit-0.4.1/eis_toolkit/conversions/csv_to_geodataframe.py` & `eis_toolkit-0.5.1/eis_toolkit/conversions/csv_to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/conversions/raster_to_dataframe.py` & `eis_toolkit-0.5.1/eis_toolkit/conversions/raster_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/calculate_base_metrics.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/calculate_base_metrics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/classification_label_evaluation.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_label_evaluation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/classification_probability_evaluation.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_probability_evaluation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_confusion_matrix.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_nn_model_performance.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_nn_model_performance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_prediction_area_curves.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_prediction_area_curves.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_rate_curve.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_rate_curve.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/evaluation/scoring.py` & `eis_toolkit-0.5.1/eis_toolkit/evaluation/scoring.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exceptions.py` & `eis_toolkit-0.5.1/eis_toolkit/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     """Exception error for invalid column index."""
 
 
 class InvalidDataShapeException(Exception):
     """Exception error for datasets with invalid shapes."""
 
 
+class InvalidModelTypeException(Exception):
+    """Exception error for invalid model type."""
+
+
 class InvalidParameterValueException(Exception):
     """Exception error class for invalid parameter values."""
 
 
 class InvalidRasterBandException(Exception):
     """Expection error class for invalid raster band selection."""
```

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/chi_square_test.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/chi_square_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/correlation_matrix.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/covariance_matrix.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/dbscan.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/dbscan.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/feature_importance.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/feature_importance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/k_means_cluster.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/k_means_cluster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/local_morans_i.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/local_morans_i.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/normality_test.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/normality_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/pca.py` & `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/pca.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/fuzzy_overlay.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/fuzzy_overlay.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         2D Numpy array with the result of the 'sum' overlay operation. Values are in range [0, 1].
 
     Raises:
         InvalidDatasetException: If input data contains less than two 2D Numpy arrays/raster bands.
         InvalidParameterValueException: If data values are not in range [0, 1].
     """
     data = _prepare_data_for_fuzzy_overlay(data)
-    return data.sum(axis=0) - np.prod(data, axis=0)
+    product_term = np.prod(1 - data, axis=0)
+    fuzzy_sum = 1 - product_term
+    return fuzzy_sum
 
 
 @beartype
 def gamma_overlay(data: Union[Sequence[np.ndarray], np.ndarray], gamma: float = 0.5) -> np.ndarray:
     """Compute a 'gamma' overlay operation with fuzzy logic.
 
     Args:
@@ -116,10 +118,11 @@
         InvalidDatasetException: If input data contains less than two 2D Numpy arrays/raster bands.
         InvalidParameterValueException: If data values or gamma are not in range [0, 1].
     """
     data = _prepare_data_for_fuzzy_overlay(data)
     if gamma < 0 or gamma > 1:
         raise InvalidParameterValueException("The gamma parameter must be in range [0, 1]")
 
-    product = np.prod(data, axis=0)
-    sum = data.sum(axis=0) - product
-    return product ** (1 - gamma) * sum**gamma
+    fuzzy_product = np.prod(data, axis=0)
+    product_term_for_sum = np.prod(1 - data, axis=0)
+    fuzzy_sum = 1 - product_term_for_sum
+    return fuzzy_product ** (1 - gamma) * fuzzy_sum**gamma
```

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/gradient_boosting.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/logistic_regression.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/machine_learning_general.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_general.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from beartype.typing import Any, List, Literal, Optional, Sequence, Tuple, Union
 from scipy import sparse
 from sklearn.base import BaseEstimator
 from sklearn.model_selection import KFold, LeaveOneOut, StratifiedKFold, train_test_split
 
 from eis_toolkit.evaluation.scoring import score_predictions
 from eis_toolkit.exceptions import (
+    InvalidDatasetException,
     InvalidParameterValueException,
     NonMatchingParameterLengthsException,
     NonMatchingRasterMetadataException,
 )
 from eis_toolkit.utilities.checks.raster import check_raster_grids
 from eis_toolkit.vector_processing.rasterize_vector import rasterize_vector
 
@@ -142,24 +143,29 @@
     Returns:
         Feature data (X) in prepared shape.
         Target labels (y) in prepared shape (if `label_file` was given).
         Refrence raster metadata .
         Nodata mask applied to X and y.
 
     Raises:
-        NonMatchingRasterMetadataException: Input feature rasters don't have same grid properties.
+        InvalidDatasetException: Input feature rasters contains only one path.
+        NonMatchingRasterMetadataException: Input feature rasters, and optionally rasterized label file,
+            don't have same grid properties.
     """
 
     def _read_and_stack_feature_raster(filepath: Union[str, os.PathLike]) -> Tuple[np.ndarray, dict]:
         """Read all bands of raster file with feature/evidence data in a stack."""
         with rasterio.open(filepath) as src:
             raster_data = np.stack([src.read(i) for i in range(1, src.count + 1)])
             profile = src.profile
         return raster_data, profile
 
+    if len(feature_raster_files) < 2:
+        raise InvalidDatasetException(f"Expected more than one feature raster file: {len(feature_raster_files)}.")
+
     # Read and stack feature rasters
     feature_data, profiles = zip(*[_read_and_stack_feature_raster(file) for file in feature_raster_files])
     if not check_raster_grids(profiles, same_extent=True):
         raise NonMatchingRasterMetadataException("Input feature rasters should have same grid properties.")
 
     reference_profile = profiles[0]
     nodata_values = [profile["nodata"] for profile in profiles]
@@ -168,17 +174,22 @@
     reshaped_data = []
     nodata_mask = None
 
     for raster, nodata in zip(feature_data, nodata_values):
         raster_reshaped = raster.reshape(raster.shape[0], -1).T
         reshaped_data.append(raster_reshaped)
 
+        nan_mask = (raster_reshaped == np.nan).any(axis=1)
+        combined_mask = nan_mask if nodata_mask is None else nodata_mask | nan_mask
+
         if nodata is not None:
             raster_mask = (raster_reshaped == nodata).any(axis=1)
-            nodata_mask = raster_mask if nodata_mask is None else nodata_mask | raster_mask
+            combined_mask = combined_mask | raster_mask
+
+        nodata_mask = combined_mask
 
     X = np.concatenate(reshaped_data, axis=1)
 
     if label_file is not None:
         # Check label file type and process accordingly
         file_extension = os.path.splitext(label_file)[1].lower()
 
@@ -187,14 +198,20 @@
             y = rasterize_vector(geodataframe=gpd.read_file(label_file), raster_profile=reference_profile)
 
         # Labels/deposits in raster format
         else:
             with rasterio.open(label_file) as label_raster:
                 y = label_raster.read(1)  # Assuming labels are in the first band
                 label_nodata = label_raster.nodata
+                profiles = list(profiles)
+                profiles.append(label_raster.profile)
+                if not check_raster_grids(profiles, same_extent=True):
+                    raise NonMatchingRasterMetadataException(
+                        "Label raster should have the same grid properties as feature rasters."
+                    )
 
             label_nodata_mask = y == label_nodata
 
             # Combine masks and apply to feature and label data
             nodata_mask = nodata_mask | label_nodata_mask.ravel()
 
         y = y.ravel()[~nodata_mask]
@@ -204,14 +221,77 @@
 
     X = X[~nodata_mask]
 
     return X, y, reference_profile, nodata_mask
 
 
 @beartype
+def read_data_for_evaluation(
+    rasters: Sequence[Union[str, os.PathLike]]
+) -> Tuple[Sequence[np.ndarray], rasterio.profiles.Profile, Any]:
+    """
+    Prepare data ready for evaluating modeling outputs.
+
+    Reads all rasters (only first band), reshapes them (flattens) and masks out all NaN
+    and nodata pixels by creating a combined mask from all input rasters.
+
+    Args:
+        rasters: List of filepaths of input rasters. Files should only include raster that have
+            the same grid properties and extent.
+
+    Returns:
+        List of reshaped and masked raster data.
+        Refrence raster profile.
+        Nodata mask applied to raster data.
+
+    Raises:
+        InvalidDatasetException: Input rasters contains only one path.
+        NonMatchingRasterMetadataException: Input rasters don't have same grid properties.
+    """
+    if len(rasters) < 2:
+        raise InvalidDatasetException(f"Expected more than one raster file: {len(rasters)}.")
+
+    profiles = []
+    raster_data = []
+    nodata_values = []
+
+    for raster in rasters:
+        with rasterio.open(raster) as src:
+            data = src.read(1)
+            profile = src.profile
+            profiles.append(profile)
+            raster_data.append(data)
+            nodata_values.append(profile.get("nodata"))
+
+    if not check_raster_grids(profiles, same_extent=True):
+        raise NonMatchingRasterMetadataException(f"Input rasters should have the same grid properties: {profiles}.")
+
+    reference_profile = profiles[0]
+    nodata_mask = None
+
+    for data, nodata in zip(raster_data, nodata_values):
+        nan_mask = np.isnan(data)
+        combined_mask = nan_mask if nodata_mask is None else nodata_mask | nan_mask
+
+        if nodata is not None:
+            raster_mask = data == nodata
+            combined_mask = combined_mask | raster_mask
+
+        nodata_mask = combined_mask
+    nodata_mask = nodata_mask.flatten()
+
+    masked_data = []
+    for data in raster_data:
+        flattened_data = data.flatten()
+        masked_data.append(flattened_data[~nodata_mask])
+
+    return masked_data, reference_profile, nodata_mask
+
+
+@beartype
 def _train_and_validate_sklearn_model(
     X: Union[np.ndarray, pd.DataFrame],
     y: Union[np.ndarray, pd.Series],
     model: BaseEstimator,
     validation_method: Literal["split", "kfold_cv", "skfold_cv", "loo_cv", "none"],
     metrics: Sequence[Literal["mse", "rmse", "mae", "r2", "accuracy", "precision", "recall", "f1"]],
     split_size: float = 0.2,
```

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/mlp.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/mlp.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/random_forests.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/random_forests.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/prediction/weights_of_evidence.py` & `eis_toolkit-0.5.1/eis_toolkit/prediction/weights_of_evidence.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/clipping.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/clipping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/create_constant_raster.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/create_constant_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/classification.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/classification.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/parameters.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/parameters.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/utilities.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/distance_to_anomaly.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/distance_to_anomaly.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/extract_values_from_raster.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/extract_values_from_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/focal.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/focal.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/kernels.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/kernels.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/speckle.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/speckle.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/utilities.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/reclassify.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/reclassify.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/reprojecting.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/reprojecting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/resampling.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/resampling.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/snapping.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/snapping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/unifying.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/unifying.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/unique_combinations.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/unique_combinations.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/raster_processing/windowing.py` & `eis_toolkit-0.5.1/eis_toolkit/raster_processing/windowing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/training_data_tools/class_balancing.py` & `eis_toolkit-0.5.1/eis_toolkit/training_data_tools/class_balancing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/binarize.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/binarize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/clip.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/clip.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/alr.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/alr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/clr.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/clr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/ilr.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/ilr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/pairwise.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/pairwise.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/plr.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/plr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/linear.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/linear.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/logarithmic.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/logarithmic.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/one_hot_encoding.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/sigmoid.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/transformations/winsorize.py` & `eis_toolkit-0.5.1/eis_toolkit/transformations/winsorize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/aitchison_geometry.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/aitchison_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/compositional.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/compositional.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/dataframe.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/geometry.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/parameter.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/parameter.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/raster.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/conversions.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/conversions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/file_io.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/file_io.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/miscellaneous.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/nodata.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/nodata.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/utilities/raster.py` & `eis_toolkit-0.5.1/eis_toolkit/utilities/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/calculate_geometry.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/calculate_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/cell_based_association.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/cell_based_association.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/distance_computation.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/distance_computation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/extract_shared_lines.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/extract_shared_lines.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/idw_interpolation.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/idw_interpolation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/kriging_interpolation.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/kriging_interpolation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/rasterize_vector.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/rasterize_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/reproject_vector.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/reproject_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/eis_toolkit/vector_processing/vector_density.py` & `eis_toolkit-0.5.1/eis_toolkit/vector_processing/vector_density.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.1/pyproject.toml` & `eis_toolkit-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eis_toolkit"
-version = "0.4.1"
+version = "0.5.1"
 description = "EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union."
 authors = []
 maintainers = ["Gispo Ltd. <info@gispo.fi>"]
 license = "EUPL-1.2"
 readme = "README.md"
 homepage = "https://eis-he.eu"
 repository = "https://github.com/GispoCoding/eis_toolkit"
```

### Comparing `eis_toolkit-0.4.1/PKG-INFO` & `eis_toolkit-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis_toolkit
-Version: 0.4.1
+Version: 0.5.1
 Summary: EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union.
 Home-page: https://eis-he.eu
 License: EUPL-1.2
 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/Engineering :: GIS,Programming Language :: Python :: 3 :: Only
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 Requires-Python: >=3.9,<3.11
@@ -78,25 +78,25 @@
 EIS Toolkit is available in conda-forge and PyPI and can be installed with one of the following commands.
 
 ```console
 pip install eis_toolkit
 ```
 
 ```console
-conda-install -c conda-forge eis_toolkit
+conda install -c conda-forge eis_toolkit
 ```
 
 You can find the latest release of EIS Toolkit also in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a Python wheel. Just download the wheel and install with pip
 
 ```console
 pip install eis_toolkit-0.4.0-py3-none-any.whl
 ```
 
 > [!TIP]
-> GDAL installation can cause issues on various platforms, especially on Windows. If you have trouble installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
+> GDAL needs to be installed separately on Windows when using pip / PyPI. If you have trouble installing EIS Toolkit in a venv due to GDAL, you can download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
 
 
 ## Usage
 EIS Toolkit can be used in Python scripts, Jupyter notebooks or via the CLI. At the moment, most tools have their own module and are imported like this:
 ```python
 # In general
 from eis_toolkit.category.module import module_function
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ihsae3_t_/tmpi57aw4kc_TarContainer/0/103", line 41, column 35: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eis_toolkit Version: 0.4.1 Summary: EIS Toolkit is
+Metadata-Version: 2.1 Name: eis_toolkit Version: 0.5.1 Summary: EIS Toolkit is
 a comprehensive collection of tools suitable for mineral prospectivity mapping.
 This toolkit has been developed as part of the Exploration Information System
 project which has been funded by European Union. Home-page: https://eis-he.eu
 License: EUPL-1.2 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/
 Engineering :: GIS,Programming Language :: Python :: 3 :: Only Maintainer:
 Gispo Ltd. Maintainer-email: info@gispo.fi Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL
@@ -37,58 +37,59 @@
 (https://github.com/GispoCoding/eis_qgis_plugin). > [!NOTE] > This repository
 is still in development. Check the [wiki page of EIS Toolkit](https://
 github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap]
 (#roadmap) for more details about the project. ## Installation We recommend
 installing EIS Toolkit in an empty virtual environment to ensure compatibility
 between package versions. EIS Toolkit is available in conda-forge and PyPI and
 can be installed with one of the following commands. ```console pip install
-eis_toolkit ``` ```console conda-install -c conda-forge eis_toolkit ``` You can
+eis_toolkit ``` ```console conda install -c conda-forge eis_toolkit ``` You can
 find the latest release of EIS Toolkit also in the [releases page](https://
 github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a
 Python wheel. Just download the wheel and install with pip ```console pip
-install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL installation can
-cause issues on various platforms, especially on Windows. If you have trouble
-installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel
-(for example from [this repository](https://github.com/cgohlke/geospatial-
-wheels/releases)), install it first, and then attempt to install EIS Toolkit
-again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter notebooks or
-via the CLI. At the moment, most tools have their own module and are imported
-like this: ```python # In general from eis_toolkit.category.module import
-module_function # Some examples from eis_toolkit.raster_processing.reprojecting
-import reproject_raster from eis_toolkit.exploratory_analyses.pca import
-compute_pca ``` You can find several Jupyter notebooks in this repostiory that
-demonstrate how tools of EIS Toolkit can be used. The documentation of EIS
-Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/). ### EIS
-QGIS Plugin For those that prefer using tools of EIS Toolkit via a graphical
-user interface, check [EIS QGIS Plugin](https://github.com/GispoCoding/
-eis_qgis_plugin). The plugin includes the main GUI application called EIS
-Wizard and all individual EIS Toolkit tools as QGIS processing algorithms. The
-plugin is developed by the same core team that develops EIS Toolkit. ### CLI
-EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line
-interface that serves as a common interface for integrating the toolkit with
-external applications, such as QGIS. However, it can be used directly too. To
-use the CLI, simply use the command ```console eis ``` or ```console eis --help
-``` to get started. However, please note that the CLI has been primarily
-designed to communicate with external programs and may feel clunky in direct
-use. ## Roadmap - Milestone 1: **Beta release 0.1** (November 2023). The
-toolkit should have the basic funtionalities required for a full MPM workflow.
-Official testing phase begins. The plugin will be still under active
-development. - Milestone 2: **Release 1.0** (April 2024). All features should
-be incorporated at this time and the toolkit useful for actual MPM work.
-Testing will continue, potential bugs will be fixed and the user experience
-refined. ## Contributing We welcome contributions to EIS Toolkit in various
-forms: - â¨ Developing new tools - ð Fixing bugs in the code - ð Bug and
-other reporting - ð¡ Feature suggestions To contribute with code or
-documentation, you'll need a local development environment and a copy of the
-repository. Please refer to the **For developers** section below for detailed
-setup instructions. If you're interested in bug reporting or making feature
-suggestions, you can familiarize yourself with the toolkit and test it as
-described in the **Usage** section. When you encounter bugs or have ideas for
-new features, you can create an issue in this repository. ### For developers
-All contributing developers need Git and a copy of the repository. ```console
-git clone https://github.com/GispoCoding/eis_toolkit.git ``` After this you
-have three options for setting up your local development environment. 1. Docker
-- [instructions](./instructions/dev_setup_with_docker.md) 2. Poetry -
-[instructions](./instructions/dev_setup_without_docker.md) 3. Conda -
-[instructions](./instructions/dev_setup_without_docker_with_conda.md) *For
-general contributing guidelines, see [CONTRIBUTING](./CONTRIBUTING.md).* ##
-License Licensed under the EUPL-1.2 or later.
+install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL needs to be
+installed separately on Windows when using pip / PyPI. If you have trouble
+installing EIS Toolkit in a venv due to GDAL, you can download a compatible
+GDAL wheel (for example from [this repository](https://github.com/cgohlke/
+geospatial-wheels/releases)), install it first, and then attempt to install EIS
+Toolkit again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter
+notebooks or via the CLI. At the moment, most tools have their own module and
+are imported like this: ```python # In general from eis_toolkit.category.module
+import module_function # Some examples from
+eis_toolkit.raster_processing.reprojecting import reproject_raster from
+eis_toolkit.exploratory_analyses.pca import compute_pca ``` You can find
+several Jupyter notebooks in this repostiory that demonstrate how tools of EIS
+Toolkit can be used. The documentation of EIS Toolkit can be read [here](https:
+//gispocoding.github.io/eis_toolkit/). ### EIS QGIS Plugin For those that
+prefer using tools of EIS Toolkit via a graphical user interface, check [EIS
+QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin
+includes the main GUI application called EIS Wizard and all individual EIS
+Toolkit tools as QGIS processing algorithms. The plugin is developed by the
+same core team that develops EIS Toolkit. ### CLI EIS Toolkit includes a
+[Typer](https://typer.tiangolo.com/) command-line interface that serves as a
+common interface for integrating the toolkit with external applications, such
+as QGIS. However, it can be used directly too. To use the CLI, simply use the
+command ```console eis ``` or ```console eis --help ``` to get started.
+However, please note that the CLI has been primarily designed to communicate
+with external programs and may feel clunky in direct use. ## Roadmap -
+Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the
+basic funtionalities required for a full MPM workflow. Official testing phase
+begins. The plugin will be still under active development. - Milestone 2:
+**Release 1.0** (April 2024). All features should be incorporated at this time
+and the toolkit useful for actual MPM work. Testing will continue, potential
+bugs will be fixed and the user experience refined. ## Contributing We welcome
+contributions to EIS Toolkit in various forms: - â¨ Developing new tools -
+ð Fixing bugs in the code - ð Bug and other reporting - ð¡ Feature
+suggestions To contribute with code or documentation, you'll need a local
+development environment and a copy of the repository. Please refer to the **For
+developers** section below for detailed setup instructions. If you're
+interested in bug reporting or making feature suggestions, you can familiarize
+yourself with the toolkit and test it as described in the **Usage** section.
+When you encounter bugs or have ideas for new features, you can create an issue
+in this repository. ### For developers All contributing developers need Git and
+a copy of the repository. ```console git clone https://github.com/GispoCoding/
+eis_toolkit.git ``` After this you have three options for setting up your local
+development environment. 1. Docker - [instructions](./instructions/
+dev_setup_with_docker.md) 2. Poetry - [instructions](./instructions/
+dev_setup_without_docker.md) 3. Conda - [instructions](./instructions/
+dev_setup_without_docker_with_conda.md) *For general contributing guidelines,
+see [CONTRIBUTING](./CONTRIBUTING.md).* ## License Licensed under the EUPL-1.2
+or later.
```

